# Comparing `tmp/django-ucam-apigatewayauth-0.0.2.tar.gz` & `tmp/django-ucam-apigatewayauth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ucam-apigatewayauth-0.0.2.tar", last modified: Fri Mar 25 11:16:37 2022, max compression
+gzip compressed data, was "django-ucam-apigatewayauth-0.0.3.tar", last modified: Thu Jun 29 11:06:50 2023, max compression
```

## Comparing `django-ucam-apigatewayauth-0.0.2.tar` & `django-ucam-apigatewayauth-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 11:16:37.690643 django-ucam-apigatewayauth-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     8038 2022-03-25 11:16:37.690643 django-ucam-apigatewayauth-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7305 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 11:16:37.682643 django-ucam-apigatewayauth-0.0.2/apigatewayauth/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/api_gateway_auth.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     6687 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/permissions_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 11:16:37.686643 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 11:16:37.686643 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 11:16:37.690643 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/mock_ibis.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/models.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/permissions_spec.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/test_model_migrations.py
--rw-rw-rw-   0 root         (0) root         (0)     5106 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/test_apigateway_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    17052 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/test_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3382 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/test_permissions_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 11:16:37.690643 django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8038 2022-03-25 11:16:37.000000 django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      936 2022-03-25 11:16:37.000000 django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 11:16:37.000000 django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       97 2022-03-25 11:16:37.000000 django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-03-25 11:16:37.000000 django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-25 11:16:37.690643 django-ucam-apigatewayauth-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1366 2022-03-25 09:43:20.000000 django-ucam-apigatewayauth-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:06:50.005085 django-ucam-apigatewayauth-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     8018 2023-06-29 11:06:50.005085 django-ucam-apigatewayauth-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7305 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:06:49.989084 django-ucam-apigatewayauth-0.0.3/apigatewayauth/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-29 11:06:47.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/api_gateway_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6687 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/permissions_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:06:49.993084 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 11:06:47.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:06:50.001085 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:06:50.001085 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      537 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 11:06:47.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/mock_ibis.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/permissions_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/test_model_migrations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5106 2023-06-29 11:06:47.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/test_apigateway_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    17052 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/test_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2023-06-29 10:31:04.000000 django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/test_permissions_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:06:50.005085 django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8018 2023-06-29 11:06:49.000000 django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-29 11:06:49.000000 django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 11:06:49.000000 django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-29 11:06:49.000000 django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 11:06:49.000000 django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 11:06:50.005085 django-ucam-apigatewayauth-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-29 11:06:47.000000 django-ucam-apigatewayauth-0.0.3/setup.py
```

### Comparing `django-ucam-apigatewayauth-0.0.2/PKG-INFO` & `django-ucam-apigatewayauth-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-ucam-apigatewayauth
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django module allow auth based on the headers passed from the API Gateway
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/django/api-gateway-auth
 Author: DevOps Division, University Information Services, University of Cambridge
 Author-email: devops@uis.cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha 
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -203,9 +202,7 @@
   def get_queryset(self):
     """
     Ensure that the queryset we use is limited based on the conditions we've defined on our model.
 
     """
 
     return IsResourceOwningPrincipal.get_queryset_for_principal(Example, self.request)
-
-
```

### Comparing `django-ucam-apigatewayauth-0.0.2/README.md` & `django-ucam-apigatewayauth-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/api_gateway_auth.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/api_gateway_auth.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/permissions.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/permissions.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/permissions_spec.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/permissions_spec.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/migrations/0001_initial.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/models.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/models.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/permissions_spec.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/permissions_spec.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/mocks/test_model_migrations.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/mocks/test_model_migrations.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/test_apigateway_auth.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/test_apigateway_auth.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/test_permissions.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/apigatewayauth/tests/test_permissions_spec.py` & `django-ucam-apigatewayauth-0.0.3/apigatewayauth/tests/test_permissions_spec.py`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/PKG-INFO` & `django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-ucam-apigatewayauth
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django module allow auth based on the headers passed from the API Gateway
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/django/api-gateway-auth
 Author: DevOps Division, University Information Services, University of Cambridge
 Author-email: devops@uis.cam.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha 
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -203,9 +202,7 @@
   def get_queryset(self):
     """
     Ensure that the queryset we use is limited based on the conditions we've defined on our model.
 
     """
 
     return IsResourceOwningPrincipal.get_queryset_for_principal(Example, self.request)
-
-
```

### Comparing `django-ucam-apigatewayauth-0.0.2/django_ucam_apigatewayauth.egg-info/SOURCES.txt` & `django-ucam-apigatewayauth-0.0.3/django_ucam_apigatewayauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ucam-apigatewayauth-0.0.2/setup.py` & `django-ucam-apigatewayauth-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='django-ucam-apigatewayauth',
     description='A Django module allow auth based on the headers passed from the API Gateway',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitlab.developers.cam.ac.uk/uis/devops/django/api-gateway-auth',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author='DevOps Division, University Information Services, University of Cambridge',
     author_email='devops@uis.cam.ac.uk',
     packages=find_packages(),
     include_package_data=True,
     install_requires=load_requirements('requirements.txt'),
     classifiers=[
```

