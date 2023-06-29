# Comparing `tmp/ms_general_utils-1.4.3.tar.gz` & `tmp/ms_general_utils-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-1.4.3.tar", last modified: Tue Jun 20 10:05:50 2023, max compression
+gzip compressed data, was "ms_general_utils-1.4.4.tar", last modified: Thu Jun 29 09:36:03 2023, max compression
```

## Comparing `ms_general_utils-1.4.3.tar` & `ms_general_utils-1.4.4.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:05:50.669259 ms_general_utils-1.4.3/
--rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2023-06-20 10:05:50.666262 ms_general_utils-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-06-20 09:54:06.000000 ms_general_utils-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 10:05:50.589721 ms_general_utils-1.4.3/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      354 2023-06-20 10:05:50.000000 ms_general_utils-1.4.3/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-06-20 10:05:50.000000 ms_general_utils-1.4.3/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:05:50.000000 ms_general_utils-1.4.3/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 10:05:50.000000 ms_general_utils-1.4.3/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 10:05:50.662264 ms_general_utils-1.4.3/ms_utils/
--rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.4.3/ms_utils/__init__.py
--rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.4.3/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.4.3/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.4.3/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.4.3/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.4.3/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.4.3/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.4.3/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      622 2023-05-19 16:18:44.000000 ms_general_utils-1.4.3/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     4721 2023-06-20 10:04:55.000000 ms_general_utils-1.4.3/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:05:50.670259 ms_general_utils-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-06-20 10:05:20.000000 ms_general_utils-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.835388 ms_general_utils-1.4.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-06-29 09:36:03.834388 ms_general_utils-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.820106 ms_general_utils-1.4.4/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.830107 ms_general_utils-1.4.4/ms_utils/
+-rw-rw-rw-   0        0        0      567 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     1073 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      568 2023-06-29 08:59:58.000000 ms_general_utils-1.4.4/ms_utils/deploy.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.832388 ms_general_utils-1.4.4/ms_utils/devops/
+-rw-rw-rw-   0        0        0      577 2023-06-29 08:11:09.000000 ms_general_utils-1.4.4/ms_utils/devops/Dockerfile
+drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.833388 ms_general_utils-1.4.4/ms_utils/devops/deploy/
+-rw-rw-rw-   0        0        0      196 2023-06-29 08:12:58.000000 ms_general_utils-1.4.4/ms_utils/devops/deploy/script.sh
+-rw-rw-rw-   0        0        0      288 2023-06-29 08:11:09.000000 ms_general_utils-1.4.4/ms_utils/devops/docker-compose.yml
+-rw-rw-rw-   0        0        0       48 2023-06-29 08:12:49.000000 ms_general_utils-1.4.4/ms_utils/devops/dockerfile.env
+-rw-rw-rw-   0        0        0      727 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0     2570 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      734 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1527 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      357 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0      622 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     4721 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:36:03.835388 ms_general_utils-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-06-29 09:35:31.000000 ms_general_utils-1.4.4/setup.py
```

### Comparing `ms_general_utils-1.4.3/LICENSE.txt` & `ms_general_utils-1.4.4/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2021 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2021 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ms_general_utils-1.4.3/ms_utils/__init__.py` & `ms_general_utils-1.4.4/ms_utils/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""
-Init imports
-"""
-from .binary_uuid import BinaryUUID
-from .func_date import convert_date_to_timestamp, get_timestamp_now, convert_timestamp_to_date
-from .prepare_json_response import prepare_json_response
-from .generic_pagination import PaginationSchema
-from .validation_utils import validate_generic_form
-from .abstract_model import BaseModel
-from .model_utils import JsonEncodeDict, generic_get_serialize_data, TimestampField
-from .view_utils import ViewGeneralMethods
-from .generic_crud_class import register_api, GenericItemCrud, GenericGroupCrud
+"""
+Init imports
+"""
+from .binary_uuid import BinaryUUID
+from .func_date import convert_date_to_timestamp, get_timestamp_now, convert_timestamp_to_date
+from .prepare_json_response import prepare_json_response
+from .generic_pagination import PaginationSchema
+from .validation_utils import validate_generic_form
+from .abstract_model import BaseModel
+from .model_utils import JsonEncodeDict, generic_get_serialize_data, TimestampField
+from .view_utils import ViewGeneralMethods
+from .generic_crud_class import register_api, GenericItemCrud, GenericGroupCrud
```

### Comparing `ms_general_utils-1.4.3/ms_utils/binary_uuid.py` & `ms_general_utils-1.4.4/ms_utils/binary_uuid.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-Binary UUID Class
-"""
-from abc import ABC
-from uuid import UUID
-from sqlalchemy.dialects.mysql import BINARY
-from sqlalchemy.types import TypeDecorator
-
-
-class BinaryUUID(TypeDecorator, ABC):
-    """Optimize UUID keys. Store as 16 bit binary, retrieve as uuid.
-    inspired by:
-        https://mysqlserverteam.com/storing-uuid-values-in-mysql-tables/
-    """
-
-    impl = BINARY(16)
-    cache_ok = True
-
-    def process_bind_param(self, value, dialect):
-        """
-        Process create data
-        """
-        try:
-            return value.bytes
-        except AttributeError:
-            try:
-                return UUID(value).bytes
-            except TypeError:
-                # for some reason we ended up with the byte string
-                # ¯\_(ツ)_/¯
-                # I'm not sure why you would do that,
-                # but here you go anyway.
-                return value
-
-    def process_result_value(self, value, dialect):
-        """
-        Process result data
-        """
-        return UUID(bytes=value)
+"""
+Binary UUID Class
+"""
+from abc import ABC
+from uuid import UUID
+from sqlalchemy.dialects.mysql import BINARY
+from sqlalchemy.types import TypeDecorator
+
+
+class BinaryUUID(TypeDecorator, ABC):
+    """Optimize UUID keys. Store as 16 bit binary, retrieve as uuid.
+    inspired by:
+        https://mysqlserverteam.com/storing-uuid-values-in-mysql-tables/
+    """
+
+    impl = BINARY(16)
+    cache_ok = True
+
+    def process_bind_param(self, value, dialect):
+        """
+        Process create data
+        """
+        try:
+            return value.bytes
+        except AttributeError:
+            try:
+                return UUID(value).bytes
+            except TypeError:
+                # for some reason we ended up with the byte string
+                # ¯\_(ツ)_/¯
+                # I'm not sure why you would do that,
+                # but here you go anyway.
+                return value
+
+    def process_result_value(self, value, dialect):
+        """
+        Process result data
+        """
+        return UUID(bytes=value)
```

### Comparing `ms_general_utils-1.4.3/ms_utils/func_date.py` & `ms_general_utils-1.4.4/ms_utils/func_date.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""
-Function date methods
-"""
-from datetime import datetime
-import pytz as pytz
-
-
-def convert_date_to_timestamp(date, format_datetime='%Y-%m-%d %H:%M:%S'):
-    """
-    Convert date to timestamp
-    """
-    if isinstance(date, str):
-        date = datetime.strptime(date, format_datetime)
-
-    if not isinstance(date, datetime):
-        raise ValueError('Incorrect data type')
-
-    return int(date.astimezone(pytz.UTC).timestamp())
-
-
-def convert_timestamp_to_date(timestamp):
-    """
-    Convert timestamp to date
-    """
-    return datetime.fromtimestamp(timestamp)
-
-
-def get_timestamp_now():
-    """
-    Get timestamp now
-    """
-    return int(datetime.now().astimezone(pytz.utc).timestamp())
+"""
+Function date methods
+"""
+from datetime import datetime
+import pytz as pytz
+
+
+def convert_date_to_timestamp(date, format_datetime='%Y-%m-%d %H:%M:%S'):
+    """
+    Convert date to timestamp
+    """
+    if isinstance(date, str):
+        date = datetime.strptime(date, format_datetime)
+
+    if not isinstance(date, datetime):
+        raise ValueError('Incorrect data type')
+
+    return int(date.astimezone(pytz.UTC).timestamp())
+
+
+def convert_timestamp_to_date(timestamp):
+    """
+    Convert timestamp to date
+    """
+    return datetime.fromtimestamp(timestamp)
+
+
+def get_timestamp_now():
+    """
+    Get timestamp now
+    """
+    return int(datetime.now().astimezone(pytz.utc).timestamp())
```

### Comparing `ms_general_utils-1.4.3/ms_utils/generic_crud_class.py` & `ms_general_utils-1.4.4/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.3/ms_utils/generic_pagination.py` & `ms_general_utils-1.4.4/ms_utils/generic_pagination.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""
-Pagination Generic Class
-"""
-from flask_marshmallow import Marshmallow
-
-
-class PaginationSchema:
-    """
-    Pagination Class
-    """
-    schema_object = None
-    ma = Marshmallow()
-
-    def __init__(self, ma, app, schema_object):
-        self.schema_object = schema_object
-        self.ma = ma
-        self.ma.init_app(app)
-        self.pagination_sub_class = self.PaginationSchemaSubClass()
-
-    class PaginationSchemaSubClass(ma.SQLAlchemyAutoSchema):
-        """
-        Pagination Schema Data
-        """
-        class Meta:
-            """
-            Meta Class
-            """
-            fields = ('has_prev', 'has_next', 'next_num', 'page', 'pages', 'per_page', 'prev_num', 'total', 'items')
+"""
+Pagination Generic Class
+"""
+from flask_marshmallow import Marshmallow
+
+
+class PaginationSchema:
+    """
+    Pagination Class
+    """
+    schema_object = None
+    ma = Marshmallow()
+
+    def __init__(self, ma, app, schema_object):
+        self.schema_object = schema_object
+        self.ma = ma
+        self.ma.init_app(app)
+        self.pagination_sub_class = self.PaginationSchemaSubClass()
+
+    class PaginationSchemaSubClass(ma.SQLAlchemyAutoSchema):
+        """
+        Pagination Schema Data
+        """
+        class Meta:
+            """
+            Meta Class
+            """
+            fields = ('has_prev', 'has_next', 'next_num', 'page', 'pages', 'per_page', 'prev_num', 'total', 'items')
```

### Comparing `ms_general_utils-1.4.3/ms_utils/model_utils.py` & `ms_general_utils-1.4.4/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.3/ms_utils/validation_utils.py` & `ms_general_utils-1.4.4/ms_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.3/ms_utils/view_utils.py` & `ms_general_utils-1.4.4/ms_utils/view_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.3/setup.py` & `ms_general_utils-1.4.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-"""
-Setup configuration file
-"""
-from setuptools import setup, find_packages
-
-setup(
-    name='ms_general_utils',
-    packages=find_packages(),
-    include_package_data=True,
-    version='1.4.3',
-    description='General functions for the implementation of microservices.',
-    authors=[
-        {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
-        {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
-    ],
-    license="GPLv3",
-    url="https://github.com/rgramos/ms-utils.git",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
-    ],
-)
+"""
+Setup configuration file
+"""
+from setuptools import setup, find_packages
+
+setup(
+    name='ms_general_utils',
+    packages=find_packages(),
+    package_data={'ms_utils': ['devops/*', 'devops/deploy/*']},
+    include_package_data=True,
+    version='1.4.4',
+    description='General functions for the implementation of microservices.',
+    authors=[
+        {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
+        {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
+    ],
+    license="GPLv3",
+    url="https://github.com/rgramos/ms-utils.git",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
+    ],
+    entry_points={
+        "flask.commands": [
+            'generate-deploy = ms_utils.deploy:generate'
+        ]
+    }
+)
```

