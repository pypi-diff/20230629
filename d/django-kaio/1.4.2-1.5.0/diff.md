# Comparing `tmp/django-kaio-1.4.2.tar.gz` & `tmp/django-kaio-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-kaio-1.4.2.tar", last modified: Thu Jan 19 14:12:26 2023, max compression
+gzip compressed data, was "django-kaio-1.5.0.tar", last modified: Thu Jun 29 14:36:48 2023, max compression
```

## Comparing `django-kaio-1.4.2.tar` & `django-kaio-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 dani      (1000) dani      (1000)        0 2023-01-19 14:12:26.000000 django-kaio-1.4.2/
--rw-rw-r--   0 dani      (1000) dani      (1000)       41 2020-11-05 07:51:29.000000 django-kaio-1.4.2/MANIFEST.in
--rw-rw-r--   0 dani      (1000) dani      (1000)     2184 2022-05-05 09:09:00.000000 django-kaio-1.4.2/setup.py
--rw-rw-r--   0 dani      (1000) dani      (1000)      376 2020-11-05 07:51:29.000000 django-kaio-1.4.2/README.rst
-drwxrwxr-x   0 dani      (1000) dani      (1000)        0 2023-01-19 14:12:26.000000 django-kaio-1.4.2/kaio/
-drwxrwxr-x   0 dani      (1000) dani      (1000)        0 2023-01-19 14:12:26.000000 django-kaio-1.4.2/kaio/management/
-drwxrwxr-x   0 dani      (1000) dani      (1000)        0 2023-01-19 14:12:26.000000 django-kaio-1.4.2/kaio/management/commands/
--rw-rw-r--   0 dani      (1000) dani      (1000)     3404 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/management/commands/kaiosettings.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1860 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/management/commands/generate_ini.py
--rw-rw-r--   0 dani      (1000) dani      (1000)        0 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/management/commands/__init__.py
--rw-rw-r--   0 dani      (1000) dani      (1000)        0 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/management/__init__.py
--rw-rw-r--   0 dani      (1000) dani      (1000)      517 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/properties.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     5668 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/options.py
-drwxrwxr-x   0 dani      (1000) dani      (1000)        0 2023-01-19 14:12:26.000000 django-kaio-1.4.2/kaio/mixins/
--rw-rw-r--   0 dani      (1000) dani      (1000)     5210 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/filerconf.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     2560 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/compress.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1122 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/security.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     2312 2022-05-02 08:22:50.000000 django-kaio-1.4.2/kaio/mixins/debug.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     3546 2023-01-19 14:06:11.000000 django-kaio-1.4.2/kaio/mixins/email.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     4241 2022-05-05 09:00:21.000000 django-kaio-1.4.2/kaio/mixins/logs.py
--rw-rw-r--   0 dani      (1000) dani      (1000)      720 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/paths.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1817 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/whitenoise.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1108 2022-05-09 10:09:34.000000 django-kaio-1.4.2/kaio/mixins/sentry.py
--rw-rw-r--   0 dani      (1000) dani      (1000)      826 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/cms.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1493 2022-05-11 07:45:40.000000 django-kaio-1.4.2/kaio/mixins/storage.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     4781 2022-05-30 09:14:53.000000 django-kaio-1.4.2/kaio/mixins/celeryconf.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     4595 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/cache.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1502 2020-11-05 07:51:29.000000 django-kaio-1.4.2/kaio/mixins/database.py
--rw-rw-r--   0 dani      (1000) dani      (1000)      709 2022-05-05 09:00:21.000000 django-kaio-1.4.2/kaio/mixins/__init__.py
--rw-rw-r--   0 dani      (1000) dani      (1000)       86 2023-01-19 14:08:43.000000 django-kaio-1.4.2/kaio/__init__.py
--rw-rw-r--   0 dani      (1000) dani      (1000)     1991 2023-01-19 14:12:26.000000 django-kaio-1.4.2/PKG-INFO
--rw-rw-r--   0 dani      (1000) dani      (1000)       38 2023-01-19 14:12:26.000000 django-kaio-1.4.2/setup.cfg
--rw-rw-r--   0 dani      (1000) dani      (1000)     3612 2023-01-19 14:09:18.000000 django-kaio-1.4.2/CHANGELOG.rst
--rw-rw-r--   0 dani      (1000) dani      (1000)     1473 2020-11-05 07:51:29.000000 django-kaio-1.4.2/LICENSE
-drwxrwxr-x   0 dani      (1000) dani      (1000)        0 2023-01-19 14:12:26.000000 django-kaio-1.4.2/django_kaio.egg-info/
--rw-rw-r--   0 dani      (1000) dani      (1000)      801 2023-01-19 14:12:26.000000 django-kaio-1.4.2/django_kaio.egg-info/SOURCES.txt
--rw-rw-r--   0 dani      (1000) dani      (1000)        1 2020-11-05 08:00:38.000000 django-kaio-1.4.2/django_kaio.egg-info/not-zip-safe
--rw-rw-r--   0 dani      (1000) dani      (1000)        5 2023-01-19 14:12:26.000000 django-kaio-1.4.2/django_kaio.egg-info/top_level.txt
--rw-rw-r--   0 dani      (1000) dani      (1000)     1991 2023-01-19 14:12:26.000000 django-kaio-1.4.2/django_kaio.egg-info/PKG-INFO
--rw-rw-r--   0 dani      (1000) dani      (1000)        1 2023-01-19 14:12:26.000000 django-kaio-1.4.2/django_kaio.egg-info/dependency_links.txt
--rw-rw-r--   0 dani      (1000) dani      (1000)       47 2023-01-19 14:12:26.000000 django-kaio-1.4.2/django_kaio.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:48.451278 django-kaio-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-29 14:36:39.000000 django-kaio-1.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-29 14:36:39.000000 django-kaio-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 14:36:39.000000 django-kaio-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-29 14:36:48.455278 django-kaio-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-29 14:36:39.000000 django-kaio-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:48.451278 django-kaio-1.5.0/django_kaio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-29 14:36:48.000000 django-kaio-1.5.0/django_kaio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-29 14:36:48.000000 django-kaio-1.5.0/django_kaio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:36:48.000000 django-kaio-1.5.0/django_kaio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:36:48.000000 django-kaio-1.5.0/django_kaio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 14:36:48.000000 django-kaio-1.5.0/django_kaio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 14:36:48.000000 django-kaio-1.5.0/django_kaio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:48.451278 django-kaio-1.5.0/kaio/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:48.451278 django-kaio-1.5.0/kaio/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:48.451278 django-kaio-1.5.0/kaio/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/management/commands/generate_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/management/commands/kaiosettings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:36:48.451278 django-kaio-1.5.0/kaio/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/celeryconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/cms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/filerconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/mixins/whitenoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-29 14:36:39.000000 django-kaio-1.5.0/kaio/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 14:36:48.455278 django-kaio-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-29 14:36:39.000000 django-kaio-1.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-kaio-1.4.2/setup.py` & `django-kaio-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,22 +48,27 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 1.8',
         'Framework :: Django :: 1.9',
         'Framework :: Django :: 1.10',
         'Framework :: Django :: 1.11',
         'Framework :: Django :: 2.0',
         'Framework :: Django :: 2.1',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `django-kaio-1.4.2/kaio/management/commands/kaiosettings.py` & `django-kaio-1.5.0/kaio/management/commands/kaiosettings.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/management/commands/generate_ini.py` & `django-kaio-1.5.0/kaio/management/commands/generate_ini.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/properties.py` & `django-kaio-1.5.0/kaio/properties.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/options.py` & `django-kaio-1.5.0/kaio/options.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/filerconf.py` & `django-kaio-1.5.0/kaio/mixins/filerconf.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/compress.py` & `django-kaio-1.5.0/kaio/mixins/compress.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/security.py` & `django-kaio-1.5.0/kaio/mixins/security.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/debug.py` & `django-kaio-1.5.0/kaio/mixins/debug.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/email.py` & `django-kaio-1.5.0/kaio/mixins/email.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/logs.py` & `django-kaio-1.5.0/kaio/mixins/logs.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/paths.py` & `django-kaio-1.5.0/kaio/mixins/paths.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/whitenoise.py` & `django-kaio-1.5.0/kaio/mixins/whitenoise.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/sentry.py` & `django-kaio-1.5.0/kaio/mixins/sentry.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/cms.py` & `django-kaio-1.5.0/kaio/mixins/cms.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/storage.py` & `django-kaio-1.5.0/kaio/mixins/storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # -*- coding: utf-8 -*-
 
 from functools import partial
 
+import django
 from kaio import Options
 
 
 opts = Options()
 get = partial(opts.get, section='Storage')
 
 
-class StorageMixin(object):
+class _BaseStorage(object):
     """Settings for django-storages
 
     Currently only supports AWS S3 with and without CloudFront.
     """
 
     # AWS S3 settings: http://django-storages.readthedocs.io/en/latest/backends/amazon-S3.html
 
     @property
-    def DEFAULT_FILE_STORAGE(self):
-        return get('DEFAULT_FILE_STORAGE', 'storages.backends.s3boto3.S3Boto3Storage')
-
-    @property
     def AWS_S3_SIGNATURE_VERSION(self):
         return get('AWS_S3_SIGNATURE_VERSION', 's3v4')
 
     @property
     def AWS_S3_REGION_NAME(self):
         return get('AWS_S3_REGION_NAME', None)
 
@@ -56,7 +53,28 @@
     @property
     def AWS_QUERYSTRING_AUTH(self):
         return get('AWS_QUERYSTRING_AUTH', True)
 
     @property
     def AWS_DEFAULT_ACL(self):
         return get('AWS_DEFAULT_ACL', 'private')
+
+
+if django.VERSION[:2] < (4, 2):
+    class StorageMixin(_BaseStorage):
+        @property
+        def DEFAULT_FILE_STORAGE(self):
+            return get('DEFAULT_FILE_STORAGE', 'storages.backends.s3boto3.S3Boto3Storage')
+else:
+    class StorageMixin(_BaseStorage):
+        @property
+        def STORAGES(self):
+            return {
+                "default": {
+                    "BACKEND": get('DEFAULT_BACKEND_STORAGE',
+                                   'storages.backends.s3boto3.S3Boto3Storage')
+                },
+                "staticfiles": {
+                    "BACKEND": get('STATICFILES_BACKEND_STORAGE',
+                                   'django.contrib.staticfiles.storage.StaticFilesStorage')
+                },
+            }
```

