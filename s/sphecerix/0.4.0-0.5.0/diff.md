# Comparing `tmp/sphecerix-0.4.0-py3-none-any.whl.zip` & `tmp/sphecerix-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,15 @@
-Zip file size: 6952 bytes, number of entries: 9
--rw-r--r--  2.0 unx      296 b- defN 23-Jun-21 07:21 sphecerix/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-21 07:21 sphecerix/_version.py
--rw-r--r--  2.0 unx     3394 b- defN 23-Jun-21 07:21 sphecerix/atomic_wave_functions.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Jun-21 07:21 sphecerix/tesseral.py
--rw-r--r--  2.0 unx    10070 b- defN 23-Jun-21 07:21 sphecerix/wignerd.py
--rw-r--r--  2.0 unx     2873 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      706 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/RECORD
-9 files, 18682 bytes uncompressed, 5740 bytes compressed:  69.3%
+Zip file size: 10968 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      465 b- defN 23-Jun-29 06:23 sphecerix/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 06:23 sphecerix/_version.py
+-rw-r--r--  2.0 unx     3394 b- defN 23-Jun-29 06:23 sphecerix/atomic_wave_functions.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jun-29 06:23 sphecerix/basis_functions.py
+-rw-r--r--  2.0 unx     3334 b- defN 23-Jun-29 06:23 sphecerix/matrixplot.py
+-rw-r--r--  2.0 unx     1437 b- defN 23-Jun-29 06:23 sphecerix/molecule.py
+-rw-r--r--  2.0 unx     5268 b- defN 23-Jun-29 06:23 sphecerix/symmetry_operations.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-29 06:23 sphecerix/tesseral.py
+-rw-r--r--  2.0 unx    10070 b- defN 23-Jun-29 06:23 sphecerix/wignerd.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-Jun-29 06:23 sphecerix-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 06:23 sphecerix-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-29 06:23 sphecerix-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1037 b- defN 23-Jun-29 06:23 sphecerix-0.5.0.dist-info/RECORD
+13 files, 29843 bytes uncompressed, 9244 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -3,26 +3,38 @@
 
 Filename: sphecerix/_version.py
 Comment: 
 
 Filename: sphecerix/atomic_wave_functions.py
 Comment: 
 
+Filename: sphecerix/basis_functions.py
+Comment: 
+
+Filename: sphecerix/matrixplot.py
+Comment: 
+
+Filename: sphecerix/molecule.py
+Comment: 
+
+Filename: sphecerix/symmetry_operations.py
+Comment: 
+
 Filename: sphecerix/tesseral.py
 Comment: 
 
 Filename: sphecerix/wignerd.py
 Comment: 
 
-Filename: sphecerix-0.4.0.dist-info/METADATA
+Filename: sphecerix-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: sphecerix-0.4.0.dist-info/WHEEL
+Filename: sphecerix-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: sphecerix-0.4.0.dist-info/top_level.txt
+Filename: sphecerix-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sphecerix-0.4.0.dist-info/RECORD
+Filename: sphecerix-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphecerix/__init__.py

```diff
@@ -1,6 +1,10 @@
 from .wignerd import tesseral_wigner_D, wigner_D, tesseral_wigner_D_mirror,\
                      tesseral_wigner_D_improper
 from .tesseral import tesseral_transformation, permutation_sh_car
 from .atomic_wave_functions import wfcart, wf, wffield, wffield_l
+from .molecule import Molecule
+from .basis_functions import BasisFunction
+from .symmetry_operations import *
+from .matrixplot import plot_matrix, visualize_matrices
 
 from ._version import __version__
```

## sphecerix/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.4.0"
+__version__ = "0.5.0"
```

## Comparing `sphecerix-0.4.0.dist-info/METADATA` & `sphecerix-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphecerix
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package for constructing Wigner-D matrices
 Home-page: https://github.com/ifilot/sphecerix
 Author: Ivo Filot
 Author-email: ivo@ivofilot.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

## Comparing `sphecerix-0.4.0.dist-info/RECORD` & `sphecerix-0.5.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-sphecerix/__init__.py,sha256=UpaZf6WK-slXc0Lpk5bFZt5yMVkuthEvdZ9eV_YCWok,296
-sphecerix/_version.py,sha256=1NSg4yHgqJJKYBklxFwmel_5eSNX51umiqsyFgx4770,21
+sphecerix/__init__.py,sha256=YZIcwUey32dAJRDfZAXmF1fCDytAPl4qe28FYFG98yw,465
+sphecerix/_version.py,sha256=pVYhOkVS5PHJd_cIEx6PTaY6VggXFTC3pqWdf0I8zao,21
 sphecerix/atomic_wave_functions.py,sha256=VO9_8spYmPvTbRncdG9aPMzjkA3qFTj6jUTJIsOyER0,3394
+sphecerix/basis_functions.py,sha256=MZSVGxvNliCJnhXWKi9YEVQNgUfFeavlvPK7cGukAx8,622
+sphecerix/matrixplot.py,sha256=sUgfo3etu9y5yAssSZwVcI_S-Q9XlDovvQMTgA1mX_8,3334
+sphecerix/molecule.py,sha256=HTSnaNntDLBlksKJ9dgaaNKpS331GnAfu_SZ5KR-Lvo,1437
+sphecerix/symmetry_operations.py,sha256=ayG_-3UdZKIBT4Qod2sN9PKgG8_ILYiOjpBxfdB6IJI,5268
 sphecerix/tesseral.py,sha256=7ak1E_tsT5IMavEVyNqaNtY64jUdfuecl8IZr2M9Rfc,1220
 sphecerix/wignerd.py,sha256=zxRNofxD_PG4fjsD91SlScWSVanRS4Cv9VtEgqn0PN0,10070
-sphecerix-0.4.0.dist-info/METADATA,sha256=DaRut1SQa0i9IzcsNKht_WvMQagLenQL93ofoOcUZ4I,2873
-sphecerix-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sphecerix-0.4.0.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
-sphecerix-0.4.0.dist-info/RECORD,,
+sphecerix-0.5.0.dist-info/METADATA,sha256=H9_M-O821fE05m-53qKEULSigR9tC9aWxDMy_LfeX7I,2873
+sphecerix-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sphecerix-0.5.0.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
+sphecerix-0.5.0.dist-info/RECORD,,
```

