# Comparing `tmp/py-avro-schema-2.1.3.tar.gz` & `tmp/py-avro-schema-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-avro-schema-2.1.3.tar", last modified: Mon Jun 26 13:25:58 2023, max compression
+gzip compressed data, was "py-avro-schema-2.2.0.tar", last modified: Thu Jun 29 11:18:40 2023, max compression
```

## Comparing `py-avro-schema-2.1.3.tar` & `py-avro-schema-2.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.143332 py-avro-schema-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.139332 py-avro-schema-2.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.139332 py-avro-schema-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-26 13:25:58.143332 py-avro-schema-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.139332 py-avro-schema-2.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/docs/py_avro_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:25:58.143332 py-avro-schema-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.139332 py-avro-schema-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.143332 py-avro-schema-2.1.3/src/py_avro_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/src/py_avro_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35266 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/src/py_avro_schema/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/src/py_avro_schema/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/src/py_avro_schema/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/src/py_avro_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.143332 py-avro-schema-2.1.3/src/py_avro_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-26 13:25:58.000000 py-avro-schema-2.1.3/src/py_avro_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 13:25:58.000000 py-avro-schema-2.1.3/src/py_avro_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:25:58.000000 py-avro-schema-2.1.3/src/py_avro_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 13:25:58.000000 py-avro-schema-2.1.3/src/py_avro_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 13:25:58.000000 py-avro-schema-2.1.3/src/py_avro_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:58.143332 py-avro-schema-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_logicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_plain_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-26 13:25:47.000000 py-avro-schema-2.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.325806 py-avro-schema-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.317806 py-avro-schema-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.321806 py-avro-schema-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-29 11:18:40.321806 py-avro-schema-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.321806 py-avro-schema-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/docs/py_avro_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:18:40.325806 py-avro-schema-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.317806 py-avro-schema-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.321806 py-avro-schema-2.2.0/src/py_avro_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/src/py_avro_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35406 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/src/py_avro_schema/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/src/py_avro_schema/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/src/py_avro_schema/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/src/py_avro_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.321806 py-avro-schema-2.2.0/src/py_avro_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-29 11:18:40.000000 py-avro-schema-2.2.0/src/py_avro_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-29 11:18:40.000000 py-avro-schema-2.2.0/src/py_avro_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:18:40.000000 py-avro-schema-2.2.0/src/py_avro_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 11:18:40.000000 py-avro-schema-2.2.0/src/py_avro_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 11:18:40.000000 py-avro-schema-2.2.0/src/py_avro_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:18:40.321806 py-avro-schema-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_logicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_plain_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-29 11:18:29.000000 py-avro-schema-2.2.0/tox.ini
```

### Comparing `py-avro-schema-2.1.3/.flake8` & `py-avro-schema-2.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/.github/workflows/release-package.yml` & `py-avro-schema-2.2.0/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/.github/workflows/test-package.yml` & `py-avro-schema-2.2.0/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/.gitignore` & `py-avro-schema-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/.pre-commit-config.yaml` & `py-avro-schema-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/LICENSE` & `py-avro-schema-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/LICENSE_HEADER.txt` & `py-avro-schema-2.2.0/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/PKG-INFO` & `py-avro-schema-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.1.3
+Version: 2.2.0
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.1.3/README.md` & `py-avro-schema-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/docs/conf.py` & `py-avro-schema-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/docs/index.rst` & `py-avro-schema-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/docs/tutorial.rst` & `py-avro-schema-2.2.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/docs/types.rst` & `py-avro-schema-2.2.0/docs/types.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/pyproject.toml` & `py-avro-schema-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/src/py_avro_schema/__init__.py` & `py-avro-schema-2.2.0/src/py_avro_schema/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,31 +23,32 @@
 """
 
 from typing import Optional, Type
 
 import memoization
 import orjson
 
-from py_avro_schema._schemas import JSON_OPTIONS, Option, schema
+from py_avro_schema._schemas import JSON_OPTIONS, Option, TypeNotSupportedError, schema
 from py_avro_schema._typing import DecimalType
 
 try:
     from importlib import metadata
 except ImportError:  # pragma: no cover
     # Python < 3.8
     import importlib_metadata as metadata  # type: ignore
 
 #: Library version, e.g. 1.0.0, taken from Git tags
 __version__ = metadata.version("py-avro-schema")
 
 
 __all__ = [
-    "generate",
     "DecimalType",
     "Option",
+    "TypeNotSupportedError",
+    "generate",
 ]
 
 
 @memoization.cached
 def generate(
     py_type: Type,
     *,
```

### Comparing `py-avro-schema-2.1.3/src/py_avro_schema/_schemas.py` & `py-avro-schema-2.2.0/src/py_avro_schema/_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 JSONObj = Dict[str, Any]
 JSONArray = List[Any]
 JSONType = Union[JSONStr, JSONObj, JSONArray]
 
 NamesType = List[str]
 
 
+class TypeNotSupportedError(TypeError):
+    """Error raised when a Avro schema cannot be generated for a given Python type"""
+
+
 class Option(enum.Flag):
     """
     Schema generation options
 
     Options can be passed in to the function :func:`py_avro_schema.generate`. Multiple values are specified like this::
 
        Option.INT_32 | Option.FLOAT_32
