# Comparing `tmp/SELDOMpy-0.6.1.tar.gz` & `tmp/SELDOMpy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.6.1.tar", last modified: Thu Jun 29 16:03:10 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.6.2.tar", last modified: Thu Jun 29 16:23:20 2023, max compression
```

## Comparing `SELDOMpy-0.6.1.tar` & `SELDOMpy-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.846143 SELDOMpy-0.6.1/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.1/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2023-06-29 16:03:10.846143 SELDOMpy-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.839120 SELDOMpy-0.6.1/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.6.1/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.845144 SELDOMpy-0.6.1/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.1/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.1/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.1/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.1/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.1/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.1/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:03:10.844145 SELDOMpy-0.6.1/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 16:03:10.000000 SELDOMpy-0.6.1/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 16:03:10.847150 SELDOMpy-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-06-29 16:03:07.000000 SELDOMpy-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:23:20.832074 SELDOMpy-0.6.2/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2023-06-29 16:23:20.832074 SELDOMpy-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 16:23:20.826090 SELDOMpy-0.6.2/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.6.2/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:23:20.831075 SELDOMpy-0.6.2/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.2/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.2/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.2/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.2/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.2/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.2/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.2/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.2/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.2/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.2/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.2/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:23:20.830073 SELDOMpy-0.6.2/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      141 2023-06-29 16:23:20.000000 SELDOMpy-0.6.2/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-29 16:23:20.000000 SELDOMpy-0.6.2/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:23:20.000000 SELDOMpy-0.6.2/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 16:23:20.000000 SELDOMpy-0.6.2/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 16:23:20.000000 SELDOMpy-0.6.2/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 16:23:20.833099 SELDOMpy-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     3088 2023-06-29 16:23:18.000000 SELDOMpy-0.6.2/setup.py
```

### Comparing `SELDOMpy-0.6.1/LICENSE.txt` & `SELDOMpy-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/buildmim.py` & `SELDOMpy-0.6.2/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/extras.py` & `SELDOMpy-0.6.2/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/gen_exps.py` & `SELDOMpy-0.6.2/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.6.2/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.6.2/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.6.2/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/plot_results.py` & `SELDOMpy-0.6.2/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.6.2/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.6.2/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.6.2/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.1/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.6.2/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

