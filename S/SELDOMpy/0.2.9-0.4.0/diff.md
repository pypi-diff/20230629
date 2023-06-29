# Comparing `tmp/SELDOMpy-0.2.9.tar.gz` & `tmp/SELDOMpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.2.9.tar", last modified: Thu Jun 29 07:35:33 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.4.0.tar", last modified: Thu Jun 29 07:38:06 2023, max compression
```

## Comparing `SELDOMpy-0.2.9.tar` & `SELDOMpy-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:35:33.741650 SELDOMpy-0.2.9/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0      641 2023-06-29 07:35:33.741650 SELDOMpy-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 07:35:33.736652 SELDOMpy-0.2.9/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-28 11:33:29.000000 SELDOMpy-0.2.9/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:35:33.740651 SELDOMpy-0.2.9/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.2.9/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.2.9/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.2.9/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.2.9/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.2.9/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.2.9/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.2.9/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.2.9/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.2.9/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.2.9/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.2.9/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:35:33.739651 SELDOMpy-0.2.9/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      641 2023-06-29 07:35:33.000000 SELDOMpy-0.2.9/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 07:35:33.000000 SELDOMpy-0.2.9/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:35:33.000000 SELDOMpy-0.2.9/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 07:35:33.000000 SELDOMpy-0.2.9/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 07:35:33.000000 SELDOMpy-0.2.9/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 07:35:33.742643 SELDOMpy-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1618 2023-06-29 07:35:30.000000 SELDOMpy-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.712660 SELDOMpy-0.4.0/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      641 2023-06-29 07:38:06.712660 SELDOMpy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.706627 SELDOMpy-0.4.0/SELDOMpy/
+-rw-rw-rw-   0        0        0      556 2023-06-29 07:38:02.000000 SELDOMpy-0.4.0/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.711628 SELDOMpy-0.4.0/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.4.0/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.4.0/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.4.0/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.4.0/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.4.0/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.4.0/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.710627 SELDOMpy-0.4.0/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      641 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 07:38:06.713661 SELDOMpy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1618 2023-06-29 07:38:02.000000 SELDOMpy-0.4.0/setup.py
```

### Comparing `SELDOMpy-0.2.9/LICENSE.txt` & `SELDOMpy-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/PKG-INFO` & `SELDOMpy-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.2.9
+Version: 0.4.0
 Summary: Package for modelling cellular signalling networks
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `SELDOMpy-0.2.9/SELDOMpy/buildmim.py` & `SELDOMpy-0.4.0/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/extras.py` & `SELDOMpy-0.4.0/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/gen_exps.py` & `SELDOMpy-0.4.0/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.4.0/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.4.0/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.4.0/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/plot_results.py` & `SELDOMpy-0.4.0/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.4.0/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.4.0/SELDOMpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.2.9
+Version: 0.4.0
 Summary: Package for modelling cellular signalling networks
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `SELDOMpy-0.2.9/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.4.0/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.2.9/setup.py` & `SELDOMpy-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     return config
 
 if __name__ == "__main__":
     setup(
         name='SELDOMpy',
         packages=['SELDOMpy'],
-        version='0.2.9',
+        version='0.4.0',
         license='MIT',
         description=DESCRIPTION,
         author='Luis Prado',
         author_email='pradolopezluis@gmail.com',
         url='https://github.com/lupralo31/SELDOMpy',
         download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
         keywords=['SOME', 'MEANINGFULL', 'KEYWORDS'],
```

