# Comparing `tmp/wad2023-program-1.2.0.tar.gz` & `tmp/wad2023-program-1.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.2.0.tar", last modified: Thu Jun 29 19:26:43 2023, max compression
+gzip compressed data, was "wad2023-program-1.2.1.dev0.tar", last modified: Thu Jun 29 19:30:17 2023, max compression
```

## Comparing `wad2023-program-1.2.0.tar` & `wad2023-program-1.2.1.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:26:43.035368 wad2023-program-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-29 19:26:43.035368 wad2023-program-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:26:43.035368 wad2023-program-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:26:43.035368 wad2023-program-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:26:43.035368 wad2023-program-1.2.0/src/wad2023_program/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/src/wad2023_program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/src/wad2023_program/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/src/wad2023_program/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/src/wad2023_program/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-29 19:26:31.000000 wad2023-program-1.2.0/src/wad2023_program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:26:43.035368 wad2023-program-1.2.0/src/wad2023_program.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-29 19:26:43.000000 wad2023-program-1.2.0/src/wad2023_program.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 19:26:43.000000 wad2023-program-1.2.0/src/wad2023_program.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:26:43.000000 wad2023-program-1.2.0/src/wad2023_program.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 19:26:43.000000 wad2023-program-1.2.0/src/wad2023_program.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 19:26:43.000000 wad2023-program-1.2.0/src/wad2023_program.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 19:26:43.000000 wad2023-program-1.2.0/src/wad2023_program.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:30:17.468729 wad2023-program-1.2.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-29 19:30:17.468729 wad2023-program-1.2.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:30:17.468729 wad2023-program-1.2.1.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:30:17.464729 wad2023-program-1.2.1.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:30:17.464729 wad2023-program-1.2.1.dev0/src/wad2023_program/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/src/wad2023_program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/src/wad2023_program/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/src/wad2023_program/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/src/wad2023_program/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-29 19:30:03.000000 wad2023-program-1.2.1.dev0/src/wad2023_program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:30:17.464729 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-29 19:30:17.000000 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 19:30:17.000000 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:30:17.000000 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 19:30:17.000000 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 19:30:17.000000 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 19:30:17.000000 wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.2.0/LICENSE` & `wad2023-program-1.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/PKG-INFO` & `wad2023-program-1.2.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.2.0
+Version: 1.2.1.dev0
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wad2023-program-1.2.0/README.md` & `wad2023-program-1.2.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/pyproject.toml` & `wad2023-program-1.2.1.dev0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "wad2023-program"
-version = "1.2.0"
+version = "1.2.1-dev"
 description = "Script to retrieve the program for WeAreDevelopers 2023 conference"
 readme = "README.md"
 authors = [{ name = "Daryl Stark", email = "daryl@dstark.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -40,15 +40,15 @@
 homepage = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
 repository = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
 
 [project.scripts]
 wad23 = "wad2023_program.__main__:main"
 
 [tool.bumpver]
-current_version = "1.2.0"
+current_version = "1.2.1-dev"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `wad2023-program-1.2.0/src/wad2023_program/__main__.py` & `wad2023-program-1.2.1.dev0/src/wad2023_program/__main__.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program/app_config.py` & `wad2023-program-1.2.1.dev0/src/wad2023_program/app_config.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program/model.py` & `wad2023-program-1.2.1.dev0/src/wad2023_program/model.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program/program.py` & `wad2023-program-1.2.1.dev0/src/wad2023_program/program.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program.egg-info/PKG-INFO` & `wad2023-program-1.2.1.dev0/src/wad2023_program.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.2.0
+Version: 1.2.1.dev0
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

