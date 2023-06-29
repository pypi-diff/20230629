# Comparing `tmp/fhir_analyzer-0.0.3.tar.gz` & `tmp/fhir_analyzer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_analyzer-0.0.3.tar", last modified: Thu Jun 29 15:03:37 2023, max compression
+gzip compressed data, was "fhir_analyzer-0.0.4.tar", last modified: Thu Jun 29 19:28:14 2023, max compression
```

## Comparing `fhir_analyzer-0.0.3.tar` & `fhir_analyzer-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.658871 fhir_analyzer-0.0.3/
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.3/LICENSE
--rw-r--r--   0 tillrostalski   (501) staff       (20)      457 2023-06-29 15:03:37.658726 fhir_analyzer-0.0.3/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.3/README.md
--rw-r--r--   0 tillrostalski   (501) staff       (20)      718 2023-06-29 15:03:28.000000 fhir_analyzer-0.0.3/pyproject.toml
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1387 2023-06-29 14:42:27.000000 fhir_analyzer-0.0.3/requirements.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 15:03:37.658913 fhir_analyzer-0.0.3/setup.cfg
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.654371 fhir_analyzer-0.0.3/src/
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.656728 fhir_analyzer-0.0.3/src/fhir_analyzer/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/constants.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4975 2023-06-25 13:42:39.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/feature_selector.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/fhirstore.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2164 2023-06-26 19:13:12.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/helper.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.658287 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)    13136 2023-06-25 20:13:44.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/comparator.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2391 2023-06-25 17:02:32.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/internal_types.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     9003 2023-06-25 20:17:45.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/patsim.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2603 2023-06-25 19:58:12.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/tmp.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.657383 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/
--rw-r--r--   0 tillrostalski   (501) staff       (20)      457 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)      638 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1387 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/requires.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.256913 fhir_analyzer-0.0.4/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.4/LICENSE
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 19:28:14.256722 fhir_analyzer-0.0.4/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.4/README.md
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      772 2023-06-29 19:28:04.000000 fhir_analyzer-0.0.4/pyproject.toml
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 19:28:14.256951 fhir_analyzer-0.0.4/setup.cfg
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.252663 fhir_analyzer-0.0.4/src/
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.254662 fhir_analyzer-0.0.4/src/fhir_analyzer/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/constants.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4975 2023-06-25 13:42:39.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/feature_selector.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/fhirstore.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2362 2023-06-29 16:04:29.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/helper.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.256176 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)    13134 2023-06-29 16:04:46.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/comparator.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2391 2023-06-25 17:02:32.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/internal_types.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     9003 2023-06-25 20:17:45.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/patsim.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2603 2023-06-25 19:58:12.000000 fhir_analyzer-0.0.4/src/fhir_analyzer/tmp.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 19:28:14.255403 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      477 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      621 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       82 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/requires.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 19:28:14.000000 fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/top_level.txt
```

### Comparing `fhir_analyzer-0.0.3/LICENSE` & `fhir_analyzer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/constants.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/feature_selector.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/feature_selector.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/fhirstore.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/fhirstore.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/helper.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from typing import Generator, Iterable
 from urllib.parse import urlparse
 from uuid import UUID
 from fhir.resources.reference import Reference
 
 from fhir_analyzer.constants import RESOURCE_LIST
 
@@ -61,7 +62,16 @@
     """Extracts the id from a uuid"""
     return uuid.split(":")[-1]
 
 
 def inputs_to_lists(*args):
     """Converts all inputs to lists"""
     return tuple([arg if isinstance(arg, list) else [arg] for arg in args])
+
+
+def cdf(x, mean, std):
+    # Compute the z-score
+    z = (x - mean) / std
+
+    # Compute the cumulative frequency score
+    cdf = 0.5 * (1 + math.erf(z / math.sqrt(2)))
+    return cdf
```

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/comparator.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/comparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import re
 import pkg_resources
 
 
 from nxontology import NXOntology
 import networkx as nx
 import pandas as pd
-from scipy.stats import norm
 
 from fhir_analyzer.feature_selector import FeatureSelector
+from fhir_analyzer.helper import cdf
 
 from fhir_analyzer.patient_similarity.internal_types import (
     CATEGORICAL_STRING,
     CODED_CONCEPT,
     CODED_NUMERICAL,
     NUMERICAL,
     CategoricalString,
@@ -150,16 +150,16 @@
 
             if std == 0:
                 return None
 
             value1 = float(feature1.value)
             value2 = float(feature2.value)
 
-            p1 = norm.cdf((value1 - mean) / std)
-            p2 = norm.cdf((value2 - mean) / std)
+            p1 = cdf((value1 - mean) / std)
+            p2 = cdf((value2 - mean) / std)
 
             similarity = 1 - abs(p1 - p2)
 
             mean_percentile = (p1 + p2) / 2
             similarity *= 2 * abs(mean_percentile - 0.5)
             return similarity
         else:
```

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/internal_types.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/internal_types.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/patsim.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/patient_similarity/patsim.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer/tmp.py` & `fhir_analyzer-0.0.4/src/fhir_analyzer/tmp.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/SOURCES.txt` & `fhir_analyzer-0.0.4/src/fhir_analyzer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-requirements.txt
 src/fhir_analyzer/__init__.py
 src/fhir_analyzer/constants.py
 src/fhir_analyzer/feature_selector.py
 src/fhir_analyzer/fhirstore.py
 src/fhir_analyzer/helper.py
 src/fhir_analyzer/tmp.py
 src/fhir_analyzer.egg-info/PKG-INFO
```

