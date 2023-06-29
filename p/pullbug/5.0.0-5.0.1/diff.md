# Comparing `tmp/pullbug-5.0.0.tar.gz` & `tmp/pullbug-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pullbug-5.0.0.tar", last modified: Mon Jun 26 17:46:02 2023, max compression
+gzip compressed data, was "pullbug-5.0.1.tar", last modified: Thu Jun 29 21:35:43 2023, max compression
```

## Comparing `pullbug-5.0.0.tar` & `pullbug-5.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 17:45:34.000000 pullbug-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 17:46:02.432378 pullbug-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 17:45:34.000000 pullbug-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/pullbug/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/bug.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/pullbug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-26 17:45:34.000000 pullbug-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:46:02.432378 pullbug-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 17:45:34.000000 pullbug-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:45:34.000000 pullbug-5.0.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-26 17:45:34.000000 pullbug-5.0.0/test/unit/test_bug.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-26 17:45:34.000000 pullbug-5.0.0/test/unit/test_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:43.447889 pullbug-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 21:35:12.000000 pullbug-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-29 21:35:43.447889 pullbug-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-29 21:35:12.000000 pullbug-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:43.447889 pullbug-5.0.1/pullbug/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-29 21:35:12.000000 pullbug-5.0.1/pullbug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-06-29 21:35:12.000000 pullbug-5.0.1/pullbug/bug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-29 21:35:12.000000 pullbug-5.0.1/pullbug/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-29 21:35:12.000000 pullbug-5.0.1/pullbug/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:12.000000 pullbug-5.0.1/pullbug/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:43.447889 pullbug-5.0.1/pullbug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-29 21:35:43.000000 pullbug-5.0.1/pullbug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 21:35:43.000000 pullbug-5.0.1/pullbug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:35:43.000000 pullbug-5.0.1/pullbug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 21:35:43.000000 pullbug-5.0.1/pullbug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 21:35:43.000000 pullbug-5.0.1/pullbug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 21:35:43.000000 pullbug-5.0.1/pullbug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-29 21:35:12.000000 pullbug-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 21:35:43.447889 pullbug-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-29 21:35:12.000000 pullbug-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:43.443889 pullbug-5.0.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:43.447889 pullbug-5.0.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:35:12.000000 pullbug-5.0.1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-29 21:35:12.000000 pullbug-5.0.1/test/unit/test_bug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-29 21:35:12.000000 pullbug-5.0.1/test/unit/test_messages.py
```

### Comparing `pullbug-5.0.0/LICENSE` & `pullbug-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pullbug-5.0.0/PKG-INFO` & `pullbug-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pullbug
-Version: 5.0.0
+Version: 5.0.1
 Summary: Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
 Home-page: http://github.com/justintime50/pullbug
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install pullbug
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 Pullbug works best when run on a schedule. Run one-off reports or setup Pullbug to notify you at whatever interval you'd like to be bugged via Discord or Slack about pull requests.
 
 Pullbug is highly customizable allowing you to choose which messaging service and what kinds of pull requests or issues you'd like.
@@ -85,15 +85,15 @@
   --quiet               Does not output when there is nothing to bug about.
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python pullbug/cli.py --help
 ```
 
 ## Trusted By
```

### Comparing `pullbug-5.0.0/README.md` & `pullbug-5.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install pullbug
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 Pullbug works best when run on a schedule. Run one-off reports or setup Pullbug to notify you at whatever interval you'd like to be bugged via Discord or Slack about pull requests.
 
 Pullbug is highly customizable allowing you to choose which messaging service and what kinds of pull requests or issues you'd like.
@@ -70,15 +70,15 @@
   --quiet               Does not output when there is nothing to bug about.
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python pullbug/cli.py --help
 ```
 
 ## Trusted By
```

### Comparing `pullbug-5.0.0/pullbug/bug.py` & `pullbug-5.0.1/pullbug/bug.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 DEFAULT_BASE_URL = 'https://api.github.com'
 
 LOGGER_NAME = 'pullbug'
 
 
 class Pullbug:
