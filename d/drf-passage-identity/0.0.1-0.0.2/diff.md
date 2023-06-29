# Comparing `tmp/drf-passage-identity-0.0.1.tar.gz` & `tmp/drf-passage-identity-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-passage-identity-0.0.1.tar", last modified: Wed Jun 28 10:35:20 2023, max compression
+gzip compressed data, was "drf-passage-identity-0.0.2.tar", last modified: Thu Jun 29 12:44:48 2023, max compression
```

## Comparing `drf-passage-identity-0.0.1.tar` & `drf-passage-identity-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 10:35:20.128412 drf-passage-identity-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-28 10:32:49.000000 drf-passage-identity-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       37 2023-06-28 10:33:26.000000 drf-passage-identity-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      926 2023-06-28 10:35:20.128412 drf-passage-identity-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-06-28 10:23:41.000000 drf-passage-identity-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-28 10:35:20.073573 drf-passage-identity-0.0.1/drf_passage_identity.egg-info/
--rw-rw-rw-   0        0        0      926 2023-06-28 10:35:19.000000 drf-passage-identity-0.0.1/drf_passage_identity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2023-06-28 10:35:20.000000 drf-passage-identity-0.0.1/drf_passage_identity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 10:35:19.000000 drf-passage-identity-0.0.1/drf_passage_identity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-28 10:35:19.000000 drf-passage-identity-0.0.1/drf_passage_identity.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-28 10:35:20.113704 drf-passage-identity-0.0.1/passage_auth/
--rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.1/passage_auth/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-28 07:46:00.000000 drf-passage-identity-0.0.1/passage_auth/admin.py
--rw-rw-rw-   0        0        0      161 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.1/passage_auth/apps.py
--rw-rw-rw-   0        0        0     1191 2023-06-28 07:32:27.000000 drf-passage-identity-0.0.1/passage_auth/authentication.py
--rw-rw-rw-   0        0        0     1317 2023-06-28 07:30:18.000000 drf-passage-identity-0.0.1/passage_auth/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:35:20.127433 drf-passage-identity-0.0.1/passage_auth/migrations/
--rw-rw-rw-   0        0        0     2069 2023-06-28 07:40:16.000000 drf-passage-identity-0.0.1/passage_auth/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.1/passage_auth/migrations/__init__.py
--rw-rw-rw-   0        0        0      881 2023-06-28 07:30:03.000000 drf-passage-identity-0.0.1/passage_auth/models.py
--rw-rw-rw-   0        0        0      366 2023-06-28 07:56:48.000000 drf-passage-identity-0.0.1/passage_auth/setup.py
--rw-rw-rw-   0        0        0       63 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.1/passage_auth/tests.py
--rw-rw-rw-   0        0        0       66 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.1/passage_auth/views.py
--rw-rw-rw-   0        0        0      897 2023-06-28 10:35:20.142140 drf-passage-identity-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-28 10:34:13.000000 drf-passage-identity-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.411280 drf-passage-identity-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-28 10:32:49.000000 drf-passage-identity-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-06-28 10:33:26.000000 drf-passage-identity-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      926 2023-06-29 12:44:48.411391 drf-passage-identity-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-06-28 10:23:41.000000 drf-passage-identity-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.396586 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/
+-rw-rw-rw-   0        0        0      926 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.408453 drf-passage-identity-0.0.2/passage_auth/
+-rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-28 07:46:00.000000 drf-passage-identity-0.0.2/passage_auth/admin.py
+-rw-rw-rw-   0        0        0      161 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/apps.py
+-rw-rw-rw-   0        0        0     1376 2023-06-29 12:29:36.000000 drf-passage-identity-0.0.2/passage_auth/authentication.py
+-rw-rw-rw-   0        0        0     1317 2023-06-28 07:30:18.000000 drf-passage-identity-0.0.2/passage_auth/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.410217 drf-passage-identity-0.0.2/passage_auth/migrations/
+-rw-rw-rw-   0        0        0     2069 2023-06-28 07:40:16.000000 drf-passage-identity-0.0.2/passage_auth/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-06-28 07:30:03.000000 drf-passage-identity-0.0.2/passage_auth/models.py
+-rw-rw-rw-   0        0        0      366 2023-06-28 07:56:48.000000 drf-passage-identity-0.0.2/passage_auth/setup.py
+-rw-rw-rw-   0        0        0       63 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/tests.py
+-rw-rw-rw-   0        0        0      141 2023-06-29 12:33:29.000000 drf-passage-identity-0.0.2/passage_auth/urls.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 12:29:54.000000 drf-passage-identity-0.0.2/passage_auth/views.py
+-rw-rw-rw-   0        0        0      959 2023-06-29 12:44:48.412484 drf-passage-identity-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-28 10:34:13.000000 drf-passage-identity-0.0.2/setup.py
```

### Comparing `drf-passage-identity-0.0.1/LICENSE` & `drf-passage-identity-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.1/PKG-INFO` & `drf-passage-identity-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-passage-identity
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to authenticate users passwordless using Passage.
 Home-page: https://github.com/kothawleprem/drf-passage-identity
 Author: Prem
 Author-email: kothawleprem@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `drf-passage-identity-0.0.1/drf_passage_identity.egg-info/PKG-INFO` & `drf-passage-identity-0.0.2/drf_passage_identity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-passage-identity
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to authenticate users passwordless using Passage.
 Home-page: https://github.com/kothawleprem/drf-passage-identity
 Author: Prem
 Author-email: kothawleprem@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `drf-passage-identity-0.0.1/drf_passage_identity.egg-info/SOURCES.txt` & `drf-passage-identity-0.0.2/drf_passage_identity.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 drf_passage_identity.egg-info/PKG-INFO
 drf_passage_identity.egg-info/SOURCES.txt
 drf_passage_identity.egg-info/dependency_links.txt
