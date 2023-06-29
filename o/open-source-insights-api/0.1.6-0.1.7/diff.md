# Comparing `tmp/open_source_insights_api-0.1.6.tar.gz` & `tmp/open_source_insights_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_insights_api-0.1.6.tar", max compression
+gzip compressed data, was "open_source_insights_api-0.1.7.tar", max compression
```

## Comparing `open_source_insights_api-0.1.6.tar` & `open_source_insights_api-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1477 2023-06-28 12:33:48.709797 open_source_insights_api-0.1.6/LICENSE
--rw-r--r--   0        0        0     1398 2023-06-28 12:33:48.709797 open_source_insights_api-0.1.6/README.md
--rw-r--r--   0        0        0       90 2023-06-28 12:56:28.669792 open_source_insights_api-0.1.6/open_source_insights_api/__init__.py
--rw-r--r--   0        0        0     7932 2023-06-28 12:33:48.709797 open_source_insights_api-0.1.6/open_source_insights_api/os_insights.py
--rw-r--r--   0        0        0      927 2023-06-28 13:06:09.219789 open_source_insights_api-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-29 12:25:06.013868 open_source_insights_api-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1398 2023-06-29 12:18:46.133876 open_source_insights_api-0.1.7/README.md
+-rw-r--r--   0        0        0       92 2023-06-29 12:19:48.163874 open_source_insights_api-0.1.7/open_source_insights_api/__init__.py
+-rw-r--r--   0        0        0    16592 2023-06-29 14:16:21.553731 open_source_insights_api-0.1.7/open_source_insights_api/os_insights.py
+-rw-r--r--   0        0        0      958 2023-06-29 12:42:04.523847 open_source_insights_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.7/PKG-INFO
```

### Comparing `open_source_insights_api-0.1.6/README.md` & `open_source_insights_api-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Open Source Insights Consume API
 
 This library will consume data from project Google Open Source Insights. 
 
 More information in [deps.dev](https://deps.dev "Website official Open Source Insights").
 
 ```shell
-pip install open_source_insights_api
+pip install open-source-insights-api
 ```
 
 Example use:
 
 ```python
 from open_source_insights_api import os_insights
```

### Comparing `open_source_insights_api-0.1.6/pyproject.toml` & `open_source_insights_api-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "open-source-insights-api"
-version = "0.1.6"
+version = "0.1.7"
+license = "MIT"
 description = "Library to consume project Open Source Insights Project from Google"
 authors = ["Cristiano Henrique <cristianovisk@gmail.com>"]
 readme = "README.md"
 packages = [{include = "open_source_insights_api"}]
 classifiers = [
-    "Topic :: Library",
+    "Topic :: Internet",
     "Environment :: Console",
     "Natural Language :: Portuguese (Brazilian)",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-requests = "^2.31.0"
+rich = "^13.4.2"
+httpx = "^0.24.1"
 
 [tool.poetry.urls]
 "Documentação" = "https://github.com/cristianovisk/open_source_insights_api/blob/main/README.md"
 "Código" = "https://github.com/cristianovisk/open_source_insights_api"
 "Bug Tracker" = "https://github.com/cristianovisk/open_source_insights_api/issues"
```

### Comparing `open_source_insights_api-0.1.6/PKG-INFO` & `open_source_insights_api-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: open-source-insights-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to consume project Open Source Insights Project from Google
+License: MIT
 Author: Cristiano Henrique
 Author-email: cristianovisk@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Library
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Classifier: Topic :: Internet
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Bug Tracker, https://github.com/cristianovisk/open_source_insights_api/issues
 Project-URL: Código, https://github.com/cristianovisk/open_source_insights_api
 Project-URL: Documentação, https://github.com/cristianovisk/open_source_insights_api/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # Open Source Insights Consume API
 
 This library will consume data from project Google Open Source Insights. 
 
 More information in [deps.dev](https://deps.dev "Website official Open Source Insights").
 
 ```shell
-pip install open_source_insights_api
+pip install open-source-insights-api
 ```
 
 Example use:
 
 ```python
 from open_source_insights_api import os_insights
```

