# Comparing `tmp/b21scripts-1.1.0.tar.gz` & `tmp/b21scripts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nathan/Documents/PYTHON/b21scripts/dist/.tmp-2sxd7dxg/b21scripts-1.1.0.tar", last modified: Mon Jun 12 10:18:26 2023, max compression
+gzip compressed data, was "/Users/nathan/Documents/PYTHON/b21scripts/dist/.tmp-1tfdo2xs/b21scripts-1.1.1.tar", last modified: Thu Jun 29 08:33:27 2023, max compression
```

## Comparing `b21scripts-1.1.0.tar` & `b21scripts-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/
--rw-r--r--   0 nathan     (503) staff       (20)     1084 2022-09-09 14:05:16.000000 b21scripts-1.1.0/LICENCE
--rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-12 10:18:26.000000 b21scripts-1.1.0/PKG-INFO
--rw-r--r--   0 nathan     (503) staff       (20)     1903 2022-09-19 18:19:39.000000 b21scripts-1.1.0/README.md
--rw-r--r--   0 nathan     (503) staff       (20)       84 2022-09-09 14:05:16.000000 b21scripts-1.1.0/pyproject.toml
--rw-r--r--   0 nathan     (503) staff       (20)      747 2023-06-12 10:18:26.000000 b21scripts-1.1.0/setup.cfg
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts/
--rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/__init__.py
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts/readwrite/
--rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/readwrite/__init__.py
--rw-r--r--   0 nathan     (503) staff       (20)    12770 2023-06-12 10:07:41.000000 b21scripts-1.1.0/src/b21scripts/readwrite/dat.py
--rw-r--r--   0 nathan     (503) staff       (20)      395 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/readwrite/interface.py
--rw-r--r--   0 nathan     (503) staff       (20)    13786 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/readwrite/pdb.py
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts/saxs/
--rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-19 18:10:28.000000 b21scripts-1.1.0/src/b21scripts/saxs/__init__.py
--rwxr-xr-x   0 nathan     (503) staff       (20)    11290 2022-09-19 16:24:23.000000 b21scripts-1.1.0/src/b21scripts/saxs/saxs_calc.py
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/
--rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/PKG-INFO
--rw-r--r--   0 nathan     (503) staff       (20)      462 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/SOURCES.txt
--rw-r--r--   0 nathan     (503) staff       (20)        1 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/dependency_links.txt
--rw-r--r--   0 nathan     (503) staff       (20)       17 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/requires.txt
--rw-r--r--   0 nathan     (503) staff       (20)       11 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/top_level.txt
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-29 08:33:27.000000 b21scripts-1.1.1/
+-rw-r--r--   0 nathan     (503) staff       (20)     1084 2022-09-09 14:05:16.000000 b21scripts-1.1.1/LICENCE
+-rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-29 08:33:27.000000 b21scripts-1.1.1/PKG-INFO
+-rw-r--r--   0 nathan     (503) staff       (20)     1903 2022-09-19 18:19:39.000000 b21scripts-1.1.1/README.md
+-rw-r--r--   0 nathan     (503) staff       (20)       84 2022-09-09 14:05:16.000000 b21scripts-1.1.1/pyproject.toml
+-rw-r--r--   0 nathan     (503) staff       (20)      747 2023-06-29 08:33:27.000000 b21scripts-1.1.1/setup.cfg
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.1.1/src/b21scripts/__init__.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts/readwrite/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.1.1/src/b21scripts/readwrite/__init__.py
+-rw-r--r--   0 nathan     (503) staff       (20)    16291 2023-06-29 08:23:32.000000 b21scripts-1.1.1/src/b21scripts/readwrite/dat.py
+-rw-r--r--   0 nathan     (503) staff       (20)      395 2022-09-09 14:05:16.000000 b21scripts-1.1.1/src/b21scripts/readwrite/interface.py
+-rw-r--r--   0 nathan     (503) staff       (20)    13786 2022-09-09 14:05:16.000000 b21scripts-1.1.1/src/b21scripts/readwrite/pdb.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts/saxs/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-19 18:10:28.000000 b21scripts-1.1.1/src/b21scripts/saxs/__init__.py
+-rwxr-xr-x   0 nathan     (503) staff       (20)    11290 2022-09-19 16:24:23.000000 b21scripts-1.1.1/src/b21scripts/saxs/saxs_calc.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts.egg-info/
+-rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts.egg-info/PKG-INFO
+-rw-r--r--   0 nathan     (503) staff       (20)      462 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan     (503) staff       (20)        1 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan     (503) staff       (20)       17 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts.egg-info/requires.txt
+-rw-r--r--   0 nathan     (503) staff       (20)       11 2023-06-29 08:33:27.000000 b21scripts-1.1.1/src/b21scripts.egg-info/top_level.txt
```

### Comparing `b21scripts-1.1.0/LICENCE` & `b21scripts-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `b21scripts-1.1.0/PKG-INFO` & `b21scripts-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b21scripts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Libraries for SAXS data manipulation and analysis
 Home-page: https://github.com/nathancowieson/b21scripts.git
 Author: Nathan Cowieson
 Author-email: nathan.cowieson@diamond.ac.uk
 Project-URL: Bug Tracker, https://github.com/pypa/b21scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `b21scripts-1.1.0/README.md` & `b21scripts-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `b21scripts-1.1.0/setup.cfg` & `b21scripts-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = b21scripts
-version = 1.1.0
+version = 1.1.1
 author = Nathan Cowieson
 author_email = nathan.cowieson@diamond.ac.uk
 description = Libraries for SAXS data manipulation and analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nathancowieson/b21scripts.git
 project_urls =
```

