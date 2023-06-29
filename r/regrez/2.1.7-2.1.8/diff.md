# Comparing `tmp/regrez-2.1.7.tar.gz` & `tmp/regrez-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-2.1.7.tar", last modified: Thu Jun 29 13:16:55 2023, max compression
+gzip compressed data, was "regrez-2.1.8.tar", last modified: Thu Jun 29 13:21:06 2023, max compression
```

## Comparing `regrez-2.1.7.tar` & `regrez-2.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:16:55.387340 regrez-2.1.7/
--rw-rw-rw-   0        0        0     2106 2023-06-29 13:16:55.356347 regrez-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1611 2023-06-29 13:16:44.000000 regrez-2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 13:16:55.162617 regrez-2.1.7/regrez/
--rw-rw-rw-   0        0        0       28 2023-06-29 12:41:43.000000 regrez-2.1.7/regrez/__init__.py
--rw-rw-rw-   0        0        0     4627 2023-06-29 13:13:54.000000 regrez-2.1.7/regrez/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:16:55.344337 regrez-2.1.7/regrez.egg-info/
--rw-rw-rw-   0        0        0     2106 2023-06-29 13:16:54.000000 regrez-2.1.7/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-29 13:16:54.000000 regrez-2.1.7/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:16:54.000000 regrez-2.1.7/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 13:16:54.000000 regrez-2.1.7/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 13:16:54.000000 regrez-2.1.7/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:16:55.388348 regrez-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-29 13:11:39.000000 regrez-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:21:06.551483 regrez-2.1.8/
+-rw-rw-rw-   0        0        0     2106 2023-06-29 13:21:06.546494 regrez-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1611 2023-06-29 13:16:44.000000 regrez-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 13:21:06.426815 regrez-2.1.8/regrez/
+-rw-rw-rw-   0        0        0       28 2023-06-29 12:41:43.000000 regrez-2.1.8/regrez/__init__.py
+-rw-rw-rw-   0        0        0     4742 2023-06-29 13:20:47.000000 regrez-2.1.8/regrez/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:21:06.541232 regrez-2.1.8/regrez.egg-info/
+-rw-rw-rw-   0        0        0     2106 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 13:21:06.000000 regrez-2.1.8/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:21:06.552495 regrez-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-29 13:20:59.000000 regrez-2.1.8/setup.py
```

### Comparing `regrez-2.1.7/PKG-INFO` & `regrez-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 2.1.7
+Version: 2.1.8
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
```

### Comparing `regrez-2.1.7/README.md` & `regrez-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `regrez-2.1.7/regrez/main.py` & `regrez-2.1.8/regrez/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,20 +52,21 @@
             print("R2-score: %.2f" % r2_score(test_y , predicted_y) )
     def Visualize(self):
         plt.scatter(self.data[self.x_label], self.data[self.y_label], color='blue')
         plt.plot(self.x, self.coef[0][0]*self.x + self.intercept[0], '-r')
         plt.xlabel(self.x_label)
         plt.ylabel(self.y_label)
         plt.show()
+#---------------------------------------------------------------------------------------------------------------#
 class Multiple:
     def __init__(self, csv_path, labels_x, labels_y): #Multiple("path", ["a", "b"], "c")
         self.csv = csv_path
         self.x_labels = labels_x
         self.y_labels = labels_y
-        self.labels = labels_x + labels_x
+        self.labels = labels_x + labels_y
         self.file = pd.read_csv(self.csv)
         self.data = self.file[self.labels]
         self.coef = 0
         self.intercept = 0
         self.x = np.asanyarray(self.data[self.x_labels])
         self.y = np.asanyarray(self.data[self.y_labels])
         self.reg = linear_model.LinearRegression()
```

### Comparing `regrez-2.1.7/regrez.egg-info/PKG-INFO` & `regrez-2.1.8/regrez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 2.1.7
+Version: 2.1.8
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
```

### Comparing `regrez-2.1.7/setup.py` & `regrez-2.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.1.7' 
+VERSION = '2.1.8' 
 DESCRIPTION = 'Easiest way to implement linear regression.'
 
 with open('README.md') as f:
     long = f.read()
 setup(
         name="regrez", 
         version=VERSION,
```

