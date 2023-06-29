# Comparing `tmp/hypernetx-2.0.1.tar.gz` & `tmp/hypernetx-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypernetx-2.0.1.tar", last modified: Tue Jun 27 23:47:28 2023, max compression
+gzip compressed data, was "hypernetx-2.0.2.tar", last modified: Thu Jun 29 16:08:54 2023, max compression
```

## Comparing `hypernetx-2.0.1.tar` & `hypernetx-2.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.287028 hypernetx-2.0.1/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1794 2023-05-15 23:30:43.000000 hypernetx-2.0.1/LICENSE.rst
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3239 2023-05-15 23:30:43.000000 hypernetx-2.0.1/LONG_DESCRIPTION.rst
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3828 2023-06-27 23:47:28.287215 hypernetx-2.0.1/PKG-INFO
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    13839 2023-06-23 18:39:50.000000 hypernetx-2.0.1/README.md
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:27.928032 hypernetx-2.0.1/hypernetx/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      394 2023-06-23 18:39:50.000000 hypernetx-2.0.1/hypernetx/__init__.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.028367 hypernetx-2.0.1/hypernetx/algorithms/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2596 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/algorithms/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    40009 2023-06-23 18:39:50.000000 hypernetx-2.0.1/hypernetx/algorithms/contagion.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     8678 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/algorithms/generative_models.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    24275 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/algorithms/homology_mod2.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    15474 2023-06-23 18:39:50.000000 hypernetx-2.0.1/hypernetx/algorithms/hypergraph_modularity.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     7820 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/algorithms/laplacians_clustering.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     9966 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/algorithms/s_centrality_measures.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.110655 hypernetx-2.0.1/hypernetx/classes/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      195 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/classes/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    55664 2023-06-27 21:38:45.000000 hypernetx-2.0.1/hypernetx/classes/entity.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    27383 2023-06-27 21:38:45.000000 hypernetx-2.0.1/hypernetx/classes/entityset.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     8557 2023-06-09 21:15:31.000000 hypernetx-2.0.1/hypernetx/classes/helpers.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    82331 2023-06-27 21:38:45.000000 hypernetx-2.0.1/hypernetx/classes/hypergraph.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.157967 hypernetx-2.0.1/hypernetx/drawing/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      151 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/drawing/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    15120 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/drawing/rubber_band.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     5596 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/drawing/two_column.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3398 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/drawing/util.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      640 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/exception.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      379 2022-07-07 16:12:57.000000 hypernetx-2.0.1/hypernetx/read_write.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.170890 hypernetx-2.0.1/hypernetx/reports/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      491 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/reports/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    11362 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/reports/descriptive_stats.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.236371 hypernetx-2.0.1/hypernetx/utils/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      760 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/utils/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2428 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/utils/decorators.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     5960 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/utils/extras.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1423 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/utils/log.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:28.286315 hypernetx-2.0.1/hypernetx/utils/toys/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      409 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/utils/toys/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      353 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/utils/toys/gene_data.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2844 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/utils/toys/harrypotter.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    14357 2023-05-15 23:30:43.000000 hypernetx-2.0.1/hypernetx/utils/toys/lesmis.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      552 2023-05-11 23:28:49.000000 hypernetx-2.0.1/hypernetx/utils/toys/transmission_problem.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-06-27 23:47:27.959199 hypernetx-2.0.1/hypernetx.egg-info/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3828 2023-06-27 23:47:27.000000 hypernetx-2.0.1/hypernetx.egg-info/PKG-INFO
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1220 2023-06-27 23:47:27.000000 hypernetx-2.0.1/hypernetx.egg-info/SOURCES.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)        1 2023-06-27 23:47:27.000000 hypernetx-2.0.1/hypernetx.egg-info/dependency_links.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1062 2023-06-27 23:47:27.000000 hypernetx-2.0.1/hypernetx.egg-info/requires.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       10 2023-06-27 23:47:27.000000 hypernetx-2.0.1/hypernetx.egg-info/top_level.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       97 2023-05-11 23:28:49.000000 hypernetx-2.0.1/pyproject.toml
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2364 2023-06-27 23:47:28.308361 hypernetx-2.0.1/setup.cfg
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       80 2023-06-23 18:39:50.000000 hypernetx-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.379040 hypernetx-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-29 16:08:45.000000 hypernetx-2.0.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-29 16:08:45.000000 hypernetx-2.0.2/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-29 16:08:54.379040 hypernetx-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-06-29 16:08:45.000000 hypernetx-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.371040 hypernetx-2.0.2/hypernetx/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.371040 hypernetx-2.0.2/hypernetx/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40009 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/contagion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/generative_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/homology_mod2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/hypergraph_modularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/laplacians_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/s_centrality_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55664 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27383 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/entityset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82331 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/hypergraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/rubber_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/two_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/read_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/reports/descriptive_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.379040 hypernetx-2.0.2/hypernetx/utils/toys/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/gene_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/harrypotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/lesmis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/transmission_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.371040 hypernetx-2.0.2/hypernetx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 16:08:45.000000 hypernetx-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-29 16:08:54.379040 hypernetx-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 16:08:45.000000 hypernetx-2.0.2/setup.py
```

### Comparing `hypernetx-2.0.1/LICENSE.rst` & `hypernetx-2.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/LONG_DESCRIPTION.rst` & `hypernetx-2.0.2/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/PKG-INFO` & `hypernetx-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypernetx
-Version: 2.0.1
+Version: 2.0.2
 Summary: HyperNetX is a Python library for the creation and study of hypergraphs.
 Home-page: https://github.com/pnnl/HyperNetX
 Author: Brenda Praggastis, Dustin Arendt, Sinan Aksoy, Emilie Purvine, Cliff Joslyn
 Author-email: hypernetx@pnnl.gov
 License: 3-Clause BSD license
 Description-Content-Type: text/x-rst
 Provides-Extra: releases
