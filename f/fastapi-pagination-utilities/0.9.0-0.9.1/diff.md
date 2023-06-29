# Comparing `tmp/fastapi-pagination-utilities-0.9.0.tar.gz` & `tmp/fastapi-pagination-utilities-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-pagination-utilities-0.9.0.tar", last modified: Tue Sep  7 13:54:05 2021, max compression
+gzip compressed data, was "fastapi-pagination-utilities-0.9.1.tar", last modified: Thu Jun 29 12:45:55 2023, max compression
```

## Comparing `fastapi-pagination-utilities-0.9.0.tar` & `fastapi-pagination-utilities-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 13:54:05.401070 fastapi-pagination-utilities-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2021-09-07 13:22:33.000000 fastapi-pagination-utilities-0.9.0/COPYING
--rw-r--r--   0 root         (0) root         (0)     2675 2021-09-07 13:54:05.401070 fastapi-pagination-utilities-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1950 2021-09-07 13:22:33.000000 fastapi-pagination-utilities-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 13:54:05.401070 fastapi-pagination-utilities-0.9.0/fastapi_pagination/
--rw-rw-rw-   0 root         (0) root         (0)     3243 2021-09-07 13:22:33.000000 fastapi-pagination-utilities-0.9.0/fastapi_pagination/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 13:54:05.401070 fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2675 2021-09-07 13:54:05.000000 fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      359 2021-09-07 13:54:05.000000 fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-07 13:54:05.000000 fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2021-09-07 13:54:05.000000 fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-09-07 13:54:05.000000 fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-09-07 13:54:05.401070 fastapi-pagination-utilities-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1508 2021-09-07 13:22:33.000000 fastapi-pagination-utilities-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 13:54:05.401070 fastapi-pagination-utilities-0.9.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-09-07 13:22:33.000000 fastapi-pagination-utilities-0.9.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2021-09-07 13:22:33.000000 fastapi-pagination-utilities-0.9.0/tests/test_pagination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:45:55.908724 fastapi-pagination-utilities-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-22 11:37:42.000000 fastapi-pagination-utilities-0.9.1/COPYING
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-29 12:45:55.908724 fastapi-pagination-utilities-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-06-22 11:37:42.000000 fastapi-pagination-utilities-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:45:55.908724 fastapi-pagination-utilities-0.9.1/fastapi_pagination/
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-22 11:37:42.000000 fastapi-pagination-utilities-0.9.1/fastapi_pagination/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:45:55.908724 fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-29 12:45:55.000000 fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      359 2023-06-29 12:45:55.000000 fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:45:55.000000 fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-29 12:45:55.000000 fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-29 12:45:55.000000 fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 12:45:55.908724 fastapi-pagination-utilities-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-06-29 12:36:50.000000 fastapi-pagination-utilities-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:45:55.908724 fastapi-pagination-utilities-0.9.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 12:45:53.000000 fastapi-pagination-utilities-0.9.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-06-22 11:37:42.000000 fastapi-pagination-utilities-0.9.1/tests/test_pagination.py
```

### Comparing `fastapi-pagination-utilities-0.9.0/COPYING` & `fastapi-pagination-utilities-0.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-utilities-0.9.0/PKG-INFO` & `fastapi-pagination-utilities-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fastapi-pagination-utilities
-Version: 0.9.0
+Version: 0.9.1
 Summary: A module containing helpers for paginating responses with FastAPI
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/lib/fastapi-pagination
 Author: University of Cambridge Information Services
 Author-email: devops+fastapi-pagination-utilities@uis.cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -89,9 +88,7 @@
 
 # Run a single test file within PyTest
 $ ./test.sh -e py3 -- tests/test_identifiers.py
 
 # Run a single test file within PyTest with verbose logging
 $ ./test.sh -e py3 -- tests/test_identifiers.py -vvv
 ```
-
-
```

### Comparing `fastapi-pagination-utilities-0.9.0/README.md` & `fastapi-pagination-utilities-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-utilities-0.9.0/fastapi_pagination/__init__.py` & `fastapi-pagination-utilities-0.9.1/fastapi_pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-pagination-utilities-0.9.0/fastapi_pagination_utilities.egg-info/PKG-INFO` & `fastapi-pagination-utilities-0.9.1/fastapi_pagination_utilities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fastapi-pagination-utilities
-Version: 0.9.0
+Version: 0.9.1
 Summary: A module containing helpers for paginating responses with FastAPI
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/lib/fastapi-pagination
 Author: University of Cambridge Information Services
 Author-email: devops+fastapi-pagination-utilities@uis.cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -89,9 +88,7 @@
 
 # Run a single test file within PyTest
 $ ./test.sh -e py3 -- tests/test_identifiers.py
 
 # Run a single test file within PyTest with verbose logging
 $ ./test.sh -e py3 -- tests/test_identifiers.py -vvv
 ```
-
-
```

### Comparing `fastapi-pagination-utilities-0.9.0/setup.py` & `fastapi-pagination-utilities-0.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 
 PACKAGE_NAME = "fastapi-pagination-utilities"
 PACKAGE_DESCRIPTION = (
     "A module containing helpers for paginating responses with FastAPI"
 )
-PACKAGE_VERSION = "0.9.0"
+PACKAGE_VERSION = "0.9.1"
 PACKAGE_URL = "https://gitlab.developers.cam.ac.uk/uis/devops/lib/fastapi-pagination"
 
 
 def load_requirements(file: str):
     """
     Load requirements file and return non-empty, non-comment lines with leading and trailing
     whitespace stripped.
```

### Comparing `fastapi-pagination-utilities-0.9.0/tests/test_pagination.py` & `fastapi-pagination-utilities-0.9.1/tests/test_pagination.py`

 * *Files identical despite different names*