### Comparing `django-kaio-1.4.2/kaio/mixins/celeryconf.py` & `django-kaio-1.5.0/kaio/mixins/celeryconf.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/cache.py` & `django-kaio-1.5.0/kaio/mixins/cache.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/database.py` & `django-kaio-1.5.0/kaio/mixins/database.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/kaio/mixins/__init__.py` & `django-kaio-1.5.0/kaio/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/PKG-INFO` & `django-kaio-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-kaio
-Version: 1.4.2
+Version: 1.5.0
 Summary: Class based settings for Django projects that can be read from multiple sources
 Home-page: https://github.com/APSL/django-kaio
 Author: APSL
 Author-email: engineering@apsl.net
 License: BSD
-Description: ===========
-        django-kaio
-        ===========
-        
-        .. image:: https://img.shields.io/pypi/v/django-kaio.svg
-            :target: https://pypi.python.org/pypi/django-kaio/
-        
-        Class based settings for Django projects that can be read from multiple sources.
-        
-        
-        Documentation
-        -------------
-        Visit the `documentation <http://django-kaio.readthedocs.io/en/latest/>`_ for an in-depth look at **django-kaio**.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -33,18 +18,38 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+===========
+django-kaio
+===========
+
+.. image:: https://img.shields.io/pypi/v/django-kaio.svg
+    :target: https://pypi.python.org/pypi/django-kaio/
+
+Class based settings for Django projects that can be read from multiple sources.
+
+
+Documentation
+-------------
+Visit the `documentation <http://django-kaio.readthedocs.io/en/latest/>`_ for an in-depth look at **django-kaio**.
```

### Comparing `django-kaio-1.4.2/CHANGELOG.rst` & `django-kaio-1.5.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ==========
 Change log
 ==========
 
