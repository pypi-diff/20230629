# Comparing `tmp/SELDOMpy-0.2.2.tar.gz` & `tmp/SELDOMpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.2.2.tar", last modified: Wed Jun 28 14:09:43 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.2.3.tar", last modified: Thu Jun 29 06:41:07 2023, max compression
```

## Comparing `SELDOMpy-0.2.2.tar` & `SELDOMpy-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 14:09:43.678941 SELDOMpy-0.2.2/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      641 2023-06-28 14:09:43.678941 SELDOMpy-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 14:09:43.673939 SELDOMpy-0.2.2/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-28 11:33:29.000000 SELDOMpy-0.2.2/SELDOMpy/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.2.2/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.2.2/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.2.2/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.2.2/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.2.2/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.2.2/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.2.2/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.2.2/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.2.2/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.2.2/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:09:43.677941 SELDOMpy-0.2.2/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      641 2023-06-28 14:09:43.000000 SELDOMpy-0.2.2/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-06-28 14:09:43.000000 SELDOMpy-0.2.2/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 14:09:43.000000 SELDOMpy-0.2.2/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-28 14:09:43.000000 SELDOMpy-0.2.2/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 14:09:43.000000 SELDOMpy-0.2.2/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-28 14:09:43.679941 SELDOMpy-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1563 2023-06-28 14:08:25.000000 SELDOMpy-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:41:07.474983 SELDOMpy-0.2.3/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      641 2023-06-29 06:41:07.475982 SELDOMpy-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 06:41:07.471982 SELDOMpy-0.2.3/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-28 11:33:29.000000 SELDOMpy-0.2.3/SELDOMpy/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.2.3/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.2.3/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.2.3/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.2.3/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.2.3/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.2.3/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.2.3/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.2.3/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.2.3/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.2.3/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:41:07.474983 SELDOMpy-0.2.3/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      641 2023-06-29 06:41:07.000000 SELDOMpy-0.2.3/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-06-29 06:41:07.000000 SELDOMpy-0.2.3/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:41:07.000000 SELDOMpy-0.2.3/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 06:41:07.000000 SELDOMpy-0.2.3/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 06:41:07.000000 SELDOMpy-0.2.3/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 06:41:07.475982 SELDOMpy-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2470 2023-06-29 06:41:04.000000 SELDOMpy-0.2.3/setup.py
```

### Comparing `SELDOMpy-0.2.2/LICENSE.txt` & `SELDOMpy-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/PKG-INFO` & `SELDOMpy-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package for modelling cellular signalling networks
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `SELDOMpy-0.2.2/SELDOMpy/buildmim.py` & `SELDOMpy-0.2.3/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/extras.py` & `SELDOMpy-0.2.3/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/gen_exps.py` & `SELDOMpy-0.2.3/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.2.3/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.2.3/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.2.3/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/plot_results.py` & `SELDOMpy-0.2.3/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.2.3/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.2.3/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.2.3/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.2/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.2.3/SELDOMpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package for modelling cellular signalling networks
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

