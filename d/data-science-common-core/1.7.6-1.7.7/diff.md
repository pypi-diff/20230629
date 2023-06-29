# Comparing `tmp/data-science-common-core-1.7.6.tar.gz` & `tmp/data-science-common-core-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-science-common-core-1.7.6.tar", max compression
+gzip compressed data, was "data-science-common-core-1.7.7.tar", max compression
```

## Comparing `data-science-common-core-1.7.6.tar` & `data-science-common-core-1.7.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.6/common/__init__.py
--rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.6/common/catrf.py
--rw-r--r--   0        0        0     2343 2023-06-06 12:45:28.311456 data-science-common-core-1.7.6/common/constants.py
--rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.6/common/custom_hgb.py
--rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.6/common/custom_multi.py
--rw-r--r--   0        0        0    17492 2023-06-06 11:26:49.982009 data-science-common-core-1.7.6/common/ft.py
--rw-r--r--   0        0        0    12414 2023-06-02 13:30:43.079972 data-science-common-core-1.7.6/common/io.py
--rw-r--r--   0        0        0    27223 2023-06-06 12:45:28.311861 data-science-common-core-1.7.6/common/logic.py
--rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.6/common/model.py
--rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.6/common/pipeline.py
--rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.6/common/plot.py
--rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.6/common/query.py
--rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.6/common/setup.py
--rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.6/common/transformer.py
--rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.6/common/utils.py
--rw-r--r--   0        0        0     1089 2023-06-06 12:45:28.312147 data-science-common-core-1.7.6/pyproject.toml
--rw-r--r--   0        0        0     1343 2023-06-06 12:45:35.809176 data-science-common-core-1.7.6/setup.py
--rw-r--r--   0        0        0     1479 2023-06-06 12:45:35.809364 data-science-common-core-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0       31 2022-08-16 12:51:34.846327 data-science-common-core-1.7.7/common/__init__.py
+-rw-r--r--   0        0        0     1772 2023-01-04 09:26:13.978265 data-science-common-core-1.7.7/common/catrf.py
+-rw-r--r--   0        0        0     2343 2023-06-06 12:45:28.311456 data-science-common-core-1.7.7/common/constants.py
+-rw-r--r--   0        0        0    28618 2022-09-16 13:05:55.366098 data-science-common-core-1.7.7/common/custom_hgb.py
+-rw-r--r--   0        0        0    14915 2022-10-06 09:48:34.061975 data-science-common-core-1.7.7/common/custom_multi.py
+-rw-r--r--   0        0        0    17492 2023-06-06 11:26:49.982009 data-science-common-core-1.7.7/common/ft.py
+-rw-r--r--   0        0        0    12414 2023-06-02 13:30:43.079972 data-science-common-core-1.7.7/common/io.py
+-rw-r--r--   0        0        0    27223 2023-06-06 12:45:28.311861 data-science-common-core-1.7.7/common/logic.py
+-rw-r--r--   0        0        0    15836 2023-01-04 09:26:13.980885 data-science-common-core-1.7.7/common/model.py
+-rw-r--r--   0        0        0     1013 2023-06-02 13:30:43.080198 data-science-common-core-1.7.7/common/pipeline.py
+-rw-r--r--   0        0        0    11465 2023-06-02 13:30:43.082632 data-science-common-core-1.7.7/common/plot.py
+-rw-r--r--   0        0        0     2100 2022-09-08 15:24:02.191811 data-science-common-core-1.7.7/common/query.py
+-rw-r--r--   0        0        0     6947 2023-01-04 09:26:13.981645 data-science-common-core-1.7.7/common/setup.py
+-rw-r--r--   0        0        0     2639 2023-06-02 13:30:43.082938 data-science-common-core-1.7.7/common/transformer.py
+-rw-r--r--   0        0        0     8736 2022-11-25 15:53:01.257516 data-science-common-core-1.7.7/common/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-29 13:14:22.427390 data-science-common-core-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0     1350 2023-06-29 13:14:26.935450 data-science-common-core-1.7.7/setup.py
+-rw-r--r--   0        0        0     1486 2023-06-29 13:14:26.935620 data-science-common-core-1.7.7/PKG-INFO
```

### Comparing `data-science-common-core-1.7.6/common/catrf.py` & `data-science-common-core-1.7.7/common/catrf.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/constants.py` & `data-science-common-core-1.7.7/common/constants.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/custom_hgb.py` & `data-science-common-core-1.7.7/common/custom_hgb.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/custom_multi.py` & `data-science-common-core-1.7.7/common/custom_multi.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/ft.py` & `data-science-common-core-1.7.7/common/ft.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/io.py` & `data-science-common-core-1.7.7/common/io.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/logic.py` & `data-science-common-core-1.7.7/common/logic.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/model.py` & `data-science-common-core-1.7.7/common/model.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/pipeline.py` & `data-science-common-core-1.7.7/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/plot.py` & `data-science-common-core-1.7.7/common/plot.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/query.py` & `data-science-common-core-1.7.7/common/query.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/setup.py` & `data-science-common-core-1.7.7/common/setup.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/transformer.py` & `data-science-common-core-1.7.7/common/transformer.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/common/utils.py` & `data-science-common-core-1.7.7/common/utils.py`

 * *Files identical despite different names*

### Comparing `data-science-common-core-1.7.6/pyproject.toml` & `data-science-common-core-1.7.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "data-science-common-core"
-version = "1.7.6"
+version = "1.7.7"
 description = "Data Science Common Core"
