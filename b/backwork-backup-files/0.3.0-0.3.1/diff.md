# Comparing `tmp/backwork-backup-files-0.3.0.tar.gz` & `tmp/backwork-backup-files-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backwork-backup-files-0.3.0.tar", last modified: Sun Aug 18 00:10:04 2019, max compression
+gzip compressed data, was "backwork-backup-files-0.3.1.tar", last modified: Thu Jun 29 17:16:45 2023, max compression
```

## Comparing `backwork-backup-files-0.3.0.tar` & `backwork-backup-files-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/files/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2833 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/files/files.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/files/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3514 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3514 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/backwork_backup_files.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2149 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-18 00:10:04.000000 backwork-backup-files-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1388 2019-08-18 00:09:39.000000 backwork-backup-files-0.3.0/setup.py
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:16:45.897879 backwork-backup-files-0.3.1/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      538 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/CHANGELOG.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      477 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)    11357 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/LICENSE
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       13 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/MANIFEST.in
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2929 2023-06-29 17:16:45.897721 backwork-backup-files-0.3.1/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2149 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/README.md
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:16:45.897219 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2929 2023-06-29 17:16:45.000000 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      372 2023-06-29 17:16:45.000000 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/SOURCES.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        1 2023-06-29 17:16:45.000000 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/dependency_links.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       93 2023-06-29 17:16:45.000000 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/entry_points.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        9 2023-06-29 17:16:45.000000 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/requires.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        6 2023-06-29 17:16:45.000000 backwork-backup-files-0.3.1/backwork_backup_files.egg-info/top_level.txt
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:16:45.897507 backwork-backup-files-0.3.1/files/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      127 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/files/__init__.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2833 2023-06-29 17:12:22.000000 backwork-backup-files-0.3.1/files/files.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       38 2023-06-29 17:16:45.897922 backwork-backup-files-0.3.1/setup.cfg
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1334 2023-06-29 17:12:48.000000 backwork-backup-files-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backwork-backup-files-0.3.0/files/files.py` & `backwork-backup-files-0.3.1/files/files.py`

 * *Files identical despite different names*

### Comparing `backwork-backup-files-0.3.0/PKG-INFO` & `backwork-backup-files-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: backwork-backup-files
-Version: 0.3.0
+Version: 0.3.1
 Summary: Backwork plug-in for file backups.
 Home-page: https://github.com/IBM/backwork-backup-files
 Author: Leons Petrazickis
 Author-email: leonsp@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-files [![Build Status](https://travis-ci.org/IBM/backwork-backup-files.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-files) [![PyPI version](https://badge.fury.io/py/backwork-backup-files.svg)](https://badge.fury.io/py/backwork-backup-files)
-        
-        Add support for file backups on [`backwork`](https://github.com/IBM/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`tar`](https://linux.die.net/man/1/tar).
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-files
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup files` and `restore files` commands
-        on `backwork`:
-        
-        #### backwork backup files
-        
-        ```sh
-        $ backwork backup files -h
-        usage: backwork backup files [-h] -f FILE
-        
-        Back up one or more files. It uses `tar -cz` which gzips the output. You can
-        use any of the arguments supported by `tar`. Add a list of files and
-        directories you want backed up as the last thing in the line. Use `tar --help`
-        for more information.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -o FILE, --output FILE  output gzipped file path
-        ```
-        
-        You can pass any option that you would normally use with `tar`:
-        
-        ```sh
-        $ backwork backup files -o foo.tgz --verbose /tmp /var/log
-        ```
-        
-        As shown in the `--help` message, there is one required arguments you
-        must use in your backup process.
-        
-        `-o FILE` or `--output FILE` will save the output of `tar` into a
-        file.
-        
-        #### backwork restore files
-        
-        ```sh
-        usage: backwork restore files [-h] input
-        
-        Restore one or more files from a .tar.gz file. It uses `tar xvzf`. You can
-        use any of the arguments supported by `tar`. Use `tar --help` for more
-        information.
-        
-        positional arguments:
-          input       .tar.gz file to restore from
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        **Important:** There is a conflict with the `-h` argument since it is reserved
-        for the help/usage message. Use `--dereference` to follow symlinks.
-        
-        ## Building and Publishing
-        
-        Travis will publish builds for you. To build, push a tag to the repo:
-        
-        ```
-        git tag -a v0.1.2 -m 'v0.1.2'
-        git push --tags
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 2 :: Only
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# backwork-backup-files [![Build Status](https://travis-ci.org/IBM/backwork-backup-files.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-files) [![PyPI version](https://badge.fury.io/py/backwork-backup-files.svg)](https://badge.fury.io/py/backwork-backup-files)
+
+Add support for file backups on [`backwork`](https://github.com/IBM/backwork).
+
+## Requirements
+This plug-in is build on top of [`tar`](https://linux.die.net/man/1/tar).
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-files
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup files` and `restore files` commands
+on `backwork`:
+
+#### backwork backup files
+
+```sh
+$ backwork backup files -h
+usage: backwork backup files [-h] -f FILE
+
+Back up one or more files. It uses `tar -cz` which gzips the output. You can
+use any of the arguments supported by `tar`. Add a list of files and
+directories you want backed up as the last thing in the line. Use `tar --help`
+for more information.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -o FILE, --output FILE  output gzipped file path
+```
+
+You can pass any option that you would normally use with `tar`:
+
+```sh
+$ backwork backup files -o foo.tgz --verbose /tmp /var/log
+```
+
+As shown in the `--help` message, there is one required arguments you
+must use in your backup process.
+
+`-o FILE` or `--output FILE` will save the output of `tar` into a
+file.
+
+#### backwork restore files
+
+```sh
+usage: backwork restore files [-h] input
+
+Restore one or more files from a .tar.gz file. It uses `tar xvzf`. You can
+use any of the arguments supported by `tar`. Use `tar --help` for more
+information.
+
+positional arguments:
+  input       .tar.gz file to restore from
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+**Important:** There is a conflict with the `-h` argument since it is reserved
+for the help/usage message. Use `--dereference` to follow symlinks.
+
+## Building and Publishing
+
+Travis will publish builds for you. To build, push a tag to the repo:
+
+```
+git tag -a v0.1.2 -m 'v0.1.2'
+git push --tags
+```
```

### Comparing `backwork-backup-files-0.3.0/backwork_backup_files.egg-info/PKG-INFO` & `backwork-backup-files-0.3.1/backwork_backup_files.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: backwork-backup-files
-Version: 0.3.0
+Version: 0.3.1
 Summary: Backwork plug-in for file backups.
 Home-page: https://github.com/IBM/backwork-backup-files
 Author: Leons Petrazickis
 Author-email: leonsp@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-files [![Build Status](https://travis-ci.org/IBM/backwork-backup-files.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-files) [![PyPI version](https://badge.fury.io/py/backwork-backup-files.svg)](https://badge.fury.io/py/backwork-backup-files)
-        
-        Add support for file backups on [`backwork`](https://github.com/IBM/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`tar`](https://linux.die.net/man/1/tar).
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-files
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup files` and `restore files` commands
-        on `backwork`:
-        
-        #### backwork backup files
-        
-        ```sh
-        $ backwork backup files -h
-        usage: backwork backup files [-h] -f FILE
-        
-        Back up one or more files. It uses `tar -cz` which gzips the output. You can
-        use any of the arguments supported by `tar`. Add a list of files and
-        directories you want backed up as the last thing in the line. Use `tar --help`
-        for more information.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -o FILE, --output FILE  output gzipped file path
-        ```
-        
-        You can pass any option that you would normally use with `tar`:
-        
-        ```sh
-        $ backwork backup files -o foo.tgz --verbose /tmp /var/log
-        ```
-        
-        As shown in the `--help` message, there is one required arguments you
-        must use in your backup process.
-        
-        `-o FILE` or `--output FILE` will save the output of `tar` into a
-        file.
-        
-        #### backwork restore files
-        
-        ```sh
-        usage: backwork restore files [-h] input
-        
-        Restore one or more files from a .tar.gz file. It uses `tar xvzf`. You can
-        use any of the arguments supported by `tar`. Use `tar --help` for more
-        information.
-        
-        positional arguments:
-          input       .tar.gz file to restore from
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        **Important:** There is a conflict with the `-h` argument since it is reserved
-        for the help/usage message. Use `--dereference` to follow symlinks.
-        
-        ## Building and Publishing
-        
-        Travis will publish builds for you. To build, push a tag to the repo:
-        
-        ```
-        git tag -a v0.1.2 -m 'v0.1.2'
-        git push --tags
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 2 :: Only
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# backwork-backup-files [![Build Status](https://travis-ci.org/IBM/backwork-backup-files.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-files) [![PyPI version](https://badge.fury.io/py/backwork-backup-files.svg)](https://badge.fury.io/py/backwork-backup-files)
+
+Add support for file backups on [`backwork`](https://github.com/IBM/backwork).
+
+## Requirements
+This plug-in is build on top of [`tar`](https://linux.die.net/man/1/tar).
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-files
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup files` and `restore files` commands
+on `backwork`:
+
+#### backwork backup files
+
+```sh
+$ backwork backup files -h
+usage: backwork backup files [-h] -f FILE
+
+Back up one or more files. It uses `tar -cz` which gzips the output. You can
+use any of the arguments supported by `tar`. Add a list of files and
+directories you want backed up as the last thing in the line. Use `tar --help`
+for more information.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -o FILE, --output FILE  output gzipped file path
+```
+
+You can pass any option that you would normally use with `tar`:
+
+```sh
+$ backwork backup files -o foo.tgz --verbose /tmp /var/log
+```
+
+As shown in the `--help` message, there is one required arguments you
+must use in your backup process.
+
+`-o FILE` or `--output FILE` will save the output of `tar` into a
+file.
+
+#### backwork restore files
+
+```sh
+usage: backwork restore files [-h] input
+
+Restore one or more files from a .tar.gz file. It uses `tar xvzf`. You can
+use any of the arguments supported by `tar`. Use `tar --help` for more
+information.
+
+positional arguments:
+  input       .tar.gz file to restore from
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+**Important:** There is a conflict with the `-h` argument since it is reserved
+for the help/usage message. Use `--dereference` to follow symlinks.
+
+## Building and Publishing
+
+Travis will publish builds for you. To build, push a tag to the repo:
+
+```
+git tag -a v0.1.2 -m 'v0.1.2'
+git push --tags
+```
```

### Comparing `backwork-backup-files-0.3.0/README.md` & `backwork-backup-files-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-files-0.3.0/CHANGELOG.md` & `backwork-backup-files-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-files-0.3.0/setup.py` & `backwork-backup-files-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 """File backup module for Backwork
 """
 
 from os import path
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(HERE, 'README.md')) as f:
+with open(path.join(HERE, "README.md")) as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="backwork-backup-files",
-    version="0.3.0",
+    version="0.3.1",
     description="Backwork plug-in for file backups.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/backwork-backup-files",
     author="Leons Petrazickis",
     author_email="leonsp@ca.ibm.com",
     license="Apache 2",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Operating System :: POSIX :: Linux",
-        'License :: OSI Approved :: Apache Software License',
+        "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 2 :: Only",
         "Topic :: System :: Archiving :: Backup",
-        "Topic :: Utilities"
+        "Topic :: Utilities",
     ],
     packages=find_packages(),
-    install_requires=[
-        "backwork"
-    ],
+    install_requires=["backwork"],
     entry_points={
-        "backwork.backups": [
-            "files=files:FilesBackup"
-        ],
-        "backwork.restores": [
-            "files=files:FilesRestore"
-        ]
-    }
+        "backwork.backups": ["files=files:FilesBackup"],
+        "backwork.restores": ["files=files:FilesRestore"],
+    },
 )
```