```

### Comparing `hypernetx-2.0.1/README.md` & `hypernetx-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/__init__.py` & `hypernetx-2.0.2/hypernetx/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/contagion.py` & `hypernetx-2.0.2/hypernetx/algorithms/contagion.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/generative_models.py` & `hypernetx-2.0.2/hypernetx/algorithms/generative_models.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/homology_mod2.py` & `hypernetx-2.0.2/hypernetx/algorithms/homology_mod2.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/hypergraph_modularity.py` & `hypernetx-2.0.2/hypernetx/algorithms/hypergraph_modularity.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/laplacians_clustering.py` & `hypernetx-2.0.2/hypernetx/algorithms/laplacians_clustering.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/algorithms/s_centrality_measures.py` & `hypernetx-2.0.2/hypernetx/algorithms/s_centrality_measures.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/classes/entity.py` & `hypernetx-2.0.2/hypernetx/classes/entity.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/classes/entityset.py` & `hypernetx-2.0.2/hypernetx/classes/entityset.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/classes/helpers.py` & `hypernetx-2.0.2/hypernetx/classes/helpers.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/classes/hypergraph.py` & `hypernetx-2.0.2/hypernetx/classes/hypergraph.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/drawing/rubber_band.py` & `hypernetx-2.0.2/hypernetx/drawing/rubber_band.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/drawing/two_column.py` & `hypernetx-2.0.2/hypernetx/drawing/two_column.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/drawing/util.py` & `hypernetx-2.0.2/hypernetx/drawing/util.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/exception.py` & `hypernetx-2.0.2/hypernetx/exception.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/reports/descriptive_stats.py` & `hypernetx-2.0.2/hypernetx/reports/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/__init__.py` & `hypernetx-2.0.2/hypernetx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/decorators.py` & `hypernetx-2.0.2/hypernetx/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/extras.py` & `hypernetx-2.0.2/hypernetx/utils/extras.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/log.py` & `hypernetx-2.0.2/hypernetx/utils/log.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/toys/harrypotter.py` & `hypernetx-2.0.2/hypernetx/utils/toys/harrypotter.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/toys/lesmis.py` & `hypernetx-2.0.2/hypernetx/utils/toys/lesmis.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx/utils/toys/transmission_problem.py` & `hypernetx-2.0.2/hypernetx/utils/toys/transmission_problem.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx.egg-info/PKG-INFO` & `hypernetx-2.0.2/hypernetx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypernetx
-Version: 2.0.1
+Version: 2.0.2
 Summary: HyperNetX is a Python library for the creation and study of hypergraphs.
 Home-page: https://github.com/pnnl/HyperNetX
 Author: Brenda Praggastis, Dustin Arendt, Sinan Aksoy, Emilie Purvine, Cliff Joslyn
 Author-email: hypernetx@pnnl.gov
 License: 3-Clause BSD license
 Description-Content-Type: text/x-rst
 Provides-Extra: releases
```

### Comparing `hypernetx-2.0.1/hypernetx.egg-info/SOURCES.txt` & `hypernetx-2.0.2/hypernetx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/hypernetx.egg-info/requires.txt` & `hypernetx-2.0.2/hypernetx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.1/setup.cfg` & `hypernetx-2.0.2/setup.cfg`

 * *Files identical despite different names*

