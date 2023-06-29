# Comparing `tmp/climatePy-0.0.4.0.tar.gz` & `tmp/climatePy-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.0.4.0.tar", last modified: Thu Jun 29 14:38:08 2023, max compression
+gzip compressed data, was "climatePy-0.0.4.1.tar", last modified: Thu Jun 29 14:45:02 2023, max compression
```

## Comparing `climatePy-0.0.4.0.tar` & `climatePy-0.0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:38:08.216241 climatePy-0.0.4.0/
--rw-rw-rw-   0        0        0     1108 2023-06-23 23:24:45.000000 climatePy-0.0.4.0/LICENSE
--rw-rw-rw-   0        0        0     5557 2023-06-29 14:38:08.215240 climatePy-0.0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5139 2023-06-28 16:33:45.000000 climatePy-0.0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:38:08.133239 climatePy-0.0.4.0/climatePy/
--rw-rw-rw-   0        0        0     1848 2023-06-29 14:34:25.000000 climatePy-0.0.4.0/climatePy/__init__.py
--rw-rw-rw-   0        0        0     8861 2023-06-29 14:21:36.000000 climatePy-0.0.4.0/climatePy/_climatepy_filter.py
--rw-rw-rw-   0        0        0    60987 2023-06-29 14:21:29.000000 climatePy-0.0.4.0/climatePy/_dap.py
--rw-rw-rw-   0        0        0     3623 2023-06-29 14:21:30.000000 climatePy-0.0.4.0/climatePy/_netrc_utils.py
--rw-rw-rw-   0        0        0    33802 2023-06-29 14:34:46.000000 climatePy-0.0.4.0/climatePy/_shortcuts.py
--rw-rw-rw-   0        0        0    27503 2023-06-29 14:21:34.000000 climatePy-0.0.4.0/climatePy/_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:38:08.143242 climatePy-0.0.4.0/climatePy/data/
--rw-rw-rw-   0        0        0 45897655 2023-03-04 16:05:07.000000 climatePy-0.0.4.0/climatePy/data/catalog.csv
-drwxrwxrwx   0        0        0        0 2023-06-29 14:38:08.142242 climatePy-0.0.4.0/climatePy.egg-info/
--rw-rw-rw-   0        0        0     5557 2023-06-29 14:38:08.000000 climatePy-0.0.4.0/climatePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-29 14:38:08.000000 climatePy-0.0.4.0/climatePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:38:08.000000 climatePy-0.0.4.0/climatePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-29 14:38:08.000000 climatePy-0.0.4.0/climatePy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 14:38:08.000000 climatePy-0.0.4.0/climatePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:38:08.216241 climatePy-0.0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-06-29 14:35:42.000000 climatePy-0.0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:38:08.214241 climatePy-0.0.4.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 21:55:17.000000 climatePy-0.0.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0    44872 2023-06-29 14:38:04.000000 climatePy-0.0.4.0/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     3187 2023-06-29 14:34:44.000000 climatePy-0.0.4.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.549918 climatePy-0.0.4.1/
+-rw-rw-rw-   0        0        0     1108 2023-06-23 23:24:45.000000 climatePy-0.0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     5557 2023-06-29 14:45:02.548919 climatePy-0.0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5139 2023-06-28 16:33:45.000000 climatePy-0.0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.461919 climatePy-0.0.4.1/climatePy/
+-rw-rw-rw-   0        0        0     1848 2023-06-29 14:34:25.000000 climatePy-0.0.4.1/climatePy/__init__.py
+-rw-rw-rw-   0        0        0     8861 2023-06-29 14:21:36.000000 climatePy-0.0.4.1/climatePy/_climatepy_filter.py
+-rw-rw-rw-   0        0        0    60987 2023-06-29 14:21:29.000000 climatePy-0.0.4.1/climatePy/_dap.py
+-rw-rw-rw-   0        0        0     3623 2023-06-29 14:21:30.000000 climatePy-0.0.4.1/climatePy/_netrc_utils.py
+-rw-rw-rw-   0        0        0    33802 2023-06-29 14:34:46.000000 climatePy-0.0.4.1/climatePy/_shortcuts.py
+-rw-rw-rw-   0        0        0    27503 2023-06-29 14:21:34.000000 climatePy-0.0.4.1/climatePy/_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.476918 climatePy-0.0.4.1/climatePy/data/
+-rw-rw-rw-   0        0        0 45897655 2023-03-04 16:05:07.000000 climatePy-0.0.4.1/climatePy/data/catalog.csv
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.475919 climatePy-0.0.4.1/climatePy.egg-info/
+-rw-rw-rw-   0        0        0     5557 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:45:02.549918 climatePy-0.0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-06-29 14:43:59.000000 climatePy-0.0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.547919 climatePy-0.0.4.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 21:55:17.000000 climatePy-0.0.4.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    44952 2023-06-29 14:43:15.000000 climatePy-0.0.4.1/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     3253 2023-06-29 14:43:13.000000 climatePy-0.0.4.1/tests/test_utils.py
```

### Comparing `climatePy-0.0.4.0/LICENSE` & `climatePy-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/PKG-INFO` & `climatePy-0.0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.0.4.0
+Version: 0.0.4.1
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.0.4.0/README.md` & `climatePy-0.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/__init__.py` & `climatePy-0.0.4.1/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/_climatepy_filter.py` & `climatePy-0.0.4.1/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/_dap.py` & `climatePy-0.0.4.1/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/_netrc_utils.py` & `climatePy-0.0.4.1/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/_shortcuts.py` & `climatePy-0.0.4.1/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/_utils.py` & `climatePy-0.0.4.1/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy/data/catalog.csv` & `climatePy-0.0.4.1/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.0/climatePy.egg-info/PKG-INFO` & `climatePy-0.0.4.1/climatePy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.0.4.0
+Version: 0.0.4.1
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.0.4.0/setup.py` & `climatePy-0.0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
-    version="0.0.4.0",                        # version
+    version="0.0.4.1",                        # version
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.0.4.0/tests/test_shortcuts.py` & `climatePy-0.0.4.1/tests/test_shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+# pytest library
 import pytest
