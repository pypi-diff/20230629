# Comparing `tmp/rdfdf-0.1.3.tar.gz` & `tmp/rdfdf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfdf-0.1.3.tar", max compression
+gzip compressed data, was "rdfdf-0.1.4.tar", max compression
```

## Comparing `rdfdf-0.1.3.tar` & `rdfdf-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.3/LICENSE
--rw-r--r--   0        0        0     8588 2023-05-24 07:20:23.215813 rdfdf-0.1.3/README.md
--rw-r--r--   0        0        0      459 2023-06-26 11:14:43.822886 rdfdf-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.3/rdfdf/__init__.py
--rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.3/rdfdf/examples/example_1.py
--rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.3/rdfdf/examples/example_2.py
--rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.3/rdfdf/examples/example_3.py
--rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.3/rdfdf/examples/example_4.py
--rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.3/rdfdf/helpers/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.3/rdfdf/helpers/importers.py
--rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.3/rdfdf/helpers/rdfdf_utils.py
--rw-r--r--   0        0        0     4004 2023-06-26 11:12:28.432496 rdfdf-0.1.3/rdfdf/rdfdf.py
--rw-r--r--   0        0        0     9145 1970-01-01 00:00:00.000000 rdfdf-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.4/LICENSE
+-rw-r--r--   0        0        0     8588 2023-05-24 07:20:23.215813 rdfdf-0.1.4/README.md
+-rw-r--r--   0        0        0      459 2023-06-29 06:44:12.207413 rdfdf-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.4/rdfdf/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_1.py
+-rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_2.py
+-rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_3.py
+-rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.4/rdfdf/examples/example_4.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.4/rdfdf/helpers/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.4/rdfdf/helpers/importers.py
+-rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.4/rdfdf/helpers/rdfdf_utils.py
+-rw-r--r--   0        0        0     4087 2023-06-29 06:34:43.690379 rdfdf-0.1.4/rdfdf/rdfdf.py
+-rw-r--r--   0        0        0     9145 1970-01-01 00:00:00.000000 rdfdf-0.1.4/PKG-INFO
```

### Comparing `rdfdf-0.1.3/LICENSE` & `rdfdf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/README.md` & `rdfdf-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/examples/example_1.py` & `rdfdf-0.1.4/rdfdf/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/examples/example_2.py` & `rdfdf-0.1.4/rdfdf/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/examples/example_3.py` & `rdfdf-0.1.4/rdfdf/examples/example_3.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/examples/example_4.py` & `rdfdf-0.1.4/rdfdf/examples/example_4.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/helpers/importers.py` & `rdfdf-0.1.4/rdfdf/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/helpers/rdfdf_utils.py` & `rdfdf-0.1.4/rdfdf/helpers/rdfdf_utils.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.3/rdfdf/rdfdf.py` & `rdfdf-0.1.4/rdfdf/rdfdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
                  column_rules: Mapping[str, Callable[[], Graph | None]],
                  graph: Graph = None):
 
         self._df = dataframe
         self._subject_column = subject_column
         self._subject_rule = subject_rule
         self._column_rules = column_rules
-        self._graph = graph or Graph()
+        # bug fix: this allows also empty but namespaced graphs
+        self._graph = Graph() if graph is None else graph
 
     def _apply_subject_rule(self, row: pd.Series) -> URIRef:
         """Applies subject_rule to the subject_column of a pd.Series row;
         conveniently allows to also pass an rdflib.Namespace (or generally Sequence types) as subject_rule.
         """
 
         try:
```

### Comparing `rdfdf-0.1.3/PKG-INFO` & `rdfdf-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfdf
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: GPL3
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

