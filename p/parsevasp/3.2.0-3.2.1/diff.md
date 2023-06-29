# Comparing `tmp/parsevasp-3.2.0.tar.gz` & `tmp/parsevasp-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsevasp-3.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "parsevasp-3.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `parsevasp-3.2.0.tar` & `parsevasp-3.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1075 2023-03-30 11:01:36.486379 parsevasp-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0      536 2023-03-30 11:01:36.486379 parsevasp-3.2.0/README.rst
--rw-r--r--   0        0        0      194 2023-06-05 13:14:19.435740 parsevasp-3.2.0/parsevasp/__init__.py
--rw-r--r--   0        0        0     5985 2023-03-30 11:01:36.486379 parsevasp-3.2.0/parsevasp/base.py
--rw-r--r--   0        0        0     4588 2023-03-30 11:01:36.486379 parsevasp-3.2.0/parsevasp/chgcar.py
--rw-r--r--   0        0        0     1943 2023-03-30 11:01:36.486379 parsevasp-3.2.0/parsevasp/constants.py
--rw-r--r--   0        0        0    10926 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/doscar.py
--rw-r--r--   0        0        0     5742 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/eigenval.py
--rw-r--r--   0        0        0    20388 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/incar.py
--rw-r--r--   0        0        0    78855 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/incar.yml
--rw-r--r--   0        0        0    37215 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/kpoints.py
--rw-r--r--   0        0        0    17776 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/outcar.py
--rw-r--r--   0        0        0    36808 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/poscar.py
--rw-r--r--   0        0        0     7046 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/potcar.py
--rw-r--r--   0        0        0    15910 2023-06-05 13:14:19.439074 parsevasp-3.2.0/parsevasp/stream.py
--rw-r--r--   0        0        0     5076 2023-06-05 13:14:19.442407 parsevasp-3.2.0/parsevasp/stream.yml
--rw-r--r--   0        0        0     9403 2023-03-30 11:01:36.489713 parsevasp-3.2.0/parsevasp/utils.py
--rw-r--r--   0        0        0   136794 2023-06-05 13:14:19.442407 parsevasp-3.2.0/parsevasp/vasprun.py
--rw-r--r--   0        0        0     3106 2023-06-05 13:14:19.442407 parsevasp-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 parsevasp-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-30 11:01:36.486379 parsevasp-3.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      536 2023-03-30 11:01:36.486379 parsevasp-3.2.1/README.rst
+-rw-r--r--   0        0        0      194 2023-06-29 19:22:12.473444 parsevasp-3.2.1/parsevasp/__init__.py
+-rw-r--r--   0        0        0     5985 2023-03-30 11:01:36.486379 parsevasp-3.2.1/parsevasp/base.py
+-rw-r--r--   0        0        0     4588 2023-03-30 11:01:36.486379 parsevasp-3.2.1/parsevasp/chgcar.py
+-rw-r--r--   0        0        0     1943 2023-03-30 11:01:36.486379 parsevasp-3.2.1/parsevasp/constants.py
+-rw-r--r--   0        0        0    10926 2023-06-05 13:14:19.439074 parsevasp-3.2.1/parsevasp/doscar.py
+-rw-r--r--   0        0        0     5742 2023-03-30 11:01:36.489713 parsevasp-3.2.1/parsevasp/eigenval.py
+-rw-r--r--   0        0        0    20388 2023-06-05 13:14:19.439074 parsevasp-3.2.1/parsevasp/incar.py
+-rw-r--r--   0        0        0    78855 2023-03-30 11:01:36.489713 parsevasp-3.2.1/parsevasp/incar.yml
+-rw-r--r--   0        0        0    37215 2023-06-05 13:14:19.439074 parsevasp-3.2.1/parsevasp/kpoints.py
+-rw-r--r--   0        0        0    17776 2023-03-30 11:01:36.489713 parsevasp-3.2.1/parsevasp/outcar.py
+-rw-r--r--   0        0        0    36808 2023-06-05 13:14:19.439074 parsevasp-3.2.1/parsevasp/poscar.py
+-rw-r--r--   0        0        0     7355 2023-06-29 19:22:12.473444 parsevasp-3.2.1/parsevasp/potcar.py
+-rw-r--r--   0        0        0    15910 2023-06-05 13:14:19.439074 parsevasp-3.2.1/parsevasp/stream.py
+-rw-r--r--   0        0        0     5076 2023-06-05 13:14:19.442407 parsevasp-3.2.1/parsevasp/stream.yml
+-rw-r--r--   0        0        0     9403 2023-03-30 11:01:36.489713 parsevasp-3.2.1/parsevasp/utils.py
+-rw-r--r--   0        0        0   136794 2023-06-05 13:14:19.442407 parsevasp-3.2.1/parsevasp/vasprun.py
+-rw-r--r--   0        0        0     3106 2023-06-05 13:14:19.442407 parsevasp-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 parsevasp-3.2.1/PKG-INFO
```

### Comparing `parsevasp-3.2.0/LICENSE.txt` & `parsevasp-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/README.rst` & `parsevasp-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/base.py` & `parsevasp-3.2.1/parsevasp/base.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/chgcar.py` & `parsevasp-3.2.1/parsevasp/chgcar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/constants.py` & `parsevasp-3.2.1/parsevasp/constants.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/doscar.py` & `parsevasp-3.2.1/parsevasp/doscar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/eigenval.py` & `parsevasp-3.2.1/parsevasp/eigenval.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/incar.py` & `parsevasp-3.2.1/parsevasp/incar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/incar.yml` & `parsevasp-3.2.1/parsevasp/incar.yml`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/kpoints.py` & `parsevasp-3.2.1/parsevasp/kpoints.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/outcar.py` & `parsevasp-3.2.1/parsevasp/outcar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/poscar.py` & `parsevasp-3.2.1/parsevasp/poscar.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/potcar.py` & `parsevasp-3.2.1/parsevasp/potcar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 """Handle POTCAR
 
-This parser takes parts of the
+In order to not have pymatgen as a dependency, this parser takes parts of the
 `pymatgen parser<https://github.com/materialsproject/pymatgen/blob/v2023.3.23/pymatgen/io/vasp/inputs.py#L1616-L2211>`_
+for POTCAR here.
+
+Copyright info from their MIT license:
+
+Copyright (c) 2011-2012 MIT & The Regents of the University of California,
+through Lawrence Berkeley National Laboratory
+
+pymatgen also uses the MIT license so see this plugins LICENSE file for its copy.
 """
 
 import re
 
 from parsevasp import utils
 from parsevasp.base import BaseParser
```

### Comparing `parsevasp-3.2.0/parsevasp/stream.py` & `parsevasp-3.2.1/parsevasp/stream.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/stream.yml` & `parsevasp-3.2.1/parsevasp/stream.yml`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/utils.py` & `parsevasp-3.2.1/parsevasp/utils.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/parsevasp/vasprun.py` & `parsevasp-3.2.1/parsevasp/vasprun.py`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/pyproject.toml` & `parsevasp-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsevasp-3.2.0/PKG-INFO` & `parsevasp-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsevasp
-Version: 3.2.0
+Version: 3.2.1
 Summary: A general parser for VASP
 Keywords: vasp,parser
 Author-email: Espen Flage-Larsen	 <espen.flage-larsen@sigma2.no>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

