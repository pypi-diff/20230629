# Comparing `tmp/awsgnssroutils-1.0.3.tar.gz` & `tmp/awsgnssroutils-1.0.4.tar.gz`

## Comparing `awsgnssroutils-1.0.3.tar` & `awsgnssroutils-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.3/src/awsgnssroutils/__init__.py
--rw-r--r--   0        0        0    38566 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.3/src/awsgnssroutils/database.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.3/LICENSE
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.3/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/src/awsgnssroutils/__init__.py
+-rw-r--r--   0        0        0    38941 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/src/awsgnssroutils/database.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/LICENSE
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/PKG-INFO
```

### Comparing `awsgnssroutils-1.0.3/src/awsgnssroutils/database.py` & `awsgnssroutils-1.0.4/src/awsgnssroutils/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """database.py
 
 Authors: Amy McVey (amcvey@aer.com) and Stephen Leroy (sleroy@aer.com)
-Date: 19 December 2022
+Date: 29 June 2023
 
 ================================================================================
 
 This module contains utilities to query the AWS Registry of Open Data repository
 of GNSS radio occultation data. It does so using database files posted in the
 AWS repository.
 
@@ -14,28 +14,28 @@
 This module defines two classes: RODatabaseClient and OccList. The first
 creates a portal to a database of RO metadata, and the second is an instance
 of a list of radio occultations (ROs). Each are described below.
 
 RODatabaseClient:
     Create an instance of a portal to a metadata on all RO data in the AWS
     Registry of Open Data. It provides an option to create a repository of
-    the RO metadata on the local file system as keyword "repository". 
+    the RO metadata on the local file system as keyword "repository".
 
-OccList: 
+OccList:
     An instance of the class OccList is contains the metadata on a list of RO
     soundings along with pointers to the RO data files in the AWS Registry of
     Open Data S3 bucket. AWS functionality is completely embedded in the
     methods of the OccList class. Those methods include the ability to
     subset/filter the list according to geolocation and time,
     GNSS transmitter/constellation, GNSS receiver, whether it is a rising or a
     setting occultation, etc. It also includes the ability to combine
     instances of OccList, save the OccList to a JSON format file for future
     restoration by RODatabaseClient.restore, and even download RO data files.
 
-See README documentation for further instruction on usage. 
+See README documentation for further instruction on usage.
 
 """
 
 #  Define parameters of the database.
 
 AWSregion = "us-east-1"
 databaseS3bucket = "gnss-ro-data"
@@ -51,33 +51,41 @@
 import json
 import re
 import time
 from botocore import UNSIGNED
 
 #  Usefule parameters.
 
-valid_processing_centers = [ "ucar", "romsaf", "jpl" ]
+
+#Update valid processing centers based on open data bucket listing
+s3 = s3fs.S3FileSystem( client_kwargs={ 'region_name': AWSregion },
+                                 config_kwargs={ 'signature_version': UNSIGNED }
+#lists processing_centers on open data bucket
+initial_prefix_array = s3.ls( os.path.join( databaseS3bucket, f'contributed/v1.1/' ) )
+valid_processing_centers = [os.path.basename(prefix) for prefix in initial_prefix_array ]
+
 valid_file_types = [ "calibratedPhase", "refractivityRetrieval", "atmosphericRetrieval" ]
 
 #  Exception handling.
 
 class Error( Exception ):
     pass
 
 class AWSgnssroutilsError( Error ):
     def __init__( self, message, comment ):
         self.message = message
         self.comment = comment
 
 
-
 ################################################################################
 #  Useful utility functions and classes.
 ################################################################################
 
+
+
 def unsigned_S3FileSystem():
     """This is a custom function that contains code to generate an authenticated
     instance of s3fs.S3FileSystem. In this particular case, authentication is
     UNSIGNED."""
 
     s3 = s3fs.S3FileSystem( client_kwargs={ 'region_name': AWSregion },
                                      config_kwargs={ 'signature_version': UNSIGNED } )
@@ -840,15 +848,15 @@
 
         #  With file array, open up and read files in to query more.
 
         ret_list = OccList( data=[], s3=self._s3 )
 
         for file in file_array:
             if self._repository is None:
-                with self._s3.open(file, 'r') as f:
+                with self._s3.open(file) as f:
                     df_dict = json.loads( f.readline() )
             else:
                 with open(file, 'r') as f:
                     df_dict = json.loads( f.readline() )
             df = list( df_dict.values() )
 
             add_list = OccList( df, self._s3 ).filter( missions=missions, receivers=receivers,
```

### Comparing `awsgnssroutils-1.0.3/LICENSE` & `awsgnssroutils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.0.3/README.md` & `awsgnssroutils-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.0.3/pyproject.toml` & `awsgnssroutils-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling", "s3fs", "numpy" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awsgnssroutils"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
 	{ name="Stephen Leroy", email="sleroy@aer.com" },
 	{ name="Amy McVey", email="amcvey@aer.com" }
 	]
 description = "Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `awsgnssroutils-1.0.3/PKG-INFO` & `awsgnssroutils-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsgnssroutils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data
 Project-URL: Homepage, https://github.com/gnss-ro/aws-opendata
 Project-URL: Bug Tracker, https://github.com/gnss-ro/aws-opendata/issues
 Author-email: Stephen Leroy <sleroy@aer.com>, Amy McVey <amcvey@aer.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

