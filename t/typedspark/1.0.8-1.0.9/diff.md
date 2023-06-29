# Comparing `tmp/typedspark-1.0.8.tar.gz` & `tmp/typedspark-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedspark-1.0.8.tar", last modified: Wed Jun 28 07:03:12 2023, max compression
+gzip compressed data, was "typedspark-1.0.9.tar", last modified: Wed Jun 28 08:43:00 2023, max compression
```

## Comparing `typedspark-1.0.8.tar` & `typedspark-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.566999 typedspark-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 07:02:54.000000 typedspark-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-28 07:03:12.566999 typedspark-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-28 07:02:54.000000 typedspark-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-28 07:02:54.000000 typedspark-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 07:03:12.566999 typedspark-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-28 07:02:54.000000 typedspark-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.562999 typedspark-1.0.8/typedspark/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.566999 typedspark-1.0.8/typedspark/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_core/column_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_core/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_core/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.566999 typedspark-1.0.8/typedspark/_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_schema/dlt_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_schema/get_schema_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_schema/get_schema_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_schema/structfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.566999 typedspark-1.0.8/typedspark/_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_transforms/structtype_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_transforms/transform_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.566999 typedspark-1.0.8/typedspark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_utils/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_utils/load_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/_utils/register_schema_to_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 07:02:54.000000 typedspark-1.0.8/typedspark/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 07:03:12.562999 typedspark-1.0.8/typedspark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-28 07:03:12.000000 typedspark-1.0.8/typedspark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 07:03:12.000000 typedspark-1.0.8/typedspark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 07:03:12.000000 typedspark-1.0.8/typedspark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-28 07:03:12.000000 typedspark-1.0.8/typedspark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 07:03:12.000000 typedspark-1.0.8/typedspark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 08:42:47.000000 typedspark-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-28 08:43:00.592497 typedspark-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-28 08:42:47.000000 typedspark-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-28 08:42:47.000000 typedspark-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 08:43:00.592497 typedspark-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-28 08:42:47.000000 typedspark-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/typedspark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/typedspark/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_core/column_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_core/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_core/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/typedspark/_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_schema/dlt_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_schema/get_schema_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_schema/get_schema_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_schema/structfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/typedspark/_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_transforms/structtype_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_transforms/transform_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/typedspark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_utils/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_utils/load_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/_utils/register_schema_to_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:42:47.000000 typedspark-1.0.9/typedspark/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:43:00.592497 typedspark-1.0.9/typedspark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-28 08:43:00.000000 typedspark-1.0.9/typedspark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-28 08:43:00.000000 typedspark-1.0.9/typedspark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 08:43:00.000000 typedspark-1.0.9/typedspark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-28 08:43:00.000000 typedspark-1.0.9/typedspark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 08:43:00.000000 typedspark-1.0.9/typedspark.egg-info/top_level.txt
```

### Comparing `typedspark-1.0.8/LICENSE.txt` & `typedspark-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/PKG-INFO` & `typedspark-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.8
+Version: 1.0.9
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.8/README.rst` & `typedspark-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/pyproject.toml` & `typedspark-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/setup.py` & `typedspark-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/__init__.py` & `typedspark-1.0.9/typedspark/__init__.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_core/column.py` & `typedspark-1.0.9/typedspark/_core/column.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             a: Column[IntegerType]
             b: Column[StringType]
     """
 
     def __new__(
         cls,
         name: str,
-        dtype: T,
+        dtype: T = DataType,  # type: ignore
         parent: Union[DataFrame, "Column", None] = None,
         curid: Optional[int] = None,
     ):
         """``__new__()`` instantiates the object (prior to ``__init__()``).
 
         Here, we simply take the provided ``name``, create a pyspark
         ``Column`` object and cast it to a typedspark ``Column`` object.
@@ -56,15 +56,15 @@
 
         column.__class__ = Column
         return column
 
     def __init__(
         self,
         name: str,
-        dtype: T,
+        dtype: T = DataType,  # type: ignore
         parent: Union[DataFrame, "Column", None] = None,
         curid: Optional[int] = None,
     ):
         # pylint: disable=unused-argument
         self.str = name
         self._dtype = dtype
         self._curid = curid
```

### Comparing `typedspark-1.0.8/typedspark/_core/column_meta.py` & `typedspark-1.0.9/typedspark/_core/column_meta.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_core/dataset.py` & `typedspark-1.0.9/typedspark/_core/dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_core/datatypes.py` & `typedspark-1.0.9/typedspark/_core/datatypes.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_core/validate_schema.py` & `typedspark-1.0.9/typedspark/_core/validate_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_schema/get_schema_definition.py` & `typedspark-1.0.9/typedspark/_schema/get_schema_definition.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_schema/get_schema_imports.py` & `typedspark-1.0.9/typedspark/_schema/get_schema_imports.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_schema/schema.py` & `typedspark-1.0.9/typedspark/_schema/schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_schema/structfield.py` & `typedspark-1.0.9/typedspark/_schema/structfield.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_transforms/structtype_column.py` & `typedspark-1.0.9/typedspark/_transforms/structtype_column.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_transforms/transform_to_schema.py` & `typedspark-1.0.9/typedspark/_transforms/transform_to_schema.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_transforms/utils.py` & `typedspark-1.0.9/typedspark/_transforms/utils.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_utils/create_dataset.py` & `typedspark-1.0.9/typedspark/_utils/create_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_utils/load_table.py` & `typedspark-1.0.9/typedspark/_utils/load_table.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark/_utils/register_schema_to_dataset.py` & `typedspark-1.0.9/typedspark/_utils/register_schema_to_dataset.py`

 * *Files identical despite different names*

### Comparing `typedspark-1.0.8/typedspark.egg-info/PKG-INFO` & `typedspark-1.0.9/typedspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedspark
-Version: 1.0.8
+Version: 1.0.9
 Summary: Column-wise type annotations for pyspark DataFrames
 Home-page: https://github.com/kaiko-ai/typedspark
 Author: Nanne Aben
 Author-email: nanne@kaiko.ai
 License: Apache-2.0
 Keywords: pyspark spark typing type checking annotations
 Classifier: Programming Language :: Python
```

### Comparing `typedspark-1.0.8/typedspark.egg-info/SOURCES.txt` & `typedspark-1.0.9/typedspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

