# Comparing `tmp/grammar_graph-0.1.8.tar.gz` & `tmp/grammar_graph-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grammar_graph-0.1.8.tar", last modified: Fri Aug 26 11:56:04 2022, max compression
+gzip compressed data, was "grammar_graph-0.1.9.tar", last modified: Fri Aug 26 12:49:59 2022, max compression
```

## Comparing `grammar_graph-0.1.8.tar` & `grammar_graph-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 11:56:04.392473 grammar_graph-0.1.8/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 grammar_graph-0.1.8/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    42217 2022-08-26 11:56:04.392909 grammar_graph-0.1.8/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      910 2022-01-10 14:25:23.000000 grammar_graph-0.1.8/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      765 2022-08-26 11:55:25.000000 grammar_graph-0.1.8/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      956 2022-08-26 11:56:04.393521 grammar_graph-0.1.8/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 grammar_graph-0.1.8/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 11:56:04.388662 grammar_graph-0.1.8/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 11:56:04.390590 grammar_graph-0.1.8/src/grammar_graph/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       22 2022-08-26 11:55:19.000000 grammar_graph-0.1.8/src/grammar_graph/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    25255 2022-08-26 11:54:59.000000 grammar_graph-0.1.8/src/grammar_graph/gg.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 11:56:04.392260 grammar_graph-0.1.8/src/grammar_graph.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    42217 2022-08-26 11:56:04.000000 grammar_graph-0.1.8/src/grammar_graph.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      309 2022-08-26 11:56:04.000000 grammar_graph-0.1.8/src/grammar_graph.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2022-08-26 11:56:04.000000 grammar_graph-0.1.8/src/grammar_graph.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      125 2022-08-26 11:56:04.000000 grammar_graph-0.1.8/src/grammar_graph.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       14 2022-08-26 11:56:04.000000 grammar_graph-0.1.8/src/grammar_graph.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 12:49:59.918434 grammar_graph-0.1.9/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35149 2021-03-30 13:41:15.000000 grammar_graph-0.1.9/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    42217 2022-08-26 12:49:59.918769 grammar_graph-0.1.9/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      910 2022-01-10 14:25:23.000000 grammar_graph-0.1.9/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      765 2022-08-26 12:49:06.000000 grammar_graph-0.1.9/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      956 2022-08-26 12:49:59.919233 grammar_graph-0.1.9/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:29:50.000000 grammar_graph-0.1.9/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 12:49:59.914060 grammar_graph-0.1.9/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 12:49:59.915981 grammar_graph-0.1.9/src/grammar_graph/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       22 2022-08-26 12:49:02.000000 grammar_graph-0.1.9/src/grammar_graph/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    25753 2022-08-26 12:48:47.000000 grammar_graph-0.1.9/src/grammar_graph/gg.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-26 12:49:59.918027 grammar_graph-0.1.9/src/grammar_graph.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    42217 2022-08-26 12:49:59.000000 grammar_graph-0.1.9/src/grammar_graph.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      309 2022-08-26 12:49:59.000000 grammar_graph-0.1.9/src/grammar_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2022-08-26 12:49:59.000000 grammar_graph-0.1.9/src/grammar_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      125 2022-08-26 12:49:59.000000 grammar_graph-0.1.9/src/grammar_graph.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       14 2022-08-26 12:49:59.000000 grammar_graph-0.1.9/src/grammar_graph.egg-info/top_level.txt
```

### Comparing `grammar_graph-0.1.8/LICENSE` & `grammar_graph-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grammar_graph-0.1.8/PKG-INFO` & `grammar_graph-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grammar_graph
-Version: 0.1.8
+Version: 0.1.9
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/GrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `grammar_graph-0.1.8/README.md` & `grammar_graph-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `grammar_graph-0.1.8/pyproject.toml` & `grammar_graph-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grammar_graph"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "Graphs from Context-Free Grammars."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `grammar_graph-0.1.8/setup.cfg` & `grammar_graph-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `grammar_graph-0.1.8/src/grammar_graph/gg.py` & `grammar_graph-0.1.9/src/grammar_graph/gg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import html
 import json
 import re
 import sys
 from abc import abstractmethod
 from functools import lru_cache
 from typing import List, Dict, Callable, Union, Optional, Tuple, cast, Set, Protocol, Generator, Iterator
