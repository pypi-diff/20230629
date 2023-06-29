# Comparing `tmp/gorilla-cli-0.0.7.tar.gz` & `tmp/gorilla-cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gorilla-cli-0.0.7.tar", last modified: Thu Jun 29 16:38:05 2023, max compression
+gzip compressed data, was "gorilla-cli-0.0.8.tar", last modified: Thu Jun 29 18:03:12 2023, max compression
```

## Comparing `gorilla-cli-0.0.7.tar` & `gorilla-cli-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.299675 gorilla-cli-0.0.7/
--rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/LICENSE
--rw-r--r--   0 shishir    (501) staff       (20)     2425 2023-06-29 16:38:05.299183 gorilla-cli-0.0.7/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)     1919 2023-06-29 16:34:42.000000 gorilla-cli-0.0.7/README.md
--rw-r--r--   0 shishir    (501) staff       (20)     6799 2023-06-29 16:35:01.000000 gorilla-cli-0.0.7/go_cli.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.296116 gorilla-cli-0.0.7/go_questionary/
--rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/constants.py
--rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/form.py
--rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompt.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.298029 gorilla-cli-0.0.7/go_questionary/prompts/
--rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/autocomplete.py
--rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/checkbox.py
--rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/common.py
--rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/confirm.py
--rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/password.py
--rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/path.py
--rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/rawselect.py
--rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/select.py
--rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/text.py
--rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/question.py
--rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/utils.py
--rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/version.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.298902 gorilla-cli-0.0.7/gorilla_cli.egg-info/
--rw-r--r--   0 shishir    (501) staff       (20)     2425 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/SOURCES.txt
--rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/dependency_links.txt
--rw-r--r--   0 shishir    (501) staff       (20)       41 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/entry_points.txt
--rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/requires.txt
--rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/top_level.txt
--rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-29 16:38:05.299792 gorilla-cli-0.0.7/setup.cfg
--rw-r--r--   0 shishir    (501) staff       (20)     1507 2023-06-29 16:35:45.000000 gorilla-cli-0.0.7/setup.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.807590 gorilla-cli-0.0.8/
+-rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/LICENSE
+-rw-r--r--   0 shishir    (501) staff       (20)     2581 2023-06-29 18:03:12.807271 gorilla-cli-0.0.8/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)     2075 2023-06-29 17:39:11.000000 gorilla-cli-0.0.8/README.md
+-rw-r--r--   0 shishir    (501) staff       (20)     6804 2023-06-29 18:03:01.000000 gorilla-cli-0.0.8/go_cli.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.804568 gorilla-cli-0.0.8/go_questionary/
+-rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/constants.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/form.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompt.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.806196 gorilla-cli-0.0.8/go_questionary/prompts/
+-rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/autocomplete.py
+-rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/checkbox.py
+-rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/common.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/confirm.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/password.py
+-rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/path.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/rawselect.py
+-rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/select.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/text.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/question.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/utils.py
+-rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/version.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.807044 gorilla-cli-0.0.8/gorilla_cli.egg-info/
+-rw-r--r--   0 shishir    (501) staff       (20)     2581 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       41 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/entry_points.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/requires.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/top_level.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-29 18:03:12.807642 gorilla-cli-0.0.8/setup.cfg
+-rw-r--r--   0 shishir    (501) staff       (20)     1507 2023-06-29 18:02:23.000000 gorilla-cli-0.0.8/setup.py
```

### Comparing `gorilla-cli-0.0.7/LICENSE` & `gorilla-cli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/PKG-INFO` & `gorilla-cli-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: gorilla-cli
-Version: 0.0.7
-Summary: LLMs for CLI
-Home-page: https://github.com/gorilla-llm/gorilla-cli
-Author: Shishir Patil, Tianjun Zhang
-Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Gorilla CLI
 
 Gorilla CLI revolutionizes your command-line interactions with a user-centric tool that understands natural language commands. Simply state your objective, and Gorilla CLI will generate potential commands for execution. No more need to recall intricate command-line arguments!
 
 Developed by UC Berkeley as a research prototype, Gorilla-CLI prioritizes user control and confidentiality:
  - Commands are executed solely with your explicit approval.
  - While we utilize queries and error logs (stderr) for model enhancement, we NEVER collect output data (stdout).
@@ -28,22 +12,28 @@
 
 ```bash
 pip install gorilla-cli
 ```
 
 ## Usage
 
-Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
+Activate Gorilla CLI with a straightforward `gorilla` followed by your command in plain English.
 
 For instance, to list all files in the current directory, type:
 
 ```bash
 $ gorilla I want to list all files in the current directory
 ```
 
+or if you prefer, you can use quotes to avoid issues with string parsing:
+
+```bash
+$ gorilla "I want to list all files in the current directory" 
+```
+
 Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
    ls -l
    ls -al
@@ -56,9 +46,7 @@
 ## Contributions
 
 We welcome your enhancements to Gorilla CLI! If you have improvements, feel free to submit a pull request on our GitHub page. 
 
 ## License
 
 Gorilla CLI operates under the Apache 2.0 license. More details can be found in the LICENSE file. We'd also like to extend our appreciation to [questionary](https://github.com/tmbo/questionary) for their fantastic UI!
