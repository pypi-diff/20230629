# Comparing `tmp/gimera-0.6.91.tar.gz` & `tmp/gimera-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.6.91.tar", last modified: Fri Jun 16 16:03:30 2023, max compression
+gzip compressed data, was "gimera-0.7.1.tar", last modified: Thu Jun 29 06:21:41 2023, max compression
```

## Comparing `gimera-0.6.91.tar` & `gimera-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.429068 gimera-0.6.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 16:02:51.000000 gimera-0.6.91/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-16 16:03:30.429068 gimera-0.6.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-16 16:02:51.000000 gimera-0.6.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.429068 gimera-0.6.91/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37466 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.429068 gimera-0.6.91/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 16:03:30.429068 gimera-0.6.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-16 16:02:51.000000 gimera-0.6.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:21:41.512135 gimera-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 06:20:56.000000 gimera-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-29 06:21:41.512135 gimera-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-29 06:20:56.000000 gimera-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:21:41.512135 gimera-0.7.1/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37461 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-29 06:20:56.000000 gimera-0.7.1/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:21:41.512135 gimera-0.7.1/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 06:21:41.000000 gimera-0.7.1/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 06:21:41.512135 gimera-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-29 06:20:56.000000 gimera-0.7.1/setup.py
```

### Comparing `gimera-0.6.91/LICENSE.txt` & `gimera-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.6.91/PKG-INFO` & `gimera-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.6.91
+Version: 0.7.1
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.6.91/README.md` & `gimera-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.6.91/gimera/config.py` & `gimera-0.7.1/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.91/gimera/gimera.py` & `gimera-0.7.1/gimera/gimera.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,31 +174,34 @@
 )
 @click.option(
     "--remove-invalid-branches",
     is_flag=True,
     help="If branch does not exist in repository, the configuration item is removed.",
 )
 @click.option(
-    "-d",
-    "--make-missing-patch-directories",
+    "-I",
+    "--non-interactive",
     is_flag=True,
-    help="Usually gimera is strict about directories. But can create patch directories on demand",
+    help="",
 )
 def apply(
     repos,
     update,
     all_integrated,
     all_submodule,
     parallel_safe,
     strict,
     recursive,
     no_patches,
     missing,
     remove_invalid_branches,
+    non_interactive,
 ):
+    if non_interactive:
+        os.environ['GIMERA_NON_INTERACTIVE'] = '1'
     if all_integrated and all_submodule:
         _raise_error("Please set either -I or -S")
     ttype = None
     ttype = REPO_TYPE_INT if all_integrated else ttype
     ttype = REPO_TYPE_SUB if all_submodule else ttype
 
     repos = list(_expand_repos(repos))
```

### Comparing `gimera-0.6.91/gimera/gitcommands.py` & `gimera-0.7.1/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.91/gimera/repo.py` & `gimera-0.7.1/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.91/gimera/tools.py` & `gimera-0.7.1/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.91/gimera.egg-info/PKG-INFO` & `gimera-0.7.1/gimera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.6.91
+Version: 0.7.1
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.6.91/setup.py` & `gimera-0.7.1/setup.py`

 * *Files identical despite different names*

