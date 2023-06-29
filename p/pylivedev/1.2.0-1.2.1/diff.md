# Comparing `tmp/pylivedev-1.2.0.tar.gz` & `tmp/pylivedev-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylivedev-1.2.0.tar", last modified: Sat May 20 20:34:14 2023, max compression
+gzip compressed data, was "pylivedev-1.2.1.tar", last modified: Thu Jun 29 18:14:07 2023, max compression
```

## Comparing `pylivedev-1.2.0.tar` & `pylivedev-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-20 20:34:14.641251 pylivedev-1.2.0/
--rw-r--r--   0 bast      (1002) bast      (1002)    11357 2021-06-08 11:58:06.000000 pylivedev-1.2.0/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)     4766 2023-05-20 20:34:14.641251 pylivedev-1.2.0/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)     4184 2023-05-20 20:12:25.000000 pylivedev-1.2.0/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-20 20:34:14.641251 pylivedev-1.2.0/pylivedev/
--rw-rw-r--   0 bast      (1002) bast      (1002)     1410 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/__init__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1143 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/__main__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     7935 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/app.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3850 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/imports.py
--rw-rw-r--   0 bast      (1002) bast      (1002)      930 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/output.py
--rw-rw-r--   0 bast      (1002) bast      (1002)       21 2023-05-20 20:31:40.000000 pylivedev-1.2.0/pylivedev/version.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-20 20:34:14.641251 pylivedev-1.2.0/pylivedev.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)     4766 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      387 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       54 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/entry_points.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       33 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/requires.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       10 2023-05-20 20:34:14.000000 pylivedev-1.2.0/pylivedev.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-01-16 16:23:48.000000 pylivedev-1.2.0/pylivedev.egg-info/zip-safe
--rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-05-20 20:34:14.641251 pylivedev-1.2.0/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)     1111 2023-05-20 20:34:00.000000 pylivedev-1.2.0/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-29 18:14:07.941239 pylivedev-1.2.1/
+-rw-r--r--   0 bast      (1000) bast      (1000)    11357 2021-06-08 11:58:06.000000 pylivedev-1.2.1/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5506 2023-06-29 18:14:07.941239 pylivedev-1.2.1/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)     4924 2023-06-29 18:10:08.000000 pylivedev-1.2.1/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-29 18:14:07.941239 pylivedev-1.2.1/pylivedev/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1410 2023-05-20 20:31:40.000000 pylivedev-1.2.1/pylivedev/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1143 2023-05-20 20:31:40.000000 pylivedev-1.2.1/pylivedev/__main__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     7935 2023-05-20 20:31:40.000000 pylivedev-1.2.1/pylivedev/app.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     3850 2023-05-20 20:31:40.000000 pylivedev-1.2.1/pylivedev/imports.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)      930 2023-05-20 20:31:40.000000 pylivedev-1.2.1/pylivedev/output.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)       21 2023-06-29 18:12:03.000000 pylivedev-1.2.1/pylivedev/version.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-29 18:14:07.941239 pylivedev-1.2.1/pylivedev.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5506 2023-06-29 18:14:07.000000 pylivedev-1.2.1/pylivedev.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      387 2023-06-29 18:14:07.000000 pylivedev-1.2.1/pylivedev.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-06-29 18:14:07.000000 pylivedev-1.2.1/pylivedev.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       54 2023-06-29 18:14:07.000000 pylivedev-1.2.1/pylivedev.egg-info/entry_points.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       33 2023-06-29 18:14:07.000000 pylivedev-1.2.1/pylivedev.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       10 2023-06-29 18:14:07.000000 pylivedev-1.2.1/pylivedev.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-01-16 16:23:48.000000 pylivedev-1.2.1/pylivedev.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1000) bast      (1000)       79 2023-06-29 18:14:07.941239 pylivedev-1.2.1/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1110 2023-06-29 18:12:05.000000 pylivedev-1.2.1/setup.py
```

### Comparing `pylivedev-1.2.0/LICENSE` & `pylivedev-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylivedev-1.2.0/PKG-INFO` & `pylivedev-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pylivedev
-Version: 1.2.0
+Version: 1.2.1
 Summary: PyLiveDev is used to keep track of files associated with your script so it can be re-started if any file is updated.
 Home-page: https://ouroboroscoding.com/pylivedev
 Author: Chris Nasr - OuroborosCoding
 Author-email: chris@ouroboroscoding.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/ouroboroscoding/pylivedev
 Project-URL: Tracker, https://github.com/ouroboroscoding/pylivedev/issues
 Keywords: python,live,development
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyLiveDev](https://ouroboroscoding.s3.us-east-2.amazonaws.com/logos/PyLiveDev_128.png)
 
+[![pypi version](https://img.shields.io/pypi/v/pylivedev.svg)](https://pypi.org/project/pylivedev) ![MIT License](https://img.shields.io/pypi/l/pylivedev.svg)
+
 Python Live Development tool.
 
 ## Description
 
 I created **PyLiveDev** because I work a lot in the microservices/REST space and found constantly having to run/restart services while developing and keeping track of multiple logs in separate windows, to be, quite frankly, a pain in my ass.
 
 Inspired by live updates while using create-react-app in development, I wanted to see if there was a way I could make a python program run multiple services and keep track of the files imported. This way if anything changed it could automatically restart those services and save time while developing. As a bonus, piping all stdout/stderr to one screen so I could immediately see if I wrote bad code or was returning something unexpected.
@@ -27,14 +29,22 @@
 
 ## Install
 
 ```console
 foo@bar:~$ pip install pylivedev
 ```
 
+## Warning
+
+If you are using PyLiveDev on a Linux kernel 2.6+, you may at some point run into an issue where the program quits, either quite immediately, or as more and more files are added to your project. This is due to a hard limit in an underlying library. When this happens add/adjust the following setting in your `/etc/sysctl.conf` file (will require root access):
+
+```fs.inotify.max_user_watches=16384```
+
+The default value is 8192, so adjust accordingly then reboot. Increase as necessary until PyLiveDev stops crashing.
+
 ## Run
 
 ```console
 foo@bar:~$ pylivedev
 ```
 
 ## Configuration
@@ -53,16 +63,16 @@
 	}
 }
 ```
 
 | Name | Type | Mandatory | Description |
 | ------ | ------ | ------ | ------ |
 | command | String | Yes | The name of the script or module to run as a process. e.g. "services.rest", "main.py" |
-| mode | "module" \| "script" | No | Tells pylivedev whether you are trying to run a stand alone script, or a python module. Defaults to "script". |
-| tracked | Boolean | No | When true, proccess is tracked via file changes. Use false for static or external modules. Defaults to true. |
+| mode | "module" \| "script" \| "exe" | No | Tells pylivedev whether you are trying to run a stand alone script, a python module, or a binary (or non-parsable) application. Defaults to "script". |
+| tracked | Boolean | No | When true, proccess is tracked via file changes. Use false for static or external modules. Defaults to true. Will be ignored if mode is set to "exe". |
 | python | String | No | The full path to the python intepreter to use to run your process. Defaults to the python interpreter running pylivedev. |
 | arguments | String[] | No | An array of additional arguments passed to the process. |
 | additional_files | String[] | No | An array of additional files to be watched/observed for changes. |
 | unbuffered | Boolean | No | Run the processed unbuffered, defaults to true. |
 | verbose | Boolean | No | Runs pylivedev in verbose mode to give more information on what is happening, what imports were found, what files have changed, etc. Defaults to false. |
 
 ## Defaults
@@ -131,13 +141,7 @@
 - nodes/rest/\_\_init\_\_.py
 - records/\_\_init\_\_.py
 
 Any time any of these files is saved/changed on the system, **PyLiveDev** would shut down the "main" process, re-parse the module looking for imports, and then restart the process.
 
 ***Note*** system and pip imports will not be added to the list, like `time` in the above example. In most cases system files don't change often and it would waste resources to watch them. If you update a pip library, or update python, it's best to shut down **PyLiveDev** [CRTL-C] and restart it.
 
-## License
-
-Apache License
-Version 2.0
-
-
```

### Comparing `pylivedev-1.2.0/README.md` & `pylivedev-1.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ![PyLiveDev](https://ouroboroscoding.s3.us-east-2.amazonaws.com/logos/PyLiveDev_128.png)
 
+[![pypi version](https://img.shields.io/pypi/v/pylivedev.svg)](https://pypi.org/project/pylivedev) ![MIT License](https://img.shields.io/pypi/l/pylivedev.svg)
+
 Python Live Development tool.
 
 ## Description
 
 I created **PyLiveDev** because I work a lot in the microservices/REST space and found constantly having to run/restart services while developing and keeping track of multiple logs in separate windows, to be, quite frankly, a pain in my ass.
 
 Inspired by live updates while using create-react-app in development, I wanted to see if there was a way I could make a python program run multiple services and keep track of the files imported. This way if anything changed it could automatically restart those services and save time while developing. As a bonus, piping all stdout/stderr to one screen so I could immediately see if I wrote bad code or was returning something unexpected.
@@ -12,14 +14,22 @@
 
 ## Install
 
 ```console
 foo@bar:~$ pip install pylivedev
 ```
 
+## Warning
+
+If you are using PyLiveDev on a Linux kernel 2.6+, you may at some point run into an issue where the program quits, either quite immediately, or as more and more files are added to your project. This is due to a hard limit in an underlying library. When this happens add/adjust the following setting in your `/etc/sysctl.conf` file (will require root access):
+
+```fs.inotify.max_user_watches=16384```
+
+The default value is 8192, so adjust accordingly then reboot. Increase as necessary until PyLiveDev stops crashing.
+
 ## Run
 
 ```console
 foo@bar:~$ pylivedev
 ```
 
 ## Configuration
@@ -38,16 +48,16 @@
 	}
 }
 ```
 
 | Name | Type | Mandatory | Description |
 | ------ | ------ | ------ | ------ |
 | command | String | Yes | The name of the script or module to run as a process. e.g. "services.rest", "main.py" |
-| mode | "module" \| "script" | No | Tells pylivedev whether you are trying to run a stand alone script, or a python module. Defaults to "script". |
-| tracked | Boolean | No | When true, proccess is tracked via file changes. Use false for static or external modules. Defaults to true. |
+| mode | "module" \| "script" \| "exe" | No | Tells pylivedev whether you are trying to run a stand alone script, a python module, or a binary (or non-parsable) application. Defaults to "script". |
+| tracked | Boolean | No | When true, proccess is tracked via file changes. Use false for static or external modules. Defaults to true. Will be ignored if mode is set to "exe". |
 | python | String | No | The full path to the python intepreter to use to run your process. Defaults to the python interpreter running pylivedev. |
 | arguments | String[] | No | An array of additional arguments passed to the process. |
 | additional_files | String[] | No | An array of additional files to be watched/observed for changes. |
 | unbuffered | Boolean | No | Run the processed unbuffered, defaults to true. |
 | verbose | Boolean | No | Runs pylivedev in verbose mode to give more information on what is happening, what imports were found, what files have changed, etc. Defaults to false. |
 
 ## Defaults
@@ -114,13 +124,8 @@
 - config.json
 - nodes/rest/main.py
 - nodes/rest/\_\_init\_\_.py
 - records/\_\_init\_\_.py
 
 Any time any of these files is saved/changed on the system, **PyLiveDev** would shut down the "main" process, re-parse the module looking for imports, and then restart the process.
 
-***Note*** system and pip imports will not be added to the list, like `time` in the above example. In most cases system files don't change often and it would waste resources to watch them. If you update a pip library, or update python, it's best to shut down **PyLiveDev** [CRTL-C] and restart it.
-
-## License
-
-Apache License
-Version 2.0
+***Note*** system and pip imports will not be added to the list, like `time` in the above example. In most cases system files don't change often and it would waste resources to watch them. If you update a pip library, or update python, it's best to shut down **PyLiveDev** [CRTL-C] and restart it.
```

### Comparing `pylivedev-1.2.0/pylivedev/__init__.py` & `pylivedev-1.2.1/pylivedev/__init__.py`

 * *Files identical despite different names*

### Comparing `pylivedev-1.2.0/pylivedev/__main__.py` & `pylivedev-1.2.1/pylivedev/__main__.py`

 * *Files identical despite different names*

### Comparing `pylivedev-1.2.0/pylivedev/app.py` & `pylivedev-1.2.1/pylivedev/app.py`

 * *Files identical despite different names*

### Comparing `pylivedev-1.2.0/pylivedev/imports.py` & `pylivedev-1.2.1/pylivedev/imports.py`

 * *Files identical despite different names*

### Comparing `pylivedev-1.2.0/pylivedev/output.py` & `pylivedev-1.2.1/pylivedev/output.py`

 * *Files identical despite different names*

### Comparing `pylivedev-1.2.0/pylivedev.egg-info/PKG-INFO` & `pylivedev-1.2.1/pylivedev.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pylivedev
-Version: 1.2.0
+Version: 1.2.1
 Summary: PyLiveDev is used to keep track of files associated with your script so it can be re-started if any file is updated.
 Home-page: https://ouroboroscoding.com/pylivedev
 Author: Chris Nasr - OuroborosCoding
 Author-email: chris@ouroboroscoding.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/ouroboroscoding/pylivedev
 Project-URL: Tracker, https://github.com/ouroboroscoding/pylivedev/issues
 Keywords: python,live,development
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyLiveDev](https://ouroboroscoding.s3.us-east-2.amazonaws.com/logos/PyLiveDev_128.png)
 
+[![pypi version](https://img.shields.io/pypi/v/pylivedev.svg)](https://pypi.org/project/pylivedev) ![MIT License](https://img.shields.io/pypi/l/pylivedev.svg)
+
 Python Live Development tool.
 
 ## Description
 
 I created **PyLiveDev** because I work a lot in the microservices/REST space and found constantly having to run/restart services while developing and keeping track of multiple logs in separate windows, to be, quite frankly, a pain in my ass.
 
 Inspired by live updates while using create-react-app in development, I wanted to see if there was a way I could make a python program run multiple services and keep track of the files imported. This way if anything changed it could automatically restart those services and save time while developing. As a bonus, piping all stdout/stderr to one screen so I could immediately see if I wrote bad code or was returning something unexpected.
@@ -27,14 +29,22 @@
 
 ## Install
 
 ```console
 foo@bar:~$ pip install pylivedev
 ```
 
+## Warning
+
+If you are using PyLiveDev on a Linux kernel 2.6+, you may at some point run into an issue where the program quits, either quite immediately, or as more and more files are added to your project. This is due to a hard limit in an underlying library. When this happens add/adjust the following setting in your `/etc/sysctl.conf` file (will require root access):
+
+```fs.inotify.max_user_watches=16384```
+
+The default value is 8192, so adjust accordingly then reboot. Increase as necessary until PyLiveDev stops crashing.
+
 ## Run
 
 ```console
 foo@bar:~$ pylivedev
 ```
 
 ## Configuration
@@ -53,16 +63,16 @@
 	}
 }
 ```
 
 | Name | Type | Mandatory | Description |
 | ------ | ------ | ------ | ------ |
 | command | String | Yes | The name of the script or module to run as a process. e.g. "services.rest", "main.py" |
-| mode | "module" \| "script" | No | Tells pylivedev whether you are trying to run a stand alone script, or a python module. Defaults to "script". |
-| tracked | Boolean | No | When true, proccess is tracked via file changes. Use false for static or external modules. Defaults to true. |
+| mode | "module" \| "script" \| "exe" | No | Tells pylivedev whether you are trying to run a stand alone script, a python module, or a binary (or non-parsable) application. Defaults to "script". |
+| tracked | Boolean | No | When true, proccess is tracked via file changes. Use false for static or external modules. Defaults to true. Will be ignored if mode is set to "exe". |
 | python | String | No | The full path to the python intepreter to use to run your process. Defaults to the python interpreter running pylivedev. |
 | arguments | String[] | No | An array of additional arguments passed to the process. |
 | additional_files | String[] | No | An array of additional files to be watched/observed for changes. |
 | unbuffered | Boolean | No | Run the processed unbuffered, defaults to true. |
 | verbose | Boolean | No | Runs pylivedev in verbose mode to give more information on what is happening, what imports were found, what files have changed, etc. Defaults to false. |
 
 ## Defaults
@@ -131,13 +141,7 @@
 - nodes/rest/\_\_init\_\_.py
 - records/\_\_init\_\_.py
 
 Any time any of these files is saved/changed on the system, **PyLiveDev** would shut down the "main" process, re-parse the module looking for imports, and then restart the process.
 
 ***Note*** system and pip imports will not be added to the list, like `time` in the above example. In most cases system files don't change often and it would waste resources to watch them. If you update a pip library, or update python, it's best to shut down **PyLiveDev** [CRTL-C] and restart it.
 
-## License
-
-Apache License
-Version 2.0
-
-
```

### Comparing `pylivedev-1.2.0/setup.py` & `pylivedev-1.2.1/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 		'termcolor>=1.1.0',
 		'watchdog>=2.1.2'
 	],
 	entry_points={
 		'console_scripts': ['pylivedev=pylivedev.__main__:cli']
 	},
 	zip_safe=True
-)
+)
```

