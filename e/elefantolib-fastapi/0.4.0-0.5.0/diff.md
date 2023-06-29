# Comparing `tmp/elefantolib_fastapi-0.4.0.tar.gz` & `tmp/elefantolib_fastapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.4.0.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.5.0.tar", max compression
```

## Comparing `elefantolib_fastapi-0.4.0.tar` & `elefantolib_fastapi-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0      878 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/README.md
--rw-r--r--   0        0        0       22 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0     1018 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/connection.py
--rw-r--r--   0        0        0      736 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/depends.py
--rw-r--r--   0        0        0      934 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/exceptions.py
--rw-r--r--   0        0        0      209 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      721 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      890 2023-05-27 13:33:00.147497 elefantolib_fastapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.4.0/setup.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0     1018 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/connection.py
+-rw-r--r--   0        0        0      878 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/depends.py
+-rw-r--r--   0        0        0      934 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/exceptions.py
+-rw-r--r--   0        0        0      604 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/middleware.py
+-rw-r--r--   0        0        0     2039 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/pagination.py
+-rw-r--r--   0        0        0      209 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      721 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      307 2023-06-29 14:55:22.735705 elefantolib_fastapi-0.5.0/elefantolib_fastapi/schemas.py
+-rw-r--r--   0        0        0      913 2023-06-29 14:55:41.595948 elefantolib_fastapi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.5.0/setup.py
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.5.0/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.4.0/README.md` & `elefantolib_fastapi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.4.0/elefantolib_fastapi/connection.py` & `elefantolib_fastapi-0.5.0/elefantolib_fastapi/connection.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.4.0/elefantolib_fastapi/depends.py` & `elefantolib_fastapi-0.5.0/elefantolib_fastapi/depends.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from typing import Annotated, NamedTuple
 
 from elefantolib_fastapi import exceptions
 from elefantolib_fastapi.requests import Request
 
-from fastapi import HTTPException, Header, status
+from fastapi import HTTPException, Header, Query, status
+
+from pydantic import BaseModel
+
+
+class PaginatedParams(BaseModel):
+    page: int = Query(1, ge=1)
+    page_size: int = Query(8, gt=0)
 
 
 class CommonHeaders(NamedTuple):
     auth_token: Annotated[str, Header(alias='Authorization')]
     correlation_id: Annotated[str, Header(alias='X-Correlation-Id')]
     locale: Annotated[str, Header(alias='Accept-Language')]
```

### Comparing `elefantolib_fastapi-0.4.0/elefantolib_fastapi/exceptions.py` & `elefantolib_fastapi-0.5.0/elefantolib_fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.4.0/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.5.0/elefantolib_fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.4.0/pyproject.toml` & `elefantolib_fastapi-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = "^0.95.2"
-redis = "^4.5.5"
+fastapi = "^0.98.0"
+redis = "^4.6.0"
 elefantolib = "^0.12.1"
+sqlalchemy = "^2.0.17"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-flake8 = "^1.1.1"
```

### Comparing `elefantolib_fastapi-0.4.0/setup.py` & `elefantolib_fastapi-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 ['elefantolib_fastapi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['elefantolib>=0.12.1,<0.13.0',
- 'fastapi>=0.95.2,<0.96.0',
- 'redis>=4.5.5,<5.0.0']
+ 'fastapi>=0.98.0,<0.99.0',
+ 'redis>=4.6.0,<5.0.0',
+ 'sqlalchemy>=2.0.17,<3.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-fastapi',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
     'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import Request\nfrom elefantolib_fastapi.routes import APIRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = APIRoute\n\n\n@app.get(\'/\')\ndef index(request: Request):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
     'author': 'gglassota',
     'author_email': 'gglassota2@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `elefantolib_fastapi-0.4.0/PKG-INFO` & `elefantolib_fastapi-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: elefantolib-fastapi
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: gglassota
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: elefantolib (>=0.12.1,<0.13.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
-Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: fastapi (>=0.98.0,<0.99.0)
+Requires-Dist: redis (>=4.6.0,<5.0.0)
+Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Elefantolib for FastAPI
 
 > **_NOTE:_**  Only for this library developers. After clone this repository you should run command:
 >
```

