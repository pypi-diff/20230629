# Comparing `tmp/reliably_cli-0.8.0.tar.gz` & `tmp/reliably_cli-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliably_cli-0.8.0.tar", last modified: Tue Jun 20 12:27:10 2023, max compression
+gzip compressed data, was "reliably_cli-0.8.1.tar", last modified: Thu Jun 29 06:18:31 2023, max compression
```

## Comparing `reliably_cli-0.8.0.tar` & `reliably_cli-0.8.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/LICENSE
--rw-r--r--   0        0        0     1478 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/README.md
--rw-r--r--   0        0        0     3015 2023-06-20 12:27:10.061474 reliably_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      114 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/reliably_cli/__init__.py
--rw-r--r--   0        0        0      881 2023-06-20 12:26:50.065176 reliably_cli-0.8.0/reliably_cli/__main__.py
--rw-r--r--   0        0        0      166 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/__version__.py
--rw-r--r--   0        0        0     1221 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/__init__.py
--rw-r--r--   0        0        0     1545 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/cli.py
--rw-r--r--   0        0        0     2770 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/plan/__init__.py
--rw-r--r--   0        0        0     1352 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/plan/providers/__init__.py
--rw-r--r--   0        0        0     3493 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/agent/plan/providers/github.py
--rw-r--r--   0        0        0     1215 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/client.py
--rw-r--r--   0        0        0     1087 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/config/__init__.py
--rw-r--r--   0        0        0     3552 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/config/cli.py
--rw-r--r--   0        0        0     2403 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/config/types.py
--rw-r--r--   0        0        0      566 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/format.py
--rw-r--r--   0        0        0      126 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/log.py
--rw-r--r--   0        0        0        0 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/__init__.py
--rw-r--r--   0        0        0      211 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/cli.py
--rw-r--r--   0        0        0     2388 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/org.py
--rw-r--r--   0        0        0    12455 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/services/plan.py
--rw-r--r--   0        0        0     2690 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/reliably_cli/types.py
--rw-r--r--   0        0        0      662 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0      581 2023-06-20 12:26:50.069176 reliably_cli-0.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 06:18:06.339973 reliably_cli-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1478 2023-06-29 06:18:06.339973 reliably_cli-0.8.1/README.md
+-rw-r--r--   0        0        0     3015 2023-06-29 06:18:31.005332 reliably_cli-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/__main__.py
+-rw-r--r--   0        0        0      166 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/__version__.py
+-rw-r--r--   0        0        0     1221 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/agent/__init__.py
+-rw-r--r--   0        0        0     1545 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/agent/cli.py
+-rw-r--r--   0        0        0     2770 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/agent/plan/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/agent/plan/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/agent/plan/providers/github.py
+-rw-r--r--   0        0        0     1215 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/client.py
+-rw-r--r--   0        0        0     1087 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/config/__init__.py
+-rw-r--r--   0        0        0     3552 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/config/cli.py
+-rw-r--r--   0        0        0     2403 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/config/types.py
+-rw-r--r--   0        0        0      566 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/format.py
+-rw-r--r--   0        0        0      126 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/log.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/services/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/services/cli.py
+-rw-r--r--   0        0        0     2388 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/services/org.py
+-rw-r--r--   0        0        0    12455 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/services/plan.py
+-rw-r--r--   0        0        0     2690 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/reliably_cli/types.py
+-rw-r--r--   0        0        0      662 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0      581 2023-06-29 06:18:06.343973 reliably_cli-0.8.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.8.1/PKG-INFO
```

### Comparing `reliably_cli-0.8.0/LICENSE` & `reliably_cli-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/README.md` & `reliably_cli-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/pyproject.toml` & `reliably_cli-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "rich>=13.3.1",
     "chaostoolkit-addons>=0.4.0",
     "chaostoolkit>=1.15.0",
     "chaostoolkit-lib>=1.33.1",
     "chaostoolkit-reliably>=0.22.0",
     "orjson>=3.8.10",
 ]
-version = "0.8.0"
+version = "0.8.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://reliably.com/"
 Repository = "https://github.com/reliablyhq/cli"
```

### Comparing `reliably_cli-0.8.0/reliably_cli/__main__.py` & `reliably_cli-0.8.1/reliably_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/agent/__init__.py` & `reliably_cli-0.8.1/reliably_cli/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/agent/cli.py` & `reliably_cli-0.8.1/reliably_cli/agent/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/agent/plan/__init__.py` & `reliably_cli-0.8.1/reliably_cli/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/agent/plan/providers/__init__.py` & `reliably_cli-0.8.1/reliably_cli/agent/plan/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/agent/plan/providers/github.py` & `reliably_cli-0.8.1/reliably_cli/agent/plan/providers/github.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/client.py` & `reliably_cli-0.8.1/reliably_cli/client.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/config/__init__.py` & `reliably_cli-0.8.1/reliably_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/config/cli.py` & `reliably_cli-0.8.1/reliably_cli/config/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/config/types.py` & `reliably_cli-0.8.1/reliably_cli/config/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/format.py` & `reliably_cli-0.8.1/reliably_cli/format.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/services/org.py` & `reliably_cli-0.8.1/reliably_cli/services/org.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/services/plan.py` & `reliably_cli-0.8.1/reliably_cli/services/plan.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/reliably_cli/types.py` & `reliably_cli-0.8.1/reliably_cli/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/tests/conftest.py` & `reliably_cli-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/tests/test_cli.py` & `reliably_cli-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.8.0/PKG-INFO` & `reliably_cli-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliably-cli
-Version: 0.8.0
+Version: 0.8.1
 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch <sylvain@reliably.com>
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reliably-cli Version: 0.8.0 Summary: Reliably CLI
+Metadata-Version: 2.1 Name: reliably-cli Version: 0.8.1 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch
 reliably.com> License: Apache-2.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Development Status :: 4 - Beta Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities Project-URL: Homepage, https://reliably.com/
```

