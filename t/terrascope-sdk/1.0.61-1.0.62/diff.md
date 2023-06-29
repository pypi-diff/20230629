# Comparing `tmp/terrascope-sdk-1.0.61.tar.gz` & `tmp/terrascope-sdk-1.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrascope-sdk-1.0.61.tar", last modified: Thu Feb  9 15:33:44 2023, max compression
+gzip compressed data, was "terrascope-sdk-1.0.62.tar", last modified: Thu Jun 29 21:44:53 2023, max compression
```

## Comparing `terrascope-sdk-1.0.61.tar` & `terrascope-sdk-1.0.62.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.025595 terrascope-sdk-1.0.61/
--rw-r--r--   0 nicholashyland   (501) staff       (20)     1061 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/LICENSE
--rw-r--r--   0 nicholashyland   (501) staff       (20)     2563 2023-02-09 15:33:44.025189 terrascope-sdk-1.0.61/PKG-INFO
--rw-r--r--   0 nicholashyland   (501) staff       (20)      846 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/README.md
--rw-r--r--   0 nicholashyland   (501) staff       (20)      991 2023-02-09 15:33:25.000000 terrascope-sdk-1.0.61/pyproject.toml
--rw-r--r--   0 nicholashyland   (501) staff       (20)       38 2023-02-09 15:33:44.025704 terrascope-sdk-1.0.61/setup.cfg
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.002605 terrascope-sdk-1.0.61/terrascope/
--rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.61/terrascope/__init__.py
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.003111 terrascope-sdk-1.0.61/terrascope/sdk/
--rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.61/terrascope/sdk/__init__.py
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.010614 terrascope-sdk-1.0.61/terrascope/sdk/api/
--rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/__init__.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    27404 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/algorithm.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    28028 2023-02-09 15:33:19.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/analysis.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    13852 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/aoi.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     6456 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/credit.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     3496 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/data.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     2353 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/permission.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    15627 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/result.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     2760 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/toi.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     4178 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/user.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)      851 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/api/visualization.py
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.012530 terrascope-sdk-1.0.61/terrascope/sdk/builder/
--rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/terrascope/sdk/builder/__init__.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    15498 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/builder/algorithm.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     7091 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/builder/analysis.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     6766 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/builder/toi.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     5280 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/terrascope_sdk.py
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.013970 terrascope-sdk-1.0.61/terrascope/sdk/tools/
--rw-r--r--   0 nicholashyland   (501) staff       (20)        0 2022-08-26 19:52:37.000000 terrascope-sdk-1.0.61/terrascope/sdk/tools/__init__.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     5752 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/tools/io.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     1396 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/terrascope/sdk/tools/sdk_support.py
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.015874 terrascope-sdk-1.0.61/terrascope_sdk.egg-info/
--rw-r--r--   0 nicholashyland   (501) staff       (20)     2563 2023-02-09 15:33:43.000000 terrascope-sdk-1.0.61/terrascope_sdk.egg-info/PKG-INFO
--rw-r--r--   0 nicholashyland   (501) staff       (20)     1293 2023-02-09 15:33:43.000000 terrascope-sdk-1.0.61/terrascope_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 nicholashyland   (501) staff       (20)        1 2023-02-09 15:33:43.000000 terrascope-sdk-1.0.61/terrascope_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 nicholashyland   (501) staff       (20)      113 2023-02-09 15:33:43.000000 terrascope-sdk-1.0.61/terrascope_sdk.egg-info/requires.txt
--rw-r--r--   0 nicholashyland   (501) staff       (20)       44 2023-02-09 15:33:43.000000 terrascope-sdk-1.0.61/terrascope_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.001099 terrascope-sdk-1.0.61/tests/
-drwxr-xr-x   0 nicholashyland   (501) staff       (20)        0 2023-02-09 15:33:44.024456 terrascope-sdk-1.0.61/tests/integration/
--rw-r--r--   0 nicholashyland   (501) staff       (20)    46388 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/tests/integration/test_algorithm.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     3065 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/tests/integration/test_algorithm_builder.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    22018 2023-02-09 15:33:19.000000 terrascope-sdk-1.0.61/tests/integration/test_analysis.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     1111 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/tests/integration/test_analysis_builder.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     6127 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/tests/integration/test_aoi.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     8417 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/tests/integration/test_credit.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     1325 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/tests/integration/test_data.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     5982 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/tests/integration/test_permission.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)     7021 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/tests/integration/test_result.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)      990 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/tests/integration/test_sdk_support.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)    13125 2022-11-14 21:34:02.000000 terrascope-sdk-1.0.61/tests/integration/test_toi.py
--rw-r--r--   0 nicholashyland   (501) staff       (20)      152 2023-02-08 19:49:23.000000 terrascope-sdk-1.0.61/tests/integration/test_visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:53.047119 terrascope-sdk-1.0.62/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-06-29 21:44:53.041128 terrascope-sdk-1.0.62/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/README.md
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-29 21:44:16.000000 terrascope-sdk-1.0.62/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 21:44:53.050591 terrascope-sdk-1.0.62/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.049999 terrascope-sdk-1.0.62/terrascope/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.084726 terrascope-sdk-1.0.62/terrascope/sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.372756 terrascope-sdk-1.0.62/terrascope/sdk/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29276 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    29668 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/analysis.py
+-rw-r--r--   0 root         (0) root         (0)    13852 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/aoi.py
+-rw-r--r--   0 root         (0) root         (0)     6456 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/credit.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-06-29 21:09:21.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/data.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/permission.py
+-rw-r--r--   0 root         (0) root         (0)    15627 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/result.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/toi.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/user.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/terrascope/sdk/api/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.447970 terrascope-sdk-1.0.62/terrascope/sdk/builder/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16253 2023-06-22 22:22:10.000000 terrascope-sdk-1.0.62/terrascope/sdk/builder/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/builder/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6766 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/builder/toi.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/terrascope/sdk/terrascope_sdk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.501107 terrascope-sdk-1.0.62/terrascope/sdk/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/tools/io.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/terrascope/sdk/tools/sdk_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.640450 terrascope-sdk-1.0.62/terrascope_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-06-29 21:44:51.000000 terrascope-sdk-1.0.62/terrascope_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-06-29 21:44:51.000000 terrascope-sdk-1.0.62/terrascope_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 21:44:51.000000 terrascope-sdk-1.0.62/terrascope_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 21:44:51.000000 terrascope-sdk-1.0.62/terrascope_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-29 21:44:51.000000 terrascope-sdk-1.0.62/terrascope_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:51.986301 terrascope-sdk-1.0.62/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:52.981886 terrascope-sdk-1.0.62/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)    46535 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_algorithm_builder.py
+-rw-r--r--   0 root         (0) root         (0)    21181 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/tests/integration/test_analysis_builder.py
+-rw-r--r--   0 root         (0) root         (0)     6127 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/tests/integration/test_aoi.py
+-rw-r--r--   0 root         (0) root         (0)     8431 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_credit.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     7040 2023-05-24 18:06:41.000000 terrascope-sdk-1.0.62/tests/integration/test_result.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/tests/integration/test_sdk_support.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/tests/integration/test_toi.py
+-rw-r--r--   0 root         (0) root         (0)      152 2023-03-21 16:29:27.000000 terrascope-sdk-1.0.62/tests/integration/test_visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:51.997726 terrascope-sdk-1.0.62/venv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:44:53.008327 terrascope-sdk-1.0.62/venv/bin/
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-03-21 16:31:43.000000 terrascope-sdk-1.0.62/venv/bin/activate_this.py
```

### Comparing `terrascope-sdk-1.0.61/LICENSE` & `terrascope-sdk-1.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/PKG-INFO` & `terrascope-sdk-1.0.62/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: terrascope-sdk
-Version: 1.0.61
+Version: 1.0.62
 Summary: A software development kit for developing projects on TerraScope
-Author-email: "Martice E. Nicks III" <martice.nicks@orbitalinsight.com>
+Author-email: Orbital Insight <info@orbitalinsight.com>
 License: Copyright 2022 Orbital Insight, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -31,24 +31,33 @@
 ## Installation
 
 [Readme: Installation](https://terrascope.readme.io/docs/installation-1)
 
 ## Usage
 
 TerraScope SDK is designed to simplify access to all the [terrascope-api](https://pypi.org/project/terrascope-api/) calls
-that are available. 
+that are available. Ensure that you have the correct terrascope-api package installed.
 
 Each API uses a client object which requires the following env variables to be set:
 
 ```shell
-TERRASCOPE_HOST=terrascope-api1.orbitalinsight.com
-TERRASCOPE_TOKEN=<TerraScope API Token>
+TERRASCOPE_API_HOST=terrascope-api1.orbitalinsight.com
+TERRASCOPE_API_TOKEN=<TerraScope API Token>
 TERRASCOPE_TIMEOUT=<Int timeout in seconds> defaults to 60 seconds
 ```
 
+You will always want to ensure that you have the correct terrascope-sdk version installed. The latest can be found here:
+https://pypi.org/project/terrascope-sdk/
+
+To manually build a local version of the terrascope-sdk (for example, if you are making changes and want to test):
+1. Update the version specified in the `pyproject.toml` file, e.g. `version = "1.0.6-test"`
+2. Execute from the top-level terrascope_sdk folder: `python3 -m build`
+3. `cd dist/`
+4. `pip3 install terrascope_sdk-1.0.6-test-py3-none-any.whl` (this file name may be different based on the version specified)
+
 ## Authors and acknowledgment
 
 Orbital Insight
 
 ## License
 
 [LICENSE](LICENSE)
```

### Comparing `terrascope-sdk-1.0.61/pyproject.toml` & `terrascope-sdk-1.0.62/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terrascope-sdk"
 
 
-version = "1.0.61"
+version = "1.0.62"
 
 
 authors = [
-    { name = "Martice E. Nicks III", email = "martice.nicks@orbitalinsight.com" },
+    { name = "Orbital Insight", email = "info@orbitalinsight.com" },
 ]
 description = "A software development kit for developing projects on TerraScope"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/algorithm.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,26 +63,32 @@
         """
         Retrieve the metadata of a particular algorithm.
 
         :param pagination:
         :param algorithm_ids:
         :return: List[Algorithm]
         """
+        fetch_all = False
         if pagination is None:
             pagination = Pagination(
                 page_size=100
             )
+            fetch_all = True
         request = AlgorithmGetRequest(
             ids=algorithm_ids,
             pagination=pagination
         )
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.algorithm.get,
-                                                                timeout=self.__timeout)
+
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.algorithm.get,
+                                                                    timeout=self.__timeout)
+        else:
+            responses = [await self.__client.api.algorithm.get(request)]
         algorithms = []
         for response in responses:
             algorithms.extend(response.algorithms)
         return algorithms
 
     async def list(self, **kwargs) -> List[Algorithm]:
         """
@@ -92,23 +98,28 @@
             -Optional Params
             - search_text: str
             - min_created_on: Datetime
             - max_created_on: Datetime
             - pagination: Pagination
         :return: List[Algorithm]
         """
-        parameters = ['search_text', 'min_created_on', 'max_created_on', 'pagination']
+        parameters = ['search_text', 'min_created_on', 'max_created_on', 'pagination', 'raw_response']
         for key in kwargs.keys():
             assert key in parameters
 
         message_fragments = []
+        fetch_all = False
         if 'pagination' not in kwargs.keys():
             message_fragments.append((AlgorithmListRequest(pagination=Pagination(
                 page_size=100
             ))))
