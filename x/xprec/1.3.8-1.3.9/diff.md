# Comparing `tmp/xprec-1.3.8.tar.gz` & `tmp/xprec-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xprec-1.3.8.tar", last modified: Tue Mar  7 16:23:58 2023, max compression
+gzip compressed data, was "xprec-1.3.9.tar", last modified: Thu Jun 29 13:09:33 2023, max compression
```

## Comparing `xprec-1.3.8.tar` & `xprec-1.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:58.461212 xprec-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-07 16:23:55.000000 xprec-1.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-07 16:23:58.461212 xprec-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-07 16:23:55.000000 xprec-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:58.461212 xprec-1.3.8/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-03-07 16:23:55.000000 xprec-1.3.8/csrc/_dd_linalg.c
--rw-r--r--   0 runner    (1001) docker     (123)    41239 2023-03-07 16:23:55.000000 xprec-1.3.8/csrc/_dd_ufunc.c
--rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-03-07 16:23:55.000000 xprec-1.3.8/csrc/dd_arith.c
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-03-07 16:23:55.000000 xprec-1.3.8/csrc/dd_arith.h
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-03-07 16:23:55.000000 xprec-1.3.8/csrc/dd_linalg.c
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-07 16:23:55.000000 xprec-1.3.8/csrc/dd_linalg.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:58.457212 xprec-1.3.8/pysrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:58.461212 xprec-1.3.8/pysrc/xprec/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-07 16:23:55.000000 xprec-1.3.8/pysrc/xprec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-03-07 16:23:55.000000 xprec-1.3.8/pysrc/xprec/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:58.461212 xprec-1.3.8/pysrc/xprec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-07 16:23:58.000000 xprec-1.3.8/pysrc/xprec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-07 16:23:58.000000 xprec-1.3.8/pysrc/xprec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 16:23:58.000000 xprec-1.3.8/pysrc/xprec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-07 16:23:58.000000 xprec-1.3.8/pysrc/xprec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-07 16:23:58.000000 xprec-1.3.8/pysrc/xprec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 16:23:58.461212 xprec-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-03-07 16:23:55.000000 xprec-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:23:58.461212 xprec-1.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-07 16:23:55.000000 xprec-1.3.8/test/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-07 16:23:55.000000 xprec-1.3.8/test/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-07 16:23:55.000000 xprec-1.3.8/test/test_mpmath.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-07 16:23:55.000000 xprec-1.3.8/test/test_ufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-07 16:23:55.000000 xprec-1.3.8/test/test_whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:33.312908 xprec-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 13:09:27.000000 xprec-1.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 13:09:33.312908 xprec-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-29 13:09:27.000000 xprec-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:33.312908 xprec-1.3.9/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-06-29 13:09:27.000000 xprec-1.3.9/csrc/_dd_linalg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41239 2023-06-29 13:09:27.000000 xprec-1.3.9/csrc/_dd_ufunc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-06-29 13:09:27.000000 xprec-1.3.9/csrc/dd_arith.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-06-29 13:09:27.000000 xprec-1.3.9/csrc/dd_arith.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-29 13:09:27.000000 xprec-1.3.9/csrc/dd_linalg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-29 13:09:27.000000 xprec-1.3.9/csrc/dd_linalg.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:33.308908 xprec-1.3.9/pysrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:33.312908 xprec-1.3.9/pysrc/xprec/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-29 13:09:27.000000 xprec-1.3.9/pysrc/xprec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-29 13:09:27.000000 xprec-1.3.9/pysrc/xprec/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:33.312908 xprec-1.3.9/pysrc/xprec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 13:09:33.000000 xprec-1.3.9/pysrc/xprec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-29 13:09:33.000000 xprec-1.3.9/pysrc/xprec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:09:33.000000 xprec-1.3.9/pysrc/xprec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 13:09:33.000000 xprec-1.3.9/pysrc/xprec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:09:33.000000 xprec-1.3.9/pysrc/xprec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:09:33.312908 xprec-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-29 13:09:27.000000 xprec-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:33.312908 xprec-1.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 13:09:27.000000 xprec-1.3.9/test/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-29 13:09:27.000000 xprec-1.3.9/test/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-29 13:09:27.000000 xprec-1.3.9/test/test_mpmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-29 13:09:27.000000 xprec-1.3.9/test/test_ufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-29 13:09:27.000000 xprec-1.3.9/test/test_whitespace.py
```

### Comparing `xprec-1.3.8/LICENSE.txt` & `xprec-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/PKG-INFO` & `xprec-1.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xprec
-Version: 1.3.8
+Version: 1.3.9
 Summary: xprec precision numpy extension
 Home-page: https://github.com/tuwien-cms/xprec
 Author: Markus Wallerberger
 Author-email: markus.wallerberger@tuwien.ac.at
 License: UNKNOWN
 Keywords: double-double
 Platform: UNKNOWN
