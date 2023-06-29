# Comparing `tmp/SELDOMpy-0.4.0.tar.gz` & `tmp/SELDOMpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.4.0.tar", last modified: Thu Jun 29 07:38:06 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.4.2.tar", last modified: Thu Jun 29 07:56:07 2023, max compression
```

## Comparing `SELDOMpy-0.4.0.tar` & `SELDOMpy-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.712660 SELDOMpy-0.4.0/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0      641 2023-06-29 07:38:06.712660 SELDOMpy-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.706627 SELDOMpy-0.4.0/SELDOMpy/
--rw-rw-rw-   0        0        0      556 2023-06-29 07:38:02.000000 SELDOMpy-0.4.0/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.711628 SELDOMpy-0.4.0/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.4.0/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.4.0/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.4.0/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.4.0/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.4.0/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.4.0/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:38:06.710627 SELDOMpy-0.4.0/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      641 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 07:38:06.000000 SELDOMpy-0.4.0/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 07:38:06.713661 SELDOMpy-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1618 2023-06-29 07:38:02.000000 SELDOMpy-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:56:07.682626 SELDOMpy-0.4.2/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      641 2023-06-29 07:56:07.683630 SELDOMpy-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:56:07.677626 SELDOMpy-0.4.2/SELDOMpy/
+-rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.4.2/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:56:07.681625 SELDOMpy-0.4.2/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.4.2/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.4.2/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.4.2/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.4.2/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.4.2/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.4.2/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.4.2/SELDOMpy/opt_mealpy.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.4.2/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.4.2/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.4.2/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.4.2/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:56:07.680626 SELDOMpy-0.4.2/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      641 2023-06-29 07:56:07.000000 SELDOMpy-0.4.2/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-06-29 07:56:07.000000 SELDOMpy-0.4.2/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:56:07.000000 SELDOMpy-0.4.2/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 07:56:07.000000 SELDOMpy-0.4.2/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 07:56:07.000000 SELDOMpy-0.4.2/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 07:56:07.683630 SELDOMpy-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-06-29 07:55:52.000000 SELDOMpy-0.4.2/setup.py
```

### Comparing `SELDOMpy-0.4.0/LICENSE.txt` & `SELDOMpy-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/PKG-INFO` & `SELDOMpy-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.4.0
+Version: 0.4.2
 Summary: Package for modelling cellular signalling networks
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `SELDOMpy-0.4.0/SELDOMpy/buildmim.py` & `SELDOMpy-0.4.2/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/extras.py` & `SELDOMpy-0.4.2/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/gen_exps.py` & `SELDOMpy-0.4.2/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.4.2/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.4.2/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.4.2/SELDOMpy/opt_mealpy.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/plot_results.py` & `SELDOMpy-0.4.2/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.4.2/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.4.2/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.4.2/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.4.2/SELDOMpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.4.0
+Version: 0.4.2
 Summary: Package for modelling cellular signalling networks
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `SELDOMpy-0.4.0/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.4.2/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.4.0/setup.py` & `SELDOMpy-0.4.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from distutils.core import setup, Extension
 import glob
 import os
 
 DESCRIPTION = 'Package for modelling cellular signalling networks'
 
-def configuration(parent_package='', top_path=None):
-    from numpy.distutils.misc_util import Configuration
-    from numpy.distutils.misc_util import get_info
-
-    # Necessary for the half-float d-type.
-    info = get_info('npymath')
-
-    config = Configuration('',
-                           parent_package,
-                           top_path)
-    config.add_extension('hello', sources=glob.glob(os.path.join(os.getcwd(), 'src', '*.c')), **info)
-    config.add_include_dirs(['include/include_amigo', 'include/include_cvodes'])
-
-    return config
-
-if __name__ == "__main__":
-    setup(
-        name='SELDOMpy',
-        packages=['SELDOMpy'],
-        version='0.4.0',
-        license='MIT',
-        description=DESCRIPTION,
-        author='Luis Prado',
-        author_email='pradolopezluis@gmail.com',
-        url='https://github.com/lupralo31/SELDOMpy',
-        download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
-        keywords=['SOME', 'MEANINGFULL', 'KEYWORDS'],
-        install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "setuptools"],
-        classifiers=[
-            'Development Status :: 3 - Alpha',
-            'Intended Audience :: Developers',
-            'Topic :: Software Development :: Build Tools',
-            'License :: OSI Approved :: MIT License',
-            'Programming Language :: Python :: 3.8',
-        ],
-        **configuration().todict()
-    )
+hello_module = Extension(
+    'SELDOMpy.hello',  # Nombre del módulo
+    sources=['src/*.c'],  # Lista de archivos fuente (.c)
+    include_dirs=['include/include_amigo', 'include/include_cvodes'],  # Lista de directorios de inclusión
+    define_macros=[],  # Macros de compilación opcionales
+    undef_macros=[],  # Macros de compilación para deshabilitar
+    library_dirs=[],  # Directorios de búsqueda de bibliotecas
+    libraries=[],  # Bibliotecas a enlazar
+)
+
+setup(
+    name='SELDOMpy',
+    packages=['SELDOMpy'],
+    version='0.4.2',
+    license='MIT',
+    description=DESCRIPTION,
+    author='Luis Prado',
+    author_email='pradolopezluis@gmail.com',
+    url='https://github.com/lupralo31/SELDOMpy',
+    download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
+    keywords=['SOME', 'MEANINGFULL', 'KEYWORDS'],
+    install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "setuptools"],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.8',
+    ],
+    ext_modules=[hello_module],  # Agregar el módulo "hello" como extensión
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

