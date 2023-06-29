# Comparing `tmp/sentry-ldap-1.2.7.tar.gz` & `tmp/sentry-ldap-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-ldap-1.2.7.tar", last modified: Thu Jun 29 04:30:38 2023, max compression
+gzip compressed data, was "sentry-ldap-1.2.8.tar", last modified: Thu Jun 29 05:33:19 2023, max compression
```

## Comparing `sentry-ldap-1.2.7.tar` & `sentry-ldap-1.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 04:30:38.923701 sentry-ldap-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 04:30:28.000000 sentry-ldap-1.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 04:30:38.923701 sentry-ldap-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 04:30:28.000000 sentry-ldap-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 04:30:38.923701 sentry-ldap-1.2.7/sentry_ldap/
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-29 04:30:28.000000 sentry-ldap-1.2.7/sentry_ldap/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 04:30:38.923701 sentry-ldap-1.2.7/sentry_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 04:30:38.000000 sentry-ldap-1.2.7/sentry_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 04:30:38.000000 sentry-ldap-1.2.7/sentry_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 04:30:38.000000 sentry-ldap-1.2.7/sentry_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 04:30:38.000000 sentry-ldap-1.2.7/sentry_ldap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 04:30:38.000000 sentry-ldap-1.2.7/sentry_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 04:30:38.000000 sentry-ldap-1.2.7/sentry_ldap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 04:30:38.923701 sentry-ldap-1.2.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-06-29 04:30:28.000000 sentry-ldap-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:33:19.106457 sentry-ldap-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 05:33:07.000000 sentry-ldap-1.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 05:33:19.106457 sentry-ldap-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 05:33:07.000000 sentry-ldap-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:33:19.106457 sentry-ldap-1.2.8/sentry_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-29 05:33:07.000000 sentry-ldap-1.2.8/sentry_ldap/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 05:33:19.106457 sentry-ldap-1.2.8/sentry_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 05:33:19.000000 sentry-ldap-1.2.8/sentry_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 05:33:19.000000 sentry-ldap-1.2.8/sentry_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 05:33:19.000000 sentry-ldap-1.2.8/sentry_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 05:33:18.000000 sentry-ldap-1.2.8/sentry_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 05:33:19.000000 sentry-ldap-1.2.8/sentry_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 05:33:19.000000 sentry-ldap-1.2.8/sentry_ldap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 05:33:19.106457 sentry-ldap-1.2.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-06-29 05:33:07.000000 sentry-ldap-1.2.8/setup.py
```

### Comparing `sentry-ldap-1.2.7/LICENSE.txt` & `sentry-ldap-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sentry-ldap-1.2.7/PKG-INFO` & `sentry-ldap-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-ldap
-Version: 1.2.7
+Version: 1.2.8
 Summary: A Sentry extension to add an LDAP server as an authentication source.
 Home-page: https://github.com/huynhminhtan/sentry-ldap
 Download-URL: https://github.com/huynhminhtan/sentry-ldap
 Author: 
 Author-email: 
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/huynhminhtan/sentry-ldap/issues
```

### Comparing `sentry-ldap-1.2.7/sentry_ldap/backend.py` & `sentry-ldap-1.2.8/sentry_ldap/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         return user
 
     def ldap_to_django_username(self, username):
         # Remove the domain part from the username
         logger.info(f'ldap_to_django_username LDAP username: {username}')
 
-        # username = username + '@' + settings.AUTH_LDAP_DEFAULT_EMAIL_DOMAIN
+        username = username + '@' + settings.AUTH_LDAP_DEFAULT_EMAIL_DOMAIN
 
         logger.info(f'ldap_to_django_username LDAP after username: {username}')
         return super().ldap_to_django_username(username)
 
     def django_to_ldap_username(self, username):
         logger.info(f'django_to_ldap_username LDAP username: {username}')
         return username
```

### Comparing `sentry-ldap-1.2.7/sentry_ldap.egg-info/PKG-INFO` & `sentry-ldap-1.2.8/sentry_ldap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-ldap
-Version: 1.2.7
+Version: 1.2.8
 Summary: A Sentry extension to add an LDAP server as an authentication source.
 Home-page: https://github.com/huynhminhtan/sentry-ldap
 Download-URL: https://github.com/huynhminhtan/sentry-ldap
 Author: 
 Author-email: 
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/huynhminhtan/sentry-ldap/issues
```

### Comparing `sentry-ldap-1.2.7/setup.py` & `sentry-ldap-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 install_requires = [
     'django-auth-ldap==4.1.0',
     'sentry>=23.6.0',
 ]
 
 setup(
     name='sentry-ldap',
-    version='1.2.7',
+    version='1.2.8',
     author='',
     author_email='',
     url='https://github.com/huynhminhtan/sentry-ldap',
     description='A Sentry extension to add an LDAP server as an authentication source.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(),
```