+drf_passage_identity.egg-info/requires.txt
 drf_passage_identity.egg-info/top_level.txt
 passage_auth/__init__.py
 passage_auth/admin.py
 passage_auth/apps.py
 passage_auth/authentication.py
 passage_auth/manager.py
 passage_auth/models.py
 passage_auth/setup.py
 passage_auth/tests.py
+passage_auth/urls.py
 passage_auth/views.py
 passage_auth/migrations/0001_initial.py
 passage_auth/migrations/__init__.py
```

### Comparing `drf-passage-identity-0.0.1/passage_auth/authentication.py` & `drf-passage-identity-0.0.2/passage_auth/authentication.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.conf import settings
 from rest_framework import authentication
+from rest_framework.exceptions import AuthenticationFailed
 
-from passageidentity import Passage
+from passageidentity import Passage, PassageError
 
 from .models import PassageUser
 
 PASSAGE_APP_ID = settings.PASSAGE_APP_ID
 PASSAGE_API_KEY = settings.PASSAGE_API_KEY
 PASSAGE_AUTH_STRATEGY = settings.PASSAGE_AUTH_STRATEGY
 psg = Passage(PASSAGE_APP_ID, PASSAGE_API_KEY, auth_strategy=PASSAGE_AUTH_STRATEGY)
@@ -14,19 +15,22 @@
 class TokenAuthentication(authentication.BaseAuthentication):
     def authenticate(self, request):
         # Get the access token from the request headers
         auth_header = request.headers.get('Authorization')
         if not auth_header:
             return None
 
-        # Extract the token from the header
-        psg_user_id = psg.authenticateRequest(request)
-        psg_user = psg.getUser(psg_user_id)
+        # Get User Id from Passage Authenticate Request
+        try:
+            psg_user_id = psg.authenticateRequest(request)
+        except PassageError as e:
+            raise AuthenticationFailed(e.message)
 
-        # Check if the token exists in the AccessToken model
+        # Check if the user exists in the database.
         try:
-            user = PassageUser.objects.get(id=psg_user.id)
+            user = PassageUser.objects.get(id=psg_user_id)
         except ObjectDoesNotExist:
-            user = PassageUser.objects.create_user(id=psg_user.id, email=psg_user.email)
+            psg_user = psg.getUser(psg_user_id)
+            user = PassageUser.objects.create_user(id=psg_user_id, email=psg_user.email)
 
         # Return the authenticated user
         return (user, None)
```

### Comparing `drf-passage-identity-0.0.1/passage_auth/manager.py` & `drf-passage-identity-0.0.2/passage_auth/manager.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.1/passage_auth/migrations/0001_initial.py` & `drf-passage-identity-0.0.2/passage_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.1/passage_auth/models.py` & `drf-passage-identity-0.0.2/passage_auth/models.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.1/setup.cfg` & `drf-passage-identity-0.0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d70 6173 7361 6765 2d69   = drf-passage-i
 00000020: 6465 6e74 6974 790d 0a76 6572 7369 6f6e  dentity..version
-00000030: 203d 2030 2e30 2e31 0d0a 6465 7363 7269   = 0.0.1..descri
+00000030: 203d 2030 2e30 2e32 0d0a 6465 7363 7269   = 0.0.2..descri
 00000040: 7074 696f 6e20 3d20 4120 446a 616e 676f  ption = A Django
 00000050: 2061 7070 2074 6f20 6175 7468 656e 7469   app to authenti
 00000060: 6361 7465 2075 7365 7273 2070 6173 7377  cate users passw
 00000070: 6f72 646c 6573 7320 7573 696e 6720 5061  ordless using Pa
 00000080: 7373 6167 652e 0d0a 6c6f 6e67 5f64 6573  ssage...long_des
 00000090: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
 000000a0: 2052 4541 444d 452e 7273 740d 0a6c 6f6e   README.rst..lon
@@ -47,11 +47,14 @@
 000002e0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
 000002f0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
 00000300: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
 00000310: 4d6f 6475 6c65 730d 0a0d 0a5b 6f70 7469  Modules....[opti
 00000320: 6f6e 735d 0d0a 696e 636c 7564 655f 7061  ons]..include_pa
 00000330: 636b 6167 655f 6461 7461 203d 2074 7275  ckage_data = tru
 00000340: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
-00000350: 6e64 3a0d 0a0d 0a5b 6567 675f 696e 666f  nd:....[egg_info
-00000360: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000370: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000380: 0a                                       .
+00000350: 6e64 3a0d 0a69 6e73 7461 6c6c 5f72 6571  nd:..install_req
+00000360: 7569 7265 7320 3d20 0d0a 0964 6a61 6e67  uires = ...djang
+00000370: 6f72 6573 7466 7261 6d65 776f 726b 0d0a  orestframework..
+00000380: 0970 6173 7361 6765 2d69 6465 6e74 6974  .passage-identit
+00000390: 790d 0a0d 0a5b 6567 675f 696e 666f 5d0d  y....[egg_info].
+000003a0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000003b0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