+            fetch_all = True
+
+        if 'raw_response' not in kwargs.keys():
+            kwargs['raw_response'] = False
 
         for key in kwargs.keys():
             if key == 'search_text':
                 message_fragments.append(AlgorithmListRequest(search_text=kwargs[key]))
             if key == 'min_created_on':
                 assert isinstance(kwargs[key], datetime)
                 min_created_on = Timestamp()
@@ -122,22 +133,32 @@
             if key == 'pagination':
                 message_fragments.append(AlgorithmListRequest(pagination=kwargs[key]))
 
         request = AlgorithmListRequest()
         for fragment in message_fragments:
             request.MergeFrom(fragment)
 
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.algorithm.list,
-                                                                timeout=self.__timeout)
-        algorithms = []
-        for response in responses:
-            algorithms.extend(response.algorithms)
-        return algorithms
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.algorithm.list,
+                                                                    timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return responses
+            else:
+                algorithms = []
+                for response in responses:
+                    algorithms.extend(response.algorithms)
+                return algorithms
+        else:
+            response = await self.__client.api.algorithm.list(request, timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return response
+            else:
+                return response.algorithms
 
 
 class APIAlgorithmVersion:
 
     def __init__(self, client: TerrascopeAsyncClient, timeout):
         self.__timeout = timeout
         self.__client = client
@@ -217,18 +238,24 @@
             - max_created_on: Datetime
             - include_all_versions: bool
 
         :return: List[AlgorithmVersion]
         """
 
         message_fragments = []
+        fetch_all = False
         if 'pagination' not in kwargs.keys():
             message_fragments.append((AlgorithmVersionListRequest(pagination=Pagination(
                 page_size=100
             ))))
+            fetch_all = True
+
+        if 'raw_response' not in kwargs.keys():
+            kwargs['raw_response'] = False
+
 
         for key in kwargs.keys():
             if key == 'algorithm_id':
                 message_fragments.append(AlgorithmVersionListRequest(algorithm_id=kwargs[key]))
             if key == 'search_text':
                 message_fragments.append(AlgorithmVersionListRequest(search_text=kwargs[key]))
             if key == 'min_created_on':
@@ -249,22 +276,32 @@
                 message_fragments.append(AlgorithmVersionListRequest(pagination=kwargs[key]))
 
         request = AlgorithmVersionListRequest()
         for fragment in message_fragments:
             request.MergeFrom(fragment)
         MessageToDict(request)
 
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.algorithm_version.list,
-                                                                timeout=self.__timeout)
-        algorithm_versions = []
-        for response in responses:
-            algorithm_versions.extend(response.algorithm_versions)
-        return algorithm_versions
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.algorithm_version.list,
+                                                                    timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return responses
+            else:
+                algorithm_versions = []
+                for response in responses:
+                    algorithm_versions.extend(response.algorithm_versions)
+                return algorithm_versions
+        else:
+            response = await self.__client.api.algorithm_version.list(request, timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return response
+            else:
+                return response.algorithm_versions
 
     async def deprecate(self, ids: List):
         """
         Deprecate the specific version of this algorithm. Deprecated algorithms can still be searched for, metadata can
         be retrieved, and can still be used to create new algorithm_configs which can be used as part of
         algorithm_computations, but they are no longer actively supported. All algorithm_configs created from this
         algorithm_version are also deprecated, but can still be used in new algorithm_computations.
@@ -379,19 +416,24 @@
             * max_created_on: google.protobuf.Timestamp,
             * include_deactivated: bool,
             * pagination: Pagination
 
         :return: List[AlgorithmConfig]
         """
         message_fragments = []
+        fetch_all = False
         if 'pagination' not in kwargs.keys():
             message_fragments.append(AlgorithmConfigListRequest(
                 pagination=Pagination(
                     page_size=100
                 )))
+            fetch_all = True
+        if 'raw_response' not in kwargs.keys():
+            kwargs['raw_response'] = False
+
         if 'include_deactivated' not in kwargs.keys():
             message_fragments.append(AlgorithmConfigListRequest(
                 include_deactivated=False
             ))
 
         for key in kwargs.keys():
             if key == 'search_text':
@@ -424,22 +466,32 @@
                 message_fragments.append(AlgorithmConfigListRequest(
                     pagination=kwargs[key]
                 ))
         request = AlgorithmConfigListRequest()
         for fragment in message_fragments:
             request.MergeFrom(fragment)
 
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.algorithm_config.list,
-                                                                timeout=self.__timeout)
-        algorithm_configs = []
-        for response in responses:
-            algorithm_configs.extend(response.algorithm_configs)
-        return algorithm_configs
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.algorithm_config.list,
+                                                                    timeout=self.__timeout)
+            if kwargs['raw_response']:
+                algorithm_configs = []
+                for response in responses:
+                    algorithm_configs.extend(response.algorithm_configs)
+                return algorithm_configs
+            else:
+                return responses
+        else:
+            response = await self.__client.api.algorithm_config.list(request, timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return response
+            else:
+                return response.algorithm_configs
 
     async def deprecate(self, algorithm_config_ids: List):
         """
         Deprecate the specific configuration of an algorithm_version. Deprecated algorithm_configs can still be
         searched for, metadata can be retrieved, and can still be used in new algorithm_computations, but they are no
         longer actively supported.
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/analysis.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,18 +90,25 @@
             - search_text: str
             - min_created_on: Datetime
             - max_created_on: Datetime
             - pagination: Pagination
         :return: List[Analysis]
         """
         request_fragments = []
+        fetch_all = False
         if 'pagination' not in kwargs.keys():
             request_fragments.append((AnalysisListRequest(pagination=Pagination(
                 page_size=100
             ))))
+            fetch_all = True
+
+        if 'raw_response' not in kwargs.keys():
+            kwargs['raw_response'] = False
+
+
         for key in kwargs.keys():
             if key == 'search_text':
                 assert isinstance(kwargs[key], str)
                 request_fragments.append(AnalysisListRequest(search_text=kwargs[key]))
             if key == 'min_created_on':
                 min_created_on = Timestamp()
                 min_created_on.FromDatetime(kwargs[key])
@@ -113,23 +120,34 @@
             if key == 'pagination':
                 request_fragments.append(AnalysisListRequest(pagination=kwargs[key]))
 
         request = AnalysisListRequest()
         for param in request_fragments:
             request.MergeFrom(param)
 
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.analysis.list,
-                                                                timeout=self.__timeout)
-        analyses = []
-        for response in responses:
-            analyses.extend(response.analyses)
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.analysis.list,
+                                                                    timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return responses
+            else:
+                analyses = []
+                for response in responses:
+                    analyses.extend(response.analyses)
+
+                return analyses
+        else:
+            response = await self.__client.api.analysis.list(request, timeout=self.__timeout)
 
-        return analyses
+            if kwargs['raw_response']:
+                return response
+            else:
+                return response.analyses
 
 
 class APIAnalysisVersion:
     def __init__(self, client: TerrascopeAsyncClient, timeout):
         self.__timeout = timeout
         self.__client = client
 
@@ -200,23 +218,29 @@
             - pagination: Pagination
         :return: List[AnalysisVersion]
         """
 
         assert kwargs.keys() is not None
 
         request_fragments = []
+        fetch_all = False
         if 'pagination' not in kwargs.keys():
             request_fragments.append((AnalysisVersionListRequest(pagination=Pagination(
                 page_size=100
             ))))
-        if 'include_manifest' not in kwargs.keys():
-            request_fragments.append(AnalysisVersionListRequest(include_manifest=False))
+            fetch_all = True
 
-        if 'include_all_versions' not in kwargs.keys():
-            request_fragments.append(AnalysisVersionListRequest(include_all_versions=False))
+        if 'raw_response' not in kwargs.keys():
+            kwargs['raw_response'] = False
+
+        if 'include_manifest' in kwargs.keys():
+            request_fragments.append(AnalysisVersionListRequest(include_manifest=True))
+
+        if 'include_all_versions' in kwargs.keys():
+            request_fragments.append(AnalysisVersionListRequest(include_all_versions=True))
 
         for key in kwargs.keys():
             if key == 'analysis_id':
                 request_fragments.append(AnalysisVersionListRequest(analysis_id=kwargs[key]))
             if key == 'search_text':
                 request_fragments.append(AnalysisVersionListRequest(search_text=kwargs[key]))
             if key == 'tag':
@@ -234,22 +258,33 @@
             if key == 'pagination':
                 request_fragments.append(AnalysisVersionListRequest(pagination=kwargs[key]))
 
         request = AnalysisVersionListRequest()
         for request_fragment in request_fragments:
             request.MergeFrom(request_fragment)
 
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.analysis_version.list,
-                                                                timeout=self.__timeout)
-        analysis_versions = []
-        for response in responses:
-            analysis_versions.extend(response.analysis_versions)
-        return analysis_versions
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.analysis_version.list,
+                                                                    timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return responses
+            else:
+                analysis_versions = []
+                for response in responses:
+                    analysis_versions.extend(response.analysis_versions)
+                return analysis_versions
+        else:
+            response = await self.__client.api.analysis_version.list(request, timeout=self.__timeout)
+
+            if kwargs['raw_response']:
+                return response
+            else:
+                return response.analysis_versions
 
     async def deprecate(self, analysis_version_ids: List):
         """
         Deprecate the specific version of this analysis. Deprecated analysiss can still be searched for, metadata can
         be retrieved, and can still be used to create new analysis_configs which can be used as part of
         analysis_computations, but they are no longer actively supported. All analysis_configs created from this
         analysis_version are also deprecated, but can still be used in new analysis_computations.
@@ -359,18 +394,23 @@
             - pagination: Pagination
 
         :return: List[AnalysisConfig]
         """
         assert kwargs.keys() is not None
 
         request_fragments = []
+        fetch_all = False
         if 'pagination' not in kwargs.keys():
             request_fragments.append(AnalysisConfigListRequest(pagination=Pagination(
                 page_size=100
             )))
+            fetch_all = True
+
+        if 'raw_response' not in kwargs.keys():
+            kwargs['raw_response'] = False
 
         for key in kwargs.keys():
             if key == 'analysis_id':
                 request_fragments.append(AnalysisConfigListRequest(analysis_id=kwargs[key]))
             if key == 'analysis_version_id':
                 request_fragments.append(AnalysisConfigListRequest(analysis_version_id=kwargs[key]))
             if key == 'subject_id':
@@ -393,22 +433,34 @@
                 request_fragments.append(AnalysisConfigListRequest(include_deactivated=False))
             if key == 'pagination':
                 request_fragments.append(AnalysisConfigListRequest(pagination=kwargs[key]))
 
         request = AnalysisConfigListRequest()
         for request_fragment in request_fragments:
             request.MergeFrom(request_fragment)
-        sdk_support = SDKSupport()
-        responses = await sdk_support.get_all_paginated_objects(request,
-                                                                api_function=self.__client.api.analysis_config.list,
-                                                                timeout=self.__timeout)
-        analysis_configs = []
-        for response in responses:
-            analysis_configs.extend(response.analysis_configs)
-        return analysis_configs
+
+        if fetch_all:
+            sdk_support = SDKSupport()
+            responses = await sdk_support.get_all_paginated_objects(request,
+                                                                    api_function=self.__client.api.analysis_config.list,
+                                                                    timeout=self.__timeout)
+            if kwargs['raw_response']:
+                return responses
+            else:
+                analysis_configs = []
+                for response in responses:
+                    analysis_configs.extend(response.analysis_configs)
+                return analysis_configs
+        else:
+            response = await self.__client.api.analysis_config.list(request)
+
+            if kwargs['raw_response']:
+                return response
+            else:
+                return response.analysis_configs
 
     async def deprecate(self, analysis_config_ids: List):
         """
         Deprecate the specific configuration of an analysis_version. Deprecated analysis_configs can still be searched
         for, metadata can be retrieved, and can still be used in new analysis_computations, but they are no longer
         actively supported.
         :param analysis_config_ids:
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/aoi.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/aoi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/credit.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/credit.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/data.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,37 +51,35 @@
     async def create(self, name: str, description: str, schema: str, data_source_ids: List,
                      sensor_type: str) -> DataType:
         """
 
         :param name:
         :param description:
         :param schema:
