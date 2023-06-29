# Comparing `tmp/SELDOMpy-0.2.4.tar.gz` & `tmp/SELDOMpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.2.4.tar", last modified: Thu Jun 29 06:55:34 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.2.5.tar", last modified: Thu Jun 29 07:08:41 2023, max compression
```

## Comparing `SELDOMpy-0.2.4.tar` & `SELDOMpy-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:55:34.633983 SELDOMpy-0.2.4/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      394 2023-06-29 06:55:34.633983 SELDOMpy-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 06:55:34.627983 SELDOMpy-0.2.4/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-28 11:33:29.000000 SELDOMpy-0.2.4/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:55:34.633013 SELDOMpy-0.2.4/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.2.4/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.2.4/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.2.4/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.2.4/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.2.4/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.2.4/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.2.4/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.2.4/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.2.4/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.2.4/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.2.4/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:55:34.631983 SELDOMpy-0.2.4/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      394 2023-06-29 06:55:34.000000 SELDOMpy-0.2.4/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 06:55:34.000000 SELDOMpy-0.2.4/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:55:34.000000 SELDOMpy-0.2.4/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 06:55:34.000000 SELDOMpy-0.2.4/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 06:55:34.000000 SELDOMpy-0.2.4/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 06:55:34.635019 SELDOMpy-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-06-29 06:55:31.000000 SELDOMpy-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:08:41.100660 SELDOMpy-0.2.5/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       82 2023-06-29 07:08:41.100660 SELDOMpy-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:08:41.095625 SELDOMpy-0.2.5/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-28 11:33:29.000000 SELDOMpy-0.2.5/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:08:41.099659 SELDOMpy-0.2.5/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.2.5/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.2.5/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.2.5/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.2.5/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.2.5/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.2.5/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.2.5/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.2.5/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.2.5/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.2.5/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.2.5/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:08:41.098628 SELDOMpy-0.2.5/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0       82 2023-06-29 07:08:40.000000 SELDOMpy-0.2.5/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-29 07:08:41.000000 SELDOMpy-0.2.5/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:08:40.000000 SELDOMpy-0.2.5/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 07:08:40.000000 SELDOMpy-0.2.5/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 07:08:41.101628 SELDOMpy-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-06-29 07:08:37.000000 SELDOMpy-0.2.5/setup.py
```

### Comparing `SELDOMpy-0.2.4/LICENSE.txt` & `SELDOMpy-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/buildmim.py` & `SELDOMpy-0.2.5/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/extras.py` & `SELDOMpy-0.2.5/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/gen_exps.py` & `SELDOMpy-0.2.5/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.2.5/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.2.5/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.2.5/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/plot_results.py` & `SELDOMpy-0.2.5/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.2.5/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.2.5/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.4/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.2.5/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

