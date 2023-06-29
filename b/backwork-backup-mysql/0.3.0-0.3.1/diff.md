# Comparing `tmp/backwork-backup-mysql-0.3.0.tar.gz` & `tmp/backwork-backup-mysql-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backwork-backup-mysql-0.3.0.tar", last modified: Sat Aug 17 23:44:07 2019, max compression
+gzip compressed data, was "backwork-backup-mysql-0.3.1.tar", last modified: Thu Jun 29 17:20:26 2023, max compression
```

## Comparing `backwork-backup-mysql-0.3.0.tar` & `backwork-backup-mysql-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3947 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2558 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3947 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/entry_points.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-17 23:44:07.000000 backwork-backup-mysql-0.3.0/mysql/
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/mysql/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4053 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/mysql/mysql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1410 2019-08-17 23:43:41.000000 backwork-backup-mysql-0.3.0/setup.py
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:20:26.944483 backwork-backup-mysql-0.3.1/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1081 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/CHANGELOG.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      477 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)    11357 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/LICENSE
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       13 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/MANIFEST.in
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     3362 2023-06-29 17:20:26.944305 backwork-backup-mysql-0.3.1/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2558 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/README.md
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:20:26.943384 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     3362 2023-06-29 17:20:26.000000 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      372 2023-06-29 17:20:26.000000 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        1 2023-06-29 17:20:26.000000 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       93 2023-06-29 17:20:26.000000 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        9 2023-06-29 17:20:26.000000 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/requires.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        6 2023-06-29 17:20:26.000000 backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/top_level.txt
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:20:26.943956 backwork-backup-mysql-0.3.1/mysql/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      101 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/mysql/__init__.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     4053 2023-06-29 17:18:31.000000 backwork-backup-mysql-0.3.1/mysql/mysql.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       38 2023-06-29 17:20:26.944539 backwork-backup-mysql-0.3.1/setup.cfg
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1355 2023-06-29 17:19:19.000000 backwork-backup-mysql-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backwork-backup-mysql-0.3.0/PKG-INFO` & `backwork-backup-mysql-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 Metadata-Version: 2.1
 Name: backwork-backup-mysql