-        :param data_source_ids:
         :param sensor_type:
         :return:
         """
         request = DataTypeCreateRequest(
             name=name,
             description=description,
             schema=schema,
-            data_source_ids=data_source_ids,
             sensor_type=sensor_type
         )
         response = await self.__client.api.data_type.create(request)
         return response.data_type
 
-    async def get(self, ids: List[str]) -> List[DataType]:
+    async def get(self, names: List[str]) -> List[DataType]:
         """
         Gets a data type that the user has access to.
 
         :param ids: These are the name fields for the data source
         :return: List[DataType]
         """
         request = DataTypeGetRequest(
-            ids=ids
+            names=names
         )
         response = await self.__client.api.data_type.get(request, timeout=self.__timeout)
         return response.data_types
 
     async def list(self, **kwargs) -> List[DataType]:
         """
         List all registered data_types.
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/permission.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/permission.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from typing import List
 
 from terrascope_api import TerrascopeAsyncClient
 from terrascope_api.models.permission_pb2 import Permission, PermissionCreateRequest, PermissionCreateResponse
-from terrascope_api.models.user_pb2 import User, UserGetRequest
+from terrascope_api.models.user_pb2 import User, UserGetRequest, UserListRequest
 
 
 class APIPermission:
     def __init__(self, client: TerrascopeAsyncClient, timeout):
         self.__timeout = timeout
         self.__client = client
 
     async def create(self, resource_ids: List[str], resource_type: Permission.ResourceType,
                      permission_type: Permission.PermissionType, user_ids: List[str] = [],
+                     user_emails: List[str] = [],
                      public: bool = False, public_confirm: bool = False) -> PermissionCreateResponse:
         """
         ...
         :param public:
-        :param user_ids: The user IDs (emails) you'd like to share the resources with.
         :param resource_ids: The resource IDs you'd like to share with the users.
+        :param user_ids: The unique user IDs you'd like to share the resources with.
+        :param user_emails: The user emails you'd like to share the resources with.
         :param resource_type: The type of resource the resource IDs reference.
         :param permission_type: Permission type to grant the users for the resource (read, write, admin).
         :param public: Flag to share publicly (all users). Must have global admin role and use the public_confirm param.
         :param public_confirm: Flag to confirm the sharing of the resource_ids publicly.
         :return: PermissionCreateResponse
         """
 
@@ -29,18 +31,29 @@
             if public_confirm:
                 uuids = ["1"]
             else:
                 print("You must set public_confirm=True to share these resources publicly")
                 return
         else:
             # Get UUID of user from emails
-            user_get_request = UserGetRequest(users=[User(email=email) for email in user_ids])
-            user_get_response = await self.__client.api.user.get(user_get_request)
-            uuids = [user.id for user in user_get_response.users]
+            uuids = []
 
