# Comparing `tmp/wad2023-program-1.0.0.tar.gz` & `tmp/wad2023-program-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.0.0.tar", last modified: Thu Jun 29 06:13:07 2023, max compression
+gzip compressed data, was "wad2023-program-1.1.0.tar", last modified: Thu Jun 29 06:07:24 2023, max compression
```

## Comparing `wad2023-program-1.0.0.tar` & `wad2023-program-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:13:07.066370 wad2023-program-1.0.0/
--rw-rw-rw-   0        0        0      419 2023-06-29 06:13:07.065374 wad2023-program-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2023-06-29 06:12:36.000000 wad2023-program-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 06:13:07.068369 wad2023-program-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 06:13:06.999372 wad2023-program-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 06:13:07.031375 wad2023-program-1.0.0/src/wad2023_program/
--rw-rw-rw-   0        0        0      174 2023-06-29 06:12:36.000000 wad2023-program-1.0.0/src/wad2023_program/__init__.py
--rw-rw-rw-   0        0        0     3103 2023-06-29 06:12:36.000000 wad2023-program-1.0.0/src/wad2023_program/__main__.py
--rw-rw-rw-   0        0        0      633 2023-06-29 05:48:10.000000 wad2023-program-1.0.0/src/wad2023_program/app_config.py
--rw-rw-rw-   0        0        0     2411 2023-06-29 06:12:36.000000 wad2023-program-1.0.0/src/wad2023_program/model.py
--rw-rw-rw-   0        0        0     3867 2023-06-29 06:12:36.000000 wad2023-program-1.0.0/src/wad2023_program/program.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:13:07.061369 wad2023-program-1.0.0/src/wad2023_program.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-29 06:13:06.000000 wad2023-program-1.0.0/src/wad2023_program.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-06-29 06:13:06.000000 wad2023-program-1.0.0/src/wad2023_program.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:13:06.000000 wad2023-program-1.0.0/src/wad2023_program.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-29 06:13:06.000000 wad2023-program-1.0.0/src/wad2023_program.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      222 2023-06-29 06:13:06.000000 wad2023-program-1.0.0/src/wad2023_program.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 06:13:06.000000 wad2023-program-1.0.0/src/wad2023_program.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 06:07:24.017146 wad2023-program-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 06:04:36.000000 wad2023-program-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4779 2023-06-29 06:07:24.013149 wad2023-program-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-06-29 06:04:36.000000 wad2023-program-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1619 2023-06-29 06:05:04.000000 wad2023-program-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 06:07:24.018142 wad2023-program-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 06:07:23.862146 wad2023-program-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 06:07:23.966145 wad2023-program-1.1.0/src/wad2023_program/
+-rw-rw-rw-   0        0        0      174 2023-06-29 06:05:04.000000 wad2023-program-1.1.0/src/wad2023_program/__init__.py
+-rw-rw-rw-   0        0        0     4179 2023-06-29 06:04:36.000000 wad2023-program-1.1.0/src/wad2023_program/__main__.py
+-rw-rw-rw-   0        0        0      633 2023-06-29 05:48:10.000000 wad2023-program-1.1.0/src/wad2023_program/app_config.py
+-rw-rw-rw-   0        0        0     3550 2023-06-29 06:04:36.000000 wad2023-program-1.1.0/src/wad2023_program/model.py
+-rw-rw-rw-   0        0        0     4256 2023-06-29 06:04:36.000000 wad2023-program-1.1.0/src/wad2023_program/program.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:07:24.006142 wad2023-program-1.1.0/src/wad2023_program.egg-info/
+-rw-rw-rw-   0        0        0     4779 2023-06-29 06:07:23.000000 wad2023-program-1.1.0/src/wad2023_program.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-29 06:07:23.000000 wad2023-program-1.1.0/src/wad2023_program.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:07:23.000000 wad2023-program-1.1.0/src/wad2023_program.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-29 06:07:23.000000 wad2023-program-1.1.0/src/wad2023_program.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      222 2023-06-29 06:07:23.000000 wad2023-program-1.1.0/src/wad2023_program.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-29 06:07:23.000000 wad2023-program-1.1.0/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.0.0/pyproject.toml` & `wad2023-program-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ['setuptools>=61.1.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "wad2023-program"
-version = "1.0.0"
+version = "1.1.0"
 description = "Script to retrieve the program for WeAreDevelopers 2023 conference"
 readme = "README.md"
 authors = [{ name = "Daryl Stark", email = "daryl@dstark.nl" }]
-#license = { file = "LICENSE" } # License is not figured out yet
+license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["conference", "program", "wearedevelopers", "wearedevs"]
 dependencies = [
     "requests >= 2.27.0",
@@ -31,19 +31,23 @@
     'autopep8 == 2.0.0',
     'pylint == 2.17.0',
     'mypy == 1.3.0',
     'flake8 == 6.0.0',
     'pydocstyle == 6.3.0',
 ]
 
+[project.urls]
+homepage = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
+repository = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
+
 [project.scripts]
 wad23 = "wad2023_program.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `wad2023-program-1.0.0/src/wad2023_program/app_config.py` & `wad2023-program-1.1.0/src/wad2023_program/app_config.py`

 * *Files identical despite different names*

### Comparing `wad2023-program-1.0.0/src/wad2023_program/program.py` & `wad2023-program-1.1.0/src/wad2023_program/program.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module with program functions.
 
 Module that contains all functions to retrieve and parse the program.
 """
 
-from os.path import expanduser
+from os.path import dirname, expanduser
+from pathlib import Path
 
 import requests
 from bs4 import BeautifulSoup
 from dateutil import parser
 
 from .app_config import AppConfig
 from .model import Session, Speaker, Stage
@@ -104,25 +105,37 @@
 
         # Append the session to the list
         conference_session_list.append(session_object)
 
     return conference_session_list
 
 
-def get_program() -> list[Session]:
+def get_program(cache: bool = True) -> list[Session]:
     """Get the program.
 
     Retrieves the program from cache or, if that fails, from the web and
     returns it parsed.
 
+    Args:
+        cache: specify if the page can be retrieved from cache.
+
     Returns:
         The parsed program.
     """
     try:
+        if not cache:
+            raise FileNotFoundError
         program = get_program_from_cache()
     except FileNotFoundError:
         program = download_program()
-        with open(expanduser(config.cache_file),
+
+        # Create cache directory
+        cache_file = expanduser(config.cache_file)
+        directory = dirname(cache_file)
+        Path(directory).mkdir(parents=True, exist_ok=True)
+
+        # Write to cache
+        with open(cache_file,
                   'w',
                   encoding='utf-16') as cache_file_handle:
             cache_file_handle.write(str(program))
     return parse_program(program)
```

