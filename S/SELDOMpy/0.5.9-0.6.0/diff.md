# Comparing `tmp/SELDOMpy-0.5.9.tar.gz` & `tmp/SELDOMpy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.5.9.tar", last modified: Thu Jun 29 15:50:05 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.6.0.tar", last modified: Thu Jun 29 15:58:39 2023, max compression
```

## Comparing `SELDOMpy-0.5.9.tar` & `SELDOMpy-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:50:05.523203 SELDOMpy-0.5.9/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.5.9/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2023-06-29 15:50:05.523203 SELDOMpy-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 15:50:05.507199 SELDOMpy-0.5.9/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.5.9/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:50:05.522201 SELDOMpy-0.5.9/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.5.9/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.5.9/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.5.9/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.5.9/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.5.9/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.5.9/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.5.9/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.5.9/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.5.9/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.5.9/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.5.9/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:50:05.520188 SELDOMpy-0.5.9/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-29 15:50:05.000000 SELDOMpy-0.5.9/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 15:50:05.000000 SELDOMpy-0.5.9/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:50:05.000000 SELDOMpy-0.5.9/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 15:50:05.000000 SELDOMpy-0.5.9/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 15:50:05.000000 SELDOMpy-0.5.9/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 15:50:05.524202 SELDOMpy-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1487 2023-06-29 15:49:57.000000 SELDOMpy-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.123562 SELDOMpy-0.6.0/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2023-06-29 15:58:39.124573 SELDOMpy-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.114563 SELDOMpy-0.6.0/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.6.0/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.121585 SELDOMpy-0.6.0/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.0/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.0/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.0/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.0/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.0/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.0/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.120567 SELDOMpy-0.6.0/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      141 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-29 15:58:39.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 15:58:39.125621 SELDOMpy-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1451 2023-06-29 15:58:31.000000 SELDOMpy-0.6.0/setup.py
```

### Comparing `SELDOMpy-0.5.9/LICENSE.txt` & `SELDOMpy-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/buildmim.py` & `SELDOMpy-0.6.0/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/extras.py` & `SELDOMpy-0.6.0/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/gen_exps.py` & `SELDOMpy-0.6.0/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.6.0/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.6.0/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.6.0/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/plot_results.py` & `SELDOMpy-0.6.0/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.6.0/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.6.0/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.5.9/setup.py` & `SELDOMpy-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 else:
     #    extra += ['-O2']
     if USE_OPENMP:
         libs += ['gomp']
         extra += ['-fopenmp']
 
 hello = Extension(name="hello",
-                  sources=["SELDOMpy/src/*.c"],
+                  sources=["src/*.c"],
                   libraries=libs,
-                  include_dirs=['SELDOMpy/include/include_amigo', 'SELDOMpy/include/include_cvodes'],
-                  library_dirs=["SELDOMpy/src"],
+                  include_dirs=['include/include_amigo', 'include/include_cvodes'],
+                  library_dirs=["src"],
                   extra_compile_args=extra
                   )
 
 setup(name="SELDOMpy",
       description="Code for xQML",
       author="S. Vanneste & M. Tristram",
-      version="0.5.9",
+      version="0.6.0",
       packages=['SELDOMpy'],
       ext_modules=[hello],
       install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "Cython"],
       cmdclass={'build_ext': build_ext}
       )
```

