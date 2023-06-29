# Comparing `tmp/backwork-backup-mongo-0.3.1.tar.gz` & `tmp/backwork-backup-mongo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backwork-backup-mongo-0.3.1.tar", last modified: Thu Mar 25 20:14:19 2021, max compression
+gzip compressed data, was "backwork-backup-mongo-0.3.2.tar", last modified: Thu Jun 29 17:24:24 2023, max compression
```

## Comparing `backwork-backup-mongo-0.3.1.tar` & `backwork-backup-mongo-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3853 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2478 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/mongo/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5293 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/mongo/mongo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/mongo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      477 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/CONTRIBUTING.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3853 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-25 20:14:19.000000 backwork-backup-mongo-0.3.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1426 2021-03-25 20:13:54.000000 backwork-backup-mongo-0.3.1/setup.py
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:24:24.599683 backwork-backup-mongo-0.3.2/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      579 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/CHANGELOG.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      477 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 liyang.wang   (501) staff       (20)    11357 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/LICENSE
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       13 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/MANIFEST.in
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     3284 2023-06-29 17:24:24.599537 backwork-backup-mongo-0.3.2/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     2478 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/README.md
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:24:24.599038 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     3284 2023-06-29 17:24:24.000000 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 liyang.wang   (501) staff       (20)      372 2023-06-29 17:24:24.000000 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        1 2023-06-29 17:24:24.000000 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       93 2023-06-29 17:24:24.000000 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/entry_points.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        9 2023-06-29 17:24:24.000000 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/requires.txt
+-rw-r--r--   0 liyang.wang   (501) staff       (20)        6 2023-06-29 17:24:24.000000 backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/top_level.txt
+drwxr-xr-x   0 liyang.wang   (501) staff       (20)        0 2023-06-29 17:24:24.599336 backwork-backup-mongo-0.3.2/mongo/
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       98 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/mongo/__init__.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     5293 2023-06-29 17:22:51.000000 backwork-backup-mongo-0.3.2/mongo/mongo.py
+-rw-r--r--   0 liyang.wang   (501) staff       (20)       38 2023-06-29 17:24:24.599719 backwork-backup-mongo-0.3.2/setup.cfg
+-rw-r--r--   0 liyang.wang   (501) staff       (20)     1372 2023-06-29 17:23:15.000000 backwork-backup-mongo-0.3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backwork-backup-mongo-0.3.1/PKG-INFO` & `backwork-backup-mongo-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 Metadata-Version: 2.1
 Name: backwork-backup-mongo
