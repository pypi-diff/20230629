# Comparing `tmp/wad2023-program-1.1.1.dev0.tar.gz` & `tmp/wad2023-program-1.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wad2023-program-1.1.1.dev0.tar", last modified: Thu Jun 29 06:21:29 2023, max compression
+gzip compressed data, was "wad2023-program-1.2.0.dev0.tar", last modified: Thu Jun 29 18:59:21 2023, max compression
```

## Comparing `wad2023-program-1.1.1.dev0.tar` & `wad2023-program-1.2.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.818737 wad2023-program-1.1.1.dev0/
--rw-rw-rw-   0        0        0     1089 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/LICENSE
--rw-rw-rw-   0        0        0     4784 2023-06-29 06:21:29.811728 wad2023-program-1.1.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2897 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/README.md
--rw-rw-rw-   0        0        0     1650 2023-06-29 06:19:31.000000 wad2023-program-1.1.1.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 06:21:29.820732 wad2023-program-1.1.1.dev0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.691730 wad2023-program-1.1.1.dev0/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.758730 wad2023-program-1.1.1.dev0/src/wad2023_program/
--rw-rw-rw-   0        0        0      178 2023-06-29 06:18:48.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/__init__.py
--rw-rw-rw-   0        0        0     4179 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/__main__.py
--rw-rw-rw-   0        0        0      633 2023-06-29 05:48:10.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/app_config.py
--rw-rw-rw-   0        0        0     3550 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/model.py
--rw-rw-rw-   0        0        0     4256 2023-06-29 06:18:23.000000 wad2023-program-1.1.1.dev0/src/wad2023_program/program.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:21:29.804748 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/
--rw-rw-rw-   0        0        0     4784 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      235 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 06:21:29.000000 wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/top_level.txt
+drwxrwxr-x   0 dast      (1000) dast      (1000)        0 2023-06-29 18:59:21.461015 wad2023-program-1.2.0.dev0/
+-rw-rw-r--   0 dast      (1000) dast      (1000)     1068 2023-06-29 17:58:47.000000 wad2023-program-1.2.0.dev0/LICENSE
+-rw-rw-r--   0 dast      (1000) dast      (1000)     4715 2023-06-29 18:59:21.461015 wad2023-program-1.2.0.dev0/PKG-INFO
+-rw-rw-r--   0 dast      (1000) dast      (1000)     2866 2023-06-29 17:58:47.000000 wad2023-program-1.2.0.dev0/README.md
+-rw-rw-r--   0 dast      (1000) dast      (1000)     1589 2023-06-29 18:11:46.000000 wad2023-program-1.2.0.dev0/pyproject.toml
+-rw-rw-r--   0 dast      (1000) dast      (1000)       38 2023-06-29 18:59:21.461015 wad2023-program-1.2.0.dev0/setup.cfg
+drwxrwxr-x   0 dast      (1000) dast      (1000)        0 2023-06-29 18:59:21.461015 wad2023-program-1.2.0.dev0/src/
+drwxrwxr-x   0 dast      (1000) dast      (1000)        0 2023-06-29 18:59:21.461015 wad2023-program-1.2.0.dev0/src/wad2023_program/
+-rw-rw-r--   0 dast      (1000) dast      (1000)      172 2023-06-29 18:11:46.000000 wad2023-program-1.2.0.dev0/src/wad2023_program/__init__.py
+-rw-rw-r--   0 dast      (1000) dast      (1000)     5128 2023-06-29 18:57:32.000000 wad2023-program-1.2.0.dev0/src/wad2023_program/__main__.py
+-rw-rw-r--   0 dast      (1000) dast      (1000)      612 2023-06-29 17:58:47.000000 wad2023-program-1.2.0.dev0/src/wad2023_program/app_config.py
+-rw-rw-r--   0 dast      (1000) dast      (1000)     3438 2023-06-29 18:28:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program/model.py
+-rw-rw-r--   0 dast      (1000) dast      (1000)     4356 2023-06-29 18:28:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program/program.py
+drwxrwxr-x   0 dast      (1000) dast      (1000)        0 2023-06-29 18:59:21.461015 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/
+-rw-rw-r--   0 dast      (1000) dast      (1000)     4715 2023-06-29 18:59:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/PKG-INFO
+-rw-rw-r--   0 dast      (1000) dast      (1000)      450 2023-06-29 18:59:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/SOURCES.txt
+-rw-rw-r--   0 dast      (1000) dast      (1000)        1 2023-06-29 18:59:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/dependency_links.txt
+-rw-rw-r--   0 dast      (1000) dast      (1000)       56 2023-06-29 18:59:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/entry_points.txt
+-rw-rw-r--   0 dast      (1000) dast      (1000)      235 2023-06-29 18:59:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/requires.txt
+-rw-rw-r--   0 dast      (1000) dast      (1000)       16 2023-06-29 18:59:21.000000 wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/top_level.txt
```

### Comparing `wad2023-program-1.1.1.dev0/PKG-INFO` & `wad2023-program-1.2.0.dev0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1
-Name: wad2023-program
-Version: 1.1.1.dev0
-Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
-Author-email: Daryl Stark <daryl@dstark.nl>
-License: MIT License
-        
-        Copyright (c) 2023 Daryl Stark
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://github.com/DarylStark/WeAreDevelopers_2023_Program
-Project-URL: repository, https://github.com/DarylStark/WeAreDevelopers_2023_Program
-Keywords: conference,program,wearedevelopers,wearedevs
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# WeAreDevelopers 2023 - Program CLI
-
-In less then a month, the [WeAreDevelopers 2023](https://www.wearedevelopers.com/world-congress) conference is finally starting! Two days of being with like-minded people, talking about code and infrastructure! If you're like me, you're very excited about this, but a bit overwhelmed by the 236 session that are planned. It's difficult to pick the sessions that are right for me. The [programpage](https://www.wearedevelopers.com/world-congress/program) on the website is not really to my liking, so I decided to create a small CLI script to browse through the sessions.
-
-# Installation
-
-Installation can be done using `pip`:
-
-```bash
-pip install wad2023-program
-```
-
-## Usage
-
-After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
-
-The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
-
--   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
--   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
--   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
--   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
--   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
--   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
-
-## Configuration
-
-There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
-
--   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
--   `PROGRAM_URL`: specifies where to download the program from. Default: `https://sessionize.com/api/v2/tx3wi18f/view/Sessions`
--   `PROGRAM_PARAMS`: dictionary that sets specific parameters to the web URL. Default: `dict = {'under': True}`
+Metadata-Version: 2.1
+Name: wad2023-program
+Version: 1.2.0.dev0
+Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
+Author-email: Daryl Stark <daryl@dstark.nl>
+License: MIT License
+        
+        Copyright (c) 2023 Daryl Stark
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/DarylStark/WeAreDevelopers_2023_Program
+Project-URL: repository, https://github.com/DarylStark/WeAreDevelopers_2023_Program
+Keywords: conference,program,wearedevelopers,wearedevs
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# WeAreDevelopers 2023 - Program CLI
+
+In less then a month, the [WeAreDevelopers 2023](https://www.wearedevelopers.com/world-congress) conference is finally starting! Two days of being with like-minded people, talking about code and infrastructure! If you're like me, you're very excited about this, but a bit overwhelmed by the 236 session that are planned. It's difficult to pick the sessions that are right for me. The [programpage](https://www.wearedevelopers.com/world-congress/program) on the website is not really to my liking, so I decided to create a small CLI script to browse through the sessions.
+
+# Installation
+
+Installation can be done using `pip`:
+
+```bash
+pip install wad2023-program
+```
+
+## Usage
+
+After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
+
+The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
+
+-   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
+-   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
+-   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
+-   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
+-   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
+-   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
+
+## Configuration
+
+There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
+
+-   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
+-   `PROGRAM_URL`: specifies where to download the program from. Default: `https://sessionize.com/api/v2/tx3wi18f/view/Sessions`
+-   `PROGRAM_PARAMS`: dictionary that sets specific parameters to the web URL. Default: `dict = {'under': True}`
```

### Comparing `wad2023-program-1.1.1.dev0/README.md` & `wad2023-program-1.2.0.dev0/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# WeAreDevelopers 2023 - Program CLI
-
-In less then a month, the [WeAreDevelopers 2023](https://www.wearedevelopers.com/world-congress) conference is finally starting! Two days of being with like-minded people, talking about code and infrastructure! If you're like me, you're very excited about this, but a bit overwhelmed by the 236 session that are planned. It's difficult to pick the sessions that are right for me. The [programpage](https://www.wearedevelopers.com/world-congress/program) on the website is not really to my liking, so I decided to create a small CLI script to browse through the sessions.
-
-# Installation
-
-Installation can be done using `pip`:
-
-```bash
-pip install wad2023-program
-```
-
-## Usage
-
-After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
-
-The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
-
--   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
--   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
--   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
--   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
--   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
--   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
-
-## Configuration
-
-There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
-
--   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
--   `PROGRAM_URL`: specifies where to download the program from. Default: `https://sessionize.com/api/v2/tx3wi18f/view/Sessions`
+# WeAreDevelopers 2023 - Program CLI
+
+In less then a month, the [WeAreDevelopers 2023](https://www.wearedevelopers.com/world-congress) conference is finally starting! Two days of being with like-minded people, talking about code and infrastructure! If you're like me, you're very excited about this, but a bit overwhelmed by the 236 session that are planned. It's difficult to pick the sessions that are right for me. The [programpage](https://www.wearedevelopers.com/world-congress/program) on the website is not really to my liking, so I decided to create a small CLI script to browse through the sessions.
+
+# Installation
+
+Installation can be done using `pip`:
+
+```bash
+pip install wad2023-program
+```
+
+## Usage
+
+After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
+
+The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
+
+-   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
+-   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
+-   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
+-   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
+-   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
+-   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
+
+## Configuration
+
+There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
+
+-   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
+-   `PROGRAM_URL`: specifies where to download the program from. Default: `https://sessionize.com/api/v2/tx3wi18f/view/Sessions`
 -   `PROGRAM_PARAMS`: dictionary that sets specific parameters to the web URL. Default: `dict = {'under': True}`
```

### Comparing `wad2023-program-1.1.1.dev0/pyproject.toml` & `wad2023-program-1.2.0.dev0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-[build-system]
-requires = ['setuptools>=61.1.0', 'wheel']
-build-backend = 'setuptools.build_meta'
-
-[project]
-name = "wad2023-program"
-version = "1.1.1-dev"
-description = "Script to retrieve the program for WeAreDevelopers 2023 conference"
-readme = "README.md"
-authors = [{ name = "Daryl Stark", email = "daryl@dstark.nl" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-keywords = ["conference", "program", "wearedevelopers", "wearedevs"]
-dependencies = [
-    "requests >= 2.27.0",
-    "pydantic >= 1.10.0",
-    "beautifulsoup4 >= 4.12.0",
-    "python-dateutil >= 2.8.0",
-    "rich >= 13.4.0",
-    "typer >= 0.9.0",
-    "pytz >= 2023.3"
-]
-requires-python = ">=3.9"
-
-[project.optional-dependencies]
-dev = [
-    'pytest >= 7.3.0',
-    'pycodestyle == 2.10.0',
-    'autopep8 == 2.0.0',
-    'pylint == 2.17.0',
-    'mypy == 1.3.0',
-    'flake8 == 6.0.0',
-    'pydocstyle == 6.3.0',
-]
-
-[project.urls]
-homepage = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
-repository = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
-
-[project.scripts]
-wad23 = "wad2023_program.__main__:main"
-
-[tool.bumpver]
-current_version = "1.1.1-dev"
-version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
-commit_message = "Version {new_version}"
-commit = true
-tag = false
-push = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/wad2023_program/__init__.py" = ["{version}"]
-
-[tool.pytest.ini_options]
-pythonpath = "./src/"
-testpaths = [
-    "tests"
+[build-system]
+requires = ['setuptools>=61.1.0', 'wheel']
+build-backend = 'setuptools.build_meta'
+
+[project]
+name = "wad2023-program"
+version = "1.2.0-dev"
+description = "Script to retrieve the program for WeAreDevelopers 2023 conference"
+readme = "README.md"
+authors = [{ name = "Daryl Stark", email = "daryl@dstark.nl" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["conference", "program", "wearedevelopers", "wearedevs"]
+dependencies = [
+    "requests >= 2.27.0",
+    "pydantic >= 1.10.0",
+    "beautifulsoup4 >= 4.12.0",
+    "python-dateutil >= 2.8.0",
+    "rich >= 13.4.0",
+    "typer >= 0.9.0",
+    "pytz >= 2023.3"
+]
+requires-python = ">=3.9"
+
+[project.optional-dependencies]
+dev = [
+    'pytest >= 7.3.0',
+    'pycodestyle == 2.10.0',
+    'autopep8 == 2.0.0',
+    'pylint == 2.17.0',
+    'mypy == 1.3.0',
+    'flake8 == 6.0.0',
+    'pydocstyle == 6.3.0',
+]
+
+[project.urls]
+homepage = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
+repository = "https://github.com/DarylStark/WeAreDevelopers_2023_Program"
+
+[project.scripts]
+wad23 = "wad2023_program.__main__:main"
+
+[tool.bumpver]
+current_version = "1.2.0-dev"
+version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
+commit_message = "Version {new_version}"
+commit = true
+tag = false
+push = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
+"src/wad2023_program/__init__.py" = ["{version}"]
+
+[tool.pytest.ini_options]
+pythonpath = "./src/"
+testpaths = [
+    "tests"
 ]
```

### Comparing `wad2023-program-1.1.1.dev0/src/wad2023_program/app_config.py` & `wad2023-program-1.2.0.dev0/src/wad2023_program/app_config.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Module with the config model.
-
-Contains the model for the configuration of the application.
-"""
-from pydantic import BaseSettings
-
-
-class AppConfig(BaseSettings):
-    """Application config model.
-
-    Class with the attributes for the configuration of the application.
-
-    Attributes:
-        cache_file: the location for the cache file.
-        program_url: the URL for the program.
-        program_params: the params for the URL.
-    """
-
-    cache_file: str = '~/.cache/program.html'
-    program_url: str = 'https://sessionize.com/api/v2/tx3wi18f/view/Sessions'
-    program_params: dict = {'under': True}
+"""Module with the config model.
+
+Contains the model for the configuration of the application.
+"""
+from pydantic import BaseSettings
+
+
+class AppConfig(BaseSettings):
+    """Application config model.
+
+    Class with the attributes for the configuration of the application.
+
+    Attributes:
+        cache_file: the location for the cache file.
+        program_url: the URL for the program.
+        program_params: the params for the URL.
+    """
+
+    cache_file: str = '~/.cache/program.html'
+    program_url: str = 'https://sessionize.com/api/v2/tx3wi18f/view/Sessions'
+    program_params: dict = {'under': True}
```

### Comparing `wad2023-program-1.1.1.dev0/src/wad2023_program/model.py` & `wad2023-program-1.2.0.dev0/src/wad2023_program/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,139 @@
-"""Model module.
-
-Contains the models for the application.
-"""
-import re
-from datetime import datetime
-
-import pytz
-from pydantic import BaseModel
-
-
-def to_timezone(datetime_utc: datetime, timezone: str) -> datetime:
-    """Convert a UTC time to a specific timezone.
-
-    Args:
-        datetime_utc: the datetime object to convert.
-        timezone: the timezone to convert to. Example: "Europe/Amsterdam.
-
-    Returns:
-        A datetime-object with the time in the set Timezone.
-    """
-    new_timezone = pytz.timezone(timezone)
-    return datetime_utc.replace(tzinfo=pytz.utc).astimezone(tz=new_timezone)
-
-
-class Model(BaseModel):
-    """Base model for all models.
-
-    Contains the main attributes for Model classes.
-    """
-
-    class Config:
-        """Config for the models.
-
-        Attributes:
-            validate_assignment: specifies if assigned values should be
-                validated by Pydantic. If this is set to False, only
-                assignments in the constructor are validated.
-        """
-
-        validate_assignment = True
-
-
-class Speaker(Model):
-    """Model for a speaker.
-
-    Class with the attributes for a speaker.
-
-    Attributes:
-        uid: the ID of the speaker.
-        name: the name of the speaker.
-    """
-
-    uid: str
-    name: str
-
-
-class Stage(Model):
-    """Model for a stage.
-
-    Class with the attributes for a stage.
-
-    Attributes:
-        uid: the ID of the stage.
-        name: the name of the stage.
-    """
-
-    id: int = 0
-    name: str = ''
-
-
-class Session(Model):
-    """Model for a session.
-
-    Class with the attributes for a session.
-
-    Attributes:
-        title: the title of the session.
-        stage: the stage where the session is hold.
-        speakers: a list with speakers for the session.
-        start_time: when the session starts.
-        end_time: when the session ends
-        tags: a list with tags.
-    """
-
-    title: str = ''
-    stage: Stage = Stage()
-    speakers: list[Speaker] = []
-    start_time: datetime = datetime.now()
-    end_time: datetime = datetime.now()
-    tags: list[str] = []
-
-    @property
-    def speaker(self) -> str:
-        """Get the speaker name.
-
-        Returns the speaker name as a string. Can be useful when sorting a list
-        of sessions.
-
-        Returns:
-            The speaker name as a string.
-        """
-        return ', '.join([speaker.name for speaker in self.speakers])
-
-    @property
-    def stage_name(self) -> str:
-        """Get the stage name.
-
-        Returns the name of the stage as a string. The API for the program adds
-        a number to the stage. We filter this out.
-
-        Returns:
-            The name of the stage.
-        """
-        stage_name = re.findall(r'^[A-Za-z0-9\ ]+', self.stage.name)
-        return stage_name[0].strip()
-
-    @property
-    def start_time_berlin(self) -> datetime:
-        """Get the start time in Berlin timezone.
-
-        Returns the start time in Berlin timezone instead of UTC.
-
-        Returns:
-            The start time in Berlin timezone.
-        """
-        return to_timezone(self.start_time, "Europe/Amsterdam")
-
-    @property
-    def end_time_berlin(self) -> datetime:
-        """Get the end time in Berlin timezone.
-
-        Returns the end time in Berlin timezone instead of UTC.
-
-        Returns:
-            The end time in Berlin timezone.
-        """
-        return to_timezone(self.end_time, "Europe/Amsterdam")
+"""Model module.
+
+Contains the models for the application.
+"""
+import re
+from datetime import datetime
+
+import pytz
+from pydantic import BaseModel
+
+
+def to_timezone(datetime_utc: datetime, timezone: str) -> datetime:
+    """Convert a UTC time to a specific timezone.
+
+    Args:
+        datetime_utc: the datetime object to convert.
+        timezone: the timezone to convert to. Example: "Europe/Amsterdam.
+
+    Returns:
+        A datetime-object with the time in the set Timezone.
+    """
+    new_timezone = pytz.timezone(timezone)
+    return datetime_utc.replace(tzinfo=pytz.utc).astimezone(tz=new_timezone)
+
+
+class Model(BaseModel):
+    """Base model for all models.
+
+    Contains the main attributes for Model classes.
+    """
+
+    class Config:
+        """Config for the models.
+
+        Attributes:
+            validate_assignment: specifies if assigned values should be
+                validated by Pydantic. If this is set to False, only
+                assignments in the constructor are validated.
+        """
+
+        validate_assignment = True
+
+
+class Speaker(Model):
+    """Model for a speaker.
+
+    Class with the attributes for a speaker.
+
+    Attributes:
+        uid: the ID of the speaker.
+        name: the name of the speaker.
+    """
+
+    uid: str
+    name: str
+
+
+class Stage(Model):
+    """Model for a stage.
+
+    Class with the attributes for a stage.
+
+    Attributes:
+        uid: the ID of the stage.
+        name: the name of the stage.
+    """
+
+    id: int = 0
+    name: str = ''
+
+
+class Session(Model):
+    """Model for a session.
+
+    Class with the attributes for a session.
+
+    Attributes:
+        title: the title of the session.
+        stage: the stage where the session is hold.
+        speakers: a list with speakers for the session.
+        start_time: when the session starts.
+        end_time: when the session ends
+        tags: a list with tags.
+    """
+
+    title: str = ''
+    stage: Stage = Stage()
+    speakers: list[Speaker] = []
+    start_time: datetime = datetime.now()
+    end_time: datetime = datetime.now()
+    tags: list[str] = []
+    description: str = ''
+
+    @property
+    def speaker(self) -> str:
+        """Get the speaker name.
+
+        Returns the speaker name as a string. Can be useful when sorting a list
+        of sessions.
+
+        Returns:
+            The speaker name as a string.
+        """
+        return ', '.join([speaker.name for speaker in self.speakers])
+
+    @property
+    def stage_name(self) -> str:
+        """Get the stage name.
+
+        Returns the name of the stage as a string. The API for the program adds
+        a number to the stage. We filter this out.
+
+        Returns:
+            The name of the stage.
+        """
+        stage_name = re.findall(r'^[A-Za-z0-9\ ]+', self.stage.name)
+        return stage_name[0].strip()
+
+    @property
+    def start_time_berlin(self) -> datetime:
+        """Get the start time in Berlin timezone.
+
+        Returns the start time in Berlin timezone instead of UTC.
+
+        Returns:
+            The start time in Berlin timezone.
+        """
+        return to_timezone(self.start_time, "Europe/Amsterdam")
+
+    @property
+    def end_time_berlin(self) -> datetime:
+        """Get the end time in Berlin timezone.
+
+        Returns the end time in Berlin timezone instead of UTC.
+
+        Returns:
+            The end time in Berlin timezone.
+        """
+        return to_timezone(self.end_time, "Europe/Amsterdam")
```

### Comparing `wad2023-program-1.1.1.dev0/src/wad2023_program/program.py` & `wad2023-program-1.2.0.dev0/src/wad2023_program/program.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,141 +1,147 @@
-"""Module with program functions.
-
-Module that contains all functions to retrieve and parse the program.
-"""
-
-from os.path import dirname, expanduser
-from pathlib import Path
-
-import requests
-from bs4 import BeautifulSoup
-from dateutil import parser
-
-from .app_config import AppConfig
-from .model import Session, Speaker, Stage
-
-# Configuration
-config = AppConfig()
-
-
-def get_program_from_cache() -> str:
-    """Get program from cache file.
-
-    Retrieves the program from the saved cache file.
-
-    Returns:
-        The HTML for the program in the cache file.
-    """
-    with open(expanduser(config.cache_file),
-              'r',
-              encoding='utf-16') as cache_file_handle:
-        return cache_file_handle.read()
-
-
-def download_program() -> str:
-    """Get program from the web.
-
-    Retrieves the program from the web URL.
-
-    Returns:
-        The HTML for the program on the web.
-
-    Raises:
-        ValueError: when a wrong status code is returned.
-    """
-    program_request = requests.get(
-        url=config.program_url,
-        params=config.program_params,
-        timeout=10)
-    if program_request.status_code != 200:
-        raise ValueError(
-            ('Did not receive responsecode 200; got ' +
-             f'responsecode {program_request.status_code}'))
-    return program_request.text
-
-
-def parse_program(program_html: str) -> list[Session]:
-    """Parse the HTML for the program.
-
-    Parses the program from the HTML returned by the webpage or from the cache.
-
-    Args:
-        program_html: the HTML from cache or from the web that contains the
-            program.
-
-    Returns:
-        A list with all Sessions.
-    """
-    # Empty session list
-    conference_session_list: list[Session] = []
-
-    # Parse the HTML
-    soup = BeautifulSoup(program_html, 'html.parser')
-    session_list = soup.find_all('ul', {'class': 'sz-sessions--list'})
-    sessions = session_list[0].find_all('li', {'class': 'sz-session--full'})
-
-    # Loop through the session and create the correct objects
-    for session in sessions:
-        # Create a new session object
-        session_object = Session()
-
-        # Get the title
-        session_object.title = session.find_all('h3')[0].text.strip()
-
-        # Get the stage
-        stage = session.find_all('div', {'class': 'sz-session__room'})[0]
-        session_object.stage = Stage(
-            id=stage['data-roomid'],
-            name=stage.text
-        )
-
-        # Get the speakers
-        speakers = session.find_all('ul', {'class': 'sz-session__speakers'})
-        for speaker in speakers[0].find_all('li'):
-            speaker_object = Speaker(
-                uid=speaker['data-speakerid'],
-                name=speaker.text.strip())
-            session_object.speakers.append(speaker_object)
-
-        # Get the session times
-        session_time = session.find_all(
-            'div', {'class': 'sz-session__time'})[0]
-        time_attribute = session_time['data-sztz'].split('|')
-        session_object.start_time = parser.parse(time_attribute[2])
-        session_object.end_time = parser.parse(time_attribute[3])
-
-        # Append the session to the list
-        conference_session_list.append(session_object)
-
-    return conference_session_list
-
-
-def get_program(cache: bool = True) -> list[Session]:
-    """Get the program.
-
-    Retrieves the program from cache or, if that fails, from the web and
-    returns it parsed.
-
-    Args:
-        cache: specify if the page can be retrieved from cache.
-
-    Returns:
-        The parsed program.
-    """
-    try:
-        if not cache:
-            raise FileNotFoundError
-        program = get_program_from_cache()
-    except FileNotFoundError:
-        program = download_program()
-
-        # Create cache directory
-        cache_file = expanduser(config.cache_file)
-        directory = dirname(cache_file)
-        Path(directory).mkdir(parents=True, exist_ok=True)
-
-        # Write to cache
-        with open(cache_file,
-                  'w',
-                  encoding='utf-16') as cache_file_handle:
-            cache_file_handle.write(str(program))
-    return parse_program(program)
+"""Module with program functions.
+
+Module that contains all functions to retrieve and parse the program.
+"""
+
+from os.path import dirname, expanduser
+from pathlib import Path
+
+import requests
+from bs4 import BeautifulSoup
+from dateutil import parser
+
+from .app_config import AppConfig
+from .model import Session, Speaker, Stage
+
+# Configuration
+config = AppConfig()
+
+
+def get_program_from_cache() -> str:
+    """Get program from cache file.
+
+    Retrieves the program from the saved cache file.
+
+    Returns:
+        The HTML for the program in the cache file.
+    """
+    with open(expanduser(config.cache_file),
+              'r',
+              encoding='utf-16') as cache_file_handle:
+        return cache_file_handle.read()
+
+
+def download_program() -> str:
+    """Get program from the web.
+
+    Retrieves the program from the web URL.
+
+    Returns:
+        The HTML for the program on the web.
+
+    Raises:
+        ValueError: when a wrong status code is returned.
+    """
+    program_request = requests.get(
+        url=config.program_url,
+        params=config.program_params,
+        timeout=10)
+    if program_request.status_code != 200:
+        raise ValueError(
+            ('Did not receive responsecode 200; got ' +
+             f'responsecode {program_request.status_code}'))
+    return program_request.text
+
+
+def parse_program(program_html: str) -> list[Session]:
+    """Parse the HTML for the program.
+
+    Parses the program from the HTML returned by the webpage or from the cache.
+
+    Args:
+        program_html: the HTML from cache or from the web that contains the
+            program.
+
+    Returns:
+        A list with all Sessions.
+    """
+    # Empty session list
+    conference_session_list: list[Session] = []
+
+    # Parse the HTML
+    soup = BeautifulSoup(program_html, 'html.parser')
+    session_list = soup.find_all('ul', {'class': 'sz-sessions--list'})
+    sessions = session_list[0].find_all('li', {'class': 'sz-session--full'})
+
+    # Loop through the session and create the correct objects
+    for session in sessions:
+        # Create a new session object
+        session_object = Session()
+
+        # Get the title
+        session_object.title = session.find_all('h3')[0].text.strip()
+
+        # Get the description
+        description_tag = session.find_all(
+            'p', {'class': 'sz-session__description'})
+        if len(description_tag) == 1:
+            session_object.description = description_tag[0].text.strip()
+
+        # Get the stage
+        stage = session.find_all('div', {'class': 'sz-session__room'})[0]
+        session_object.stage = Stage(
+            id=stage['data-roomid'],
+            name=stage.text
+        )
+
+        # Get the speakers
+        speakers = session.find_all('ul', {'class': 'sz-session__speakers'})
+        for speaker in speakers[0].find_all('li'):
+            speaker_object = Speaker(
+                uid=speaker['data-speakerid'],
+                name=speaker.text.strip())
+            session_object.speakers.append(speaker_object)
+
+        # Get the session times
+        session_time = session.find_all(
+            'div', {'class': 'sz-session__time'})[0]
+        time_attribute = session_time['data-sztz'].split('|')
+        session_object.start_time = parser.parse(time_attribute[2])
+        session_object.end_time = parser.parse(time_attribute[3])
+
+        # Append the session to the list
+        conference_session_list.append(session_object)
+
+    return conference_session_list
+
+
+def get_program(cache: bool = True) -> list[Session]:
+    """Get the program.
+
+    Retrieves the program from cache or, if that fails, from the web and
+    returns it parsed.
+
+    Args:
+        cache: specify if the page can be retrieved from cache.
+
+    Returns:
+        The parsed program.
+    """
+    try:
+        if not cache:
+            raise FileNotFoundError
+        program = get_program_from_cache()
+    except FileNotFoundError:
+        program = download_program()
+
+        # Create cache directory
+        cache_file = expanduser(config.cache_file)
+        directory = dirname(cache_file)
+        Path(directory).mkdir(parents=True, exist_ok=True)
+
+        # Write to cache
+        with open(cache_file,
+                  'w',
+                  encoding='utf-16') as cache_file_handle:
+            cache_file_handle.write(str(program))
+    return parse_program(program)
```

### Comparing `wad2023-program-1.1.1.dev0/src/wad2023_program.egg-info/PKG-INFO` & `wad2023-program-1.2.0.dev0/src/wad2023_program.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1
-Name: wad2023-program
-Version: 1.1.1.dev0
-Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
-Author-email: Daryl Stark <daryl@dstark.nl>
-License: MIT License
-        
-        Copyright (c) 2023 Daryl Stark
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://github.com/DarylStark/WeAreDevelopers_2023_Program
-Project-URL: repository, https://github.com/DarylStark/WeAreDevelopers_2023_Program
-Keywords: conference,program,wearedevelopers,wearedevs
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# WeAreDevelopers 2023 - Program CLI
-
-In less then a month, the [WeAreDevelopers 2023](https://www.wearedevelopers.com/world-congress) conference is finally starting! Two days of being with like-minded people, talking about code and infrastructure! If you're like me, you're very excited about this, but a bit overwhelmed by the 236 session that are planned. It's difficult to pick the sessions that are right for me. The [programpage](https://www.wearedevelopers.com/world-congress/program) on the website is not really to my liking, so I decided to create a small CLI script to browse through the sessions.
-
-# Installation
-
-Installation can be done using `pip`:
-
-```bash
-pip install wad2023-program
-```
-
-## Usage
-
-After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
-
-The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
-
--   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
--   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
--   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
--   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
--   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
--   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
-
-## Configuration
-
-There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
-
--   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
--   `PROGRAM_URL`: specifies where to download the program from. Default: `https://sessionize.com/api/v2/tx3wi18f/view/Sessions`
--   `PROGRAM_PARAMS`: dictionary that sets specific parameters to the web URL. Default: `dict = {'under': True}`
+Metadata-Version: 2.1
+Name: wad2023-program
+Version: 1.2.0.dev0
+Summary: Script to retrieve the program for WeAreDevelopers 2023 conference
+Author-email: Daryl Stark <daryl@dstark.nl>
+License: MIT License
+        
+        Copyright (c) 2023 Daryl Stark
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/DarylStark/WeAreDevelopers_2023_Program
+Project-URL: repository, https://github.com/DarylStark/WeAreDevelopers_2023_Program
+Keywords: conference,program,wearedevelopers,wearedevs
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# WeAreDevelopers 2023 - Program CLI
+
+In less then a month, the [WeAreDevelopers 2023](https://www.wearedevelopers.com/world-congress) conference is finally starting! Two days of being with like-minded people, talking about code and infrastructure! If you're like me, you're very excited about this, but a bit overwhelmed by the 236 session that are planned. It's difficult to pick the sessions that are right for me. The [programpage](https://www.wearedevelopers.com/world-congress/program) on the website is not really to my liking, so I decided to create a small CLI script to browse through the sessions.
+
+# Installation
+
+Installation can be done using `pip`:
+
+```bash
+pip install wad2023-program
+```
+
+## Usage
+
+After installing, the CLI script can be executed by executing the `wad23` command in your browser. By executing it without arguments, you get a complete list of all sessions. the first time you run the script, it will download these sessions from the program page (from [Sessionize](https://sessionize.com/api/v2/tx3wi18f/view/Sessions) to be precise) and save the page to your `.cache` folder in your homefolder (the folder will be created if it doesn't exist). All subsequent requests will be done using the cache the original page is not flooded with requests.
+
+The script has a few command line arguments you can use to sort and filter the list. You can use `--help` to see these. Here is a list of the command line options:
+
+-   `--sort=<sort_field>`: specify a field to sort on. Can be `start`, `end`, `title`, `speaker` or `stage`.
+-   `--in-title=<text>`: shows only session with a specific word in the title field. For example, the command line argument `--in-title=python` will only display sessions with the word Python in it.
+-   `--in-speaker=<text>`: shows only sessions with a specific word in the speaker field.
+-   `--stage=<stage_name>`: filters on stage. The stage has to match exactly, like `--stage="Stage 2"`, for instance.
+-   `--output=<output_format>`: let's you specify a output format. Can be either `table` (default), or `csv` for CSV output.
+-   `--cache` and `--no-cache`: specifies if the script should use the cache. By default, it uses the cache file, but if you want to skip that, you can specify `--no-cache`. Be warned though: do _not_ flood the webserver of Sessionize with requests!
+
+## Configuration
+
+There is not much to configure for the application, but there are a few configuration options you have. These configuration options are set with environment variables:
+
+-   `CACHE_FILE`: specifies where the cache file should be placed. Default: `~/.cache/program.html`
+-   `PROGRAM_URL`: specifies where to download the program from. Default: `https://sessionize.com/api/v2/tx3wi18f/view/Sessions`
+-   `PROGRAM_PARAMS`: dictionary that sets specific parameters to the web URL. Default: `dict = {'under': True}`
```

