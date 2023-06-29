# Comparing `tmp/sniimapp-0.0.2.tar.gz` & `tmp/sniimapp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.2.tar", last modified: Thu Jun 29 21:03:56 2023, max compression
+gzip compressed data, was "sniimapp-0.0.3.tar", last modified: Thu Jun 29 21:07:56 2023, max compression
```

## Comparing `sniimapp-0.0.2.tar` & `sniimapp-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:03:56.503090 sniimapp-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:03:56.503090 sniimapp-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2023-06-29 20:55:17.000000 sniimapp-0.0.2/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-29 21:03:28.000000 sniimapp-0.0.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 21:03:56.503090 sniimapp-0.0.2/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:03:56.503090 sniimapp-0.0.2/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:03:56.000000 sniimapp-0.0.2/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-29 21:03:56.000000 sniimapp-0.0.2/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 21:03:56.000000 sniimapp-0.0.2/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-29 21:03:56.000000 sniimapp-0.0.2/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1917 2023-06-29 20:57:42.000000 sniimapp-0.0.2/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:07:56.624972 sniimapp-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:07:56.624972 sniimapp-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2023-06-29 20:55:17.000000 sniimapp-0.0.3/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-29 21:07:38.000000 sniimapp-0.0.3/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 21:07:56.624972 sniimapp-0.0.3/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:07:56.624972 sniimapp-0.0.3/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2023-06-29 21:06:21.000000 sniimapp-0.0.3/sniimapp.py
```

### Comparing `sniimapp-0.0.2/LICENSE` & `sniimapp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.2/PKG-INFO` & `sniimapp-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.2/pyproject.toml` & `sniimapp-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.2/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.3/sniimapp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.2/sniimapp.py` & `sniimapp-0.0.3/sniimapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,33 @@
         self.product = product
         self.start_date = start_date
         self.end_date   = end_date
         self.MONGO_HOST = '18.215.228.120' #os.environ.get('MONGO_HOST')
         self.MONGO_PORT = '27017'          #os.environ.get('MONGO_PORT')
         self.MONGO_USER = 'fcca_read_1'    #os.environ.get('MONGO_USER')
         self.MONGO_PASSW ='Fcc4_R3_d_1'    #os.environ.get('MONGO_PASSWORD')
-        self.dbms=dbms
         self.client = MongoClient(self._connection_string)
         self.MONGO_DB = os.environ.get('MONGO_DATABASE')
         if product == 'fyh':
             self.db_collection = 'sniim_fyh'
         if product == 'granos':
             self.db_collection = 'sniim_granos'
         self.db = self.client[self.MONGO_DB]
         self.collection = self.db[self.db_collection]
 
     def get_data(self):
         start_date = self.start_date
         end_date   = self.end_date
-        dbms       = self.dbms
         if self.product == 'granos':
-            result = self.db_con('sniim_granos', start_date, end_date, dbms)
+            result = self.db_con('sniim_granos', start_date, end_date)
         if self.product == 'fyh':
-            result = self.db_con('sniim_fyh', start_date, end_date, dbms)
+            result = self.db_con('sniim_fyh', start_date, end_date)
         return result
 
-    def db_con(self, product, start_date, end_date, dbms):
+    def db_con(self, product, start_date, end_date):
         start_date = datetime.datetime.strptime(start_date, "%d/%m/%Y")
         end_date   = datetime.datetime.strptime(end_date,   "%d/%m/%Y")
         return self.collection.find({"fecha":{"$gte":start_date,"$lte":end_date}})
     
     @property
     def _connection_string(self):
         if os.environ.get('CONNECT_WITH_USER', 'False') == 'True':
```

