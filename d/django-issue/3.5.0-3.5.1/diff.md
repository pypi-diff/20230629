# Comparing `tmp/django-issue-3.5.0.tar.gz` & `tmp/django-issue-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-issue-3.5.0.tar", last modified: Thu Jun 29 00:32:22 2023, max compression
+gzip compressed data, was "django-issue-3.5.1.tar", last modified: Thu Jun 29 13:52:09 2023, max compression
```

## Comparing `django-issue-3.5.0.tar` & `django-issue-3.5.1.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.141413 django-issue-3.5.0/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-01-23 14:57:04.000000 django-issue-3.5.0/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       34 2023-01-23 14:57:04.000000 django-issue-3.5.0/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     1890 2023-06-29 00:32:22.141413 django-issue-3.5.0/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1105 2023-01-23 14:57:04.000000 django-issue-3.5.0/README.rst
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.137413 django-issue-3.5.0/django_issue.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1890 2023-06-29 00:32:22.000000 django-issue-3.5.0/django_issue.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)      909 2023-06-29 00:32:22.000000 django-issue-3.5.0/django_issue.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 00:32:22.000000 django-issue-3.5.0/django_issue.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 00:32:21.000000 django-issue-3.5.0/django_issue.egg-info/not-zip-safe
--rw-rw-r--   0 wes       (1000) wes       (1000)       66 2023-06-29 00:32:22.000000 django-issue-3.5.0/django_issue.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        6 2023-06-29 00:32:22.000000 django-issue-3.5.0/django_issue.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.137413 django-issue-3.5.0/issue/
--rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      427 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/actions.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      119 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      417 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/builder.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      764 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/check.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.137413 django-issue-3.5.0/issue/management/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/management/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.137413 django-issue-3.5.0/issue/management/commands/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/management/commands/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      257 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/management/commands/check_assertions.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      241 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/management/commands/respond_to_issues.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.137413 django-issue-3.5.0/issue/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     4870 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/migrations/0001_0004_squashed.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1251 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/migrations/0005_responder_allow_retry.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/migrations/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.141413 django-issue-3.5.0/issue/migrations/datamigrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)      499 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/migrations/datamigrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    13365 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 00:32:22.141413 django-issue-3.5.0/issue/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1433 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/tests/action_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1927 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/tests/builder_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2174 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/tests/checker_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      604 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/tests/management_command_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    25131 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      114 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-01-23 14:57:04.000000 django-issue-3.5.0/issue/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 00:24:39.000000 django-issue-3.5.0/issue/version.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      253 2023-06-29 00:32:22.141413 django-issue-3.5.0/setup.cfg
--rwxrwxr-x   0 wes       (1000) wes       (1000)     1822 2023-06-29 00:24:39.000000 django-issue-3.5.0/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-01-23 14:57:04.000000 django-issue-3.5.1/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2023-06-29 13:48:27.000000 django-issue-3.5.1/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1890 2023-06-29 13:52:09.720062 django-issue-3.5.1/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1105 2023-01-23 14:57:04.000000 django-issue-3.5.1/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/django_issue.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1890 2023-06-29 13:52:09.000000 django-issue-3.5.1/django_issue.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      999 2023-06-29 13:52:09.000000 django-issue-3.5.1/django_issue.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 13:52:09.000000 django-issue-3.5.1/django_issue.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 00:32:21.000000 django-issue-3.5.1/django_issue.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)       66 2023-06-29 13:52:09.000000 django-issue-3.5.1/django_issue.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        6 2023-06-29 13:52:09.000000 django-issue-3.5.1/django_issue.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/issue/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-29 00:24:39.000000 django-issue-3.5.1/issue/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      427 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/actions.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      119 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      417 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/builder.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      764 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/check.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/issue/management/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/management/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/issue/management/commands/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/management/commands/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      257 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/management/commands/check_assertions.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      241 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/management/commands/respond_to_issues.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/issue/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4870 2023-06-29 00:24:39.000000 django-issue-3.5.1/issue/migrations/0001_0004_squashed.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1251 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/migrations/0005_responder_allow_retry.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/migrations/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/issue/migrations/datamigrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      499 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/migrations/datamigrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    13365 2023-06-29 00:24:39.000000 django-issue-3.5.1/issue/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/issue/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1433 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/tests/action_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1927 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/tests/builder_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2174 2023-06-29 00:24:39.000000 django-issue-3.5.1/issue/tests/checker_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      604 2023-06-29 00:24:39.000000 django-issue-3.5.1/issue/tests/management_command_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    25131 2023-06-29 00:24:39.000000 django-issue-3.5.1/issue/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      114 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-01-23 14:57:04.000000 django-issue-3.5.1/issue/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 13:48:42.000000 django-issue-3.5.1/issue/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:52:09.720062 django-issue-3.5.1/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2023-01-23 14:57:04.000000 django-issue-3.5.1/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       70 2023-06-29 00:24:39.000000 django-issue-3.5.1/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       89 2023-06-29 00:24:39.000000 django-issue-3.5.1/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      253 2023-06-29 13:52:09.720062 django-issue-3.5.1/setup.cfg
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1822 2023-06-29 00:24:39.000000 django-issue-3.5.1/setup.py
```

### Comparing `django-issue-3.5.0/LICENSE` & `django-issue-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/PKG-INFO` & `django-issue-3.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-issue
-Version: 3.5.0
+Version: 3.5.1
 Summary: An app for tracking ongoing issues within your web application!
 Home-page: https://github.com/ambitioninc/django-issue
 Author: Josh Marlow
 Author-email: opensource@ambition.com
 License: MIT
 Keywords: python,issue
 Classifier: Programming Language :: Python
```

### Comparing `django-issue-3.5.0/README.rst` & `django-issue-3.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/django_issue.egg-info/PKG-INFO` & `django-issue-3.5.1/django_issue.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-issue
-Version: 3.5.0
+Version: 3.5.1
 Summary: An app for tracking ongoing issues within your web application!
 Home-page: https://github.com/ambitioninc/django-issue
 Author: Josh Marlow
 Author-email: opensource@ambition.com
 License: MIT
 Keywords: python,issue
 Classifier: Programming Language :: Python
```

### Comparing `django-issue-3.5.0/issue/check.py` & `django-issue-3.5.1/issue/check.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/migrations/0001_0004_squashed.py` & `django-issue-3.5.1/issue/migrations/0001_0004_squashed.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/migrations/0005_responder_allow_retry.py` & `django-issue-3.5.1/issue/migrations/0005_responder_allow_retry.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/models.py` & `django-issue-3.5.1/issue/models.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/tests/action_tests.py` & `django-issue-3.5.1/issue/tests/action_tests.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/tests/builder_tests.py` & `django-issue-3.5.1/issue/tests/builder_tests.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/tests/checker_tests.py` & `django-issue-3.5.1/issue/tests/checker_tests.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/tests/management_command_tests.py` & `django-issue-3.5.1/issue/tests/management_command_tests.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/issue/tests/model_tests.py` & `django-issue-3.5.1/issue/tests/model_tests.py`

 * *Files identical despite different names*

### Comparing `django-issue-3.5.0/setup.py` & `django-issue-3.5.1/setup.py`

 * *Files identical despite different names*

