# Comparing `tmp/gorilla-cli-0.0.6.tar.gz` & `tmp/gorilla-cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gorilla-cli-0.0.6.tar", last modified: Sun Jun 25 09:10:16 2023, max compression
+gzip compressed data, was "gorilla-cli-0.0.7.tar", last modified: Thu Jun 29 16:38:05 2023, max compression
```

## Comparing `gorilla-cli-0.0.6.tar` & `gorilla-cli-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.242728 gorilla-cli-0.0.6/
--rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/LICENSE
--rw-r--r--   0 shishir    (501) staff       (20)     2420 2023-06-25 09:10:16.242452 gorilla-cli-0.0.6/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)     1914 2023-06-25 09:09:40.000000 gorilla-cli-0.0.6/README.md
--rw-r--r--   0 shishir    (501) staff       (20)     6755 2023-06-25 08:59:47.000000 gorilla-cli-0.0.6/go_cli.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.239848 gorilla-cli-0.0.6/go_questionary/
--rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/constants.py
--rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/form.py
--rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompt.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.241428 gorilla-cli-0.0.6/go_questionary/prompts/
--rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/autocomplete.py
--rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/checkbox.py
--rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/common.py
--rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/confirm.py
--rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/password.py
--rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/path.py
--rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/rawselect.py
--rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/select.py
--rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/text.py
--rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/question.py
--rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/utils.py
--rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/version.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.242235 gorilla-cli-0.0.6/gorilla_cli.egg-info/
--rw-r--r--   0 shishir    (501) staff       (20)     2420 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/SOURCES.txt
--rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/dependency_links.txt
--rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/entry_points.txt
--rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/requires.txt
--rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/top_level.txt
--rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-25 09:10:16.242780 gorilla-cli-0.0.6/setup.cfg
--rw-r--r--   0 shishir    (501) staff       (20)     1502 2023-06-25 01:01:09.000000 gorilla-cli-0.0.6/setup.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.299675 gorilla-cli-0.0.7/
+-rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/LICENSE
+-rw-r--r--   0 shishir    (501) staff       (20)     2425 2023-06-29 16:38:05.299183 gorilla-cli-0.0.7/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)     1919 2023-06-29 16:34:42.000000 gorilla-cli-0.0.7/README.md
+-rw-r--r--   0 shishir    (501) staff       (20)     6799 2023-06-29 16:35:01.000000 gorilla-cli-0.0.7/go_cli.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.296116 gorilla-cli-0.0.7/go_questionary/
+-rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/constants.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/form.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompt.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.298029 gorilla-cli-0.0.7/go_questionary/prompts/
+-rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/autocomplete.py
+-rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/checkbox.py
+-rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/common.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/confirm.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/password.py
+-rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/path.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/rawselect.py
+-rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/select.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/prompts/text.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/question.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/utils.py
+-rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.7/go_questionary/version.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 16:38:05.298902 gorilla-cli-0.0.7/gorilla_cli.egg-info/
+-rw-r--r--   0 shishir    (501) staff       (20)     2425 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       41 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/entry_points.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/requires.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-29 16:38:05.000000 gorilla-cli-0.0.7/gorilla_cli.egg-info/top_level.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-29 16:38:05.299792 gorilla-cli-0.0.7/setup.cfg
+-rw-r--r--   0 shishir    (501) staff       (20)     1507 2023-06-29 16:35:45.000000 gorilla-cli-0.0.7/setup.py
```

### Comparing `gorilla-cli-0.0.6/LICENSE` & `gorilla-cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/PKG-INFO` & `gorilla-cli-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gorilla-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: LLMs for CLI
 Home-page: https://github.com/gorilla-llm/gorilla-cli
 Author: Shishir Patil, Tianjun Zhang
 Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 ## Usage
 
 Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
 
 For instance, to list all files in the current directory, type:
 
 ```bash
-$ go I want to list all files in the current directory
+$ gorilla I want to list all files in the current directory
 ```
 
 Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
```

### Comparing `gorilla-cli-0.0.6/README.md` & `gorilla-cli-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## Usage
 
 Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
 
 For instance, to list all files in the current directory, type:
 
 ```bash
-$ go I want to list all files in the current directory
+$ gorilla I want to list all files in the current directory
 ```
 
 Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
