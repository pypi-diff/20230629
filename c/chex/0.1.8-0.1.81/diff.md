# Comparing `tmp/chex-0.1.8.tar.gz` & `tmp/chex-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chex-0.1.8.tar", last modified: Tue Jun 27 13:15:17 2023, max compression
+gzip compressed data, was "chex-0.1.81.tar", last modified: Thu Jun 29 10:59:31 2023, max compression
```

## Comparing `chex-0.1.8.tar` & `chex-0.1.81.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 13:15:05.000000 chex-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-27 13:15:05.000000 chex-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-27 13:15:17.489947 chex-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-06-27 13:15:05.000000 chex-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.485947 chex-0.1.8/chex/
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-27 13:15:05.000000 chex-0.1.8/chex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/chex/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64909 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_chexify.py
--rw-r--r--   0 runner    (1001) docker     (123)    23171 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_chexify_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_internal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    73097 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/asserts_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dataclass_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/dimensions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/fake_set_n_cpu_devices_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/restrict_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/restrict_backends_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-27 13:15:05.000000 chex-0.1.8/chex/_src/variants_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 13:15:05.000000 chex-0.1.8/chex/chex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:05.000000 chex-0.1.8/chex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/chex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 13:15:17.000000 chex-0.1.8/chex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:15:17.489947 chex-0.1.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 13:15:05.000000 chex-0.1.8/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 13:15:05.000000 chex-0.1.8/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:15:05.000000 chex-0.1.8/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:15:17.489947 chex-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-27 13:15:05.000000 chex-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.849064 chex-0.1.81/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 10:59:21.000000 chex-0.1.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 10:59:21.000000 chex-0.1.81/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-06-29 10:59:31.849064 chex-0.1.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-06-29 10:59:21.000000 chex-0.1.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.841064 chex-0.1.81/chex/
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-29 10:59:21.000000 chex-0.1.81/chex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.849064 chex-0.1.81/chex/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64909 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_chexify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23171 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_chexify_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_internal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73097 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/asserts_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dataclass_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/dimensions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/fake_set_n_cpu_devices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/restrict_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/restrict_backends_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20448 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-29 10:59:21.000000 chex-0.1.81/chex/_src/variants_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-29 10:59:21.000000 chex-0.1.81/chex/chex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:21.000000 chex-0.1.81/chex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.841064 chex-0.1.81/chex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 10:59:31.000000 chex-0.1.81/chex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:59:31.849064 chex-0.1.81/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 10:59:21.000000 chex-0.1.81/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 10:59:21.000000 chex-0.1.81/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 10:59:21.000000 chex-0.1.81/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:59:31.849064 chex-0.1.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-29 10:59:21.000000 chex-0.1.81/setup.py
```

### Comparing `chex-0.1.8/LICENSE` & `chex-0.1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/PKG-INFO` & `chex-0.1.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chex
-Version: 0.1.8
+Version: 0.1.81
 Summary: Chex: Testing made fun, in JAX!
 Home-page: https://github.com/deepmind/chex
 Author: DeepMind
 Author-email: chex-dev@google.com
 License: Apache 2.0
 Keywords: jax testing debugging python machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chex-0.1.8/README.md` & `chex-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/__init__.py` & `chex-0.1.81/chex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 from chex._src.variants import all_variants
 from chex._src.variants import ChexVariantType
 from chex._src.variants import params_product
 from chex._src.variants import TestCase
 from chex._src.variants import variants
 
 
-__version__ = "0.1.8"
+__version__ = "0.1.81"
 
 __all__ = (
     "all_variants",
     "Array",
     "ArrayBatched",
     "ArrayDevice",
     "ArrayDeviceTree",
```

### Comparing `chex-0.1.8/chex/_src/__init__.py` & `chex-0.1.81/chex/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/asserts.py` & `chex-0.1.81/chex/_src/asserts.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/asserts_chexify.py` & `chex-0.1.81/chex/_src/asserts_chexify.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/asserts_chexify_test.py` & `chex-0.1.81/chex/_src/asserts_chexify_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/asserts_internal.py` & `chex-0.1.81/chex/_src/asserts_internal.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/asserts_internal_test.py` & `chex-0.1.81/chex/_src/asserts_internal_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/asserts_test.py` & `chex-0.1.81/chex/_src/asserts_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/dataclass.py` & `chex-0.1.81/chex/_src/dataclass.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/dataclass_test.py` & `chex-0.1.81/chex/_src/dataclass_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/dimensions.py` & `chex-0.1.81/chex/_src/dimensions.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/dimensions_test.py` & `chex-0.1.81/chex/_src/dimensions_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/fake.py` & `chex-0.1.81/chex/_src/fake.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/fake_set_n_cpu_devices_test.py` & `chex-0.1.81/chex/_src/fake_set_n_cpu_devices_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/fake_test.py` & `chex-0.1.81/chex/_src/fake_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/pytypes.py` & `chex-0.1.81/chex/_src/pytypes.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/restrict_backends.py` & `chex-0.1.81/chex/_src/restrict_backends.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/restrict_backends_test.py` & `chex-0.1.81/chex/_src/restrict_backends_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/variants.py` & `chex-0.1.81/chex/_src/variants.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/_src/variants_test.py` & `chex-0.1.81/chex/_src/variants_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex/chex_test.py` & `chex-0.1.81/chex/chex_test.py`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/chex.egg-info/PKG-INFO` & `chex-0.1.81/chex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chex
-Version: 0.1.8
+Version: 0.1.81
 Summary: Chex: Testing made fun, in JAX!
 Home-page: https://github.com/deepmind/chex
 Author: DeepMind
 Author-email: chex-dev@google.com
 License: Apache 2.0
 Keywords: jax testing debugging python machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chex-0.1.8/chex.egg-info/SOURCES.txt` & `chex-0.1.81/chex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chex-0.1.8/setup.py` & `chex-0.1.81/setup.py`

 * *Files identical despite different names*

