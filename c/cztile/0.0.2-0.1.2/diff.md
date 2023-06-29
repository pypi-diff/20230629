# Comparing `tmp/cztile-0.0.2.tar.gz` & `tmp/cztile-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cztile-0.0.2.tar", last modified: Wed Apr  6 17:13:20 2022, max compression
+gzip compressed data, was "cztile-0.1.2.tar", last modified: Thu Jun 29 16:14:09 2023, max compression
```

## Comparing `cztile-0.0.2.tar` & `cztile-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-04-06 17:13:20.896283 cztile-0.0.2/
--rw-rw-rw-   0        0        0    11558 2022-04-06 17:12:40.000000 cztile-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2022-04-06 17:12:40.000000 cztile-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      192 2022-04-06 17:12:40.000000 cztile-0.0.2/NOTICE.txt
--rw-rw-rw-   0        0        0     6567 2022-04-06 17:13:20.896283 cztile-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5896 2022-04-06 17:12:40.000000 cztile-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-04-06 17:13:20.893284 cztile-0.0.2/cztile/
--rw-rw-rw-   0        0        0      771 2022-04-06 17:12:40.000000 cztile-0.0.2/cztile/__init__.py
--rw-rw-rw-   0        0        0     9056 2022-04-06 17:12:40.000000 cztile-0.0.2/cztile/fixed_total_area_strategy.py
--rw-rw-rw-   0        0        0     3707 2022-04-06 17:12:40.000000 cztile-0.0.2/cztile/tiling_strategy.py
-drwxrwxrwx   0        0        0        0 2022-04-06 17:13:20.895282 cztile-0.0.2/cztile.egg-info/
--rw-rw-rw-   0        0        0     6567 2022-04-06 17:13:20.000000 cztile-0.0.2/cztile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2022-04-06 17:13:20.000000 cztile-0.0.2/cztile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-06 17:13:20.000000 cztile-0.0.2/cztile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      482 2022-04-06 17:13:20.000000 cztile-0.0.2/cztile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-04-06 17:13:20.000000 cztile-0.0.2/cztile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1411 2022-04-06 17:13:20.897284 cztile-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3128 2022-04-06 17:12:40.000000 cztile-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:14:09.554933 cztile-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-29 16:13:11.000000 cztile-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 16:13:11.000000 cztile-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      192 2023-06-29 16:13:11.000000 cztile-0.1.2/NOTICE.txt
+-rw-rw-rw-   0        0        0     6650 2023-06-29 16:14:09.554933 cztile-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5896 2023-06-29 16:13:11.000000 cztile-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 16:14:09.554933 cztile-0.1.2/cztile/
+-rw-rw-rw-   0        0        0      771 2023-06-29 16:13:11.000000 cztile-0.1.2/cztile/__init__.py
+-rw-rw-rw-   0        0        0     9056 2023-06-29 16:13:11.000000 cztile-0.1.2/cztile/fixed_total_area_strategy.py
+-rw-rw-rw-   0        0        0     3707 2023-06-29 16:13:11.000000 cztile-0.1.2/cztile/tiling_strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:14:09.554933 cztile-0.1.2/cztile.egg-info/
+-rw-rw-rw-   0        0        0     6650 2023-06-29 16:14:09.000000 cztile-0.1.2/cztile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-29 16:14:09.000000 cztile-0.1.2/cztile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:14:09.000000 cztile-0.1.2/cztile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 16:14:09.000000 cztile-0.1.2/cztile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1399 2023-06-29 16:14:09.554933 cztile-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2493 2023-06-29 16:13:11.000000 cztile-0.1.2/setup.py
```

### Comparing `cztile-0.0.2/LICENSE.txt` & `cztile-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cztile-0.0.2/PKG-INFO` & `cztile-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: cztile
-Version: 0.0.2
+Version: 0.1.2
 Summary: A set of tiling utilities
-Home-page: UNKNOWN
 Author: Nuno Mesquita
 Author-email: nuno.mesquita@zeiss.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.6,<3.10
