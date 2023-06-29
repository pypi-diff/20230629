# Comparing `tmp/SELDOMpy-0.5.7.tar.gz` & `tmp/SELDOMpy-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.5.7.tar", last modified: Thu Jun 29 15:40:16 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.5.8.tar", last modified: Thu Jun 29 15:42:55 2023, max compression
```

## Comparing `SELDOMpy-0.5.7.tar` & `SELDOMpy-0.5.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:40:16.465394 SELDOMpy-0.5.7/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.5.7/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2023-06-29 15:40:16.465394 SELDOMpy-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 15:40:16.459392 SELDOMpy-0.5.7/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.5.7/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:40:16.464385 SELDOMpy-0.5.7/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.5.7/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.5.7/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.5.7/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.5.7/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.5.7/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.5.7/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.5.7/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.5.7/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.5.7/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.5.7/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.5.7/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:40:16.463399 SELDOMpy-0.5.7/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-29 15:40:16.000000 SELDOMpy-0.5.7/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 15:40:16.000000 SELDOMpy-0.5.7/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:40:16.000000 SELDOMpy-0.5.7/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 15:40:16.000000 SELDOMpy-0.5.7/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 15:40:16.000000 SELDOMpy-0.5.7/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 15:40:16.466395 SELDOMpy-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-06-29 15:40:02.000000 SELDOMpy-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:42:55.184648 SELDOMpy-0.5.8/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.5.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2023-06-29 15:42:55.185655 SELDOMpy-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:42:55.178665 SELDOMpy-0.5.8/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.5.8/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:42:55.183632 SELDOMpy-0.5.8/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.5.8/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.5.8/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.5.8/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.5.8/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.5.8/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.5.8/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.5.8/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.5.8/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.5.8/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.5.8/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.5.8/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:42:55.182685 SELDOMpy-0.5.8/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      141 2023-06-29 15:42:55.000000 SELDOMpy-0.5.8/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-29 15:42:55.000000 SELDOMpy-0.5.8/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:42:55.000000 SELDOMpy-0.5.8/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 15:42:55.000000 SELDOMpy-0.5.8/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 15:42:55.000000 SELDOMpy-0.5.8/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 15:42:55.185655 SELDOMpy-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1460 2023-06-29 15:42:42.000000 SELDOMpy-0.5.8/setup.py
```

### Comparing `SELDOMpy-0.5.7/LICENSE.txt` & `SELDOMpy-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/buildmim.py` & `SELDOMpy-0.5.8/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/extras.py` & `SELDOMpy-0.5.8/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/gen_exps.py` & `SELDOMpy-0.5.8/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.5.8/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.5.8/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.5.8/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/plot_results.py` & `SELDOMpy-0.5.8/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.5.8/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.5.8/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.5.8/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.5.8/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.7/setup.py` & `SELDOMpy-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 import sys
-import numpy as np
+#import numpy as np
 from distutils.core import setup, Extension
 from Cython.Distutils import build_ext
 import glob
 import os
 
 # Get numpy include directory (works across versions)
 #numpy_include = np.get_include()
@@ -43,13 +43,13 @@
                   library_dirs=["SELDOMpy/src"],
                   extra_compile_args=extra
                   )
 
 setup(name="SELDOMpy",
       description="Code for xQML",
       author="S. Vanneste & M. Tristram",
-      version="0.5.7",
+      version="0.5.8",
       packages=['SELDOMpy'],
       ext_modules=[hello],
       install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "Cython"],
       cmdclass={'build_ext': build_ext}
       )
```