+            for user_id in user_ids:
+                uuids.append(user_id)
+
+            for user_email in user_emails:
+                user_list_request = UserListRequest(email=user_email)
+                user_list_response = await self.__client.api.user.list(user_list_request)
+
+                uuids += [user.id for user in user_list_response.users]
+
+        # include users specified by uuid + user_ids
+        uuids = list(set(uuids))
+
+        #  print(f'uuids= {uuids}')
         request = PermissionCreateRequest(
             permissions=[
                 Permission(
                     resource_type=resource_type,
                     resource_ids=resource_ids,
                     subject_ids=uuids,
                     permission_types=[permission_type]
@@ -50,7 +63,8 @@
         response = await self.__client.api.permission.create(request)
         return response
 
     async def get(self):
         """
         """
         pass
+
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/result.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/result.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/toi.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/toi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/api/user.py` & `terrascope-sdk-1.0.62/terrascope/sdk/api/user.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/builder/algorithm.py` & `terrascope-sdk-1.0.62/terrascope/sdk/builder/algorithm.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,65 +5,65 @@
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.struct_pb2 import Struct
 
 from terrascope.sdk.builder.toi import Frequency
 
 
 class DataType(Enum):
-    ALGORITHM = "algorithm"
     PINGS = "pings"
-    TRACK_PINGS = "track_pings"
+    DEVICE_TRACKS = "device_tracks"
+    DEVICE_VISITS = "device_visits"
     OPTICAL_IMAGERY = "optical_imagery"
+    OBJECT_DETECTION = "object_detection"
+    MULTICLASS_OBJECT_DETECTION = "multiclass_object_detection"
     SPOT_MOSAIC = "spot_mosaic"
     PSSCENE = "psscene"
     SKYSAT = "skysat"
     POPULATION = "population"
     PROXIMITY_ZONE_UDC = "proximity_zone_udc"
+    HEURISTIC_JUMPS = "heuristic_jumps"
+    NAVIGATIONAL_QUALITY_INDICATORS = "navigational_quality_indicators"
+    GNSS_CLUSTERS = "gnss_clusters"
+    CROP_CIRCLES = "crop_circles"
+    TRACEABILITY_CLUSTERS = "traceability_clusters"
+    TRACEABILITY_HEATMAP = "traceability_heatmap"
+    UDC_HEATMAP = "unique_device_count_heatmap"
+    UDC = "unique_device_count"
 
 
 class DataSource(Enum):
     # Ping Sources
     GEOLOCATION = "geolocation_pings"
     SAFEGRAPH = "safegraph_pings"
     XMODE = "xmode_pings"
     CUEBIQ = "cuebiq_pings"
     BLOGWATCHER = "blogwatcher_pings"
     SPIRE = "spire_pings"
+    SPIRE_NMEA = "spire-nmea_pings"
     CUEBIQ_WORKBENCH = "cuebiq-workbench_pings"
     WEJO = "wejo_pings"
     HAWKEYE360 = "hawkeye360_pings"
     OTONOMO = "otonomo_pings"
     ADSBX = "adsbx_pings"
     EXACTEARTH = "exact-earth_pings"
     EXACTEARTH_NMEA = "exact-earth_nmea-pings"
 
-    # Algorithm Sources
-    ORBITAL_ALGORITHM = "orbital-insight_algorithm"
-    ADSBX_TRACKS = "adsbx_track_pings"
-    SAFEGRAPH_TRACKS = "safegraph_track_pings"
-    EXACTEARTH_TRACKS = "exact-earth_track_pings"
-    EXACTEARTH_NMEA_TRACKS = "exact-earth-nmea_track_pings"
-    XMODE_TRACKS = "xmode_track_pings"
-    CUEBIQ_TRACKS = "cuebiq_track_pings"
-    BLOGWATCHER_TRACKS = "blogwatcher_track_pings"
-    SPIRE_TRACKS = "spire_track_pings"
-    CUEBIQ_WORKBENCH_TRACKS = "cuebiq-workbench_track_pings"
-    WEJO_TRACKS = "wejo_track_pings"
-    HAWKEYE360_TRACKS = "hawkeye360_track_pings"
 
     # Imagery Sources
     IMAGERY = "imagery_imagery"
     PLANET_REORTHOTILE = "planet_REOrthoTile"
     PLANET_PSORTHOTILE = "planet_OSOrthoTile"
     PLANET_PSSCENE4BAND = "planet_PSScene4Band"
     PLANET_SKYSATSCENE = "planet_SkySatScene"
     PLANET_SKYSATCOLLECT = "planet_SkySatCollect"
     AIRBUS_SPOT7 = "airbus_SPOT7"
     AIRBUS_PHR1A = "airbus_PHR1A"
     AIRBUS_PHR1B = "airbus_PHR1B"
+    MAXAR_WORLDVIEW_2 = "maxar_Worldview_02"
+    AIRBUS_SPOT = "airbus_SPOT"
 
 
 class ReleaseStatus(Enum):
     DEV = "DEV"
     QA = "QA"
     STAGE = "STAGE"
     PROD = "PROD"
@@ -115,15 +115,20 @@
         }
         self.__parameters = {
             "parameters": []
         }
         self.__grouping = {
             "grouping": {}
         }
-        self.__parallelization = []
+        self.__parallelization = {
+            "parallelization": {
+                "dimensions": [],
+                "configuration": {}
+            }
+        }
         self.__restrictions = {
             "restrictions": {}
         }
         self.__outputs = {
             "outputs": {}
         }
         self.__performance_metrics = {
@@ -173,37 +178,37 @@
     def metadata_indicator(self, indicator: str):
         self.__metadata['metadata']['indicator'] = indicator
 
     def metadata_tags(self, tags: List):
         self.__metadata['metadata']['tags'] = tags
 
     # Interface
-    def interface_required(self, interface_type: InterfaceType):
+    def interface_required(self, interface_type: str):
         self.interface_interface_type(interface_type=interface_type)
 
-    def interface_interface_type(self, interface_type: InterfaceType):
-        self.__interface['interface']["interface_type"] = interface_type.value
+    def interface_interface_type(self, interface_type: str):
+        self.__interface['interface']["interface_type"] = interface_type
         self.__required['interface']['interface_type'] = True
 
     def interface_adapter(self, adapter: str):
         self.__interface['interface']['adapter'] = adapter
 
     # Inputs
-    def inputs_add_data_type(self, data_type_name: DataType, **kwargs):
+    def inputs_add_data_type(self, data_type_name: str, **kwargs):
         """
         [REQUIRED]
 
         Adds data types this algorithm is allowed to have as inputs.
 
         :param data_type_name:
         :param kwargs:
         :return:
         """
         entry = {
-            "data_type_name": data_type_name.value
+            "data_type_name": data_type_name
         }
         if 'min_count' in kwargs.keys():
             entry['min_count'] = kwargs['min_count']
         if 'max_count' in kwargs.keys():
             entry['max_count'] = kwargs['max_count']
         if 'parameters' in kwargs.keys():
             entry['parameters'] = kwargs['parameters']
@@ -262,16 +267,19 @@
     def grouping_frequency(self, frequency: str, value: int):
         assert isinstance(value, int)
         assert isinstance(frequency, str)
         self.__grouping['grouping']['frequency'] = frequency
         self.__grouping['grouping']['value'] = value
 
     # Parallelization
-    def parallelization_add_entry(self, and_set: List):
-        self.__parallelization.append(and_set)
+    def parallelization_add_dimension(self, and_set: List):
+        self.__parallelization['parallelization']['dimensions'].append(and_set)
+
+    def parallelization_add_configuration(self, config: Dict):
+        self.__parallelization['parallelization']['configuration'].update(config)
 
     # Restrictions
     def restriction_spatial(self, permission_type: PermissionType,
                             overridable: bool,
                             geometry):
         self.__restrictions['spatial_restriction']['permission_type'] = permission_type
         self.__restrictions['spatial_restriction']['overridable'] = overridable
@@ -281,15 +289,15 @@
         self.__restrictions['temporal_restriction'] = tois
 
     def restriction_size(self):
         # TODO
         pass
 
     # Outputs
-    def outputs_add_data_types(self, output_data_types: List, observation_value_columns: List, **kwargs):
+    def outputs_add_data_types(self, output_data_types: List[str], observation_value_columns: List, **kwargs):
         self.__outputs['outputs']['output_data_types'] = output_data_types
         self.__outputs['outputs']['observation_value_columns'] = observation_value_columns
         self.__required['outputs']['output_data_types'] = True
         self.__required['outputs']['observation_value_columns'] = True
 
     # Performance Metrics
 
@@ -310,15 +318,16 @@
         manifest.update(self.__outputs)
         manifest.update(self.__manifest_version)
 
         if len(self.__performance_metrics) > 0:
             manifest.update(self.__parameters)
         if len(self.__grouping.keys()) > 0:
             manifest.update(self.__grouping)
-        if len(self.__parallelization) > 0:
+        if (self.__parallelization['parallelization']['dimensions']
+                or self.__parallelization['parallelization']['configuration']):
             manifest.update(self.__parallelization)
         if len(self.__restrictions.keys()) > 0:
             manifest.update(self.__restrictions)
         if len(self.__performance_metrics.keys()) > 0:
             manifest.update(self.__performance_metrics)
 
         for outer_key in self.__required.keys():
@@ -352,54 +361,60 @@
         }
         self.__algorithm_parameters = {
             "parameters": {}
         }
         self.__grouping = {
             "grouping": {}
         }
+        self.__parallelization_configuration = {
+            "parallelization_configuration": {}
+        }
         self.__data_sources = []
         # Set Default grouping frequency
         self.grouping_frequency(Frequency.DAILY, 1)
 
-    def add_data_source(self, data_type: DataType, data_source: DataSource, data_parameters: Dict = None):
+    def add_data_source(self, data_type: str, data_source: DataSource = None, data_parameters: Dict = None):
 
         data_type_exists = False
         for source in self.__data_sources:
             # Check if Data Type Element Exists
-            if source['data_type_name'] == data_type.value:
+            if source['data_type_name'] == data_type:
                 data_type_exists = True
                 for source_id in source['data_source_ids']:
                     if source_id == data_source.value:
                         logging.info("data source [{}] already registered.".format(data_source))
                         return
 
         if not data_type_exists:
             self.__data_sources.append({
-                "data_type_name": data_type.value,
-                "data_source_ids": [data_source.value]
+                "data_type_name": data_type,
+                "data_source_ids": [data_source.value] if data_source else []
             })
         else:
             for source in self.__data_sources:
-                if source['data_type_name'] == data_type.value:
+                if source['data_type_name'] == data_type and data_source:
                     source['data_source_ids'].append(data_source.value)
 
         if data_parameters is not None:
             for source in self.__data_sources:
-                if source['data_type_name'] == data_type.value:
+                if source['data_type_name'] == data_type:
                     source['parameters'] = data_parameters
 
         self.__required['data_sources'] = True
 
     def add_algorithm_parameter(self, key: str, value):
         for param in self.__algorithm_parameters['parameters'].keys():
             if key == param:
                 assert key != param
 
         self.__algorithm_parameters['parameters'][key] = value
 
+    def update_parallelization_configuration(self, configuration: Dict):
+        self.__parallelization_configuration['parallelization_configuration'].update(configuration)
+
     # Grouping
     def grouping_frequency(self, frequency: Frequency, value: int):
         assert isinstance(frequency, Frequency)
         assert isinstance(value, int)
         self.__grouping['grouping']['frequency'] = Frequency(frequency).name
         self.__grouping['grouping']['value'] = value
         self.__required['grouping'] = True
@@ -419,10 +434,11 @@
                 logging.info("[{}] - was not set, and is required.".format(key))
                 assert self.__required[key]
 
         algorithm_config = Struct()
         algorithm_config.update({"data_sources": self.__data_sources})
         algorithm_config.update(self.__algorithm_parameters)
         algorithm_config.update(self.__grouping)
+        algorithm_config.update(self.__parallelization_configuration)
 
         MessageToDict(algorithm_config)
         return algorithm_config
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/builder/analysis.py` & `terrascope-sdk-1.0.62/terrascope/sdk/builder/analysis.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/builder/toi.py` & `terrascope-sdk-1.0.62/terrascope/sdk/builder/toi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/terrascope_sdk.py` & `terrascope-sdk-1.0.62/terrascope/sdk/terrascope_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     client: TerrascopeAsyncClient
 
     def __init__(self, client: TerrascopeAsyncClient = None, timeout: int = None):
         if timeout is None:
             timeout = int(os.getenv('TERRASCOPE_TIMEOUT', default='60'))
         if client is None:
-            client = self.__get_client()
+            client = self.create_client()
 
         # Set Up Algo APIs
         self.algorithm = APIAlgorithm(client=client, timeout=timeout)
         self.algorithm_version = APIAlgorithmVersion(client=client, timeout=timeout)
         self.algorithm_config = APIAlgorithmConfig(client=client, timeout=timeout)
         self.algorithm_computation = APIAlgorithmComputation(client=client, timeout=timeout)
 
@@ -95,46 +95,42 @@
         # Set Up Visualization APIs
         self.visualization = APIVisualization(client=client, timeout=timeout)
 
         # Set Up User APIs
         self.user = APIUser(client=client, timeout=timeout)
 
     @staticmethod
-    def __get_client() -> TerrascopeAsyncClient:
+    def create_client(terrascope_host: str = None, terrascope_api_token: str = None) -> TerrascopeAsyncClient:
         """
         Description:
 
         Sets up the client / session once for the instance of the builder.
         All subsequent calls to this builder will use this client (session) to complete events.
 
         envs:
         OI_PAPI_HOST: url for terrascope env
         USER_TOKEN: your api key
 
         :return: TerrascopeAsyncClient object and sets the internal self to the client. Will likely not need client outside
         this classes scope.
         """
 
-        # Set client params once, then just return object as needed.
+        if not terrascope_host:
+            assert os.environ['TERRASCOPE_API_HOST'] is not None
+            terrascope_host = os.environ['TERRASCOPE_API_HOST']
 
-        assert os.environ['TERRASCOPE_HOST'] is not None
-        terrascope_host = os.environ['TERRASCOPE_HOST']
         terrascope_port_str = os.getenv('TERRASCOPE_PORT', default='443')
         terrascope_port = int(terrascope_port_str)
-        assert os.environ['TERRASCOPE_API_TOKEN'] is not None
-        terrascope_api_token = os.getenv('TERRASCOPE_API_TOKEN')
+
+        if not terrascope_api_token:
+            assert os.environ['TERRASCOPE_API_TOKEN'] is not None
+            terrascope_api_token = os.getenv('TERRASCOPE_API_TOKEN')
+
         secure_string = os.getenv('TERRASCOPE_SECURE', default='True')
         secure = True if secure_string in ['True', 'true', 'Yes', 'yes', '1'] else False
-        client = TerrascopeAsyncClient(terrascope_host, terrascope_port, api_token=terrascope_api_token, secure=secure)
 
-        return client
+        root_certificates_file = os.getenv("TERRASCOPE_API_ROOT_CERTIFICATES_FILE")
 
-    @staticmethod
-    def create_client(terrascope_host: str, terrascope_api_token: str):
-        """
-        Creates a new session client with specified host/token
+        client = TerrascopeAsyncClient(terrascope_host, terrascope_port, api_token=terrascope_api_token,
+                                       secure=secure, root_certificates_file=root_certificates_file)
 
-        :param terrascope_host:
-        :param terrascope_api_token:
-        :return: TerrascopeAsyncClient
-        """
-        return TerrascopeAsyncClient(terrascope_host, 443, api_token=terrascope_api_token, secure=True)
+        return client
```

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/tools/io.py` & `terrascope-sdk-1.0.62/terrascope/sdk/tools/io.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope/sdk/tools/sdk_support.py` & `terrascope-sdk-1.0.62/terrascope/sdk/tools/sdk_support.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/terrascope_sdk.egg-info/PKG-INFO` & `terrascope-sdk-1.0.62/terrascope_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: terrascope-sdk
-Version: 1.0.61
+Version: 1.0.62
 Summary: A software development kit for developing projects on TerraScope
-Author-email: "Martice E. Nicks III" <martice.nicks@orbitalinsight.com>
+Author-email: Orbital Insight <info@orbitalinsight.com>
 License: Copyright 2022 Orbital Insight, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -31,24 +31,33 @@
 ## Installation
 
 [Readme: Installation](https://terrascope.readme.io/docs/installation-1)
 
 ## Usage
 
 TerraScope SDK is designed to simplify access to all the [terrascope-api](https://pypi.org/project/terrascope-api/) calls
-that are available. 
+that are available. Ensure that you have the correct terrascope-api package installed.
 
 Each API uses a client object which requires the following env variables to be set:
 
 ```shell
-TERRASCOPE_HOST=terrascope-api1.orbitalinsight.com
-TERRASCOPE_TOKEN=<TerraScope API Token>
+TERRASCOPE_API_HOST=terrascope-api1.orbitalinsight.com
+TERRASCOPE_API_TOKEN=<TerraScope API Token>
 TERRASCOPE_TIMEOUT=<Int timeout in seconds> defaults to 60 seconds
 ```
 
+You will always want to ensure that you have the correct terrascope-sdk version installed. The latest can be found here:
+https://pypi.org/project/terrascope-sdk/
+
+To manually build a local version of the terrascope-sdk (for example, if you are making changes and want to test):
+1. Update the version specified in the `pyproject.toml` file, e.g. `version = "1.0.6-test"`
+2. Execute from the top-level terrascope_sdk folder: `python3 -m build`
+3. `cd dist/`
+4. `pip3 install terrascope_sdk-1.0.6-test-py3-none-any.whl` (this file name may be different based on the version specified)
+
 ## Authors and acknowledgment
 
 Orbital Insight
 
 ## License
 
 [LICENSE](LICENSE)
```

### Comparing `terrascope-sdk-1.0.61/terrascope_sdk.egg-info/SOURCES.txt` & `terrascope-sdk-1.0.62/terrascope_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,9 @@
 tests/integration/test_aoi.py
 tests/integration/test_credit.py
 tests/integration/test_data.py
 tests/integration/test_permission.py
 tests/integration/test_result.py
 tests/integration/test_sdk_support.py
 tests/integration/test_toi.py
-tests/integration/test_visualization.py
+tests/integration/test_visualization.py
+venv/bin/activate_this.py
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_algorithm.py` & `terrascope-sdk-1.0.62/tests/integration/test_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import time
 import uuid
 from datetime import datetime
-
 import pytest
-from terrascope_api.models.common_models_pb2 import Pagination
 
-from terrascope.sdk.builder.algorithm import AlgorithmManifest, InterfaceType, DataType, \
-    AlgorithmConfiguration, \
-    DataSource
+from terrascope_api.models.common_models_pb2 import Pagination
+from terrascope.sdk.builder.algorithm import (
+    AlgorithmManifest, InterfaceType, DataType, AlgorithmConfiguration, DataSource
+)
 from terrascope.sdk.builder.toi import Frequency
 from terrascope.sdk.builder.toi import TOIBuilder, TOIRuleBuilder
 from terrascope.sdk.terrascope_sdk import TerraScopeSDK
 
 
 class TestAlgorithm:
     @pytest.mark.asyncio
@@ -110,15 +109,15 @@
                                                          author=author)
             if i + 1 == int(algorithm_count / 2):
                 time.sleep(10)
                 halfway = datetime.utcnow()
             algorithm_ids.append(algorithm_model.id)
 
         # search text
-        algorithms = await sdk.algorithm.list(search_text=name, pagination=Pagination(page_size=5))
+        algorithms = await sdk.algorithm.list(search_text=name)
         assert len(algorithm_ids) == len(algorithms)
         algorithms = await sdk.algorithm.list(min_created_on=now, max_created_on=halfway)
         assert len(algorithms) == algorithm_count / 2
 
 
 class TestAlgorithmVersion:
     @pytest.mark.asyncio
@@ -135,16 +134,16 @@
         assert algorithm.name == algo_1_name
         assert algorithm.display_name == algo_1_display_name
         assert algorithm.author == algo_1_author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=2,
                                       max_count=2)
 
         manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                                command=["python",
                                                         "/orbital/base/algorithms/"
                                                         "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
@@ -179,16 +178,16 @@
 
         algorithm_version_ids = []
         for i in range(version_count):
             manifest = AlgorithmManifest()
             manifest.metadata_required(
                 description="Testing algo manifest builder",
                 version="0.0.{}".format(i))
-            manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-            manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+            manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+            manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                           min_count=2,
                                           max_count=2)
 
             manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                                    command=["python",
                                                             "/orbital/base/algorithms/"
                                                             "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
@@ -228,16 +227,16 @@
         now = datetime.utcnow()
         halfway = None
         for i in range(version_count):
             manifest = AlgorithmManifest()
             manifest.metadata_required(
                 description="Testing algo manifest builder",
                 version="0.1.{}".format(i))
-            manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-            manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+            manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+            manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                           min_count=2,
                                           max_count=2)
 
             manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                                    command=["python",
                                                             "/orbital/base/algorithms/"
                                                             "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
@@ -249,16 +248,15 @@
                                                                    algorithm_manifest=manifest)
             if i + 1 == version_count / 2:
                 halfway = datetime.utcnow()
             assert algorithm_version.id is not None
             algorithm_version_ids.append(algorithm_version.id)
 
         algorithm_versions = await sdk.algorithm_version.list(algorithm_id=algorithm.id,
-                                                              include_all_versions=True,
-                                                              pagination=Pagination(page_size=5))
+                                                              include_all_versions=True)
         assert len(algorithm_versions) == len(algorithm_version_ids)
 
         algorithm_versions = await sdk.algorithm_version.list(tag=tag_search_key, include_all_versions=True)
         assert len(algorithm_versions) == version_count
         algorithm_versions = await sdk.algorithm_version.list(min_created_on=now,
                                                               max_created_on=halfway, include_all_versions=True)
         assert len(algorithm_versions) == version_count / 2
