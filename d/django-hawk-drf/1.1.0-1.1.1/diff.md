# Comparing `tmp/django_hawk_drf-1.1.0.tar.gz` & `tmp/django_hawk_drf-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hawk_drf-1.1.0.tar", max compression
+gzip compressed data, was "django_hawk_drf-1.1.1.tar", max compression
```

## Comparing `django_hawk_drf-1.1.0.tar` & `django_hawk_drf-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1091 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/LICENSE
--rw-r--r--   0        0        0     1923 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/README.md
--rw-r--r--   0        0        0        0 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/__init__.py
--rw-r--r--   0        0        0     1432 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/authentication.py
--rw-r--r--   0        0        0      456 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/middleware.py
--rw-r--r--   0        0        0        0 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/py.typed
--rw-r--r--   0        0        0        0 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/tests/__init__.py
--rw-r--r--   0        0        0     1038 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/tests/settings.py
--rw-r--r--   0        0        0     4976 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/tests/test_views.py
--rw-r--r--   0        0        0     1320 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/tests/test_views_drf.py
--rw-r--r--   0        0        0      226 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/tests/urls.py
--rw-r--r--   0        0        0      322 2022-11-21 10:17:07.126758 django_hawk_drf-1.1.0/django_hawk_drf/tests/views.py
--rw-r--r--   0        0        0      865 2022-11-21 10:49:31.850578 django_hawk_drf-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 django_hawk_drf-1.1.0/setup.py
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 django_hawk_drf-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-16 13:43:22.139548 django_hawk_drf-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1923 2022-11-17 14:01:10.415215 django_hawk_drf-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 13:43:22.140010 django_hawk_drf-1.1.1/django_hawk_drf/__init__.py
+-rw-r--r--   0        0        0     1432 2022-11-17 14:14:29.583724 django_hawk_drf-1.1.1/django_hawk_drf/authentication.py
+-rw-r--r--   0        0        0      456 2022-11-16 17:20:52.552597 django_hawk_drf-1.1.1/django_hawk_drf/middleware.py
+-rw-r--r--   0        0        0        0 2022-11-16 13:43:22.140195 django_hawk_drf-1.1.1/django_hawk_drf/py.typed
+-rw-r--r--   0        0        0        0 2022-11-16 13:43:22.140314 django_hawk_drf-1.1.1/django_hawk_drf/tests/__init__.py
+-rw-r--r--   0        0        0     1038 2022-11-17 13:24:37.636493 django_hawk_drf-1.1.1/django_hawk_drf/tests/settings.py
+-rw-r--r--   0        0        0     4976 2022-11-17 13:25:17.553947 django_hawk_drf-1.1.1/django_hawk_drf/tests/test_views.py
+-rw-r--r--   0        0        0     2003 2023-05-22 11:11:44.028060 django_hawk_drf-1.1.1/django_hawk_drf/tests/test_views_drf.py
+-rw-r--r--   0        0        0      226 2022-11-16 13:43:22.140763 django_hawk_drf-1.1.1/django_hawk_drf/tests/urls.py
+-rw-r--r--   0        0        0      322 2023-05-22 11:16:39.851832 django_hawk_drf-1.1.1/django_hawk_drf/tests/views.py
+-rw-r--r--   0        0        0      865 2023-06-29 10:54:09.643176 django_hawk_drf-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 django_hawk_drf-1.1.1/PKG-INFO
```

### Comparing `django_hawk_drf-1.1.0/LICENSE` & `django_hawk_drf-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hawk_drf-1.1.0/README.md` & `django_hawk_drf-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_hawk_drf-1.1.0/django_hawk_drf/authentication.py` & `django_hawk_drf-1.1.1/django_hawk_drf/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hawk_drf-1.1.0/django_hawk_drf/tests/settings.py` & `django_hawk_drf-1.1.1/django_hawk_drf/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_hawk_drf-1.1.0/django_hawk_drf/tests/test_views.py` & `django_hawk_drf-1.1.1/django_hawk_drf/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_hawk_drf-1.1.0/pyproject.toml` & `django_hawk_drf-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "django-hawk-drf"
-version = "1.1.0"
+version = "1.1.1"
 description = "Authenticate Django Rest Framework Views with django-hawk"
 authors = [
     "Cameron Lamb <live.services@digital.trade.gov.uk>"
 ]
 license = "MIT"
 readme = "README.md"
 keywords = [
```

### Comparing `django_hawk_drf-1.1.0/setup.py` & `django_hawk_drf-1.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,96 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-hawk-drf
+Version: 1.1.1
+Summary: Authenticate Django Rest Framework Views with django-hawk
+Home-page: https://github.com/uktrade/django-hawk-drf/
+License: MIT
+Keywords: django
+Author: Cameron Lamb
+Author-email: live.services@digital.trade.gov.uk
+Requires-Python: >=3.6.2,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=2.2,<4.2)
+Requires-Dist: django-hawk (>=1.1.0,<2.0.0)
+Requires-Dist: djangorestframework (>=3.10.3,<4.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['django_hawk_drf', 'django_hawk_drf.tests']
+# Django Hawk DRF
 
-package_data = \
-{'': ['*']}
+This package provides [Django Rest Framework](https://github.com/encode/django-rest-framework/) helper classes for use with [Django Hawk](https://github.com/uktrade/django-hawk).
 
-install_requires = \
-['Django>=2.2,<4.2',
- 'django-hawk>=1.1.0,<2.0.0',
- 'djangorestframework>=3.10.3,<4.0']
-
-setup_kwargs = {
-    'name': 'django-hawk-drf',
-    'version': '1.1.0',
-    'description': 'Authenticate Django Rest Framework Views with django-hawk',
-    'long_description': '# Django Hawk DRF\n\nThis package provides [Django Rest Framework](https://github.com/encode/django-rest-framework/) helper classes for use with [Django Hawk](https://github.com/uktrade/django-hawk).\n\n## Installation\n\nRead the [Django Hawk installation](https://github.com/uktrade/django-hawk#installation) documentation.\n\n## Example usage\n\nRead the [Django Hawk example usage](https://github.com/uktrade/django-hawk#example-usage) documentation.\n\nAdd the `HawkResponseMiddleware` to the `MIDDLEWARE` setting in your project like so:\n\n```\nMIDDLEWARE = [\n    ...\n    "django_hawk.middleware.HawkResponseMiddleware",\n    "django_hawk_drf.middleware.HawkResponseMiddleware",\n    ...\n]\n```\n\nTo check the you can use the `django_hawk.authentication.HawkAuthentication` authentication class.\n\n```python\nfrom rest_framework.response import Response\nfrom rest_framework.viewsets import ViewSet\n\nfrom django_hawk_drf.authentication import HawkAuthentication\n\n\nclass ExampleViewSet(ViewSet):\n    authentication_classes = (HawkAuthentication,)\n    permission_classes = ()\n\n    def list(self, request):\n        return Response([])\n```\n\n## Testing\n\nTests belong in the `/django_hawk_drf/tests/` directory. You can run the tests by installing the requirements like so:\n\n\n```\nmake setup\n```\n\nNow you can run the tests using the following command:\n\n```\npoetry run python manage.py test\n```\n\n### Tox tests\n\nWe use [tox](https://pypi.org/project/tox/) to test compatibility across different Django versions.\n\nTo run these tests with tox, just run the following:\n\n```\nmake tox\n```\n\n## Pushing to PyPI\n\n- [PyPI Package](https://pypi.org/project/django-hawk-drf/)\n- [Test PyPI Package](https://test.pypi.org/project/django-hawk-drf/)\n\nRunning `make build-package` will build the package into the `dist/` directory\nRunning `make push-pypi-test` will push the built package to Test PyPI\nRunning `make push-pypi` will push the built package to PyPI\n',
-    'author': 'Cameron Lamb',
-    'author_email': 'live.services@digital.trade.gov.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/uktrade/django-hawk-drf/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0',
-}
+## Installation
 
+Read the [Django Hawk installation](https://github.com/uktrade/django-hawk#installation) documentation.
+
+## Example usage
+
+Read the [Django Hawk example usage](https://github.com/uktrade/django-hawk#example-usage) documentation.
+
+Add the `HawkResponseMiddleware` to the `MIDDLEWARE` setting in your project like so:
+
+```
+MIDDLEWARE = [
+    ...
+    "django_hawk.middleware.HawkResponseMiddleware",
+    "django_hawk_drf.middleware.HawkResponseMiddleware",
+    ...
+]
+```
+
+To check the you can use the `django_hawk.authentication.HawkAuthentication` authentication class.
+
+```python
+from rest_framework.response import Response
+from rest_framework.viewsets import ViewSet
+
+from django_hawk_drf.authentication import HawkAuthentication
+
+
+class ExampleViewSet(ViewSet):
+    authentication_classes = (HawkAuthentication,)
+    permission_classes = ()
+
+    def list(self, request):
+        return Response([])
+```
+
+## Testing
+
+Tests belong in the `/django_hawk_drf/tests/` directory. You can run the tests by installing the requirements like so:
+
+
+```
+make setup
+```
+
+Now you can run the tests using the following command:
+
+```
+poetry run python manage.py test
+```
+
+### Tox tests
+
+We use [tox](https://pypi.org/project/tox/) to test compatibility across different Django versions.
+
+To run these tests with tox, just run the following:
+
+```
+make tox
+```
+
+## Pushing to PyPI
+
+- [PyPI Package](https://pypi.org/project/django-hawk-drf/)
+- [Test PyPI Package](https://test.pypi.org/project/django-hawk-drf/)
+
+Running `make build-package` will build the package into the `dist/` directory
+Running `make push-pypi-test` will push the built package to Test PyPI
+Running `make push-pypi` will push the built package to PyPI
 
-setup(**setup_kwargs)
```

