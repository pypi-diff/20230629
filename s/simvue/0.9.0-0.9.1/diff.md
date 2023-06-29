# Comparing `tmp/simvue-0.9.0.tar.gz` & `tmp/simvue-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simvue-0.9.0.tar", last modified: Wed Jan 25 15:01:16 2023, max compression
+gzip compressed data, was "simvue-0.9.1.tar", last modified: Wed Jan 25 21:15:35 2023, max compression
```

## Comparing `simvue-0.9.0.tar` & `simvue-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 15:01:16.552285 simvue-0.9.0/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3770 2023-01-25 15:01:16.552285 simvue-0.9.0/PKG-INFO
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2885 2023-01-25 14:57:49.000000 simvue-0.9.0/README.md
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 15:01:16.552285 simvue-0.9.0/bin/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      763 2023-01-25 14:57:49.000000 simvue-0.9.0/bin/simvue_sender
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       38 2023-01-25 15:01:16.552285 simvue-0.9.0/setup.cfg
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      766 2023-01-25 14:57:49.000000 simvue-0.9.0/setup.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 15:01:16.552285 simvue-0.9.0/simvue/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      152 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/__init__.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1333 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/api.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4826 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/client.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      530 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/handler.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     1728 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/metrics.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      459 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/models.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3174 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/offline.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)   150877 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/pynvml.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7005 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/remote.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)    22429 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/run.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     7816 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/sender.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     4863 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/serialization.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      249 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/simvue.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     2161 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/utilities.py
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     5562 2023-01-25 14:57:49.000000 simvue-0.9.0/simvue/worker.py
-drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 15:01:16.552285 simvue-0.9.0/simvue.egg-info/
--rw-rw-r--   0 rocky     (1000) rocky     (1000)     3770 2023-01-25 15:01:16.000000 simvue-0.9.0/simvue.egg-info/PKG-INFO
--rw-rw-r--   0 rocky     (1000) rocky     (1000)      479 2023-01-25 15:01:16.000000 simvue-0.9.0/simvue.egg-info/SOURCES.txt
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        1 2023-01-25 15:01:16.000000 simvue-0.9.0/simvue.egg-info/dependency_links.txt
--rw-rw-r--   0 rocky     (1000) rocky     (1000)       60 2023-01-25 15:01:16.000000 simvue-0.9.0/simvue.egg-info/requires.txt
--rw-rw-r--   0 rocky     (1000) rocky     (1000)        7 2023-01-25 15:01:16.000000 simvue-0.9.0/simvue.egg-info/top_level.txt
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 21:15:35.534604 simvue-0.9.1/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3873 2023-01-25 21:15:35.534604 simvue-0.9.1/PKG-INFO
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2980 2023-01-25 21:11:11.000000 simvue-0.9.1/README.md
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 21:15:35.533604 simvue-0.9.1/bin/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      763 2023-01-25 21:11:11.000000 simvue-0.9.1/bin/simvue_sender
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       38 2023-01-25 21:15:35.534604 simvue-0.9.1/setup.cfg
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      766 2023-01-25 21:11:11.000000 simvue-0.9.1/setup.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 21:15:35.533604 simvue-0.9.1/simvue/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      152 2023-01-25 21:15:30.000000 simvue-0.9.1/simvue/__init__.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1397 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/api.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4826 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/client.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      530 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/handler.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     1728 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/metrics.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      459 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/models.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3174 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/offline.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)   150877 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/pynvml.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7005 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/remote.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)    22569 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/run.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     7816 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/sender.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     4863 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/serialization.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      249 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/simvue.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     2161 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/utilities.py
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     5562 2023-01-25 21:11:11.000000 simvue-0.9.1/simvue/worker.py
+drwxrwxr-x   0 rocky     (1000) rocky     (1000)        0 2023-01-25 21:15:35.534604 simvue-0.9.1/simvue.egg-info/
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)     3873 2023-01-25 21:15:35.000000 simvue-0.9.1/simvue.egg-info/PKG-INFO
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)      479 2023-01-25 21:15:35.000000 simvue-0.9.1/simvue.egg-info/SOURCES.txt
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        1 2023-01-25 21:15:35.000000 simvue-0.9.1/simvue.egg-info/dependency_links.txt
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)       60 2023-01-25 21:15:35.000000 simvue-0.9.1/simvue.egg-info/requires.txt
+-rw-rw-r--   0 rocky     (1000) rocky     (1000)        7 2023-01-25 21:15:35.000000 simvue-0.9.1/simvue.egg-info/top_level.txt
```

### Comparing `simvue-0.9.0/PKG-INFO` & `simvue-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simvue
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simulation tracking and monitoring
 Home-page: https://simvue.io
 Author-email: info@simvue.io
 License: UNKNOWN
 Description: 
         # Simvue Python client
         
