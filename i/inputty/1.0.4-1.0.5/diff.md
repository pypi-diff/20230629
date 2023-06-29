# Comparing `tmp/inputty-1.0.4.tar.gz` & `tmp/inputty-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-1.0.4.tar", last modified: Sun Jun 18 11:19:04 2023, max compression
+gzip compressed data, was "inputty-1.0.5.tar", last modified: Thu Jun 29 10:27:04 2023, max compression
```

## Comparing `inputty-1.0.4.tar` & `inputty-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.4/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1242 2023-06-18 11:19:04.962110 inputty-1.0.4/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.4/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.4/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-18 11:17:15.000000 inputty-1.0.4/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.4/inputty/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2129 2023-06-18 11:11:12.000000 inputty-1.0.4/inputty/src/colours.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9133 2023-06-18 10:50:30.000000 inputty-1.0.4/inputty/src/input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.4/inputty/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3219 2023-06-17 09:42:30.000000 inputty-1.0.4/inputty/tests/test_input.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      664 2023-06-18 11:15:07.000000 inputty-1.0.4/inputty/tests/test_prompt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      551 2023-06-18 10:49:43.000000 inputty-1.0.4/inputty/xxx.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1242 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      370 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-18 11:19:04.965443 inputty-1.0.4/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.4/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:27:04.174599 inputty-1.0.5/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.5/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1265 2023-06-29 10:27:04.174599 inputty-1.0.5/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.5/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:27:04.171265 inputty-1.0.5/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.5/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 10:24:22.000000 inputty-1.0.5/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:27:04.171265 inputty-1.0.5/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.5/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2129 2023-06-18 11:11:12.000000 inputty-1.0.5/inputty/src/colours.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9168 2023-06-29 10:24:22.000000 inputty-1.0.5/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:27:04.174599 inputty-1.0.5/inputty/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.5/inputty/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3219 2023-06-17 09:42:30.000000 inputty-1.0.5/inputty/tests/test_input.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      664 2023-06-29 10:24:22.000000 inputty-1.0.5/inputty/tests/test_prompt.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:27:04.171265 inputty-1.0.5/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1265 2023-06-29 10:27:04.000000 inputty-1.0.5/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      355 2023-06-29 10:27:04.000000 inputty-1.0.5/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 10:27:04.000000 inputty-1.0.5/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-06-29 10:27:04.000000 inputty-1.0.5/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 10:27:04.174599 inputty-1.0.5/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.5/setup.py
```

### Comparing `inputty-1.0.4/LICENSE.txt` & `inputty-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-1.0.4/PKG-INFO` & `inputty-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.4
+Version: 1.0.5
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
+Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # inputty
 
 A module to facilitate CLI inputs.
 
@@ -21,14 +20,20 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.5 29 Jun 2023
+
+1. xxx
+
+------
+
 Version 1.0.4 18 June 2023
 
 1. Colour cues
 
 ------
 
 Version 1.0.3 6 June 2023
@@ -85,9 +90,7 @@
 ------
 
 Version 0.0.0 9 May 2023
 
 1. Initial version
 
 ------
-
-
```

### Comparing `inputty-1.0.4/inputty/src/colours.py` & `inputty-1.0.5/inputty/src/colours.py`

 * *Files identical despite different names*

### Comparing `inputty-1.0.4/inputty/src/input.py` & `inputty-1.0.5/inputty/src/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 'S': (function_three, [files_to_copy]),
                 'Q': (quit, []),
             }
         If the process key is <RTN> (RETURN) then a null input will invoke the associated process.
 
         If the process key is <INTEGERS> (INTEGER_SELECTION) then a valid input is created for
         integers in the range (min_integer to the max_integer) and
-        the call is to function_one with the  parameter input integer.)
+        the call is to function_one with the first parameter the integer that has been input.)
 
 
     validation: dict[str, x]
         experimental
 
     Methods
     -------
@@ -117,14 +117,15 @@
             response = input(self.prompt)
 
             # Handle null input
             if not response:
                 if RETURN in self.processes:
                     return RETURN
                 continue
+
             if response in self.processes:
                 return response
 
             # Capture string
             if STRING in self.processes:
                 return response
 
@@ -235,16 +236,17 @@
         return INVALID_INPUT_MSG
 
     def colorize_prompt(self, prompt, processes, colours) -> str:
         colours = get_colour_map(colours)
         prompt = prompt.strip() + ' '
         for key, item in processes.items():
             if f"'{key}'" in prompt:
-                # prompt = prompt.replace(f"'{key}'", f"{Fore.BLUE}{key}{''}")
-                prompt = prompt.replace(f"'{key}'", self.colorize_key(key, colours))
+                prompt = prompt.replace(f"'{key}'", key)
+            if f"{key}" in prompt:
+                prompt = prompt.replace(f"{key}", self.colorize_key(key, colours))
         return prompt
 
     @staticmethod
     def colorize_key(key: str, colours) -> str:
         text_fore = colours['text-fore']
         text_style = colours['text-style']
         text_back = colours['text-back']
```

### Comparing `inputty-1.0.4/inputty/tests/test_input.py` & `inputty-1.0.5/inputty/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `inputty-1.0.4/inputty/tests/test_prompt.py` & `inputty-1.0.5/inputty/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `inputty-1.0.4/inputty.egg-info/PKG-INFO` & `inputty-1.0.5/inputty.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.4
+Version: 1.0.5
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
+Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # inputty
 
 A module to facilitate CLI inputs.
 
@@ -21,14 +20,20 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.5 29 Jun 2023
+
+1. xxx
+
+------
+
 Version 1.0.4 18 June 2023
 
 1. Colour cues
 
 ------
 
 Version 1.0.3 6 June 2023
@@ -85,9 +90,7 @@
 ------
 
 Version 0.0.0 9 May 2023
 
 1. Initial version
 
 ------
-
-
```

### Comparing `inputty-1.0.4/setup.py` & `inputty-1.0.5/setup.py`

 * *Files identical despite different names*