-    def __init__(  # nosec - no hardcoded token here, ignore
+    def __init__(  # nosec hardcoded_password_default
         self,
         github_owner: str,
         github_token: Optional[str] = None,
         github_state: GITHUB_STATE_CHOICES = 'open',
         github_context: GITHUB_CONTEXT_CHOICES = 'users',
         pulls: bool = False,
         issues: bool = False,
```

### Comparing `pullbug-5.0.0/pullbug/cli.py` & `pullbug-5.0.1/pullbug/cli.py`

 * *Files identical despite different names*

### Comparing `pullbug-5.0.0/pullbug/messages.py` & `pullbug-5.0.1/pullbug/messages.py`

 * *Files identical despite different names*

### Comparing `pullbug-5.0.0/pullbug.egg-info/PKG-INFO` & `pullbug-5.0.1/pullbug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pullbug
-Version: 5.0.0
+Version: 5.0.1
 Summary: Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
 Home-page: http://github.com/justintime50/pullbug
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install pullbug
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 Pullbug works best when run on a schedule. Run one-off reports or setup Pullbug to notify you at whatever interval you'd like to be bugged via Discord or Slack about pull requests.
 
 Pullbug is highly customizable allowing you to choose which messaging service and what kinds of pull requests or issues you'd like.
@@ -85,15 +85,15 @@
   --quiet               Does not output when there is nothing to bug about.
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python pullbug/cli.py --help
 ```
 
 ## Trusted By
```

### Comparing `pullbug-5.0.0/setup.py` & `pullbug-5.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 REQUIREMENTS = [
-    'PyGithub == 1.*',
+    'PyGithub >= 1.59.0',
     'requests == 2.*',
     'slackclient == 2.*',
     'woodchips == 0.2.*',
 ]
 
 DEV_REQUIREMENTS = [
     'bandit == 1.7.*',
@@ -22,15 +22,15 @@
     'pytest-cov == 4.*',
     'twine == 4.*',
     'types-requests',
 ]
 
 setuptools.setup(
     name='pullbug',
-    version='5.0.0',
+    version='5.0.1',
     description='Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/pullbug',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
```

### Comparing `pullbug-5.0.0/test/unit/test_bug.py` & `pullbug-5.0.1/test/unit/test_bug.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 )
 
 import pytest
 
 from pullbug.bug import Pullbug
 
 
+@patch('pullbug.bug.Pullbug.send_messages')
 @patch('pullbug.bug.Pullbug.get_pull_requests')
 @patch('pullbug.bug.Pullbug.get_repos')
 @patch('logging.Logger.info')
-def test_run_pull_requests(mock_logger, mock_get_repos, mock_pull_request):
+def test_run_pull_requests(mock_logger, mock_get_repos, mock_pull_request, mock_send_messages):
     Pullbug(
         github_owner='justintime50',
         github_token='123',
         github_context='users',
         pulls=True,
     ).run()
 
     mock_get_repos.assert_called_once()
     mock_pull_request.assert_called_once()
     mock_logger.assert_called()
+    mock_send_messages.assert_called_once()
 
 
 @patch('pullbug.bug.Pullbug.get_pull_requests', return_value=[])
 @patch('pullbug.bug.Pullbug.get_repos')
 @patch('logging.Logger.info')
 def test_run_no_pull_requests(mock_logger, mock_get_repos, mock_pull_request):
     Pullbug(
@@ -36,28 +38,30 @@
     ).run()
 
     mock_get_repos.assert_called_once()
     mock_pull_request.assert_called_once()
     assert mock_logger.call_count == 4
 
 
+@patch('pullbug.bug.Pullbug.send_messages')
 @patch('pullbug.bug.Pullbug.get_issues')
 @patch('pullbug.bug.Pullbug.get_repos')
 @patch('logging.Logger.info')
-def test_run_issues(mock_logger, mock_get_repos, mock_issues):
+def test_run_issues(mock_logger, mock_get_repos, mock_issues, mock_send_messages):
     Pullbug(
         github_owner='justintime50',
         github_token='123',
         github_context='users',
         issues=True,
     ).run()
 
     mock_get_repos.assert_called_once()
     mock_issues.assert_called_once()
     mock_logger.assert_called()
+    mock_send_messages.assert_called_once()
 
 
 @patch('pullbug.bug.Pullbug.get_issues', return_value=[])
 @patch('pullbug.bug.Pullbug.get_repos')
 @patch('logging.Logger.info')
 def test_run_no_issues(mock_logger, mock_get_repos, mock_issues):
     Pullbug(
```

### Comparing `pullbug-5.0.0/test/unit/test_messages.py` & `pullbug-5.0.1/test/unit/test_messages.py`

 * *Files identical despite different names*

