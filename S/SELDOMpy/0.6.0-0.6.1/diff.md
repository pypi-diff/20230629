# Comparing `tmp/SELDOMpy-0.6.0.tar.gz` & `tmp/SELDOMpy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.6.0.tar", last modified: Thu Jun 29 15:58:39 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.6.1.tar", last modified: Thu Jun 29 16:03:10 2023, max compression
```

## Comparing `SELDOMpy-0.6.0.tar` & `SELDOMpy-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.123562 SELDOMpy-0.6.0/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2023-06-29 15:58:39.124573 SELDOMpy-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.114563 SELDOMpy-0.6.0/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.6.0/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.121585 SELDOMpy-0.6.0/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.0/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.0/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.0/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.0/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.0/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.0/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:58:39.120567 SELDOMpy-0.6.0/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 15:58:39.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 15:58:38.000000 SELDOMpy-0.6.0/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 15:58:39.125621 SELDOMpy-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1451 2023-06-29 15:58:31.000000 SELDOMpy-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.846143 SELDOMpy-0.6.1/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2023-06-29 16:03:10.846143 SELDOMpy-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.839120 SELDOMpy-0.6.1/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.6.1/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.845144 SELDOMpy-0.6.1/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.1/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.1/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.1/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.1/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.1/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.1/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.844145 SELDOMpy-0.6.1/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      141 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 16:03:10.847150 SELDOMpy-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-06-29 16:03:07.000000 SELDOMpy-0.6.1/setup.py
```

### Comparing `SELDOMpy-0.6.0/LICENSE.txt` & `SELDOMpy-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/buildmim.py` & `SELDOMpy-0.6.1/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/extras.py` & `SELDOMpy-0.6.1/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/gen_exps.py` & `SELDOMpy-0.6.1/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.6.1/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.6.1/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.6.1/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/plot_results.py` & `SELDOMpy-0.6.1/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.6.1/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.6.1/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.0/setup.py` & `SELDOMpy-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 else:
     #    extra += ['-O2']
     if USE_OPENMP:
         libs += ['gomp']
         extra += ['-fopenmp']
 
 hello = Extension(name="hello",
-                  sources=["src/*.c"],
+                  sources=["src"],
                   libraries=libs,
                   include_dirs=['include/include_amigo', 'include/include_cvodes'],
                   library_dirs=["src"],
                   extra_compile_args=extra
                   )
 
 setup(name="SELDOMpy",
       description="Code for xQML",
       author="S. Vanneste & M. Tristram",
-      version="0.6.0",
+      version="0.6.1",
       packages=['SELDOMpy'],
       ext_modules=[hello],
       install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "Cython"],
       cmdclass={'build_ext': build_ext}
       )
```

