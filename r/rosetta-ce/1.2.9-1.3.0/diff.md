# Comparing `tmp/rosetta-ce-1.2.9.tar.gz` & `tmp/rosetta-ce-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.2.9.tar", last modified: Thu Jun 29 14:07:53 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.0.tar", last modified: Thu Jun 29 15:07:02 2023, max compression
```

## Comparing `rosetta-ce-1.2.9.tar` & `rosetta-ce-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 14:07:53.529858 rosetta-ce-1.2.9/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.2.9/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 14:07:53.529543 rosetta-ce-1.2.9/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.2.9/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 14:07:53.524275 rosetta-ce-1.2.9/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.2.9/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 14:07:53.526098 rosetta-ce-1.2.9/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.2.9/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.2.9/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.2.9/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.2.9/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.2.9/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    33107 2023-06-29 14:07:09.000000 rosetta-ce-1.2.9/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     7785 2023-06-29 06:42:23.000000 rosetta-ce-1.2.9/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 14:07:53.527842 rosetta-ce-1.2.9/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 14:07:53.000000 rosetta-ce-1.2.9/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 14:07:53.000000 rosetta-ce-1.2.9/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 14:07:53.000000 rosetta-ce-1.2.9/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 14:07:53.000000 rosetta-ce-1.2.9/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 14:07:53.000000 rosetta-ce-1.2.9/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 14:07:53.529906 rosetta-ce-1.2.9/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 14:07:20.000000 rosetta-ce-1.2.9/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 14:07:53.529055 rosetta-ce-1.2.9/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.2.9/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.2.9/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.2.9/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.666349 rosetta-ce-1.3.0/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.0/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:07:02.666054 rosetta-ce-1.3.0/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.0/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.660006 rosetta-ce-1.3.0/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.0/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.662026 rosetta-ce-1.3.0/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.0/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.0/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.0/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.0/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.0/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    33530 2023-06-29 15:05:33.000000 rosetta-ce-1.3.0/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     7785 2023-06-29 06:42:23.000000 rosetta-ce-1.3.0/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.664106 rosetta-ce-1.3.0/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 15:07:02.666393 rosetta-ce-1.3.0/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 15:05:54.000000 rosetta-ce-1.3.0/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.665521 rosetta-ce-1.3.0/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.0/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.0/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.0/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.2.9/LICENSE` & `rosetta-ce-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/PKG-INFO` & `rosetta-ce-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.2.9
+Version: 1.3.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.2.9/README.md` & `rosetta-ce-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/rosetta/constants/sensors.py` & `rosetta-ce-1.3.0/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/rosetta/constants/sources.py` & `rosetta-ce-1.3.0/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/rosetta/constants/systems.py` & `rosetta-ce-1.3.0/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/rosetta/rconverter.py` & `rosetta-ce-1.3.0/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/rosetta/rfaker.py` & `rosetta-ce-1.3.0/rosetta/rfaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,23 +542,27 @@
                 'cve': cve_id
             }
             json_messages.append(event)
         return json_messages
 
     @classmethod
     def incidents(cls, count, fields: Optional[str] = None, timestamp: Optional[datetime] = None,
+                  vendor: Optional[str] = None, product: Optional[str] = None, version: Optional[str] = None,
                   observables: Optional[Observables] = None) -> List[dict]:
         """
         Generates a list of fake incident data.
 
         Args:
             count (int): The number of incidents to generate.
             fields (str, optional): A comma-separated list of incident fields to include in the output. If None,
                 all fields will be included. Valid options are: 'id', 'duration', 'type', 'analyst', 'severity',
                 'description', 'events'.
+            vendor: Optional. The vendor.
+            product: Optional. The product.
+            version: Optional. The version.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
 
         Returns:
             List[Dict]: A list of incident dictionaries. Each dictionary contains the following fields:
                 - 'id' (int): A unique identifier for the incident.
                 - 'type' (str): The type of incident.
@@ -624,16 +628,18 @@
                     incident['severity'] = severity
                 if 'description' in field_list:
                     incident_description = faker.paragraph(nb_sentences=1, ext_word_list=description)
                     incident['description'] = incident_description
                 if 'events' in field_list:
                     incident['events'] = [
                         {"event": cls.syslog(count=1, timestamp=timestamp, observables=observables)[0]},
-                        {"event": cls.cef(count=1, timestamp=timestamp, observables=observables)[0]},
-                        {"event": cls.leef(count=1, timestamp=timestamp, observables=observables)[0]},
+                        {"event": cls.cef(count=1, timestamp=timestamp, vendor=vendor, product=product,
+                                          version=version, observables=observables)[0]},
+                        {"event": cls.leef(count=1, timestamp=timestamp, vendor=vendor, product=product,
+                                           version=version, observables=observables)[0]},
                         {"event": cls.winevent(count=1, timestamp=timestamp, observables=observables)[0]},
                         {"event": cls.json(count=1, timestamp=timestamp, observables=observables)[0]}
                     ]
             else:
                 incident = {
                     "id": incident_id,
                     "type": incident_type,
```

### Comparing `rosetta-ce-1.2.9/rosetta/rsender.py` & `rosetta-ce-1.3.0/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.0/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.2.9
+Version: 1.3.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.2.9/setup.py` & `rosetta-ce-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.2.9",
+    version="1.3.0",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.2.9/tests/test_rconverter.py` & `rosetta-ce-1.3.0/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/tests/test_rfaker.py` & `rosetta-ce-1.3.0/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.2.9/tests/test_rsender.py` & `rosetta-ce-1.3.0/tests/test_rsender.py`

 * *Files identical despite different names*

