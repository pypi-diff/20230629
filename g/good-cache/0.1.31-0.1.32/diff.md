# Comparing `tmp/good_cache-0.1.31.tar.gz` & `tmp/good_cache-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "good_cache-0.1.31.tar", last modified: Thu Jun  8 02:25:55 2023, max compression
+gzip compressed data, was "good_cache-0.1.32.tar", last modified: Thu Jun 29 11:44:43 2023, max compression
```

## Comparing `good_cache-0.1.31.tar` & `good_cache-0.1.32.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.551959 good_cache-0.1.31/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)    11357 2023-05-04 02:17:26.000000 good_cache-0.1.31/LICENSE
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1575 2023-06-08 02:25:55.551959 good_cache-0.1.31/PKG-INFO
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1204 2023-06-08 02:11:57.000000 good_cache-0.1.31/README.md
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       38 2023-06-08 02:25:55.551959 good_cache-0.1.31/setup.cfg
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      759 2023-06-08 02:20:59.000000 good_cache-0.1.31/setup.py
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.547959 good_cache-0.1.31/src/
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.551959 good_cache-0.1.31/src/good_cache/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       48 2023-06-08 02:11:57.000000 good_cache-0.1.31/src/good_cache/__init__.py
--rwxrwxr-x   0 asundaram  (1000) asundaram  (1000)     7901 2023-06-08 02:11:57.000000 good_cache-0.1.31/src/good_cache/cache.py
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1239 2023-05-04 02:17:26.000000 good_cache-0.1.31/src/good_cache/utils.py
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.551959 good_cache-0.1.31/src/good_cache.egg-info/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1575 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/PKG-INFO
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      290 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/requires.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/top_level.txt
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-29 11:44:43.537011 good_cache-0.1.32/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)    11357 2023-06-09 02:28:31.000000 good_cache-0.1.32/LICENSE
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1686 2023-06-29 11:44:43.537011 good_cache-0.1.32/PKG-INFO
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1352 2023-06-29 11:38:49.000000 good_cache-0.1.32/README.md
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       38 2023-06-29 11:44:43.537011 good_cache-0.1.32/setup.cfg
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      759 2023-06-29 11:31:25.000000 good_cache-0.1.32/setup.py
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-29 11:44:43.533011 good_cache-0.1.32/src/
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-29 11:44:43.537011 good_cache-0.1.32/src/good_cache/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       48 2023-06-09 02:28:31.000000 good_cache-0.1.32/src/good_cache/__init__.py
+-rwxrwxr-x   0 asundaram  (1000) asundaram  (1000)     9872 2023-06-29 11:40:26.000000 good_cache-0.1.32/src/good_cache/cache.py
+-rwxrwxr-x   0 asundaram  (1000) asundaram  (1000)     1692 2023-06-10 03:07:05.000000 good_cache-0.1.32/src/good_cache/utils.py
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-29 11:44:43.537011 good_cache-0.1.32/src/good_cache.egg-info/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1686 2023-06-29 11:44:43.000000 good_cache-0.1.32/src/good_cache.egg-info/PKG-INFO
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      290 2023-06-29 11:44:43.000000 good_cache-0.1.32/src/good_cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-29 11:44:43.000000 good_cache-0.1.32/src/good_cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       18 2023-06-29 11:44:43.000000 good_cache-0.1.32/src/good_cache.egg-info/requires.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-29 11:44:43.000000 good_cache-0.1.32/src/good_cache.egg-info/top_level.txt
```

### Comparing `good_cache-0.1.31/LICENSE` & `good_cache-0.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `good_cache-0.1.31/PKG-INFO` & `good_cache-0.1.32/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: good_cache
-Version: 0.1.31
+Version: 0.1.32
 Summary: Efficient function output caching based on input files and other parameters to the function.
 Home-page: https://github.com/arunsundaram50/good-cache.git
 Author: Arun Sundaram
 Author-email: arun_co@yahoo.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # good_cache
 `good_cache` is a Python library that caches the output of your functions. If your function has to read large files as its input or if it has to read files in a directory, and optionally some non-file function parameter values such as a str, int, bool, etc. values then `good_cache` can remember the input combination and return the ouput to the caller as long as the input combination has been seen (and cached) by `good_cache` previously.
 
 ### Here is an article that goes into some detail about `good_cache`:
@@ -37,8 +35,9 @@
         with open(filename, 'rt') as file:
             numbers = list(map(int, file.readlines()))
             result += sum(numbers)
     return result
 ```
 
 
