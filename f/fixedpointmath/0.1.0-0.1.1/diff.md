# Comparing `tmp/fixedpointmath-0.1.0.tar.gz` & `tmp/fixedpointmath-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixedpointmath-0.1.0.tar", last modified: Thu Jun 29 17:06:20 2023, max compression
+gzip compressed data, was "fixedpointmath-0.1.1.tar", last modified: Thu Jun 29 18:47:36 2023, max compression
```

## Comparing `fixedpointmath-0.1.0.tar` & `fixedpointmath-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 17:06:20.778598 fixedpointmath-0.1.0/
--rw-r--r--   0 slundquist   (501) staff       (20)     2439 2023-06-29 17:06:20.778483 fixedpointmath-0.1.0/PKG-INFO
--rw-r--r--   0 slundquist   (501) staff       (20)     1793 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/README.md
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 17:06:20.777175 fixedpointmath-0.1.0/fixedpointmath/
--rw-r--r--   0 slundquist   (501) staff       (20)      503 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/fixedpointmath/__init__.py
--rw-r--r--   0 slundquist   (501) staff       (20)      213 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/fixedpointmath/errors.py
--rw-r--r--   0 slundquist   (501) staff       (20)    30490 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/fixedpointmath/fixed_point.py
--rw-r--r--   0 slundquist   (501) staff       (20)    11036 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/fixedpointmath/fixed_point_integer_math.py
--rw-r--r--   0 slundquist   (501) staff       (20)     1823 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/fixedpointmath/fixed_point_math.py
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 17:06:20.777581 fixedpointmath-0.1.0/fixedpointmath.egg-info/
--rw-r--r--   0 slundquist   (501) staff       (20)     2439 2023-06-29 17:06:20.000000 fixedpointmath-0.1.0/fixedpointmath.egg-info/PKG-INFO
--rw-r--r--   0 slundquist   (501) staff       (20)      513 2023-06-29 17:06:20.000000 fixedpointmath-0.1.0/fixedpointmath.egg-info/SOURCES.txt
--rw-r--r--   0 slundquist   (501) staff       (20)        1 2023-06-29 17:06:20.000000 fixedpointmath-0.1.0/fixedpointmath.egg-info/dependency_links.txt
--rw-r--r--   0 slundquist   (501) staff       (20)       15 2023-06-29 17:06:20.000000 fixedpointmath-0.1.0/fixedpointmath.egg-info/top_level.txt
--rw-r--r--   0 slundquist   (501) staff       (20)      826 2023-06-29 17:05:49.000000 fixedpointmath-0.1.0/pyproject.toml
--rw-r--r--   0 slundquist   (501) staff       (20)       38 2023-06-29 17:06:20.778629 fixedpointmath-0.1.0/setup.cfg
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 17:06:20.778347 fixedpointmath-0.1.0/tests/
--rw-r--r--   0 slundquist   (501) staff       (20)    23960 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/tests/test_fp_arithmetic_sugar.py
--rw-r--r--   0 slundquist   (501) staff       (20)    13308 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/tests/test_fp_class.py
--rw-r--r--   0 slundquist   (501) staff       (20)    17686 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/tests/test_fp_integer_math.py
--rw-r--r--   0 slundquist   (501) staff       (20)     4959 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/tests/test_fp_math.py
--rw-r--r--   0 slundquist   (501) staff       (20)     2281 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/tests/test_fp_nonfinite_checks.py
--rw-r--r--   0 slundquist   (501) staff       (20)     4527 2023-06-28 23:35:55.000000 fixedpointmath-0.1.0/tests/test_fp_relational_sugar.py
+drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.079268 fixedpointmath-0.1.1/
+-rw-r--r--   0 slundquist   (501) staff       (20)     2075 2023-06-29 18:47:36.079158 fixedpointmath-0.1.1/PKG-INFO
+-rw-r--r--   0 slundquist   (501) staff       (20)     1429 2023-06-29 18:44:26.000000 fixedpointmath-0.1.1/README.md
+drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.077742 fixedpointmath-0.1.1/fixedpointmath/
+-rw-r--r--   0 slundquist   (501) staff       (20)      503 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/__init__.py
+-rw-r--r--   0 slundquist   (501) staff       (20)      213 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/errors.py
+-rw-r--r--   0 slundquist   (501) staff       (20)    30490 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/fixed_point.py
+-rw-r--r--   0 slundquist   (501) staff       (20)    11036 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/fixed_point_integer_math.py
+-rw-r--r--   0 slundquist   (501) staff       (20)     1823 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/fixed_point_math.py
+drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.078171 fixedpointmath-0.1.1/fixedpointmath.egg-info/
+-rw-r--r--   0 slundquist   (501) staff       (20)     2075 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/PKG-INFO
+-rw-r--r--   0 slundquist   (501) staff       (20)      513 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/SOURCES.txt
+-rw-r--r--   0 slundquist   (501) staff       (20)        1 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/dependency_links.txt
+-rw-r--r--   0 slundquist   (501) staff       (20)       15 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/top_level.txt
+-rw-r--r--   0 slundquist   (501) staff       (20)      738 2023-06-29 18:47:24.000000 fixedpointmath-0.1.1/pyproject.toml
+-rw-r--r--   0 slundquist   (501) staff       (20)       38 2023-06-29 18:47:36.079301 fixedpointmath-0.1.1/setup.cfg
+drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.078985 fixedpointmath-0.1.1/tests/
+-rw-r--r--   0 slundquist   (501) staff       (20)    23960 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_arithmetic_sugar.py
+-rw-r--r--   0 slundquist   (501) staff       (20)    13308 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_class.py
+-rw-r--r--   0 slundquist   (501) staff       (20)    17686 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_integer_math.py
+-rw-r--r--   0 slundquist   (501) staff       (20)     4959 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_math.py
+-rw-r--r--   0 slundquist   (501) staff       (20)     2281 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_nonfinite_checks.py
+-rw-r--r--   0 slundquist   (501) staff       (20)     4527 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_relational_sugar.py
```

### Comparing `fixedpointmath-0.1.0/fixedpointmath/fixed_point.py` & `fixedpointmath-0.1.1/fixedpointmath/fixed_point.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/fixedpointmath/fixed_point_integer_math.py` & `fixedpointmath-0.1.1/fixedpointmath/fixed_point_integer_math.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/fixedpointmath/fixed_point_math.py` & `fixedpointmath-0.1.1/fixedpointmath/fixed_point_math.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/fixedpointmath.egg-info/SOURCES.txt` & `fixedpointmath-0.1.1/fixedpointmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/pyproject.toml` & `fixedpointmath-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixedpointmath"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Dylan Paiton", email = "dylan@delv.tech" },
     { name = "Mihai Cosma", email = "mihai@delv.tech" },
     { name = "Matthew Brown", email = "matt@delv.tech" },
     { name = "Sheng Lundquist", email = "sheng@delv.tech" },
 ]
 description = "Fixed-point arithmetic and type that mirrors popular Solidity implementations"
@@ -15,11 +15,7 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/delvtech/agent_0"
 "Bug Tracker" = "https://github.com/delvtech/agent_0/issues"
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
```

### Comparing `fixedpointmath-0.1.0/tests/test_fp_arithmetic_sugar.py` & `fixedpointmath-0.1.1/tests/test_fp_arithmetic_sugar.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/tests/test_fp_class.py` & `fixedpointmath-0.1.1/tests/test_fp_class.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/tests/test_fp_integer_math.py` & `fixedpointmath-0.1.1/tests/test_fp_integer_math.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/tests/test_fp_math.py` & `fixedpointmath-0.1.1/tests/test_fp_math.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/tests/test_fp_nonfinite_checks.py` & `fixedpointmath-0.1.1/tests/test_fp_nonfinite_checks.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.0/tests/test_fp_relational_sugar.py` & `fixedpointmath-0.1.1/tests/test_fp_relational_sugar.py`

 * *Files identical despite different names*

