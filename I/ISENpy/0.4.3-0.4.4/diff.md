# Comparing `tmp/ISENpy-0.4.3.tar.gz` & `tmp/ISENpy-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ISENpy-0.4.3.tar", last modified: Thu Jun 29 15:54:05 2023, max compression
+gzip compressed data, was "ISENpy-0.4.4.tar", last modified: Thu Jun 29 16:36:48 2023, max compression
```

## Comparing `ISENpy-0.4.3.tar` & `ISENpy-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 15:54:05.833326 ISENpy-0.4.3/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 15:54:05.831680 ISENpy-0.4.3/ISENpy/
--rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-29 15:53:06.000000 ISENpy-0.4.3/ISENpy/__init__.py
--rwxr-xr-x   0 corentin   (501) staff       (20)     7083 2023-06-29 10:44:46.000000 ISENpy-0.4.3/ISENpy/client.py
--rwxr-xr-x   0 corentin   (501) staff       (20)    30076 2023-06-29 15:52:59.000000 ISENpy-0.4.3/ISENpy/dataClasses.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 15:54:05.832915 ISENpy-0.4.3/ISENpy.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.4.3/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 15:54:05.833146 ISENpy-0.4.3/PKG-INFO
--rwxr-xr-x   0 corentin   (501) staff       (20)     4991 2023-06-28 13:43:43.000000 ISENpy-0.4.3/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-29 15:54:05.833364 ISENpy-0.4.3/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-29 15:52:49.000000 ISENpy-0.4.3/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 16:36:48.791375 ISENpy-0.4.4/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 16:36:48.790190 ISENpy-0.4.4/ISENpy/
+-rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-29 16:35:56.000000 ISENpy-0.4.4/ISENpy/__init__.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)     7083 2023-06-29 10:44:46.000000 ISENpy-0.4.4/ISENpy/client.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)    30381 2023-06-29 16:35:56.000000 ISENpy-0.4.4/ISENpy/dataClasses.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 16:36:48.791056 ISENpy-0.4.4/ISENpy.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 16:36:48.000000 ISENpy-0.4.4/ISENpy.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-29 16:36:48.000000 ISENpy-0.4.4/ISENpy.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-29 16:36:48.000000 ISENpy-0.4.4/ISENpy.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-29 16:36:48.000000 ISENpy-0.4.4/ISENpy.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-29 16:36:48.000000 ISENpy-0.4.4/ISENpy.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.4.4/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 16:36:48.791253 ISENpy-0.4.4/PKG-INFO
+-rwxr-xr-x   0 corentin   (501) staff       (20)     4991 2023-06-28 13:43:43.000000 ISENpy-0.4.4/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-29 16:36:48.791414 ISENpy-0.4.4/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-29 16:35:56.000000 ISENpy-0.4.4/setup.py
```

### Comparing `ISENpy-0.4.3/ISENpy/__init__.py` & `ISENpy-0.4.4/ISENpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 """
 
 
 __title__ = "ISENpy"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 
 from .dataClasses import *
 from .client import *
```

### Comparing `ISENpy-0.4.3/ISENpy/client.py` & `ISENpy-0.4.4/ISENpy/client.py`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.3/ISENpy/dataClasses.py` & `ISENpy-0.4.4/ISENpy/dataClasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,19 +567,19 @@
 
         self.payloadReport = self.__getPayloadOfThePage(req.text)
 
         soup = BeautifulSoup(req.text, "html.parser")
 
         report = soup.find("div", {"class": "ui-datatable-tablewrapper"}).find("select").find_all("option")
 
-        result = {"nbReport": len(report), "data": {}}
+        result = {"nbReport": len(report), "data": []}
 
         for i in report:
             nameFile = i.text.split(".pdf")[0].strip() + ".pdf"
-            result["data"][nameFile] = i["value"]
+            result["data"].append({"name": nameFile, "id": i["value"]})
 
         self.infoReport = result
 
         return result
 
 
     def downloadReport(self, path: str = None, idReport: str = None) -> None:
@@ -600,21 +600,27 @@
         if self.infoReport["nbReport"] == 0:
             raise Exception("The user does not have any report")
 
         if self.infoReport["nbReport"] > 1 and path is not None:
             raise Exception("The user has more than one report. Please choose either no path or no specific path.")
 
         if path is None and idReport is not None:
-            path = list(self.infoReport["data"].keys())[0]
+            # self.infoReport format : {"nbReport": int, "data":  ({"name": "name", "id":"id"}, ...)}]}
+            for i in self.infoReport["data"]:
+                if i["id"] == idReport:
+                    path = i["name"]
+                    break
+            if path is None:
+                raise Exception("The report is not found")
 
         if idReport is None:
-            for i in self.infoReport["data"].keys():
+            for i in self.infoReport["data"]:
                 if path is None:
-                    path = i
-                self.downloadReport(path, self.infoReport["data"][i])
+                    path = i["name"]
+                self.downloadReport(path=i["name"], idReport=i["id"])
                 return
 
         urlChoixDonnee = "https://web.isen-ouest.fr/webAurion/faces/ChoixDonnee.xhtml"
 
         payload = {
             'form:j_idt193:0:j_idt209': 'form:j_idt193:0:j_idt209',
             "form:j_idt193:0:documents_input": idReport,
```

### Comparing `ISENpy-0.4.3/ISENpy.egg-info/PKG-INFO` & `ISENpy-0.4.4/ISENpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.4.3/LICENSE` & `ISENpy-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.3/PKG-INFO` & `ISENpy-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.4.3/README.md` & `ISENpy-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.3/setup.py` & `ISENpy-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ISENpy',
-    version='0.4.3',    
+    version='0.4.4',    
     description='A python API wrapper for ISEN-OUEST',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/ISENpy',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

