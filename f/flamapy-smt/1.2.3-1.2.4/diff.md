# Comparing `tmp/flamapy-smt-1.2.3.tar.gz` & `tmp/flamapy-smt-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-smt-1.2.3.tar", last modified: Sat Apr 22 14:43:15 2023, max compression
+gzip compressed data, was "flamapy-smt-1.2.4.tar", last modified: Thu Jun 29 12:14:41 2023, max compression
```

## Comparing `flamapy-smt-1.2.3.tar` & `flamapy-smt-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/models/pysmt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/complete_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/filter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/number_of_products.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/valid_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/valid_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/transformations/graph_to_smt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy_smt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/models/pysmt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/complete_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/filter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/number_of_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/valid_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/valid_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/transformations/graph_to_smt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/flamapy_smt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-29 12:14:41.000000 flamapy-smt-1.2.4/flamapy_smt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-29 12:14:41.000000 flamapy-smt-1.2.4/flamapy_smt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:14:41.000000 flamapy-smt-1.2.4/flamapy_smt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 12:14:41.000000 flamapy-smt-1.2.4/flamapy_smt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 12:14:41.000000 flamapy-smt-1.2.4/flamapy_smt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:14:41.285000 flamapy-smt-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 12:14:29.000000 flamapy-smt-1.2.4/setup.py
```

### Comparing `flamapy-smt-1.2.3/LICENSE.md` & `flamapy-smt-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/PKG-INFO` & `flamapy-smt-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-smt
-Version: 1.2.3
+Version: 1.2.4
 Summary: This repo host the SMT model concrete classes
 Home-page: https://github.com/flamapy/smt_metamodel
 Author: Antonio Germán Márquez Trujillo
 Author-email: amtrujillo@us.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/__init__.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/complete_config.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/complete_config.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/filter_configs.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/filter_configs.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/number_of_products.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/number_of_products.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/valid_config.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/operations/valid_config.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py` & `flamapy-smt-1.2.4/flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/flamapy_smt.egg-info/PKG-INFO` & `flamapy-smt-1.2.4/flamapy_smt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-smt
-Version: 1.2.3
+Version: 1.2.4
 Summary: This repo host the SMT model concrete classes
 Home-page: https://github.com/flamapy/smt_metamodel
 Author: Antonio Germán Márquez Trujillo
 Author-email: amtrujillo@us.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `flamapy-smt-1.2.3/flamapy_smt.egg-info/SOURCES.txt` & `flamapy-smt-1.2.4/flamapy_smt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.3/setup.py` & `flamapy-smt-1.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='flamapy-smt',
-    version='1.2.3',
+    version='1.2.4',
     author='Antonio Germán Márquez Trujillo',
     author_email='amtrujillo@us.es',
     description='This repo host the SMT model concrete classes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/flamapy/smt_metamodel',
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.10',
     install_requires=[
-        'z3-solver==4.12.1.0',
-        'flamapy==1.0.1'
+        'z3-solver==4.12.2.0',
+        'flamapy==1.1.3'
     ],
     tests_requires=[
-        'prospector[with_everything]==1.8.3',
+        'prospector[with_everything]==1.10.2',
         'mypy==0.982',
-        'types-setuptools==67.6.0.8'
+        'types-setuptools==68.0.0.0'
     ]
 )
```

