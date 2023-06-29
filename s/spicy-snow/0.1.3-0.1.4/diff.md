# Comparing `tmp/spicy-snow-0.1.3.tar.gz` & `tmp/spicy-snow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicy-snow-0.1.3.tar", last modified: Thu May 18 18:51:43 2023, max compression
+gzip compressed data, was "spicy-snow-0.1.4.tar", last modified: Thu Jun 29 19:04:51 2023, max compression
```

## Comparing `spicy-snow-0.1.3.tar` & `spicy-snow-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.161347 spicy-snow-0.1.3/spicy_snow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/spicy_snow/IO/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/IO/user_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/IO/user_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/spicy_snow/download/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/download/forest_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/download/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/download/snow_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/download/snowex_lidar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/spicy_snow/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/processing/s1_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/processing/snow_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/processing/wet_snow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/spicy_snow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/utils/nsidc.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/utils/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/spicy_snow/utils/spicy_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/spicy_snow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-18 18:51:43.000000 spicy-snow-0.1.3/spicy_snow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-18 18:51:43.000000 spicy-snow-0.1.3/spicy_snow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:51:43.000000 spicy-snow-0.1.3/spicy_snow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 18:51:43.000000 spicy-snow-0.1.3/spicy_snow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 18:51:43.000000 spicy-snow-0.1.3/spicy_snow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:51:43.165347 spicy-snow-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/tests/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/tests/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/tests/test_snow_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    23142 2023-05-18 18:51:29.000000 spicy-snow-0.1.3/tests/test_wetsnow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.319858 spicy-snow-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 19:04:33.000000 spicy-snow-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-29 19:04:51.319858 spicy-snow-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-29 19:04:33.000000 spicy-snow-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:04:51.319858 spicy-snow-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.311858 spicy-snow-0.1.4/spicy_snow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.311858 spicy-snow-0.1.4/spicy_snow/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/IO/user_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/IO/user_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.315858 spicy-snow-0.1.4/spicy_snow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/download/forest_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/download/sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/download/snow_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/download/snowex_lidar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.315858 spicy-snow-0.1.4/spicy_snow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/processing/s1_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/processing/snow_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/processing/wet_snow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.315858 spicy-snow-0.1.4/spicy_snow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/utils/nsidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/utils/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/spicy_snow/utils/spicy_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.311858 spicy-snow-0.1.4/spicy_snow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-29 19:04:51.000000 spicy-snow-0.1.4/spicy_snow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 19:04:51.000000 spicy-snow-0.1.4/spicy_snow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:04:51.000000 spicy-snow-0.1.4/spicy_snow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 19:04:51.000000 spicy-snow-0.1.4/spicy_snow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 19:04:51.000000 spicy-snow-0.1.4/spicy_snow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:04:51.319858 spicy-snow-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/tests/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/tests/test_snow_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24521 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/tests/test_wetsnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-29 19:04:34.000000 spicy-snow-0.1.4/tests/test_wrappers.py
```

### Comparing `spicy-snow-0.1.3/LICENSE` & `spicy-snow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/PKG-INFO` & `spicy-snow-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicy-snow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Snow Depth Retrievals from Sentinel-1 Backscatter.
 Home-page: https://github.com/SnowEx/spicy-snow
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![MIT License][license-shield]][license-url]
-[![PIP](https://img.shields.io/badge/pip-0.1.2-purple)](https://img.shields.io/badge/pip-0.1.2-purple)
+[![PIP](https://img.shields.io/badge/pip-0.1.3-purple)](https://img.shields.io/badge/pip-0.1.3-purple)
 [![COVERAGE](https://img.shields.io/badge/coverage-86%25-green)](https://img.shields.io/badge/coverage-86%25-green) 
 [![DOI](https://zenodo.org/badge/590243635.svg)](https://zenodo.org/badge/latestdoi/590243635)
 
 # spicy-snow
 
 Python module to use volumetric scattering at C-band to calculate snow depths from Sentinel-1 imagery using Lieven et al.'s 2021 technique.
 
@@ -123,15 +123,15 @@
 
 Readme template: https://github.com/othneildrew/Best-README-Template
 
 Title image: https://openai.com/dall-e-2/
 
 ## Contact
 
-Zach Keskinen: zacharykeskinen@boisestate.edu
+Zach Hoppinen: zacharykeskinen@boisestate.edu
 
 Project Link: https://github.com/SnowEx/spicy-snow
 
 ## Links to relevant repos/sites
 
 Sentinel 1 Download:
 https://github.com/ASFHyP3/hyp3-sdk
```

### Comparing `spicy-snow-0.1.3/README.md` & `spicy-snow-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![MIT License][license-shield]][license-url]
-[![PIP](https://img.shields.io/badge/pip-0.1.2-purple)](https://img.shields.io/badge/pip-0.1.2-purple)
+[![PIP](https://img.shields.io/badge/pip-0.1.3-purple)](https://img.shields.io/badge/pip-0.1.3-purple)
 [![COVERAGE](https://img.shields.io/badge/coverage-86%25-green)](https://img.shields.io/badge/coverage-86%25-green) 
 [![DOI](https://zenodo.org/badge/590243635.svg)](https://zenodo.org/badge/latestdoi/590243635)
 
 # spicy-snow
 
 Python module to use volumetric scattering at C-band to calculate snow depths from Sentinel-1 imagery using Lieven et al.'s 2021 technique.
 
@@ -104,15 +104,15 @@
 
 Readme template: https://github.com/othneildrew/Best-README-Template
 
 Title image: https://openai.com/dall-e-2/
 
 ## Contact
 
-Zach Keskinen: zacharykeskinen@boisestate.edu
+Zach Hoppinen: zacharykeskinen@boisestate.edu
 
 Project Link: https://github.com/SnowEx/spicy-snow
 
 ## Links to relevant repos/sites
 
 Sentinel 1 Download:
 https://github.com/ASFHyP3/hyp3-sdk
```

### Comparing `spicy-snow-0.1.3/setup.py` & `spicy-snow-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 twine upload dist/*
 
 in the home directory of this file.
 
 to have github auto-release:
 https://dev.to/iamtekson/publish-package-to-pypi-and-release-new-version-using-github-actions-108k
 
-git tag -a "v0.0.6" -m "new tag"
-git push --tags
+git tag -a 0.0.6 -m "new tag"
+git push origin 0.0.6
 """
 
 import io
 import os
 import sys
 from shutil import rmtree
 
@@ -114,15 +114,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.1.3', # change to value if not using github auto upload
+    version='0.1.4', # change to value if not using github auto upload
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
@@ -148,8 +148,8 @@
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
-)
+)
```

### Comparing `spicy-snow-0.1.3/spicy_snow/IO/user_area.py` & `spicy-snow-0.1.4/spicy_snow/IO/user_area.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/IO/user_dates.py` & `spicy-snow-0.1.4/spicy_snow/IO/user_dates.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/download/forest_cover.py` & `spicy-snow-0.1.4/spicy_snow/download/forest_cover.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/download/sentinel1.py` & `spicy-snow-0.1.4/spicy_snow/download/sentinel1.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     if type(area) != shapely.geometry.Polygon:
         raise TypeError("Geometry must be a shapely.geometry.box type")
     if type(dates[0]) != str:
         raise TypeError("Provide at start and end date in format (YYYY-MM-DD, YYYY_MM_DD)")
     dates = [pd.to_datetime(d) for d in dates]
     if dates[1] < dates[0]:
         raise ValueError("End date is before start date")
-    if dates[0].year < 2017 or dates[1].year < 2017:
+    if dates[0].year < 2014 or dates[1].year < 2014:
         raise IndexError("Dates are prior to Sentinel-1 launch dates")
     if dates[0].date() > date.today() or dates[1].date() > date.today():
         raise IndexError("Dates are in the future.")
     if area.bounds[3] > 90 or area.bounds[1] < 0 or area.bounds[2] > 180\
         or area.bounds[0] < -180:
         raise IndexError("Coordinates must be between 0-90N and -180-180")
 
@@ -312,8 +312,8 @@
     
     # s1_units tag
     s1_dataset = s1_power_to_dB(s1_dataset)
     s1_dataset.attrs['s1_units'] = 'dB'
 
     return s1_dataset
 
-# End of file
+# End of file
```

### Comparing `spicy-snow-0.1.3/spicy_snow/download/snow_cover.py` & `spicy-snow-0.1.4/spicy_snow/download/snow_cover.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/download/snowex_lidar.py` & `spicy-snow-0.1.4/spicy_snow/download/snowex_lidar.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/processing/s1_preprocessing.py` & `spicy-snow-0.1.4/spicy_snow/processing/s1_preprocessing.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/processing/snow_index.py` & `spicy-snow-0.1.4/spicy_snow/processing/snow_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,26 +227,27 @@
     prev_si = (prev['snow_index'] * wts).sum(dim = 'time', skipna = True) / wts.sum(dim = 'time', skipna = True)
     # this is weird but works
     # (prev['snow_index']*wts).sum(dim = 'time') treats nans as 0 so they don't
     # propogate through time series (maybe a problem later for wet snow masking)
 
     return prev_si
 
-def calc_snow_index(dataset: xr.Dataset, inplace: bool = False) -> Union[None, xr.Dataset]:
+def calc_snow_index(dataset: xr.Dataset, ims_masking: bool = True, inplace: bool = False) -> Union[None, xr.Dataset]:
     """
     Calculate snow index for each time step from previous time steps' snow index
     weights, and current delta-gamma.
 
     SI (i, t) = SI (i, t_previous) + delta-gamma (i, t)
 
     with SI (i, t_previous) as:
         SI (i, t_previous) = sum (t_pri - 5/11 days, t_pri + 5/11 days)(SI * weights) / sum(weights)
 
     Args:
     dataset: Xarray Dataset of sentinel images with delta-gamma
+    ims_masking: whether to mask pixels with the IMS data
     inplace: operate on dataset in place or return copy
 
     Returns:
     dataset: Xarray Dataset of sentinel images with snow-index added as band
     """
     # check inplace flag
     if not inplace:
@@ -267,15 +268,16 @@
         # set prev_si to 0 at nans
         prev_si = prev_si.where(~prev_si.isnull(), 0)
         
         # add deltaGamma to previous snow index
         dataset['snow_index'].loc[dict(time = ct)] = prev_si + dataset['deltaGamma'].sel(time = ct)
         
         # change to 0 when ims snow cover is not 4
-        dataset['snow_index'].loc[dict(time = ct)] = dataset['snow_index'].sel(time = ct).where(dataset['ims'].sel(time = ct) == 4, 0)
+        if ims_masking:
+            dataset['snow_index'].loc[dict(time = ct)] = dataset['snow_index'].sel(time = ct).where(dataset['ims'].sel(time = ct) == 4, 0)
 
         # change to 0 when snow_index is negative
         dataset['snow_index'].loc[dict(time = ct)] = \
             dataset['snow_index'].sel(time = ct).where((dataset['snow_index'].sel(time = ct).isnull()) | (dataset['snow_index'].sel(time = ct) > 0), 0)
     
     if not inplace:
         return dataset
```

### Comparing `spicy-snow-0.1.3/spicy_snow/processing/wet_snow.py` & `spicy-snow-0.1.4/spicy_snow/processing/wet_snow.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     # identify possible re-freezing by increases of deltaGammaNaught of 2dB
     dataset['freeze_flag'] = dataset['freeze_flag'].where(dataset['deltaGamma'] < freeze_thresh, 1)
 
     if not inplace:
         return dataset
 
-def id_wet_negative_si(dataset: xr.Dataset, inplace: bool = False) -> Union[None, xr.Dataset]:
+def id_wet_negative_si(dataset: xr.Dataset, wet_SI_thresh = 0, inplace: bool = False) -> Union[None, xr.Dataset]:
     """
     Additional wet snow criteria if sd retrieval (snow-index since they are linear)
     becomes negative with snow cover is present we set pixel to wet.
 
     Args:
     dataset: xarray dataset with snow_index as data vars
     inplace: return copy of dataset or operate on dataset inplace?
@@ -98,15 +98,15 @@
           f"Missing variables {necessary_vars.difference(set(dataset.data_vars))}"
 
     # add alt_wet_flag to dataset if not already present    
     if 'alt_wet_flag' not in dataset.data_vars:
         dataset['alt_wet_flag'] = xr.zeros_like(dataset['deltaVV'])
 
     # identify wetting of snow by negative snow index with snow present
-    dataset['alt_wet_flag'] = dataset['alt_wet_flag'].where(((dataset['ims'] != 4) | (dataset['snow_index'] > 0)), 1)
+    dataset['alt_wet_flag'] = dataset['alt_wet_flag'].where(((dataset['ims'] != 4) | (dataset['snow_index'] > wet_SI_thresh)), 1)
 
     if not inplace:
         return dataset
 
 def flag_wet_snow(dataset: xr.Dataset, inplace: bool = False) -> Union[None, xr.Dataset]:
     """
     Identifies time steps with wet snow. Sets all time slices, for a relative orbit,
```

### Comparing `spicy-snow-0.1.3/spicy_snow/utils/download.py` & `spicy-snow-0.1.4/spicy_snow/utils/download.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/utils/nsidc.py` & `spicy-snow-0.1.4/spicy_snow/utils/nsidc.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow/utils/spicy_logging.py` & `spicy-snow-0.1.4/spicy_snow/utils/spicy_logging.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/spicy_snow.egg-info/PKG-INFO` & `spicy-snow-0.1.4/spicy_snow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicy-snow
-Version: 0.1.3
+Version: 0.1.4
 Summary: Snow Depth Retrievals from Sentinel-1 Backscatter.
 Home-page: https://github.com/SnowEx/spicy-snow
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![MIT License][license-shield]][license-url]
-[![PIP](https://img.shields.io/badge/pip-0.1.2-purple)](https://img.shields.io/badge/pip-0.1.2-purple)
+[![PIP](https://img.shields.io/badge/pip-0.1.3-purple)](https://img.shields.io/badge/pip-0.1.3-purple)
 [![COVERAGE](https://img.shields.io/badge/coverage-86%25-green)](https://img.shields.io/badge/coverage-86%25-green) 
 [![DOI](https://zenodo.org/badge/590243635.svg)](https://zenodo.org/badge/latestdoi/590243635)
 
 # spicy-snow
 
 Python module to use volumetric scattering at C-band to calculate snow depths from Sentinel-1 imagery using Lieven et al.'s 2021 technique.
 
@@ -123,15 +123,15 @@
 
 Readme template: https://github.com/othneildrew/Best-README-Template
 
 Title image: https://openai.com/dall-e-2/
 
 ## Contact
 
-Zach Keskinen: zacharykeskinen@boisestate.edu
+Zach Hoppinen: zacharykeskinen@boisestate.edu
 
 Project Link: https://github.com/SnowEx/spicy-snow
 
 ## Links to relevant repos/sites
 
 Sentinel 1 Download:
 https://github.com/ASFHyP3/hyp3-sdk
```

### Comparing `spicy-snow-0.1.3/spicy_snow.egg-info/SOURCES.txt` & `spicy-snow-0.1.4/spicy_snow.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 spicy_snow/utils/nsidc.py
 spicy_snow/utils/raster.py
 spicy_snow/utils/spicy_logging.py
 tests/test_IO.py
 tests/test_downloads.py
 tests/test_preprocessing.py
 tests/test_snow_index.py
-tests/test_wetsnow.py
+tests/test_wetsnow.py
+tests/test_wrappers.py
```

### Comparing `spicy-snow-0.1.3/tests/test_IO.py` & `spicy-snow-0.1.4/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/tests/test_downloads.py` & `spicy-snow-0.1.4/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/tests/test_preprocessing.py` & `spicy-snow-0.1.4/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `spicy-snow-0.1.3/tests/test_snow_index.py` & `spicy-snow-0.1.4/tests/test_snow_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,14 +529,20 @@
         test_ds['deltaGamma'].loc[dict(time = '2020-01-01', x = 5, y = 5)] = 5
         test_ds['deltaGamma'].loc[dict(time = '2020-01-02', x = 5, y = 5)] = 5
         
         ds = calc_snow_index(test_ds)
 
         assert ds['snow_index'].sel(time = '2020-01-02', x = 5, y = 5) == 0
 
+        # check with ims_masking disabled
+
+        ds = calc_snow_index(test_ds, ims_masking=False)
+
+        assert ds['snow_index'].sel(time = '2020-01-02', x = 5, y = 5) != 0
+
     def test_snow_index_to_depth(self):
 
         backscatter = np.random.randn(10, 10, 3, 3)
         snow_index = np.random.randn(10, 10 , 3)
         times = [np.datetime64(t) for t in ['2020-01-01', '2020-01-07', '2020-01-14']]
         x = np.linspace(0, 9, 10)
         y = np.linspace(10, 19, 10)
```

### Comparing `spicy-snow-0.1.3/tests/test_wetsnow.py` & `spicy-snow-0.1.4/tests/test_wetsnow.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,54 @@
 
         assert ds['alt_wet_flag'][0,0,0] == 0
         assert ds['alt_wet_flag'][0,1,0] == 1
         assert ds['alt_wet_flag'][0,2,0] == 0
         assert ds['alt_wet_flag'][0,3,0] == 0
         assert ds['alt_wet_flag'][0,1,1] == 1
 
+    def test_negative_snow_index_wet_threshold(self, ds = test_ds):
+        """
+        Testing negative SI wet snow threshold for non zero threshold
+        """
+
+        # ims is not snow, and SI is below threshold so shouldn't flag
+        ds['ims'][0,0,0] = 2
+        ds['snow_index'][0,0,0] = -2
+
+        # ims is snow and SI is below threshold so should flag
+        ds['ims'][0,1,0] = 4
+        ds['snow_index'][0,1,0] = -2
+
+        # ims is not snow and si is above threshold so shouldn't flag
+        ds['ims'][0,2,0] = 2
+        ds['snow_index'][0,2,0] = 1
+
+        # ims is snow but SI is above threshold so shouldn't flag
+        ds['ims'][0,3,0] = 4
+        ds['snow_index'][0,3,0] = 1
+
+        # ims is snow and SI is below threshold so should flag
+        ds['ims'][0,1,1] = 4
+        ds['snow_index'][0,1,1] = -2
+
+        # ims is snow and SI is above threshold so should not flag
+        ds['ims'][0,1,2] = 4
+        ds['snow_index'][0,1,2] = -0.9
+
+
+        # identify possible newly wet snow in regions with SI < 4 and IMS == 4
+        ds = id_wet_negative_si(ds, wet_SI_thresh = -1)
+
+        assert ds['alt_wet_flag'][0,0,0] == 0
+        assert ds['alt_wet_flag'][0,1,0] == 1
+        assert ds['alt_wet_flag'][0,2,0] == 0
+        assert ds['alt_wet_flag'][0,3,0] == 0
+        assert ds['alt_wet_flag'][0,1,1] == 1
+        assert ds['alt_wet_flag'][0,1,2] == 0
+
     def test_id_wet_one_orbit(self):
         """
         Test id wet snow
         """
         fcf = np.random.randn(10, 10)/10 + 0.5
         deltaVV = np.random.randn(10, 10, 6) * 3
         deltaCR = np.random.randn(10, 10, 6) * 3
```

