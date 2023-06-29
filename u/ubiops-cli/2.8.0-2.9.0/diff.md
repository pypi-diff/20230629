# Comparing `tmp/ubiops-cli-2.8.0.tar.gz` & `tmp/ubiops-cli-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubiops-cli-2.8.0.tar", last modified: Thu Mar 17 09:11:17 2022, max compression
+gzip compressed data, was "dist/ubiops-cli-2.9.0.tar", last modified: Thu May 12 10:50:43 2022, max compression
```

## Comparing `ubiops-cli-2.8.0.tar` & `ubiops-cli-2.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/
--rw-r--r--   0 sascha    (1000) sascha    (1000)       17 2020-11-19 07:42:58.000000 ubiops-cli-2.8.0/MANIFEST.in
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1043 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/PKG-INFO
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     3128 2022-03-17 09:04:05.000000 ubiops-cli-2.8.0/README.md
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       38 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/setup.cfg
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1891 2022-03-17 09:04:53.000000 ubiops-cli-2.8.0/setup.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/__init__.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      667 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/constants.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      108 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/exceptions.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli/ignore/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/ignore/__init__.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     6714 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/ignore/ignore.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     3519 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/ignore/utils.py
--rwxrwxr-x   0 sascha    (1000) sascha    (1000)     2860 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/main.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli/src/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/__init__.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     3961 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/auth.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     2961 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/blobs.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1073 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/config.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1535 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/deployment_builds.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     3482 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/deployment_revisions.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    10414 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/deployment_versions.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    35757 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/deployments.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    14666 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/environment_variables.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     6166 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/exports.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/__init__.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     2021 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/click_helpers.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     8473 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/deployment_helpers.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    20644 2022-03-17 08:56:43.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/formatting.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1574 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/helpers.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    25059 2022-03-17 08:56:29.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/options.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     8314 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/pipeline_helpers.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     4423 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/helpers/requests.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     8683 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/imports.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     6109 2022-03-17 08:56:43.000000 ubiops-cli-2.8.0/ubiops_cli/src/logs.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    12108 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/pipeline_versions.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    25743 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/pipelines.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     4630 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/projects.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     4732 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/src/request_schedules.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     9970 2022-03-02 07:57:22.000000 ubiops-cli-2.8.0/ubiops_cli/utils.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       18 2022-03-17 08:56:29.000000 ubiops-cli-2.8.0/ubiops_cli/version.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1043 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/PKG-INFO
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1241 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        1 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       67 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/entry_points.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      149 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/requires.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       11 2022-03-17 09:11:17.000000 ubiops-cli-2.8.0/ubiops_cli.egg-info/top_level.txt
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/
+-rw-r--r--   0 sascha    (1000) sascha    (1000)       17 2020-11-19 07:42:58.000000 ubiops-cli-2.9.0/MANIFEST.in
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1043 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/PKG-INFO
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     3128 2022-05-12 10:41:08.000000 ubiops-cli-2.9.0/README.md
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)       38 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/setup.cfg
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1891 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/setup.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/__init__.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)      667 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/constants.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)      108 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/exceptions.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli/ignore/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/ignore/__init__.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     6714 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/ignore/ignore.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     3519 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/ignore/utils.py
+-rwxrwxr-x   0 sascha    (1000) sascha    (1000)     2860 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/main.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli/src/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/__init__.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     3961 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/auth.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     2961 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/blobs.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1073 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/config.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1535 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/deployment_builds.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     3482 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/deployment_revisions.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    10576 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/deployment_versions.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    35960 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/deployments.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    14666 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/environment_variables.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     6166 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/exports.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        0 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/__init__.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     2021 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/click_helpers.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     8158 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/deployment_helpers.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    20653 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/formatting.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1574 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/helpers.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    25081 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/options.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     8314 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/pipeline_helpers.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     4423 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/helpers/requests.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     8646 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/imports.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     6345 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/logs.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    12108 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/pipeline_versions.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)    25743 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/pipelines.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     4630 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/projects.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     4654 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/src/request_schedules.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     9970 2022-03-02 07:57:22.000000 ubiops-cli-2.9.0/ubiops_cli/utils.py
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)       18 2022-05-12 10:27:22.000000 ubiops-cli-2.9.0/ubiops_cli/version.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1043 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1241 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        1 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)       67 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)      149 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/requires.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)       11 2022-05-12 10:50:43.000000 ubiops-cli-2.9.0/ubiops_cli.egg-info/top_level.txt
```

### Comparing `ubiops-cli-2.8.0/PKG-INFO` & `ubiops-cli-2.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ubiops-cli
-Version: 2.8.0
+Version: 2.9.0
 Summary: UbiOps Command Line Interface to interact with the UbiOps API. 
 Home-page: https://github.com/UbiOps/command-line-interface.git
 Author: UbiOps
 License: Apache 2.0
 Project-URL: Documentation, https://ubiops.com/docs
 Project-URL: Source, https://github.com/UbiOps/command-line-interface.git
 Description: 
         Command Line Interface to interact with the UbiOps API (v2.1).
         
         Read the documentation at: https://github.com/UbiOps/command-line-interface
         
         More information about UbiOps: https://ubiops.com/
         