@@ -277,16 +275,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=2,
                                       max_count=2)
 
         manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                                command=["python",
                                                         "/orbital/base/algorithms/"
                                                         "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
@@ -315,16 +313,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=2,
                                       max_count=2)
 
         manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                                command=["python",
                                                         "/orbital/base/algorithms/"
                                                         "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
@@ -356,16 +354,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=1,
                                       max_count=1)
         manifest.grouping_frequency("DAILY", 1)
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
@@ -380,15 +378,15 @@
         manifest.container_parameters_resource_request(memory_gb=5, cpu_millicore=200)
         algorithm_version = await sdk.algorithm_version.create(algorithm_id=algorithm.id,
                                                                algorithm_manifest=manifest)
 
         assert algorithm_version.id is not None
 
         configuration = AlgorithmConfiguration()
-        configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+        configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
         configuration.grouping_frequency(Frequency.WEEKLY, 1)
         algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                     name="device_visit_sdk_test_config",
                                                                     description="A test configuration.",
                                                                     algorithm_config=configuration)
 
         assert algorithm_configuration.id is not None
@@ -407,16 +405,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=1,
                                       max_count=1)
         manifest.grouping_frequency("DAILY", 1)
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
@@ -431,15 +429,15 @@
         manifest.container_parameters_resource_request(memory_gb=5, cpu_millicore=200)
         algorithm_version = await sdk.algorithm_version.create(algorithm_id=algorithm.id,
                                                                algorithm_manifest=manifest)
 
         assert algorithm_version.id is not None
 
         configuration = AlgorithmConfiguration()
-        configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+        configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
         configuration.grouping_frequency(Frequency.WEEKLY, 1)
         algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                     name="device_visit_sdk_test_config",
                                                                     description="A test configuration.",
                                                                     algorithm_config=configuration)
         assert algorithm_configuration.id is not None
 
@@ -466,16 +464,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=1,
                                       max_count=1)
 
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
@@ -491,15 +489,15 @@
         algorithm_version = await sdk.algorithm_version.create(algorithm_id=algorithm.id,
                                                                algorithm_manifest=manifest)
 
         assert algorithm_version.id is not None
         config_ids = []
         for i in range(config_count):
             configuration = AlgorithmConfiguration()
-            configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+            configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
 
             algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                         name="device_visit_sdk_test_config",
                                                                         description="A test configuration.",
                                                                         algorithm_config=configuration)
 
             assert algorithm_configuration.id is not None
@@ -526,16 +524,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=1,
                                       max_count=1)
 
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
@@ -552,27 +550,28 @@
                                                                algorithm_manifest=manifest)
 
         assert algorithm_version.id is not None
         config_ids = []
         search_me = str(uuid.uuid4())
         for i in range(config_count):
             configuration = AlgorithmConfiguration()
-            configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+            configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
 
             algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                         name="device_visit_sdk_test_config",
                                                                         description=search_me,
                                                                         algorithm_config=configuration)
 
             assert algorithm_configuration.id is not None
             config_ids.append(algorithm_configuration.id)
 
         configurations = await sdk.algorithm_config.list()
         assert len(configurations) > 0
-        configurations = await sdk.algorithm_config.list(algorithm_id=algorithm.id, pagination=Pagination(page_size=5))
+        configurations = await sdk.algorithm_config.list(algorithm_version_id=algorithm_version.id,
+                                                         include_all_versions=True)
         assert len(config_ids) == config_count == len(configurations)
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize("config_count", [
         10
     ])
     async def test_deprecate(self, config_count):
@@ -588,16 +587,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=1,
                                       max_count=1)
 
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
@@ -614,15 +613,15 @@
                                                                algorithm_manifest=manifest)
 
         assert algorithm_version.id is not None
         config_ids = []
         search_me = str(uuid.uuid4())
         for i in range(config_count):
             configuration = AlgorithmConfiguration()
-            configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+            configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
 
             algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                         name="device_visit_sdk_test_config",
                                                                         description=search_me,
                                                                         algorithm_config=configuration)
 
             assert algorithm_configuration.id is not None
@@ -650,16 +649,16 @@
         assert algorithm.name == name
         assert algorithm.display_name == display_name
         assert algorithm.author == author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=1,
                                       max_count=1)
 
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
@@ -676,15 +675,15 @@
                                                                algorithm_manifest=manifest)
 
         assert algorithm_version.id is not None
         config_ids = []
         search_me = str(uuid.uuid4())
         for i in range(config_count):
             configuration = AlgorithmConfiguration()
-            configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+            configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
 
             algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                         name="device_visit_sdk_test_config",
                                                                         description=search_me,
                                                                         algorithm_config=configuration)
 
             assert algorithm_configuration.id is not None
@@ -722,16 +721,16 @@
         device_visit_algorithm = await sdk.algorithm.create(name="device-visits-{}".format(uuid.uuid4()),
                                                             author="sdk@orbitalinsight.com",
                                                             display_name="Device Visits")
 
         logging.info(device_visit_algorithm.id)
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder", version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS)
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value)
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
         manifest.outputs_add_data_types(output_data_types=["device_visits"],
                                         observation_value_columns=["unique_device_count"])
         manifest.parameter_add(name="look_back_time", type="integer", default=3600,
@@ -739,15 +738,15 @@
         manifest.parameter_add(name="look_forward_time", type="integer", default=3600,
                                description="how far to look back")
         manifest.container_parameters_resource_request(memory_gb=5, cpu_millicore=200)
         device_visit_algorithm_version = await sdk.algorithm_version.create(algorithm_id=device_visit_algorithm.id,
                                                                             algorithm_manifest=manifest)
 
         config = AlgorithmConfiguration()
-        config.add_data_source(data_type=DataType.PINGS, data_source=DataSource.WEJO)
+        config.add_data_source(data_type=DataType.PINGS.value, data_source=DataSource.WEJO)
 
         device_visit_algorithm_config = await sdk.algorithm_config.create(
             algorithm_version_id=device_visit_algorithm_version.id,
             name="device_visit_test_{}".format(uuid.uuid4()), description="a description", algorithm_config=config)
 
         algorithm_computation = await sdk.algorithm_computation.create(
             aoi_collection_id=aoi_collection.id,
@@ -782,16 +781,16 @@
 
         device_visit_algorithm = await sdk.algorithm.create(name="device-visits-{}".format(uuid.uuid4()),
                                                             author="sdk@orbitalinsight.com",
                                                             display_name="Device Visits")
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest factory", version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS)
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value)
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
         manifest.outputs_add_data_types(output_data_types=["device_visits"],
                                         observation_value_columns=["unique_device_count"])
         manifest.parameter_add(name="look_back_time", type="integer", default=3600,
@@ -799,15 +798,15 @@
         manifest.parameter_add(name="look_forward_time", type="integer", default=3600,
                                description="how far to look back")
         manifest.container_parameters_resource_request(memory_gb=5, cpu_millicore=200)
         device_visit_algorithm_version = await sdk.algorithm_version.create(algorithm_id=device_visit_algorithm.id,
                                                                             algorithm_manifest=manifest)
 
         config = AlgorithmConfiguration()
-        config.add_data_source(data_type=DataType.PINGS, data_source=DataSource.WEJO)
+        config.add_data_source(data_type=DataType.PINGS.value, data_source=DataSource.WEJO)
 
         device_visit_algorithm_config = await sdk.algorithm_config.create(
             algorithm_version_id=device_visit_algorithm_version.id,
             name="device_visit_test_{}".format(uuid.uuid4()), description="a description", algorithm_config=config)
 
         algorithm_computation = await sdk.algorithm_computation.create(
             aoi_collection_id=aoi_collection.id,
@@ -839,16 +838,16 @@
 
         device_visit_algorithm = await sdk.algorithm.create(name="device-visits-{}".format(uuid.uuid4()),
                                                             author="sdk@orbitalinsight.com",
                                                             display_name="Device Visits")
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest factory", version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS)
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value)
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
         manifest.outputs_add_data_types(output_data_types=["device_visits"],
                                         observation_value_columns=["unique_device_count"])
         manifest.parameter_add(name="look_back_time", type="integer", default=3600,
@@ -856,15 +855,15 @@
         manifest.parameter_add(name="look_forward_time", type="integer", default=3600,
                                description="how far to look back")
         manifest.container_parameters_resource_request(memory_gb=5, cpu_millicore=200)
         device_visit_algorithm_version = await sdk.algorithm_version.create(algorithm_id=device_visit_algorithm.id,
                                                                             algorithm_manifest=manifest)
 
         config = AlgorithmConfiguration()
-        config.add_data_source(data_type=DataType.PINGS, data_source=DataSource.WEJO)
+        config.add_data_source(data_type=DataType.PINGS.value, data_source=DataSource.WEJO)
 
         device_visit_algorithm_config = await sdk.algorithm_config.create(
             algorithm_version_id=device_visit_algorithm_version.id,
             name="device_visit_test_{}".format(uuid.uuid4()), description="a description", algorithm_config=config)
 
         algorithm_computation = await sdk.algorithm_computation.create(
             aoi_collection_id=aoi_collection.id,
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_algorithm_builder.py` & `terrascope-sdk-1.0.62/tests/integration/test_algorithm_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pytest
 
-import json
 from google.protobuf.json_format import MessageToDict
 from terrascope.sdk.builder.algorithm import AlgorithmManifest, InterfaceType, DataType
 
 
 class TestAlgorithmManifest:
     @pytest.mark.asyncio
     async def test_algorithm_manifest(self):
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.1.0")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                       min_count=2)
 
         manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                                command=["python",
                                                         "/orbital/base/algorithms/"
                                                         "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
         manifest.outputs_add_data_types(output_data_types=["device_visits"],
@@ -26,16 +25,16 @@
         print(manifest_struct)
 
     @pytest.mark.asyncio
     async def test_algorithm_manifest_imagery(self):
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder for imagery",
                                    version="0.1.0")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.OPTICAL_IMAGERY, parameters={"image_processing_spec": "PL-SkySatCollect"})
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.OPTICAL_IMAGERY.value, parameters={"image_processing_spec": "PL-SkySatCollect"})
         manifest.container_parameters_required(image="orbitalinsight/skysat_ship_detector:1a354abc",
                                                command=["python",
                                                         "/orbital/base/algorithms/skysat_ship/src/py/skysat_ship_detector/simple_inference.py"])
         manifest.outputs_add_data_types(output_data_types=["object_detection"],
                                         observation_value_columns=["count"])
 
         manifest_json = MessageToDict(manifest.get())
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_analysis.py` & `terrascope-sdk-1.0.62/tests/integration/test_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 async def algorithm_version_create(algorithm_manifest_version: str, algorithm_id: str):
     sdk = TerraScopeSDK()
     manifest = AlgorithmManifest()
     manifest.metadata_required(
         description="Testing algo manifest builder",
         version=algorithm_manifest_version
     )
-    manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-    manifest.inputs_add_data_type(data_type_name=DataType.PINGS,
+    manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+    manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value,
                                   min_count=1,
                                   max_count=2)
 
     manifest.container_parameters_required(image="orbitalinsight/raw_foottraffic:84c76f7f",
                                            command=["python",
                                                     "/orbital/base/algorithms/"
                                                     "raw_foottraffic/src/py/raw_foottraffic/simple_foottraffic.py"])
@@ -54,15 +54,15 @@
     assert algorithm_version.id is not None
     return algorithm_version
 
 
 async def algorithm_config_create(algorithm_version_id: str):
     sdk = TerraScopeSDK()
     algorithm_config_build = AlgorithmConfiguration()
-    algorithm_config_build.add_data_source(data_type=DataType.PINGS, data_source=DataSource.WEJO)
+    algorithm_config_build.add_data_source(data_type=DataType.PINGS.value, data_source=DataSource.WEJO)
     algorithm_config = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version_id,
                                                          algorithm_config=algorithm_config_build,
                                                          name="test_config-{}".format(uuid.uuid4()),
                                                          description="sdk test config")
     return algorithm_config
 
 
@@ -147,228 +147,225 @@
         interval=1
     ))
     toi = await sdk.toi.create(toi_configuration.get())
     assert toi.id is not None
     return toi
 
 
