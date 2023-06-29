# Comparing `tmp/pyassist-0.1.tar.gz` & `tmp/pyassist-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassist-0.1.tar", last modified: Wed Jun 28 16:53:53 2023, max compression
+gzip compressed data, was "pyassist-0.2.tar", last modified: Thu Jun 29 11:46:16 2023, max compression
```

## Comparing `pyassist-0.1.tar` & `pyassist-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 16:53:53.711411 pyassist-0.1/
--rw-rw-rw-   0        0        0     1063 2023-06-28 16:14:31.000000 pyassist-0.1/LICENSE
--rw-rw-rw-   0        0        0      842 2023-06-28 16:53:53.711411 pyassist-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-06-28 16:30:47.000000 pyassist-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 16:53:53.694238 pyassist-0.1/pyassist/
--rw-rw-rw-   0        0        0       70 2023-06-28 14:55:39.000000 pyassist-0.1/pyassist/__init__.py
--rw-rw-rw-   0        0        0     1919 2023-06-28 16:08:10.000000 pyassist-0.1/pyassist/process.py
--rw-rw-rw-   0        0        0     1763 2023-06-28 16:06:08.000000 pyassist-0.1/pyassist/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 16:53:53.710403 pyassist-0.1/pyassist.egg-info/
--rw-rw-rw-   0        0        0      842 2023-06-28 16:53:53.000000 pyassist-0.1/pyassist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-28 16:53:53.000000 pyassist-0.1/pyassist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 16:53:53.000000 pyassist-0.1/pyassist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 16:53:53.000000 pyassist-0.1/pyassist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-28 16:53:53.712418 pyassist-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-06-28 16:53:51.000000 pyassist-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:46:16.469097 pyassist-0.2/
+-rw-rw-rw-   0        0        0     1063 2023-06-28 16:14:31.000000 pyassist-0.2/LICENSE
+-rw-rw-rw-   0        0        0      867 2023-06-29 11:46:16.469097 pyassist-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-06-28 16:30:47.000000 pyassist-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 11:46:16.451092 pyassist-0.2/pyassist/
+-rw-rw-rw-   0        0        0      100 2023-06-28 17:27:27.000000 pyassist-0.2/pyassist/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-06-29 10:33:09.000000 pyassist-0.2/pyassist/process.py
+-rw-rw-rw-   0        0        0     1961 2023-06-29 10:33:04.000000 pyassist-0.2/pyassist/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:46:16.468096 pyassist-0.2/pyassist.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-06-29 11:46:16.000000 pyassist-0.2/pyassist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-29 11:46:16.000000 pyassist-0.2/pyassist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:46:16.000000 pyassist-0.2/pyassist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-29 11:46:16.000000 pyassist-0.2/pyassist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 11:46:16.000000 pyassist-0.2/pyassist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 11:46:16.470097 pyassist-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1925 2023-06-29 11:41:28.000000 pyassist-0.2/setup.py
```

### Comparing `pyassist-0.1/LICENSE` & `pyassist-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassist-0.1/PKG-INFO` & `pyassist-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyassist
-Version: 0.1
+Version: 0.2
 Summary: This is Python Utility
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
-Keywords: Logger,Easy,PySy
+Keywords: Utility,utils,pyutils,assist,easy,service
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `pyassist-0.1/pyassist/process.py` & `pyassist-0.2/pyassist/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import subprocess
 from .utils import Utilities
 # Contains Process/ Subprocess related Functions
-class ProcessUtilities(Utilities):
+class Process(Utilities):
     def __init__(self, **kwargs):
+        if "name" not in kwargs:
+            kwargs["name"] = (f"{__class__}".split("'")[1])
         super().__init__(**kwargs)
-        # botname = kwargs["botname"]
-        # if botname:
-        # else:
-        #     super().__init__(botname=logger.__get_bot_name__(__file__), **kwargs)
-        self.print_debug_log(f"Initialized {self.__class__}")
+        self.debug(f"Initialized: {kwargs['name']}")
 
     def run_process(self, process_list, stream=False):
         header = "run_process: "
         self.info(header + str(process_list))
         process = subprocess.Popen(process_list[0],
                                 shell=True,
                                 stdout=subprocess.PIPE,
```

### Comparing `pyassist-0.1/pyassist/utils.py` & `pyassist-0.2/pyassist/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from .import datetime, os
 start_time = datetime.now()
 from time import sleep
 from pyloggerutils import Logger
 
+# def get_logger(**kwargs):
+#     return Logger(**kwargs)
+
 class Utilities():
 
     MODULE = __name__
 
     def __init__(self, **kwargs):
-        kwargs["name"] = "Utilities"
-        logger = self.get_logger(kwargs)
+        if "name" not in kwargs:
+            kwargs["name"] = (f"{__class__}".split("'")[1])
+        self.get_logger(**kwargs)
+        self.debug(f"Initialized: {kwargs['name']}")
+
+    def get_logger(self, **kwargs):
+        logger = Logger(**kwargs)
         self.info = logger.info
         self.error = logger.error
         self.warning = logger.warning
         self.debug = logger.debug
         self.critical = logger.critical
-
-    def get_logger(self, **kwargs):
-        return Logger(**kwargs)
+        self.logger = logger
 
     def parent_dir(self, filename):
         expanded_dir = os.path.expanduser(filename)
         realpath_dir = os.path.realpath(expanded_dir)
         directory = os.path.dirname(realpath_dir)
         return directory
```

### Comparing `pyassist-0.1/pyassist.egg-info/PKG-INFO` & `pyassist-0.2/pyassist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyassist
-Version: 0.1
+Version: 0.2
 Summary: This is Python Utility
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
-Keywords: Logger,Easy,PySy
+Keywords: Utility,utils,pyutils,assist,easy,service
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `pyassist-0.1/setup.py` & `pyassist-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'pyassist',         # How you named your package folder (MyLib)
   packages = ['pyassist'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = """This is Python Utility""",   # Give a short description about your library
   author = 'Sabari Rajan',                   # Type in your name
   author_email = 'mailme@isbarirajan.com',      # Type in your E-Mail
   url = 'https://github.com/ISabariRajan',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.1.tar.gz',    # I explain this later on
-  keywords = ['Logger', 'Easy', 'PySy'],   # Keywords that define your package best
-  install_requires=[],
+  download_url = 'https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.tar.gz',    # I explain this later on
+  keywords = ['Utility', 'utils', 'pyutils', 'assist', 'easy', 'service'],   # Keywords that define your package best
+  install_requires=[
+      "lxml", "pyloggerutils", "requests", "urllib3"
+  ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
```

