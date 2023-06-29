# Comparing `tmp/pyees-1.3.3.tar.gz` & `tmp/pyees-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.3.tar", last modified: Thu Jun 29 05:52:47 2023, max compression
+gzip compressed data, was "pyees-1.3.4.tar", last modified: Thu Jun 29 06:36:38 2023, max compression
```

## Comparing `pyees-1.3.3.tar` & `pyees-1.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 05:52:47.784478 pyees-1.3.3/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-06-29 05:52:47.800104 pyees-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 05:52:47.533400 pyees-1.3.3/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.3/pyees/__init__.py
--rw-rw-rw-   0        0        0    12847 2023-06-28 06:38:17.000000 pyees-1.3.3/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.3.3/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.3.3/pyees/prop.py
--rw-rw-rw-   0        0        0    18070 2023-06-29 05:52:25.000000 pyees-1.3.3/pyees/sheet.py
--rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.3/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.3/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-06-28 06:38:39.000000 pyees-1.3.3/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.3.3/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.3/pyees/testPyees.py
--rw-rw-rw-   0        0        0    16959 2023-06-28 06:46:30.000000 pyees-1.3.3/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.3/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.3/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.3/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.3/pyees/unit.py
--rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.3/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-29 05:52:47.737601 pyees-1.3.3/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-06-29 05:52:45.000000 pyees-1.3.3/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-29 05:52:46.000000 pyees-1.3.3/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 05:52:45.000000 pyees-1.3.3/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-29 05:52:45.000000 pyees-1.3.3/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 05:52:45.000000 pyees-1.3.3/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 05:52:47.846981 pyees-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-06-29 05:52:38.000000 pyees-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:36:38.226601 pyees-1.3.4/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-06-29 06:36:38.242227 pyees-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 06:36:37.960965 pyees-1.3.4/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.4/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12847 2023-06-28 06:38:17.000000 pyees-1.3.4/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.3.4/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.3.4/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.4/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.4/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.4/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-06-28 06:38:39.000000 pyees-1.3.4/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.3.4/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.4/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.4/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.4/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.4/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.4/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.4/pyees/unit.py
+-rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.4/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:36:38.179724 pyees-1.3.4/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-29 06:36:38.289104 pyees-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-06-29 06:36:29.000000 pyees-1.3.4/setup.py
```

### Comparing `pyees-1.3.3/LICENSE.txt` & `pyees-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/PKG-INFO` & `pyees-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.3
+Version: 1.3.4
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.3/README.md` & `pyees-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/fit.py` & `pyees-1.3.4/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/profilePyees.py` & `pyees-1.3.4/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/prop.py` & `pyees-1.3.4/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/sheet.py` & `pyees-1.3.4/pyees/sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,24 +116,28 @@
         extension = os.path.splitext(xlFile)[1]
         supportedExtensions = ['.xls', '.xlsx']
         if extension not in supportedExtensions:
             raise ValueError(f'The file extension is not supported. The supported extension are {supportedExtensions}')
 
         # parse functions for the specific extension and get all sheets
         if extension == '.xls':
-            self.wb = xlrd.open_workbook(xlFile)
+            self.wb = xlrd.open_workbook(xlFile, formatting_info=True)
             
             self.sheets = self.wb.sheets()
             if not sheets is None:
                 if not isinstance(sheets, list):
                     sheets = [sheets]
                 self.sheets = [elem for i,elem in enumerate(self.sheets) if i in sheets]
 
             def readCell(sheet, row, col):
-                return sheet.cell(row, col).value
+                cell = sheet.cell(row,col)
+                if cell.ctype == 2:
+                    return cell.value
+                else:
+                    return np.nan
 
             def readRow(sheet, row):
                 return [elem.value for elem in sheet.row(row)]
 
             def readCol(sheet, col):
                 return [elem.value for elem in sheet.col(col)]
 
@@ -142,15 +146,20 @@
             self.sheets = [self.wb[elem] for elem in self.wb.sheetnames]
             if not sheets is None:
                 if not isinstance(sheets, list):
                     sheets = [sheets]
                 self.sheets = [elem for i,elem in enumerate(self.sheets) if i in sheets]
                 
             def readCell(sheet, row, col):
-                return sheet.cell(row + 1, col + 1).value
+                cell = sheet.cell(row+1,col+1)
+                try:
+                    float(cell.value)
+                    return cell.value
+                except ValueError:
+                    return np.nan
 
             def readRow(sheet, row):
                 return [elem.value for elem in list(sheet.iter_rows())[row]]
 
             def readCol(sheet, col):
                 return [elem.value for elem in list(sheet.iter_cols())[col]]
 
@@ -446,8 +455,10 @@
                 variables.append(item)
         
         return iter(variables)
     
     def pop(self, index = -1):
         for key, item in self.__dict__.items():
             if isinstance(item, scalarVariable):
-                item.pop(index)
+                item.pop(index)
+
+
```

### Comparing `pyees-1.3.3/pyees/solve.py` & `pyees-1.3.4/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/stackOverflowODR.py` & `pyees-1.3.4/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/testFit.py` & `pyees-1.3.4/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/testProp.py` & `pyees-1.3.4/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/testPyees.py` & `pyees-1.3.4/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/testSheet.py` & `pyees-1.3.4/pyees/testSheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,9 +289,30 @@
         np.testing.assert_array_equal(dat.A.value, [1, 2, 5])
         self.assertEqual(str(dat.A.unit), 'L/min')
         np.testing.assert_array_equal(dat.A.uncert, [0, 0, 0])
         np.testing.assert_array_equal(dat.B.value, [5, 6, 9])
         self.assertEqual(str(dat.B.unit), 'mA')
         np.testing.assert_array_equal(dat.B.uncert, [0, 0, 0])
         
+    def testReadNAN(self):
+        dat = sheetsFromFile('testData/data9.xls', 'A-B')
+        
+        np.testing.assert_equal(dat.A.value, [np.nan, 1])
+        self.assertEqual(dat.A.unit, '1')
+        np.testing.assert_equal(dat.A.uncert, [0, 0])
+        
+        np.testing.assert_equal(dat.B.value, [np.nan, 2])
+        self.assertEqual(dat.B.unit, '1')
+        np.testing.assert_equal(dat.B.uncert, [0, 0])
+        
+        dat = sheetsFromFile('testData/data10.xlsx', 'A-B')
+        np.testing.assert_equal(dat.A.value, [np.nan])
+        self.assertEqual(dat.A.unit, '1')
+        np.testing.assert_equal(dat.A.uncert, [0])
+        
+        np.testing.assert_equal(dat.B.value, [np.nan])
+        self.assertEqual(dat.B.unit, '1')
+        np.testing.assert_equal(dat.B.uncert, [0])
+        
+        
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyees-1.3.3/pyees/testSolve.py` & `pyees-1.3.4/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/testUnit.py` & `pyees-1.3.4/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/testVariable.py` & `pyees-1.3.4/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/unit.py` & `pyees-1.3.4/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees/variable.py` & `pyees-1.3.4/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.3/pyees.egg-info/PKG-INFO` & `pyees-1.3.4/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.3
+Version: 1.3.4
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.3/setup.py` & `pyees-1.3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.3',
+    version='1.3.4',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