### Comparing `b21scripts-1.1.0/src/b21scripts/readwrite/dat.py` & `b21scripts-1.1.1/src/b21scripts/readwrite/dat.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         self.type = 'dat'
 
         
 
         self.hashdata = pd.DataFrame.from_dict( {'Q': [], 'I': [], 'E': []}, orient='columns').set_index('Q')
         self.header=''
         self.footer=''
+        self.outliers = []
 
         #The units dictionary allows on the fly output in different unit schemes
         self.units={}
         self.add_unit('linear', lambda x: x, r'Q ($\AA^{-1}$)')
         self.add_unit('^2', lambda x: np.power(x,2), r'Q ($\AA^{-1}$)$^{2}$')
         self.add_unit('^3', lambda x: np.power(x,3), r'Q ($\AA^{-1}$)$^{3}$')
         self.add_unit('^4', lambda x: np.power(x,4), r'Q ($\AA^{-1}$)$^{4}$')
@@ -130,14 +131,15 @@
             self.footer=''.join(datdata[data_end+1:])
 
         #Parse the data
         if data_end > data_start:
             self.hashdata = pd.read_table(self.datfile,
                                           skiprows=data_start,
                                           engine='python',
+                                          delim_whitespace=True,
                                           skipfooter=len(datdata)-data_end,
                                           names=['Q','I','E'],
                                           index_col=0
             )
         self.logger.info(f'Parsed dat file with {self.hashdata.index.size} points.')
                 
             
@@ -147,15 +149,15 @@
         if q in self.hashdata.index:
             self.logger.debug(f'Q value {q} was found in the dat file')
             return tuple(self.hashdata.xs(q))
         else:
             self.logger.debug(f'Q value {q} was not found in the dat file')
             return False
 