-Version: 0.3.0
+Version: 0.3.1
 Summary: Backwork plug-in for MySQL backups.
 Home-page: https://github.com/IBM/backwork-backup-mysql
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-mysql [![Build Status](https://travis-ci.org/IBM/backwork-backup-mysql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mysql) [![PyPI version](https://badge.fury.io/py/backwork-backup-mysql.svg)](https://badge.fury.io/py/backwork-backup-mysql)
-        Add support for MySQL backups on [`backwork`](https://github.com/IBM/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`mysqldump`](http://dev.mysql.com/doc/refman/en/mysqldump.html),
-        so you will need to it installed.
-        
-        `mysqldump` is part of the `mysql` client.cd .
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-mysql
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup mysql` and `restore mysql` commands
-        on `backwork`:
-        
-        
-        #### backwork backup mysql
-        ```sh
-        $ backwork backup mysql -h
-        usage: backwork backup mysql [-h] [--gzip] [-o OUTPUT]
-        
-        Backup a MySQL database. It uses `mysqldump` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `mysqldump`. Use `mysqldump -h` for more information.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --gzip                compress output file  (requires gzip to be installed)
-          -o OUTPUT, --output OUTPUT
-                                output file path
-        ```
-        
-        You can pass any option that you would normally use on `mysqldump`:
-        
-        ```sh
-        $ backwork backup mysql --host 192.168.99.1 -u root -ppassword --port 32769 --all-databases
-        ```
-        
-        As shown in the `--help` message, there are two extra arguments you can use in
-        your backup process `--gzip` and `-o`.
-        
-        `--gzip` will compress the output and requires the `gzip` command to be
-        available in your system.
-        
-        `-o OUTPUT` or `--output OUTPUT` will save the output of `mysqldump` into a
-        file.
-        
-        #### backwork restore mysql
-        
-        ```sh
-        usage: backwork restore mysql [-h] [--gzip] [-i INPUT]
-        
-        Restore MySQL databases. It uses `mysql` so it's required to have it
-        installed and added to the system's PATH.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --gzip                decompress backup file before restoring (requires gzip to be installed)
-          ```
-        
-        You can pass any option that you would normally use to connect to your mysql instance:
-        
-        ```sh
-        $ backwork restore mysql --host 192.168.99.1 -u root -ppassword --port 32769 --gzip --input=="mybackup.archive.gz"
-        ```
-        
-        **Important:** There is a conflict with the `-h` argument since it is reserved
-        for the help/usage message. User `--host` to pass the hostname.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 2 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# backwork-backup-mysql [![Build Status](https://travis-ci.org/IBM/backwork-backup-mysql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mysql) [![PyPI version](https://badge.fury.io/py/backwork-backup-mysql.svg)](https://badge.fury.io/py/backwork-backup-mysql)
+Add support for MySQL backups on [`backwork`](https://github.com/IBM/backwork).
+
+## Requirements
+This plug-in is build on top of [`mysqldump`](http://dev.mysql.com/doc/refman/en/mysqldump.html),
+so you will need to it installed.
+
+`mysqldump` is part of the `mysql` client.cd .
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-mysql
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup mysql` and `restore mysql` commands
+on `backwork`:
+
+
+#### backwork backup mysql
+```sh
+$ backwork backup mysql -h
+usage: backwork backup mysql [-h] [--gzip] [-o OUTPUT]
+
+Backup a MySQL database. It uses `mysqldump` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `mysqldump`. Use `mysqldump -h` for more information.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --gzip                compress output file  (requires gzip to be installed)
+  -o OUTPUT, --output OUTPUT
+                        output file path
+```
+
+You can pass any option that you would normally use on `mysqldump`:
+
+```sh
+$ backwork backup mysql --host 192.168.99.1 -u root -ppassword --port 32769 --all-databases
+```
+
+As shown in the `--help` message, there are two extra arguments you can use in
+your backup process `--gzip` and `-o`.
+
+`--gzip` will compress the output and requires the `gzip` command to be
+available in your system.
+
+`-o OUTPUT` or `--output OUTPUT` will save the output of `mysqldump` into a
+file.
+
+#### backwork restore mysql
+
+```sh
+usage: backwork restore mysql [-h] [--gzip] [-i INPUT]
+
+Restore MySQL databases. It uses `mysql` so it's required to have it
+installed and added to the system's PATH.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --gzip                decompress backup file before restoring (requires gzip to be installed)
+  ```
+
+You can pass any option that you would normally use to connect to your mysql instance:
+
+```sh
+$ backwork restore mysql --host 192.168.99.1 -u root -ppassword --port 32769 --gzip --input=="mybackup.archive.gz"
+```
+
+**Important:** There is a conflict with the `-h` argument since it is reserved
+for the help/usage message. User `--host` to pass the hostname.
```

### Comparing `backwork-backup-mysql-0.3.0/README.md` & `backwork-backup-mysql-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-mysql-0.3.0/backwork_backup_mysql.egg-info/PKG-INFO` & `backwork-backup-mysql-0.3.1/backwork_backup_mysql.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 Metadata-Version: 2.1
 Name: backwork-backup-mysql
-Version: 0.3.0
+Version: 0.3.1
 Summary: Backwork plug-in for MySQL backups.
 Home-page: https://github.com/IBM/backwork-backup-mysql
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-mysql [![Build Status](https://travis-ci.org/IBM/backwork-backup-mysql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mysql) [![PyPI version](https://badge.fury.io/py/backwork-backup-mysql.svg)](https://badge.fury.io/py/backwork-backup-mysql)
-        Add support for MySQL backups on [`backwork`](https://github.com/IBM/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`mysqldump`](http://dev.mysql.com/doc/refman/en/mysqldump.html),
-        so you will need to it installed.
-        
-        `mysqldump` is part of the `mysql` client.cd .
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-mysql
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup mysql` and `restore mysql` commands
-        on `backwork`:
-        
-        
-        #### backwork backup mysql
-        ```sh
-        $ backwork backup mysql -h
-        usage: backwork backup mysql [-h] [--gzip] [-o OUTPUT]
-        
-        Backup a MySQL database. It uses `mysqldump` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `mysqldump`. Use `mysqldump -h` for more information.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --gzip                compress output file  (requires gzip to be installed)
-          -o OUTPUT, --output OUTPUT
-                                output file path
-        ```
-        
-        You can pass any option that you would normally use on `mysqldump`:
-        
-        ```sh
-        $ backwork backup mysql --host 192.168.99.1 -u root -ppassword --port 32769 --all-databases
-        ```
-        
-        As shown in the `--help` message, there are two extra arguments you can use in
-        your backup process `--gzip` and `-o`.
-        
-        `--gzip` will compress the output and requires the `gzip` command to be
-        available in your system.
-        
-        `-o OUTPUT` or `--output OUTPUT` will save the output of `mysqldump` into a
-        file.
-        
-        #### backwork restore mysql
-        
-        ```sh
-        usage: backwork restore mysql [-h] [--gzip] [-i INPUT]
-        
-        Restore MySQL databases. It uses `mysql` so it's required to have it
-        installed and added to the system's PATH.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --gzip                decompress backup file before restoring (requires gzip to be installed)
-          ```
-        
-        You can pass any option that you would normally use to connect to your mysql instance:
-        
-        ```sh
-        $ backwork restore mysql --host 192.168.99.1 -u root -ppassword --port 32769 --gzip --input=="mybackup.archive.gz"
-        ```
-        
-        **Important:** There is a conflict with the `-h` argument since it is reserved
-        for the help/usage message. User `--host` to pass the hostname.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 2 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# backwork-backup-mysql [![Build Status](https://travis-ci.org/IBM/backwork-backup-mysql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mysql) [![PyPI version](https://badge.fury.io/py/backwork-backup-mysql.svg)](https://badge.fury.io/py/backwork-backup-mysql)
+Add support for MySQL backups on [`backwork`](https://github.com/IBM/backwork).
+
+## Requirements
+This plug-in is build on top of [`mysqldump`](http://dev.mysql.com/doc/refman/en/mysqldump.html),
+so you will need to it installed.
+
+`mysqldump` is part of the `mysql` client.cd .
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-mysql
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup mysql` and `restore mysql` commands
+on `backwork`:
+
+
+#### backwork backup mysql
+```sh
+$ backwork backup mysql -h
+usage: backwork backup mysql [-h] [--gzip] [-o OUTPUT]
+
+Backup a MySQL database. It uses `mysqldump` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `mysqldump`. Use `mysqldump -h` for more information.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --gzip                compress output file  (requires gzip to be installed)
+  -o OUTPUT, --output OUTPUT
+                        output file path
+```
+
+You can pass any option that you would normally use on `mysqldump`:
+
+```sh
+$ backwork backup mysql --host 192.168.99.1 -u root -ppassword --port 32769 --all-databases
+```
+
+As shown in the `--help` message, there are two extra arguments you can use in
+your backup process `--gzip` and `-o`.
+
+`--gzip` will compress the output and requires the `gzip` command to be
+available in your system.
+
+`-o OUTPUT` or `--output OUTPUT` will save the output of `mysqldump` into a
+file.
+
+#### backwork restore mysql
+
+```sh
+usage: backwork restore mysql [-h] [--gzip] [-i INPUT]
+
+Restore MySQL databases. It uses `mysql` so it's required to have it
+installed and added to the system's PATH.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --gzip                decompress backup file before restoring (requires gzip to be installed)
+  ```
+
+You can pass any option that you would normally use to connect to your mysql instance:
+
+```sh
+$ backwork restore mysql --host 192.168.99.1 -u root -ppassword --port 32769 --gzip --input=="mybackup.archive.gz"
+```
+
+**Important:** There is a conflict with the `-h` argument since it is reserved
+for the help/usage message. User `--host` to pass the hostname.
```

### Comparing `backwork-backup-mysql-0.3.0/mysql/mysql.py` & `backwork-backup-mysql-0.3.1/mysql/mysql.py`

 * *Files identical despite different names*

### Comparing `backwork-backup-mysql-0.3.0/CHANGELOG.md` & `backwork-backup-mysql-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-mysql-0.3.0/setup.py` & `backwork-backup-mysql-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Add support for MySQL backups
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
     name="backwork-backup-mysql",
-    version="0.3.0",
+    version="0.3.1",
     description="Backwork plug-in for MySQL backups.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/backwork-backup-mysql",
     author="Luiz Aoqui",
     author_email="laoqui@ca.ibm.com",
     license="Apache 2",
@@ -24,25 +25,19 @@
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 2 :: Only",
-        'License :: OSI Approved :: Apache Software License',
+        "License :: OSI Approved :: Apache Software License",
         "Topic :: Database",
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
-            "mysql=mysql:MySQLBackup"
-        ],
-        "backwork.restores": [
-            "mysql=mysql:MySQLRestore"
-        ],
-    }
+        "backwork.backups": ["mysql=mysql:MySQLBackup"],
+        "backwork.restores": ["mysql=mysql:MySQLRestore"],
+    },
 )
```

