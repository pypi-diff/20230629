# Comparing `tmp/arq-django-admin-0.2.4.tar.gz` & `tmp/arq-django-admin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arq-django-admin-0.2.4.tar", last modified: Thu Nov 17 13:19:06 2022, max compression
+gzip compressed data, was "arq-django-admin-0.3.0.tar", last modified: Thu Jun 29 11:44:17 2023, max compression
```

## Comparing `arq-django-admin-0.2.4.tar` & `arq-django-admin-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/arq_admin/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/job.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4711 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/arq_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/arq_admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/templates/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/arq_admin/templates/arq_admin/
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/templates/arq_admin/job_abort.html
--rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/templates/arq_admin/job_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/templates/arq_admin/jobs.html
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/templates/arq_admin/queues.html
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/arq_admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/arq_django_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-17 13:19:06.000000 arq-django-admin-0.2.4/arq_django_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-17 13:19:06.000000 arq-django-admin-0.2.4/arq_django_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 13:19:06.000000 arq-django-admin-0.2.4/arq_django_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-17 13:19:06.000000 arq-django-admin-0.2.4/arq_django_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-17 13:19:06.000000 arq-django-admin-0.2.4/arq_django_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 13:19:06.000000 arq-django-admin-0.2.4/arq_django_admin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-11-17 13:19:06.259405 arq-django-admin-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-17 13:18:57.000000 arq-django-admin-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_abort.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/jobs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/templates/arq_admin/queues.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/arq_admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:44:17.110884 arq-django-admin-0.3.0/arq_django_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:44:17.000000 arq-django-admin-0.3.0/arq_django_admin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-29 11:44:17.114884 arq-django-admin-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-29 11:44:05.000000 arq-django-admin-0.3.0/setup.py
```

### Comparing `arq-django-admin-0.2.4/LICENSE` & `arq-django-admin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/PKG-INFO` & `arq-django-admin-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arq-django-admin
-Version: 0.2.4
+Version: 0.3.0
 Summary: An app that provides Django admin for ARQ
 Home-page: https://github.com/SlavaSkvortsov/arq-django-admin
 Author: Slava Skvortsov
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arq-django-admin-0.2.4/README.md` & `arq-django-admin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/job.py` & `arq-django-admin-0.3.0/arq_admin/job.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/settings.py` & `arq-django-admin-0.3.0/arq_admin/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 
     if ARQ_DESERIALIZER_BY_QUEUE:
         raise ImproperlyConfigured('You cannot define both ARQ_DESERIALIZER and ARQ_DESERIALIZER_BY_QUEUE')
 
     ARQ_DESERIALIZER_BY_QUEUE = defaultdict(lambda: ARQ_DESERIALIZER)
 
 ARQ_JOB_ABORT_TIMEOUT = getattr(settings, 'ARQ_JOB_ABORT_TIMEOUT', 5)
+
+ARQ_MAX_CONNECTIONS = getattr(settings, 'ARQ_MAX_CONNECTIONS', 100)
```

### Comparing `arq-django-admin-0.2.4/arq_admin/templates/arq_admin/job_abort.html` & `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_abort.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/templates/arq_admin/job_detail.html` & `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/job_detail.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/templates/arq_admin/jobs.html` & `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/jobs.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/templates/arq_admin/queues.html` & `arq-django-admin-0.3.0/arq_admin/templates/arq_admin/queues.html`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/urls.py` & `arq-django-admin-0.3.0/arq_admin/urls.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_admin/views.py` & `arq-django-admin-0.3.0/arq_admin/views.py`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/arq_django_admin.egg-info/PKG-INFO` & `arq-django-admin-0.3.0/arq_django_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arq-django-admin
-Version: 0.2.4
+Version: 0.3.0
 Summary: An app that provides Django admin for ARQ
 Home-page: https://github.com/SlavaSkvortsov/arq-django-admin
 Author: Slava Skvortsov
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arq-django-admin-0.2.4/arq_django_admin.egg-info/SOURCES.txt` & `arq-django-admin-0.3.0/arq_django_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/setup.cfg` & `arq-django-admin-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arq-django-admin-0.2.4/setup.py` & `arq-django-admin-0.3.0/setup.py`

 * *Files identical despite different names*