-# from .climatePy import shortcuts
-
-# from src.climatePy import shortcuts
-# from src.climatePy import dap
-# from src.climatePy import climatepy_filter
-# from src.climatePy import utils
 
+# import climatePy modules
 import climatePy
+
+# data manipulation libs
 import pandas as pd
 import geopandas as gpd
 import xarray as xr
-# import matplotlib.pyplot as plt
 
+# standard python libs
 import re
 from datetime import datetime
 
+
+# old imports
+# from .climatePy import shortcuts
+# from src.climatePy import shortcuts
+# from src.climatePy import dap
+# from src.climatePy import climatepy_filter
+# from src.climatePy import utils
+
 # AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
 # AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
 
 # @pytest.fixture(params=['miami_dade_county', 'san_luis_obispo_county', 
 #                         'litchfield_county', 'tuscaloosa_county', 
 #                         'boulder_county', 'king_county'])
```

### Comparing `climatePy-0.0.4.0/tests/test_utils.py` & `climatePy-0.0.4.1/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+# pytest library
 import pytest
 
-# from climatePy import utils
-
-# from src.climatePy import utils
-# import climatePy
-
+# import climatePy utils module
 import climatePy._utils as climatePy
 
+# standard python libs
 import re
 from datetime import datetime
 
+# old imports
+# from climatePy import utils
+# from src.climatePy import utils
 
 def test_getExtension():
     # Test cases where the input string contains a file extension
     assert climatePy.getExtension('myfile.txt') == 'txt'
     assert climatePy.getExtension('my.file.with.multiple.dots.txt') == 'txt'
     assert climatePy.getExtension('/path/to/myfile.txt') == 'txt'
     assert climatePy.getExtension('/path/to/my.file.with.multiple.dots.txt') == 'txt'
```