+Requires-Python: >3.6,<3.12
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 # cztile - Python package to simplify the process of tiling arrays
 
 This project provides simple-to-use tiling functionality for arrays. It is not linked directly to the CZI file format, but can be of use to process such images in an efficient and **tile-wise** manner, which is especially important when dealing with larger images.  
 
@@ -95,9 +93,7 @@
 
 **By using any of those examples you agree to this disclaimer.**
 
 Version: 2022.04.06
 
 Copyright (c) 2022 Carl Zeiss AG, Germany. All Rights Reserved.  
 
-
-
```

### Comparing `cztile-0.0.2/README.md` & `cztile-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cztile-0.0.2/cztile/__init__.py` & `cztile-0.1.2/cztile/__init__.py`

 * *Files identical despite different names*

### Comparing `cztile-0.0.2/cztile/fixed_total_area_strategy.py` & `cztile-0.1.2/cztile/fixed_total_area_strategy.py`

 * *Files identical despite different names*

### Comparing `cztile-0.0.2/cztile/tiling_strategy.py` & `cztile-0.1.2/cztile/tiling_strategy.py`

 * *Files identical despite different names*

### Comparing `cztile-0.0.2/cztile.egg-info/PKG-INFO` & `cztile-0.1.2/cztile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: cztile
-Version: 0.0.2
+Version: 0.1.2
 Summary: A set of tiling utilities
-Home-page: UNKNOWN
 Author: Nuno Mesquita
 Author-email: nuno.mesquita@zeiss.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.6,<3.10
+Requires-Python: >3.6,<3.12
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 # cztile - Python package to simplify the process of tiling arrays
 
 This project provides simple-to-use tiling functionality for arrays. It is not linked directly to the CZI file format, but can be of use to process such images in an efficient and **tile-wise** manner, which is especially important when dealing with larger images.  
 
@@ -95,9 +93,7 @@
 
 **By using any of those examples you agree to this disclaimer.**
 
 Version: 2022.04.06
 
 Copyright (c) 2022 Carl Zeiss AG, Germany. All Rights Reserved.  
 
-
-
```

### Comparing `cztile-0.0.2/setup.cfg` & `cztile-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -49,41 +49,40 @@
 00000300: 0a09 6d69 7373 696e 672d 7969 656c 642d  ..missing-yield-
 00000310: 646f 632c 0d0a 096d 6973 7369 6e67 2d72  doc,...missing-r
 00000320: 6574 7572 6e2d 646f 632c 0d0a 0975 6e73  eturn-doc,...uns
 00000330: 7065 6369 6669 6564 2d65 6e63 6f64 696e  pecified-encodin
 00000340: 672c 0d0a 0964 7570 6c69 6361 7465 2d63  g,...duplicate-c
 00000350: 6f64 650d 0a0d 0a5b 7079 6c69 6e74 2e6d  ode....[pylint.m
 00000360: 6573 7361 6765 735f 636f 6e74 726f 6c5d  essages_control]
