# Comparing `tmp/gascompressibility-0.1.5.tar.gz` & `tmp/gascompressibility-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gascompressibility-0.1.5.tar", last modified: Thu Jun 29 17:15:56 2023, max compression
+gzip compressed data, was "gascompressibility-0.1.6.tar", last modified: Thu Jun 29 18:28:54 2023, max compression
```

## Comparing `gascompressibility-0.1.5.tar` & `gascompressibility-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    11101 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    10123 2023-06-28 22:59:44.000000 gascompressibility-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility/
--rw-rw-rw-   0        0        0      209 2023-06-28 22:34:59.000000 gascompressibility-0.1.5/gascompressibility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility/pseudocritical/
--rw-rw-rw-   0        0        0    17368 2023-06-28 22:59:09.000000 gascompressibility-0.1.5/gascompressibility/pseudocritical/Piper.py
--rw-rw-rw-   0        0        0    20360 2023-06-28 23:30:34.000000 gascompressibility-0.1.5/gascompressibility/pseudocritical/Sutton.py
--rw-rw-rw-   0        0        0       56 2023-06-28 22:59:09.000000 gascompressibility-0.1.5/gascompressibility/pseudocritical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.5/gascompressibility/utilities/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.5/gascompressibility/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/
--rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/DAK.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/hall_yarborough.py
--rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/kareem.py
--rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/londono.py
--rw-rw-rw-   0        0        0     6067 2023-06-28 22:59:09.000000 gascompressibility-0.1.5/gascompressibility/z_correlation/z_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0    11101 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1549 2023-06-29 17:15:44.000000 gascompressibility-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:15:56.000000 gascompressibility-0.1.5/tests/
--rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.5/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.788940 gascompressibility-0.1.6/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    11101 2023-06-29 18:28:54.788940 gascompressibility-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10123 2023-06-28 22:59:44.000000 gascompressibility-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.740970 gascompressibility-0.1.6/gascompressibility/
+-rw-rw-rw-   0        0        0      209 2023-06-28 22:34:59.000000 gascompressibility-0.1.6/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.759968 gascompressibility-0.1.6/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0    17335 2023-06-29 17:48:34.000000 gascompressibility-0.1.6/gascompressibility/pseudocritical/Piper.py
+-rw-rw-rw-   0        0        0    20224 2023-06-29 17:48:34.000000 gascompressibility-0.1.6/gascompressibility/pseudocritical/Sutton.py
+-rw-rw-rw-   0        0        0       56 2023-06-29 18:25:42.000000 gascompressibility-0.1.6/gascompressibility/pseudocritical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.764973 gascompressibility-0.1.6/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.6/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.6/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.783940 gascompressibility-0.1.6/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0     5965 2023-06-29 18:26:44.000000 gascompressibility-0.1.6/gascompressibility/z_correlation/z_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.757969 gascompressibility-0.1.6/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    11101 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:28:54.000000 gascompressibility-0.1.6/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:28:54.789939 gascompressibility-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-06-29 18:28:09.000000 gascompressibility-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:28:54.787940 gascompressibility-0.1.6/tests/
+-rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.6/tests/test_gascomp.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gascompressibility-0.1.5/LICENSE` & `gascompressibility-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.5/PKG-INFO` & `gascompressibility-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.5
+Version: 0.1.6
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.5/README.md` & `gascompressibility-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.5/gascompressibility/pseudocritical/Piper.py` & `gascompressibility-0.1.6/gascompressibility/pseudocritical/Piper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import matplotlib.pyplot as plt
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
 from gascompressibility.utilities.utilities import calc_psig_to_psia
 
 """
 This is a Piper module
```

### Comparing `gascompressibility-0.1.5/gascompressibility/pseudocritical/Sutton.py` & `gascompressibility-0.1.6/gascompressibility/pseudocritical/Sutton.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import numpy as np
-from scipy import optimize
-import matplotlib.pyplot as plt
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
 from gascompressibility.utilities.utilities import calc_psig_to_psia
-from gascompressibility.z_correlation import z_helper
 
 
 class Sutton():
 
     """
     Class object to calculate pseudo-critical properties.
```

### Comparing `gascompressibility-0.1.5/gascompressibility/z_correlation/DAK.py` & `gascompressibility-0.1.6/gascompressibility/z_correlation/DAK.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.5/gascompressibility/z_correlation/hall_yarborough.py` & `gascompressibility-0.1.6/gascompressibility/z_correlation/hall_yarborough.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.5/gascompressibility/z_correlation/kareem.py` & `gascompressibility-0.1.6/gascompressibility/z_correlation/kareem.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.5/gascompressibility/z_correlation/londono.py` & `gascompressibility-0.1.6/gascompressibility/z_correlation/londono.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.5/gascompressibility/z_correlation/z_helper.py` & `gascompressibility-0.1.6/gascompressibility/z_correlation/z_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,20 @@
             ps_props = {'z': Z, 'Pr': Pr, 'Tr': Tr}
             return ps_props
         else:
             return Z
 
     # Pr and Tr are NOT provided:
     if pmodel == 'Piper':
-        pc_instance = Piper.Piper()  # this import doesn't work on this file but it will work when imported from other files
+        pc_instance = Piper()
         Tr, Pr = pc_instance._initialize_Tr_and_Pr(sg=sg, P=P, T=T, Tr=Tr, Pr=Pr, H2S=H2S, CO2=CO2, N2=N2, ignore_conflict=ignore_conflict, **kwargs)
     elif pmodel == 'Sutton':
         if N2 is not None:
             raise KeyError('pmodel="Sutton" does not support N2 as input. Set N2=None')
-        pc_instance = Sutton.Sutton()
+        pc_instance = Sutton()
         Tr, Pr = pc_instance._initialize_Tr_and_Pr(sg=sg, P=P, T=T, Tr=Tr, Pr=Pr, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict, **kwargs)
     else:
         raise KeyError(
             'Pseudo-critical model "%s" is not implemented. Choose from the list of available models: %s' % (pmodel, pmodels_ks)
         )
 
     Z = _calc_z_explicit_implicit_helper(Pr, Tr, z_model, zmodel, guess, newton_kwargs, ps_props)
```

### Comparing `gascompressibility-0.1.5/gascompressibility.egg-info/PKG-INFO` & `gascompressibility-0.1.6/gascompressibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.5
+Version: 0.1.6
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.5/gascompressibility.egg-info/SOURCES.txt` & `gascompressibility-0.1.6/gascompressibility.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 gascompressibility.egg-info/SOURCES.txt
 gascompressibility.egg-info/dependency_links.txt
 gascompressibility.egg-info/requires.txt
 gascompressibility.egg-info/top_level.txt
 gascompressibility/pseudocritical/Piper.py
 gascompressibility/pseudocritical/Sutton.py
 gascompressibility/pseudocritical/__init__.py
+gascompressibility/pseudocritical/piper.py
+gascompressibility/pseudocritical/sutton.py
 gascompressibility/utilities/__init__.py
 gascompressibility/utilities/utilities.py
 gascompressibility/z_correlation/DAK.py
 gascompressibility/z_correlation/__init__.py
 gascompressibility/z_correlation/hall_yarborough.py
 gascompressibility/z_correlation/kareem.py
 gascompressibility/z_correlation/londono.py
```

### Comparing `gascompressibility-0.1.5/setup.py` & `gascompressibility-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
```

### Comparing `gascompressibility-0.1.5/tests/test_gascomp.py` & `gascompressibility-0.1.6/tests/test_gascomp.py`

 * *Files identical despite different names*