-authors = ["Unsal Gokdag <unsal.gokdag@forto.com>", "PietroAnsidei <pietro.ansidei@forto.com>", "Naomi Nguyen <naomi.nguyen@forto.com>", "Kumar Rajendrababu <kumar.rajendrababu@forto.com>"]
+authors = ["Unsal Gokdag <unsal.gokdag@forto.com>", "Naomi Nguyen <naomi.nguyen@forto.com>", "Kumar Rajendrababu <kumar.rajendrababu@forto.com>", "Reet Kanjilal <reet.kanjilal@forto.com>"]
 packages = [
     { include = "common/*.py"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 google-cloud-bigquery-storage = "^2.14.1"
@@ -25,15 +25,15 @@
 imblearn = "^0.0"
 protobuf = "^3.20.1"
 pgzip = "^0.3.1"
 toml = "^0.10.2"
 webencodings = "^0.5.1"
 pkginfo = "^1.8.3"
 catboost = "^1.0.6"
-grpcio = "1.51.1"
+grpcio = "^1.56.0"
 scipy = "^1.9.3"
 tomli = "^2.0.1"
 importlib-metadata = "^5.2.0"
 setuptools = "^65.6.3"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `data-science-common-core-1.7.6/setup.py` & `data-science-common-core-1.7.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = \
 ['catboost>=1.0.6,<2.0.0',
  'db-dtypes>=1.0.2,<2.0.0',
  'google-cloud-bigquery-storage>=2.14.1,<3.0.0',
  'google-cloud-bigquery>=3.2.0,<4.0.0',
  'google-cloud-storage>=2.4.0,<3.0.0',
- 'grpcio==1.51.1',
+ 'grpcio>=1.56.0,<2.0.0',
  'gspread-dataframe>=3.3.0,<4.0.0',
  'gspread>=5.4.0,<6.0.0',
  'imblearn>=0.0,<0.1',
  'importlib-metadata>=5.2.0,<6.0.0',
  'matplotlib>=3.5.2,<4.0.0',
  'pandas>=1.4.3,<2.0.0',
  'pgzip>=0.3.1,<0.4.0',
@@ -32,15 +32,15 @@
  'toml>=0.10.2,<0.11.0',
  'tomli>=2.0.1,<3.0.0',
  'tqdm>=4.64.0,<5.0.0',
  'webencodings>=0.5.1,<0.6.0']
 
 setup_kwargs = {
     'name': 'data-science-common-core',
-    'version': '1.7.6',
+    'version': '1.7.7',
     'description': 'Data Science Common Core',
     'long_description': None,
     'author': 'Unsal Gokdag',
     'author_email': 'unsal.gokdag@forto.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `data-science-common-core-1.7.6/PKG-INFO` & `data-science-common-core-1.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: data-science-common-core
-Version: 1.7.6
+Version: 1.7.7
 Summary: Data Science Common Core
 Author: Unsal Gokdag
 Author-email: unsal.gokdag@forto.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: catboost (>=1.0.6,<2.0.0)
 Requires-Dist: db-dtypes (>=1.0.2,<2.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.2.0,<4.0.0)
 Requires-Dist: google-cloud-bigquery-storage (>=2.14.1,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.4.0,<3.0.0)
-Requires-Dist: grpcio (==1.51.1)
+Requires-Dist: grpcio (>=1.56.0,<2.0.0)
 Requires-Dist: gspread (>=5.4.0,<6.0.0)
 Requires-Dist: gspread-dataframe (>=3.3.0,<4.0.0)
 Requires-Dist: imblearn (>=0.0,<0.1)
 Requires-Dist: importlib-metadata (>=5.2.0,<6.0.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pgzip (>=0.3.1,<0.4.0)
```

