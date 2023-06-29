# Comparing `tmp/pycareer-0.1.5.tar.gz` & `tmp/pycareer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycareer-0.1.5.tar", max compression
+gzip compressed data, was "pycareer-0.1.6.tar", max compression
```

## Comparing `pycareer-0.1.5.tar` & `pycareer-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       45 2023-06-29 10:24:03.366914 pycareer-0.1.5/README.md
--rw-r--r--   0        0        0      105 2023-06-29 11:56:51.611692 pycareer-0.1.5/pycareer/__init__.py
--rw-r--r--   0        0        0     1049 2023-06-29 11:03:51.378455 pycareer-0.1.5/pycareer/cli.py
--rw-r--r--   0        0        0      604 2023-06-29 11:01:31.439498 pycareer-0.1.5/pycareer/formatter.py
--rw-r--r--   0        0        0      181 2023-06-29 10:34:05.809716 pycareer-0.1.5/pycareer/models.py
--rw-r--r--   0        0        0     1025 2023-06-29 11:01:31.443498 pycareer-0.1.5/pycareer/request.py
--rw-r--r--   0        0        0     1134 2023-06-29 11:56:51.627692 pycareer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pycareer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      663 2023-06-29 13:01:15.297309 pycareer-0.1.6/README.md
+-rw-r--r--   0        0        0      105 2023-06-29 11:56:51.611692 pycareer-0.1.6/pycareer/__init__.py
+-rw-r--r--   0        0        0     1049 2023-06-29 11:03:51.378455 pycareer-0.1.6/pycareer/cli.py
+-rw-r--r--   0        0        0      628 2023-06-29 12:45:11.377114 pycareer-0.1.6/pycareer/formatter.py
+-rw-r--r--   0        0        0      181 2023-06-29 10:34:05.809716 pycareer-0.1.6/pycareer/models.py
+-rw-r--r--   0        0        0     1025 2023-06-29 11:01:31.443498 pycareer-0.1.6/pycareer/request.py
+-rw-r--r--   0        0        0     1134 2023-06-29 12:45:43.697171 pycareer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 pycareer-0.1.6/PKG-INFO
```

### Comparing `pycareer-0.1.5/pycareer/cli.py` & `pycareer-0.1.6/pycareer/cli.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.5/pycareer/formatter.py` & `pycareer-0.1.6/pycareer/formatter.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,9 +14,10 @@
     table.add_column("Location")
     table.add_column("Salary")
     table.add_column("URL")
     table.add_column("Date")
 
     for job in jobs:
         table.add_row(job.id, job.title, job.company or "-", job.location or "-", job.salary or "-", job.url, job.date)
+        table.add_row()
 
     console.print(table)
```

### Comparing `pycareer-0.1.5/pycareer/request.py` & `pycareer-0.1.6/pycareer/request.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.5/pyproject.toml` & `pycareer-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [project.urls]
 Homepage = "https://pycareer.io"
 Documentation = "https://github.com/tadasgedgaudas/pycareer/README.md"
 Repository = "https://github.com/tadasgedgaudas/pycareer"
 
 [tool.poetry]
 name = "pycareer"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Tadas Gedgaudas <tadasgedgaudas@0xw.app>"]
 readme = "README.md"
 packages = [{include = "pycareer"}]
 
 
 [tool.poetry.dependencies]
```

