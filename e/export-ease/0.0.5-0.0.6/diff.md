# Comparing `tmp/export_ease-0.0.5.tar.gz` & `tmp/export_ease-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ease-0.0.5.tar", last modified: Mon Apr 17 01:35:35 2023, max compression
+gzip compressed data, was "export_ease-0.0.6.tar", last modified: Thu Jun 29 20:48:01 2023, max compression
```

## Comparing `export_ease-0.0.5.tar` & `export_ease-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.846650 export_ease-0.0.5/
--rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.5/LICENSE
--rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-17 01:35:35.846496 export_ease-0.0.5/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)     4253 2023-04-16 22:09:55.000000 export_ease-0.0.5/README.md
--rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-17 01:35:19.000000 export_ease-0.0.5/pyproject.toml
--rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-17 01:35:35.846692 export_ease-0.0.5/setup.cfg
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.845024 export_ease-0.0.5/src/
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.845770 export_ease-0.0.5/src/export_ease/
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.5/src/export_ease/__init__.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.5/src/export_ease/comtrade.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 23:10:39.000000 export_ease-0.0.5/src/export_ease/imf.py
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.846307 export_ease-0.0.5/src/export_ease.egg-info/
--rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/SOURCES.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/dependency_links.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/top_level.txt
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-06-29 20:48:01.538364 export_ease-0.0.6/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.6/LICENSE
+-rw-r--r--   0 pauldilly   (501) staff       (20)     5129 2023-06-29 20:48:01.538248 export_ease-0.0.6/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4603 2023-06-29 15:15:05.000000 export_ease-0.0.6/README.md
+-rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-06-29 20:43:07.000000 export_ease-0.0.6/pyproject.toml
+-rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-06-29 20:48:01.538408 export_ease-0.0.6/setup.cfg
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-06-29 20:48:01.536787 export_ease-0.0.6/src/
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-06-29 20:48:01.537567 export_ease-0.0.6/src/export_ease/
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.6/src/export_ease/__init__.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     5187 2023-06-29 14:26:25.000000 export_ease-0.0.6/src/export_ease/comtrade.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     3761 2023-04-17 01:36:11.000000 export_ease-0.0.6/src/export_ease/imf.py
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-06-29 20:48:01.538074 export_ease-0.0.6/src/export_ease.egg-info/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     5129 2023-06-29 20:48:01.000000 export_ease-0.0.6/src/export_ease.egg-info/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-06-29 20:48:01.000000 export_ease-0.0.6/src/export_ease.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-06-29 20:48:01.000000 export_ease-0.0.6/src/export_ease.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-06-29 20:48:01.000000 export_ease-0.0.6/src/export_ease.egg-info/top_level.txt
```

### Comparing `export_ease-0.0.5/LICENSE` & `export_ease-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.5/PKG-INFO` & `export_ease-0.0.6/src/export_ease.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: export_ease
-Version: 0.0.5
+Name: export-ease
+Version: 0.0.6
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,16 +13,18 @@
 
 # export_ease
 Built upon Python modules that call JSON RESTful API to gather macroeconomic data, this package offers a streamlined interface through which you can request and subsequently analyze vast amounts of macroeconomic data from sources including UN Comtrade and the International Monetary Fund (IMF). Below is a step-by-step guide detailing effective use of this program. (This package was built to supplement a [research project](https://github.com/pcd15/Econ-Sanctions/blob/main/README.md) led by Morad Bali at Duke University's Nicholas School of the Environment. The link provided offers further resources to tidy the data that this package writes.)
 ## Running the Program
 ### Comtrade
 * This part of the program utilizes the [comtradeapicall](https://pypi.org/project/comtradeapicall/) Python package to implement additional functionality.
 * To query export data from Comtrade, you can use the following methods:
-  * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reportner to all its partners)
+  * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reporter to all its partners)
   * ```get_total_exports```: writes csv file containing total-export (exports to world) data for all available reporters
+  * ```get_all_imports```: writes csv file containing import data for all available country pairs (i.e., imports to each reporter from all its partners)
+  * ```get_total_imports```: writes csv file containing total-import (imports from world) data for all available reporters
 * When you run these functions, you'll need to enter the criteria for your query. Both of these functions require two arguments, the first being the frequency ("A" for annual, "M" for monthly, or "B" for both) and the second being the year for which to gather data (e.g., 2021). Once the program's finished running, it'll output the names of the files that were just created.
 ### IMF
 * Functions with which to query data:
   * ```get_reporter_exports```: writes csv file containing value exports from reporter provided in console input to all its partners 
   * ```get_total_exports```: same as Comtrade's get_total_exports method
 * The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the arguments for get_reporter_exports (get_total_exports is the same across Comtrade and IMF): the first argument is the name of the reporting country for which you'd like to gather (e.g., "France"), followed by the frequency and year (in the same format as Comtrade's).
   * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