```

### Comparing `gorilla-cli-0.0.6/go_cli.py` & `gorilla-cli-0.0.7/go_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 SERVER_URL = "http://34.135.112.197:8000"
 UPDATE_CHECK_FILE = os.path.expanduser("~/.gorilla-cli-last-update-check")
 USERID_FILE = os.path.expanduser("~/.gorilla-cli-userid")
 ISSUE_URL = f"https://github.com/gorilla-llm/gorilla-cli/issues/new"
 WELCOME_TEXT = """🦍 Welcome to Gorilla-CLI! Enhance your Command Line with the power of LLMs! 
 
 Simply use `go <your desired operation>` and Gorilla will do the rest. For instance:
-    go what is the path of my current directory
-    go list all my GCP instances
+    gorilla what is the path of my current directory
+    gorilla list all my GCP instances
 
 Created as a research prototype by UC Berkeley, Gorilla-CLI ensures user control and privacy:
  - Commands are executed only with explicit user approval.
  - While queries and error (stderr) logs are used to refine our model, we NEVER gather output (stdout) data.
 
 Visit us at github.com/gorilla-llm/gorilla-cli and start talking to your CLI!"""
 
@@ -50,15 +50,15 @@
         last_check_date = datetime.datetime.now() - datetime.timedelta(days=1)
     if datetime.datetime.now() - last_check_date >= datetime.timedelta(days=1):
         try:
             response = requests.get("https://pypi.org/pypi/gorilla-cli/json")
             latest_version = response.json()["info"]["version"]
 
             if latest_version > __version__:
-                print(f"A new version of gorilla-cli is available: {latest_version}")
+                print(f"A new version is available: {latest_version}. Update with `pip install --upgrade gorilla-cli`")
         except Exception as e:
             print("Unable to check for updates:", e)
         try:
             with open(UPDATE_CHECK_FILE, "w") as f:
                 f.write(datetime.datetime.now().strftime("%Y-%m-%d"))
         except Exception as e:
             print("Unable to write update check file:", e)
```

### Comparing `gorilla-cli-0.0.6/go_questionary/__init__.py` & `gorilla-cli-0.0.7/go_questionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/constants.py` & `gorilla-cli-0.0.7/go_questionary/constants.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/form.py` & `gorilla-cli-0.0.7/go_questionary/form.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompt.py` & `gorilla-cli-0.0.7/go_questionary/prompt.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/__init__.py` & `gorilla-cli-0.0.7/go_questionary/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/autocomplete.py` & `gorilla-cli-0.0.7/go_questionary/prompts/autocomplete.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/checkbox.py` & `gorilla-cli-0.0.7/go_questionary/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/common.py` & `gorilla-cli-0.0.7/go_questionary/prompts/common.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/confirm.py` & `gorilla-cli-0.0.7/go_questionary/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/password.py` & `gorilla-cli-0.0.7/go_questionary/prompts/password.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/path.py` & `gorilla-cli-0.0.7/go_questionary/prompts/path.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/rawselect.py` & `gorilla-cli-0.0.7/go_questionary/prompts/rawselect.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/select.py` & `gorilla-cli-0.0.7/go_questionary/prompts/select.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/prompts/text.py` & `gorilla-cli-0.0.7/go_questionary/prompts/text.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/question.py` & `gorilla-cli-0.0.7/go_questionary/question.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/go_questionary/utils.py` & `gorilla-cli-0.0.7/go_questionary/utils.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/gorilla_cli.egg-info/PKG-INFO` & `gorilla-cli-0.0.7/gorilla_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gorilla-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: LLMs for CLI
 Home-page: https://github.com/gorilla-llm/gorilla-cli
 Author: Shishir Patil, Tianjun Zhang
 Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 ## Usage
 
 Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
 
 For instance, to list all files in the current directory, type:
 
 ```bash
-$ go I want to list all files in the current directory
+$ gorilla I want to list all files in the current directory
 ```
 
 Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
```

### Comparing `gorilla-cli-0.0.6/gorilla_cli.egg-info/SOURCES.txt` & `gorilla-cli-0.0.7/gorilla_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.6/setup.py` & `gorilla-cli-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name="gorilla-cli",
-    version="0.0.6",
+    version="0.0.7",
     url="https://github.com/gorilla-llm/gorilla-cli",
     author="Shishir Patil, Tianjun Zhang",
     author_email="sgp@berkeley.edu, tianjunz@berkeley.edu",
     description="LLMs for CLI",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     py_modules=["go_cli"],
@@ -28,15 +28,15 @@
     install_requires=[
         "requests",
         "halo",
         "prompt-toolkit",
     ],
     entry_points={
         "console_scripts": [
-            "go=go_cli:main",
+            "gorilla=go_cli:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
```

