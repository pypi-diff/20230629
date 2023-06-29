# Comparing `tmp/oapi-1.59.4.tar.gz` & `tmp/oapi-1.59.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oapi-1.59.4.tar", last modified: Wed May 17 04:40:52 2023, max compression
+gzip compressed data, was "oapi-1.59.5.tar", last modified: Thu Jun 29 17:30:14 2023, max compression
```

## Comparing `oapi-1.59.4.tar` & `oapi-1.59.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:52.505836 oapi-1.59.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 04:40:05.000000 oapi-1.59.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-17 04:40:52.505836 oapi-1.59.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-17 04:40:05.000000 oapi-1.59.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:52.505836 oapi-1.59.4/oapi/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/_multipart_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   126802 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    61478 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:52.505836 oapi-1.59.4/oapi/oas/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/oas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125708 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/oas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/oas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/oas/references.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:05.000000 oapi-1.59.4/oapi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:52.505836 oapi-1.59.4/oapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-17 04:40:52.000000 oapi-1.59.4/oapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 04:40:52.000000 oapi-1.59.4/oapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 04:40:52.000000 oapi-1.59.4/oapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 04:40:52.000000 oapi-1.59.4/oapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 04:40:52.000000 oapi-1.59.4/oapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 04:40:05.000000 oapi-1.59.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-17 04:40:52.505836 oapi-1.59.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 04:40:05.000000 oapi-1.59.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 04:40:52.505836 oapi-1.59.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-17 04:40:05.000000 oapi-1.59.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-17 04:40:05.000000 oapi-1.59.4/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.015496 oapi-1.59.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 17:29:18.000000 oapi-1.59.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 17:30:14.015496 oapi-1.59.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-29 17:29:18.000000 oapi-1.59.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/oapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/_multipart_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126802 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61478 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/oapi/oas/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125708 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/oapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 17:29:18.000000 oapi-1.59.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 17:30:14.015496 oapi-1.59.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 17:29:18.000000 oapi-1.59.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 17:29:18.000000 oapi-1.59.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-29 17:29:18.000000 oapi-1.59.5/tests/test_model.py
```

### Comparing `oapi-1.59.4/LICENSE` & `oapi-1.59.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/PKG-INFO` & `oapi-1.59.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-Metadata-Version: 2.1
-Name: oapi
-Version: 1.59.4
-Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
-Home-page: https://github.com/enorganic/oapi
-Author-email: david@belais.me
-License: MIT
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # oapi
 
+[![test](https://github.com/enorganic/oapi/actions/workflows/test.yml/badge.svg)](https://github.com/enorganic/oapi/actions/workflows/test.yml)
+[![distribute](https://github.com/enorganic/oapi/actions/workflows/distribute.yml/badge.svg)](https://github.com/enorganic/oapi/actions/workflows/distribute.yml)
+
 `oapi` is a library and CLI for authoring python data models (for clients
 *or* servers), and/or client libraries, for web APIs, based on an
 OpenAPI specification (both OpenAPI/Swagger [version 2](https://bit.ly/36VneDU)
 and [version 3](https://bit.ly/3OHGRQV) are supported).
 
 `oapi`-generated packages/modules differ from those generated by other tools
 (including but not limited to
```

### Comparing `oapi-1.59.4/README.md` & `oapi-1.59.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,23 @@
+Metadata-Version: 2.1
+Name: oapi
+Version: 1.59.5
+Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
+Home-page: https://github.com/enorganic/oapi
+Author-email: david@belais.me
+License: MIT
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # oapi
 
+[![test](https://github.com/enorganic/oapi/actions/workflows/test.yml/badge.svg)](https://github.com/enorganic/oapi/actions/workflows/test.yml)
+[![distribute](https://github.com/enorganic/oapi/actions/workflows/distribute.yml/badge.svg)](https://github.com/enorganic/oapi/actions/workflows/distribute.yml)
+
 `oapi` is a library and CLI for authoring python data models (for clients
 *or* servers), and/or client libraries, for web APIs, based on an
 OpenAPI specification (both OpenAPI/Swagger [version 2](https://bit.ly/36VneDU)
 and [version 3](https://bit.ly/3OHGRQV) are supported).
 
 `oapi`-generated packages/modules differ from those generated by other tools
 (including but not limited to
```

### Comparing `oapi-1.59.4/oapi/_multipart_request.py` & `oapi-1.59.5/oapi/_multipart_request.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/oapi/_utilities.py` & `oapi-1.59.5/oapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/oapi/client.py` & `oapi-1.59.5/oapi/client.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/oapi/model.py` & `oapi-1.59.5/oapi/model.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/oapi/oas/model.py` & `oapi-1.59.5/oapi/oas/model.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/oapi/oas/references.py` & `oapi-1.59.5/oapi/oas/references.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.4/oapi.egg-info/PKG-INFO` & `oapi-1.59.5/oapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: oapi
-Version: 1.59.4
+Version: 1.59.5
 Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 Home-page: https://github.com/enorganic/oapi
 Author-email: david@belais.me
 License: MIT
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # oapi
 
+[![test](https://github.com/enorganic/oapi/actions/workflows/test.yml/badge.svg)](https://github.com/enorganic/oapi/actions/workflows/test.yml)
+[![distribute](https://github.com/enorganic/oapi/actions/workflows/distribute.yml/badge.svg)](https://github.com/enorganic/oapi/actions/workflows/distribute.yml)
+
 `oapi` is a library and CLI for authoring python data models (for clients
 *or* servers), and/or client libraries, for web APIs, based on an
 OpenAPI specification (both OpenAPI/Swagger [version 2](https://bit.ly/36VneDU)
 and [version 3](https://bit.ly/3OHGRQV) are supported).
 
 `oapi`-generated packages/modules differ from those generated by other tools
 (including but not limited to
```

### Comparing `oapi-1.59.4/setup.cfg` & `oapi-1.59.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [metadata]
 name = oapi
-version = 1.59.4
+version = 1.59.5
 author_email = david@belais.me
 description = An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/enorganic/oapi
 
 [options]
 python_requires = ~=3.7
 packages = find:
 include_package_data = True
 install_requires = 
 	pyyaml>2
-	iso8601~=1.1
+	iso8601~=2.0
 	sob~=1.50
-	jsonpointer~=2.3
+	jsonpointer~=2.4
 	more-itertools>=8.0,<10.0
 
 [options.package_data]
 * = py.typed
 
 [egg_info]
 tag_build =
```

### Comparing `oapi-1.59.4/tests/test_model.py` & `oapi-1.59.5/tests/test_model.py`

 * *Files identical despite different names*

