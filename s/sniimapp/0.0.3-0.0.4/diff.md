# Comparing `tmp/sniimapp-0.0.3.tar.gz` & `tmp/sniimapp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.3.tar", last modified: Thu Jun 29 21:07:56 2023, max compression
+gzip compressed data, was "sniimapp-0.0.4.tar", last modified: Thu Jun 29 21:19:41 2023, max compression
```

## Comparing `sniimapp-0.0.3.tar` & `sniimapp-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:07:56.624972 sniimapp-0.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:07:56.624972 sniimapp-0.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2023-06-29 20:55:17.000000 sniimapp-0.0.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-29 21:07:38.000000 sniimapp-0.0.3/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 21:07:56.624972 sniimapp-0.0.3/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:07:56.624972 sniimapp-0.0.3/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-29 21:07:56.000000 sniimapp-0.0.3/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2023-06-29 21:06:21.000000 sniimapp-0.0.3/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:19:41.723255 sniimapp-0.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:19:41.723255 sniimapp-0.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2023-06-29 20:55:17.000000 sniimapp-0.0.4/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-29 21:15:54.000000 sniimapp-0.0.4/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 21:19:41.723255 sniimapp-0.0.4/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:19:41.723255 sniimapp-0.0.4/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      947 2023-06-29 21:19:41.000000 sniimapp-0.0.4/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-29 21:19:41.000000 sniimapp-0.0.4/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 21:19:41.000000 sniimapp-0.0.4/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-29 21:19:41.000000 sniimapp-0.0.4/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1951 2023-06-29 21:19:11.000000 sniimapp-0.0.4/sniimapp.py
```

### Comparing `sniimapp-0.0.3/LICENSE` & `sniimapp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.3/PKG-INFO` & `sniimapp-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.3/pyproject.toml` & `sniimapp-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.3/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.4/sniimapp.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.3/sniimapp.py` & `sniimapp-0.0.4/sniimapp.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         if self.product == 'fyh':
             result = self.db_con('sniim_fyh', start_date, end_date)
         return result
 
     def db_con(self, product, start_date, end_date):
         start_date = datetime.datetime.strptime(start_date, "%d/%m/%Y")
         end_date   = datetime.datetime.strptime(end_date,   "%d/%m/%Y")
+        start_date = start_date.strftime('%d/%m/%Y')
+        end_date   = end_date.strftime('%d/%m/%Y'  )
         return self.collection.find({"fecha":{"$gte":start_date,"$lte":end_date}})
     
     @property
     def _connection_string(self):
         if os.environ.get('CONNECT_WITH_USER', 'False') == 'True':
             return "mongodb://{0}:{1}@{2}:{3}".format(self.MONGO_USER, self.MONGO_PASSW, self.MONGO_HOST, self.MONGO_PORT)
         else:
```

