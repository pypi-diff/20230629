# Comparing `tmp/backwork-backup-postgresql-0.2.1.tar.gz` & `tmp/backwork-backup-postgresql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backwork-backup-postgresql-0.2.1.tar", last modified: Sun Aug 18 01:14:32 2019, max compression
+gzip compressed data, was "backwork-backup-postgresql-0.2.2.tar", last modified: Thu Jun 29 17:26:04 2023, max compression
```

## Comparing `backwork-backup-postgresql-0.2.1.tar` & `backwork-backup-postgresql-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/postgresql/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/postgresql/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/postgresql/postgresql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3345 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/CONTRIBUTING.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3345 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-18 01:14:32.000000 backwork-backup-postgresql-0.2.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2019-08-18 01:14:07.000000 backwork-backup-postgresql-0.2.1/setup.py
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:26:04.710675 backwork-backup-postgresql-0.2.2/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1111 2023-06-29 17:25:21.000000 backwork-backup-postgresql-0.2.2/CHANGELOG.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      477 2023-06-29 17:25:21.000000 backwork-backup-postgresql-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)    11357 2023-06-29 17:25:21.000000 backwork-backup-postgresql-0.2.2/LICENSE
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       13 2023-06-29 17:25:21.000000 backwork-backup-postgresql-0.2.2/MANIFEST.in
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2912 2023-06-29 17:26:04.710481 backwork-backup-postgresql-0.2.2/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2093 2023-06-29 17:25:21.000000 backwork-backup-postgresql-0.2.2/README.md
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:26:04.709567 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2912 2023-06-29 17:26:04.000000 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      417 2023-06-29 17:26:04.000000 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        1 2023-06-29 17:26:04.000000 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       60 2023-06-29 17:26:04.000000 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/entry_points.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        9 2023-06-29 17:26:04.000000 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/requires.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       11 2023-06-29 17:26:04.000000 backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/top_level.txt
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:26:04.710223 backwork-backup-postgresql-0.2.2/postgresql/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       84 2023-06-29 17:25:46.000000 backwork-backup-postgresql-0.2.2/postgresql/__init__.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2737 2023-06-29 17:25:41.000000 backwork-backup-postgresql-0.2.2/postgresql/postgresql.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       38 2023-06-29 17:26:04.710750 backwork-backup-postgresql-0.2.2/setup.cfg
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1316 2023-06-29 17:25:38.000000 backwork-backup-postgresql-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backwork-backup-postgresql-0.2.1/postgresql/postgresql.py` & `backwork-backup-postgresql-0.2.2/postgresql/postgresql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,74 +1,83 @@
 """Add support for PostgreSQL backups
 """
 
 import logging
+import os
 import subprocess
 import sys
-import os
 
 LOG = logging.getLogger(__name__)
 
 
 class PostgreSQLBackupException(Exception):  # pylint: disable=unused-variable
     """Raise for errors"""
+
     pass
 
 
 class PostgreSQLBackup(object):
     """Backup a PostgreSQL database.
 
     It uses `pg_dump` so it's required to have it installed and added to the
     system's PATH. You can use any of the arguments supported by `pg_dump`.
     Use `pg_dump --help` for more information.
     """
+
     command = "postgresql"
 
     def __init__(self, args, extra):
         self.args = args
         self.extra = extra
 
     @classmethod
     def parse_args(cls, subparsers):
         """Create the `postgresql` subparser for the `backup` command."""
         pg_parser = subparsers.add_parser(cls.command, description=cls.__doc__)
 
-        pg_parser.add_argument("--gzip", action="store_true", required=False,
-                               help="compress output file (requires gzip to be installed)")
-
-        pg_parser.add_argument("-o", "--output", required=False,
-                               help="output file path")
-
-        pg_parser.add_argument("-P", "--password", required=True,
-                               help="PostgreSQL connection password")
+        pg_parser.add_argument(
+            "--gzip",
+            action="store_true",
+            required=False,
+            help="compress output file (requires gzip to be installed)",
+        )
+
+        pg_parser.add_argument(
+            "-o", "--output", required=False, help="output file path"
+        )
+
+        pg_parser.add_argument(
+            "-P", "--password", required=True, help="PostgreSQL connection password"
+        )
 
     def backup(self):
         """Backup a PostgreSQL database."""
         output_file = sys.stdout
         gzip_out = None
         pg_dump_out = None
 
         if self.args.output:
             LOG.info("starting postgresql backup...")
-            output_file = open(self.args.output, 'w')
+            output_file = open(self.args.output, "w")
 
         if self.args.gzip:
             pg_dump_out = subprocess.PIPE
             gzip_out = output_file
         else:
             pg_dump_out = output_file
 
         try:
-            os.environ['PGPASSWORD'] = self.args.password
+            os.environ["PGPASSWORD"] = self.args.password
             pg_dump_cmd = ["pg_dump"] + self.extra
             pg_dump_process = subprocess.Popen(pg_dump_cmd, stdout=pg_dump_out)
 
             if self.args.gzip:
-                gzip_process = subprocess.Popen(["gzip"], stdin=pg_dump_process.stdout,
-                                                stdout=gzip_out)
+                gzip_process = subprocess.Popen(
+                    ["gzip"], stdin=pg_dump_process.stdout, stdout=gzip_out
+                )
                 pg_dump_process.stdout.close()
                 if gzip_process.wait() != 0:
                     raise PostgreSQLBackupException("gzip failed for Postgres")
 
             if pg_dump_process.wait() != 0:
                 raise PostgreSQLBackupException("pg_dump failed for Postgres")
```

### Comparing `backwork-backup-postgresql-0.2.1/PKG-INFO` & `backwork-backup-postgresql-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: backwork-backup-postgresql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Backwork plug-in for PostgreSQL backups.
 Home-page: https://github.com/ibm/backwork-backup-postgresql
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-postgresql [![Build Status](https://travis-ci.org/IBM/backwork-backup-postgresql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-postgresql) [![PyPI version](https://badge.fury.io/py/backwork-backup-postgresql.svg)](https://badge.fury.io/py/backwork-backup-postgresql)
-        Add support for PostgreSQL backups on [`backwork`](https://github.ibm.com/apset/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`pg_dump`](https://www.postgresql.org/docs/current/static/app-pgdump.html),
-        so you will need to it installed.
-        
-        `pg_dump` is part of the `postgresql` client.
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-postgresql
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup mysql` command
-        on `backwork`.
-        
-        ```sh
-        backwork backup postgresql -h
-        usage: backwork backup postgresql [-h] [--gzip] [-o OUTPUT] -P PASSWORD
-        
-        Backup a PostgreSQL database. It uses `pg_dump` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `pg_dump`. Use `pg_dump --help` for more information.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --gzip                compress output file (requires gzip to be installed)
-          -o OUTPUT, --output OUTPUT
-                                output file path
-          -P PASSWORD, --password PASSWORD
-                                PostgreSQL connection password
-        ```
-        
-        You can pass any option that you would normally use on `mysqldump`:
-        
-        ```sh
-        $ backwork backup postgresql -P password --host=192.168.99.1 --username=root --port=32769 --dbname=MY_DATABASE
-        ```
-        
-        As shown in the `--help` message, there are two extra arguments you can use in
-        your backup process `--gzip` and `-o`.
-        
-        `--gzip` will compress the output and requires the `gzip` command to be
-        available in your system.
-        
-        `-o OUTPUT` or `--output OUTPUT` will save the output of `pg_dump` into a
-        file.
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
+# backwork-backup-postgresql [![Build Status](https://travis-ci.org/IBM/backwork-backup-postgresql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-postgresql) [![PyPI version](https://badge.fury.io/py/backwork-backup-postgresql.svg)](https://badge.fury.io/py/backwork-backup-postgresql)
+Add support for PostgreSQL backups on [`backwork`](https://github.ibm.com/apset/backwork).
+
+## Requirements
+This plug-in is build on top of [`pg_dump`](https://www.postgresql.org/docs/current/static/app-pgdump.html),
+so you will need to it installed.
+
+`pg_dump` is part of the `postgresql` client.
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-postgresql
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup mysql` command
+on `backwork`.
+
+```sh
+backwork backup postgresql -h
+usage: backwork backup postgresql [-h] [--gzip] [-o OUTPUT] -P PASSWORD
+
+Backup a PostgreSQL database. It uses `pg_dump` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `pg_dump`. Use `pg_dump --help` for more information.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --gzip                compress output file (requires gzip to be installed)
+  -o OUTPUT, --output OUTPUT
+                        output file path
+  -P PASSWORD, --password PASSWORD
+                        PostgreSQL connection password
+```
+
+You can pass any option that you would normally use on `mysqldump`:
+
+```sh
+$ backwork backup postgresql -P password --host=192.168.99.1 --username=root --port=32769 --dbname=MY_DATABASE
+```
+
+As shown in the `--help` message, there are two extra arguments you can use in
+your backup process `--gzip` and `-o`.
+
+`--gzip` will compress the output and requires the `gzip` command to be
+available in your system.
+
+`-o OUTPUT` or `--output OUTPUT` will save the output of `pg_dump` into a
+file.
+
+**Important:** There is a conflict with the `-h` argument since it is reserved
+for the help/usage message. User `--host` to pass the hostname.
```

### Comparing `backwork-backup-postgresql-0.2.1/README.md` & `backwork-backup-postgresql-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-postgresql-0.2.1/backwork_backup_postgresql.egg-info/PKG-INFO` & `backwork-backup-postgresql-0.2.2/backwork_backup_postgresql.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: backwork-backup-postgresql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Backwork plug-in for PostgreSQL backups.
 Home-page: https://github.com/ibm/backwork-backup-postgresql
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-postgresql [![Build Status](https://travis-ci.org/IBM/backwork-backup-postgresql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-postgresql) [![PyPI version](https://badge.fury.io/py/backwork-backup-postgresql.svg)](https://badge.fury.io/py/backwork-backup-postgresql)
-        Add support for PostgreSQL backups on [`backwork`](https://github.ibm.com/apset/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`pg_dump`](https://www.postgresql.org/docs/current/static/app-pgdump.html),
-        so you will need to it installed.
-        
-        `pg_dump` is part of the `postgresql` client.
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-postgresql
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup mysql` command
-        on `backwork`.
-        
-        ```sh
-        backwork backup postgresql -h
-        usage: backwork backup postgresql [-h] [--gzip] [-o OUTPUT] -P PASSWORD
-        
-        Backup a PostgreSQL database. It uses `pg_dump` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `pg_dump`. Use `pg_dump --help` for more information.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --gzip                compress output file (requires gzip to be installed)
-          -o OUTPUT, --output OUTPUT
-                                output file path
-          -P PASSWORD, --password PASSWORD
-                                PostgreSQL connection password
-        ```
-        
-        You can pass any option that you would normally use on `mysqldump`:
-        
-        ```sh
-        $ backwork backup postgresql -P password --host=192.168.99.1 --username=root --port=32769 --dbname=MY_DATABASE
-        ```
-        
-        As shown in the `--help` message, there are two extra arguments you can use in
-        your backup process `--gzip` and `-o`.
-        
-        `--gzip` will compress the output and requires the `gzip` command to be
-        available in your system.
-        
-        `-o OUTPUT` or `--output OUTPUT` will save the output of `pg_dump` into a
-        file.
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
+# backwork-backup-postgresql [![Build Status](https://travis-ci.org/IBM/backwork-backup-postgresql.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-postgresql) [![PyPI version](https://badge.fury.io/py/backwork-backup-postgresql.svg)](https://badge.fury.io/py/backwork-backup-postgresql)
+Add support for PostgreSQL backups on [`backwork`](https://github.ibm.com/apset/backwork).
+
+## Requirements
+This plug-in is build on top of [`pg_dump`](https://www.postgresql.org/docs/current/static/app-pgdump.html),
+so you will need to it installed.
+
+`pg_dump` is part of the `postgresql` client.
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-postgresql
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup mysql` command
+on `backwork`.
+
+```sh
+backwork backup postgresql -h
+usage: backwork backup postgresql [-h] [--gzip] [-o OUTPUT] -P PASSWORD
+
+Backup a PostgreSQL database. It uses `pg_dump` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `pg_dump`. Use `pg_dump --help` for more information.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --gzip                compress output file (requires gzip to be installed)
+  -o OUTPUT, --output OUTPUT
+                        output file path
+  -P PASSWORD, --password PASSWORD
+                        PostgreSQL connection password
+```
+
+You can pass any option that you would normally use on `mysqldump`:
+
+```sh
+$ backwork backup postgresql -P password --host=192.168.99.1 --username=root --port=32769 --dbname=MY_DATABASE
+```
+
+As shown in the `--help` message, there are two extra arguments you can use in
+your backup process `--gzip` and `-o`.
+
+`--gzip` will compress the output and requires the `gzip` command to be
+available in your system.
+
+`-o OUTPUT` or `--output OUTPUT` will save the output of `pg_dump` into a
+file.
+
+**Important:** There is a conflict with the `-h` argument since it is reserved
+for the help/usage message. User `--host` to pass the hostname.
```

### Comparing `backwork-backup-postgresql-0.2.1/CHANGELOG.md` & `backwork-backup-postgresql-0.2.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-postgresql-0.2.1/setup.py` & `backwork-backup-postgresql-0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Add support for PostgreSQL backups
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
     name="backwork-backup-postgresql",
-    version="0.2.1",
+    version="0.2.2",
     description="Backwork plug-in for PostgreSQL backups.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/ibm/backwork-backup-postgresql",
     author="Luiz Aoqui",
     author_email="laoqui@ca.ibm.com",
     license="Apache 2",
@@ -24,22 +25,16 @@
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
-    entry_points={
-        "backwork.backups": [
-            "postgresql=postgresql:PostgreSQLBackup"
-        ]
-    }
+    install_requires=["backwork"],
+    entry_points={"backwork.backups": ["postgresql=postgresql:PostgreSQLBackup"]},
 )
```