@@ -36,12 +38,15 @@
 from export_ease.comtrade import Comtrade     # importing the Comtrade class
 from export_ease.imf import IMF     # importing the IMF class
 
 # see above documentation
 Comtrade.get_all_exports("B", 2021)
 Comtrade.get_total_exports("B", 2021)
 
+Comtrade.get_all_imports("B", 2021)
+Comtrade.get_total_imports("B", 2021)
+
 IMF.get_reporter_exports("France", "B", 2021)
 IMF.get_total_exports("B", 2021)
 ```
 
 The above code can also be found in the ```test``` folder in the [GitHub repository](https://github.com/pcd15/export_pkg) for this package.
```

### Comparing `export_ease-0.0.5/README.md` & `export_ease-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # export_ease
 Built upon Python modules that call JSON RESTful API to gather macroeconomic data, this package offers a streamlined interface through which you can request and subsequently analyze vast amounts of macroeconomic data from sources including UN Comtrade and the International Monetary Fund (IMF). Below is a step-by-step guide detailing effective use of this program. (This package was built to supplement a [research project](https://github.com/pcd15/Econ-Sanctions/blob/main/README.md) led by Morad Bali at Duke University's Nicholas School of the Environment. The link provided offers further resources to tidy the data that this package writes.)
 ## Running the Program
 ### Comtrade
 * This part of the program utilizes the [comtradeapicall](https://pypi.org/project/comtradeapicall/) Python package to implement additional functionality.
 * To query export data from Comtrade, you can use the following methods:
-  * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reportner to all its partners)
+  * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reporter to all its partners)
   * ```get_total_exports```: writes csv file containing total-export (exports to world) data for all available reporters
+  * ```get_all_imports```: writes csv file containing import data for all available country pairs (i.e., imports to each reporter from all its partners)
+  * ```get_total_imports```: writes csv file containing total-import (imports from world) data for all available reporters
 * When you run these functions, you'll need to enter the criteria for your query. Both of these functions require two arguments, the first being the frequency ("A" for annual, "M" for monthly, or "B" for both) and the second being the year for which to gather data (e.g., 2021). Once the program's finished running, it'll output the names of the files that were just created.
 ### IMF
 * Functions with which to query data:
   * ```get_reporter_exports```: writes csv file containing value exports from reporter provided in console input to all its partners 
   * ```get_total_exports```: same as Comtrade's get_total_exports method
 * The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the arguments for get_reporter_exports (get_total_exports is the same across Comtrade and IMF): the first argument is the name of the reporting country for which you'd like to gather (e.g., "France"), followed by the frequency and year (in the same format as Comtrade's).
   * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
@@ -23,12 +25,15 @@
 from export_ease.comtrade import Comtrade     # importing the Comtrade class
 from export_ease.imf import IMF     # importing the IMF class
 
 # see above documentation
 Comtrade.get_all_exports("B", 2021)
 Comtrade.get_total_exports("B", 2021)
 
+Comtrade.get_all_imports("B", 2021)
+Comtrade.get_total_imports("B", 2021)
+
 IMF.get_reporter_exports("France", "B", 2021)
 IMF.get_total_exports("B", 2021)
 ```
 
 The above code can also be found in the ```test``` folder in the [GitHub repository](https://github.com/pcd15/export_pkg) for this package.
```

### Comparing `export_ease-0.0.5/pyproject.toml` & `export_ease-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "export_ease"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Paul Dilly", email="paul.dilly@duke.edu" },
 ]
 description = "A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `export_ease-0.0.5/src/export_ease/comtrade.py` & `export_ease-0.0.6/src/export_ease/comtrade.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,7 +48,47 @@
                                                 partner2Code=None,
                                                 customsCode=None, motCode=None, maxRecords=None, format_output='JSON',
                                                 aggregateBy=None, breakdownMode='classic', countOnly=None, includeDesc=True)
             df = pandas.DataFrame(mydf)
             file_name = f'comtrade_total_exports_{year}{freq}.csv'
             print(f'Writing {file_name}....')
             df.to_csv(os.path.join(Comtrade.directory, file_name))
