# Comparing `tmp/fhir_analyzer-0.0.4.tar.gz` & `tmp/fhir_analyzer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_analyzer-0.0.4.tar", last modified: Thu Jun 29 19:28:14 2023, max compression
+gzip compressed data, was "fhir_analyzer-0.0.5.tar", last modified: Thu Jun 29 20:12:50 2023, max compression
```

## Comparing `fhir_analyzer-0.0.4.tar` & `fhir_analyzer-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.256913 fhir_analyzer-0.0.4/
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.4/LICENSE
--rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 19:28:14.256722 fhir_analyzer-0.0.4/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.4/README.md
--rw-r--r--   0 tillrostalski   (501) staff       (20)      772 2023-06-29 19:28:04.000000 fhir_analyzer-0.0.4/pyproject.toml
--rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 19:28:14.256951 fhir_analyzer-0.0.4/setup.cfg
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.252663 fhir_analyzer-0.0.4/src/
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.254662 fhir_analyzer-0.0.4/src/fhir_analyzer/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/constants.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4975 2023-06-25 13:42:39.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/feature_selector.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/fhirstore.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/helper.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.256176 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)    13134 2023-06-29 16:04:46.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/comparator.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2391 2023-06-25 17:02:32.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/internal_types.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     9003 2023-06-25 20:17:45.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/patsim.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2603 2023-06-25 19:58:12.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/tmp.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.255403 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/
--rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)      621 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       82 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/requires.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.363669 fhir_analyzer-0.0.5/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.5/LICENSE
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 20:12:50.363498 fhir_analyzer-0.0.5/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.5/README.md
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      782 2023-06-29 20:12:40.000000 fhir_analyzer-0.0.5/pyproject.toml
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 20:12:50.363711 fhir_analyzer-0.0.5/setup.cfg
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.358518 fhir_analyzer-0.0.5/src/
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.361236 fhir_analyzer-0.0.5/src/fhir_analyzer/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/constants.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     5021 2023-06-29 20:08:59.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/feature_selector.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/fhirstore.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/helper.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.363160 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)    13134 2023-06-29 20:01:02.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/comparator.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2389 2023-06-29 20:09:09.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/internal_types.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     9244 2023-06-29 20:08:44.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/patsim.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2521 2023-06-29 20:10:42.000000 fhir_analyzer-0.0.5/src/fhir_analyzer/tmp.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 20:12:50.362367 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      621 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       82 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/requires.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 20:12:50.000000 fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/top_level.txt
```

### Comparing `fhir_analyzer-0.0.4/LICENSE` & `fhir_analyzer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.4/pyproject.toml` & `fhir_analyzer-0.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fhir_analyzer"
-version = "0.0.4"
-authors = [
-  { name="Till Rostalski", email="tillrostalski@gmail.com" },
-]
+version = "0.0.5"
+authors = [{ name = "Till Rostalski", email = "tillrostalski@gmail.com" }]
 description = "A small FHIR package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+dependencies = [
+  "fhir.resources",
+  "pydantic",
+  "pandas",
+  "fhirpathpy",
+  "networkx",
+  "nxontology",
 ]
-dependencies=["fhir.resources", "pydantic", "pandas", "fhirpathpy", "networkx", "nxontology"]
 
 [project.optional-dependencies]
 dev = ["pytest", "twine"]
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/constants.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/feature_selector.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable
+from typing import Any, Callable, Union
 
 from fhirpathpy import compile
 import pandas as pd
 
 from fhir_analyzer.fhirstore import Fhirstore
 
 
@@ -89,17 +89,19 @@
                     for resource in patient_resources[resource_type]:
                         target = self._get_target(resource, target_fns, conditional_fns)
                         self._update_patient_features(patient_id, feature_name, target)
 
     def _get_target(
         self,
         resource: Any,
-        target_fns: list[Callable[[Any], Any]] | dict[str, Callable[[Any], Any]],
-        conditional_fns: list[tuple[Callable[[Any], bool], Callable[[Any], Any]]]
-        | dict[str, tuple[Callable[[Any], bool], Callable[[Any], Any]]],
+        target_fns: Union[list[Callable[[Any], Any]], dict[str, Callable[[Any], Any]]],
+        conditional_fns: Union[
+            list[tuple[Callable[[Any], bool], Callable[[Any], Any]]],
+            dict[str, tuple[Callable[[Any], bool], Callable[[Any], Any]]],
+        ],
     ):
         target = {}
         if conditional_fns:
             for targ_n, cond_fns in conditional_fns.items():
                 temp_target = self._evaluate_conditional_functions(resource, cond_fns)
                 if temp_target:
                     target[targ_n] = temp_target
