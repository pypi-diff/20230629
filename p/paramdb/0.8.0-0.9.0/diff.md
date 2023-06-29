# Comparing `tmp/paramdb-0.8.0.tar.gz` & `tmp/paramdb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramdb-0.8.0.tar", max compression
+gzip compressed data, was "paramdb-0.9.0.tar", max compression
```

## Comparing `paramdb-0.8.0.tar` & `paramdb-0.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1521 2023-06-10 00:17:43.196195 paramdb-0.8.0/LICENSE
--rw-r--r--   0        0        0     1861 2023-06-10 00:17:43.196195 paramdb-0.8.0/README.md
--rw-r--r--   0        0        0      706 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/__init__.py
--rw-r--r--   0        0        0     9560 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_database.py
--rw-r--r--   0        0        0      571 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_keys.py
--rw-r--r--   0        0        0        0 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_param_data/__init__.py
--rw-r--r--   0        0        0     6622 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_param_data/_collections.py
--rw-r--r--   0        0        0     3498 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_param_data/_dataclasses.py
--rw-r--r--   0        0        0     4343 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_param_data/_param_data.py
--rw-r--r--   0        0        0     1177 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/_param_data/_type_mixins.py
--rw-r--r--   0        0        0        0 2023-06-10 00:17:43.200195 paramdb-0.8.0/paramdb/py.typed
--rw-r--r--   0        0        0     1212 2023-06-10 00:17:43.200195 paramdb-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 paramdb-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-29 19:01:15.627857 paramdb-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1861 2023-06-29 19:01:15.627857 paramdb-0.9.0/README.md
+-rw-r--r--   0        0        0      706 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/__init__.py
+-rw-r--r--   0        0        0    10274 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_database.py
+-rw-r--r--   0        0        0      571 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_keys.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/__init__.py
+-rw-r--r--   0        0        0     6622 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_collections.py
+-rw-r--r--   0        0        0     3498 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_dataclasses.py
+-rw-r--r--   0        0        0     4343 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_param_data.py
+-rw-r--r--   0        0        0     1177 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_type_mixins.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/py.typed
+-rw-r--r--   0        0        0     1213 2023-06-29 19:01:15.627857 paramdb-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 paramdb-0.9.0/PKG-INFO
```

### Comparing `paramdb-0.8.0/LICENSE` & `paramdb-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/README.md` & `paramdb-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/paramdb/__init__.py` & `paramdb-0.9.0/paramdb/__init__.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/paramdb/_database.py` & `paramdb-0.9.0/paramdb/_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,18 +140,24 @@
         class Root(Struct):
             pass
 
         param_db = ParamDB[Root]("path/to/param.db")
     """
 
     def __init__(self, path: str):
+        self._path = path
         self._engine = create_engine(URL.create("sqlite+pysqlite", database=path))
         self._Session = sessionmaker(self._engine)  # pylint: disable=invalid-name
         _Base.metadata.create_all(self._engine)
 
+    @property
+    def path(self) -> str:
+        """Path of the database file."""
+        return self._path
+
     def commit(self, message: str, data: T) -> int:
         """
         Commit the given data to the database with the given message and return the ID
         of the new commit.
         """
         with self._Session.begin() as session:
             snapshot = _Snapshot(
@@ -194,18 +200,17 @@
             else select_stmt.where(_Snapshot.id == commit_id)  # Specified commit
         )
         with self._Session() as session:
             data = session.scalar(select_stmt)
         if data is None:
             raise IndexError(
                 f"cannot load most recent commit because database"
-                f" '{self._engine.url.database}' has no commits"
+                f" '{self._path}' has no commits"
                 if commit_id is None
-                else f"commit {commit_id} does not exist in database"
-                f" '{self._engine.url.database}'"
+                else f"commit {commit_id} does not exist in database" f" '{self._path}'"
             )
         return json.loads(
             _decompress(data),
             object_hook=_from_dict if load_classes else None,
         )
 
     @property
@@ -213,14 +218,26 @@
         """Number of commits in the database."""
         count_func = func.count()  # pylint: disable=not-callable
         select_stmt = select(count_func).select_from(_Snapshot)
         with self._Session() as session:
             count = session.execute(select_stmt).scalar()
         return count if count is not None else 0
 
+    @property
+    def latest_commit(self) -> CommitEntry | None:
+        """Latest commit added to the database, or None if the database is empty."""
+        max_id_func = func.max(_Snapshot.id)  # pylint: disable=not-callable
+        select_max_id = select(max_id_func).scalar_subquery()
+        select_stmt = select(
+            _Snapshot.id, _Snapshot.message, _Snapshot.timestamp
+        ).where(_Snapshot.id == select_max_id)
+        with self._Session() as session:
+            latest_entry = session.execute(select_stmt).mappings().first()
+        return None if latest_entry is None else CommitEntry(**latest_entry)
+
     def commit_history(
         self,
         start: int | None = None,
         end: int | None = None,
     ) -> list[CommitEntry]:
         """
         Retrieve the commit history as a list of :py:class:`CommitEntry` between the
```

### Comparing `paramdb-0.8.0/paramdb/_keys.py` & `paramdb-0.9.0/paramdb/_keys.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/paramdb/_param_data/_collections.py` & `paramdb-0.9.0/paramdb/_param_data/_collections.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/paramdb/_param_data/_dataclasses.py` & `paramdb-0.9.0/paramdb/_param_data/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/paramdb/_param_data/_param_data.py` & `paramdb-0.9.0/paramdb/_param_data/_param_data.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/paramdb/_param_data/_type_mixins.py` & `paramdb-0.9.0/paramdb/_param_data/_type_mixins.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.8.0/pyproject.toml` & `paramdb-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "paramdb"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python package for storing and retrieving experiment parameters."
 authors = ["Alex Hadley <alexhad6@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/PainterQubits/paramdb"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typing-extensions = "^4.6.3"
-sqlalchemy = "^2.0.15"
+typing-extensions = "^4.7.0"
+sqlalchemy = "^2.0.17"
 zstandard = "^0.21.0"
 astropy = {version = "^5.3", optional = true}
 
 [tool.poetry.extras]
 astropy = ["astropy"]
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
+pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 flake8 = "^6.0.0"
 pylint = "^2.17.4"
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 black = "^23.3.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "6.2.1"
-myst-parser = "^1.0.0"
+sphinx = "^7.0.1"
+myst-parser = "^2.0.0"
 furo = "^2023.5.20"
 sphinx-copybutton = "^0.5.2"
 jupyter-sphinx = "^0.4.0"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
```

### Comparing `paramdb-0.8.0/PKG-INFO` & `paramdb-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: paramdb
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package for storing and retrieving experiment parameters.
 Home-page: https://github.com/PainterQubits/paramdb
 License: BSD-3-Clause
 Author: Alex Hadley
 Author-email: alexhad6@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: astropy
 Requires-Dist: astropy (>=5.3,<6.0) ; extra == "astropy"
-Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
-Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
+Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
+Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
 Requires-Dist: zstandard (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/PainterQubits/paramdb
 Description-Content-Type: text/markdown
 
 # ParamDB
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/paramdb)](https://pypi.org/project/paramdb/)
```