-
-
```

### Comparing `gorilla-cli-0.0.7/README.md` & `gorilla-cli-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: gorilla-cli
+Version: 0.0.8
+Summary: LLMs for CLI
+Home-page: https://github.com/gorilla-llm/gorilla-cli
+Author: Shishir Patil, Tianjun Zhang
+Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Gorilla CLI
 
 Gorilla CLI revolutionizes your command-line interactions with a user-centric tool that understands natural language commands. Simply state your objective, and Gorilla CLI will generate potential commands for execution. No more need to recall intricate command-line arguments!
 
 Developed by UC Berkeley as a research prototype, Gorilla-CLI prioritizes user control and confidentiality:
  - Commands are executed solely with your explicit approval.
  - While we utilize queries and error logs (stderr) for model enhancement, we NEVER collect output data (stdout).
@@ -12,22 +28,28 @@
 
 ```bash
 pip install gorilla-cli
 ```
 
 ## Usage
 
-Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
+Activate Gorilla CLI with a straightforward `gorilla` followed by your command in plain English.
 
 For instance, to list all files in the current directory, type:
 
 ```bash
 $ gorilla I want to list all files in the current directory
 ```
 
+or if you prefer, you can use quotes to avoid issues with string parsing:
+
+```bash
+$ gorilla "I want to list all files in the current directory" 
+```
+
 Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
    ls -l
    ls -al
@@ -40,7 +62,9 @@
 ## Contributions
 
 We welcome your enhancements to Gorilla CLI! If you have improvements, feel free to submit a pull request on our GitHub page. 
 
 ## License
 
 Gorilla CLI operates under the Apache 2.0 license. More details can be found in the LICENSE file. We'd also like to extend our appreciation to [questionary](https://github.com/tmbo/questionary) for their fantastic UI!
+
+
```

### Comparing `gorilla-cli-0.0.7/go_cli.py` & `gorilla-cli-0.0.8/go_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 import requests
 import subprocess
 import urllib.parse
 import sys
 from halo import Halo
 import go_questionary
 
-__version__ = "0.0.6"  # current version
+__version__ = "0.0.8"  # current version
 SERVER_URL = "http://34.135.112.197:8000"
 UPDATE_CHECK_FILE = os.path.expanduser("~/.gorilla-cli-last-update-check")
 USERID_FILE = os.path.expanduser("~/.gorilla-cli-userid")
 ISSUE_URL = f"https://github.com/gorilla-llm/gorilla-cli/issues/new"
 WELCOME_TEXT = """🦍 Welcome to Gorilla-CLI! Enhance your Command Line with the power of LLMs! 
 
-Simply use `go <your desired operation>` and Gorilla will do the rest. For instance:
+Simply use `gorilla <your desired operation>` and Gorilla will do the rest. For instance:
     gorilla what is the path of my current directory
     gorilla list all my GCP instances
 
 Created as a research prototype by UC Berkeley, Gorilla-CLI ensures user control and privacy:
  - Commands are executed only with explicit user approval.
  - While queries and error (stderr) logs are used to refine our model, we NEVER gather output (stdout) data.
```

### Comparing `gorilla-cli-0.0.7/go_questionary/__init__.py` & `gorilla-cli-0.0.8/go_questionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/constants.py` & `gorilla-cli-0.0.8/go_questionary/constants.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/form.py` & `gorilla-cli-0.0.8/go_questionary/form.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompt.py` & `gorilla-cli-0.0.8/go_questionary/prompt.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/__init__.py` & `gorilla-cli-0.0.8/go_questionary/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/autocomplete.py` & `gorilla-cli-0.0.8/go_questionary/prompts/autocomplete.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/checkbox.py` & `gorilla-cli-0.0.8/go_questionary/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/common.py` & `gorilla-cli-0.0.8/go_questionary/prompts/common.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/confirm.py` & `gorilla-cli-0.0.8/go_questionary/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/password.py` & `gorilla-cli-0.0.8/go_questionary/prompts/password.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/path.py` & `gorilla-cli-0.0.8/go_questionary/prompts/path.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/rawselect.py` & `gorilla-cli-0.0.8/go_questionary/prompts/rawselect.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/select.py` & `gorilla-cli-0.0.8/go_questionary/prompts/select.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/prompts/text.py` & `gorilla-cli-0.0.8/go_questionary/prompts/text.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/question.py` & `gorilla-cli-0.0.8/go_questionary/question.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/go_questionary/utils.py` & `gorilla-cli-0.0.8/go_questionary/utils.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/gorilla_cli.egg-info/PKG-INFO` & `gorilla-cli-0.0.8/gorilla_cli.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gorilla-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: LLMs for CLI
 Home-page: https://github.com/gorilla-llm/gorilla-cli
 Author: Shishir Patil, Tianjun Zhang
 Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,22 +28,28 @@
 
 ```bash
 pip install gorilla-cli
 ```
 
 ## Usage
 
-Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
+Activate Gorilla CLI with a straightforward `gorilla` followed by your command in plain English.
 
 For instance, to list all files in the current directory, type:
 
 ```bash
 $ gorilla I want to list all files in the current directory
 ```
 
+or if you prefer, you can use quotes to avoid issues with string parsing:
+
+```bash
+$ gorilla "I want to list all files in the current directory" 
+```
+
 Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
    ls -l
    ls -al
```

### Comparing `gorilla-cli-0.0.7/gorilla_cli.egg-info/SOURCES.txt` & `gorilla-cli-0.0.8/gorilla_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.7/setup.py` & `gorilla-cli-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name="gorilla-cli",
-    version="0.0.7",
+    version="0.0.8",
     url="https://github.com/gorilla-llm/gorilla-cli",
     author="Shishir Patil, Tianjun Zhang",
     author_email="sgp@berkeley.edu, tianjunz@berkeley.edu",
     description="LLMs for CLI",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     py_modules=["go_cli"],
```