-
+### Here's an example of how you can evict a previous cache for a particular parameter(s)
+evicted = sum_numbers_in_files.evict(['a.txt', 'b.txt'])
```

### Comparing `good_cache-0.1.31/README.md` & `good_cache-0.1.32/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,7 +24,10 @@
     for filename in filenames:
         with open(filename, 'rt') as file:
             numbers = list(map(int, file.readlines()))
             result += sum(numbers)
     return result
 ```
 
+
+### Here's an example of how you can evict a previous cache for a particular parameter(s)
+evicted = sum_numbers_in_files.evict(['a.txt', 'b.txt'])
```

### Comparing `good_cache-0.1.31/setup.py` & `good_cache-0.1.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setup(
     name='good_cache',
-    version='0.1.31',
+    version='0.1.32',
     url='https://github.com/arunsundaram50/good-cache.git',
     author='Arun Sundaram',
     author_email='arun_co@yahoo.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     description='Efficient function output caching based on input files and other parameters to the function.',
     packages=find_packages(where="src"),  # Specifies the src directory
```

### Comparing `good_cache-0.1.31/src/good_cache/cache.py` & `good_cache-0.1.32/src/good_cache/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,47 @@
 #!/usr/bin/env python3
 
 import os, pickle, tempfile, threading, timeit, traceback, shutil
 from . import utils
+# import utils # for local testing
 from send2trash import send2trash
 from inspect import getfullargspec
+import pandas as pd
+
+
+def find_storage(file_with_no_ext):
+  for ext in ['parquet', 'pickle']:
+    if os.path.exists(f'{file_with_no_ext}.{ext}'):
+      return ext, f'{file_with_no_ext}.{ext}'
+  return None, None
+
+
+def get_storage(obj, file_with_no_ext):
+  if isinstance(obj, pd.DataFrame):
+    return "parquet", f'{file_with_no_ext}.parquet'
+  return "pickle", f'{file_with_no_ext}.pickle'
+
+
+def save_object(obj, filename):
+  if filename.endswith(".parquet"):
+    obj.to_parquet(filename)
+  else:
+    with open_and_lock_cache_file(filename, 'wb') as f:
+      pickle.dump(obj, f)
+
+
+def read_object(filename):
+  _, extension = os.path.splitext(filename)
+
+  if extension == '.parquet':
+    return pd.read_parquet(filename)
+  else:
+    with open_and_lock_cache_file(filename, 'rb') as f:
+      return pickle.load(f)
+
 
 cache_file_locks = {}
 
 def get_cache_file_lock(filename):
   # Get or create a lock for the given filename
   with cache_file_locks.setdefault(filename, threading.Lock()):
     # Return the lock associated with the filename
@@ -38,53 +72,71 @@
 
   def inner(f):
     argspec = getfullargspec(f)
     if files_arg_name:
       files_arg_pos = argspec.args.index(files_arg_name)
     else:
       files_arg_pos = None
-    def wrapper(*args, **kwargs):
-      if files_arg_pos:
+
+    def get_cache_file(*args, **kwargs):
+      if files_arg_pos!=None:
         files_arg_val = args[files_arg_pos]
       else:
         files_arg_val = ''
       args_as_str = f_args_to_str(*args, **kwargs)
       if shorten_cache_file:
         dyn_part = utils.compute_hash(args_as_str)
       else:
         dyn_part = args_as_str
-      cache_file = f'{tempfile.gettempdir()}/cache/{f.__name__}/{dyn_part}.pickle'
+      file_stem = f'{tempfile.gettempdir()}/cache/{f.__name__}/{dyn_part}'
+      storage_type, cache_file = find_storage(file_stem)
+      return storage_type, cache_file, files_arg_val, file_stem
+
+    def evict(*args, **kwargs):
+      _, cache_file, _, _ = get_cache_file(*args, **kwargs)
+      if os.path.exists(cache_file):
+        try:
+          send2trash(cache_file)
+          return True
+        except:
+          os.unlink(cache_file)
+          return True
+      return False
+
+    def wrapper(*args, **kwargs):
+      storage_type, cache_file, files_arg_val, file_stem = get_cache_file(*args, **kwargs)
 
       # recreate stale file
       ret = None
-      if utils.is_stale(cache_file, files_arg_val):
-        utils.ensure_parent(cache_file)
+      if storage_type == None or utils.is_stale(cache_file, files_arg_val):
         try:
           ret = f(*args)
           if not f_is_content_cacheable(ret):
             return ret
