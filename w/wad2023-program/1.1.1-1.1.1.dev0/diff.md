# Comparing `tmp/wad2023-program-1.1.1.tar.gz` & `tmp/wad2023-program-1.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.1.1.tar", last modified: Thu Jun 29 06:24:27 2023, max compression
+gzip compressed data, was "wad2023-program-1.1.1.dev0.tar", last modified: Thu Jun 29 06:21:29 2023, max compression
```

## Comparing `wad2023-program-1.1.1.tar` & `wad2023-program-1.1.1.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:24:27.610131 wad2023-program-1.1.1/
--rw-rw-rw-   0        0        0     1089 2023-06-29 06:18:23.000000 wad2023-program-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4779 2023-06-29 06:24:27.608131 wad2023-program-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2897 2023-06-29 06:18:23.000000 wad2023-program-1.1.1/README.md
--rw-rw-rw-   0        0        0     1642 2023-06-29 06:23:51.000000 wad2023-program-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 06:24:27.611131 wad2023-program-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 06:24:27.530133 wad2023-program-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 06:24:27.576144 wad2023-program-1.1.1/src/wad2023_program/
--rw-rw-rw-   0        0        0      174 2023-06-29 06:23:51.000000 wad2023-program-1.1.1/src/wad2023_program/__init__.py
--rw-rw-rw-   0        0        0     4179 2023-06-29 06:18:23.000000 wad2023-program-1.1.1/src/wad2023_program/__main__.py
--rw-rw-rw-   0        0        0      633 2023-06-29 05:48:10.000000 wad2023-program-1.1.1/src/wad2023_program/app_config.py
--rw-rw-rw-   0        0        0     3550 2023-06-29 06:18:23.000000 wad2023-program-1.1.1/src/wad2023_program/model.py
--rw-rw-rw-   0        0        0     4256 2023-06-29 06:18:23.000000 wad2023-program-1.1.1/src/wad2023_program/program.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:24:27.604133 wad2023-program-1.1.1/src/wad2023_program.egg-info/
--rw-rw-rw-   0        0        0     4779 2023-06-29 06:24:27.000000 wad2023-program-1.1.1/src/wad2023_program.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-29 06:24:27.000000 wad2023-program-1.1.1/src/wad2023_program.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:24:27.000000 wad2023-program-1.1.1/src/wad2023_program.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-29 06:24:27.000000 wad2023-program-1.1.1/src/wad2023_program.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      235 2023-06-29 06:24:27.000000 wad2023-program-1.1.1/src/wad2023_program.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 06:24:27.000000 wad2023-program-1.1.1/src/wad2023_program.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.818737 wad2023-program-1.1.1.dev0/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/LICENSE
+-rw-rw-rw-   0        0        0     4784 2023-06-29 06:21:29.811728 wad2023-program-1.1.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/README.md
+-rw-rw-rw-   0        0        0     1650 2023-06-29 06:19:31.000000 wad2023-program-1.1.1.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 06:21:29.820732 wad2023-program-1.1.1.dev0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.691730 wad2023-program-1.1.1.dev0/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.758730 wad2023-program-1.1.1.dev0/src/wad2023_program/
+-rw-rw-rw-   0        0        0      178 2023-06-29 06:18:48.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/__init__.py
+-rw-rw-rw-   0        0        0     4179 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/__main__.py
+-rw-rw-rw-   0        0        0      633 2023-06-29 05:48:10.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/app_config.py
+-rw-rw-rw-   0        0        0     3550 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/model.py
+-rw-rw-rw-   0        0        0     4256 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/program.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.804748 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/
+-rw-rw-rw-   0        0        0     4784 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      235 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.1.1/LICENSE` & `wad2023-program-1.1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.1.1/PKG-INFO` & `wad2023-program-1.1.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.1.1
+Version: 1.1.1.dev0
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wad2023-program-1.1.1/README.md` & `wad2023-program-1.1.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.1.1/pyproject.toml` & `wad2023-program-1.1.1.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "wad2023-program"
-version = "1.1.1"
+version = "1.1.1-dev"
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
-current_version = "1.1.1"
+current_version = "1.1.1-dev"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `wad2023-program-1.1.1/src/wad2023_program/__main__.py` & `wad2023-program-1.1.1.dev0/src/wad2023_program/__main__.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.1.1/src/wad2023_program/app_config.py` & `wad2023-program-1.1.1.dev0/src/wad2023_program/app_config.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.1.1/src/wad2023_program/model.py` & `wad2023-program-1.1.1.dev0/src/wad2023_program/model.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.1.1/src/wad2023_program/program.py` & `wad2023-program-1.1.1.dev0/src/wad2023_program/program.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.1.1/src/wad2023_program.egg-info/PKG-INFO` & `wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.1.1
+Version: 1.1.1.dev0
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