@@ -139,15 +143,15 @@
         lambda obj: inspect.isclass(obj) and issubclass(obj, Schema) and not inspect.isabstract(obj),
     )
     for _, schema_class in schema_classes:
         # Find the first schema class that handles py_type
         schema_obj = schema_class(py_type, namespace=namespace, options=options)  # type: ignore
         if schema_obj:
             return schema_obj
-    raise TypeError(f"Cannot generate Avro schema for Python type {py_type}")
+    raise TypeNotSupportedError(f"Cannot generate Avro schema for Python type {py_type}")
 
 
 class Schema(abc.ABC):
     """Schema base"""
 
     def __new__(cls, py_type: Type, namespace: Optional[str] = None, options: Option = Option(0)):
         """
```

### Comparing `py-avro-schema-2.1.3/src/py_avro_schema/_testing.py` & `py-avro-schema-2.2.0/src/py_avro_schema/_testing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/src/py_avro_schema/_typing.py` & `py-avro-schema-2.2.0/src/py_avro_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/src/py_avro_schema.egg-info/PKG-INFO` & `py-avro-schema-2.2.0/src/py_avro_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.1.3
+Version: 2.2.0
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.1.3/src/py_avro_schema.egg-info/SOURCES.txt` & `py-avro-schema-2.2.0/src/py_avro_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tests/test_avro_schema.py` & `py-avro-schema-2.2.0/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tests/test_dataclass.py` & `py-avro-schema-2.2.0/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tests/test_logicals.py` & `py-avro-schema-2.2.0/tests/test_logicals.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tests/test_plain_class.py` & `py-avro-schema-2.2.0/tests/test_plain_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import re
 
 import pytest
 
+import py_avro_schema
 from py_avro_schema._testing import assert_schema
 
 
 def test_plain_class_with_type_hints():
     class PyType:
         """A port, not using dataclass"""
 
@@ -62,14 +63,14 @@
         def __init__(self, name, *, country="NLD", latitude, longitude):  # note the non-default kwargs near the end!
             self.name = name
             self.country = country.upper()
             self.latitude = latitude
             self.longitude = longitude
 
     with pytest.raises(
-        TypeError,
+        py_avro_schema.TypeNotSupportedError,
         match=re.escape(
             "Cannot generate Avro schema for Python type <class 'test_plain_class.test_plain_class_no_type_hints."
             "<locals>.PyType'>"
         ),
     ):
         assert_schema(PyType, {})
```

### Comparing `py-avro-schema-2.1.3/tests/test_primitives.py` & `py-avro-schema-2.2.0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tests/test_pydantic.py` & `py-avro-schema-2.2.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tests/test_typing.py` & `py-avro-schema-2.2.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.3/tox.ini` & `py-avro-schema-2.2.0/tox.ini`

 * *Files identical despite different names*

