# Comparing `tmp/pyloggerutils-0.1.3.tar.gz` & `tmp/pyloggerutils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggerutils-0.1.3.tar", last modified: Tue Jun 27 18:17:32 2023, max compression
+gzip compressed data, was "pyloggerutils-0.1.4.tar", last modified: Thu Jun 29 09:44:01 2023, max compression
```

## Comparing `pyloggerutils-0.1.3.tar` & `pyloggerutils-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 18:17:32.828725 pyloggerutils-0.1.3/
--rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1029 2023-06-27 18:17:32.828725 pyloggerutils-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 18:17:32.814725 pyloggerutils-0.1.3/pyloggerutils/
--rw-rw-rw-   0        0        0     1397 2023-06-27 18:09:21.000000 pyloggerutils-0.1.3/pyloggerutils/__init__.py
--rw-rw-rw-   0        0        0     2396 2023-06-27 18:10:34.000000 pyloggerutils-0.1.3/pyloggerutils/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-27 18:17:32.827724 pyloggerutils-0.1.3/pyloggerutils.egg-info/
--rw-rw-rw-   0        0        0     1029 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-27 18:17:32.000000 pyloggerutils-0.1.3/pyloggerutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-27 18:17:32.833745 pyloggerutils-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1850 2023-06-27 18:16:28.000000 pyloggerutils-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:44:01.743206 pyloggerutils-0.1.4/
+-rw-rw-rw-   0        0        0     1063 2023-06-27 12:21:53.000000 pyloggerutils-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1029 2023-06-29 09:44:01.744204 pyloggerutils-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-27 13:04:54.000000 pyloggerutils-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 09:44:01.729205 pyloggerutils-0.1.4/pyloggerutils/
+-rw-rw-rw-   0        0        0     1428 2023-06-28 15:41:35.000000 pyloggerutils-0.1.4/pyloggerutils/__init__.py
+-rw-rw-rw-   0        0        0     2558 2023-06-29 09:34:38.000000 pyloggerutils-0.1.4/pyloggerutils/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:44:01.743206 pyloggerutils-0.1.4/pyloggerutils.egg-info/
+-rw-rw-rw-   0        0        0     1029 2023-06-29 09:44:01.000000 pyloggerutils-0.1.4/pyloggerutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-29 09:44:01.000000 pyloggerutils-0.1.4/pyloggerutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:44:01.000000 pyloggerutils-0.1.4/pyloggerutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 09:44:01.000000 pyloggerutils-0.1.4/pyloggerutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 09:44:01.745205 pyloggerutils-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-29 09:36:13.000000 pyloggerutils-0.1.4/setup.py
```

### Comparing `pyloggerutils-0.1.3/LICENSE` & `pyloggerutils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggerutils-0.1.3/PKG-INFO` & `pyloggerutils-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyloggerutils
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is Python Logger
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.3.tar.gz
+Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.4.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Logger,Easy,PySy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyloggerutils-0.1.3/pyloggerutils/__init__.py` & `pyloggerutils-0.1.4/pyloggerutils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,26 @@
             "class": "logging.StreamHandler",
             "level": "DEBUG"
         },
         "fileHandler":{
             "formatter": "std_out",
             "class": "logging.handlers.TimedRotatingFileHandler",
             "level": "DEBUG",
-            "filename": "testing.log"
+            "filename": "debug.log"
             # "args": ('testing.log','w0',0,5)
         },
         "fileErrorHandler":{
             "formatter": "std_out",
             "class": "logging.handlers.TimedRotatingFileHandler",
             "level": "ERROR",
-            "filename": "testing-error.log"
+            "filename": "error.log"
         }
     },
     "formatters":{
         "std_out": {
             # "format": "%(asctime)s : %(levelname)s : %(module)s : %(funcName)s : %(lineno)d : (Process Details : (%(process)d, %(processName)s), Thread Details : (%(thread)d, %(threadName)s))\nLog : %(message)s",
-            "format": "%(message)s",
+            "format": "%(asctime)s - %(name)s [%(processName)s] %(message)s",
             "datefmt":"%d-%m-%Y %I:%M:%S"
         }
     }
 }
 from .logger import Logger as Logger
