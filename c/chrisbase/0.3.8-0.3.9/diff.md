# Comparing `tmp/chrisbase-0.3.8.tar.gz` & `tmp/chrisbase-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisbase-0.3.8.tar", last modified: Thu May 18 18:28:11 2023, max compression
+gzip compressed data, was "chrisbase-0.3.9.tar", last modified: Thu Jun 29 13:53:46 2023, max compression
```

## Comparing `chrisbase-0.3.8.tar` & `chrisbase-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:28:11.755527 chrisbase-0.3.8/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-14 13:51:31.000000 chrisbase-0.3.8/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-05-18 18:28:11.755527 chrisbase-0.3.8/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-05-14 13:51:31.000000 chrisbase-0.3.8/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-14 13:51:31.000000 chrisbase-0.3.8/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      946 2023-05-18 18:28:11.755527 chrisbase-0.3.8/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:28:11.751527 chrisbase-0.3.8/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:28:11.751527 chrisbase-0.3.8/src/chrisbase/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:31.000000 chrisbase-0.3.8/src/chrisbase/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-05-14 13:51:31.000000 chrisbase-0.3.8/src/chrisbase/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    23294 2023-05-18 12:31:35.000000 chrisbase-0.3.8/src/chrisbase/io.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-05-14 13:51:31.000000 chrisbase-0.3.8/src/chrisbase/morp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-05-14 13:51:31.000000 chrisbase-0.3.8/src/chrisbase/time.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-05-14 13:51:31.000000 chrisbase-0.3.8/src/chrisbase/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:28:11.755527 chrisbase-0.3.8/src/chrisbase.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      431 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      129 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 18:28:11.000000 chrisbase-0.3.8/src/chrisbase.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.140365 chrisbase-0.3.9/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-06-29 13:39:47.000000 chrisbase-0.3.9/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-06-29 13:53:46.140365 chrisbase-0.3.9/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-06-29 13:39:47.000000 chrisbase-0.3.9/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-06-29 13:39:47.000000 chrisbase-0.3.9/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      956 2023-06-29 13:53:46.140365 chrisbase-0.3.9/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.136366 chrisbase-0.3.9/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.136366 chrisbase-0.3.9/src/chrisbase/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23190 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/io.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/morp.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/time.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.140365 chrisbase-0.3.9/src/chrisbase.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      431 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      138 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 13:53:45.000000 chrisbase-0.3.9/src/chrisbase.egg-info/zip-safe
```

### Comparing `chrisbase-0.3.8/LICENSE` & `chrisbase-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.8/PKG-INFO` & `chrisbase-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.3.8
+Version: 0.3.9
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrisbase-0.3.8/setup.cfg` & `chrisbase-0.3.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrisbase
-version = 0.3.8
+version = 0.3.9
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrisbase
 description = A base tool for python programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -32,14 +32,15 @@
 	chrisdict
 	matplotlib
 	sqlalchemy
 	dataclasses
 	dataclasses-json
 	scikit-learn
 	seqeval
+	openpyxl
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = README.md
```

### Comparing `chrisbase-0.3.8/src/chrisbase/io.py` & `chrisbase-0.3.9/src/chrisbase/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 def file_table(tabular_data, headers=(), tablefmt="pipe", showindex="default", transposed_df=False, file=sys_stdout, **kwargs):
     if not headers and isinstance(tabular_data, pd.DataFrame):
         if showindex is True or showindex == "default" or showindex == "always" or \
                 not isinstance(showindex, str) and isinstance(showindex, Iterable) and len(showindex) != len(tabular_data):
             if transposed_df:
                 if isinstance(tabular_data.columns, pd.RangeIndex):
-                    headers = ['key'] + list(range(1, len(tabular_data.columns) + 1))
+                    headers = ['key'] + list(map(str(range(1, len(tabular_data.columns) + 1))))
                 else:
                     headers = ['key'] + list(tabular_data.columns)
             else:
                 headers = ['#'] + list(tabular_data.columns)
                 showindex = range(1, len(tabular_data) + 1)
         else:
             headers = tabular_data.columns
@@ -665,24 +665,22 @@
 class ProjectEnv(DataClassJsonMixin):
     project: str = field()
     hostname: str = field(init=False)
     hostaddr: str = field(init=False)
     python_path: Path = field(init=False)
     working_path: Path = field(init=False)
     running_file: Path = field(init=False)
-    running_gpus: str | None = field(default=None)
+    logging_file: Path = field(default="logger.out")
     argument_file: Path = field(default="arguments.json")
 
     def __post_init__(self):
         assert self.project, "Project name must be provided"
         self.hostname = get_hostname()
         self.hostaddr = get_hostaddr()
         self.python_path = Path(sys.executable)
         self.running_file = running_file()
         self.project_path = first_or([x for x in self.running_file.parents if x.name.startswith(self.project)])
         assert self.project_path, f"Could not find project path for {self.project} in {', '.join([str(x) for x in self.running_file.parents])}"
         self.working_path = cwd(self.project_path)
         self.running_file = self.running_file.relative_to(self.working_path)
-        if self.running_gpus:
-            from chrislab.common.util import cuda_visible_devices
-            self.running_gpus = cuda_visible_devices(self.running_gpus)
+        self.logging_file = Path(self.logging_file)
         self.argument_file = Path(self.argument_file)
```

### Comparing `chrisbase-0.3.8/src/chrisbase/morp.py` & `chrisbase-0.3.9/src/chrisbase/morp.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.8/src/chrisbase/time.py` & `chrisbase-0.3.9/src/chrisbase/time.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.8/src/chrisbase/util.py` & `chrisbase-0.3.9/src/chrisbase/util.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.8/src/chrisbase.egg-info/PKG-INFO` & `chrisbase-0.3.9/src/chrisbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.3.8
+Version: 0.3.9
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

