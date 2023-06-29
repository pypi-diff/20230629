# Comparing `tmp/fastapi_orm_manager-0.0.8.tar.gz` & `tmp/fastapi_orm_manager-0.0.9.tar.gz`

## Comparing `fastapi_orm_manager-0.0.8.tar` & `fastapi_orm_manager-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/requirements.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/fastapi_manager/__init__.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/fastapi_manager/decorators.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/fastapi_manager/managers.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/fastapi_manager/meta.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/fastapi_manager/pagination.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/LICENSE
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/fastapi_manager/__init__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/fastapi_manager/decorators.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/fastapi_manager/managers.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/fastapi_manager/meta.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/fastapi_manager/pagination.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/LICENSE
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastapi_orm_manager-0.0.9/PKG-INFO
```

### Comparing `fastapi_orm_manager-0.0.8/fastapi_manager/decorators.py` & `fastapi_orm_manager-0.0.9/fastapi_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `fastapi_orm_manager-0.0.8/fastapi_manager/managers.py` & `fastapi_orm_manager-0.0.9/fastapi_manager/managers.py`

 * *Files identical despite different names*

### Comparing `fastapi_orm_manager-0.0.8/fastapi_manager/meta.py` & `fastapi_orm_manager-0.0.9/fastapi_manager/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_orm_manager-0.0.8/fastapi_manager/pagination.py` & `fastapi_orm_manager-0.0.9/fastapi_manager/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sqlalchemy import func, Select
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Session
 
 
 class Pagination(BaseModel):
     page: int
-    results: Union[Sequence[any], List[any]]
+    results: Union[Sequence, List]
     total: int
     has_prev: bool
     has_next: bool
 
 
 class Paginator:
     per_page: int = 25
```

### Comparing `fastapi_orm_manager-0.0.8/.gitignore` & `fastapi_orm_manager-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_orm_manager-0.0.8/LICENSE` & `fastapi_orm_manager-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_orm_manager-0.0.8/pyproject.toml` & `fastapi_orm_manager-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi-orm-manager"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Nazar Kaliuzhnyi", email = "kaluzghnyy@gmail.com" },
 ]
 description = "A base manager class to handle CRUD on SQLAlchemy models. Suitable to use in FastAPI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fastapi_orm_manager-0.0.8/PKG-INFO` & `fastapi_orm_manager-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-orm-manager
-Version: 0.0.8
+Version: 0.0.9
 Summary: A base manager class to handle CRUD on SQLAlchemy models. Suitable to use in FastAPI projects.
 Project-URL: Homepage, https://github.com/nakeeon/FastAPI-ORM-Manager
 Project-URL: Bug Tracker, https://github.com/nakeeon/FastAPI-ORM-Manager/issues
 Author-email: Nazar Kaliuzhnyi <kaluzghnyy@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

