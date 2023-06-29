# Comparing `tmp/fhir_analyzer-0.0.2.tar.gz` & `tmp/fhir_analyzer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_analyzer-0.0.2.tar", last modified: Thu Jun 29 14:47:56 2023, max compression
+gzip compressed data, was "fhir_analyzer-0.0.3.tar", last modified: Thu Jun 29 15:03:37 2023, max compression
```

## Comparing `fhir_analyzer-0.0.2.tar` & `fhir_analyzer-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 14:47:56.526715 fhir_analyzer-0.0.2/
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.2/LICENSE
--rw-r--r--   0 tillrostalski   (501) staff       (20)      458 2023-06-29 14:47:56.526586 fhir_analyzer-0.0.2/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.2/README.md
--rw-r--r--   0 tillrostalski   (501) staff       (20)      719 2023-06-29 14:47:44.000000 fhir_analyzer-0.0.2/pyproject.toml
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1387 2023-06-29 14:42:27.000000 fhir_analyzer-0.0.2/requirements.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 14:47:56.526748 fhir_analyzer-0.0.2/setup.cfg
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 14:47:56.522812 fhir_analyzer-0.0.2/src/
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 14:47:56.524948 fhir_analyzer-0.0.2/src/fhir_analyzer/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/constants.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     4975 2023-06-25 13:42:39.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/feature_selector.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/fhirstore.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2164 2023-06-26 19:13:12.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/helper.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 14:47:56.526310 fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/
--rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/__init__.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)    13136 2023-06-25 20:13:44.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/comparator.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2391 2023-06-25 17:02:32.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/internal_types.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     9003 2023-06-25 20:17:45.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/patsim.py
--rw-r--r--   0 tillrostalski   (501) staff       (20)     2603 2023-06-25 19:58:12.000000 fhir_analyzer-0.0.2/src/fhir_analyzer/tmp.py
-drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 14:47:56.525604 fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/
--rw-r--r--   0 tillrostalski   (501) staff       (20)      458 2023-06-29 14:47:56.000000 fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 tillrostalski   (501) staff       (20)      638 2023-06-29 14:47:56.000000 fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 14:47:56.000000 fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)     1387 2023-06-29 14:47:56.000000 fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/requires.txt
--rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 14:47:56.000000 fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.658871 fhir_analyzer-0.0.3/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1071 2023-06-25 13:13:22.000000 fhir_analyzer-0.0.3/LICENSE
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      457 2023-06-29 15:03:37.658726 fhir_analyzer-0.0.3/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       16 2023-06-24 16:03:53.000000 fhir_analyzer-0.0.3/README.md
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      718 2023-06-29 15:03:28.000000 fhir_analyzer-0.0.3/pyproject.toml
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1387 2023-06-29 14:42:27.000000 fhir_analyzer-0.0.3/requirements.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       38 2023-06-29 15:03:37.658913 fhir_analyzer-0.0.3/setup.cfg
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.654371 fhir_analyzer-0.0.3/src/
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.656728 fhir_analyzer-0.0.3/src/fhir_analyzer/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-18 09:07:45.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4139 2023-06-18 17:05:10.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/constants.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     4975 2023-06-25 13:42:39.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/feature_selector.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     3444 2023-06-19 15:53:02.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/fhirstore.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2164 2023-06-26 19:13:12.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/helper.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.658287 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        0 2023-06-19 15:56:47.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/__init__.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)    13136 2023-06-25 20:13:44.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/comparator.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2391 2023-06-25 17:02:32.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/internal_types.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     9003 2023-06-25 20:17:45.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/patsim.py
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     2603 2023-06-25 19:58:12.000000 fhir_analyzer-0.0.3/src/fhir_analyzer/tmp.py
+drwxr-xr-x   0 tillrostalski   (501) staff       (20)        0 2023-06-29 15:03:37.657383 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      457 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 tillrostalski   (501) staff       (20)      638 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)        1 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)     1387 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/requires.txt
+-rw-r--r--   0 tillrostalski   (501) staff       (20)       14 2023-06-29 15:03:37.000000 fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/top_level.txt
```

### Comparing `fhir_analyzer-0.0.2/LICENSE` & `fhir_analyzer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/pyproject.toml` & `fhir_analyzer-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fhir_analyzer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Till Rostalski", email="tillrostalski@gmail.com" },
 ]
 description = "A small FHIR package"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
```

### Comparing `fhir_analyzer-0.0.2/requirements.txt` & `fhir_analyzer-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/constants.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/constants.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/feature_selector.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/feature_selector.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/fhirstore.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/fhirstore.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/helper.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/helper.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/comparator.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/comparator.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/internal_types.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/internal_types.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/patient_similarity/patsim.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/patient_similarity/patsim.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer/tmp.py` & `fhir_analyzer-0.0.3/src/fhir_analyzer/tmp.py`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/SOURCES.txt` & `fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fhir_analyzer-0.0.2/src/fhir_analyzer.egg-info/requires.txt` & `fhir_analyzer-0.0.3/src/fhir_analyzer.egg-info/requires.txt`

 * *Files identical despite different names*