+v1.5.0 (2023-06-29)
+--------------------
+
+* Support Python 3.11 and Django 4.2.
+* Migrate ReadTheDocs configuration file to v2.
+* GitHub Actions to deploy to PyPI.
+
 v1.4.2 (2023-01-19)
 --------------------
 
 * Add more settings for django_yubin: MAILER_STORAGE_DELETE.
 
 v1.4.1 (2023-01-11)
 --------------------
```

### Comparing `django-kaio-1.4.2/LICENSE` & `django-kaio-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-kaio-1.4.2/django_kaio.egg-info/SOURCES.txt` & `django-kaio-1.5.0/django_kaio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 django_kaio.egg-info/PKG-INFO
 django_kaio.egg-info/SOURCES.txt
 django_kaio.egg-info/dependency_links.txt
 django_kaio.egg-info/not-zip-safe
 django_kaio.egg-info/requires.txt
 django_kaio.egg-info/top_level.txt
```

### Comparing `django-kaio-1.4.2/django_kaio.egg-info/PKG-INFO` & `django-kaio-1.5.0/django_kaio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-kaio
-Version: 1.4.2
+Version: 1.5.0
 Summary: Class based settings for Django projects that can be read from multiple sources
 Home-page: https://github.com/APSL/django-kaio
 Author: APSL
 Author-email: engineering@apsl.net
 License: BSD
-Description: ===========
-        django-kaio
-        ===========
-        
-        .. image:: https://img.shields.io/pypi/v/django-kaio.svg
-            :target: https://pypi.python.org/pypi/django-kaio/
-        
-        Class based settings for Django projects that can be read from multiple sources.
-        
-        
-        Documentation
-        -------------
-        Visit the `documentation <http://django-kaio.readthedocs.io/en/latest/>`_ for an in-depth look at **django-kaio**.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -33,18 +18,38 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+===========
+django-kaio
+===========
+
+.. image:: https://img.shields.io/pypi/v/django-kaio.svg
+    :target: https://pypi.python.org/pypi/django-kaio/
+
+Class based settings for Django projects that can be read from multiple sources.
+
+
+Documentation
+-------------
+Visit the `documentation <http://django-kaio.readthedocs.io/en/latest/>`_ for an in-depth look at **django-kaio**.
```

