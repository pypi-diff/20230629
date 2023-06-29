# Comparing `tmp/backwork-0.2.0.tar.gz` & `tmp/backwork-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backwork-0.2.0.tar", last modified: Wed Aug 14 20:11:57 2019, max compression
+gzip compressed data, was "dist/backwork-0.3.0.tar", last modified: Sat Aug 17 23:00:16 2019, max compression
```

## Comparing `backwork-0.2.0.tar` & `backwork-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-14 20:11:57.000000 backwork-0.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-08-14 20:11:33.000000 backwork-0.2.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    13305 2019-08-14 20:11:57.000000 backwork-0.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10000 2019-08-14 20:11:33.000000 backwork-0.2.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/notifiers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      811 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/lib/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1191 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/upload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1627 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/backup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1259 2019-08-14 20:11:33.000000 backwork-0.2.0/backwork/backwork.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-14 20:11:57.000000 backwork-0.2.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13305 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      355 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       44 2019-08-14 20:11:57.000000 backwork-0.2.0/backwork.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      605 2019-08-14 20:11:33.000000 backwork-0.2.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2019-08-14 20:11:33.000000 backwork-0.2.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:00:16.000000 backwork-0.3.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-08-17 22:59:54.000000 backwork-0.3.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15525 2019-08-17 23:00:16.000000 backwork-0.3.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11780 2019-08-17 22:59:54.000000 backwork-0.3.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      477 2019-08-17 22:59:54.000000 backwork-0.3.0/CONTRIBUTING.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1278 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/show.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/notifiers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      811 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/lib/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/lib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1191 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/upload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/restore.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1266 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/download.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1627 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/backup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      209 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1666 2019-08-17 22:59:54.000000 backwork-0.3.0/backwork/backwork.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-17 23:00:16.000000 backwork-0.3.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15525 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      429 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       44 2019-08-17 23:00:16.000000 backwork-0.3.0/backwork.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      695 2019-08-17 22:59:54.000000 backwork-0.3.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2019-08-17 22:59:54.000000 backwork-0.3.0/setup.py
```

### Comparing `backwork-0.2.0/PKG-INFO` & `backwork-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 Metadata-Version: 2.1
 Name: backwork
-Version: 0.2.0
+Version: 0.3.0
 Summary: Backup made easy.
 Home-page: https://github.com/ibm/backwork
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
 Description: # backwork [![Build Status](https://travis-ci.org/IBM/backwork.svg?branch=master)](https://travis-ci.org/IBM/backwork) [![PyPI version](https://badge.fury.io/py/backwork.svg)](https://badge.fury.io/py/backwork)
         Backup simplified.
         
-        `backwork` is a toolkit that simplifies the process of backing up databases. It
-        handles the backup process itself as well as upload and error notification.
+        `backwork` is a toolkit that simplifies the process of backing up and restoring databases. It
+        handles the backup process itself as well as upload, download, restoration, and error notification.
         
         ## Prerequisites
         * Python 2.7
         
         ## Installing
         You can install `backwork` using `pip`:
         ```sh
         $ pip install backwork
         ```
         
         ## Running
         After installing you should have a `backwork` command available.
         ```
         $ backwork --help
-        usage: backwork [-h] [-n NOTIFIERS] {backup,upload} ...
+        usage: backwork [-h] [-n NOTIFIERS] {backup,restore,upload,download} ...
         
         positional arguments:
-          {backup,upload}
+          {backup,restore,upload,download}
         
         optional arguments:
           -h, --help            show this help message and exit
           -n NOTIFIERS, --notify NOTIFIERS
                                 enable a notifier, it can be used multiple times
         ```
         
         ## Plug-ins
         Just having `backwork` is not enough. You will need to the plug-ins that
-        suit your needs. You can install plugins by running:
+        suit your needs. You can install plug-ins by running:
         ```sh
-        $ pip install <plugin_name>
+        $ pip install <plug-in_name>
         ```