+
+    # function to get all available country-pair import data
+    @classmethod
+    def get_all_imports(cls, freq, year):
+        if freq == "B":
+            Comtrade.get_all_imports("A", year)
+            Comtrade.get_all_imports("M", year)
+        else:
+            date = year
+            if freq == 'M':
+                date = f'{year}01,{year}02,{year}03,{year}04,{year}05,{year}06,{year}07,{year}08,{year}09,{year}10,{year}11,{year}12'
+            mydf = comtradeapicall.getFinalData(Comtrade.subscription_key, typeCode='C', freqCode=freq, clCode='HS', period=date,
+                                                reporterCode=None, cmdCode='TOTAL', flowCode='M', partnerCode=None,
+                                                partner2Code=None,
+                                                customsCode=None, motCode=None, maxRecords=None, format_output='JSON',
+                                                aggregateBy=None, breakdownMode='classic', countOnly=None, includeDesc=True)
+            df = pandas.DataFrame(mydf)
+            file_name = f'comtrade_all_imports_{year}{freq}.csv'
+            print(f'Writing {file_name}....')
+            df.to_csv(os.path.join(Comtrade.directory, file_name))
+
+    # function to get all available total-import data (i.e., partner is world)
+    @classmethod
+    def get_total_imports(cls, freq, year):
+        if freq == "B":
+            Comtrade.get_total_imports("A", year)
+            Comtrade.get_total_imports("M", year)
+        else:
+            date = year
+            if freq == 'M':
+                date = f'{year}01,{year}02,{year}03,{year}04,{year}05,{year}06,{year}07,{year}08,{year}09,{year}10,{year}11,{year}12'
+            mydf = comtradeapicall.getFinalData(Comtrade.subscription_key, typeCode='C', freqCode=freq, clCode='HS', period=date,
+                                                reporterCode=None, cmdCode='TOTAL', flowCode='M', partnerCode=0,
+                                                partner2Code=None,
+                                                customsCode=None, motCode=None, maxRecords=None, format_output='JSON',
+                                                aggregateBy=None, breakdownMode='classic', countOnly=None, includeDesc=True)
+            df = pandas.DataFrame(mydf)
+            file_name = f'comtrade_total_imports_{year}{freq}.csv'
+            print(f'Writing {file_name}....')
+            df.to_csv(os.path.join(Comtrade.directory, file_name))
```

### Comparing `export_ease-0.0.5/src/export_ease/imf.py` & `export_ease-0.0.6/src/export_ease/imf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class IMF:
    
     root = "http://dataservices.imf.org/REST/SDMX_JSON.svc/"
     cwd = os.getcwd()
     parent = os.path.dirname(cwd)
     directory = os.path.join(parent, "data")
-    json_path = os.path.join(cwd, "my.json")
+    json_path = os.path.join(directory, "my.json")
 
     # dictionary to store country names as keys and corresponding country codes as values
     country_dict = {} 
 
     def __init__(self):
         pass
```

### Comparing `export_ease-0.0.5/src/export_ease.egg-info/PKG-INFO` & `export_ease-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: export-ease
-Version: 0.0.5
+Name: export_ease
+Version: 0.0.6
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,16 +13,18 @@
 
 # export_ease
 Built upon Python modules that call JSON RESTful API to gather macroeconomic data, this package offers a streamlined interface through which you can request and subsequently analyze vast amounts of macroeconomic data from sources including UN Comtrade and the International Monetary Fund (IMF). Below is a step-by-step guide detailing effective use of this program. (This package was built to supplement a [research project](https://github.com/pcd15/Econ-Sanctions/blob/main/README.md) led by Morad Bali at Duke University's Nicholas School of the Environment. The link provided offers further resources to tidy the data that this package writes.)
 ## Running the Program
 ### Comtrade
 * This part of the program utilizes the [comtradeapicall](https://pypi.org/project/comtradeapicall/) Python package to implement additional functionality.
 * To query export data from Comtrade, you can use the following methods:
-  * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reportner to all its partners)
+  * ```get_all_exports```: writes csv file containing export data for all available country pairs (i.e., exports from each reporter to all its partners)
   * ```get_total_exports```: writes csv file containing total-export (exports to world) data for all available reporters
+  * ```get_all_imports```: writes csv file containing import data for all available country pairs (i.e., imports to each reporter from all its partners)
+  * ```get_total_imports```: writes csv file containing total-import (imports from world) data for all available reporters
 * When you run these functions, you'll need to enter the criteria for your query. Both of these functions require two arguments, the first being the frequency ("A" for annual, "M" for monthly, or "B" for both) and the second being the year for which to gather data (e.g., 2021). Once the program's finished running, it'll output the names of the files that were just created.
 ### IMF
 * Functions with which to query data:
   * ```get_reporter_exports```: writes csv file containing value exports from reporter provided in console input to all its partners 
   * ```get_total_exports```: same as Comtrade's get_total_exports method
 * The code to get IMF data is almost identical in structure to Comtrade's. The only difference is the arguments for get_reporter_exports (get_total_exports is the same across Comtrade and IMF): the first argument is the name of the reporting country for which you'd like to gather (e.g., "France"), followed by the frequency and year (in the same format as Comtrade's).
   * If you input an incorrect country name for ```get_reporter_exports```, you can check country_codes.csv to see valid country names (this file is written by the program when you run ```get_reporter_exports```).
@@ -36,12 +38,15 @@
 from export_ease.comtrade import Comtrade     # importing the Comtrade class
 from export_ease.imf import IMF     # importing the IMF class
 
 # see above documentation
 Comtrade.get_all_exports("B", 2021)
 Comtrade.get_total_exports("B", 2021)
 
+Comtrade.get_all_imports("B", 2021)
+Comtrade.get_total_imports("B", 2021)
+
 IMF.get_reporter_exports("France", "B", 2021)
 IMF.get_total_exports("B", 2021)
 ```
 
 The above code can also be found in the ```test``` folder in the [GitHub repository](https://github.com/pcd15/export_pkg) for this package.
```

