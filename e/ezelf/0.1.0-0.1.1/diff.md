# Comparing `tmp/ezelf-0.1.0.tar.gz` & `tmp/ezelf-0.1.1.tar.gz`

## Comparing `ezelf-0.1.0.tar` & `ezelf-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.1.0/tox.ini
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ezelf-0.1.0/src/fake.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ezelf-0.1.0/src/ezelf/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ezelf-0.1.0/src/ezelf/__main__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ezelf-0.1.0/src/ezelf/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ezelf-0.1.0/src/ezelf/sync/__init__.py
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 ezelf-0.1.0/src/ezelf/sync/ezpie.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ezelf-0.1.0/tests/test_simple.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ezelf-0.1.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.1.0/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.1.0/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ezelf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 ezelf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 ezelf-0.1.1/tox.ini
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ezelf-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ezelf-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ezelf-0.1.1/src/fake.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ezelf-0.1.1/src/ezelf/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ezelf-0.1.1/src/ezelf/__main__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ezelf-0.1.1/src/ezelf/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ezelf-0.1.1/src/ezelf/sync/__init__.py
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 ezelf-0.1.1/src/ezelf/sync/ezpie.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ezelf-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ezelf-0.1.1/tests/test_simple.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ezelf-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ezelf-0.1.1/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ezelf-0.1.1/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ezelf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 ezelf-0.1.1/PKG-INFO
```

### Comparing `ezelf-0.1.0/tox.ini` & `ezelf-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/.github/workflows/release.yml` & `ezelf-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/.github/workflows/test.yml` & `ezelf-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/src/ezelf/main.py` & `ezelf-0.1.1/src/ezelf/main.py`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/src/ezelf/sync/ezpie.py` & `ezelf-0.1.1/src/ezelf/sync/ezpie.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         raise EzpieSyncError(f"prepare param raise exception: {e}")
 
     if data is None:
         raise EzpieSyncError("data is None")
 
     sync_url = f"{sync_host}{sync_api}"
 
+    logging.info(f"payload: {data}")
     try:
         response = requests.post(sync_url, json=data, timeout=(6, 4))
     except Exception as e:
         raise EzpieSyncError(f"requests except, {e}")
 
     response_code = response.status_code
     if response_code != 200:
```

### Comparing `ezelf-0.1.0/tests/test_simple.py` & `ezelf-0.1.1/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/.gitignore` & `ezelf-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/LICENSE` & `ezelf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezelf-0.1.0/PKG-INFO` & `ezelf-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezelf
-Version: 0.1.0
+Version: 0.1.1
 Summary: A elf for ezpie
 License: MIT License
         
         Copyright (c) 2023 ez-pie
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

