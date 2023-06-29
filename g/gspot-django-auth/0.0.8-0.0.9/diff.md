# Comparing `tmp/gspot_django_auth-0.0.8.tar.gz` & `tmp/gspot_django_auth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.0.8.tar", last modified: Thu Jun 29 18:21:49 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.0.9.tar", last modified: Thu Jun 29 18:24:47 2023, max compression
```

## Comparing `gspot_django_auth-0.0.8.tar` & `gspot_django_auth-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:21:49.524361 gspot_django_auth-0.0.8/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.8/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.8/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:21:49.524458 gspot_django_auth-0.0.8/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      656 2023-06-27 14:59:12.000000 gspot_django_auth-0.0.8/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:21:49.523144 gspot_django_auth-0.0.8/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.8/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1210 2023-06-27 16:54:34.000000 gspot_django_auth-0.0.8/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      362 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.8/gspot_django_auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1204 2023-06-27 17:15:40.000000 gspot_django_auth-0.0.8/gspot_django_auth/models.py
--rw-r--r--   0 vitya      (501) staff       (20)      557 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.8/gspot_django_auth/permissions.py
--rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.8/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.8/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:21:49.524209 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      487 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-29 18:21:48.000000 gspot_django_auth-0.0.8/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-29 18:21:49.524799 gspot_django_auth-0.0.8/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      132 2023-06-29 18:20:10.000000 gspot_django_auth-0.0.8/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:24:47.284955 gspot_django_auth-0.0.9/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.9/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.9/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:24:47.285071 gspot_django_auth-0.0.9/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      656 2023-06-29 18:24:44.000000 gspot_django_auth-0.0.9/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:24:47.283858 gspot_django_auth-0.0.9/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.9/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-06-29 18:23:56.000000 gspot_django_auth-0.0.9/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      362 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.9/gspot_django_auth/exceptions.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1204 2023-06-27 17:15:40.000000 gspot_django_auth-0.0.9/gspot_django_auth/models.py
+-rw-r--r--   0 vitya      (501) staff       (20)      557 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.9/gspot_django_auth/permissions.py
+-rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.9/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.9/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:24:47.284790 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      487 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-29 18:24:47.000000 gspot_django_auth-0.0.9/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-29 18:24:17.000000 gspot_django_auth-0.0.9/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-29 18:24:47.285433 gspot_django_auth-0.0.9/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      132 2023-06-29 18:20:10.000000 gspot_django_auth-0.0.9/setup.py
```

### Comparing `gspot_django_auth-0.0.8/LICENSE` & `gspot_django_auth-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.8/PKG-INFO` & `gspot_django_auth-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_django_auth
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
@@ -36,15 +36,15 @@
 - `REDIS_ACCESS_PREFIX`
 - `REDIS_ACCESS_DB`
 - `REDIS_HOST`
 - `REDIS_PORT`
 - `REDIS_PASSWORD`
 - `GET_TOKEN_FROM` - 'headers' or 'cookies'
 
-2. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
+3. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
 
 ```
 REST_FRAMEWORK = {
     ...
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'gspot_django_auth.authentication.CustomJWTAuthentication'
     ],
```

### Comparing `gspot_django_auth-0.0.8/README.md` & `gspot_django_auth-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - `REDIS_ACCESS_PREFIX`
 - `REDIS_ACCESS_DB`
 - `REDIS_HOST`
 - `REDIS_PORT`
 - `REDIS_PASSWORD`
 - `GET_TOKEN_FROM` - 'headers' or 'cookies'
 
-2. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
+3. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
 
 ```
 REST_FRAMEWORK = {
     ...
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'gspot_django_auth.authentication.CustomJWTAuthentication'
     ],
```

### Comparing `gspot_django_auth-0.0.8/gspot_django_auth/authentication.py` & `gspot_django_auth-0.0.9/gspot_django_auth/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from django.conf import settings
 from rest_framework.authentication import BaseAuthentication
 
-from .models import UserFactory
 from .exceptions import AuthenticationFailed
+from .models import UserFactory
 from .token import Token
 
 
 class CustomJWTAuthentication(BaseAuthentication):
     def authenticate(self, request):
         jwt_token = self.get_token(request)
         token = Token()
 
         data = token.get_token_data(jwt_token)
         if not data:
             raise AuthenticationFailed('No data')
         user_class = UserFactory().get_user(data.pop('role'))
-        return user_class(**data)
+        return user_class(**data), jwt_token
 
     def get_token(self, request) -> str:
         if settings.GET_TOKEN_FROM == 'headers':
             token = self._get_token_from_header(request)
         else:
             token = self._get_token_from_cookies(request)
```

### Comparing `gspot_django_auth-0.0.8/gspot_django_auth/models.py` & `gspot_django_auth-0.0.9/gspot_django_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.8/gspot_django_auth/permissions.py` & `gspot_django_auth-0.0.9/gspot_django_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.8/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.0.9/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.8/gspot_django_auth/token.py` & `gspot_django_auth-0.0.9/gspot_django_auth/token.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.8/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.0.9/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
@@ -36,15 +36,15 @@
 - `REDIS_ACCESS_PREFIX`
 - `REDIS_ACCESS_DB`
 - `REDIS_HOST`
 - `REDIS_PORT`
 - `REDIS_PASSWORD`
 - `GET_TOKEN_FROM` - 'headers' or 'cookies'
 
-2. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
+3. Add CustomJWTAuthentication to DEFAULT_AUTHENTICATION_CLASSES in settings.py
 
 ```
 REST_FRAMEWORK = {
     ...
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'gspot_django_auth.authentication.CustomJWTAuthentication'
     ],
```

### Comparing `gspot_django_auth-0.0.8/pyproject.toml` & `gspot_django_auth-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.0.8/setup.cfg` & `gspot_django_auth-0.0.9/setup.cfg`

 * *Files identical despite different names*