-00000370: 0d0a 6469 7361 626c 6520 3d20 4330 3333  ..disable = C033
-00000380: 302c 4330 3332 362c 5230 3430 320d 0a76  0,C0326,R0402..v
-00000390: 6172 6961 626c 652d 7267 7820 3d20 5e28  ariable-rgx = ^(
-000003a0: 3f21 2e2a 285b 5f5d 295c 3129 5e28 3f3d  ?!.*([_])\1)^(?=
-000003b0: 2e7b 312c 3330 7d24 295b 612d 7a5f 5d5b  .{1,30}$)[a-z_][
-000003c0: 612d 7a30 2d39 5f5d 7b30 2c7d 240d 0a0d  a-z0-9_]{0,}$...
-000003d0: 0a5b 6d79 7079 5d0d 0a64 6973 616c 6c6f  .[mypy]..disallo
-000003e0: 775f 756e 7479 7065 645f 6465 6673 203d  w_untyped_defs =
-000003f0: 2054 7275 650d 0a64 6973 616c 6c6f 775f   True..disallow_
-00000400: 696e 636f 6d70 6c65 7465 5f64 6566 7320  incomplete_defs 
-00000410: 3d20 5472 7565 0d0a 6368 6563 6b5f 756e  = True..check_un
-00000420: 7479 7065 645f 6465 6673 203d 2054 7275  typed_defs = Tru
-00000430: 650d 0a6e 6f5f 696d 706c 6963 6974 5f6f  e..no_implicit_o
-00000440: 7074 696f 6e61 6c20 3d20 5472 7565 0d0a  ptional = True..
-00000450: 7374 7269 6374 5f6f 7074 696f 6e61 6c20  strict_optional 
-00000460: 3d20 5472 7565 0d0a 7374 7269 6374 5f65  = True..strict_e
-00000470: 7175 616c 6974 7920 3d20 5472 7565 0d0a  quality = True..
-00000480: 7761 726e 5f72 6564 756e 6461 6e74 5f63  warn_redundant_c
-00000490: 6173 7473 203d 2054 7275 650d 0a77 6172  asts = True..war
-000004a0: 6e5f 756e 7573 6564 5f69 676e 6f72 6573  n_unused_ignores
-000004b0: 203d 2054 7275 650d 0a77 6172 6e5f 7265   = True..warn_re
-000004c0: 7475 726e 5f61 6e79 203d 2054 7275 650d  turn_any = True.
-000004d0: 0a77 6172 6e5f 756e 7573 6564 5f63 6f6e  .warn_unused_con
-000004e0: 6669 6773 203d 2054 7275 650d 0a77 6172  figs = True..war
-000004f0: 6e5f 756e 7265 6163 6861 626c 6520 3d20  n_unreachable = 
-00000500: 5472 7565 0d0a 6e6f 5f69 6d70 6c69 6369  True..no_implici
-00000510: 745f 7265 6578 706f 7274 203d 2054 7275  t_reexport = Tru
-00000520: 650d 0a0d 0a5b 6d79 7079 2d73 6574 7570  e....[mypy-setup
-00000530: 746f 6f6c 735d 0d0a 6967 6e6f 7265 5f6d  tools]..ignore_m
-00000540: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
-00000550: 2054 7275 650d 0a0d 0a5b 6567 675f 696e   True....[egg_in
-00000560: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000570: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000580: 0a0d 0a                                  ...
+00000370: 0d0a 6469 7361 626c 6520 3d20 5230 3430  ..disable = R040
+00000380: 320d 0a76 6172 6961 626c 652d 7267 7820  2..variable-rgx 
+00000390: 3d20 5e28 3f21 2e2a 285b 5f5d 295c 3129  = ^(?!.*([_])\1)
+000003a0: 5e28 3f3d 2e7b 312c 3330 7d24 295b 612d  ^(?=.{1,30}$)[a-
+000003b0: 7a5f 5d5b 612d 7a30 2d39 5f5d 7b30 2c7d  z_][a-z0-9_]{0,}
+000003c0: 240d 0a0d 0a5b 6d79 7079 5d0d 0a64 6973  $....[mypy]..dis
+000003d0: 616c 6c6f 775f 756e 7479 7065 645f 6465  allow_untyped_de
+000003e0: 6673 203d 2054 7275 650d 0a64 6973 616c  fs = True..disal
+000003f0: 6c6f 775f 696e 636f 6d70 6c65 7465 5f64  low_incomplete_d
+00000400: 6566 7320 3d20 5472 7565 0d0a 6368 6563  efs = True..chec
+00000410: 6b5f 756e 7479 7065 645f 6465 6673 203d  k_untyped_defs =
+00000420: 2054 7275 650d 0a6e 6f5f 696d 706c 6963   True..no_implic
+00000430: 6974 5f6f 7074 696f 6e61 6c20 3d20 5472  it_optional = Tr
+00000440: 7565 0d0a 7374 7269 6374 5f6f 7074 696f  ue..strict_optio
+00000450: 6e61 6c20 3d20 5472 7565 0d0a 7374 7269  nal = True..stri
+00000460: 6374 5f65 7175 616c 6974 7920 3d20 5472  ct_equality = Tr
+00000470: 7565 0d0a 7761 726e 5f72 6564 756e 6461  ue..warn_redunda
+00000480: 6e74 5f63 6173 7473 203d 2054 7275 650d  nt_casts = True.
+00000490: 0a77 6172 6e5f 756e 7573 6564 5f69 676e  .warn_unused_ign
+000004a0: 6f72 6573 203d 2054 7275 650d 0a77 6172  ores = True..war
+000004b0: 6e5f 7265 7475 726e 5f61 6e79 203d 2054  n_return_any = T
+000004c0: 7275 650d 0a77 6172 6e5f 756e 7573 6564  rue..warn_unused
+000004d0: 5f63 6f6e 6669 6773 203d 2054 7275 650d  _configs = True.
+000004e0: 0a77 6172 6e5f 756e 7265 6163 6861 626c  .warn_unreachabl
+000004f0: 6520 3d20 5472 7565 0d0a 6e6f 5f69 6d70  e = True..no_imp
+00000500: 6c69 6369 745f 7265 6578 706f 7274 203d  licit_reexport =
+00000510: 2054 7275 650d 0a0d 0a5b 6d79 7079 2d73   True....[mypy-s
+00000520: 6574 7570 746f 6f6c 735d 0d0a 6967 6e6f  etuptools]..igno
+00000530: 7265 5f6d 6973 7369 6e67 5f69 6d70 6f72  re_missing_impor
+00000540: 7473 203d 2054 7275 650d 0a0d 0a5b 6567  ts = True....[eg
+00000550: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000560: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000570: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `cztile-0.0.2/setup.py` & `cztile-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,41 +2,15 @@
 from typing import List
 
 import setuptools
 
 # no external requirements of now
 requirements: List[str] = []
 
-test_requirements = [
-    "pytest",
-    "pytest-cov",
-    "pytest-timeout",
-    "mypy",
-    "types-all",
-    "pylint_runner",
-    "flake8",
-    "flake8-docstrings",
-    "flake8-bugbear",
-    "bandit",
-    "black",
-]
-
-dev_requirements = test_requirements.copy()
-
-extra_requirements = {
-    "test": test_requirements,
-    "dev": dev_requirements,
-    "all": [
-        *requirements,
-        *test_requirements,
-        *dev_requirements,
-    ],
-}
-
-VERSION = "0.0.2"
+VERSION = "0.1.2"
 
 # pylint: disable=line-too-long
 with open("README.md", "r", encoding="utf-8") as fh_read:
     long_description = fh_read.read()
 setuptools.setup(
     name="cztile",
     version=VERSION,
@@ -51,29 +25,27 @@
     packages=setuptools.find_packages(exclude=["test", "test.*"]),
     license_files=["LICENSE.txt", "NOTICE.txt"],
     # Classifiers help users find your project by categorizing it.
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Scientific/Engineering :: Image Processing",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     # Make required Python version compliant with official TF docs (https://www.tensorflow.org/install)
     # It follows: We build a pure Python wheel
     # Note that Python used to build the sources specifies the Python version of the dist (relevant during build only)
     # See https://packaging.python.org/guides/distributing-packages-using-setuptools/#pure-python-wheels for more info
     # We also restrict the code to >3.6 to:
     # - fully benefit from type annotations (See https://realpython.com/python-type-checking/ for more info)
     # - having dataclasses natively supported (starting 3.7+)
     # - + see https://realpython.com/python-data-classes/
     # - + no need to include it as ext. pkg through backport in 3.6 (dev.to/hanpari/dataclasses-in-python-3-6-29id)
-    # We also restrict the code to <3.10 since:
-    # - No source distribution support for 3.10 yet
-    # - + See https://stackoverflow.com/questions/69458399/numpy-1-21-2-may-not-yet-support-python-3-10
-    # - + See https://github.com/numpy/numpy/issues/17044
-    # - + not relevant as of today, but maybe in the future
-    python_requires=">3.6,<3.10",
+    python_requires=">3.6,<3.12",
     install_requires=requirements,
-    extras_require=extra_requirements,
 )
```

