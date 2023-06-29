# Comparing `tmp/django-cas-sso-1.2.7.tar.gz` & `tmp/django-cas-sso-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cas-sso-1.2.7.tar", last modified: Thu Dec 16 14:53:12 2021, max compression
+gzip compressed data, was "django-cas-sso-1.2.8.tar", last modified: Thu Jun 29 07:40:23 2023, max compression
```

## Comparing `django-cas-sso-1.2.7.tar` & `django-cas-sso-1.2.8.tar`

### file list

```diff
@@ -1,48 +1,40 @@
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.318093 django-cas-sso-1.2.7/
--rw-r--r--   0 toma      (1000) users      (985)      281 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/.gitignore
--rw-r--r--   0 toma      (1000) users      (985)      404 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/.travis.yml
--rw-r--r--   0 toma      (1000) users      (985)       43 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/MANIFEST.in
--rw-r--r--   0 toma      (1000) users      (985)     5304 2021-12-16 14:53:12.318093 django-cas-sso-1.2.7/PKG-INFO
--rw-r--r--   0 toma      (1000) users      (985)     4426 2021-12-16 14:49:15.000000 django-cas-sso-1.2.7/README.md
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.311093 django-cas-sso-1.2.7/django_cas/
--rw-r--r--   0 toma      (1000) users      (985)      899 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/django_cas/__init__.py
--rw-r--r--   0 toma      (1000) users      (985)      180 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/django_cas/apps.py
--rw-r--r--   0 toma      (1000) users      (985)     5029 2021-12-16 14:37:26.000000 django-cas-sso-1.2.7/django_cas/backends.py
--rw-r--r--   0 toma      (1000) users      (985)     3117 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/decorators.py
--rw-r--r--   0 toma      (1000) users      (985)      250 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/exceptions.py
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.311093 django-cas-sso-1.2.7/django_cas/management/
--rw-r--r--   0 toma      (1000) users      (985)        0 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/management/__init__.py
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.312093 django-cas-sso-1.2.7/django_cas/management/commands/
--rw-r--r--   0 toma      (1000) users      (985)        0 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/management/commands/__init__.py
--rw-r--r--   0 toma      (1000) users      (985)      599 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/management/commands/clearcassessions.py
--rw-r--r--   0 toma      (1000) users      (985)     4628 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/middleware.py
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.313093 django-cas-sso-1.2.7/django_cas/migrations/
--rw-r--r--   0 toma      (1000) users      (985)     1620 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/migrations/0001_initial.py
--rw-r--r--   0 toma      (1000) users      (985)        0 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/migrations/__init__.py
--rw-r--r--   0 toma      (1000) users      (985)     4910 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/models.py
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.314093 django-cas-sso-1.2.7/django_cas/tests/
--rw-r--r--   0 toma      (1000) users      (985)    12351 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/django_cas/tests/cas_tests.py
--rw-r--r--   0 toma      (1000) users      (985)      428 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/tests/get_pgt.py
--rw-r--r--   0 toma      (1000) users      (985)      199 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/django_cas/urls.py
--rw-r--r--   0 toma      (1000) users      (985)      459 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/django_cas/utils.py
--rw-r--r--   0 toma      (1000) users      (985)     7334 2021-12-16 14:37:26.000000 django-cas-sso-1.2.7/django_cas/views.py
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.316093 django-cas-sso-1.2.7/django_cas_sso.egg-info/
--rw-r--r--   0 toma      (1000) users      (985)     5304 2021-12-16 14:53:11.000000 django-cas-sso-1.2.7/django_cas_sso.egg-info/PKG-INFO
--rw-r--r--   0 toma      (1000) users      (985)      945 2021-12-16 14:53:12.000000 django-cas-sso-1.2.7/django_cas_sso.egg-info/SOURCES.txt
--rw-r--r--   0 toma      (1000) users      (985)        1 2021-12-16 14:53:11.000000 django-cas-sso-1.2.7/django_cas_sso.egg-info/dependency_links.txt
--rw-r--r--   0 toma      (1000) users      (985)        4 2021-12-16 14:53:11.000000 django-cas-sso-1.2.7/django_cas_sso.egg-info/requires.txt
--rw-r--r--   0 toma      (1000) users      (985)       17 2021-12-16 14:53:11.000000 django-cas-sso-1.2.7/django_cas_sso.egg-info/top_level.txt
--rw-r--r--   0 toma      (1000) users      (985)        1 2020-05-26 11:25:18.000000 django-cas-sso-1.2.7/django_cas_sso.egg-info/zip-safe
--rw-r--r--   0 toma      (1000) users      (985)       13 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/requirements-test.txt
--rw-r--r--   0 toma      (1000) users      (985)        4 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/requirements.txt
--rw-r--r--   0 toma      (1000) users      (985)     1481 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/runtests.py
--rw-r--r--   0 toma      (1000) users      (985)       67 2021-12-16 14:53:12.318093 django-cas-sso-1.2.7/setup.cfg
--rw-r--r--   0 toma      (1000) users      (985)     2300 2021-12-16 14:37:58.000000 django-cas-sso-1.2.7/setup.py
-drwxr-xr-x   0 toma      (1000) users      (985)        0 2021-12-16 14:53:12.317093 django-cas-sso-1.2.7/tests/
--rw-r--r--   0 toma      (1000) users      (985)        0 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/tests/__init__.py
--rw-r--r--   0 toma      (1000) users      (985)     1555 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/tests/test_clearsessions.py
--rw-r--r--   0 toma      (1000) users      (985)     2198 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/tests/test_middleware.py
--rw-r--r--   0 toma      (1000) users      (985)      192 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/tests/test_settings.py
--rw-r--r--   0 toma      (1000) users      (985)      507 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/tests/urls.py
--rw-r--r--   0 toma      (1000) users      (985)      239 2020-05-26 07:16:57.000000 django-cas-sso-1.2.7/tests/views.py
--rw-r--r--   0 toma      (1000) users      (985)      342 2021-12-16 13:53:46.000000 django-cas-sso-1.2.7/tox.ini
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.690371 django-cas-sso-1.2.8/
+-rw-r--r--   0 virgile    (503) staff       (20)       43 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/MANIFEST.in
+-rw-r--r--   0 virgile    (503) staff       (20)     5284 2023-06-29 07:40:23.690458 django-cas-sso-1.2.8/PKG-INFO
+-rw-r--r--   0 virgile    (503) staff       (20)     4426 2023-06-29 07:33:27.000000 django-cas-sso-1.2.8/README.md
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.687497 django-cas-sso-1.2.8/django_cas/
+-rw-r--r--   0 virgile    (503) staff       (20)      899 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/django_cas/__init__.py
+-rw-r--r--   0 virgile    (503) staff       (20)      180 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/django_cas/apps.py
+-rw-r--r--   0 virgile    (503) staff       (20)     5029 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/django_cas/backends.py
+-rw-r--r--   0 virgile    (503) staff       (20)     3117 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/decorators.py
+-rw-r--r--   0 virgile    (503) staff       (20)      250 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/exceptions.py
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.687640 django-cas-sso-1.2.8/django_cas/management/
+-rw-r--r--   0 virgile    (503) staff       (20)        0 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/management/__init__.py
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.687823 django-cas-sso-1.2.8/django_cas/management/commands/
+-rw-r--r--   0 virgile    (503) staff       (20)        0 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/management/commands/__init__.py
+-rw-r--r--   0 virgile    (503) staff       (20)      599 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/management/commands/clearcassessions.py
+-rw-r--r--   0 virgile    (503) staff       (20)     4628 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/django_cas/middleware.py
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.688359 django-cas-sso-1.2.8/django_cas/migrations/
+-rw-r--r--   0 virgile    (503) staff       (20)     1620 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/migrations/0001_initial.py
+-rw-r--r--   0 virgile    (503) staff       (20)        0 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/django_cas/migrations/__init__.py
+-rw-r--r--   0 virgile    (503) staff       (20)     4908 2023-06-29 07:31:05.000000 django-cas-sso-1.2.8/django_cas/models.py
+-rw-r--r--   0 virgile    (503) staff       (20)      191 2023-06-29 07:31:05.000000 django-cas-sso-1.2.8/django_cas/urls.py
+-rw-r--r--   0 virgile    (503) staff       (20)      459 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/django_cas/utils.py
+-rw-r--r--   0 virgile    (503) staff       (20)     7334 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/django_cas/views.py
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.689036 django-cas-sso-1.2.8/django_cas_sso.egg-info/
+-rw-r--r--   0 virgile    (503) staff       (20)     5284 2023-06-29 07:40:23.000000 django-cas-sso-1.2.8/django_cas_sso.egg-info/PKG-INFO
+-rw-r--r--   0 virgile    (503) staff       (20)      822 2023-06-29 07:40:23.000000 django-cas-sso-1.2.8/django_cas_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 virgile    (503) staff       (20)        1 2023-06-29 07:40:23.000000 django-cas-sso-1.2.8/django_cas_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 virgile    (503) staff       (20)        4 2023-06-29 07:40:23.000000 django-cas-sso-1.2.8/django_cas_sso.egg-info/requires.txt
+-rw-r--r--   0 virgile    (503) staff       (20)       17 2023-06-29 07:40:23.000000 django-cas-sso-1.2.8/django_cas_sso.egg-info/top_level.txt
+-rw-r--r--   0 virgile    (503) staff       (20)        1 2023-06-29 07:36:25.000000 django-cas-sso-1.2.8/django_cas_sso.egg-info/zip-safe
+-rw-r--r--   0 virgile    (503) staff       (20)        4 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/requirements.txt
+-rw-r--r--   0 virgile    (503) staff       (20)       67 2023-06-29 07:40:23.690783 django-cas-sso-1.2.8/setup.cfg
+-rw-r--r--   0 virgile    (503) staff       (20)     2300 2023-06-29 07:33:27.000000 django-cas-sso-1.2.8/setup.py
+drwxr-xr-x   0 virgile    (503) staff       (20)        0 2023-06-29 07:40:23.690059 django-cas-sso-1.2.8/tests/
+-rw-r--r--   0 virgile    (503) staff       (20)        0 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/tests/__init__.py
+-rw-r--r--   0 virgile    (503) staff       (20)     1555 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/tests/test_clearsessions.py
+-rw-r--r--   0 virgile    (503) staff       (20)     2198 2022-02-23 08:06:50.000000 django-cas-sso-1.2.8/tests/test_middleware.py
+-rw-r--r--   0 virgile    (503) staff       (20)      192 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/tests/test_settings.py
+-rw-r--r--   0 virgile    (503) staff       (20)      507 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/tests/urls.py
+-rw-r--r--   0 virgile    (503) staff       (20)      239 2019-10-07 16:03:46.000000 django-cas-sso-1.2.8/tests/views.py
```

### Comparing `django-cas-sso-1.2.7/PKG-INFO` & `django-cas-sso-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-cas-sso
-Version: 1.2.7
+Version: 1.2.8
 Summary: Django Cas SSO Client (inherited from django-cas)
 Home-page: http://github.com/unistra/django-cas/