-        UbiOps-cli is compatible with Python 3.5+ and is distributed under the Apache 2.0 License.
+        UbiOps-cli is compatible with Python 3.6+ and is distributed under the Apache 2.0 License.
         
 Keywords: UbiOps Command Line Interface
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
```

### Comparing `ubiops-cli-2.8.0/README.md` & `ubiops-cli-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/setup.py` & `ubiops-cli-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     return """
 Command Line Interface to interact with the UbiOps API (v2.1).
 
 Read the documentation at: https://github.com/UbiOps/command-line-interface
 
 More information about UbiOps: https://ubiops.com/
 
-UbiOps-cli is compatible with Python 3.5+ and is distributed under the Apache 2.0 License.
+UbiOps-cli is compatible with Python 3.6+ and is distributed under the Apache 2.0 License.
 """
 
 
-ubiops_version = "3.8.0"
+ubiops_version = "3.9.0"
 REQUIRES = ["urllib3>=1.15", "six>=1.10", "certifi", "requests>=2.17.3", "tabulate==0.8.7",
             "python-dateutil", "click>=7.0", "ConfigParser==4.0.2", "colorama==0.4.3", "pyyaml",
             "ubiops==%s" % ubiops_version]
 
 setup(
     name=NAME,
     version=VERSION,
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/constants.py` & `ubiops-cli-2.9.0/ubiops_cli/constants.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/ignore/ignore.py` & `ubiops-cli-2.9.0/ubiops_cli/ignore/ignore.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/ignore/utils.py` & `ubiops-cli-2.9.0/ubiops_cli/ignore/utils.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/main.py` & `ubiops-cli-2.9.0/ubiops_cli/main.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/auth.py` & `ubiops-cli-2.9.0/ubiops_cli/src/auth.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/blobs.py` & `ubiops-cli-2.9.0/ubiops_cli/src/blobs.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/config.py` & `ubiops-cli-2.9.0/ubiops_cli/src/config.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/deployment_builds.py` & `ubiops-cli-2.9.0/ubiops_cli/src/deployment_builds.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/deployment_revisions.py` & `ubiops-cli-2.9.0/ubiops_cli/src/deployment_revisions.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/deployment_versions.py` & `ubiops-cli-2.9.0/ubiops_cli/src/deployment_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ubiops_cli.src.helpers.deployment_helpers import define_deployment_version, update_deployment_file, \
     DEPLOYMENT_VERSION_FIELDS, DEPLOYMENT_VERSION_FIELDS_UPDATE, DEPLOYMENT_VERSION_FIELDS_RENAMED
 from ubiops_cli.src.helpers.helpers import get_label_filter
 from ubiops_cli.src.helpers.formatting import print_list, print_item, format_yaml
 from ubiops_cli.src.helpers.options import *
 
 
-LIST_ITEMS = ['last_updated', 'version', 'deployment_mode', 'status', 'labels']
+LIST_ITEMS = ['last_updated', 'version', 'status', 'labels']
 
 
 @click.group(["deployment_versions", "versions"], short_help="Manage your deployment versions")
 def commands():
     """Manage your deployment versions."""
     pass
 
@@ -81,15 +81,14 @@
     language: python3.7
     instance_type: 2048mb
     minimum_instances: 0
     maximum_instances: 5
     maximum_idle_time: 300
     request_retention_mode: none
     request_retention_time: 604800
-    deployment_mode: express
     ```
     """
 
     project_name = get_current_project(error=True)
 
     # Show version details
     client = init_client()
@@ -123,15 +122,15 @@
 @VERSION_NAME_OVERRULE
 @LANGUAGE
 @INSTANCE_TYPE
 @MEMORY_ALLOCATION
 @MIN_INSTANCES
 @MAX_INSTANCES
 @MAX_IDLE_TIME
-@DEPLOYMENT_MODE
+@DEPLOYMENT_MODE_DEPRECATED
 @RETENTION_MODE
 @RETENTION_TIME
 @VERSION_LABELS
 @VERSION_DESCRIPTION
 @VERSION_YAML_FILE
 @DEPLOYMENT_FILE
 @CREATE_FORMATS
@@ -151,19 +150,16 @@
     language: python3.7
     instance_type: 2048mb
     minimum_instances: 0
     maximum_instances: 1
     maximum_idle_time: 300
     request_retention_mode: none
     request_retention_time: 604800
-    deployment_mode: express
     ```
 
-    Provide either deployment mode 'express' or 'batch', default is 'express'.
-
     Those parameters can also be provided as command options. If both a `<yaml_file>` is set and
     options are given, the options defined by `<yaml_file>` will be overwritten by the specified command options.
     The version name can either be passed as command argument or specified inside the yaml file using `<version_name>`.
     """
 
     project_name = get_current_project(error=True)
 
@@ -171,14 +167,20 @@
     client = init_client()
 
     assert 'deployment_name' in yaml_content or deployment_name, 'Please, specify the deployment name in either ' \
                                                                  'the yaml file or as a command argument'
     assert 'version_name' in yaml_content or version_name, 'Please, specify the version name in either ' \
                                                            'the yaml file or as a command argument'
 
+    if format_ != 'json' and ('deployment_mode' in yaml_content or kwargs['deployment_mode']):
+        click.secho(
+            "Deprecation warning: 'deployment_mode' is deprecated. From now on, both direct and batch requests can be "
+            "made to the same deployment version.", fg='red'
+        )
+
     kwargs = define_deployment_version(kwargs, yaml_content, extra_yaml_fields=['deployment_file'])
 
     if format_ != 'json' and kwargs['memory_allocation'] and not kwargs['instance_type']:
         click.secho(
             "Deprecation warning: parameter 'memory_allocation' is deprecated, use 'instance_type' instead",
             fg='red'
         )
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/deployments.py` & `ubiops-cli-2.9.0/ubiops_cli/src/deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 @VERSION_YAML_FILE
 @LANGUAGE
 @INSTANCE_TYPE
 @MEMORY_ALLOCATION
 @MIN_INSTANCES
 @MAX_INSTANCES
 @MAX_IDLE_TIME
-@DEPLOYMENT_MODE
+@DEPLOYMENT_MODE_DEPRECATED
 @RETENTION_MODE
 @RETENTION_TIME
 @VERSION_LABELS
 @VERSION_DESCRIPTION
 @OVERWRITE
 @ASSUME_YES
 @QUIET
@@ -394,16 +394,14 @@
     file is assumed to be equal to the wellknown '.gitignore' file.
 
     If you want to store a local copy of the uploaded zip file, please use the `<output_path>` option.
     The `<output_path>` option will be used as output location of the zip file. If the `<output_path>` is a
     directory, the zip will be saved in `[deployment_name]_[deployment_version]_[datetime.now()].zip`. Use
     the `<assume_yes>` option to overwrite without confirmation if file specified in `<output_path>` already exists.
 
-    Provide either deployment mode 'express' or 'batch', default is 'express'.
-
     \b
     It is possible to define the parameters using a yaml file.
     For example:
     ```
     deployment_name: my-deployment-name
     version_name: my-deployment-version
     version_description: Version created via command line.
@@ -413,15 +411,14 @@
     language: python3.7
     instance_type: 2048mb
     minimum_instances: 0
     maximum_instances: 1
     maximum_idle_time: 300
     request_retention_mode: none
     request_retention_time: 604800
-    deployment_mode: express
     ```
 
     Those parameters can also be provided as command options. If both a `<yaml_file>` is set and options are given,
     the options defined by `<yaml_file>` will be overwritten by the specified command options. The deployment name can
     either be passed as command argument or specified inside the yaml file using `<deployment_name>`.
 
     It's not possible to update the programming language and deployment mode of an existing deployment version.
@@ -438,30 +435,34 @@
     yaml_content = read_yaml(yaml_file, required_fields=[])
 
     assert 'deployment_name' in yaml_content or deployment_name, 'Please, specify the deployment name in either the ' \
                                                                  'yaml file or as a command argument'
     assert 'version_name' in yaml_content or version_name, 'Please, specify the version name in either the yaml ' \
                                                            'file or as a command option'
 
+    if not quiet and ('deployment_mode' in yaml_content or kwargs['deployment_mode']):
+        click.secho(
+            "Deprecation warning: 'deployment_mode' is deprecated. From now on, both direct and batch requests can be "
+            "made to the same deployment version.", fg='red'
+        )
+
     deployment_name = set_dict_default(deployment_name, yaml_content, 'deployment_name')
     version_name = set_dict_default(version_name, yaml_content, 'version_name')
 
     existing_version = None
     if overwrite:
         try:
             existing_version = client.deployment_versions_get(
                 project_name=project_name, deployment_name=deployment_name, version=version_name
             )
         except api.exceptions.ApiException:
             # Do nothing if version doesn't exist
             pass
 
-    kwargs = define_deployment_version(
-        kwargs, yaml_content, extra_yaml_fields=['deployment_file', 'ignore_file']
-    )
+    kwargs = define_deployment_version(kwargs, yaml_content, extra_yaml_fields=['deployment_file', 'ignore_file'])
     kwargs['ignore_file'] = DEFAULT_IGNORE_FILE if kwargs['ignore_file'] is None else kwargs['ignore_file']
 
     if not quiet and kwargs['memory_allocation'] and not kwargs['instance_type']:
         click.secho(
             "Deprecation warning: parameter 'memory_allocation' is deprecated, use 'instance_type' instead",
             fg='red'
         )
@@ -541,16 +542,16 @@
 @REQUEST_DATA_FILE
 @REQUEST_TIMEOUT
 @REQUESTS_FORMATS
 def requests_create(deployment_name, version_name, batch, data, json_file, timeout, format_):
     """
     Create a deployment request and retrieve request IDs to collect the results later.
     Use the option `timeout` to specify the timeout of the request. The minimum value is 10 seconds. The maximum value
-    is 3600 (1 hour) for express deployments and 345600 (96 hours) for batch deployments. The default value is 300
-    (5 minutes) for express deployments and 14400 (4 hours) for batch deployments.
+    is 3600 (1 hour) for direct (synchronous) requests and 345600 (96 hours) for batch (asynchronous) requests.
+    The default value is 300 (5 minutes) for direct requests and 14400 (4 hours) for batch requests.
 
     Use the version option to make a request to a specific deployment version:
     `ubiops deployments requests create <my-deployment> -v <my-version> --data <input>`
 
     If not specified, a request is made to the default version:
     `ubiops deployments requests create <my-deployment> --data <input>`
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/environment_variables.py` & `ubiops-cli-2.9.0/ubiops_cli/src/environment_variables.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/exports.py` & `ubiops-cli-2.9.0/ubiops_cli/src/exports.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/click_helpers.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/click_helpers.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/deployment_helpers.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/deployment_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     SYS_DEPLOYMENT_FILE_NAME_VALUE
 from ubiops_cli.src.helpers.helpers import strings_to_dict
 
 
 DEPLOYMENT_REQUIRED_FIELDS = ['input_type', 'output_type']
 DEPLOYMENT_VERSION_FIELDS = [
     'description', 'labels', 'language', 'instance_type', 'memory_allocation', 'minimum_instances', 'maximum_instances',
-    'maximum_idle_time', 'deployment_mode', 'request_retention_mode', 'request_retention_time'
+    'maximum_idle_time', 'request_retention_mode', 'request_retention_time'
 ]
 DEPLOYMENT_VERSION_FIELDS_UPDATE = [
     'version', 'description', 'labels', 'instance_type', 'memory_allocation', 'minimum_instances', 'maximum_instances',
     'maximum_idle_time', 'request_retention_mode', 'request_retention_time'
 ]
 DEPLOYMENT_VERSION_FIELDS_WAIT = [
     'instance_type', 'memory_allocation', 'minimum_instances', 'maximum_instances', 'maximum_idle_time'
@@ -22,15 +22,14 @@
     'instance_type': str,
     'memory_allocation': int,
     'minimum_instances': int,
     'maximum_instances': int,
     'maximum_idle_time': int,
     'description': str,
     'labels': dict,
-    'deployment_mode': str,
     'request_retention_mode': str,
     'request_retention_time': int,
 }
 DEPLOYMENT_VERSION_FIELDS_RENAMED = {
     'version': 'version_name', 'description': 'version_description', 'labels': 'version_labels'
 }
 
@@ -157,18 +156,14 @@
         **{k: update_fields[k] for k in DEPLOYMENT_VERSION_FIELDS_UPDATE if k in update_fields}
     )
 
     if (hasattr(existing_version, 'language') and 'language' in update_fields
             and existing_version.language != update_fields['language']):
         raise Exception("The programming language of an existing version cannot be changed")
 