-          with open_and_lock_cache_file(cache_file, 'wb') as fp:
-            pickle.dump(ret, fp)
+          storage_type, cache_file = get_storage(ret, file_stem)
+          utils.ensure_parent(cache_file)
+          save_object(ret, cache_file)
         except:
-          if os.path.exists(cache_file):
+          if cache_file!=None and os.path.exists(cache_file):
             send2trash(cache_file)
           raise ValueError(f"Error invoking {f.__name__}")
 
       # load file
       try:
-        with open_and_lock_cache_file(cache_file, 'rb') as fp:
-          ret = pickle.load(fp)
+        ret = read_object(cache_file)
       except:
         utils.log(traceback.format_exc(0))
-        if os.path.exists(cache_file):
+        if cache_file!=None and os.path.exists(cache_file):
           send2trash(cache_file)
         raise ValueError(f"Error reading previous result of {f.__name__}")
 
       return ret
 
+    wrapper.get_cache_file = get_cache_file
+    wrapper.evict = evict
     return wrapper
   return inner
 
 
 """
 Usecase: when the output is dependant on dir and the optional parameters passed to the function.
 Output is kept in file system and reused if the dir was not modified and if the paramerers were used previously
@@ -94,14 +146,15 @@
   shorten_cache_file = dec_kwargs['shorten_cache_file'] if 'shorten_cache_file' in dec_kwargs else True
   f_args_to_str = dec_kwargs['args_to_str'] if 'args_to_str' in dec_kwargs else lambda f: ''
   f_is_content_cacheable = dec_kwargs['is_content_cacheable'] if 'is_content_cacheable' in dec_kwargs else lambda f: True
 
   def inner(f):
     argspec = getfullargspec(f)
     dir_arg_pos = argspec.args.index(dir_arg_name)
+
     def wrapper(*args, **kwargs):
       dir_arg_val = args[dir_arg_pos]
       arg_str = f_args_to_str(*args, **kwargs)
       dyn_part = f'{dir_arg_val}/{arg_str}'
       if shorten_cache_file:
         dyn_part = utils.compute_hash(dyn_part)
       cache_file = f'{tempfile.gettempdir()}/cache/{f.__name__}/{dyn_part}.pickle'
@@ -236,9 +289,22 @@
     return ", ".join(a + b)
 
   @fs_files_cache(files="filenames", args_to_str=my_args_to_str)
   def only_params_with_files_custom(filenames, a, b):
     print('processing a+b')
     return str(a+b)+str(filenames)
 
-  print(only_params_with_files_custom(['a.txt, b.txt'], 1, 25))
+  if not os.path.exists('/tmp/a.txt'):
+    with open('/tmp/a.txt', 'wt') as fp:
+      print(1, file=fp)
+      print(2, file=fp)
+      print(3, file=fp)
+
+  if not os.path.exists('/tmp/b.txt'):
+    with open('/tmp/b.txt', 'wt') as fp:
+      print(1, file=fp)
+
+  storage_type, cache_file, _, _ = only_params_with_files_custom.get_cache_file(['a.txt, b.txt'], 1, 25)
+  print(f'{storage_type=}, {cache_file=}')
+  # only_params_with_files_custom.evict(['/tmp/a.txt', '/tmp/b.txt'], 1, 25)
+  print(only_params_with_files_custom(['/tmp/a.txt', '/tmp/b.txt'], 1, 25))
```

### Comparing `good_cache-0.1.31/src/good_cache.egg-info/PKG-INFO` & `good_cache-0.1.32/src/good_cache.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: good-cache
-Version: 0.1.31
+Version: 0.1.32
 Summary: Efficient function output caching based on input files and other parameters to the function.
 Home-page: https://github.com/arunsundaram50/good-cache.git
 Author: Arun Sundaram
 Author-email: arun_co@yahoo.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # good_cache
 `good_cache` is a Python library that caches the output of your functions. If your function has to read large files as its input or if it has to read files in a directory, and optionally some non-file function parameter values such as a str, int, bool, etc. values then `good_cache` can remember the input combination and return the ouput to the caller as long as the input combination has been seen (and cached) by `good_cache` previously.
 
 ### Here is an article that goes into some detail about `good_cache`:
@@ -37,8 +35,9 @@
         with open(filename, 'rt') as file:
             numbers = list(map(int, file.readlines()))
             result += sum(numbers)
     return result
 ```
 
 
-
+### Here's an example of how you can evict a previous cache for a particular parameter(s)
+evicted = sum_numbers_in_files.evict(['a.txt', 'b.txt'])
```

