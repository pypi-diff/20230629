# Comparing `tmp/PCCanalyser-0.5.0.tar.gz` & `tmp/PCCanalyser-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCCanalyser-0.5.0.tar", last modified: Tue Jun  6 20:11:56 2023, max compression
+gzip compressed data, was "PCCanalyser-0.5.1.tar", last modified: Thu Jun 29 20:44:55 2023, max compression
```

## Comparing `PCCanalyser-0.5.0.tar` & `PCCanalyser-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.765819 PCCanalyser-0.5.0/
--rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.5.0/LICENSE
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.761885 PCCanalyser-0.5.0/PCCanalyser.egg-info/
--rw-r--r--   0 v94623eb2   (504) staff       (20)    16261 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)      482 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/entry_points.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       76 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/requires.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-06-06 20:11:56.000000 PCCanalyser-0.5.0/PCCanalyser.egg-info/top_level.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)    16261 2023-06-06 20:11:56.765569 PCCanalyser-0.5.0/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)    16117 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/README.md
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.764626 PCCanalyser-0.5.0/matgen/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.0/matgen/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    65850 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     1648 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/characterise.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     5922 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/entropic.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    19059 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/matutils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/ndisangles.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/ndisorientquat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    12153 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/sparsemat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/matgen/utils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      901 2023-06-06 20:11:05.000000 PCCanalyser-0.5.0/pyproject.toml
--rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-06-06 20:11:56.765872 PCCanalyser-0.5.0/setup.cfg
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-06 20:11:56.765314 PCCanalyser-0.5.0/tests/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.0/tests/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.5.0/tests/test_base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-06-06 19:55:50.000000 PCCanalyser-0.5.0/tests/test_sparsemat.py
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.663468 PCCanalyser-0.5.1/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.5.1/LICENSE
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.637054 PCCanalyser-0.5.1/PCCanalyser.egg-info/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16282 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      482 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/entry_points.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       76 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/requires.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/top_level.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16282 2023-06-29 20:44:55.662856 PCCanalyser-0.5.1/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16117 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/README.md
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.646735 PCCanalyser-0.5.1/matgen/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.1/matgen/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    65850 2023-06-29 20:36:38.000000 PCCanalyser-0.5.1/matgen/base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1648 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/characterise.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     5922 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/entropic.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    19059 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/matutils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/ndisangles.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/ndisorientquat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    12153 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/sparsemat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/utils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      940 2023-06-29 20:43:04.000000 PCCanalyser-0.5.1/pyproject.toml
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-06-29 20:44:55.663558 PCCanalyser-0.5.1/setup.cfg
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.649227 PCCanalyser-0.5.1/tests/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.1/tests/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.5.1/tests/test_base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/tests/test_sparsemat.py
```

### Comparing `PCCanalyser-0.5.0/LICENSE` & `PCCanalyser-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/PCCanalyser.egg-info/PKG-INFO` & `PCCanalyser-0.5.1/PCCanalyser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: PCCanalyser
-Version: 0.5.0
+Version: 0.5.1
 Summary: Polyhedral Cell Complex (PCC) Analysis tools
+Author: Oleg Bushuev
 Project-URL: documentation, https://github.com/PRISBteam/Voronoi_PCC_Analyser
 Project-URL: repository, https://github.com/PRISBteam/Voronoi_PCC_Analyser.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Polyhedral Cell Complex (PCC) Analyser
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.0 Summary: Polyhedral Cell
-Complex (PCC) Analysis tools Project-URL: documentation, https://github.com/
-PRISBteam/Voronoi_PCC_Analyser Project-URL: repository, https://github.com/
-PRISBteam/Voronoi_PCC_Analyser.git Description-Content-Type: text/markdown
-License-File: LICENSE # Polyhedral Cell Complex (PCC) Analyser ## Quick start
-Installation: ``` pip install PCCanalyser ``` Using of classes: ``` from
-matgen.base import CellComplex from matgen.entropic import TripleJunctionSet
-``` Command-line interface (CLI) tools: ``` # generate sparse matrices
-sparsemat --file complex.tess --dir path/to/target/directory # find
+Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.1 Summary: Polyhedral Cell
+Complex (PCC) Analysis tools Author: Oleg Bushuev Project-URL: documentation,
+https://github.com/PRISBteam/Voronoi_PCC_Analyser Project-URL: repository,
+https://github.com/PRISBteam/Voronoi_PCC_Analyser.git Description-Content-Type:
+text/markdown License-File: LICENSE # Polyhedral Cell Complex (PCC) Analyser ##
+Quick start Installation: ``` pip install PCCanalyser ``` Using of classes: ```
+from matgen.base import CellComplex from matgen.entropic import
+TripleJunctionSet ``` Command-line interface (CLI) tools: ``` # generate sparse
+matrices sparsemat --file complex.tess --dir path/to/target/directory # find
 disorientation angles between neighbouring grains of orders less than N
 ndisanples --file complex.tess --dir path/to/target/directory --max-order N #
 find disorientation angles between neighbouring grains of orders less than N in
 quaternions ndisorientquat --file complex.tess --dir path/to/target/directory -
 -max-order N # characteristics of a cell complex characterise --dir path/to/
 files ``` For details see: [tutorial/Examples.ipynb](tutorial/Examples.ipynb)
 The code addressed the practical needs of creating discrete (combinatorial)
```