@@ -48,14 +48,24 @@
     z = np.sin(x)
 
     # do some linalg
     import xprec.linalg
     A = np.vander(np.linspace(-1, 1, 80, dtype=ddouble), 150)
     U, s, VT = xprec.linalg.svd(A)
 
+Trouble shooting
+---
+
+* icc<br>
+You may suffer from a long runtime when xprec is built with icc. If you encounter this problem, please try the following:
+
+```
+CFLAGS="-fp-model=precise" pip install xprec
+```
+
 Licence
 -------
 The xprec library is
 Copyright (C) 2021 Markus Wallerberger.
 Licensed under the MIT license (see LICENSE.txt).
 
 Contains code from the QD library, which is
```

### Comparing `xprec-1.3.8/csrc/_dd_linalg.c` & `xprec-1.3.9/csrc/_dd_linalg.c`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/csrc/_dd_ufunc.c` & `xprec-1.3.9/csrc/_dd_ufunc.c`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/csrc/dd_arith.c` & `xprec-1.3.9/csrc/dd_arith.c`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/csrc/dd_arith.h` & `xprec-1.3.9/csrc/dd_arith.h`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/csrc/dd_linalg.c` & `xprec-1.3.9/csrc/dd_linalg.c`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/csrc/dd_linalg.h` & `xprec-1.3.9/csrc/dd_linalg.h`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/pysrc/xprec/__init__.py` & `xprec-1.3.9/pysrc/xprec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     import numpy as np
     from xprec import ddouble
 
     x = np.arange(5, dtype=ddouble)
     print(2 * x)
 
 """
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 import numpy as _np
 
 from . import _dd_ufunc
 from . import _dd_linalg    # needed for matmul
 
 ddouble = _dd_ufunc.dtype
```

### Comparing `xprec-1.3.8/pysrc/xprec/linalg.py` & `xprec-1.3.9/pysrc/xprec/linalg.py`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/pysrc/xprec.egg-info/PKG-INFO` & `xprec-1.3.9/pysrc/xprec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xprec
-Version: 1.3.8
+Version: 1.3.9
 Summary: xprec precision numpy extension
 Home-page: https://github.com/tuwien-cms/xprec
 Author: Markus Wallerberger
 Author-email: markus.wallerberger@tuwien.ac.at
 License: UNKNOWN
 Keywords: double-double
 Platform: UNKNOWN
@@ -48,14 +48,24 @@
     z = np.sin(x)
 
     # do some linalg
     import xprec.linalg
     A = np.vander(np.linspace(-1, 1, 80, dtype=ddouble), 150)
     U, s, VT = xprec.linalg.svd(A)
 
+Trouble shooting
+---
+
+* icc<br>
+You may suffer from a long runtime when xprec is built with icc. If you encounter this problem, please try the following:
+
+```
+CFLAGS="-fp-model=precise" pip install xprec
+```
+
 Licence
 -------
 The xprec library is
 Copyright (C) 2021 Markus Wallerberger.
 Licensed under the MIT license (see LICENSE.txt).
 
 Contains code from the QD library, which is
```

### Comparing `xprec-1.3.8/setup.py` & `xprec-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/test/test_dtype.py` & `xprec-1.3.9/test/test_dtype.py`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/test/test_linalg.py` & `xprec-1.3.9/test/test_linalg.py`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/test/test_mpmath.py` & `xprec-1.3.9/test/test_mpmath.py`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/test/test_ufunc.py` & `xprec-1.3.9/test/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `xprec-1.3.8/test/test_whitespace.py` & `xprec-1.3.9/test/test_whitespace.py`

 * *Files identical despite different names*