-    if (hasattr(existing_version, 'deployment_mode') and 'deployment_mode' in update_fields
-            and existing_version.deployment_mode != update_fields['deployment_mode']):
-        raise Exception("The deployment mode of an existing version cannot be changed")
-
     has_changed_fields = False
     for field in DEPLOYMENT_VERSION_FIELDS_WAIT:
         has_field = hasattr(existing_version, field) and field in update_fields
         if has_field and getattr(existing_version, field) != update_fields[field]:
             has_changed_fields = True
 
     client.deployment_versions_update(
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/formatting.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
 
 def format_logs_oneline(logs):
     overview = ''
     total = len(logs)
     for i, log in enumerate(logs):
         overview += click.style(str(log.id), fg='yellow')
         overview += ' '
-        overview += click.style(format_datetime(parse_datetime(log.date), '%H:%M:%S %Z'), fg='green')
+        overview += click.style(format_datetime(parse_datetime(log.date), '%Y-%m-%d %H:%M:%S %Z'), fg='green')
         overview += ' '
 
         # Change the color of the log depending on the log level
         if log.level == 'error':
             # Change the color of all lines if the log contains multiple lines
             log_lines = log.log.split('\n')
             log_line = '\n'.join([click.style(item, fg='red') for item in log_lines])
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/helpers.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/options.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 OFFSET = click.option(
     '--offset', required=False, default=None, type=int, metavar='<int>',
     help="The starting point: if offset equals 2, then the first 2 records will be omitted"
 )
 
 # Formatting output
 LOGS_FORMATS = click.option(
-    '-fmt', '--format', 'format_',  default='reference', help="The output format",
+    '-fmt', '--format', 'format_',  default='oneline', help="The output format",
     type=click.Choice(['oneline', 'reference', 'extended', 'json'], case_sensitive=False), show_default=True
 )
 REQUESTS_FORMATS = click.option(
     '-fmt', '--format', 'format_',  default='reference', help="The output format",
     type=click.Choice(['oneline', 'reference', 'json'], case_sensitive=False), show_default=True
 )
 PROJECTS_FORMATS = click.option(
@@ -174,18 +174,18 @@
     '-max', '--maximum_instances', required=False, default=None, type=int, metavar='<int>',
     help="Maximum number of instances"
 )
 MAX_IDLE_TIME = click.option(
     '-t', '--maximum_idle_time', required=False, default=None, type=int, metavar='<int>',
     help="Maximum idle time before shutting down instance (seconds)"
 )
-DEPLOYMENT_MODE = click.option(
+DEPLOYMENT_MODE_DEPRECATED = click.option(
     '-dm', '--deployment_mode', required=False, default=None,
     type=click.Choice(['express', 'batch'], case_sensitive=False),
-    help="The type of the deployment version"
+    help="[DEPRECATED] The type of the deployment version"
 )
 RETENTION_MODE = click.option(
     '-rtm', '--request_retention_mode', required=False, default=None,
     type=click.Choice(['none', 'metadata', 'full'], case_sensitive=False),
     help="Mode of request retention for requests to the version"
 )
 RETENTION_TIME = click.option(
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/pipeline_helpers.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/pipeline_helpers.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/helpers/requests.py` & `ubiops-cli-2.9.0/ubiops_cli/src/helpers/requests.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/imports.py` & `ubiops-cli-2.9.0/ubiops_cli/src/imports.py`

 * *Files identical despite different names*

```diff
@@ -118,15 +118,14 @@
             data_type: int
         default_version: v1
         versions:
           v1:
             zip: "deployments/deployment_deployment-1/versions/deployment_deployment-1_version_v1.zip"
             description:
             language: python3.8
-            deployment_mode: express
             maximum_idle_time: 300
             minimum_instances: 0
             maximum_instances: 5
             memory_allocation: 512
             request_retention_mode: full
             request_retention_time: 604800
             environment_variables:
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/logs.py` & `ubiops-cli-2.9.0/ubiops_cli/src/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,45 +57,53 @@
         filters['deployment_request_id'] = request_id
     if pipeline_request_id:
         filters['pipeline_request_id'] = pipeline_request_id
     if system is not None:
         filters['system'] = system
     if level:
         filters['level'] = level
+
     if start_date is not None:
         try:
             start_date = format_datetime(parse_datetime(start_date), fmt='%Y-%m-%dT%H:%M:%SZ')
         except ValueError:
             raise Exception(
                 "Failed to parse start_date. Please use iso-format, for example, '2020-01-01T00:00:00.000000Z'"
             )
     elif start_date is None and start_log is None:
         start_date = str(datetime.now())
+
     log_filters = api.LogsCreate(filters=filters, date=start_date, id=start_log, date_range=date_range, limit=limit)
     logs = client.projects_log_list(project_name=project_name, data=log_filters)
     client.api_client.close()
 
     if format_ == 'json':
         click.echo(format_json(logs))
         return
 
     if len(logs) > 0:
         if format_ == 'oneline':
+            # Make sure logs are sorted old to new
+            logs = list(reversed(logs)) if date_range < 0 else logs
             lines = format_logs_oneline(logs)
+            click.echo(lines)
         elif format_ == 'reference':
             lines = format_logs_reference(logs)
+            click.echo_via_pager(lines)
         elif format_ == 'extended':
             lines = format_logs_reference(
                 logs,
                 extended=['deployment_request_id', 'pipeline_request_id', 'deployment_name', 'deployment_version',
                           'pipeline_name', 'pipeline_version', 'pipeline_object_name', 'build_id', 'level']
             )
+            click.echo_via_pager(lines)
         else:
             lines = format_logs_reference(logs)
-        click.echo_via_pager(lines)
+            click.echo_via_pager(lines)
+
     elif start_date:
         starting_point = parse_datetime(start_date).isoformat()
         if date_range > 0:
             end_point = (parse_datetime(start_date) + timedelta(seconds=date_range)).isoformat()
         else:
             end_point = (parse_datetime(start_date) - timedelta(seconds=abs(date_range))).isoformat()
         click.echo("No logs found between <%s> and <%s>" % (starting_point, end_point))
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/pipeline_versions.py` & `ubiops-cli-2.9.0/ubiops_cli/src/pipeline_versions.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/pipelines.py` & `ubiops-cli-2.9.0/ubiops_cli/src/pipelines.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/projects.py` & `ubiops-cli-2.9.0/ubiops_cli/src/projects.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli/src/request_schedules.py` & `ubiops-cli-2.9.0/ubiops_cli/src/request_schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,15 @@
 @SCHEDULE
 @REQUEST_TIMEOUT
 @IS_ENABLED
 @CREATE_FORMATS
 def schedules_create(schedule_name, object_type, object_name, object_version, data, format_, **kwargs):
     """
     Create a new request schedule.
-
-    - For express mode deployments, direct requests will be made
-    - For batch mode deployments, batch requests will be made
-    - For pipelines, batch requests will be made
+    A batch request will be created to your deployment/pipeline according to the defined schedule.
     """
 
     project_name = get_current_project(error=True)
 
     client = init_client()
     obj = get_schedule_object(client, project_name, object_type, object_name)
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli/utils.py` & `ubiops-cli-2.9.0/ubiops_cli/utils.py`

 * *Files identical despite different names*

### Comparing `ubiops-cli-2.8.0/ubiops_cli.egg-info/PKG-INFO` & `ubiops-cli-2.9.0/ubiops_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ubiops-cli
-Version: 2.8.0
+Version: 2.9.0
 Summary: UbiOps Command Line Interface to interact with the UbiOps API. 
 Home-page: https://github.com/UbiOps/command-line-interface.git
 Author: UbiOps
 License: Apache 2.0
 Project-URL: Documentation, https://ubiops.com/docs
 Project-URL: Source, https://github.com/UbiOps/command-line-interface.git
 Description: 
         Command Line Interface to interact with the UbiOps API (v2.1).
         
         Read the documentation at: https://github.com/UbiOps/command-line-interface
         
         More information about UbiOps: https://ubiops.com/
         
-        UbiOps-cli is compatible with Python 3.5+ and is distributed under the Apache 2.0 License.
+        UbiOps-cli is compatible with Python 3.6+ and is distributed under the Apache 2.0 License.
         
 Keywords: UbiOps Command Line Interface
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
```

### Comparing `ubiops-cli-2.8.0/ubiops_cli.egg-info/SOURCES.txt` & `ubiops-cli-2.9.0/ubiops_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