### Comparing `PCCanalyser-0.5.0/PKG-INFO` & `PCCanalyser-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: PCCanalyser
-Version: 0.5.0
+Version: 0.5.1
 Summary: Polyhedral Cell Complex (PCC) Analysis tools
+Author: Oleg Bushuev
 Project-URL: documentation, https://github.com/PRISBteam/Voronoi_PCC_Analyser
 Project-URL: repository, https://github.com/PRISBteam/Voronoi_PCC_Analyser.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Polyhedral Cell Complex (PCC) Analyser
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.0 Summary: Polyhedral Cell
-Complex (PCC) Analysis tools Project-URL: documentation, https://github.com/
-PRISBteam/Voronoi_PCC_Analyser Project-URL: repository, https://github.com/
-PRISBteam/Voronoi_PCC_Analyser.git Description-Content-Type: text/markdown
-License-File: LICENSE # Polyhedral Cell Complex (PCC) Analyser ## Quick start
-Installation: ``` pip install PCCanalyser ``` Using of classes: ``` from
-matgen.base import CellComplex from matgen.entropic import TripleJunctionSet
-``` Command-line interface (CLI) tools: ``` # generate sparse matrices
-sparsemat --file complex.tess --dir path/to/target/directory # find
+Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.1 Summary: Polyhedral Cell
+Complex (PCC) Analysis tools Author: Oleg Bushuev Project-URL: documentation,
+https://github.com/PRISBteam/Voronoi_PCC_Analyser Project-URL: repository,
+https://github.com/PRISBteam/Voronoi_PCC_Analyser.git Description-Content-Type:
+text/markdown License-File: LICENSE # Polyhedral Cell Complex (PCC) Analyser ##
+Quick start Installation: ``` pip install PCCanalyser ``` Using of classes: ```
+from matgen.base import CellComplex from matgen.entropic import
+TripleJunctionSet ``` Command-line interface (CLI) tools: ``` # generate sparse
+matrices sparsemat --file complex.tess --dir path/to/target/directory # find
 disorientation angles between neighbouring grains of orders less than N
 ndisanples --file complex.tess --dir path/to/target/directory --max-order N #
 find disorientation angles between neighbouring grains of orders less than N in
 quaternions ndisorientquat --file complex.tess --dir path/to/target/directory -
 -max-order N # characteristics of a cell complex characterise --dir path/to/
 files ``` For details see: [tutorial/Examples.ipynb](tutorial/Examples.ipynb)
 The code addressed the practical needs of creating discrete (combinatorial)
```

### Comparing `PCCanalyser-0.5.0/README.md` & `PCCanalyser-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/base.py` & `PCCanalyser-0.5.1/matgen/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
                 coeff = 0
         except:
             coeff = 1
 
         if self.is_external:
             return 0
         else:
-            return (2 * self.gb_index) / (3 * len(self.n_ids) * coeff)
+            return (2 * self.gb_index) / (3 * len(self.n_ids)) * coeff
         
 
 class TripleJunction(LowerOrderCell):
     """
     Triple junction (TJ). 
     2D: 0-cells (vertices) are considered to be triple junctions.
     3D: 1-cells (edges) are considered to be triple junctions.
```

### Comparing `PCCanalyser-0.5.0/matgen/characterise.py` & `PCCanalyser-0.5.1/matgen/characterise.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/entropic.py` & `PCCanalyser-0.5.1/matgen/entropic.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/matutils.py` & `PCCanalyser-0.5.1/matgen/matutils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/ndisangles.py` & `PCCanalyser-0.5.1/matgen/ndisangles.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/ndisorientquat.py` & `PCCanalyser-0.5.1/matgen/ndisorientquat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/sparsemat.py` & `PCCanalyser-0.5.1/matgen/sparsemat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/matgen/utils.py` & `PCCanalyser-0.5.1/matgen/utils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.0/pyproject.toml` & `PCCanalyser-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PCCanalyser"
-version = "0.5.0"
+version = "0.5.1"
 dependencies = [
     "numpy >= 1.21.5", "scipy >= 1.7.3", "tqdm >= 4.64.1",
     "jupyterlab >= 3.4.4", "matplotlib >= 3.5.2",
 ]
 description = "Polyhedral Cell Complex (PCC) Analysis tools"
 readme = "README.md"
+authors = [{ name = "Oleg Bushuev" },]
 
 [project.urls]
 documentation = "https://github.com/PRISBteam/Voronoi_PCC_Analyser"
 repository = "https://github.com/PRISBteam/Voronoi_PCC_Analyser.git"
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
```

