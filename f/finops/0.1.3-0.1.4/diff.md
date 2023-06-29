# Comparing `tmp/finops-0.1.3.tar.gz` & `tmp/finops-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.1.3.tar", last modified: Fri Jun 23 13:56:50 2023, max compression
+gzip compressed data, was "finops-0.1.4.tar", last modified: Thu Jun 29 13:56:00 2023, max compression
```

## Comparing `finops-0.1.3.tar` & `finops-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-23 13:56:40.000000 finops-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-23 13:56:50.060248 finops-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 13:56:40.000000 finops-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 13:56:40.000000 finops-0.1.3/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-23 13:56:40.000000 finops-0.1.3/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 13:56:40.000000 finops-0.1.3/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-23 13:56:40.000000 finops-0.1.3/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-23 13:56:40.000000 finops-0.1.3/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:56:50.060248 finops-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 13:56:40.000000 finops-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:40.000000 finops-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_utils/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-29 13:55:48.000000 finops-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 13:56:00.862787 finops-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-29 13:55:48.000000 finops-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 13:55:48.000000 finops-0.1.4/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-29 13:55:48.000000 finops-0.1.4/finops/codal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-29 13:55:48.000000 finops-0.1.4/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 13:55:48.000000 finops-0.1.4/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-29 13:55:48.000000 finops-0.1.4/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-29 13:55:48.000000 finops-0.1.4/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 13:55:48.000000 finops-0.1.4/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:56:00.000000 finops-0.1.4/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:56:00.862787 finops-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 13:55:48.000000 finops-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:55:48.000000 finops-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:56:00.862787 finops-0.1.4/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-29 13:55:48.000000 finops-0.1.4/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.1.3/LICENSE` & `finops-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.1.3/PKG-INFO` & `finops-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.1.3/README.md` & `finops-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.1.3/finops/utils/downloader.py` & `finops-0.1.4/finops/utils/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import os
 import json
 import requests
 import pandas as pd
-from .wrappers import lock
 from bs4 import BeautifulSoup
+from finops.config import USER_AGENT
 
 
 class Downloader:
     @staticmethod
     def _create_csv_file(path, columns):
         if os.path.isfile(path):
             existing_columns = pd.read_csv(path, nrows=0).columns.tolist()
@@ -19,15 +19,15 @@
         else:
             directory = os.path.dirname(path)
             if directory:
                 os.makedirs(directory, exist_ok=True)
             pd.DataFrame(columns=columns).to_csv(path, index=False)
 
     @staticmethod
-    def _download(url, user_agent, timeout=None):
+    def _download(url, user_agent=USER_AGENT, timeout=None):
         response = requests.get(
             url,
             headers={"user-agent": user_agent},
             timeout=timeout,
         )
         response.raise_for_status()
         return response
```

### Comparing `finops-0.1.3/finops.egg-info/PKG-INFO` & `finops-0.1.4/finops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.1.3/setup.py` & `finops-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.1.3',
+    version='0.1.4',
     description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -23,9 +23,11 @@
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'pandas',
         'requests',
         'beautifulsoup4',
         'datetime',
+        'jdatetime',
+        'selenium',
     ],
 )
```

### Comparing `finops-0.1.3/tests/test_tehran_stock_exchange.py` & `finops-0.1.4/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.3/tests/test_ticker.py` & `finops-0.1.4/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.3/tests/test_utils/test_downloader.py` & `finops-0.1.4/tests/test_utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.3/tests/test_utils/test_scraper.py` & `finops-0.1.4/tests/test_utils/test_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
             self.traded_dates, self.start_date, self.end_date
         )
         expected_dates = [date(2022, 1, 3)]
         self.assertListEqual(filtered_dates, expected_dates)
 
     def test_get_ticker_scraped_dates(self):
         ticker_index = 0
-        scraped_dates = Scraper._get_ticker_scraped_dates(self.log, ticker_index)
+        scraped_dates = Scraper._get_scraped_dates(self.log, ticker_index)
         expected_dates = [date(2022, 1, 1), date(2022, 1, 2), date(2022, 1, 3)]
         self.assertListEqual(list(scraped_dates), expected_dates)
```

