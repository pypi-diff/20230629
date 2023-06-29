# Comparing `tmp/piproc-0.1.8.tar.gz` & `tmp/piproc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piproc-0.1.8.tar", last modified: Thu Apr 27 14:13:36 2023, max compression
+gzip compressed data, was "piproc-0.1.9.tar", last modified: Thu Jun 29 08:22:33 2023, max compression
```

## Comparing `piproc-0.1.8.tar` & `piproc-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 14:13:36.111532 piproc-0.1.8/
--rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      266 2023-04-27 14:13:36.112042 piproc-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 14:13:36.094682 piproc-0.1.8/piproc/
--rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.8/piproc/__init__.py
--rw-rw-rw-   0        0        0    15987 2023-04-27 14:10:12.000000 piproc-0.1.8/piproc/main.py
--rw-rw-rw-   0        0        0     2834 2023-04-12 12:34:42.000000 piproc-0.1.8/piproc/tables.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:13:36.110528 piproc-0.1.8/piproc.egg-info/
--rw-rw-rw-   0        0        0      266 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-27 14:13:36.000000 piproc-0.1.8/piproc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 14:13:35.000000 piproc-0.1.8/piproc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      366 2023-04-27 14:13:36.113045 piproc-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:22:33.073951 piproc-0.1.9/
+-rw-rw-rw-   0        0        0     1087 2022-12-05 10:29:23.000000 piproc-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-06-29 08:22:33.074991 piproc-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6283 2022-11-24 11:51:36.000000 piproc-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:22:33.060835 piproc-0.1.9/piproc/
+-rw-rw-rw-   0        0        0       30 2022-11-24 13:51:50.000000 piproc-0.1.9/piproc/__init__.py
+-rw-rw-rw-   0        0        0    15749 2023-06-29 08:17:51.000000 piproc-0.1.9/piproc/main.py
+-rw-rw-rw-   0        0        0     2713 2023-06-29 08:18:55.000000 piproc-0.1.9/piproc/tables.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:22:33.073951 piproc-0.1.9/piproc.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-06-29 08:22:32.000000 piproc-0.1.9/piproc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-29 08:22:32.000000 piproc-0.1.9/piproc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:22:32.000000 piproc-0.1.9/piproc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-29 08:22:32.000000 piproc-0.1.9/piproc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 08:22:32.000000 piproc-0.1.9/piproc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      366 2023-06-29 08:22:33.075992 piproc-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-11-24 13:47:48.000000 piproc-0.1.9/setup.py
```

### Comparing `piproc-0.1.8/LICENSE` & `piproc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `piproc-0.1.8/README.md` & `piproc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `piproc-0.1.8/piproc/main.py` & `piproc-0.1.9/piproc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,18 @@
     def __init__(self):
         '''
         Initialise connection to the processing database, using locally found credentials or
         downloading them from s3.
         '''
         cred_path = os.path.join(up(up(__file__)), 'credentials.yml')
 
-        # The try/except is a hack for the cassini project, remove once competition is done.
-        try:
-            if not os.path.isfile(cred_path):
-                s3 = boto3.client('s3')
-                s3.download_file('dockerfilecfg', 'credentials.yml', 
-                    os.path.join(up(up(__file__)), 'credentials.yml'))
-        except NoCredentialsError:
-            cred_path = '/opt/cassini_vis/cred_files/credentials_piproc.yml'
+        if not os.path.isfile(cred_path):
+            s3 = boto3.client('s3')
+            s3.download_file('dockerfilecfg', 'credentials.yml', 
+                os.path.join(up(up(__file__)), 'credentials.yml'))
 
         with open(cred_path, 'r') as f:
             self.cred = yaml.safe_load(f)
 
         db = sqlalchemy.create_engine('postgresql:///processing', 
             connect_args={'host': self.cred['processing_db']['host'],
                           'user': self.cred['processing_db']['user'],
```

### Comparing `piproc-0.1.8/piproc/tables.py` & `piproc-0.1.9/piproc/tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
     no_downloaded = Column(Integer)
     date_downloaded = Column(DateTime)
     download_path = Column(String)
     indexed = Column(Integer)
     no_indexed = Column(Integer)
     date_indexed = Column(DateTime)
     index_path = Column(String)
-    fdi = Column(Integer)
-    no_fdi = Column(Integer)
-    date_fdi = Column(DateTime)
-    fdi_path = Column(String)
     prediction = Column(Integer)
     no_prediction = Column(Integer)
     date_prediction = Column(DateTime)
     pred_path = Column(String)
     model = Column(String)
 
 class Products(Base):
```

