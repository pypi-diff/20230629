# Comparing `tmp/fca-algorithms-0.2.4.tar.gz` & `tmp/fca-algorithms-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fca-algorithms-0.2.4.tar", last modified: Fri Jun 16 08:09:20 2023, max compression
+gzip compressed data, was "fca-algorithms-1.0.0.tar", last modified: Thu Jun 29 15:00:04 2023, max compression
```

## Comparing `fca-algorithms-0.2.4.tar` & `fca-algorithms-1.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.132321 fca-algorithms-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)    18655 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-16 08:09:20.132321 fca-algorithms-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 08:09:20.132321 fca-algorithms-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.123321 fca-algorithms-0.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.126321 fca-algorithms-0.2.4/src/fca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5422 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/api_models.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/association_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/base_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/border_hasse.py
--rw-rw-rw-   0 root         (0) root         (0)     1800 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/get_lattice.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/in_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.126321 fca-algorithms-0.2.4/src/fca/plot/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7164 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/plot/tikz_tpl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.128321 fca-algorithms-0.2.4/src/fca/rca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/rca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2523 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/rca/cpop.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/rca/models.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/rca/p18n.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/rca/rca.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/rca/rca_mickael.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.129320 fca-algorithms-0.2.4/src/fca/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/scripts/export_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/scripts/fca_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/scripts/import_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.129320 fca-algorithms-0.2.4/src/fca/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/fca/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.131321 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-16 08:09:20.000000 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      942 2023-06-16 08:09:20.000000 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 08:09:20.000000 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-16 08:09:20.000000 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-16 08:09:20.000000 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-16 08:09:20.000000 fca-algorithms-0.2.4/src/fca_algorithms.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 08:09:20.132321 fca-algorithms-0.2.4/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2915 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/tests/test_in_close.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-16 08:08:54.000000 fca-algorithms-0.2.4/src/tests/test_rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.946639 fca-algorithms-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18655 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-06-29 15:00:04.945639 fca-algorithms-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 15:00:04.946639 fca-algorithms-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.937639 fca-algorithms-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.939639 fca-algorithms-1.0.0/src/fca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5422 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/api_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/association_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/base_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/border_hasse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/get_lattice.py
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/in_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.940639 fca-algorithms-1.0.0/src/fca/plot/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7164 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/plot/tikz_tpl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.941639 fca-algorithms-1.0.0/src/fca/rca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/cpop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/p18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/rca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/rca/rca_mickael.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.942639 fca-algorithms-1.0.0/src/fca/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/export_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/fca_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/scripts/import_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.943639 fca-algorithms-1.0.0/src/fca/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/fca/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.944639 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      942 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-29 15:00:04.000000 fca-algorithms-1.0.0/src/fca_algorithms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:00:04.945639 fca-algorithms-1.0.0/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/test_in_close.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-06-29 14:59:37.000000 fca-algorithms-1.0.0/src/tests/test_rca.py
```

### Comparing `fca-algorithms-0.2.4/LICENSE` & `fca-algorithms-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/PKG-INFO` & `fca-algorithms-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fca-algorithms
-Version: 0.2.4
+Version: 1.0.0
 Summary: FCA basic algorithms
 Author: Ramshell
 Author-email: ramshellcinox@gmail.com
 License: CC By 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `fca-algorithms-0.2.4/README.md` & `fca-algorithms-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/setup.py` & `fca-algorithms-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fca-algorithms",
-    version="0.2.4",
+    version="1.0.0",
     author="Ramshell",
     author_email="ramshellcinox@gmail.com",
     license="CC By 4.0",
     description="FCA basic algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -19,14 +19,15 @@
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
         'apyori>=1.1.2',
         'networkx>=2.5',
         'matplotlib>=3.3',
+        'fca_algorithms_cpp>=0.1.3',
     ],
     entry_points={
         'console_scripts': [
             'fca_cli=fca.scripts.fca_cli:main',
         ]
     },
 )
```

### Comparing `fca-algorithms-0.2.4/src/fca/api_models.py` & `fca-algorithms-1.0.0/src/fca/api_models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/association_rules.py` & `fca-algorithms-1.0.0/src/fca/association_rules.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/base_models.py` & `fca-algorithms-1.0.0/src/fca/base_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 
 class Context:
-    def __init__(self, O, A, I):
+    def __init__(self, O, A, I: List[List[int]]):
         """
         :param O: a list of objects (strings for the moment) len(O) = n
         :param A: a list of attributes (strings for the moment) len(A) = m
         :param I: a nm incidence matrix, beign I[i][j] = 1 if object i has the attribute j, 0 <= i <= n, 0 <= j <= m
         """
         self.O: List = O
         self.A: List = A
@@ -20,25 +20,25 @@
 
     def _derivative_attr(self, Y):
         res = set()
         for attr in Y:
             attr_idx = self.A.index(attr)
             for obj in self.O:
                 obj_idx = self.O.index(obj)
-                if I[obj_idx][attr_idx]:
+                if self.I[obj_idx][attr_idx]:
                     res.add(obj)
         return list(res)
 
     def _derivative_obj(self, Objs):
         res = set()
         for obj in Objs:
             obj_idx = self.O.index(obj)
             for attr in self.A:
                 attr_idx = self.A.index(attr)
-                if I[obj_idx][attr_idx]:
+                if self.I[obj_idx][attr_idx]:
                     res.add(attr)
         return list(res)
 
     def __repr__(self):
         return f'O: {self.O},\n' \
                f'A: {self.A},\n' \
                f'I: {self.I}'
@@ -56,15 +56,15 @@
         self.O = O
         self.A = A
         # this is not supposed to change, so it's a frozenset
         self._set_O = frozenset(O)
         self.parents = parents
         self.children = children
 
-    def in_extent(o) -> bool:
+    def in_extent(self, o) -> bool:
         return o in self._set_O  # O(1) amortised
 
     def add_child(self, concept):
         self.children.append(concept)
         concept.parents.append(self)
 
     def __repr__(self):
```

### Comparing `fca-algorithms-0.2.4/src/fca/border_hasse.py` & `fca-algorithms-1.0.0/src/fca/border_hasse.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/get_lattice.py` & `fca-algorithms-1.0.0/src/fca/get_lattice.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/plot/plot.py` & `fca-algorithms-1.0.0/src/fca/plot/plot.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/rca/cpop.py` & `fca-algorithms-1.0.0/src/fca/rca/cpop.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/rca/models.py` & `fca-algorithms-1.0.0/src/fca/rca/models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/rca/rca.py` & `fca-algorithms-1.0.0/src/fca/rca/rca.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/rca/rca_mickael.py` & `fca-algorithms-1.0.0/src/fca/rca/rca_mickael.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/scripts/export_utils.py` & `fca-algorithms-1.0.0/src/fca/scripts/export_utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/scripts/fca_cli.py` & `fca-algorithms-1.0.0/src/fca/scripts/fca_cli.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/scripts/import_utils.py` & `fca-algorithms-1.0.0/src/fca/scripts/import_utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca/utils/utils.py` & `fca-algorithms-1.0.0/src/fca/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/fca_algorithms.egg-info/PKG-INFO` & `fca-algorithms-1.0.0/src/fca_algorithms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fca-algorithms
-Version: 0.2.4
+Version: 1.0.0
 Summary: FCA basic algorithms
 Author: Ramshell
 Author-email: ramshellcinox@gmail.com
 License: CC By 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `fca-algorithms-0.2.4/src/fca_algorithms.egg-info/SOURCES.txt` & `fca-algorithms-1.0.0/src/fca_algorithms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/tests/test_api.py` & `fca-algorithms-1.0.0/src/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.4/src/tests/test_in_close.py` & `fca-algorithms-1.0.0/src/tests/test_in_close.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     assert res == expected_result
 
 
 def test_inclose_solver_returns_all_the_concepts_when_there_are_objects_with_all_attributes(
         create_objects_and_attributes):
     O, A, I = create_objects_and_attributes
     c = Context(O, A, I)
-    c.I[1][1] = True
+    c.I[1][1] = 1
     concepts = Inclose().get_concepts(c)
     res = [x.to_tuple() for x in concepts]
     assert (['Tg05FX'], ['Effect', 'Power', 'Control', 'Short']) in res
 
 
 def test_inclose_solver_returns_association_rules(
         create_objects_and_attributes):
```

### Comparing `fca-algorithms-0.2.4/src/tests/test_rca.py` & `fca-algorithms-1.0.0/src/tests/test_rca.py`

 * *Files identical despite different names*

