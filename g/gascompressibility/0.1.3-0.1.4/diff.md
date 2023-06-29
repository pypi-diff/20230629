# Comparing `tmp/gascompressibility-0.1.3.tar.gz` & `tmp/gascompressibility-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.1.3.tar", last modified: Thu Jun 29 01:47:03 2023, max compression
+gzip compressed data, was "dist\gascompressibility-0.1.4.tar", last modified: Thu Jun 29 15:50:54 2023, max compression
```

## Comparing `gascompressibility-0.1.3.tar` & `gascompressibility-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.385289 gascompressibility-0.1.3/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    11101 2023-06-29 01:47:03.385289 gascompressibility-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    10123 2023-06-28 22:59:44.000000 gascompressibility-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.317860 gascompressibility-0.1.3/gascompressibility/
--rw-rw-rw-   0        0        0      209 2023-06-28 22:34:59.000000 gascompressibility-0.1.3/gascompressibility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.346766 gascompressibility-0.1.3/gascompressibility/pseudocritical/
--rw-rw-rw-   0        0        0    17368 2023-06-28 22:59:09.000000 gascompressibility-0.1.3/gascompressibility/pseudocritical/Piper.py
--rw-rw-rw-   0        0        0    20360 2023-06-28 23:30:34.000000 gascompressibility-0.1.3/gascompressibility/pseudocritical/Sutton.py
--rw-rw-rw-   0        0        0       56 2023-06-28 22:59:09.000000 gascompressibility-0.1.3/gascompressibility/pseudocritical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.351765 gascompressibility-0.1.3/gascompressibility/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.3/gascompressibility/utilities/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.3/gascompressibility/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.373772 gascompressibility-0.1.3/gascompressibility/z_correlation/
--rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.3/gascompressibility/z_correlation/DAK.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.3/gascompressibility/z_correlation/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.3/gascompressibility/z_correlation/hall_yarborough.py
--rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.3/gascompressibility/z_correlation/kareem.py
--rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.3/gascompressibility/z_correlation/londono.py
--rw-rw-rw-   0        0        0     6067 2023-06-28 22:59:09.000000 gascompressibility-0.1.3/gascompressibility/z_correlation/z_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.336861 gascompressibility-0.1.3/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0    11101 2023-06-29 01:47:03.000000 gascompressibility-0.1.3/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2023-06-29 01:47:03.000000 gascompressibility-0.1.3/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 01:47:03.000000 gascompressibility-0.1.3/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-29 01:47:03.000000 gascompressibility-0.1.3/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 01:47:03.000000 gascompressibility-0.1.3/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 01:47:03.385289 gascompressibility-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1472 2023-06-29 01:47:01.000000 gascompressibility-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:47:03.384293 gascompressibility-0.1.3/tests/
--rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.3/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    11101 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10123 2023-06-28 22:59:44.000000 gascompressibility-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility/
+-rw-rw-rw-   0        0        0      209 2023-06-28 22:34:59.000000 gascompressibility-0.1.4/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0    17368 2023-06-28 22:59:09.000000 gascompressibility-0.1.4/gascompressibility/pseudocritical/Piper.py
+-rw-rw-rw-   0        0        0    20360 2023-06-28 23:30:34.000000 gascompressibility-0.1.4/gascompressibility/pseudocritical/Sutton.py
+-rw-rw-rw-   0        0        0       56 2023-06-28 22:59:09.000000 gascompressibility-0.1.4/gascompressibility/pseudocritical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.4/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.4/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0     6067 2023-06-28 22:59:09.000000 gascompressibility-0.1.4/gascompressibility/z_correlation/z_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    11101 2023-06-29 15:50:53.000000 gascompressibility-0.1.4/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:50:53.000000 gascompressibility-0.1.4/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1479 2023-06-29 15:09:03.000000 gascompressibility-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:50:54.000000 gascompressibility-0.1.4/tests/
+-rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.4/tests/test_gascomp.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `gascompressibility-0.1.3/LICENSE` & `gascompressibility-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/PKG-INFO` & `gascompressibility-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.3
+Version: 0.1.4
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.3/README.md` & `gascompressibility-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/pseudocritical/Piper.py` & `gascompressibility-0.1.4/gascompressibility/pseudocritical/Piper.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/pseudocritical/Sutton.py` & `gascompressibility-0.1.4/gascompressibility/pseudocritical/Sutton.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/z_correlation/DAK.py` & `gascompressibility-0.1.4/gascompressibility/z_correlation/DAK.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/z_correlation/hall_yarborough.py` & `gascompressibility-0.1.4/gascompressibility/z_correlation/hall_yarborough.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/z_correlation/kareem.py` & `gascompressibility-0.1.4/gascompressibility/z_correlation/kareem.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/z_correlation/londono.py` & `gascompressibility-0.1.4/gascompressibility/z_correlation/londono.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility/z_correlation/z_helper.py` & `gascompressibility-0.1.4/gascompressibility/z_correlation/z_helper.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/gascompressibility.egg-info/PKG-INFO` & `gascompressibility-0.1.4/gascompressibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.3
+Version: 0.1.4
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.1.3/gascompressibility.egg-info/SOURCES.txt` & `gascompressibility-0.1.4/gascompressibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.3/setup.py` & `gascompressibility-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,42 +17,42 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
         "notes.py",
-        "custom.svg",
         "testruns.ipynb",
         "papers",
         "docs",
         "docs_save_6_24",
     ]),
     description='GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     classifiers=classifiers(),
     license='MIT',
     author='Eric Kim',
     author_email='aegis4048@gmail.com',
     install_requires=[
-        'numpy>=1.22',
-        'scipy>=1.9.1',
-        'matplotlib>=3.5.1',
+        'numpy>=1.14',
+        'scipy>=1.5',
+        'matplotlib>=3.2.1',
     ],
     url='https://github.com/aegis4048/GasCompressibiltiy-py/tree/main',
 )
 
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload --skip-existing dist/*
 
 # python -m twine upload --skip-existing --repository testpypi dist/*
+# python setup.py install --user
```

### Comparing `gascompressibility-0.1.3/tests/test_gascomp.py` & `gascompressibility-0.1.4/tests/test_gascomp.py`

 * *Files identical despite different names*