-# class TestAnalysis:
-#     @pytest.mark.asyncio
-#     async def test_create(self):
-#         await analysis_create(name="integration-test-{}".format(datetime.now()), author="terrascope-sdk")
-#
-#     @pytest.mark.asyncio
-#     async def test_update(self):
-#         pass
-#
-#     @pytest.mark.asyncio
-#     @pytest.mark.parametrize("analysis_id_count", [
-#         1,
-#         10,
-#         25,
-#         45
-#     ])
-#     async def test_get(self, analysis_id_count: int):
-#         sdk = TerraScopeSDK()
-#         analysis_ids = []
-#         for i in range(analysis_id_count):
-#             analysis = await analysis_create(name="analysis_get_element_{}".format(uuid.uuid4()),
-#                                              author="terrascope-sdk-pytest")
-#             analysis_ids.append(analysis.id)
-#         assert len(analysis_ids) == analysis_id_count
-#         analyses = await sdk.analysis.get(ids=analysis_ids,
-#                                           pagination=Pagination(page_size=5))
-#         assert len(analyses) == analysis_id_count
-#
-#     @pytest.mark.asyncio
-#     @pytest.mark.parametrize("analysis_count", [
-#         10,
-#         20
-#     ])
-#     async def test_list(self, analysis_count):
-#         sdk = TerraScopeSDK()
-#         start = datetime.utcnow()
-#         halfway = None
-#         search_text = uuid.uuid4()
-#         for i in range(analysis_count):
-#             await analysis_create(name="sdk-search-me-{}-{}".format(i, search_text),
-#                                   author="terrascope-sdk-list-integration")
-#             if i + 1 == analysis_count / 2:
-#                 time.sleep(10)
-#                 halfway = datetime.utcnow()
-#
-#         results = await sdk.analysis.list(search_text=str(search_text),
-#                                           pagination=Pagination(page_size=5))
-#         assert len(results) == analysis_count
-#
-#         search_results = await sdk.analysis.list(min_created_on=start, max_created_on=halfway)
-#         assert len(search_results) == analysis_count / 2
-#
-#
-# class TestAnalysisVersion:
-#     @pytest.mark.asyncio
-#     async def test_create(self):
-#         algorithm = await algorithm_create()
-#         algorithm_version_ids = []
-#         for i in range(3):
-#             algorithm_version = await algorithm_version_create("0.0.{}".format(i + 1), algorithm.id)
-#             algorithm_version_ids.append(algorithm_version.id)
-#         analysis = await analysis_create(name="analysis-version-create-test-{}".format(uuid.uuid4()),
-#                                          author="terrascope-sdk")
-#         await analysis_version_create(analysis.id, algorithm_version_ids, [(0, 1), (1, 2)])
-#
-#     @pytest.mark.asyncio
-#     @pytest.mark.parametrize("analysis_version_id_count", [
-#         1,
-#         10,
-#         25,
-#         45
-#     ])
-#     async def test_get(self, analysis_version_id_count):
-#         sdk = TerraScopeSDK()
-#         algorithm = await algorithm_create()
-#         algorithm_version_ids = []
-#         for i in range(3):
-#             algorithm_version = await algorithm_version_create("0.0.{}".format(i + 1), algorithm.id)
-#             algorithm_version_ids.append(algorithm_version.id)
-#         analysis = await analysis_create(name="analysis-version-get-test-{}".format(datetime.now()),
-#                                               author="terrascope-sdk")
-#         analysis_version_ids = []
-#         for i in range(analysis_version_id_count):
-#             analysis_version, _ = await analysis_version_create(analysis.id, algorithm_version_ids, [(0, 1), (1, 2)])
-#             analysis_version_ids.append(analysis_version.id)
-#         assert len(analysis_version_ids) == analysis_version_id_count
-#
-#         # Algo details should fail since fake algo
-#         analysis_versions = await sdk.analysis_version.get(ids=analysis_version_ids,
-#                                                            include_manifest=True,
-#                                                            pagination=Pagination(page_size=5))
-#
-#         assert len(analysis_versions) == analysis_version_id_count
-#
-#     @pytest.mark.asyncio
-#     @pytest.mark.parametrize("analysis_version_id_count", [
-#         10,
-#         20
-#     ])
-#     async def test_list(self, analysis_version_id_count: int):
-#         sdk = TerraScopeSDK()
-#         algorithm = await algorithm_create()
-#         algorithm_version_ids = []
-#         for i in range(3):
-#             algorithm_version = await algorithm_version_create("0.0.{}".format(i + 1), algorithm.id)
-#             algorithm_version_ids.append(algorithm_version.id)
-#         analysis = await analysis_create(name="analysis-version-list-test-{}".format(datetime.now()),
-#                                               author="terrascope-sdk")
-#
-#         min_created_on = datetime.utcnow()
-#         max_created_on = None
-#         analysis_version_ids = []
-#         for i in range(analysis_version_id_count):
-#             analysis_version, _ = await analysis_version_create(analysis.id, algorithm_version_ids, [(0, 1), (1, 2)])
-#             if i == (analysis_version_id_count / 2) - 1:
-#                 time.sleep(10)
-#                 max_created_on = datetime.utcnow()
-#
-#             analysis_version_ids.append(analysis_version.id)
-#
-#         analysis_versions = await sdk.analysis_version.list(analysis_id=analysis.id, include_all_versions=False)
-#
-#         assert len(analysis_versions) == 1
-#
-#         analysis_versions = await sdk.analysis_version.list(analysis_id=analysis.id,
-#                                                             include_all_versions=True)
-#         assert len(analysis_versions) == len(analysis_version_ids)
-#         for version in analysis_versions:
-#             assert version.analysis_id == analysis.id
-#
-#         analysis_versions = await sdk.analysis_version.list(min_created_on=min_created_on,
-#                                                             max_created_on=max_created_on,
-#                                                             include_all_versions=True,
-#                                                             pagination=Pagination(page_size=5))
-#         assert len(analysis_versions) == analysis_version_id_count / 2
-#
-#     @pytest.mark.asyncio
-#     async def test_deprecate(self):
-#         pass
-#
-#     @pytest.mark.asyncio
-#     async def test_deactivate(self):
-#         pass
-#
-#
+class TestAnalysis:
+    @pytest.mark.asyncio
+    async def test_create(self):
+        await analysis_create(name="integration-test-{}".format(datetime.now()), author="terrascope-sdk")
+
+    @pytest.mark.asyncio
+    async def test_update(self):
+        pass
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("analysis_id_count", [
+        1,
+        10,
+        25,
+        45
+    ])
+    async def test_get(self, analysis_id_count: int):
+        sdk = TerraScopeSDK()
+        analysis_ids = []
+        for i in range(analysis_id_count):
+            analysis = await analysis_create(name="analysis_get_element_{}".format(uuid.uuid4()),
+                                             author="terrascope-sdk-pytest")
+            analysis_ids.append(analysis.id)
+        assert len(analysis_ids) == analysis_id_count
+        analyses = await sdk.analysis.get(ids=analysis_ids,
+                                          pagination=Pagination(page_size=5))
+        assert len(analyses) == analysis_id_count
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("analysis_count", [
+        10,
+        20
+    ])
+    async def test_list(self, analysis_count):
+        sdk = TerraScopeSDK()
+        start = datetime.utcnow()
+        halfway = None
+        search_text = uuid.uuid4()
+        for i in range(analysis_count):
+            await analysis_create(name="sdk-search-me-{}-{}".format(i, search_text),
+                                  author="terrascope-sdk-list-integration")
+            if i + 1 == analysis_count / 2:
+                time.sleep(10)
+                halfway = datetime.utcnow()
+
+        results = await sdk.analysis.list(search_text=str(search_text))
+        assert len(results) == analysis_count
+
+        search_results = await sdk.analysis.list(min_created_on=start, max_created_on=halfway)
+        assert len(search_results) == analysis_count / 2
+
+
+class TestAnalysisVersion:
+    @pytest.mark.asyncio
+    async def test_create(self):
+        algorithm = await algorithm_create()
+        algorithm_version_ids = []
+        for i in range(3):
+            algorithm_version = await algorithm_version_create("0.0.{}".format(i + 1), algorithm.id)
+            algorithm_version_ids.append(algorithm_version.id)
+        analysis = await analysis_create(name="analysis-version-create-test-{}".format(uuid.uuid4()),
+                                         author="terrascope-sdk")
+        await analysis_version_create(analysis.id, algorithm_version_ids, [(0, 1), (1, 2)])
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("analysis_version_id_count", [
+        1,
+        10,
+        25,
+        45
+    ])
+    async def test_get(self, analysis_version_id_count):
+        sdk = TerraScopeSDK()
+        algorithm = await algorithm_create()
+        algorithm_version_ids = []
+        for i in range(3):
+            algorithm_version = await algorithm_version_create("0.0.{}".format(i + 1), algorithm.id)
+            algorithm_version_ids.append(algorithm_version.id)
+        analysis = await analysis_create(name="analysis-version-get-test-{}".format(datetime.now()),
+                                              author="terrascope-sdk")
+        analysis_version_ids = []
+        for i in range(analysis_version_id_count):
+            analysis_version, _ = await analysis_version_create(analysis.id, algorithm_version_ids, [(0, 1), (1, 2)])
+            analysis_version_ids.append(analysis_version.id)
+        assert len(analysis_version_ids) == analysis_version_id_count
+
+        # Algo details should fail since fake algo
+        analysis_versions = await sdk.analysis_version.get(ids=analysis_version_ids,
+                                                           include_manifest=True,
+                                                           pagination=Pagination(page_size=5))
+
+        assert len(analysis_versions) == analysis_version_id_count
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("analysis_version_id_count", [
+        10,
+        20
+    ])
+    async def test_list(self, analysis_version_id_count: int):
+        sdk = TerraScopeSDK()
+        algorithm = await algorithm_create()
+        algorithm_version_ids = []
+        for i in range(3):
+            algorithm_version = await algorithm_version_create("0.0.{}".format(i + 1), algorithm.id)
+            algorithm_version_ids.append(algorithm_version.id)
+        analysis = await analysis_create(name="analysis-version-list-test-{}".format(datetime.now()),
+                                              author="terrascope-sdk")
+
+        min_created_on = datetime.utcnow()
+        max_created_on = None
+        analysis_version_ids = []
+        for i in range(analysis_version_id_count):
+            analysis_version, _ = await analysis_version_create(analysis.id, algorithm_version_ids, [(0, 1), (1, 2)])
+            if i == (analysis_version_id_count / 2) - 1:
+                time.sleep(10)
+                max_created_on = datetime.utcnow()
+
+            analysis_version_ids.append(analysis_version.id)
+
+        analysis_versions = await sdk.analysis_version.list(analysis_id=analysis.id, include_all_versions=False)
+
+        assert len(analysis_versions) == 1
+
+        analysis_versions = await sdk.analysis_version.list(analysis_id=analysis.id,
+                                                            include_all_versions=True)
+        assert len(analysis_versions) == len(analysis_version_ids)
+        for version in analysis_versions:
+            assert version.analysis_id == analysis.id
+
+        analysis_versions = await sdk.analysis_version.list(min_created_on=min_created_on,
+                                                            max_created_on=max_created_on,
+                                                            include_all_versions=True)
+        assert len(analysis_versions) == analysis_version_id_count / 2
+
+    @pytest.mark.asyncio
+    async def test_deprecate(self):
+        pass
+
+    @pytest.mark.asyncio
+    async def test_deactivate(self):
+        pass
+
+
 class TestAnalysisConfig:
     @pytest.mark.asyncio