@@ -535,30 +536,39 @@
         :return: The k-paths in the given tree.
         """
         assert k > 0
         orig_k = k
         k += k - 1  # Each path of k terminal/nonterminal nodes includes k-1 choice nodes
 
         # For open trees: Extend all paths ending with None with the possible k-paths for the last nonterminal.
-        all_paths = self.graph_paths_from_tree(tree, include_terminals=include_terminals)
+        all_paths = self.graph_paths_from_tree(tree, include_terminals=True)
+
+        @functools.lru_cache
+        def remove_terminals(path: Tuple[Node, ...]) -> Tuple[Node, ...]:
+            if include_terminals or not isinstance(path[-1], TerminalNode):
+                return path
+            else:
+                return path[:-2]
 
         concrete_k_paths: List[Tuple[Node, ...]] = [
             kpath
             for path in all_paths
             for kpath in [
-                path[i:i + k]
-                for i in range(0, len(path) - k + 1, 1)
-                if path[i + k - 1] is not None]
+                remove_terminals(path)[i:i + k]
+                for i in range(0, len(remove_terminals(path)) - k + 1, 1)
+                if remove_terminals(path)[i + k - 1] is not None]
             if (len(kpath) == k and
                 not isinstance(kpath[0], ChoiceNode) and
                 not isinstance(kpath[-1], ChoiceNode))
         ]
 
         assert all(p[-1] is not None for p in concrete_k_paths)
-        assert all(any(p[-1] == kpath[-1] for kpath in concrete_k_paths) for p in all_paths if p[-1] and len(p) >= k)
+        assert all(
+            any(remove_terminals(p)[-1] == kpath[-1] for kpath in concrete_k_paths)
+            for p in all_paths if len(remove_terminals(p)) >= k)
 
         if not include_potential_paths:
             return set(concrete_k_paths)
 
         # For open trees: Extend all paths ending with None with the possible k-paths for the last nonterminal.
         potential_k_paths: List[Tuple[Node, ...]] = []
 
@@ -568,15 +578,18 @@
             nonterminal_kpaths = self.nonterminal_kpaths(
                 cast(NonterminalNode, prefix[-1]), orig_k, up_to=True, include_terminals=include_terminals)
             potential_k_paths.extend([p for p in nonterminal_kpaths if len(p) == k])
             for postfix in [p for p in nonterminal_kpaths if p[0] == prefix[-1]]:
                 path = prefix[:-1] + postfix
                 potential_k_paths.extend([path[i:i + k] for i in range(0, len(path) - k + 1, 2)])
 
-        potential_k_paths_set = set(potential_k_paths)
+        potential_k_paths_set = {
+            path if include_terminals or not isinstance(path[-1], TerminalNode)
+            else path[:-2]
+            for path in potential_k_paths}
         assert not potential_k_paths_set or potential_k_paths_set.intersection(self.k_paths(orig_k))
 
         return set(concrete_k_paths) | potential_k_paths_set
 
     @lru_cache(maxsize=None)
     def k_paths(
             self,
@@ -694,8 +707,8 @@
 
 
 def path_to_string(p, include_choice_node=True) -> str:
     return " ".join([
         f'"{n.symbol}" ({n.id})' if isinstance(n, TerminalNode)
         else n.symbol
         for n in p
-        if include_choice_node or not isinstance(n, ChoiceNode)])
+        if include_choice_node or not isinstance(n, ChoiceNode)])
```

### Comparing `grammar_graph-0.1.8/src/grammar_graph.egg-info/PKG-INFO` & `grammar_graph-0.1.9/src/grammar_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grammar-graph
-Version: 0.1.8
+Version: 0.1.9
 Summary: Graphs from Context-Free Grammars.
 Home-page: https://github.com/rindPHI/GrammarGraph
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