```

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/fhirstore.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/fhirstore.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/helper.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/helper.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/comparator.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/comparator.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/internal_types.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/internal_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from dataclasses import dataclass
+from typing import Union
+
 
 CODED_CONCEPT = "coded_concept"
 CATEGORICAL_STRING = "categorical_string"
 NUMERICAL = "numerical"
 CODED_NUMERICAL = "coded_numerical"
 
 
@@ -51,15 +52,15 @@
     def __init__(
         self,
         value: float,
         code: str,
         code_mean: float,
         code_std_dev: float,
         feature_name: str,
-        is_abnormal: bool | None = None,
+        is_abnormal: Union[bool, None] = None,
     ):
         if not isinstance(value, float):
             raise ValueError(
                 f"Feature value for {feature_name} expected float, got {type(value)}: {value}"
             )
         if not isinstance(code, str):
             raise ValueError(
```

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/patsim.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/patient_similarity/patsim.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from fhir_analyzer.feature_selector import FeatureSelector
 
 from fhir_analyzer.fhirstore import Fhirstore
 from fhir_analyzer.constants import (
     default_target_paths,
     default_system_paths,
     default_code_paths,
@@ -63,17 +64,19 @@
             self.add_numerical_feature(*args, **kwargs)
         else:
             raise ValueError(f"Invalid feature type: {type}")
 
     def add_categorical_feature(
         self,
         name: str,
-        resource_types: list[str] | str,
-        target_paths: list[str] | str | None = None,
-        conditional_target_paths: list[dict[str, str]] | dict[str, str] | None = None,
+        resource_types: Union[list[str], str],
+        target_paths: Union[list[str], str, None] = None,
+        conditional_target_paths: Union[
+            list[dict[str, str]], dict[str, str], None
+        ] = None,
     ):
         if isinstance(resource_types, str):
             resource_types = [resource_types]
         if isinstance(target_paths, str):
             target_paths = [target_paths]
         validate_paths(
             paths=target_paths,
@@ -95,17 +98,19 @@
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
         )
 
     def add_numerical_feature(
         self,
         name: str,
-        resource_types: list[str] | str,
-        target_paths: list[str] | str | None = None,
-        conditional_target_paths: list[dict[str, str]] | dict[str, str] | None = None,
+        resource_types: Union[list[str], str],
+        target_paths: Union[list[str], str, None] = None,
+        conditional_target_paths: Union[
+            list[dict[str, str]], dict[str, str], None
+        ] = None,
     ):
         if isinstance(resource_types, str):
             resource_types = [resource_types]
         if isinstance(target_paths, str):
             target_paths = [target_paths]
         validate_paths(
             paths=target_paths,
@@ -125,19 +130,23 @@
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
         )
 
     def add_coded_concept_feature(
         self,
         name: str,
-        resource_types: list[str] | str,
-        code_paths: list[str] | str | None = None,
-        system_paths: list[str] | str | None = None,
-        conditional_code_paths: list[dict[str, str]] | dict[str, str] | None = None,
-        conditional_system_paths: list[dict[str, str]] | dict[str, str] | None = None,
+        resource_types: Union[list[str], str],
+        code_paths: Union[list[str], str, None] = None,
+        system_paths: Union[list[str], str, None] = None,
+        conditional_code_paths: Union[
+            list[dict[str, str]], dict[str, str], None
+        ] = None,
+        conditional_system_paths: Union[
+            list[dict[str, str]], dict[str, str], None
+        ] = None,
     ):
         if isinstance(resource_types, str):
             resource_types = [resource_types]
         if isinstance(code_paths, str):
             code_paths = [code_paths]
         if isinstance(system_paths, str):
             system_paths = [system_paths]
@@ -180,19 +189,23 @@
             target_paths=target_paths,
             conditional_target_paths=conditional_target_paths,
         )
 
     def add_coded_numerical_feature(
         self,
         name: str,
-        resource_types: list[str] | str,
-        value_paths: list[str] | str | None = None,
-        code_paths: list[str] | str | None = None,
-        conditional_value_paths: list[dict[str, str]] | dict[str, str] | None = None,
-        conditional_code_paths: list[dict[str, str]] | dict[str, str] | None = None,
+        resource_types: Union[list[str], str],
+        value_paths: Union[list[str], str, None] = None,
+        code_paths: Union[list[str], str, None] = None,
+        conditional_value_paths: Union[
+            list[dict[str, str]], dict[str, str], None
+        ] = None,
+        conditional_code_paths: Union[
+            list[dict[str, str]], dict[str, str], None
+        ] = None,
     ):
         if isinstance(resource_types, str):
             resource_types = [resource_types]
         if isinstance(code_paths, str):
             code_paths = [code_paths]
         if isinstance(value_paths, str):
             value_paths = [value_paths]
```

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer/tmp.py` & `fhir_analyzer-0.0.5/src/fhir_analyzer/tmp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from fhir_analyzer.patient_similarity.patsim import Patsim
 import json
+import os
+print(os.getcwd())
 
 ex = {
     "resourceType": "Observation",
     "id": "f9c5653f-a8c8-4c07-89d9-e7e66dcce4c8",
     "status": "final",
     "category": [
         {
@@ -67,18 +69,15 @@
                 "code": "mm[Hg]",
             },
         },
     ],
 }
 
 patsim = Patsim()
-with open("data/bundles/test_bundle_001.json", "r") as f:
-    bundle = json.load(f)
-    patsim.add_bundle(bundle)
-with open("data/bundles/test_bundle_002.json", "r") as f:
+with open("../data/bundles/test_bundle_001.json", "r") as f:
     bundle = json.load(f)
     patsim.add_bundle(bundle)
 patsim.add_coded_concept_feature(
     name="Diagnoses",
     resource_types=["Condition"],
     code_paths=["code.coding.code"],
     system_paths=["code.coding.system"],
```

### Comparing `fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/SOURCES.txt` & `fhir_analyzer-0.0.5/src/fhir_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