-#     async def test_create(self):
-#         algorithm = await algorithm_create()
-#         algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
-#         analysis = await analysis_create(name="analysis-config-create-test-{}".format(datetime.now()),
-#                                               author="terrascope-sdk")
-#         analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
-#         algorithm_config = await algorithm_config_create(algorithm_version.id)
-#         await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
-#
-#     @pytest.mark.asyncio
-#     async def test_update(self):
-#         pass
-#
-#     @pytest.mark.asyncio
-#     @pytest.mark.parametrize("config_count", [
-#         1,
-#         10,
-#         25,
-#         45
-#     ])
-#     async def test_get(self, config_count: int):
-#         sdk = TerraScopeSDK()
-#         algorithm = await algorithm_create()
-#         algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
-#         analysis = await analysis_create(name="analysis-config-get-test-{}".format(datetime.now()),
-#                                               author="terrascope-sdk")
-#         analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
-#         algorithm_config = await algorithm_config_create(algorithm_version.id)
-#         analysis_config_ids = []
-#         for i in range(config_count):
-#             analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
-#             analysis_config_ids.append(analysis_config.id)
-#
-#         analysis_configs = await sdk.analysis_config.get(ids=analysis_config_ids,
-#                                                          include_algorithm_details=False,
-#                                                          pagination=Pagination(page_size=5))
-#
-#         assert len(analysis_configs) == config_count
-#
-#     @pytest.mark.asyncio
-#     @pytest.mark.parametrize("config_count", [
-#         1,
-#         10,
-#         25
-#     ])
-#     async def test_list(self, config_count: int):
-#         sdk = TerraScopeSDK()
-#         algorithm = await algorithm_create()
-#         algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
-#         analysis = await analysis_create(name="analysis-config-list-test-{}".format(datetime.now()),
-#                                               author="terrascope-sdk")
-#         analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
-#         algorithm_config = await algorithm_config_create(algorithm_version.id)
-#
-#         analysis_config_ids = []
-#         for i in range(config_count):
-#             analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
-#             analysis_config_ids.append(analysis_config.id)
-#
-#         analysis_configs = await sdk.analysis_config.list(analysis_version_id=analysis_version.id,
-#                                                           pagination=Pagination(page_size=5))
-#         assert len(analysis_configs) == config_count
-#
-#     @pytest.mark.asyncio
-#     async def test_deprecate(self):
-#         pass
-#
+    async def test_create(self):
+        algorithm = await algorithm_create()
+        algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
+        analysis = await analysis_create(name="analysis-config-create-test-{}".format(datetime.now()),
+                                              author="terrascope-sdk")
+        analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
+        algorithm_config = await algorithm_config_create(algorithm_version.id)
+        await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
+
+    @pytest.mark.asyncio
+    async def test_update(self):
+        pass
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("config_count", [
+        1,
+        10,
+        25,
+        45
+    ])
+    async def test_get(self, config_count: int):
+        sdk = TerraScopeSDK()
+        algorithm = await algorithm_create()
+        algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
+        analysis = await analysis_create(name="analysis-config-get-test-{}".format(datetime.now()),
+                                              author="terrascope-sdk")
+        analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
+        algorithm_config = await algorithm_config_create(algorithm_version.id)
+        analysis_config_ids = []
+        for i in range(config_count):
+            analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
+            analysis_config_ids.append(analysis_config.id)
+
+        analysis_configs = await sdk.analysis_config.get(ids=analysis_config_ids,
+                                                         include_algorithm_details=False,
+                                                         pagination=Pagination(page_size=5))
+
+        assert len(analysis_configs) == config_count
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("config_count", [
+        1,
+        10,
+        25
+    ])
+    async def test_list(self, config_count: int):
+        sdk = TerraScopeSDK()
+        algorithm = await algorithm_create()
+        algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
+        analysis = await analysis_create(name="analysis-config-list-test-{}".format(datetime.now()),
+                                              author="terrascope-sdk")
+        analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
+        algorithm_config = await algorithm_config_create(algorithm_version.id)
+
+        analysis_config_ids = []
+        for i in range(config_count):
+            analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
+            analysis_config_ids.append(analysis_config.id)
+
+        analysis_configs = await sdk.analysis_config.list(analysis_version_id=analysis_version.id)
+        assert len(analysis_configs) == config_count
+
+    @pytest.mark.asyncio
+    async def test_deprecate(self):
+        pass
+
     @pytest.mark.asyncio
     @pytest.mark.parametrize("config_count", [
         1,
         10,
         25
     ])
     @pytest.mark.asyncio
@@ -384,105 +381,103 @@
         analysis_config_ids = []
         for i in range(config_count):
             analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
             analysis_config_ids.append(analysis_config.id)
 
         # DEACTIVATE ANALYSIS CONFIG
         await sdk.analysis_config.deactivate(analysis_config_ids)
-        import pdb
-        pdb.set_trace()
 
         # Check that List request doesn't return de-activated Analysis Configs unless specified
         analysis_configs = await sdk.analysis_config.list(analysis_version_id=analysis_version.id)
         assert len(analysis_configs) == 0
         analysis_configs = await sdk.analysis_config.list(analysis_version_id=analysis_version.id,
                                                           include_deactivated=True)
         assert len(analysis_configs) == config_count
 
         # Check that Analysis Configs can still be queried through the get request, but has deactivated flag set
         analysis_configs = await sdk.analysis_config.get(ids=analysis_config_ids, include_algorithm_details=False)
         assert all([analysis_config.is_deactivated for analysis_config in analysis_configs])
-#
-#     @pytest.mark.asyncio
-#     async def test_delete(self):
-#         pass
-#
-#
-# class TestAnalysisComputation:
-#     @pytest.mark.asyncio
-#     async def test_create(self):
-#         # SETUP ALGORITHM
-#         algorithm = await algorithm_create()
-#         algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
-#         algorithm_config = await algorithm_config_create(algorithm_version.id)
-#
-#         # SETUP ANALYSIS
-#         name = "analysis-computation-create-test-{}".format(datetime.now())
-#         analysis = await analysis_create(name=name, author="terrascope-sdk")
-#         analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
-#         analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
-#
-#         # SETUP AOI
-#         aoi_collection = await aoi_collection_create(name)
-#
-#         # SETUP TOI
-#         toi = await toi_create()
-#
-#         # SETUP ANALYSIS COMPUTATION
-#         await analysis_computation_create(analysis_config.id, toi.id, aoi_collection.id)
-#
-#     @pytest.mark.asyncio
-#     async def test_run(self):
-#         sdk = TerraScopeSDK()
-#         # SETUP ALGORITHM
-#         algorithm = await algorithm_create()
-#         algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
-#         algorithm_config = await algorithm_config_create(algorithm_version.id)
-#
-#         # SETUP ANALYSIS
-#         name = "analysis-computation-run-test-{}".format(datetime.now())
-#         analysis = await analysis_create(name=name, author="terrascope-sdk")
-#         analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
-#         analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
-#
-#         # SETUP AOI
-#         aoi_collection = await aoi_collection_create(name)
-#
-#         # SETUP TOI
-#         toi = await toi_create()
-#
-#         # SETUP ANALYSIS COMPUTATION
-#         analysis_computation = await analysis_computation_create(analysis_config.id, toi.id, aoi_collection.id)
-#
-#         # RUN ANALYSIS COMPUTATION
-#         await sdk.analysis_computation.run([analysis_computation.id])
-#
-#     @pytest.mark.asyncio
-#     async def test_get(self):
-#         sdk = TerraScopeSDK()
-#         # SETUP ALGORITHM
-#         algorithm = await algorithm_create()
-#         algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
-#         algorithm_config = await algorithm_config_create(algorithm_version.id)
-#
-#         # SETUP ANALYSIS
-#         name = "analysis-computation-get-test-{}".format(datetime.now())
-#         analysis = await analysis_create(name=name, author="terrascope-sdk")
-#         analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
-#         analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
-#
-#         # SETUP AOI
-#         aoi_collection = await aoi_collection_create(name)
-#
-#         # SETUP TOI
-#         toi = await toi_create()
-#
-#         # SETUP ANALYSIS COMPUTATION
-#         analysis_computation = await analysis_computation_create(analysis_config.id, toi.id, aoi_collection.id)
-#
-#         # GET ANALYSIS COMPUTATION
-#         analysis_computation = await sdk.analysis_computation.get([analysis_computation.id])
-#         assert analysis_computation is not None
-#
-#     @pytest.mark.asyncio
-#     async def test_list(self):
-#         pass
+
+    @pytest.mark.asyncio
+    async def test_delete(self):
+        pass
+
+
+class TestAnalysisComputation:
+    @pytest.mark.asyncio
+    async def test_create(self):
+        # SETUP ALGORITHM
+        algorithm = await algorithm_create()
+        algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
+        algorithm_config = await algorithm_config_create(algorithm_version.id)
+
+        # SETUP ANALYSIS
+        name = "analysis-computation-create-test-{}".format(datetime.now())
+        analysis = await analysis_create(name=name, author="terrascope-sdk")
+        analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
+        analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
+
+        # SETUP AOI
+        aoi_collection = await aoi_collection_create(name)
+
+        # SETUP TOI
+        toi = await toi_create()
+
+        # SETUP ANALYSIS COMPUTATION
+        await analysis_computation_create(analysis_config.id, toi.id, aoi_collection.id)
+
+    @pytest.mark.asyncio
+    async def test_run(self):
+        sdk = TerraScopeSDK()
+        # SETUP ALGORITHM
+        algorithm = await algorithm_create()
+        algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
+        algorithm_config = await algorithm_config_create(algorithm_version.id)
+
+        # SETUP ANALYSIS
+        name = "analysis-computation-run-test-{}".format(datetime.now())
+        analysis = await analysis_create(name=name, author="terrascope-sdk")
+        analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
+        analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
+
+        # SETUP AOI
+        aoi_collection = await aoi_collection_create(name)
+
+        # SETUP TOI
+        toi = await toi_create()
+
+        # SETUP ANALYSIS COMPUTATION
+        analysis_computation = await analysis_computation_create(analysis_config.id, toi.id, aoi_collection.id)
+
+        # RUN ANALYSIS COMPUTATION
+        await sdk.analysis_computation.run([analysis_computation.id])
+
+    @pytest.mark.asyncio
+    async def test_get(self):
+        sdk = TerraScopeSDK()
+        # SETUP ALGORITHM
+        algorithm = await algorithm_create()
+        algorithm_version = await algorithm_version_create("0.0.1", algorithm.id)
+        algorithm_config = await algorithm_config_create(algorithm_version.id)
+
+        # SETUP ANALYSIS
+        name = "analysis-computation-get-test-{}".format(datetime.now())
+        analysis = await analysis_create(name=name, author="terrascope-sdk")
+        analysis_version, manifest = await analysis_version_create(analysis.id, [algorithm_version.id], [])
+        analysis_config = await analysis_config_create(analysis_version.id, algorithm_config.id, manifest)
+
+        # SETUP AOI
+        aoi_collection = await aoi_collection_create(name)
+
+        # SETUP TOI
+        toi = await toi_create()
+
+        # SETUP ANALYSIS COMPUTATION
+        analysis_computation = await analysis_computation_create(analysis_config.id, toi.id, aoi_collection.id)
+
+        # GET ANALYSIS COMPUTATION
+        analysis_computation = await sdk.analysis_computation.get([analysis_computation.id])
+        assert analysis_computation is not None
+
+    @pytest.mark.asyncio
+    async def test_list(self):
+        pass
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_analysis_builder.py` & `terrascope-sdk-1.0.62/tests/integration/test_analysis_builder.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_aoi.py` & `terrascope-sdk-1.0.62/tests/integration/test_aoi.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_credit.py` & `terrascope-sdk-1.0.62/tests/integration/test_credit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import uuid
 from datetime import datetime
 
 import pytest
 
 from terrascope.sdk.builder.toi import TOIBuilder, TOIRuleBuilder, Frequency
