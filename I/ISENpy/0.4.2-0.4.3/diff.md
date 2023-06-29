# Comparing `tmp/ISENpy-0.4.2.tar.gz` & `tmp/ISENpy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ISENpy-0.4.2.tar", last modified: Thu Jun 29 11:17:19 2023, max compression
+gzip compressed data, was "ISENpy-0.4.3.tar", last modified: Thu Jun 29 15:54:05 2023, max compression
```

## Comparing `ISENpy-0.4.2.tar` & `ISENpy-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 11:17:19.015312 ISENpy-0.4.2/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 11:17:19.014534 ISENpy-0.4.2/ISENpy/
--rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-29 11:16:26.000000 ISENpy-0.4.2/ISENpy/__init__.py
--rwxr-xr-x   0 corentin   (501) staff       (20)     7083 2023-06-29 10:44:46.000000 ISENpy-0.4.2/ISENpy/client.py
--rwxr-xr-x   0 corentin   (501) staff       (20)    29896 2023-06-29 11:14:47.000000 ISENpy-0.4.2/ISENpy/dataClasses.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 11:17:19.015073 ISENpy-0.4.2/ISENpy.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 11:17:19.000000 ISENpy-0.4.2/ISENpy.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-29 11:17:19.000000 ISENpy-0.4.2/ISENpy.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-29 11:17:19.000000 ISENpy-0.4.2/ISENpy.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-29 11:17:19.000000 ISENpy-0.4.2/ISENpy.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-29 11:17:19.000000 ISENpy-0.4.2/ISENpy.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.4.2/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 11:17:19.015208 ISENpy-0.4.2/PKG-INFO
--rwxr-xr-x   0 corentin   (501) staff       (20)     4991 2023-06-28 13:43:43.000000 ISENpy-0.4.2/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-29 11:17:19.015348 ISENpy-0.4.2/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-29 11:16:29.000000 ISENpy-0.4.2/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 15:54:05.833326 ISENpy-0.4.3/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 15:54:05.831680 ISENpy-0.4.3/ISENpy/
+-rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-29 15:53:06.000000 ISENpy-0.4.3/ISENpy/__init__.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)     7083 2023-06-29 10:44:46.000000 ISENpy-0.4.3/ISENpy/client.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)    30076 2023-06-29 15:52:59.000000 ISENpy-0.4.3/ISENpy/dataClasses.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 15:54:05.832915 ISENpy-0.4.3/ISENpy.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-29 15:54:05.000000 ISENpy-0.4.3/ISENpy.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.4.3/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 15:54:05.833146 ISENpy-0.4.3/PKG-INFO
+-rwxr-xr-x   0 corentin   (501) staff       (20)     4991 2023-06-28 13:43:43.000000 ISENpy-0.4.3/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-29 15:54:05.833364 ISENpy-0.4.3/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-29 15:52:49.000000 ISENpy-0.4.3/setup.py
```

### Comparing `ISENpy-0.4.2/ISENpy/__init__.py` & `ISENpy-0.4.3/ISENpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 """
 
 
 __title__ = "ISENpy"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 
 from .dataClasses import *
 from .client import *
```

### Comparing `ISENpy-0.4.2/ISENpy/client.py` & `ISENpy-0.4.3/ISENpy/client.py`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.2/ISENpy/dataClasses.py` & `ISENpy-0.4.3/ISENpy/dataClasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,27 +279,30 @@
         for i in planning["events"]:
             info = i["title"].split(" - ")
             planning_data = {
                 "id": i["id"],
                 "start": i["start"],
                 "end": i["end"],
                 "className": i["className"],
-                "debut": info[0],
-                "fin": info[1],
-                "salle": info[-1],
                 "type": info[2],
                 "matiere": info[3] if i["className"] != "DS" else ", ".join(info[4:-3]),
                 "description": ", ".join(info[4:-2]) if i["className"] != "DS" else ", ".join(info[4:-3]),
                 "intervenants": info[-2]
             }
 
             if isOtherPlanning:
+                planning_data["debut"] = info[0]
+                planning_data["fin"] = info[1]
+                planning_data["salle"] = info[-1]
                 planning_data["classe"] = classe
             else:
-                planning_data["classe"] = classe if i["className"] == "DS" else info[-1]
+                planning_data["debut"] = info[0].split(" à ")[0]
+                planning_data["fin"] = info[0].split(" à ")[1]
+                planning_data["salle"] = info[1]
+                planning_data["classe"] = info[-1]
 
             workingTime.append(planning_data)
 
         # Return the list of dict of the planning
         return workingTime
 
 
@@ -338,82 +341,85 @@
 
     def getClassPlanning(self):
         """Get the planning of the webAurion class.
 
         Returns:
             list: List of classes.
         """
-        information = "Group Schedules"
+        information = "Plannings des groupes"
         id_information = self.id_leftMenu[information]
         soup = self.__soupForPlanning(self.dataOtherPlanning, id_information)
-        listOfClasses = soup.find("li", {"class": "fully-loaded-children"}).find_all("li")
+        listOfClasses = soup.find("li", {"class": "enfants-entierement-charges"}).find_all("li")
         for child in listOfClasses:
             self.classPlanning[child.find("span", {"class": "ui-menuitem-text"}).text] = child["class"][-2].split("_")[-1]
         return list(self.classPlanning.keys())
 
 
-    def getClassCity(self, classPlanning: str = "CIR"):
+    def getClassCity(self, classPlanning: str = "Plannings CIR"):
         """Get the city of the class.
 
         Args:
             classPlanning (str, optional): Class of the planning. Defaults to "CIR".
 
         Returns:
             list: List of cities.
         """
-        classPlanning = "Planning " + classPlanning
+        classPlanning = classPlanning
         id_classPlanning = self.classPlanning[classPlanning]
         soup = self.__soupForPlanning(self.dataOtherPlanning, id_classPlanning)
         listOfCities = soup.find("li", {"class": f"submenu_{id_classPlanning}"}).find_all("li")
         for child in listOfCities:
             self.classCity[child.find("span", {"class": "ui-menuitem-text"}).text] = child["class"][-2].split("_")[-1]
         self.classPlanning[classPlanning] = {"city": self.classCity}
         return list(self.classCity.keys())
 
 
-    def getClassYear(self, classPlanning: str = "CIR", classCity: str = "Caen"):
+    def getClassYear(self, classCity: str = "Plannings CIR Caen"):
         """Get the year of the class.
 
         Args:
             classPlanning (str, optional): Class of the planning. Defaults to "CIR".
             classCity (str, optional): City of the planning. Defaults to "Caen".
 
         Returns:
             list: List of years.
         """
-        classPlanning = "Planning " + classPlanning
-        classCity = classPlanning + " " + classCity
+        
+        classPlanning = " ".join(classCity.split(" ")[:-1])
+
         id_classCity = self.classPlanning[classPlanning]["city"][classCity]
         soup = self.__soupForPlanning(self.dataOtherPlanning, id_classCity)
         listOfYears = soup.find("li", {"class": f"submenu_{id_classCity}"}).find_all("li")
         for child in listOfYears:
             dictionary = child.find("a")["onclick"].split("'form',")[1].split(").submit")[0].replace("'", '"')
             try:
                 dictionary = json.loads(dictionary)
             except:
                 dictionary = {}
             self.classYear[child.find("span", {"class": "ui-menuitem-text"}).text] = dictionary
         self.classPlanning[classPlanning]["city"][classCity] = {"year": self.classYear}
         return list(self.classYear.keys())
 
 
-    def getClassGroup(self, classPlanning: str = "CIR", classCity: str = "Caen", classYear: str = "1"):
+    def getClassGroup(self, classYear: str = "Plannings CIR Caen 1"):
         """Get the group of the class.
 
         Args:
             classPlanning (str, optional): Class of the planning. Defaults to "CIR".
             classCity (str, optional): City of the planning. Defaults to "Caen".
             classYear (str, optional): Year of the planning. Defaults to "1".
 
         Returns:
             list: List of groups.
         """
-        classPlanning = "Planning " + classPlanning
-        classCity = classPlanning + " " + classCity
-        classYear = classPlanning + " " + classYear
+
+        classPlanning = " ".join(classYear.split(" ")[:-2])
+        classCity = classPlanning + " " + classYear.split(" ")[-2]
+        classYear = classPlanning + " " + classYear.split(" ")[-1]
+        
         payloadOfLastClass = self.classYear[classYear]
         payloadOfLastClass.update(self.payload)
         req = self.session.post(self.baseMainPageUrl, data=payloadOfLastClass)
         soup = BeautifulSoup(req.text, "html.parser")
         allLastClass = soup.find("tbody", {"class": "ui-datatable-data"}).find_all("tr")
         for child in allLastClass:
             self.classGroup[child.find("span", {"class": "preformatted"}).text] = child["data-rk"]
@@ -456,15 +462,17 @@
 
         for city in allClassesPossible[classPlanning]:
             if classCity in city.keys() and classYear not in city[classCity]:
                 raise Exception("The classYear is not in the list of the planning", city[classCity])
 
         classPlanning = "Plannings " + classPlanning
         classCity = classPlanning + " " + classCity
+        globalClass = classCity + " " + classYear
         classYear = classPlanning + " " + classYear
+        
 
         self.getClassPlanning()
 
         if classPlanning not in self.classPlanning:
             raise Exception("The classPlanning is not in the list of the planning")
 
         if not classPlanning:
@@ -474,20 +482,20 @@
             raise Exception("Enter value of", list(self.classPlanning[classPlanning]["city"].keys()))
 
         self.getClassCity(classPlanning)
 
         if not classYear:
             raise Exception("Enter value of", list(self.classPlanning[classPlanning]["city"][classCity]["year"].keys()))
 
-        self.getClassYear(classPlanning, classCity)
+        self.getClassYear(classCity)
 
         if not classGroup:
             raise Exception("Enter value of", list(self.classPlanning[classPlanning]["city"][classCity]["year"][classYear]["group"].keys()))
 
-        self.getClassGroup(classPlanning, classCity, classYear)
+        self.getClassGroup(globalClass)
 
         if classGroup not in self.classGroup:
             raise Exception("The classGroup is not in the list of the planning", list(self.classGroup.keys()))
 
         lastPayload = {
             "form:j_idt181_reflowDD": "0_0",
             "form:j_idt181:j_idt186:filter": "",
```

### Comparing `ISENpy-0.4.2/ISENpy.egg-info/PKG-INFO` & `ISENpy-0.4.3/ISENpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.4.2/LICENSE` & `ISENpy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.2/PKG-INFO` & `ISENpy-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.4.2/README.md` & `ISENpy-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.2/setup.py` & `ISENpy-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ISENpy',
-    version='0.4.2',    
+    version='0.4.3',    
     description='A python API wrapper for ISEN-OUEST',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/ISENpy',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