```

### Comparing `pyloggerutils-0.1.3/pyloggerutils/logger.py` & `pyloggerutils-0.1.4/pyloggerutils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # from logging.handlers import File
 from logging import getLogger
 from logging.config import dictConfig
 import inspect
 class Logger:
 
     name = "Logger"
+    add_index = 3
     def __init__(self, **kwargs):
         if "name" in kwargs:
             self.name = kwargs["name"]
         self.config_logger()
     
     def config_logger(self):
         dictConfig(LOG_CONFIG)
@@ -19,18 +20,19 @@
 
     def __get_file_name__(self, file_name):
         return os.path.basename(file_name)
 
     def __get_bot_name__(self, file_name):
         return os.path.splitext(self.__get_file_name__(file_name))[0]
 
-    def __get_frameinfo(self, add_index=3):
+    def __get_frameinfo(self, add_index=False):
         innerframe = inspect.currentframe()
         outerframes = inspect.getouterframes(innerframe)
-
+        if not add_index:
+            add_index = self.add_index
         for index, frame in enumerate(outerframes):
             if(frame.function == "__get_frameinfo"):
                 # add_index - Which function calls this function
                 # +1 -> either debug, info, warning, error functions which is calling this function
                 # +2 -> The Function that calls the above log functions, n -> until the top most function
                 index += add_index
                 break
@@ -38,16 +40,19 @@
 
     def msg(self, msg):
         frame_info = self.__get_frameinfo()
         function_name = frame_info.function
         module_name = self.__get_bot_name__(frame_info.filename)
         log_level = self.__get_frameinfo(add_index=2)
         log_level = log_level.function.split(".")
-        log_level = log_level[len(log_level)-1]
-        msg = f"{datetime.strftime(datetime.now(), LOG_DATE_FORMAT)} | [{module_name.rjust(10)}.{function_name.ljust(10)}] | [{log_level.rjust(8)}] : {msg}"
+        log_level = f"[{log_level[len(log_level)-1].rjust(8).upper()}]"
+        # msgdate= f"{datetime.strftime(datetime.now(), LOG_DATE_FORMAT)}"
+        class_fun = f"[{module_name.rjust(10)}.{function_name.ljust(10)}]"
+
+        msg = f"- {class_fun} - {log_level} : {msg}"
         return msg
 
     def debug(self, msg, *args, **kwargs):
         self.logger.debug(self.msg(msg), *args, **kwargs)
 
     def info(self, msg, *args, **kwargs):
         self.logger.info(self.msg(msg), *args, **kwargs)
```

### Comparing `pyloggerutils-0.1.3/pyloggerutils.egg-info/PKG-INFO` & `pyloggerutils-0.1.4/pyloggerutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyloggerutils
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is Python Logger
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.3.tar.gz
+Download-URL: https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.4.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Logger,Easy,PySy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyloggerutils-0.1.3/setup.py` & `pyloggerutils-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'pyloggerutils',         # How you named your package folder (MyLib)
   packages = ['pyloggerutils'],   # Chose the same as "name"
-  version = '0.1.3',      # Start with a small number and increase it with every change you make
+  version = '0.1.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = """This is Python Logger""",   # Give a short description about your library
   author = 'Sabari Rajan',                   # Type in your name
   author_email = 'mailme@isbarirajan.com',      # Type in your E-Mail
   url = 'https://github.com/ISabariRajan',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.3.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ISabariRajan/pyloggerutils/archive/refs/tags/v-0.1.4.tar.gz',    # I explain this later on
   keywords = ['Logger', 'Easy', 'PySy'],   # Keywords that define your package best
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

