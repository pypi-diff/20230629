# Comparing `tmp/gspot_django_auth-0.0.7.tar.gz` & `tmp/gspot_django_auth-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.0.7.tar", last modified: Tue Jun 27 17:16:13 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.0.8.tar", last modified: Thu Jun 29 18:21:49 2023, max compression
```

## Comparing `gspot_django_auth-0.0.7.tar` & `gspot_django_auth-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 17:16:13.433357 gspot_django_auth-0.0.7/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.7/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.7/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-27 17:16:13.433441 gspot_django_auth-0.0.7/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      656 2023-06-27 14:59:12.000000 gspot_django_auth-0.0.7/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 17:16:13.432357 gspot_django_auth-0.0.7/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.7/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1210 2023-06-27 16:54:34.000000 gspot_django_auth-0.0.7/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      362 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.7/gspot_django_auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1204 2023-06-27 17:15:40.000000 gspot_django_auth-0.0.7/gspot_django_auth/models.py
--rw-r--r--   0 vitya      (501) staff       (20)      557 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.7/gspot_django_auth/permissions.py
--rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.7/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.7/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-27 17:16:13.433209 gspot_django_auth-0.0.7/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-27 17:16:13.000000 gspot_django_auth-0.0.7/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      487 2023-06-27 17:16:13.000000 gspot_django_auth-0.0.7/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-27 17:16:13.000000 gspot_django_auth-0.0.7/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-27 17:16:13.000000 gspot_django_auth-0.0.7/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-27 17:16:13.000000 gspot_django_auth-0.0.7/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-27 17:11:37.000000 gspot_django_auth-0.0.7/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-27 17:16:13.433761 gspot_django_auth-0.0.7/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)       37 2023-06-24 17:48:18.000000 gspot_django_auth-0.0.7/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:21:49.524361 gspot_django_auth-0.0.8/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.0.8/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.0.8/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:21:49.524458 gspot_django_auth-0.0.8/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      656 2023-06-27 14:59:12.000000 gspot_django_auth-0.0.8/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:21:49.523144 gspot_django_auth-0.0.8/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.0.8/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1210 2023-06-27 16:54:34.000000 gspot_django_auth-0.0.8/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      362 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.8/gspot_django_auth/exceptions.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1204 2023-06-27 17:15:40.000000 gspot_django_auth-0.0.8/gspot_django_auth/models.py
+-rw-r--r--   0 vitya      (501) staff       (20)      557 2023-06-27 16:34:36.000000 gspot_django_auth-0.0.8/gspot_django_auth/permissions.py
+-rw-r--r--   0 vitya      (501) staff       (20)      943 2023-06-27 12:40:56.000000 gspot_django_auth-0.0.8/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      712 2023-06-27 14:04:18.000000 gspot_django_auth-0.0.8/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-06-29 18:21:49.524209 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     1251 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      487 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-06-29 18:21:49.000000 gspot_django_auth-0.0.8/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-06-29 18:21:48.000000 gspot_django_auth-0.0.8/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-06-29 18:21:49.524799 gspot_django_auth-0.0.8/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      132 2023-06-29 18:20:10.000000 gspot_django_auth-0.0.8/setup.py
```

### Comparing `gspot_django_auth-0.0.7/LICENSE` & `gspot_django_auth-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/PKG-INFO` & `gspot_django_auth-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot_django_auth
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.7/README.md` & `gspot_django_auth-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/gspot_django_auth/authentication.py` & `gspot_django_auth-0.0.8/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/gspot_django_auth/models.py` & `gspot_django_auth-0.0.8/gspot_django_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/gspot_django_auth/permissions.py` & `gspot_django_auth-0.0.8/gspot_django_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.0.8/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/gspot_django_auth/token.py` & `gspot_django_auth-0.0.8/gspot_django_auth/token.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.0.7/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.0.8/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
```

### Comparing `gspot_django_auth-0.0.7/pyproject.toml` & `gspot_django_auth-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.0.7/setup.cfg` & `gspot_django_auth-0.0.8/setup.cfg`

 * *Files identical despite different names*

