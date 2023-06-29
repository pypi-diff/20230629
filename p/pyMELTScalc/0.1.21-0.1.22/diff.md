# Comparing `tmp/pyMELTScalc-0.1.21.tar.gz` & `tmp/pyMELTScalc-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMELTScalc-0.1.21.tar", last modified: Thu Jun 29 19:59:14 2023, max compression
+gzip compressed data, was "pyMELTScalc-0.1.22.tar", last modified: Thu Jun 29 20:48:14 2023, max compression
```

## Comparing `pyMELTScalc-0.1.21.tar` & `pyMELTScalc-0.1.22.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:59:14.589529 pyMELTScalc-0.1.21/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-29 19:59:14.585529 pyMELTScalc-0.1.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:59:14.589529 pyMELTScalc-0.1.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:59:14.585529 pyMELTScalc-0.1.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:59:14.585529 pyMELTScalc-0.1.21/src/pyMELTScalc/
--rw-r--r--   0 runner    (1001) docker     (123)    42082 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Barom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/GenFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Holland.py
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Liq.py
--rw-r--r--   0 runner    (1001) docker     (123)    43028 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/MELTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    24305 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Path_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/PhaseDiagrams.py
--rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/Saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-29 19:59:03.000000 pyMELTScalc-0.1.21/src/pyMELTScalc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:59:14.585529 pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-29 19:59:14.000000 pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-29 19:59:14.000000 pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:59:14.000000 pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 19:59:14.000000 pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 19:59:14.000000 pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.473933 pyMELTScalc-0.1.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.473933 pyMELTScalc-0.1.22/src/pyMELTScalc/
+-rw-r--r--   0 runner    (1001) docker     (123)    42082 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Barom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/GenFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Holland.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Liq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43028 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/MELTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24305 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Path_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/PhaseDiagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/Saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-29 20:48:00.000000 pyMELTScalc-0.1.22/src/pyMELTScalc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:48:14.477933 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 20:48:14.000000 pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/top_level.txt
```

### Comparing `pyMELTScalc-0.1.21/PKG-INFO` & `pyMELTScalc-0.1.22/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: pyMELTScalc
-Version: 0.1.21
+Version: 0.1.22
 Summary: pyMELTScalc
 Home-page: https://github.com/gleesonm1/pyMELTScalc
 Author: Matthew Gleeson
 Author-email: gleesonm@berkeley.edu
 License: UNKNOWN
-Description: ## pyMELTScalc
+Description: ## ReadTheDocs
+        
+        https://pymeltscalc.readthedocs.io/en/latest/
+        
+        ## pyMELTScalc
         
         Petrological calculations using the MELTS or thermodynamic databases. Through integration with the pyMAGEMINcalc repository, calculations can also be performed using the thermodynamic database of Holland et al. (2018).
         
         # Using MELTS
         As a default, this package uses the MELTS algorithms and the alphaMELTS for Python package, developed by Dr Paula Antoshechkina, to perform the thermodynamic calculations. Therefore, it is neccessary for any user to first download the alphaMELTS for Python package. Luckily, version 1.2.0beta of MELTS for Python is included in this repository and we have extensively checked that this version of MELTS for Python works with out code. Future versions of MELTS for Python might be available via:
         https://magmasource.caltech.edu/gitlist/MELTS_Matlab.git/
         although we caution that newer versions of MELTS for Python may not be compatible with pyMELTScalc.
```

### Comparing `pyMELTScalc-0.1.21/README.md` & `pyMELTScalc-0.1.22/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## ReadTheDocs
+
+https://pymeltscalc.readthedocs.io/en/latest/
+
 ## pyMELTScalc
 
 Petrological calculations using the MELTS or thermodynamic databases. Through integration with the pyMAGEMINcalc repository, calculations can also be performed using the thermodynamic database of Holland et al. (2018).
 
 # Using MELTS
 As a default, this package uses the MELTS algorithms and the alphaMELTS for Python package, developed by Dr Paula Antoshechkina, to perform the thermodynamic calculations. Therefore, it is neccessary for any user to first download the alphaMELTS for Python package. Luckily, version 1.2.0beta of MELTS for Python is included in this repository and we have extensively checked that this version of MELTS for Python works with out code. Future versions of MELTS for Python might be available via:
 https://magmasource.caltech.edu/gitlist/MELTS_Matlab.git/
```

### Comparing `pyMELTScalc-0.1.21/setup.py` & `pyMELTScalc-0.1.22/setup.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Barom.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Barom.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/GenFuncs.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/GenFuncs.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Holland.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Holland.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Liq.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Liq.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/MELTS.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/MELTS.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Path.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Path.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Path_wrappers.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Path_wrappers.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/PhaseDiagrams.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/PhaseDiagrams.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Plotting.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Plotting.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/Saturation.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/Saturation.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc/__init__.py` & `pyMELTScalc-0.1.22/src/pyMELTScalc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/PKG-INFO` & `pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: pyMELTScalc
-Version: 0.1.21
+Version: 0.1.22
 Summary: pyMELTScalc
 Home-page: https://github.com/gleesonm1/pyMELTScalc
 Author: Matthew Gleeson
 Author-email: gleesonm@berkeley.edu
 License: UNKNOWN
-Description: ## pyMELTScalc
+Description: ## ReadTheDocs
+        
+        https://pymeltscalc.readthedocs.io/en/latest/
+        
+        ## pyMELTScalc
         
         Petrological calculations using the MELTS or thermodynamic databases. Through integration with the pyMAGEMINcalc repository, calculations can also be performed using the thermodynamic database of Holland et al. (2018).
         
         # Using MELTS
         As a default, this package uses the MELTS algorithms and the alphaMELTS for Python package, developed by Dr Paula Antoshechkina, to perform the thermodynamic calculations. Therefore, it is neccessary for any user to first download the alphaMELTS for Python package. Luckily, version 1.2.0beta of MELTS for Python is included in this repository and we have extensively checked that this version of MELTS for Python works with out code. Future versions of MELTS for Python might be available via:
         https://magmasource.caltech.edu/gitlist/MELTS_Matlab.git/
         although we caution that newer versions of MELTS for Python may not be compatible with pyMELTScalc.
```

### Comparing `pyMELTScalc-0.1.21/src/pyMELTScalc.egg-info/SOURCES.txt` & `pyMELTScalc-0.1.22/src/pyMELTScalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