@@ -33,15 +33,16 @@
         
         ...
         
         if __name__ == "__main__":
         
             ...
         
-            # Using a context manager means that the status will be set to completed automatically
+            # Using a context manager means that the status will be set to completed automatically,
+            # and also means that if the code exits with an exception this will be reported to Simvue
             with Run() as run:
         
                 # Specify a run name, metadata (dict), tags (list), description, folder
                 run.init('example-run-name',
                          {'learning_rate': 0.001, 'training_steps': 2000, 'batch_size': 32}, # Metadaata
                          ['tensorflow'],                                                     # Tags
                          'This is a test.',                                                  # Description
```

### Comparing `simvue-0.9.0/README.md` & `simvue-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 ...
 
 if __name__ == "__main__":
 
     ...
 
-    # Using a context manager means that the status will be set to completed automatically
+    # Using a context manager means that the status will be set to completed automatically,
+    # and also means that if the code exits with an exception this will be reported to Simvue
     with Run() as run:
 
         # Specify a run name, metadata (dict), tags (list), description, folder
         run.init('example-run-name',
                  {'learning_rate': 0.001, 'training_steps': 2000, 'batch_size': 32}, # Metadaata
                  ['tensorflow'],                                                     # Tags
                  'This is a test.',                                                  # Description
```

### Comparing `simvue-0.9.0/bin/simvue_sender` & `simvue-0.9.1/bin/simvue_sender`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/setup.py` & `simvue-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/api.py` & `simvue-0.9.1/simvue/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,22 +24,24 @@
     """
     HTTP POST with retries
     """
     if is_json:
         data = json.dumps(data)
         headers = set_json_header(headers)
     response = requests.post(url, headers=headers, data=data, timeout=DEFAULT_API_TIMEOUT)
+    response.raise_for_status()
 
     return response
 
 @retry(wait=wait_exponential(multiplier=RETRY_MULTIPLIER, min=RETRY_MIN, max=RETRY_MAX),
                              stop=stop_after_attempt(RETRY_STOP))
 def put(url, headers, data, is_json=True, timeout=DEFAULT_API_TIMEOUT):
     """
     HTTP PUT with retries
     """
     if is_json:
         data = json.dumps(data)
         headers = set_json_header(headers)
     response = requests.put(url, headers=headers, data=data, timeout=timeout)
+    response.raise_for_status()
 
     return response
```

### Comparing `simvue-0.9.0/simvue/client.py` & `simvue-0.9.1/simvue/client.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/handler.py` & `simvue-0.9.1/simvue/handler.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/metrics.py` & `simvue-0.9.1/simvue/metrics.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/offline.py` & `simvue-0.9.1/simvue/offline.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/pynvml.py` & `simvue-0.9.1/simvue/pynvml.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/remote.py` & `simvue-0.9.1/simvue/remote.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/run.py` & `simvue-0.9.1/simvue/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,14 +553,16 @@
             mimetype = filetype
 
         if mimetype:
             data['type'] = mimetype
 
         if not is_file:
             data['pickled'], data['type'] = Serializer().serialize(filename, allow_pickle)
+            if not data['type'] and not allow_pickle:
+                self._error('Unable to save Python object, set allow_pickle to True')
             data['checksum'] = calculate_sha256(data['pickled'], False)
             data['originalPath'] = ''
             data['size'] = sys.getsizeof(data['pickled'])
 
         # Register file
         if not self._simvue.save_file(data):
             return False
```

### Comparing `simvue-0.9.0/simvue/sender.py` & `simvue-0.9.1/simvue/sender.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/serialization.py` & `simvue-0.9.1/simvue/serialization.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/utilities.py` & `simvue-0.9.1/simvue/utilities.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue/worker.py` & `simvue-0.9.1/simvue/worker.py`

 * *Files identical despite different names*

### Comparing `simvue-0.9.0/simvue.egg-info/PKG-INFO` & `simvue-0.9.1/simvue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simvue
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simulation tracking and monitoring
 Home-page: https://simvue.io
 Author-email: info@simvue.io
 License: UNKNOWN
 Description: 
         # Simvue Python client
         
@@ -33,15 +33,16 @@
         
         ...
         
         if __name__ == "__main__":
         
             ...
         
-            # Using a context manager means that the status will be set to completed automatically
+            # Using a context manager means that the status will be set to completed automatically,
+            # and also means that if the code exits with an exception this will be reported to Simvue
             with Run() as run:
         
                 # Specify a run name, metadata (dict), tags (list), description, folder
                 run.init('example-run-name',
                          {'learning_rate': 0.001, 'training_steps': 2000, 'batch_size': 32}, # Metadaata
                          ['tensorflow'],                                                     # Tags
                          'This is a test.',                                                  # Description
```