-from terrascope.sdk.builder.algorithm import AlgorithmManifest, InterfaceType, DataType, \
-    AlgorithmConfiguration, \
-    DataSource
+from terrascope.sdk.builder.algorithm import (
+    AlgorithmManifest, InterfaceType, DataType, AlgorithmConfiguration, DataSource
+)
 from terrascope.sdk.terrascope_sdk import TerraScopeSDK
 
 
 class TestCredit:
     @pytest.mark.asyncio
     async def test_estimate(self):
         sdk = TerraScopeSDK()
@@ -32,16 +32,16 @@
 
         device_visit_algorithm = await sdk.algorithm.create(name="device-visits-{}".format(uuid.uuid4()),
                                                             author="sdk@orbitalinsight.com",
                                                             display_name="Device Visits")
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder", version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS)
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value)
         manifest.container_parameters_required(image="orbitalinsight/device_visits:5a579e59",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
         manifest.outputs_add_data_types(output_data_types=["device_visits"],
                                         observation_value_columns=["unique_device_count"])
         manifest.parameter_add(name="look_back_time", type="integer", default=3600,
@@ -53,15 +53,15 @@
                                                                             algorithm_manifest=manifest)
 
         await sdk.credit.set_algorithm(algorithm_version_id=device_visit_algorithm_version.id,
                                        algorithm_execution_price=0.01,
                                        algorithm_value_price=0.01)
 
         config = AlgorithmConfiguration()
-        config.add_data_source(data_type=DataType.PINGS, data_source=DataSource.WEJO)
+        config.add_data_source(data_type=DataType.PINGS.value, data_source=DataSource.WEJO)
 
         device_visit_algorithm_config = await sdk.algorithm_config.create(
             algorithm_version_id=device_visit_algorithm_version.id,
             name="device_visit_test_{}".format(uuid.uuid4()), description="a description", algorithm_config=config)
 
         algorithm_computation = await sdk.algorithm_computation.create(
             aoi_collection_id=aoi_collection.id,
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_data.py` & `terrascope-sdk-1.0.62/tests/integration/test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from terrascope.sdk.terrascope_sdk import TerraScopeSDK
 
 
 class TestDataSource:
     @pytest.mark.asyncio
     async def test_get(self):
         sdk = TerraScopeSDK()
-        ids = ["blogwatcher_track_pings", "adsbx_track_pings"]
+        ids = ["blogwatcher_pings", "adsbx_pings"]
         sources = await sdk.data_source.get(ids=ids)
         assert len(sources) == len(ids)
 
     @pytest.mark.asyncio
     async def test_list(self):
         sdk = TerraScopeSDK()
         data_sources = await sdk.data_source.list()
@@ -36,8 +36,8 @@
 
         data_types = await sdk.data_type.list(search_text="ping")
         assert len(data_types) == 2
 
     @pytest.mark.asyncio
     async def test_create(self):
         sdk = TerraScopeSDK()
-        data_type = await sdk.data_type.create(name="test_data_type", description="test description", schema="", data_source_ids=[])
+        data_type = await sdk.data_type.create(name="test_data_type", description="test description", schema="", data_source_ids=[])
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_permission.py` & `terrascope-sdk-1.0.62/tests/integration/test_permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import uuid
 
 import pytest
 from terrascope_api.models.permission_pb2 import Permission
 
-from terrascope.sdk.builder.algorithm import AlgorithmManifest, AlgorithmConfiguration, DataType, DataSource, \
-    InterfaceType
+from terrascope.sdk.builder.algorithm import AlgorithmManifest, AlgorithmConfiguration, DataType, InterfaceType
 from terrascope.sdk.builder.analysis import AnalysisManifest
 from terrascope.sdk.terrascope_sdk import TerraScopeSDK
 
 
 class TestPermission:
 
     def __init__(self):
@@ -25,25 +24,25 @@
         algorithm_id = algorithm.id
         self.algorithm_id = algorithm_id
         print('algo id:', algorithm_id)
 
         # Algorithm Version (not shareable, to feed to config)
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="test-manifest", version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.NO_OP_WORKER)
-        manifest.inputs_add_data_type(DataType.TRACK_PINGS)
-        manifest.outputs_add_data_types(output_data_types=["device_tracks"],
+        manifest.interface_required(interface_type=InterfaceType.NO_OP_WORKER.value)
+        manifest.inputs_add_data_type(DataType.DEVICE_VISITS.value)
+        manifest.outputs_add_data_types(output_data_types=[DataType.DEVICE_TRACKS.value],
                                         observation_value_columns=["device_tracks"])
         manifest.container_parameters_required(image="", command=[])
         algorithm_version = await sdk.algorithm_version.create(algorithm_id=algorithm_id, algorithm_manifest=manifest)
         print('algo version id:', algorithm_version.id)
 
         # Algorithm Config
         configuration = AlgorithmConfiguration()
-        configuration.add_data_source(data_type=DataType.TRACK_PINGS, data_source=DataSource.SAFEGRAPH_TRACKS)
+        configuration.add_data_source(data_type=DataType.DEVICE_VISITS.value)
         algo_config = await sdk.algorithm_config.create(
             algorithm_version_id=algorithm_version.id,
             name="Permission Test Config",
             description="Permission Test Config",
             algorithm_config=configuration)
         algo_config_id = algo_config.id
         self.algo_config_id = algo_config_id
@@ -109,12 +108,12 @@
             pass
         elif resource_type == Permission.ResourceType.TOI:
             pass
         elif resource_type == Permission.ResourceType.AOI_COLLECTION:
             pass
 
         response = sdk.permission.create(resource_ids=[resource_id], resource_type=resource_type,
-                                         permission_type=permission_type, user_ids=["test_user1@oi.com"],
+                                         permission_type=permission_type, user_emails=["test_user1@oi.com"],
                                          public=False, public_confirm=False)
 
         assert response is not None
         assert 200 <= response.status_code < 300
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_result.py` & `terrascope-sdk-1.0.62/tests/integration/test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os.path
 import uuid
-from datetime import datetime
-
 import pytest
+import os.path
+import logging
+from datetime import datetime
 
 from terrascope.sdk.builder.toi import TOIBuilder, TOIRuleBuilder, Frequency
-from terrascope.sdk.builder.algorithm import AlgorithmManifest, AlgorithmConfiguration, \
-    InterfaceType, DataType, DataSource
+from terrascope.sdk.builder.algorithm import (
+    AlgorithmManifest, AlgorithmConfiguration, InterfaceType, DataType, DataSource
+)
 from terrascope.sdk.builder.analysis import AnalysisManifest, AnalysisConfiguration
 from terrascope.sdk.terrascope_sdk import TerraScopeSDK
 
-import logging
 
 class TestResult:
 
     @pytest.mark.asyncio
     # @pytest.mark.parametrize()
     async def test_result_get_export(self):
         # SETUP ALGORITHM
@@ -30,16 +30,16 @@
         assert algorithm.name == algorithm_name
         assert algorithm.display_name == algorithm_display_name
         assert algorithm.author == algorithm_author
 
         manifest = AlgorithmManifest()
         manifest.metadata_required(description="Testing algo manifest builder",
                                    version="0.0.1")
-        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER)
-        manifest.inputs_add_data_type(data_type_name=DataType.PINGS)
+        manifest.interface_required(interface_type=InterfaceType.FILESYSTEM_TASK_WORKER.value)
+        manifest.inputs_add_data_type(data_type_name=DataType.PINGS.value)
 
         manifest.container_parameters_required(image="orbitalinsight/device_visits:1d77d321",
                                                command=["python",
                                                         "/orbital/base/algorithms/device_visits/src/py/"
                                                         "device_visits/device_visits.py"])
         manifest.outputs_add_data_types(output_data_types=["device_visits"],
                                         observation_value_columns=["device_visits"])
@@ -55,15 +55,15 @@
 
         assert algorithm_version.id is not None
         await sdk.credit.set_algorithm(algorithm_version_id=algorithm_version.id,
                                        algorithm_execution_price=1.0,
                                        algorithm_value_price=0.0)
 
         configuration = AlgorithmConfiguration()
-        configuration.add_data_source(DataType.PINGS, DataSource.WEJO)
+        configuration.add_data_source(DataType.PINGS.value, DataSource.WEJO)
 
         algorithm_configuration = await sdk.algorithm_config.create(algorithm_version_id=algorithm_version.id,
                                                                     name="device_visit_sdk_test_config",
                                                                     description="A test configuration.",
                                                                     algorithm_config=configuration)
         # AOI Setup
         aoi_collection = await sdk.aoi_collection.create(aoi_collection_name=str(uuid.uuid4()))
```

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_sdk_support.py` & `terrascope-sdk-1.0.62/tests/integration/test_sdk_support.py`

 * *Files identical despite different names*

### Comparing `terrascope-sdk-1.0.61/tests/integration/test_toi.py` & `terrascope-sdk-1.0.62/tests/integration/test_toi.py`

 * *Files identical despite different names*

