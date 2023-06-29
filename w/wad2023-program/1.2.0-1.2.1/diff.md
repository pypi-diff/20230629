# Comparing `tmp/wad2023-program-1.2.0.tar.gz` & `tmp/wad2023-program-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.2.0.tar", last modified: Thu Jun 29 19:26:43 2023, max compression
+gzip compressed data, was "wad2023-program-1.2.1.tar", last modified: Thu Jun 29 19:35:02 2023, max compression
```

## Comparing `wad2023-program-1.2.0.tar` & `wad2023-program-1.2.1.tar`

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
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.981096 wad2023-program-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.981096 wad2023-program-1.2.1/src/wad2023_program/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-29 19:34:52.000000 wad2023-program-1.2.1/src/wad2023_program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:02.985097 wad2023-program-1.2.1/src/wad2023_program.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 19:35:02.000000 wad2023-program-1.2.1/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.2.0/LICENSE` & `wad2023-program-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/PKG-INFO` & `wad2023-program-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.2.0
+Version: 1.2.1
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,16 +52,17 @@
 After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
 
 The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
 
 -   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
 -   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
 -   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
+-   `--in-description=<text>`: shows only sessions with a specific word in the description field.
 -   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
--   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
+-   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), `csv` for CSV output or `details` for detailed output. The detailed output will also display the description.
 -   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
 
 ## Configuration
 
 There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
 
 -   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
```

### Comparing `wad2023-program-1.2.0/README.md` & `wad2023-program-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
 
 The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
 
 -   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
 -   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
 -   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
+-   `--in-description=<text>`: shows only sessions with a specific word in the description field.
 -   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
--   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
+-   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), `csv` for CSV output or `details` for detailed output. The detailed output will also display the description.
 -   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
 
 ## Configuration
 
 There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
 
 -   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
```

### Comparing `wad2023-program-1.2.0/pyproject.toml` & `wad2023-program-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "wad2023-program"
-version = "1.2.0"
+version = "1.2.1"
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
+current_version = "1.2.1"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `wad2023-program-1.2.0/src/wad2023_program/__main__.py` & `wad2023-program-1.2.1/src/wad2023_program/__main__.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program/app_config.py` & `wad2023-program-1.2.1/src/wad2023_program/app_config.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program/model.py` & `wad2023-program-1.2.1/src/wad2023_program/model.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program/program.py` & `wad2023-program-1.2.1/src/wad2023_program/program.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.2.0/src/wad2023_program.egg-info/PKG-INFO` & `wad2023-program-1.2.1/src/wad2023_program.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wad2023-program
-Version: 1.2.0
+Version: 1.2.1
 Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
 Author-email: Daryl Stark <daryl@dstark.nl>
 License: MIT License
         
         Copyright (c) 2023 Daryl Stark
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -52,16 +52,17 @@
 After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
 
 The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
 
 -   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
 -   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
 -   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
+-   `--in-description=<text>`: shows only sessions with a specific word in the description field.
 -   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
--   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
+-   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), `csv` for CSV output or `details` for detailed output. The detailed output will also display the description.
 -   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
 
 ## Configuration
 
 There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
 
 -   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
```