+        You can discover available plug-ins by [viewing the `backwork-plugin` topic on Github.](https://github.com/topics/backwork-plugin)
         
         Plug-ins are divided into three categories:
         
         ### Backup
-        Backup plugins are responsible for connecting to a databases and doing the
-        actual backup process.
+        Backup plug-ins are responsible for connecting to databases and doing the
+        actual backup process, as well as the restore process for the backups.
+        You can discover available backup plug-ins by [viewing the `backwork-plugin-backup` topic on Github.](https://github.com/topics/backwork-plugin-backup)
         
-        Once you install a backup plug-in it will be available via the `backwork backup`
-        command:
+        Once you install a backup plug-in it will be available via the `backwork backup` and `backwork restore` commands:
         ```sh
         $ backwork backup --help
         usage: backwork backup [-h] [-U] {mongo} ...
         
         Perform database backups. Run `backwork backup {database_type} -h` for more
         details on each supported database.
         
@@ -63,40 +64,85 @@
         
         optional arguments:
           -h, --help    show this help message and exit
           -U, --upload  output backup data to stdout to allow piping it to an upload
                         command
         ```
         
-        #### Available plugin-ins:
-        * [backwork-backup-mongo](https://github.ibm.com/apset/backwork-backup-mongo)
+        ```
+        usage: backwork restore [-h] [-U] {mongo} ...
+        
+        Perform database restores. Run `backwork restore {database_type} -h` for more
+        details on each supported database.
+        
+        positional arguments:
+          {mongo}
+        
+        optional arguments:
+          -h, --help    show this help message and exit
+        ```
+        
+        
+        #### Available plug-ins:
+        * `backwork-backup-mongo`
         
         ### Upload
-        Upload plug-ins store your backup files securely in a remote storage.
+        Upload plug-ins store and retrieve your backup files securely from remote storage.
+        You can discover available upload plug-ins by [viewing the `backwork-plugin-upload` topic on Github.](https://github.com/topics/backwork-plugin-upload)
         
-        You can use them with the `backwork upload` command:
+        You can use them with the `backwork upload`, `backwork show`, and `backwork download` commands:
         ```sh
         $ backwork upload --help
         usage: backwork upload [-h] {softlayer} ...
         
         Upload a file to remote service. Run `backwork upload {service} -h` for more
         details on each supported service.
         
         positional arguments:
           {softlayer}
         
         optional arguments:
           -h, --help   show this help message and exit
         ```
-        #### Available plugin-ins:
-        * [backwork-upload-softlayer](https://github.ibm.com/apset/backwork-upload-softlayer)
+        
+        ```sh
+        $ backwork show --help
+        usage: backwork show [-h] {cos} ...
+        
+        Shows available backups on a remote service. Run `backwork show {service} -h` for
+        more details on each supported service.
+        
+        positional arguments:
+          {cos}
+        
+        optional arguments:
+          -h, --help  show this help message and exit
+        ```
+        
+        ```sh
+        $ backwork download --help
+        usage: backwork download [-h] {softlayer} ...
+        
+        Download a file from a remote service. Run `backwork upload {service} -h` for more
+        details on each supported service.
+        
+        positional arguments:
+          {softlayer}
+        
+        optional arguments:
+          -h, --help   show this help message and exit
+        ```
+        
+        #### Available plug-ins:
+        * `backwork-upload-softlayer`
         
         ### Notifiers
         Notifiers tell you when things go wrong. More important than having a backup
         process configured is knowing when this process fails.
+        You can discover available notifier plug-ins by [viewing the `backwork-plugin-notifier` topic on Github.](https://github.com/topics/backwork-plugin-notifier)
         
         Notifiers are enabled on the `backwork` command using the `-n` or `--notify`
         arguments. They may also require some extra values, such API keys.
         
         ```sh
         $ backwork --help
         usage: backwork [-h] [-n NOTIFIERS] [--sentry-dsn SENTRY_DSN]
@@ -113,15 +159,15 @@
                                 Sentry DSN to be used for notifications. It can also
                                 be set with the evironment variable $SENTRY_DSN.
         ```
         
         You can enable as many notifiers as you want on a command.
         
         **Available plug-ins:**
-        * [backwork-notify-sentry](https://github.ibm.com/apset/backwork-notify-sentry)
+        * `backwork-notify-sentry`
         
         ## Examples
         #### Backup a MongoDB database running locally
         ```sh
         $ backwork backup mongo
         2017-01-15 03:58:15,270 backup.mongo INFO    starting mongo backup...
         2017-01-15 03:58:15,270 backup.mongo INFO    saving file to /Users/laoqui/Projects/backwork/dumps/mongo_backup_20170115-035815.archive.gz
@@ -271,38 +317,47 @@
                 If `msg` is an exception, the call to this method will be in the context
                 of an `except`, meaning you will be able to access `sys.exc_info()`.
                 """
                 raise NotImplementedError("Base method not overriden.")
         ```
         
         To make your package visible to `backwork` you will also need to declare an
-        [`entry_point`](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plugins)
+        [`entry_point`](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plug-ins)
         in your `setup.py` file.
         
         Each plug-in type has a different `entry_point` key:
         
         #### Backups:
         ```python
         setup(
             ...
             entry_points={
                 "backwork.backups": [
                     "<COMMAND NAME>": "module:BackupClass"
+                ],
+                "backwork.restores": [
+                    "<COMMAND NAME>": "module:RestoreClass"
                 ]
             },
             ...
         ```
         
         #### Uploads:
         ```python
         setup(
             ...
             entry_points={
                 "backwork.uploads": [
                     "<COMMAND NAME>": "module:UploadClass"
+                ],
+                "backwork.shows": [
+                    "<COMMAND NAME>": "module:ShowClass"
+                ]
+                "backwork.downloads": [
+                    "<COMMAND NAME>": "module:DownloadClass"
                 ]
             },
             ...
         ```
         
         #### Notifiers:
         ```python
```

### Comparing `backwork-0.2.0/README.md` & `backwork-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # backwork [![Build Status](https://travis-ci.org/IBM/backwork.svg?branch=master)](https://travis-ci.org/IBM/backwork) [![PyPI version](https://badge.fury.io/py/backwork.svg)](https://badge.fury.io/py/backwork)
 Backup simplified.
 
-`backwork` is a toolkit that simplifies the process of backing up databases. It
-handles the backup process itself as well as upload and error notification.
+`backwork` is a toolkit that simplifies the process of backing up and restoring databases. It
+handles the backup process itself as well as upload, download, restoration, and error notification.
 
 ## Prerequisites
 * Python 2.7
 
 ## Installing
 You can install `backwork` using `pip`:
 ```sh
 $ pip install backwork
 ```
 
 ## Running
 After installing you should have a `backwork` command available.
 ```
 $ backwork --help
-usage: backwork [-h] [-n NOTIFIERS] {backup,upload} ...
+usage: backwork [-h] [-n NOTIFIERS] {backup,restore,upload,download} ...
 
 positional arguments:
-  {backup,upload}
+  {backup,restore,upload,download}
 
 optional arguments:
   -h, --help            show this help message and exit
   -n NOTIFIERS, --notify NOTIFIERS
                         enable a notifier, it can be used multiple times
 ```
 
 ## Plug-ins
 Just having `backwork` is not enough. You will need to the plug-ins that
-suit your needs. You can install plugins by running:
+suit your needs. You can install plug-ins by running:
 ```sh
-$ pip install <plugin_name>
+$ pip install <plug-in_name>
 ```
+You can discover available plug-ins by [viewing the `backwork-plugin` topic on Github.](https://github.com/topics/backwork-plugin)
 
 Plug-ins are divided into three categories:
 
 ### Backup
-Backup plugins are responsible for connecting to a databases and doing the
-actual backup process.
+Backup plug-ins are responsible for connecting to databases and doing the
+actual backup process, as well as the restore process for the backups.
+You can discover available backup plug-ins by [viewing the `backwork-plugin-backup` topic on Github.](https://github.com/topics/backwork-plugin-backup)
 
-Once you install a backup plug-in it will be available via the `backwork backup`
-command:
+Once you install a backup plug-in it will be available via the `backwork backup` and `backwork restore` commands:
 ```sh
 $ backwork backup --help
 usage: backwork backup [-h] [-U] {mongo} ...
 
 Perform database backups. Run `backwork backup {database_type} -h` for more
 details on each supported database.
 
@@ -55,40 +56,85 @@
 
 optional arguments:
   -h, --help    show this help message and exit
   -U, --upload  output backup data to stdout to allow piping it to an upload
                 command
 ```
 
-#### Available plugin-ins:
-* [backwork-backup-mongo](https://github.ibm.com/apset/backwork-backup-mongo)
+```
+usage: backwork restore [-h] [-U] {mongo} ...
+
+Perform database restores. Run `backwork restore {database_type} -h` for more
+details on each supported database.
+
+positional arguments:
+  {mongo}
+
+optional arguments:
+  -h, --help    show this help message and exit
+```
+
+
+#### Available plug-ins:
+* `backwork-backup-mongo`
 
 ### Upload
-Upload plug-ins store your backup files securely in a remote storage.
+Upload plug-ins store and retrieve your backup files securely from remote storage.
+You can discover available upload plug-ins by [viewing the `backwork-plugin-upload` topic on Github.](https://github.com/topics/backwork-plugin-upload)
 
-You can use them with the `backwork upload` command:
+You can use them with the `backwork upload`, `backwork show`, and `backwork download` commands:
 ```sh
 $ backwork upload --help
 usage: backwork upload [-h] {softlayer} ...
 
 Upload a file to remote service. Run `backwork upload {service} -h` for more
 details on each supported service.
 
 positional arguments:
   {softlayer}
 
 optional arguments:
   -h, --help   show this help message and exit
 ```
-#### Available plugin-ins:
-* [backwork-upload-softlayer](https://github.ibm.com/apset/backwork-upload-softlayer)
+
+```sh
+$ backwork show --help
+usage: backwork show [-h] {cos} ...
+
+Shows available backups on a remote service. Run `backwork show {service} -h` for
+more details on each supported service.
+
+positional arguments:
+  {cos}
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+```sh
+$ backwork download --help
+usage: backwork download [-h] {softlayer} ...
+
+Download a file from a remote service. Run `backwork upload {service} -h` for more
+details on each supported service.
+
+positional arguments:
+  {softlayer}
+
+optional arguments:
+  -h, --help   show this help message and exit
+```
+
+#### Available plug-ins:
+* `backwork-upload-softlayer`
 
 ### Notifiers
 Notifiers tell you when things go wrong. More important than having a backup
 process configured is knowing when this process fails.
+You can discover available notifier plug-ins by [viewing the `backwork-plugin-notifier` topic on Github.](https://github.com/topics/backwork-plugin-notifier)
 
 Notifiers are enabled on the `backwork` command using the `-n` or `--notify`
 arguments. They may also require some extra values, such API keys.
 
 ```sh
 $ backwork --help
 usage: backwork [-h] [-n NOTIFIERS] [--sentry-dsn SENTRY_DSN]
@@ -105,15 +151,15 @@
                         Sentry DSN to be used for notifications. It can also
                         be set with the evironment variable $SENTRY_DSN.
 ```
 
 You can enable as many notifiers as you want on a command.
 
 **Available plug-ins:**
-* [backwork-notify-sentry](https://github.ibm.com/apset/backwork-notify-sentry)
+* `backwork-notify-sentry`
 
 ## Examples
 #### Backup a MongoDB database running locally
 ```sh
 $ backwork backup mongo
 2017-01-15 03:58:15,270 backup.mongo INFO    starting mongo backup...
 2017-01-15 03:58:15,270 backup.mongo INFO    saving file to /Users/laoqui/Projects/backwork/dumps/mongo_backup_20170115-035815.archive.gz
@@ -263,38 +309,47 @@
         If `msg` is an exception, the call to this method will be in the context
         of an `except`, meaning you will be able to access `sys.exc_info()`.
         """
         raise NotImplementedError("Base method not overriden.")
 ```
 
 To make your package visible to `backwork` you will also need to declare an
-[`entry_point`](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plugins)
+[`entry_point`](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plug-ins)
 in your `setup.py` file.
 
 Each plug-in type has a different `entry_point` key:
 
 #### Backups:
 ```python
 setup(
     ...
     entry_points={
         "backwork.backups": [
             "<COMMAND NAME>": "module:BackupClass"
+        ],
+        "backwork.restores": [
+            "<COMMAND NAME>": "module:RestoreClass"
         ]
     },
     ...
 ```
 
 #### Uploads:
 ```python
 setup(
     ...
     entry_points={
         "backwork.uploads": [
             "<COMMAND NAME>": "module:UploadClass"
+        ],
+        "backwork.shows": [
+            "<COMMAND NAME>": "module:ShowClass"
+        ]
+        "backwork.downloads": [
+            "<COMMAND NAME>": "module:DownloadClass"
         ]
     },
     ...
 ```
 
 #### Notifiers:
 ```python
```

### Comparing `backwork-0.2.0/backwork/notifiers.py` & `backwork-0.3.0/backwork/notifiers.py`

 * *Files identical despite different names*

### Comparing `backwork-0.2.0/backwork/lib/utils.py` & `backwork-0.3.0/backwork/lib/utils.py`

 * *Files identical despite different names*

### Comparing `backwork-0.2.0/backwork/upload.py` & `backwork-0.3.0/backwork/upload.py`

 * *Files identical despite different names*

### Comparing `backwork-0.2.0/backwork/backup.py` & `backwork-0.3.0/backwork/backup.py`

 * *Files identical despite different names*

### Comparing `backwork-0.2.0/backwork/backwork.py` & `backwork-0.3.0/backwork/backwork.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 """
 
 import argparse
 import logging
 import sys
 
 from . import backup
+from . import restore
 from . import notifiers
 from . import upload
+from . import show
+from . import download
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO,
                     format="%(asctime)s %(name)s %(levelname)-7s %(message)s")
 
 LOG = logging.getLogger(__name__)
 
 
@@ -25,28 +28,40 @@
 
     # parse notifier arguments
     notifiers.parse_args(parser)
 
     # parse subcommand
     subparsers = parser.add_subparsers(dest="command")
     backup.parse_args(subparsers)
+    restore.parse_args(subparsers)
     upload.parse_args(subparsers)
+    show.parse_args(subparsers)
+    download.parse_args(subparsers)
 
     return parser.parse_known_args()
 
 
 def main():
     """Core functionality."""
     args, extra = parse_args()
     notifiers.initialize(args, extra)
 
     try:
         if args.command == "backup":
             backup.backup(args, extra)
 
+        elif args.command == "restore":
+            restore.restore(args, extra)
+
         elif args.command == "upload":
             upload.upload(args, extra)
 
+        elif args.command == "show":
+            show.show(args, extra)
+
+        elif args.command == "download":
+            download.download(args, extra)
+
     except Exception as error:  # pylint: disable=broad-except
         notifiers.notify(error)
         LOG.exception(error)
         sys.exit(1)
```

### Comparing `backwork-0.2.0/backwork.egg-info/PKG-INFO` & `backwork-0.3.0/backwork.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 Metadata-Version: 2.1
 Name: backwork
-Version: 0.2.0
+Version: 0.3.0
 Summary: Backup made easy.
 Home-page: https://github.com/ibm/backwork
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
 Description: # backwork [![Build Status](https://travis-ci.org/IBM/backwork.svg?branch=master)](https://travis-ci.org/IBM/backwork) [![PyPI version](https://badge.fury.io/py/backwork.svg)](https://badge.fury.io/py/backwork)
         Backup simplified.
         
-        `backwork` is a toolkit that simplifies the process of backing up databases. It
-        handles the backup process itself as well as upload and error notification.
+        `backwork` is a toolkit that simplifies the process of backing up and restoring databases. It
+        handles the backup process itself as well as upload, download, restoration, and error notification.
         
         ## Prerequisites
         * Python 2.7
         
         ## Installing
         You can install `backwork` using `pip`:
         ```sh
         $ pip install backwork
         ```
         
         ## Running
         After installing you should have a `backwork` command available.
         ```
         $ backwork --help
-        usage: backwork [-h] [-n NOTIFIERS] {backup,upload} ...
+        usage: backwork [-h] [-n NOTIFIERS] {backup,restore,upload,download} ...
         
         positional arguments:
-          {backup,upload}
+          {backup,restore,upload,download}
         
         optional arguments:
           -h, --help            show this help message and exit
           -n NOTIFIERS, --notify NOTIFIERS
                                 enable a notifier, it can be used multiple times
         ```
         
         ## Plug-ins
         Just having `backwork` is not enough. You will need to the plug-ins that
-        suit your needs. You can install plugins by running:
+        suit your needs. You can install plug-ins by running:
         ```sh
-        $ pip install <plugin_name>
+        $ pip install <plug-in_name>
         ```
+        You can discover available plug-ins by [viewing the `backwork-plugin` topic on Github.](https://github.com/topics/backwork-plugin)
         
         Plug-ins are divided into three categories:
         
         ### Backup
-        Backup plugins are responsible for connecting to a databases and doing the
-        actual backup process.
+        Backup plug-ins are responsible for connecting to databases and doing the
+        actual backup process, as well as the restore process for the backups.
+        You can discover available backup plug-ins by [viewing the `backwork-plugin-backup` topic on Github.](https://github.com/topics/backwork-plugin-backup)
         
-        Once you install a backup plug-in it will be available via the `backwork backup`
-        command:
+        Once you install a backup plug-in it will be available via the `backwork backup` and `backwork restore` commands:
         ```sh
         $ backwork backup --help
         usage: backwork backup [-h] [-U] {mongo} ...
         
         Perform database backups. Run `backwork backup {database_type} -h` for more
         details on each supported database.
         
@@ -63,40 +64,85 @@
         
         optional arguments:
           -h, --help    show this help message and exit
           -U, --upload  output backup data to stdout to allow piping it to an upload
                         command
         ```
         
-        #### Available plugin-ins:
-        * [backwork-backup-mongo](https://github.ibm.com/apset/backwork-backup-mongo)
+        ```
+        usage: backwork restore [-h] [-U] {mongo} ...
+        
+        Perform database restores. Run `backwork restore {database_type} -h` for more
+        details on each supported database.
+        
+        positional arguments:
+          {mongo}
+        
+        optional arguments:
+          -h, --help    show this help message and exit
+        ```
+        
+        
+        #### Available plug-ins:
+        * `backwork-backup-mongo`
         
         ### Upload
-        Upload plug-ins store your backup files securely in a remote storage.
+        Upload plug-ins store and retrieve your backup files securely from remote storage.
+        You can discover available upload plug-ins by [viewing the `backwork-plugin-upload` topic on Github.](https://github.com/topics/backwork-plugin-upload)
         
-        You can use them with the `backwork upload` command:
+        You can use them with the `backwork upload`, `backwork show`, and `backwork download` commands:
         ```sh
         $ backwork upload --help
         usage: backwork upload [-h] {softlayer} ...
         
         Upload a file to remote service. Run `backwork upload {service} -h` for more
         details on each supported service.
         
         positional arguments:
           {softlayer}
         
         optional arguments:
           -h, --help   show this help message and exit
         ```
-        #### Available plugin-ins:
-        * [backwork-upload-softlayer](https://github.ibm.com/apset/backwork-upload-softlayer)
+        
+        ```sh
+        $ backwork show --help
+        usage: backwork show [-h] {cos} ...
+        
+        Shows available backups on a remote service. Run `backwork show {service} -h` for
+        more details on each supported service.
+        
+        positional arguments:
+          {cos}
+        
+        optional arguments:
+          -h, --help  show this help message and exit
+        ```
+        
+        ```sh
+        $ backwork download --help
+        usage: backwork download [-h] {softlayer} ...
+        
+        Download a file from a remote service. Run `backwork upload {service} -h` for more
+        details on each supported service.
+        
+        positional arguments:
+          {softlayer}
+        
+        optional arguments:
+          -h, --help   show this help message and exit
+        ```
+        
+        #### Available plug-ins:
+        * `backwork-upload-softlayer`
         
         ### Notifiers
         Notifiers tell you when things go wrong. More important than having a backup
         process configured is knowing when this process fails.
+        You can discover available notifier plug-ins by [viewing the `backwork-plugin-notifier` topic on Github.](https://github.com/topics/backwork-plugin-notifier)
         
         Notifiers are enabled on the `backwork` command using the `-n` or `--notify`
         arguments. They may also require some extra values, such API keys.
         
         ```sh
         $ backwork --help
         usage: backwork [-h] [-n NOTIFIERS] [--sentry-dsn SENTRY_DSN]
@@ -113,15 +159,15 @@
                                 Sentry DSN to be used for notifications. It can also
                                 be set with the evironment variable $SENTRY_DSN.
         ```
         
         You can enable as many notifiers as you want on a command.
         
         **Available plug-ins:**
-        * [backwork-notify-sentry](https://github.ibm.com/apset/backwork-notify-sentry)
+        * `backwork-notify-sentry`
         
         ## Examples
         #### Backup a MongoDB database running locally
         ```sh
         $ backwork backup mongo
         2017-01-15 03:58:15,270 backup.mongo INFO    starting mongo backup...
         2017-01-15 03:58:15,270 backup.mongo INFO    saving file to /Users/laoqui/Projects/backwork/dumps/mongo_backup_20170115-035815.archive.gz
@@ -271,38 +317,47 @@
                 If `msg` is an exception, the call to this method will be in the context
                 of an `except`, meaning you will be able to access `sys.exc_info()`.
                 """
                 raise NotImplementedError("Base method not overriden.")
         ```
         
         To make your package visible to `backwork` you will also need to declare an
-        [`entry_point`](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plugins)
+        [`entry_point`](https://setuptools.readthedocs.io/en/latest/setuptools.html#dynamic-discovery-of-services-and-plug-ins)
         in your `setup.py` file.
         
         Each plug-in type has a different `entry_point` key:
         
         #### Backups:
         ```python
         setup(
             ...
             entry_points={
                 "backwork.backups": [
                     "<COMMAND NAME>": "module:BackupClass"
+                ],
+                "backwork.restores": [
+                    "<COMMAND NAME>": "module:RestoreClass"
                 ]
             },
             ...
         ```
         
         #### Uploads:
         ```python
         setup(
             ...
             entry_points={
                 "backwork.uploads": [
                     "<COMMAND NAME>": "module:UploadClass"
+                ],
+                "backwork.shows": [
+                    "<COMMAND NAME>": "module:ShowClass"
+                ]
+                "backwork.downloads": [
+                    "<COMMAND NAME>": "module:DownloadClass"
                 ]
             },
             ...
         ```
         
         #### Notifiers:
         ```python
```

### Comparing `backwork-0.2.0/CHANGELOG.md` & `backwork-0.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
-## [0.2.0][] - 2019-08-14
+## [0.3.0][] - 2019-08-17
+### Added
+- Added `show`, `download`, and `restore` subcommands
 
+## [0.2.0][] - 2019-08-14
 ### Changed
 -  Changed package name from `monsoon` to `backwork`
 
 ## [0.1.7][] - 2017-06-07
 ### Fixed
 -   Version number
 -   Module includes
```

### Comparing `backwork-0.2.0/setup.py` & `backwork-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md')) as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="backwork",
-    version="0.2.0",
+    version="0.3.0",
     description="Backup made easy.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/ibm/backwork",
     author="Luiz Aoqui",
     author_email="laoqui@ca.ibm.com",
     license="Apache 2",
```