+Download-URL: http://pypi.python.org/pypi/django-cas-sso
 Author: di-dip-unistra
 Author-email: di-dip@unistra.fr
 Maintainer: di-dip-unistra
 Maintainer-email: di-dip@unistra.fr
 License: MIT
-Download-URL: http://pypi.python.org/pypi/django-cas-sso
 Keywords: django,cas,sso
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
@@ -26,15 +25,15 @@
 
 [![Code Health](https://landscape.io/github/unistra/django-cas/master/landscape.svg?style=flat)](https://landscape.io/github/unistra/django-cas/master)
 
 CAS client for Django. This is K-State&#39;s fork of the original, which lives at
 https://bitbucket.org/cpcc/django-cas/overview. This fork is actively maintaned and
 includes several new features.
 
-Current version: 1.2.7
+Current version: 1.2.8
 
 https://github.com/kstateome/django-cas
 
 ## Install
 
 See the document at Bitbucket
 
@@ -164,9 +163,7 @@
 
 To force the service url to always target HTTPS, set `CAS_FORCE_SSL_SERVICE_URL` to `True`.
 
 ## Proxy Tickets
 
 This fork also includes Edmund Crewe's proxy ticket patch:
 http://code.google.com/r/edmundcrewe-proxypatch/source/browse/django-cas-proxy.patch
-
-
```

### Comparing `django-cas-sso-1.2.7/README.md` & `django-cas-sso-1.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![Code Health](https://landscape.io/github/unistra/django-cas/master/landscape.svg?style=flat)](https://landscape.io/github/unistra/django-cas/master)
 
 CAS client for Django. This is K-State&#39;s fork of the original, which lives at
 https://bitbucket.org/cpcc/django-cas/overview. This fork is actively maintaned and
 includes several new features.
 
-Current version: 1.2.7
+Current version: 1.2.8
 
 https://github.com/kstateome/django-cas
 
 ## Install
 
 See the document at Bitbucket
```

### Comparing `django-cas-sso-1.2.7/django_cas/__init__.py` & `django-cas-sso-1.2.8/django_cas/__init__.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas/backends.py` & `django-cas-sso-1.2.8/django_cas/backends.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas/decorators.py` & `django-cas-sso-1.2.8/django_cas/decorators.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas/management/commands/clearcassessions.py` & `django-cas-sso-1.2.8/django_cas/management/commands/clearcassessions.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas/middleware.py` & `django-cas-sso-1.2.8/django_cas/middleware.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas/migrations/0001_initial.py` & `django-cas-sso-1.2.8/django_cas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas/models.py` & `django-cas-sso-1.2.8/django_cas/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from django.db.models.signals import post_save
 from datetime import datetime
 # Single Sign Out
 from django.contrib.auth import BACKEND_SESSION_KEY
 from django.contrib.auth.signals import user_logged_out, user_logged_in
 from django.contrib.sessions.backends.db import SessionStore
 from django.dispatch import receiver
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class Tgt(models.Model):
     username = models.CharField(max_length=255, unique=True)
     tgt = models.CharField(max_length=255)
 
     def get_proxy_ticket_for(self, service):
@@ -69,15 +69,15 @@
     try:
         return Tgt.objects.get(username=user.username)
     except ObjectDoesNotExist:
         raise CasTicketException("no ticket found for user " + user.username)
 
 
 def delete_old_tickets(**kwargs):
-    """ Delete tickets if they are over 2 days old 
+    """ Delete tickets if they are over 2 days old
         kwargs = ['raw', 'signal', 'instance', 'sender', 'created']
     """
     sender = kwargs.get('sender', None)
     now = datetime.now()
     expire = datetime(now.year, now.month, now.day - 2)
     sender.objects.filter(created__lt=expire).delete()
```

### Comparing `django-cas-sso-1.2.7/django_cas/views.py` & `django-cas-sso-1.2.8/django_cas/views.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/django_cas_sso.egg-info/PKG-INFO` & `django-cas-sso-1.2.8/django_cas_sso.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-cas-sso
-Version: 1.2.7
+Version: 1.2.8
 Summary: Django Cas SSO Client (inherited from django-cas)
 Home-page: http://github.com/unistra/django-cas/
+Download-URL: http://pypi.python.org/pypi/django-cas-sso
 Author: di-dip-unistra
 Author-email: di-dip@unistra.fr
 Maintainer: di-dip-unistra
 Maintainer-email: di-dip@unistra.fr
 License: MIT
-Download-URL: http://pypi.python.org/pypi/django-cas-sso
 Keywords: django,cas,sso
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
@@ -26,15 +25,15 @@
 
 [![Code Health](https://landscape.io/github/unistra/django-cas/master/landscape.svg?style=flat)](https://landscape.io/github/unistra/django-cas/master)
 
 CAS client for Django. This is K-State&#39;s fork of the original, which lives at
 https://bitbucket.org/cpcc/django-cas/overview. This fork is actively maintaned and
 includes several new features.
 
-Current version: 1.2.7
+Current version: 1.2.8
 
 https://github.com/kstateome/django-cas
 
 ## Install
 
 See the document at Bitbucket
 
@@ -164,9 +163,7 @@
 
 To force the service url to always target HTTPS, set `CAS_FORCE_SSL_SERVICE_URL` to `True`.
 
 ## Proxy Tickets
 
 This fork also includes Edmund Crewe's proxy ticket patch:
 http://code.google.com/r/edmundcrewe-proxypatch/source/browse/django-cas-proxy.patch
-
-
```

### Comparing `django-cas-sso-1.2.7/django_cas_sso.egg-info/SOURCES.txt` & `django-cas-sso-1.2.8/django_cas_sso.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-.gitignore
-.travis.yml
 MANIFEST.in
 README.md
-requirements-test.txt
 requirements.txt
-runtests.py
 setup.cfg
 setup.py
-tox.ini
 django_cas/__init__.py
 django_cas/apps.py
 django_cas/backends.py
 django_cas/decorators.py
 django_cas/exceptions.py
 django_cas/middleware.py
 django_cas/models.py
@@ -19,16 +14,14 @@
 django_cas/utils.py
 django_cas/views.py
 django_cas/management/__init__.py
 django_cas/management/commands/__init__.py
 django_cas/management/commands/clearcassessions.py
 django_cas/migrations/0001_initial.py
 django_cas/migrations/__init__.py
-django_cas/tests/cas_tests.py
-django_cas/tests/get_pgt.py
 django_cas_sso.egg-info/PKG-INFO
 django_cas_sso.egg-info/SOURCES.txt
 django_cas_sso.egg-info/dependency_links.txt
 django_cas_sso.egg-info/requires.txt
 django_cas_sso.egg-info/top_level.txt
 django_cas_sso.egg-info/zip-safe
 tests/__init__.py
```

### Comparing `django-cas-sso-1.2.7/setup.py` & `django-cas-sso-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-version = '1.2.7'
+version = '1.2.8'
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 def recursive_requirements(requirement_file, libs, links, path=''):
     if not requirement_file.startswith(path):
         requirement_file = os.path.join(path, requirement_file)
```

### Comparing `django-cas-sso-1.2.7/tests/test_clearsessions.py` & `django-cas-sso-1.2.8/tests/test_clearsessions.py`

 * *Files identical despite different names*

### Comparing `django-cas-sso-1.2.7/tests/test_middleware.py` & `django-cas-sso-1.2.8/tests/test_middleware.py`

 * *Files identical despite different names*

