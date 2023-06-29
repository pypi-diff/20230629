# Comparing `tmp/imessage_reader-0.5.0.tar.gz` & `tmp/imessage_reader-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessage_reader-0.5.0.tar", last modified: Tue Mar  7 15:18:43 2023, max compression
+gzip compressed data, was "imessage_reader-0.6.0.tar", last modified: Thu Jun 29 11:39:07 2023, max compression
```

## Comparing `imessage_reader-0.5.0.tar` & `imessage_reader-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-03-07 15:18:43.280355 imessage_reader-0.5.0/
--rw-r--r--   0 bodo       (501) staff       (20)     1077 2022-07-13 15:56:51.000000 imessage_reader-0.5.0/LICENSE
--rw-r--r--   0 bodo       (501) staff       (20)     3605 2023-03-07 15:18:43.280230 imessage_reader-0.5.0/PKG-INFO
--rw-r--r--   0 bodo       (501) staff       (20)     2914 2022-07-13 15:56:51.000000 imessage_reader-0.5.0/README.md
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-03-07 15:18:43.279210 imessage_reader-0.5.0/imessage_reader/
--rw-r--r--   0 bodo       (501) staff       (20)       88 2022-07-13 15:56:51.000000 imessage_reader-0.5.0/imessage_reader/__init__.py
--rw-r--r--   0 bodo       (501) staff       (20)     1741 2023-03-07 12:18:10.000000 imessage_reader-0.5.0/imessage_reader/cli.py
--rw-r--r--   0 bodo       (501) staff       (20)     1285 2023-03-07 15:06:46.000000 imessage_reader-0.5.0/imessage_reader/common.py
--rw-r--r--   0 bodo       (501) staff       (20)     1965 2022-07-13 15:56:51.000000 imessage_reader-0.5.0/imessage_reader/create_sqlite.py
--rw-r--r--   0 bodo       (501) staff       (20)     1040 2023-03-07 15:06:46.000000 imessage_reader-0.5.0/imessage_reader/data_container.py
--rw-r--r--   0 bodo       (501) staff       (20)     5668 2023-03-07 15:06:46.000000 imessage_reader-0.5.0/imessage_reader/fetch_data.py
--rw-r--r--   0 bodo       (501) staff       (20)      657 2022-07-13 15:56:51.000000 imessage_reader-0.5.0/imessage_reader/info.py
--rw-r--r--   0 bodo       (501) staff       (20)     3680 2022-07-13 15:56:51.000000 imessage_reader-0.5.0/imessage_reader/write_excel.py
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-03-07 15:18:43.280011 imessage_reader-0.5.0/imessage_reader.egg-info/
--rw-r--r--   0 bodo       (501) staff       (20)     3605 2023-03-07 15:18:43.000000 imessage_reader-0.5.0/imessage_reader.egg-info/PKG-INFO
--rw-r--r--   0 bodo       (501) staff       (20)      491 2023-03-07 15:18:43.000000 imessage_reader-0.5.0/imessage_reader.egg-info/SOURCES.txt
--rw-r--r--   0 bodo       (501) staff       (20)        1 2023-03-07 15:18:43.000000 imessage_reader-0.5.0/imessage_reader.egg-info/dependency_links.txt
--rw-r--r--   0 bodo       (501) staff       (20)       61 2023-03-07 15:18:43.000000 imessage_reader-0.5.0/imessage_reader.egg-info/entry_points.txt
--rw-r--r--   0 bodo       (501) staff       (20)        9 2023-03-07 15:18:43.000000 imessage_reader-0.5.0/imessage_reader.egg-info/requires.txt
--rw-r--r--   0 bodo       (501) staff       (20)       16 2023-03-07 15:18:43.000000 imessage_reader-0.5.0/imessage_reader.egg-info/top_level.txt
--rw-r--r--   0 bodo       (501) staff       (20)       38 2023-03-07 15:18:43.280397 imessage_reader-0.5.0/setup.cfg
--rw-r--r--   0 bodo       (501) staff       (20)     1163 2023-03-07 15:18:06.000000 imessage_reader-0.5.0/setup.py
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.535405 imessage_reader-0.6.0/
+-rw-r--r--   0 bodo       (501) staff       (20)     1077 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/LICENSE
+-rw-r--r--   0 bodo       (501) staff       (20)     4507 2023-06-29 11:39:07.535273 imessage_reader-0.6.0/PKG-INFO
+-rw-r--r--   0 bodo       (501) staff       (20)     3866 2023-06-29 11:35:11.000000 imessage_reader-0.6.0/README.md
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.533387 imessage_reader-0.6.0/imessage_reader/
+-rw-r--r--   0 bodo       (501) staff       (20)       88 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/imessage_reader/__init__.py
+-rw-r--r--   0 bodo       (501) staff       (20)     2823 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/cli.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1294 2023-06-29 11:35:11.000000 imessage_reader-0.6.0/imessage_reader/common.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1947 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/create_sqlite.py
+-rw-r--r--   0 bodo       (501) staff       (20)      997 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/data_container.py
+-rw-r--r--   0 bodo       (501) staff       (20)     6071 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/fetch_data.py
+-rw-r--r--   0 bodo       (501) staff       (20)      627 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/info.py
+-rw-r--r--   0 bodo       (501) staff       (20)     3610 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/write_excel.py
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.534005 imessage_reader-0.6.0/imessage_reader.egg-info/
+-rw-r--r--   0 bodo       (501) staff       (20)     4507 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/PKG-INFO
+-rw-r--r--   0 bodo       (501) staff       (20)      659 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 bodo       (501) staff       (20)        1 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 bodo       (501) staff       (20)       61 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/entry_points.txt
+-rw-r--r--   0 bodo       (501) staff       (20)        9 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/requires.txt
+-rw-r--r--   0 bodo       (501) staff       (20)       16 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/top_level.txt
+-rw-r--r--   0 bodo       (501) staff       (20)       38 2023-06-29 11:39:07.535437 imessage_reader-0.6.0/setup.cfg
+-rw-r--r--   0 bodo       (501) staff       (20)     1114 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/setup.py
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.535059 imessage_reader-0.6.0/tests/
+-rw-r--r--   0 bodo       (501) staff       (20)      669 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/tests/test_cli.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1146 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_create_sqlite.py
+-rw-r--r--   0 bodo       (501) staff       (20)      882 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_fetch_db.py
+-rw-r--r--   0 bodo       (501) staff       (20)      515 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_get_platform.py
+-rw-r--r--   0 bodo       (501) staff       (20)      269 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_info.py
+-rw-r--r--   0 bodo       (501) staff       (20)     2440 2023-04-11 15:45:17.000000 imessage_reader-0.6.0/tests/test_message_data.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1187 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_write_excel.py
```

### Comparing `imessage_reader-0.5.0/LICENSE` & `imessage_reader-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.5.0/PKG-INFO` & `imessage_reader-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,123 @@
-Metadata-Version: 2.1
-Name: imessage_reader
-Version: 0.5.0
-Summary: Fetch recipients and chat messages from the chat.db database.
-Home-page: https://github.com/niftycode/imessage_reader
-Author: Bodo Schönfeld
-Author-email: bodo.schoenfeld@niftycode.de
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # imessage_reader
 
