# Comparing `tmp/fca-algorithms-1.0.0.tar.gz` & `tmp/fca-algorithms-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fca-algorithms-1.0.0.tar", last modified: Thu Jun 29 15:00:04 2023, max compression
+gzip compressed data, was "fca-algorithms-1.0.1.tar", last modified: Thu Jun 29 15:15:17 2023, max compression
```

## Comparing `fca-algorithms-1.0.0.tar` & `fca-algorithms-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.946639 fca-algorithms-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    18655 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-29 15:00:04.945639 fca-algorithms-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 15:00:04.946639 fca-algorithms-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.937639 fca-algorithms-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.939639 fca-algorithms-1.0.0/src/fca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5422 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/api_models.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/association_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/base_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/border_hasse.py
--rw-rw-rw-   0 root         (0) root         (0)     1800 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/get_lattice.py
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/in_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.940639 fca-algorithms-1.0.0/src/fca/plot/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7164 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/plot/tikz_tpl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.941639 fca-algorithms-1.0.0/src/fca/rca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2523 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/cpop.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/models.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/p18n.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/rca.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/rca_mickael.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.942639 fca-algorithms-1.0.0/src/fca/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/export_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/fca_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/import_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.943639 fca-algorithms-1.0.0/src/fca/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.944639 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      942 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.945639 fca-algorithms-1.0.0/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/test_in_close.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/test_rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:17.004505 fca-algorithms-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    18655 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-06-29 15:15:17.003505 fca-algorithms-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 15:15:17.004505 fca-algorithms-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:16.993505 fca-algorithms-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:16.995505 fca-algorithms-1.0.1/src/fca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5422 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/api_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/association_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/base_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/border_hasse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/get_lattice.py
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/in_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:16.996505 fca-algorithms-1.0.1/src/fca/plot/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7164 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/plot/tikz_tpl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:16.998505 fca-algorithms-1.0.1/src/fca/rca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/rca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/rca/cpop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/rca/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/rca/p18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/rca/rca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/rca/rca_mickael.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:17.000505 fca-algorithms-1.0.1/src/fca/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/scripts/export_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/scripts/fca_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/scripts/import_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:17.000505 fca-algorithms-1.0.1/src/fca/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/fca/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:17.002505 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-06-29 15:15:16.000000 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      942 2023-06-29 15:15:16.000000 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 15:15:16.000000 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-29 15:15:16.000000 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-29 15:15:16.000000 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-29 15:15:16.000000 fca-algorithms-1.0.1/src/fca_algorithms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:15:17.003505 fca-algorithms-1.0.1/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/tests/test_in_close.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-29 15:14:48.000000 fca-algorithms-1.0.1/src/tests/test_rca.py
```

### Comparing `fca-algorithms-1.0.0/LICENSE` & `fca-algorithms-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/PKG-INFO` & `fca-algorithms-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,13 @@
-Metadata-Version: 2.1
-Name: fca-algorithms
-Version: 1.0.0
-Summary: FCA basic algorithms
-Author: Ramshell
-Author-email: ramshellcinox@gmail.com
-License: CC By 4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![build](https://gitlab.com/cps-phd-leutwyler-nicolas/rca_fca_general/badges/master/pipeline.svg)
 
 
 # FCA algorithms
 
-This is a module providing a set of commonly used algorithms in FCA, RCA, and some of its variants. Its general intention is to provide an easy to use API so that it's easier to create other programs using these algorithms. Since it's built with python, the overall performance is not expected to be outstanding. Having that said, the chosen algorithms have a somewhat low algorithmic temporal complexity.
+This is a module providing a set of commonly used algorithms in FCA, RCA, and some of its variants. Its general intention is to provide an easy to use API so that it's easier to create other programs using these algorithms. The main algorithm that calculates formal concepts is `inclose`, and, in [this version](https://pypi.org/project/fca-algorithms/1.0.0/), it is implemented in C++. Considering this, the API is expected to behave somewhat acceptably.
 
 
 # CLI
 
 
 ## FCA
 
@@ -66,18 +53,18 @@
 # FCA utils
 
 Module for FCA basics such as retrieving concepts, drawing a hasse diagram, etc
 
 ## Getting formal concepts
 
 ```python
-from fca.api_models import Context
+from fca.api_models import Context, Concept
 
-c = Context(O, A, I)
-concepts = c.get_concepts(c)
+c = Context(O : List[str], A : List[str], I : List[List[int]])
+concepts = c.get_concepts(c) List[Concept]
 ```
 
 ## Getting association rules
 
 
 ```python
 from fca.api_models import Context
```

### Comparing `fca-algorithms-1.0.0/README.md` & `fca-algorithms-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,26 @@
+Metadata-Version: 2.1
+Name: fca-algorithms
+Version: 1.0.1
+Summary: FCA basic algorithms
+Author: Ramshell
+Author-email: ramshellcinox@gmail.com
+License: CC By 4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![build](https://gitlab.com/cps-phd-leutwyler-nicolas/rca_fca_general/badges/master/pipeline.svg)
 
 
 # FCA algorithms
 
-This is a module providing a set of commonly used algorithms in FCA, RCA, and some of its variants. Its general intention is to provide an easy to use API so that it's easier to create other programs using these algorithms. Since it's built with python, the overall performance is not expected to be outstanding. Having that said, the chosen algorithms have a somewhat low algorithmic temporal complexity.
+This is a module providing a set of commonly used algorithms in FCA, RCA, and some of its variants. Its general intention is to provide an easy to use API so that it's easier to create other programs using these algorithms. The main algorithm that calculates formal concepts is `inclose`, and, in [this version](https://pypi.org/project/fca-algorithms/1.0.0/), it is implemented in C++. Considering this, the API is expected to behave somewhat acceptably.
 
 
 # CLI
 
 
 ## FCA
 
@@ -53,18 +66,18 @@
 # FCA utils
 
 Module for FCA basics such as retrieving concepts, drawing a hasse diagram, etc
 
 ## Getting formal concepts
 
 ```python
-from fca.api_models import Context
+from fca.api_models import Context, Concept
 
-c = Context(O, A, I)
-concepts = c.get_concepts(c)
+c = Context(O : List[str], A : List[str], I : List[List[int]])
+concepts = c.get_concepts(c) List[Concept]
 ```
 
 ## Getting association rules
 
 
 ```python
 from fca.api_models import Context
```

### Comparing `fca-algorithms-1.0.0/setup.py` & `fca-algorithms-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fca-algorithms",
-    version="1.0.0",
+    version="1.0.1",
     author="Ramshell",
     author_email="ramshellcinox@gmail.com",
     license="CC By 4.0",
     description="FCA basic algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `fca-algorithms-1.0.0/src/fca/api_models.py` & `fca-algorithms-1.0.1/src/fca/api_models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/association_rules.py` & `fca-algorithms-1.0.1/src/fca/association_rules.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/base_models.py` & `fca-algorithms-1.0.1/src/fca/base_models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/border_hasse.py` & `fca-algorithms-1.0.1/src/fca/border_hasse.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/get_lattice.py` & `fca-algorithms-1.0.1/src/fca/get_lattice.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/plot/plot.py` & `fca-algorithms-1.0.1/src/fca/plot/plot.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/rca/cpop.py` & `fca-algorithms-1.0.1/src/fca/rca/cpop.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/rca/models.py` & `fca-algorithms-1.0.1/src/fca/rca/models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/rca/rca.py` & `fca-algorithms-1.0.1/src/fca/rca/rca.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/rca/rca_mickael.py` & `fca-algorithms-1.0.1/src/fca/rca/rca_mickael.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/scripts/export_utils.py` & `fca-algorithms-1.0.1/src/fca/scripts/export_utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/scripts/fca_cli.py` & `fca-algorithms-1.0.1/src/fca/scripts/fca_cli.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/scripts/import_utils.py` & `fca-algorithms-1.0.1/src/fca/scripts/import_utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca/utils/utils.py` & `fca-algorithms-1.0.1/src/fca/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/fca_algorithms.egg-info/PKG-INFO` & `fca-algorithms-1.0.1/src/fca_algorithms.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fca-algorithms
-Version: 1.0.0
+Version: 1.0.1
 Summary: FCA basic algorithms
 Author: Ramshell
 Author-email: ramshellcinox@gmail.com
 License: CC By 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 ![build](https://gitlab.com/cps-phd-leutwyler-nicolas/rca_fca_general/badges/master/pipeline.svg)
 
 
 # FCA algorithms
 
-This is a module providing a set of commonly used algorithms in FCA, RCA, and some of its variants. Its general intention is to provide an easy to use API so that it's easier to create other programs using these algorithms. Since it's built with python, the overall performance is not expected to be outstanding. Having that said, the chosen algorithms have a somewhat low algorithmic temporal complexity.
+This is a module providing a set of commonly used algorithms in FCA, RCA, and some of its variants. Its general intention is to provide an easy to use API so that it's easier to create other programs using these algorithms. The main algorithm that calculates formal concepts is `inclose`, and, in [this version](https://pypi.org/project/fca-algorithms/1.0.0/), it is implemented in C++. Considering this, the API is expected to behave somewhat acceptably.
 
 
 # CLI
 
 
 ## FCA
 
@@ -66,18 +66,18 @@
 # FCA utils
 
 Module for FCA basics such as retrieving concepts, drawing a hasse diagram, etc
 
 ## Getting formal concepts
 
 ```python
-from fca.api_models import Context
+from fca.api_models import Context, Concept
 
-c = Context(O, A, I)
-concepts = c.get_concepts(c)
+c = Context(O : List[str], A : List[str], I : List[List[int]])
+concepts = c.get_concepts(c) List[Concept]
 ```
 
 ## Getting association rules
 
 
 ```python
 from fca.api_models import Context
```

### Comparing `fca-algorithms-1.0.0/src/fca_algorithms.egg-info/SOURCES.txt` & `fca-algorithms-1.0.1/src/fca_algorithms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/tests/conftest.py` & `fca-algorithms-1.0.1/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/tests/test_api.py` & `fca-algorithms-1.0.1/src/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/tests/test_in_close.py` & `fca-algorithms-1.0.1/src/tests/test_in_close.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-1.0.0/src/tests/test_rca.py` & `fca-algorithms-1.0.1/src/tests/test_rca.py`

 * *Files identical despite different names*