-Version: 0.3.1
+Version: 0.3.2
 Summary: Backwork plug-in for MongoDB backups.
 Home-page: https://github.com/IBM/backwork-backup-mongo
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-mongo [![Build Status](https://travis-ci.org/IBM/backwork-backup-mongo.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mongo) [![PyPI version](https://badge.fury.io/py/backwork-backup-mongo.svg)](https://badge.fury.io/py/backwork-backup-mongo)
-        Adds support for MongoDB backups to [`backwork`](https://github.com/IBM/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`mongodump`](https://docs.mongodb.com/manual/reference/program/mongodump/#bin.mongodump),
-        so you will need to have [`mongo-tools`](https://github.com/mongodb/mongo-tools)
-        installed.
-        
-        If you already have the `mongod` server or `mongo` client installed then you
-        should have `mongodump`. If not, you can install them using the
-        [official packages](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/#packages)
-        or build from [source](https://github.com/mongodb/mongo-tools).
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-mongo
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup mongo` and `restore mongo` commands
-        on `backwork`.
-        
-        
-        #### `backwork backup mongo`
-        ```sh
-        $ backwork backup mongo --help
-        usage: backwork backup mongo [-h]
-        
-        Backup a MongoDB database. It uses `mongodump` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `mongodump`. Use `mongodump --help` for more information.
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        You can pass any option that you would normally use on `mongodump`, e.g.:
-        
-        ```sh
-        $ backwork backup mongo --user=user --password=pass --host=mongo
-        ```
-        
-        The only exception is `-h` which is reserved for the help/usage message, so the
-        host needs to be passed as `--host`.
-        
-        
-        
-        #### `backwork restore mongo`
-        
-        ```sh
-        $ backwork restore mongo --help
-        usage: backwork restore mongo [-h]
-        
-        Restore a MongoDB database. It uses `mongorestore` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `mongorestore`. Use `mongorestore --help` for more information.
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        You can pass any option that you would normally use on `mongorestore`, e.g.:
-        
-        ```sh
-        $ backwork restore mongo --user=user --password=pass --host=mongo dumps
-        ```
-        
-        The only exception is `-h` which is reserved for the help/usage message, so the
-        host needs to be passed as `--host`.
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
+# backwork-backup-mongo [![Build Status](https://travis-ci.org/IBM/backwork-backup-mongo.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mongo) [![PyPI version](https://badge.fury.io/py/backwork-backup-mongo.svg)](https://badge.fury.io/py/backwork-backup-mongo)
+Adds support for MongoDB backups to [`backwork`](https://github.com/IBM/backwork).
+
+## Requirements
+This plug-in is build on top of [`mongodump`](https://docs.mongodb.com/manual/reference/program/mongodump/#bin.mongodump),
+so you will need to have [`mongo-tools`](https://github.com/mongodb/mongo-tools)
+installed.
+
+If you already have the `mongod` server or `mongo` client installed then you
+should have `mongodump`. If not, you can install them using the
+[official packages](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/#packages)
+or build from [source](https://github.com/mongodb/mongo-tools).
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-mongo
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup mongo` and `restore mongo` commands
+on `backwork`.
+
+
+#### `backwork backup mongo`
+```sh
+$ backwork backup mongo --help
+usage: backwork backup mongo [-h]
+
+Backup a MongoDB database. It uses `mongodump` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `mongodump`. Use `mongodump --help` for more information.
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+You can pass any option that you would normally use on `mongodump`, e.g.:
+
+```sh
+$ backwork backup mongo --user=user --password=pass --host=mongo
+```
+
+The only exception is `-h` which is reserved for the help/usage message, so the
+host needs to be passed as `--host`.
+
+
+
+#### `backwork restore mongo`
+
+```sh
+$ backwork restore mongo --help
+usage: backwork restore mongo [-h]
+
+Restore a MongoDB database. It uses `mongorestore` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `mongorestore`. Use `mongorestore --help` for more information.
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+You can pass any option that you would normally use on `mongorestore`, e.g.:
+
+```sh
+$ backwork restore mongo --user=user --password=pass --host=mongo dumps
+```
+
+The only exception is `-h` which is reserved for the help/usage message, so the
+host needs to be passed as `--host`.
```

### Comparing `backwork-backup-mongo-0.3.1/README.md` & `backwork-backup-mongo-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-mongo-0.3.1/mongo/mongo.py` & `backwork-backup-mongo-0.3.2/mongo/mongo.py`

 * *Files identical despite different names*

### Comparing `backwork-backup-mongo-0.3.1/backwork_backup_mongo.egg-info/PKG-INFO` & `backwork-backup-mongo-0.3.2/backwork_backup_mongo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 Metadata-Version: 2.1
 Name: backwork-backup-mongo
-Version: 0.3.1
+Version: 0.3.2
 Summary: Backwork plug-in for MongoDB backups.
 Home-page: https://github.com/IBM/backwork-backup-mongo
 Author: Luiz Aoqui
 Author-email: laoqui@ca.ibm.com
 License: Apache 2
-Description: # backwork-backup-mongo [![Build Status](https://travis-ci.org/IBM/backwork-backup-mongo.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mongo) [![PyPI version](https://badge.fury.io/py/backwork-backup-mongo.svg)](https://badge.fury.io/py/backwork-backup-mongo)
-        Adds support for MongoDB backups to [`backwork`](https://github.com/IBM/backwork).
-        
-        ## Requirements
-        This plug-in is build on top of [`mongodump`](https://docs.mongodb.com/manual/reference/program/mongodump/#bin.mongodump),
-        so you will need to have [`mongo-tools`](https://github.com/mongodb/mongo-tools)
-        installed.
-        
-        If you already have the `mongod` server or `mongo` client installed then you
-        should have `mongodump`. If not, you can install them using the
-        [official packages](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/#packages)
-        or build from [source](https://github.com/mongodb/mongo-tools).
-        
-        ## Installing
-        You can use `pip` to install this plug-in:
-        ```sh
-        $ pip install backwork-backup-mongo
-        ```
-        
-        ## Using
-        After installing the plug-in you will be able to use the `backup mongo` and `restore mongo` commands
-        on `backwork`.
-        
-        
-        #### `backwork backup mongo`
-        ```sh
-        $ backwork backup mongo --help
-        usage: backwork backup mongo [-h]
-        
-        Backup a MongoDB database. It uses `mongodump` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `mongodump`. Use `mongodump --help` for more information.
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        You can pass any option that you would normally use on `mongodump`, e.g.:
-        
-        ```sh
-        $ backwork backup mongo --user=user --password=pass --host=mongo
-        ```
-        
-        The only exception is `-h` which is reserved for the help/usage message, so the
-        host needs to be passed as `--host`.
-        
-        
-        
-        #### `backwork restore mongo`
-        
-        ```sh
-        $ backwork restore mongo --help
-        usage: backwork restore mongo [-h]
-        
-        Restore a MongoDB database. It uses `mongorestore` so it's required to have it
-        installed and added to the system's PATH. You can use any of the arguments
-        supported by `mongorestore`. Use `mongorestore --help` for more information.
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        You can pass any option that you would normally use on `mongorestore`, e.g.:
-        
-        ```sh
-        $ backwork restore mongo --user=user --password=pass --host=mongo dumps
-        ```
-        
-        The only exception is `-h` which is reserved for the help/usage message, so the
-        host needs to be passed as `--host`.
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
+# backwork-backup-mongo [![Build Status](https://travis-ci.org/IBM/backwork-backup-mongo.svg?branch=master)](https://travis-ci.org/IBM/backwork-backup-mongo) [![PyPI version](https://badge.fury.io/py/backwork-backup-mongo.svg)](https://badge.fury.io/py/backwork-backup-mongo)
+Adds support for MongoDB backups to [`backwork`](https://github.com/IBM/backwork).
+
+## Requirements
+This plug-in is build on top of [`mongodump`](https://docs.mongodb.com/manual/reference/program/mongodump/#bin.mongodump),
+so you will need to have [`mongo-tools`](https://github.com/mongodb/mongo-tools)
+installed.
+
+If you already have the `mongod` server or `mongo` client installed then you
+should have `mongodump`. If not, you can install them using the
+[official packages](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/#packages)
+or build from [source](https://github.com/mongodb/mongo-tools).
+
+## Installing
+You can use `pip` to install this plug-in:
+```sh
+$ pip install backwork-backup-mongo
+```
+
+## Using
+After installing the plug-in you will be able to use the `backup mongo` and `restore mongo` commands
+on `backwork`.
+
+
+#### `backwork backup mongo`
+```sh
+$ backwork backup mongo --help
+usage: backwork backup mongo [-h]
+
+Backup a MongoDB database. It uses `mongodump` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `mongodump`. Use `mongodump --help` for more information.
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+You can pass any option that you would normally use on `mongodump`, e.g.:
+
+```sh
+$ backwork backup mongo --user=user --password=pass --host=mongo
+```
+
+The only exception is `-h` which is reserved for the help/usage message, so the
+host needs to be passed as `--host`.
+
+
+
+#### `backwork restore mongo`
+
+```sh
+$ backwork restore mongo --help
+usage: backwork restore mongo [-h]
+
+Restore a MongoDB database. It uses `mongorestore` so it's required to have it
+installed and added to the system's PATH. You can use any of the arguments
+supported by `mongorestore`. Use `mongorestore --help` for more information.
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+You can pass any option that you would normally use on `mongorestore`, e.g.:
+
+```sh
+$ backwork restore mongo --user=user --password=pass --host=mongo dumps
+```
+
+The only exception is `-h` which is reserved for the help/usage message, so the
+host needs to be passed as `--host`.
```

### Comparing `backwork-backup-mongo-0.3.1/CHANGELOG.md` & `backwork-backup-mongo-0.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `backwork-backup-mongo-0.3.1/setup.py` & `backwork-backup-mongo-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Add support for MongoDB backups on backwork.
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
     name="backwork-backup-mongo",
-    version="0.3.1",
+    version="0.3.2",
     description="Backwork plug-in for MongoDB backups.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/backwork-backup-mongo",
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
-            "mongo=mongo:MongoBackup"
-        ],
-        "backwork.restores": [
-            "mongo=mongo:MongoRestore"
-        ]
-    }
+        "backwork.backups": ["mongo=mongo:MongoBackup"],
+        "backwork.restores": ["mongo=mongo:MongoRestore"],
+    },
 )
```