-    def return_data_column(self, column='I', qmin=None, qmax=None, unit=None):
+    def return_data_column(self, column='I', qmin=None, qmax=None, unit=None, drop_outliers=True):
         '''Given column "Q", "I" or "E" will return data as a numpy array
         
         The optional argument unit refers to the entries in the units dictionary
         that stores lambda functions that allows the specified data column to be
         output with altered units i.e choosing column='I' and unit='^2' will output
         an array containing I^2 rather than I. The exception is for units that
         refer to more than one data column i.e. 'q^2*I(q)' that might be used for
@@ -183,40 +185,103 @@
         if unit:
             if unit in self.units.keys():
                 if len(signature(self.units[unit][0]).parameters) > 2:
                     self.logger.error('Unit functions should not contain more than 2 arguments')
                     return False
                 elif len(signature(self.units[unit][0]).parameters) == 2:
                     self.logger.info('The requested unit function has 2 arguments, will assume these refer to Q,I')
-                    return self.units[unit][0](self.hashdata.loc[qmin:qmax].index.values,self.hashdata.loc[qmin:qmax]['I'].values)
+                    if drop_outliers:
+                        return self.units[unit][0](self.hashdata.drop(self.outliers).loc[qmin:qmax].index.values,self.hashdata.loc[qmin:qmax]['I'].values)
+                    else:
+                        return self.units[unit][0](self.hashdata.loc[qmin:qmax].index.values,self.hashdata.loc[qmin:qmax]['I'].values)
                 elif str(column).upper() in ['I', 'E']:
-                    return self.units[unit][0](self.hashdata.loc[qmin:qmax][column].values)
+                    if drop_outliers:
+                        return self.units[unit][0](self.hashdata.drop(self.outliers).loc[qmin:qmax][column].values)
+                    else:
+                        return self.units[unit][0](self.hashdata.loc[qmin:qmax][column].values)
                 elif str(column).upper() == 'Q':
-                    return self.units[unit][0](self.hashdata.loc[qmin:qmax].index.values)
+                    if drop_outliers:
+                        return self.units[unit][0](self.hashdata.drop(self.outliers).loc[qmin:qmax].index.values)
+                    else:
+                        return self.units[unit][0](self.hashdata.loc[qmin:qmax].index.values)
                 else:
                     self.logger.error('ReturnDataColumn function requires you specify either Q, I or E')
                     return False
             else:
                 self.logger.error(f'Unit {unit} is not in the units definition')
                 return False
         else:
             if str(column).upper() in ['I', 'E']:
-                return self.hashdata.loc[qmin:qmax][column].values
+                if drop_outliers:
+                    return self.hashdata.drop(self.outliers).loc[qmin:qmax][column].values
+                else:
+                    return self.hashdata.loc[qmin:qmax][column].values
             elif str(column).upper() == 'Q':
-                return self.hashdata.loc[qmin:qmax].index.values
+                if drop_outliers:
+                    return self.hashdata.drop(self.outliers).loc[qmin:qmax].index.values
+                else:
+                    return self.hashdata.loc[qmin:qmax].index.values
             else:
                 self.logger.error('ReturnDataColumn function requires you specify either Q, I or E')
                 return False
-        
+
+    def find_outliers(self, n_stds=3, window_size=11):
+        ''' Finds outliers in dat files i.e. hot pixels etc
+
+        Applies a rolling window to the dat file data and identifies outliers
+        as being n_stds (default is 3) x the median error taken from the error
+        column above the median intensity value. Returns the outliers as an
+        array of Q values
+        '''
+        self.logger.debug('The find_outliers method was called')
+        if not isinstance(n_stds, (float, int)):
+            self.logger.error('the n_stds option in the find_outliers function needs to be a number')
+            return False
+
+        if not isinstance(window_size, (int)):
+            self.logger.error('the window_size option in the find_outliers function should be an integer')
+            return False
+
+        if (window_size % 2) == 0:
+            self.logger.warning('the window_size option in the find_outliers function should be odd, will add 1')
+            window_size+=1
+
+        r = self.hashdata.rolling(window_size, center=True)
+        outliers = (self.hashdata['I'] > ( r.I.median() + (3 * r.E.median()))).to_frame(name='outlier').query('outlier').index.to_list()
+        self.logger.info(f'Found {len(outliers)} outliers')
+        return outliers
+
+    def set_outliers(self, n_stds=3, window_size=11):
+        ''' Runs the find_outliers function and sets result to self.outliers'''
+        self.logger.debug('The set_outliers method was called')
+        if not isinstance(n_stds, (float, int)):
+            self.logger.error('the n_stds option in the find_outliers function needs to be a number')
+            return False
+
+        if not isinstance(window_size, (int)):
+            self.logger.error('the window_size option in the find_outliers function should be an integer')
+            return False
+
+        if (window_size % 2) == 0:
+            self.logger.warning('the window_size option in the find_outliers function should be odd, will add 1')
+            window_size+=1
+
+        self.outliers = self.find_outliers(n_stds, window_size)
+
+    def clear_outliers(self):
+        '''Clears the outliers list'''
+        self.logger.debug('The clear_outliers method was called')
+        self.outliers = []
+            
     def return_file(self):
         self.logger.debug('The return_file method was called')        
         self.logger.info('Writing out a formatted DAT file')
         string_list = [self.header]
         string_list.append("%-15s %-13s %-13s\n" % ("Q(A-1)","I(au)","Error"))
-        for q in self.return_data_column('Q'):
+        for q in self.return_data_column('Q', drop_outliers=True):
             if q > 0:
                 i,e = self.return_ie_data(q)
                 string_list.append('{:<15.7E} {:<13.6E} {:<13.6E}\n'.format(q,i,e))
         string_list.append(self.footer)
         return ''.join(string_list)
 
 
@@ -272,17 +337,21 @@
         if log_x:
             plt.xscale('log')
         if title:
             ax.set_title(f'{title}', fontsize=fontsize)
         plt.rc('lines', linewidth=linewidth)
         ax.set_ylabel(y_label, fontsize=fontsize)
         ax.set_xlabel(x_label, fontsize=fontsize)
-        q=self.return_data_column(column='Q', qmin=qrange_min, qmax=qrange_max, unit=x_unit).tolist()
-        i=self.return_data_column(column='I', qmin=qrange_min, qmax=qrange_max, unit=y_unit).tolist()
+        q=self.return_data_column(column='Q', qmin=qrange_min, qmax=qrange_max, unit=x_unit, drop_outliers=False).tolist()
+        i=self.return_data_column(column='I', qmin=qrange_min, qmax=qrange_max, unit=y_unit, drop_outliers=False).tolist()
         plt.plot(q,i)
+        if len(self.outliers) > 0:
+            q_outlier = self.hashdata.loc[self.outliers].index.to_list()
+            i_outlier = self.hashdata.loc[self.outliers].I.to_list()
+            plt.plot(q_outlier, i_outlier, 'ro')
         y_bottom,y_top = plt.ylim()
         self.logger.debug(f'autoscale limits are {y_top}x{y_bottom}')
         if yrange_min == None:
             yrange_min=y_bottom
         if yrange_max == None:
             yrange_max=y_top
         plt.ylim(bottom=yrange_min,top=yrange_max)
```

### Comparing `b21scripts-1.1.0/src/b21scripts/readwrite/pdb.py` & `b21scripts-1.1.1/src/b21scripts/readwrite/pdb.py`

 * *Files identical despite different names*

### Comparing `b21scripts-1.1.0/src/b21scripts/saxs/saxs_calc.py` & `b21scripts-1.1.1/src/b21scripts/saxs/saxs_calc.py`

 * *Files identical despite different names*

### Comparing `b21scripts-1.1.0/src/b21scripts.egg-info/PKG-INFO` & `b21scripts-1.1.1/src/b21scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b21scripts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Libraries for SAXS data manipulation and analysis
 Home-page: https://github.com/nathancowieson/b21scripts.git
 Author: Nathan Cowieson
 Author-email: nathan.cowieson@diamond.ac.uk
 Project-URL: Bug Tracker, https://github.com/pypa/b21scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

