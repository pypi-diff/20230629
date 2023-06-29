# Comparing `tmp/resgen-python-0.5.4.tar.gz` & `tmp/resgen-python-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resgen-python-0.5.4.tar", last modified: Thu Feb 10 05:05:23 2022, max compression
+gzip compressed data, was "resgen-python-0.5.5.tar", last modified: Thu Jun 29 14:00:28 2023, max compression
```

## Comparing `resgen-python-0.5.4.tar` & `resgen-python-0.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:23.765391 resgen-python-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-10 05:05:08.000000 resgen-python-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-02-10 05:05:23.765391 resgen-python-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-10 05:05:08.000000 resgen-python-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-02-10 05:05:08.000000 resgen-python-0.5.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:23.761390 resgen-python-0.5.4/resgen/
--rw-r--r--   0 runner    (1001) docker     (121)    32189 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:23.761390 resgen-python-0.5.4/resgen/list/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/list/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:23.761390 resgen-python-0.5.4/resgen/sync/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-02-10 05:05:08.000000 resgen-python-0.5.4/resgen/sync/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 05:05:23.765391 resgen-python-0.5.4/resgen_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-10 05:05:23.000000 resgen-python-0.5.4/resgen_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-10 05:05:23.765391 resgen-python-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-02-10 05:05:08.000000 resgen-python-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:28.936756 resgen-python-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 14:00:15.000000 resgen-python-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-29 14:00:28.936756 resgen-python-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-29 14:00:15.000000 resgen-python-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 14:00:15.000000 resgen-python-0.5.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:28.932755 resgen-python-0.5.5/resgen/
+-rw-r--r--   0 runner    (1001) docker     (123)    32189 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:28.932755 resgen-python-0.5.5/resgen/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/list/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:28.932755 resgen-python-0.5.5/resgen/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-29 14:00:15.000000 resgen-python-0.5.5/resgen/sync/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:00:28.932755 resgen-python-0.5.5/resgen_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 14:00:28.000000 resgen-python-0.5.5/resgen_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:00:28.936756 resgen-python-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-29 14:00:15.000000 resgen-python-0.5.5/setup.py
```

### Comparing `resgen-python-0.5.4/PKG-INFO` & `resgen-python-0.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: resgen-python
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python bindings for the resgen genomic data service
 Home-page: https://github.com/reservoirgenomics/resgen-python
 Author: Peter Kerpedjiev
 Author-email: pkerpedjiev@gmail.com
-License: UNKNOWN
 Keywords: resgen
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
-
-UNKNOWN
-
```

### Comparing `resgen-python-0.5.4/resgen/__init__.py` & `resgen-python-0.5.5/resgen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # from higlass.utils import fill_filetype_and_datatype
 from resgen import aws
 
 # import resgen.utils as rgu
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 
 RESGEN_HOST = "https://resgen.io"
 RESGEN_BUCKET = "resgen"
 RESGEN_AUTH0_CLIENT_ID = "NT4NPUbrBKU3N9HVcqLP8819P7ZD91iU"
 RESGEN_AUTH0_DOMAIN = "https://auth.resgen.io"
 # RESGEN_HOST = "http://localhost:8000"
 # RESGEN_BUCKET = "resgen-test"
```

### Comparing `resgen-python-0.5.4/resgen/aws.py` & `resgen-python-0.5.5/resgen/aws.py`

 * *Files identical despite different names*

### Comparing `resgen-python-0.5.4/resgen/list/commands.py` & `resgen-python-0.5.5/resgen/list/commands.py`

 * *Files identical despite different names*

### Comparing `resgen-python-0.5.4/resgen/sync/commands.py` & `resgen-python-0.5.5/resgen/sync/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,24 @@
 @click.argument("gruser")
 @click.argument("project")
 @click.argument("datasets", nargs=-1)
 @click.option("-t", "--tag", multiple=True)
 @click.option("--sync-remote/--no-sync-remote", default=False)
 @click.option("--name", default=None)
 @click.option("--sync-full-path/--no-sync-full-path", default=False)
-def datasets(gruser, project, datasets, tag, sync_remote, name, sync_full_path):
+@click.option("-f", "--force-update", default=False)
+def datasets(gruser, project, datasets, tag, sync_remote, name, sync_full_path,
+             force_update):
     """Upload if a file with the same name doesn't already exist.
 
     If files are of the form "filename1,filename2" it will be assumed
     that filename2 is the index file for filename1.
+
+    If -f/--force-update is specified, files will be uploaded even if they already exist
+    in the project.
     """
     try:
         try:
             rgc = rg.connect()
         except rg.UnknownConnectionException:
             logger.error("Unable to login, please check your username and password")
             return
@@ -53,21 +58,30 @@
                     str(metadata),
                 )
                 project.sync_dataset(
                     parts[0],
                     index_filepath=parts[1],
                     sync_remote=sync_remote,
                     sync_full_path=sync_full_path,
-                    **metadata
+                    force_update=force_update,
+                    **metadata,
                 )
             else:
                 logger.info(
-                    "Syncing dataset: %s with metadata: %s", parts[0], str(metadata),
+                    "Syncing dataset: %s with metadata: %s",
+                    parts[0],
+                    str(metadata),
+                )
+                project.sync_dataset(
+                    dataset,
+                    sync_remote,
+                    sync_full_path=sync_full_path,
+                    force_update=force_update,
+                    **metadata
                 )
-                project.sync_dataset(dataset, sync_remote, sync_full_path=sync_full_path, **metadata)
     except rg.InvalidCredentialsException:
         logger.error(
             "Invalid credentials. Make sure that they are set in either "
             "~/.resgen/credentials or in the environment variables RESGEN_USERNAME "
             "and RESGEN_PASSWORD."
         )
```

### Comparing `resgen-python-0.5.4/resgen_python.egg-info/PKG-INFO` & `resgen-python-0.5.5/resgen_python.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: resgen-python
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python bindings for the resgen genomic data service
 Home-page: https://github.com/reservoirgenomics/resgen-python
 Author: Peter Kerpedjiev
 Author-email: pkerpedjiev@gmail.com
-License: UNKNOWN
 Keywords: resgen
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
-
-UNKNOWN
-
```

### Comparing `resgen-python-0.5.4/setup.py` & `resgen-python-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def get_requirements(path):
     content = read(path)
     return [req for req in content.split("\n") if req != "" and not req.startswith("#")]
 
 
 setup_args = {
     "name": "resgen-python",
-    "version": "0.5.4",
+    "version": "0.5.5",
     "packages": find_packages(),
     "description": "Python bindings for the resgen genomic data service",
     # "long_description": read("README.md"),
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/reservoirgenomics/resgen-python",
     "include_package_data": True,
     "zip_safe": False,
```