-![](img/license-MIT-green.svg) ![](img/python-3.8-blue.svg) ![](https://img.shields.io/github/last-commit/niftycode/imessage_reader.svg?style=flat) ![](https://img.shields.io/github/issues/niftycode/imessage_reader.svg?style=flat) ![](https://img.shields.io/travis/niftycode/imessage_reader/master) ![](https://img.shields.io/pypi/v/imessage_reader)
+![](img/license-MIT-green.svg) ![](img/python-3.9-blue.svg) ![](https://img.shields.io/github/last-commit/niftycode/imessage_reader.svg?style=flat) ![](https://img.shields.io/github/issues/niftycode/imessage_reader.svg?style=flat)  ![](https://img.shields.io/pypi/v/imessage_reader)
 
-This is a forensic tool written in Python 3. Use this tool to fetch the content (phone numbers, email addresses,
-messages and the account) from the *chat.db* database file on **macOS** (version 10.14 or above).
+This is a forensic tool written in Python 3. Use this tool to fetch the content (phone numbers, email addresses, messages and the account) from the *chat.db* database file on **macOS** (version 10.14 or above).
 
 The following information is currently being read from the database:
 
 * user id (sender's or recipient's phone number or email address)
 * message
 * date and time
 * service (iMessage or SMS)
 * account (destination caller id)
 * is the message from me
 
 ## Background
 
-Received messages (iMessage or SMS) and attachments will be saved in "~/Library/Messages". This directory contains a "
-chat.db" file (SQLite3) with two tables of interest: *handle* and *message*. The *handle* table contains the
-recipients (email address or phone number). The received messages are in the *message* table.
+Received messages (iMessage or SMS) and attachments will be saved in "~/Library/Messages". This directory contains a "chat.db" file (SQLite3) with two tables of interest: *handle* and *message*. The *handle* table contains the recipients (email address or phone number). The received messages are in the *message* table.
 
 ## Note
 
-Since the iMessage database is only available under macOS, it makes no sense to use this tool under Windows or Linux.
+Of course, the chat.db file is only created under macOS. Nevertheless, this program can also be used under Linux. In contrast to use under macOS, the path to the chat.db file must then be specified (see below).
 
 ## Requirements
 
-* **Python 3.8+**
+* Python 3.9+
 * openpyxl
 
 To run tests install **pytest**:
 
     pip3 install pytest
 
 ## Install
 
-    pip3 install imessage_reader
+    pip3 install imessage-reader
 
 ## Usage (CLI)
 
+## Specify no options
+
 Start the program with:
 
     imessage_reader
 
-This will show you all users and messages.
+This will show you all users and messages in the Terminal. If no option (`-p <PATH>`) is specified, the default directory (under macOS) is searched for the chat.db file.
+
+## Specify a PATH as argument
+
+A different path to chat.db file can be specified with the `-p` option:
+
+    imessage_reader -p <PATH>
+
+Unless the `-o` option is also used, the data is displayed in the Terminal.
+
+## Specify an output argument
+
+You can create an Excel file containing users, messages, date and service (SMS or iMessage). The file will be stored in the
+Documents folder:
 
-Use
+    imessage_reader -o e
 
-    imessage_reader -e
+or
 
-to create an Excel file containing users, messages, date and service (SMS or iMessage). The file will be stored in the
-Desktop folder.
+    imessage_reader -o excel
 
-Use
+You can create a SQLite3 database containing users, messages, date and service (SMS or iMessage). The file will be stored in the Documents folder:
 
-    imessage_reader -s
+    imessage_reader -o s
 
-to create a SQLite3 database containing users, messages, date and service (SMS or iMessage). The file will be stored in
-the Desktop folder.
+or
 
-Use
+    imessage_reader -o sqlite
+
+If you only want to see a list of recipients use:
 
     imessage_reader -r
 
-to show a list of recipients.
+or
+
+    imessage_reader --recipients
 
-**Note**: You need access to the *Library* folder in order to read the iMessage database file ("chat.db"). You can add
-access (for *Terminal* or *iTerm*) in
+**Note**: On **macOS** you need access to the *Library* folder in order to read the iMessage database file ("chat.db"). You can add access (for *Terminal* or *iTerm*) in
 
     > System Preferences > Security & Privacy > Privacy > Full Disk Access
 
+## Specify a PATH and an output argument
+
+You can combine the `-p` with the `-o` option:
+
+    imessage_reader -p /home/bodo/Downloads -o excel
+
+In this example the chat.db file is located in the Downloads folder (on a Linux machine). And the Excel file will be created in the Documents folder.
+
 ## Usage (import module)
 
 To get the messages use following code:
 
     from imessage_reader import fetch_data
-
+    
+    DB_PATH = /home/bodo/Downloads/chat.db
+    
     # Create a FetchData instance
-    fd = fetch_data.FetchData()
+    fd = fetch_data.FetchData(DB_PATH)
 
     # Store messages in my_data
-    # This is a list of tuples containing user id, message and service.
-    # service -> iMessage or SMS
+    # This is a list of tuples containing user id, message and service (iMessage or SMS).
     my_data = fd.get_messages()
     print(my_data)
 
 ## ToDo
 
 * ~~Get the date of messages~~
 * ~~Fetch the date of received messages.~~
-* Show a list of all known recipients.
+* ~~Show a list of all known recipients.~~
 * ~~Did the user receive the message via SMS or via iMessage?~~
 * ~~Create SQLite3 database.~~
+* ~~Specify a different path to the chat.db file.~~
 * Show attachments.
 * Add more tests.
 
 ## Changelog
 
 see [CHANGELOG.rst](https://github.com/niftycode/imessage_reader/blob/master/CHANGELOG.rst)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `imessage_reader-0.5.0/imessage_reader/common.py` & `imessage_reader-0.6.0/imessage_reader/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 common.py
-Python 3.8+
+Python 3.9+
 Date created: June 14th, 2020
-Date modified: February 26th, 2022
+Date modified: June 3rd, 2023
 """
 
 import platform
 import sqlite3
 import sys
 from enum import Enum
 
-VERSION = "0.5.0"
+VERSION = "0.6.0"
 
 
 class Platform(Enum):
-    """
-    An enum used to indicate the system's operating system
+    """An enum used to indicate the running operating system
     """
 
     OTHER = 0
     LINUX = 1
     MAC = 2
     WINDOWS = 3
 
 
 def get_platform() -> str:
-    """
-    Get the current operating system.
-    :return: The operating system this program is running on
+    """Get the current operating system.
+
+    :return: the operating system this program is running on
     """
     system = platform.system()
     if system == "Linux":
         return str(Platform.LINUX.name)
     if system == "Darwin":
         return str(Platform.MAC.name)
     if system == "Windows":
         return str(Platform.WINDOWS.name)
     raise NotImplementedError(f"Platform {system} is not supported yet!")
 
 
 def fetch_db_data(db, command) -> list:
-    """
-    Send queries to the sqlite database and return the results.
-    :param db: The path to the database.
-    :param command: The Sqlite command.
-    :return: Data from the database
+    """Send queries to the sqlite database and return the results.
+
+    :param db: the path to the database
+    :param command: the SQL command
+    :return: data from the database
     """
     try:
         conn = sqlite3.connect(db)
         cur = conn.cursor()
         cur.execute(command)
         return cur.fetchall()
     except Exception as e:
-        sys.exit("Error reading the database: %s" % e)
+        sys.exit(f"Error reading the database: {e}\nDid you specify the correct path?")
```

### Comparing `imessage_reader-0.5.0/imessage_reader/create_sqlite.py` & `imessage_reader-0.6.0/imessage_reader/create_sqlite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Create a SQLite3 database containing iMessage data (user id, text, date, service)
-Python 3.8+
+Python 3.9+
 Date created: April 30th, 2021
 Date modified: August 28th, 2021
 """
 
 import sqlite3
 
 
 class CreateDatabase:
-    """This class manages the export to SQLite"""
+    """This class manages the export to SQLite.
+    """
 
     def __init__(self, imessage_data: list, file_path: str):
-        """
-        init function of this class
-        :param imessage_data: List with MessageData objects
+        """Constructor method
+
+        :param imessage_data: list with MessageData objects
                 containing user id, text, date, service and account
-        :param file_path: The path to the loaction of the Excel file
+        :param file_path: the path to the location of the Excel file
         """
         self.imessage_data = imessage_data
         self.file_path = file_path
 
     def create_sqlite_db(self):
-        """
-        Create a SQLite3 database in the Desktop folder.
+        """Create a SQLite3 database in the Desktop folder.
         Add user, text, date and service to the database.
         """
         database = self.file_path + "iMessage-Data.sqlite"
 
         conn = sqlite3.connect(database)
         cur = conn.cursor()
 
@@ -61,9 +61,9 @@
             )
 
         conn.commit()
         cur.close()
 
         print()
         print(">>> SQLite database successfully created! <<<")
-        print("You find the Database in your Desktop folder.")
+        print("You find the Database in your Documents folder.")
         print()
```

### Comparing `imessage_reader-0.5.0/imessage_reader/data_container.py` & `imessage_reader-0.6.0/imessage_reader/data_container.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 
 """
 Data Container
-Python 3.8+
+Python 3.9+
 Author: niftycode
 Modified by: -
 Date created: February 19th, 2022
 Date modified: -
 """
 
 from dataclasses import dataclass
 
 
 @dataclass
 class MessageData:
-    """
-    This dataclass is the store for the data:
+    """This dataclass is the store for the data:
     user id, text, date, service and account (caller id).
     """
 
     user_id: str
     text: str
     date: str
     service: str
     account: str
     is_from_me: int
 
     def __str__(self):
-        """
-        String representation
-        :return: String representation of this object
+        """String representation
+
+        :return: the representation of this object
         """
         return (
             f"user id:\t\t{self.user_id}\n"
             f"date and time:\t\t{self.date}\n"
             f"service:\t\t{self.service}\n"
             f"caller id:\t\t{self.account}\n"
             f"is_from_me:\t\t{self.is_from_me}\n"
             f"\n"
             f"text:\n"
-            f"========\n"
+            f"=====\n"
             f"{self.text}\n"
             f"\n"
             f"----------------------------------------------------------------\n"
         )
```

### Comparing `imessage_reader-0.5.0/imessage_reader/fetch_data.py` & `imessage_reader-0.6.0/imessage_reader/fetch_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 
 """
-Fetch data, print data and export data to excel.
-Python 3.8+
+Fetch data, print data, show recipients or export data.
+Python 3.9+
 Author: niftycode
 Modified by: thecircleisround
 Date created: October 8th, 2020
-Date modified: February 19th, 2022
+Date modified: June 27th, 2023
 """
 
 import sys
+import logging
 
 from os.path import expanduser
 
 from imessage_reader import common, create_sqlite, write_excel, data_container
 
 
+# logging.basicConfig(level=logging.DEBUG)
+logging.basicConfig(level=logging.INFO)
+
+
 # noinspection PyMethodMayBeStatic
 class FetchData:
     """
-    This class contains the methods to fetch, print and export the messages.
+    This class contains the methods to fetch,
+    print and export the messages.
     """
 
-    # The path to the iMessage database
-    DB_PATH = expanduser("~") + "/Library/Messages/chat.db"
-
     # The SQL command
     SQL_CMD = (
         "SELECT "
         "text, "
         "datetime((date / 1000000000) + 978307200, 'unixepoch', 'localtime'),"
         "handle.id, "
         "handle.service, "
@@ -37,65 +39,77 @@
         "message.is_from_me, "
         "message.attributedBody, "
         "message.cache_has_attachments "
         "FROM message "
         "JOIN handle on message.handle_id=handle.ROWID"
     )
 
-    def __init__(self, system=None):
+    def __init__(self, db_path: str, system=None):
+        """Constructor method
+
+        :param db_path: Path to the chat.db file
+        :param system: Operating System
+        """
+        self.db_path = db_path
         if system is None:
             self.operating_system = common.get_platform()
 
     def _check_system(self):
-        if self.operating_system != "MAC":
+        # TODO: Change this later (So, it can be used on Windows too.)
+        if self.operating_system == "WINDOWS":
             sys.exit("Your operating system is not supported yet!")
 
     def _read_database(self) -> list:
-        """
-        Fetch data from the database and store the data in a list.
-        :return: List containing the user id, messages, the service and the account
+        """Fetch data from the database and store the data in a list.
+
+        :return: list containing the user id, messages, the service and the account
         """
 
-        rval = common.fetch_db_data(self.DB_PATH, self.SQL_CMD)
+        rval = common.fetch_db_data(self.db_path, self.SQL_CMD)
 
         data = []
         for row in rval:
             text = row[0]
             if row[7] == 1:
                 text = "<Message with no text, but an attachment.>"
-            # the chatdb has some weird behavior where sometimes the text value is None
-            # and the text string is buried in an binary blob under the attributedBody field.
+            # the chat.db has some weird behavior where sometimes the text value is None
+            # and the text string is buried in a binary blob under the attributedBody field.
             if text is None and row[6] is not None:
                 try:
-                    text = row[6].split(b'NSString')[1]
-                    text = text[5:]  # stripping some preamble which generally looks like this: b'\x01\x94\x84\x01+'
-
-                    if text[0] == 129:  # this 129 is b'\x81, python indexes byte strings as ints, this is equivalent to text[0:1] == b'\x81'
-                        length = int.from_bytes(text[1:3], 'little')
-                        text = text[3:length + 3]
+                    text = row[6].split(b"NSString")[1]
+                    text = text[
+                        5:
+                    ]  # stripping some preamble which generally looks like this: b'\x01\x94\x84\x01+'
+
+                    # this 129 is b'\x81, python indexes byte strings as ints,
+                    # this is equivalent to text[0:1] == b'\x81'
+                    if text[0] == 129:
+                        length = int.from_bytes(text[1:3], "little")
+                        text = text[3: length + 3]
                     else:
                         length = text[0]
-                        text = text[1:length + 1]
+                        text = text[1: length + 1]
                     text = text.decode()
+
+                    logging.debug(text)
+
                 except Exception as e:
-                    print("ERROR: Can't read a message.")
                     print(e)
+                    sys.exit("ERROR: Can't read a message.")
 
             data.append(
-                data_container.MessageData(
-                    row[2], text, row[1], row[3], row[4], row[5]
-                )
+                data_container.MessageData(row[2], text, row[1], row[3], row[4], row[5])
             )
 
         return data
 
     def show_user_txt(self, export: str):
-        """
-        Invoke _read_database(), print fetched data and export data.
-        This method is for CLI usage.
+        """Invoke _read_database(), print fetched data and export data.
+        (This method is for CLI usage.)
+
         :param export: Determine whether to export data
         """
 
         # Check the running operating system
         self._check_system()
 
         # Read chat.db
@@ -110,38 +124,40 @@
         if export == "excel":
             self._export_excel(fetched_data)
 
         # SQLite3 export
         if export == "sqlite":
             self._export_sqlite(fetched_data)
 
+        # Show all recipients
         if export == "recipients":
             self._get_recipients()
 
     def _export_excel(self, data: list):
-        """
-        Export data (write Excel file)
+        """Export data (write Excel file)
+
         :param data: message objects containing user id, message, date, service, account
         """
-        file_path = expanduser("~") + "/Desktop/"
+        file_path = expanduser("~") + "/Documents/"
+        # TODO: Exception handling
         ew = write_excel.ExelWriter(data, file_path)
         ew.write_data()
 
     def _export_sqlite(self, data: list):
+        """Export data (create SQLite3 database).
+
+        :param data: message objects containing user id, message, date, service, account
         """
-        Export data (create SQLite3 database)
-        :param data: message objects containig user id, message, date, service, account
-        """
-        file_path = expanduser("~") + "/Desktop/"
+        file_path = expanduser("~") + "/Documents/"
+        # TODO: Exception handling
         cd = create_sqlite.CreateDatabase(data, file_path)
         cd.create_sqlite_db()
 
     def _get_recipients(self):
-        """
-        Create a list containing all recipients and
+        """Create a list containing all recipients and
         show the recipients in the command line.
         """
         fetched_data = self._read_database()
 
         # Create a list with recipients
         recipients = [i.user_id for i in fetched_data if i.is_from_me == 0]
 
@@ -149,19 +165,20 @@
         print("List of Recipients")
         print("------------------------")
         print()
 
         for recipient in recipients:
             print(recipient)
 
+    '''
     def get_messages(self) -> list:
-        """
-        Create a list with tuples (user id, message, date, service, account, is_from_me)
-        This method is for module usage.
-        :return: List with tuples (user id, message, date, service, account, is_from_me)
+        """Create a list with tuples (user id, message, date, service, account, is_from_me)
+        (This method is for module usage.)
+
+        :return: list with tuples (user id, message, date, service, account, is_from_me)
         """
         fetched_data = self._read_database()
 
         users = []
         messages = []
         dates = []
         service = []
@@ -175,7 +192,8 @@
             service.append(data.service)
             account.append(data.account)
             is_from_me.append(data.is_from_me)
 
         data = list(zip(users, messages, dates, service, account, is_from_me))
 
         return data
+'''
```

### Comparing `imessage_reader-0.5.0/imessage_reader/info.py` & `imessage_reader-0.6.0/imessage_reader/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 
 """
 App info, license, version
-Python 3.8+
+Python 3.9+
 Date created: June 14th, 2020
 Date modified: February 22nd, 2022
 """
 
 
 from imessage_reader import common
 
 VERSION = common.VERSION
 
 
 def app_info():
-    """
-    Show app infos (Version & License)
+    """Show app infos (Version & License)
     """
     print("\n\n    ##### A Python script to read iMessage data #####")
     print("    #              Created by niftycode             #")
     print(f"    #                 Version {VERSION}                 #")
     print("    #                  MIT License                  #")
     print("    #################################################\n\n")
     print()
```

### Comparing `imessage_reader-0.5.0/imessage_reader/write_excel.py` & `imessage_reader-0.6.0/imessage_reader/write_excel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 
 """
 Write Excel file containing iMessage data (user id, text, date, service, account)
-Python 3.8+
+Python 3.9+
 Date created: October 1st, 2020
 Date modified: August 28th, 2021
 """
 
 from datetime import datetime
 
 import openpyxl
 from openpyxl.styles import Font
 
 
 class ExelWriter:
-    """
-    This class manages the export to excel.
+    """This class manages the export to excel.
     """
 
     def __init__(self, imessage_data: list, file_path: str):
-        """
-        The init function of this class
-        :param imessage_data: List with MessageData objects
+        """Constructor method
+
+        :param imessage_data: list with MessageData objects
                 containing user id, text, date, service and account
-        :param file_path: The path to the loaction of the Excel file
+        :param file_path: path to the location of the Excel file
         """
         self.imessage_data = imessage_data
         self.file_path = file_path
 
     def write_data(self):
-        """
-        Write data (user id, text, date, service, account, is_from_me) to Excel
+        """Write data to Excel
+        (user id, text, date, service, account, is_from_me)
         """
 
         users = []
         messages = []
         dates = []
         services = []
         accounts = []
@@ -112,20 +109,19 @@
 
         # Write is_from_me to 6th column
         is_from_me_row = 2
         for from_me in is_from_me:
             sheet.cell(row=is_from_me_row, column=6).value = from_me
             is_from_me_row += 1
 
-        # Save the workbook (excel file)
+        # Save the workbook (Excel file)
         try:
             workbook.save(
-                self.file_path
-                + f'iMessage-Data_{datetime.now().strftime("%Y-%m-%d")}.xlsx'
+                self.file_path + f'iMessage-Data_{datetime.now().strftime("%Y-%m-%d")}.xlsx'
             )
             print()
             print(">>> Excel file successfully created! <<<")
-            print("You find the Excel file in your Desktop folder.")
+            print("You find the Excel file in your Documents folder.")
             print()
         except IOError as e:
             print(">>> Cannot write Excel file! <<<")
             print(e)
```

### Comparing `imessage_reader-0.5.0/imessage_reader.egg-info/PKG-INFO` & `imessage_reader-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,141 @@
 Metadata-Version: 2.1
-Name: imessage-reader
-Version: 0.5.0
+Name: imessage_reader
+Version: 0.6.0
 Summary: Fetch recipients and chat messages from the chat.db database.
 Home-page: https://github.com/niftycode/imessage_reader
 Author: Bodo Schönfeld
 Author-email: bodo.schoenfeld@niftycode.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # imessage_reader
 
-![](img/license-MIT-green.svg) ![](img/python-3.8-blue.svg) ![](https://img.shields.io/github/last-commit/niftycode/imessage_reader.svg?style=flat) ![](https://img.shields.io/github/issues/niftycode/imessage_reader.svg?style=flat) ![](https://img.shields.io/travis/niftycode/imessage_reader/master) ![](https://img.shields.io/pypi/v/imessage_reader)
+![](img/license-MIT-green.svg) ![](img/python-3.9-blue.svg) ![](https://img.shields.io/github/last-commit/niftycode/imessage_reader.svg?style=flat) ![](https://img.shields.io/github/issues/niftycode/imessage_reader.svg?style=flat)  ![](https://img.shields.io/pypi/v/imessage_reader)
 
-This is a forensic tool written in Python 3. Use this tool to fetch the content (phone numbers, email addresses,
-messages and the account) from the *chat.db* database file on **macOS** (version 10.14 or above).
+This is a forensic tool written in Python 3. Use this tool to fetch the content (phone numbers, email addresses, messages and the account) from the *chat.db* database file on **macOS** (version 10.14 or above).
 
 The following information is currently being read from the database:
 
 * user id (sender's or recipient's phone number or email address)
 * message
 * date and time
 * service (iMessage or SMS)
 * account (destination caller id)
 * is the message from me
 
 ## Background
 
-Received messages (iMessage or SMS) and attachments will be saved in "~/Library/Messages". This directory contains a "
-chat.db" file (SQLite3) with two tables of interest: *handle* and *message*. The *handle* table contains the
-recipients (email address or phone number). The received messages are in the *message* table.
+Received messages (iMessage or SMS) and attachments will be saved in "~/Library/Messages". This directory contains a "chat.db" file (SQLite3) with two tables of interest: *handle* and *message*. The *handle* table contains the recipients (email address or phone number). The received messages are in the *message* table.
 
 ## Note
 
-Since the iMessage database is only available under macOS, it makes no sense to use this tool under Windows or Linux.
+Of course, the chat.db file is only created under macOS. Nevertheless, this program can also be used under Linux. In contrast to use under macOS, the path to the chat.db file must then be specified (see below).
 
 ## Requirements
 
-* **Python 3.8+**
+* Python 3.9+
 * openpyxl
 
 To run tests install **pytest**:
 
     pip3 install pytest
 
 ## Install
 
-    pip3 install imessage_reader
+    pip3 install imessage-reader
 
 ## Usage (CLI)
 
+## Specify no options
+
 Start the program with:
 
     imessage_reader
 
-This will show you all users and messages.
+This will show you all users and messages in the Terminal. If no option (`-p <PATH>`) is specified, the default directory (under macOS) is searched for the chat.db file.
+
+## Specify a PATH as argument
+
+A different path to chat.db file can be specified with the `-p` option:
+
+    imessage_reader -p <PATH>
+
+Unless the `-o` option is also used, the data is displayed in the Terminal.
+
+## Specify an output argument
+
+You can create an Excel file containing users, messages, date and service (SMS or iMessage). The file will be stored in the
+Documents folder:
 
-Use
+    imessage_reader -o e
 
-    imessage_reader -e
+or
 
-to create an Excel file containing users, messages, date and service (SMS or iMessage). The file will be stored in the
-Desktop folder.
+    imessage_reader -o excel
 
-Use
+You can create a SQLite3 database containing users, messages, date and service (SMS or iMessage). The file will be stored in the Documents folder:
 
-    imessage_reader -s
+    imessage_reader -o s
 
-to create a SQLite3 database containing users, messages, date and service (SMS or iMessage). The file will be stored in
-the Desktop folder.
+or
 
-Use
+    imessage_reader -o sqlite
+
+If you only want to see a list of recipients use:
 
     imessage_reader -r
 
-to show a list of recipients.
+or
+
+    imessage_reader --recipients
 
-**Note**: You need access to the *Library* folder in order to read the iMessage database file ("chat.db"). You can add
-access (for *Terminal* or *iTerm*) in
+**Note**: On **macOS** you need access to the *Library* folder in order to read the iMessage database file ("chat.db"). You can add access (for *Terminal* or *iTerm*) in
 
     > System Preferences > Security & Privacy > Privacy > Full Disk Access
 
+## Specify a PATH and an output argument
+
+You can combine the `-p` with the `-o` option:
+
+    imessage_reader -p /home/bodo/Downloads -o excel
+
+In this example the chat.db file is located in the Downloads folder (on a Linux machine). And the Excel file will be created in the Documents folder.
+
 ## Usage (import module)
 
 To get the messages use following code:
 
     from imessage_reader import fetch_data
-
+    
+    DB_PATH = /home/bodo/Downloads/chat.db
+    
     # Create a FetchData instance
-    fd = fetch_data.FetchData()
+    fd = fetch_data.FetchData(DB_PATH)
 
     # Store messages in my_data
-    # This is a list of tuples containing user id, message and service.
-    # service -> iMessage or SMS
+    # This is a list of tuples containing user id, message and service (iMessage or SMS).
     my_data = fd.get_messages()
     print(my_data)
 
 ## ToDo
 
 * ~~Get the date of messages~~
 * ~~Fetch the date of received messages.~~
-* Show a list of all known recipients.
+* ~~Show a list of all known recipients.~~
 * ~~Did the user receive the message via SMS or via iMessage?~~
 * ~~Create SQLite3 database.~~
+* ~~Specify a different path to the chat.db file.~~
 * Show attachments.
 * Add more tests.
 
 ## Changelog
 
 see [CHANGELOG.rst](https://github.com/niftycode/imessage_reader/blob/master/CHANGELOG.rst)
```

### Comparing `imessage_reader-0.5.0/setup.py` & `imessage_reader-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     author_email='bodo.schoenfeld@niftycode.de',
     url='https://github.com/niftycode/imessage_reader',
 
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: MacOS',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
 
     packages=find_packages(exclude=('tests', 'docs')),
     python_requires='>=3.8',
```

