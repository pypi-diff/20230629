# Comparing `tmp/Pegamoid-2.7.tar.gz` & `tmp/Pegamoid-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pegamoid-2.7.tar", last modified: Thu Feb  2 12:58:57 2023, max compression
+gzip compressed data, was "Pegamoid-2.8.tar", last modified: Thu Jun 29 12:51:49 2023, max compression
```

## Comparing `Pegamoid-2.7.tar` & `Pegamoid-2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-02-02 12:58:57.232803 Pegamoid-2.7/
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)    35059 2019-10-28 09:04:52.000000 Pegamoid-2.7/LICENSE
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8547 2023-02-02 12:58:57.232803 Pegamoid-2.7/PKG-INFO
-drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-02-02 12:58:57.232803 Pegamoid-2.7/Pegamoid.egg-info/
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8547 2023-02-02 12:58:57.000000 Pegamoid-2.7/Pegamoid.egg-info/PKG-INFO
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)      197 2023-02-02 12:58:57.000000 Pegamoid-2.7/Pegamoid.egg-info/SOURCES.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-02-02 12:58:57.000000 Pegamoid-2.7/Pegamoid.egg-info/dependency_links.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       76 2023-02-02 12:58:57.000000 Pegamoid-2.7/Pegamoid.egg-info/requires.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-02-02 12:58:57.000000 Pegamoid-2.7/Pegamoid.egg-info/top_level.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8423 2020-09-15 10:56:55.000000 Pegamoid-2.7/README.md
--rwxrwxr-x   0 ignacio   (1001) ignacio   (1001)   299872 2023-02-02 12:49:06.000000 Pegamoid-2.7/pegamoid.py
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       38 2023-02-02 12:58:57.232803 Pegamoid-2.7/setup.cfg
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     1093 2023-02-02 12:48:52.000000 Pegamoid-2.7/setup.py
+drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-06-29 12:51:49.536503 Pegamoid-2.8/
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)    35059 2019-10-28 09:04:52.000000 Pegamoid-2.8/LICENSE
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8547 2023-06-29 12:51:49.532503 Pegamoid-2.8/PKG-INFO
+drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-06-29 12:51:49.532503 Pegamoid-2.8/Pegamoid.egg-info/
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8547 2023-06-29 12:51:49.000000 Pegamoid-2.8/Pegamoid.egg-info/PKG-INFO
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)      197 2023-06-29 12:51:49.000000 Pegamoid-2.8/Pegamoid.egg-info/SOURCES.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-06-29 12:51:49.000000 Pegamoid-2.8/Pegamoid.egg-info/dependency_links.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       76 2023-06-29 12:51:49.000000 Pegamoid-2.8/Pegamoid.egg-info/requires.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-06-29 12:51:49.000000 Pegamoid-2.8/Pegamoid.egg-info/top_level.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8423 2020-09-15 10:56:55.000000 Pegamoid-2.8/README.md
+-rwxrwxr-x   0 ignacio   (1001) ignacio   (1001)   300231 2023-06-29 12:48:14.000000 Pegamoid-2.8/pegamoid.py
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       38 2023-06-29 12:51:49.536503 Pegamoid-2.8/setup.cfg
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     1093 2023-06-26 10:41:31.000000 Pegamoid-2.8/setup.py
```

### Comparing `Pegamoid-2.7/LICENSE` & `Pegamoid-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Pegamoid-2.7/PKG-INFO` & `Pegamoid-2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pegamoid
-Version: 2.7
+Version: 2.8
 Summary: Orbital viewer for OpenMolcas
 Home-page: https://gitlab.com/Jellby/Pegamoid
 Author: Ignacio Fdez. Galván
 Author-email: jellby@yahoo.com
 License: GPL v3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Pegamoid-2.7/Pegamoid.egg-info/PKG-INFO` & `Pegamoid-2.8/Pegamoid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pegamoid
-Version: 2.7
+Version: 2.8
 Summary: Orbital viewer for OpenMolcas
 Home-page: https://gitlab.com/Jellby/Pegamoid
 Author: Ignacio Fdez. Galván
 Author-email: jellby@yahoo.com
 License: GPL v3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Pegamoid-2.7/README.md` & `Pegamoid-2.8/README.md`

 * *Files identical despite different names*

### Comparing `Pegamoid-2.7/pegamoid.py` & `Pegamoid-2.8/pegamoid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import division, absolute_import, print_function
 from builtins import bytes, dict, int, range, super
 
 __name__ = 'Pegamoid'
 __author__ = u'Ignacio Fdez. Galván'
 __copyright__ = u'Copyright © 2018–2020,2022–2023'
 __license__ = 'GPL v3.0'
-__version__ = '2.7'
+__version__ = '2.8'
 
 import sys
 try:
   from qtpy.QtCore import Qt, QObject, QThread, QEvent, QSettings
   from qtpy.QtWidgets import *
   from qtpy.QtGui import QPixmap, QIcon, QKeySequence, QColor, QPalette
   import qtpy
@@ -1200,139 +1200,144 @@
       while ((not line.startswith('#INFO')) and (line != '')):
         line = f.readline()
       sections['INFO'] = True
       line = f.readline()
       uhf, nsym, _ = (int(i) for i in f.readline().split())
       N_bas = np.array([int(i) for i in f.readline().split()])
       nMO = np.array([int(i) for i in f.readline().split()])
+      irrep = self.irrep
+      desymmetrized = False
       if (not np.array_equal(N_bas, self.N_bas)):
-        return 'Incompatible InpOrb data'
-      # Decide whether or not beta orbitals will be read
+        # Allow files with desymmetrized orbitals (e.g. NTOrb.SO)
+        if ((len(N_bas) == 1) and (N_bas[0] == sum(self.N_bas))):
+          desymmetrized = True
+          irrep = ['?']
+        else:
+          return 'Incompatible InpOrb data'
+      # Clear orbitals and decide whether or not beta orbitals will be read
+      self.MO = [{} for i in range(sum(nMO))]
       if (uhf):
         self.MO_b = deepcopy(self.MO)
       else:
         self.MO_a = []
         self.MO_b = []
-      ii = [sum(self.N_bas[:i]) for i in range(len(self.N_bas))]
+      ii = [sum(N_bas[:i]) for i in range(len(N_bas))]
+      jj = [sum(nMO[:i]) for i in range(len(nMO))]
       # Read until EOF
       while (line != ''):
         # Find next section
         while ((not line.startswith('#')) and (line != '')):
           line = f.readline()
         # Read orbital coefficients, only the non-zero (by symmetry)
         # coefficients are written in the file
         if (line.startswith('#ORB')):
           sections['ORB'] = True
           line = '\n'
-          j = 0
-          for i,b,s in zip(ii, self.N_bas, self.irrep):
-            for orb in self.MO[i:i+b]:
+          for i,j,b,n,s in zip(ii, jj, N_bas, nMO, irrep):
+            for orb in self.MO[j:j+n]:
               orb['sym'] = s
-              orb['coeff'] = np.zeros(sum(self.N_bas))
+              orb['coeff'] = np.zeros(sum(N_bas))
               cff = []
               f.readline()
               while (len(cff) < b):
                 line = f.readline()
                 if (re.search(r'\.[^ ]*\.', line)):
                   cff.extend(fortrannums.findall(line))
                 else:
                   cff.extend(line.split())
               orb['coeff'][i:i+b] = [fortran_float(c) for c in cff]
-              j += b
         elif (line.startswith('#UORB')):
           sections['UORB'] = True
           line = '\n'
           if (uhf):
-            j = 0
-            for i,b,s in zip(ii, self.N_bas, self.irrep):
-              for orb in self.MO_b[i:i+b]:
+            for i,j,b,n,s in zip(ii, jj, N_bas, nMO, irrep):
+              for orb in self.MO_b[j:j+b]:
                 orb['sym'] = s
-                orb['coeff'] = np.zeros(sum(self.N_bas))
+                orb['coeff'] = np.zeros(sum(N_bas))
                 cff = []
                 f.readline()
                 while (len(cff) < b):
                   line = f.readline()
                   if (re.search(r'\.[^ ]*\.', line)):
                     cff.extend(fortrannums.findall(line))
                   else:
                     cff.extend(line.split())
                 orb['coeff'][i:i+b] = [fortran_float(c) for c in cff]
-                j += b
         # Read the occupations
         elif (line.startswith('#OCC')):
           sections['OCC'] = True
           line = '\n'
           f.readline()
           occ = []
-          for i,b in zip(ii, self.N_bas):
-            while (len(occ) < i+b):
+          for i,b,n in zip(jj, N_bas, nMO):
+            while (len(occ) < i+n):
               line = f.readline()
               if (re.search(r'\.[^ ]*\.', line)):
                 occ.extend(fortrannums.findall(line))
               else:
                 occ.extend(line.split())
         elif (line.startswith('#UOCC')):
           sections['UOCC'] = True
           line = '\n'
           if (uhf):
             f.readline()
-            for i,b in zip(ii, self.N_bas):
-              while (len(occ) < len(self.MO)+i+b):
+            for i,b,n in zip(jj, N_bas, nMO):
+              while (len(occ) < len(self.MO)+i+n):
                 line = f.readline()
                 if (re.search(r'\.[^ ]*\.', line)):
                   occ.extend(fortrannums.findall(line))
                 else:
                   occ.extend(line.split())
         # Read the energies
         elif (line.startswith('#ONE')):
           sections['ONE'] = True
           line = '\n'
           f.readline()
           ene = []
-          for i,b in zip(ii, self.N_bas):
-            while (len(ene) < i+b):
+          for i,b,n in zip(jj, N_bas, nMO):
+            while (len(ene) < i+n):
               line = f.readline()
               if (re.search(r'\.[^ ]*\.', line)):
                 ene.extend(fortrannums.findall(line))
               else:
                 ene.extend(line.split())
         elif (line.startswith('#UONE')):
           sections['UONE'] = True
           line = '\n'
           if (uhf):
             f.readline()
-            for i,b in zip(ii, self.N_bas):
-              while (len(ene) < len(self.MO)+i+b):
+            for i,b,n in zip(jj, N_bas, nMO):
+              while (len(ene) < len(self.MO)+i+n):
                 line = f.readline()
                 if (re.search(r'\.[^ ]*\.', line)):
                   ene.extend(fortrannums.findall(line))
                 else:
                   ene.extend(line.split())
         # Read the orbital types (same for alpha and beta)
         elif (line.startswith('#INDEX')):
           sections['INDEX'] = True
           line = '\n'
           idx = ''
-          for i,b in zip(ii, self.N_bas):
+          for i,b,n in zip(jj, N_bas, nMO):
             line = f.readline()
-            while (len(idx) < i+b):
+            while (len(idx) < i+n):
               idx += f.readline().split()[1]
           for i,o in enumerate(self.MO):
             o['type'] = idx[i].upper()
             o.pop('newtype', None)
           for i,o in enumerate(self.MO_b):
             o['type'] = idx[i].upper()
             o.pop('newtype', None)
         elif (line.startswith('#')):
           line = '\n'
       # Desymmetrize the orbital coefficients
       if (sections.get('ORB')):
         if (uhf and (not sections.get('UORB'))):
           return 'No UORB section'
-        if (len(self.N_bas) > 1):
+        if (len(N_bas) > 1):
           for orb in self.MO + self.MO_b:
             orb['coeff'] = np.dot(self.mat, orb['coeff'])
       else:
         return 'No ORB section'
       # Assign occupations
       if (sections.get('OCC')):
         if (uhf and (not sections.get('UOCC'))):
@@ -2653,20 +2658,20 @@
     self.panelBox.setWhatsThis('If checked, the text panel with orbital information will be included in the saved image.')
 
   def toggle_state(self, text):
     self.saveButton.setEnabled(bool(text))
 
   def select_file(self):
     result = QFileDialog.getSaveFileName(self, 'Save image')
-    if (not result):
-      return
     try:
       filename, _ = result
     except ValueError:
       filename = result
+    if (not filename):
+      return
     self.fileBox.setText(filename)
 
   def save_screenshot(self):
     filename = str(self.fileBox.text())
     if (filename == ''):
       self.parent().show_error('Filename not specified')
       return
@@ -5357,14 +5362,16 @@
       a.SetInputConnection(g.GetOutputPort())
       a.Assign('Gradients', 'VECTORS', 'POINT_DATA')
       b = vtk.vtkArrayCalculator()
       b.SetInputConnection(a.GetOutputPort())
       b.AddScalarArrayName('Values')
       b.SetFunction('abs(Values)')
       b.SetResultArrayName('Values')
+      b.ReplaceInvalidValuesOn()
+      b.SetReplacementValue(0.0)
       sl = vtk.vtkStreamTracer()
       sl.SetInputConnection(b.GetOutputPort())
       sl.SetIntegratorTypeToRungeKutta45()
       sl.SetInitialIntegrationStep(0.1)
       sl.SetMinimumIntegrationStep(1e-6) # make it small enough to be able to converge (see below)
       sl.SetTerminalSpeed(1e-8)          # affects tails, but also convergence to stationary points
       sl.SetMaximumNumberOfSteps(100)
@@ -5907,20 +5914,20 @@
     if (self._computeVolumeThread.isRunning()):
       self.interrupt.put(True)
 
   def write_hdf5(self, *args):
     if (self.orbitals.type != 'hdf5'):
       return
     result = QFileDialog.getSaveFileName(self, 'Save HDF5')
-    if (not result):
-      return
     try:
       filename, _ = result
     except ValueError:
       filename = result
+    if (not filename):
+      return
     self._write_hdf5(filename)
 
   def _write_hdf5(self, filename):
     notes = [n['note'] for n in self.notes]
     if (any(notes)):
       self.orbitals.notes = notes
     else:
@@ -5932,20 +5939,20 @@
       traceback.print_exc()
       self.show_error(error)
 
   def write_inporb(self, *args):
     if (not self.haveInpOrb):
       return
     result = QFileDialog.getSaveFileName(self, 'Save InpOrb')
-    if (not result):
-      return
     try:
       filename, _ = result
     except ValueError:
       filename = result
+    if (not filename):
+      return
     self._write_inporb(filename)
 
   def _write_inporb(self, filename):
     try:
       if (self.orbitals.inporb == 'gen'):
         self.orbitals.create_inporb(filename, self.MO)
       else:
@@ -5955,20 +5962,20 @@
       traceback.print_exc()
       self.show_error(error)
 
   def write_cube(self, *args):
     if (self.surface is None):
       return
     result = QFileDialog.getSaveFileName(self, 'Save cube')
-    if (not result):
-      return
     try:
       filename, _ = result
     except ValueError:
       filename = result
+    if (not filename):
+      return
     try:
       data = self.xyz.GetInput()
       ngrid = data.GetDimensions()
       grid = data.GetSpacing()
       orig = list(data.GetOrigin())
       transform = self.xyz.GetTransform().GetMatrix()
       try:
```

### Comparing `Pegamoid-2.7/setup.py` & `Pegamoid-2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 
 with open("README.md", "r") as f:
     # Remove screenshots
     long_description = re.sub('Screenshots\n-*\n*(<.*> *\n*)*', '', f.read())
 
 setup(name='Pegamoid',
-      version='2.7',
+      version='2.8',
       description='Orbital viewer for OpenMolcas',
       author=u'Ignacio Fdez. Galván',
       author_email='jellby@yahoo.com',
       url='https://gitlab.com/Jellby/Pegamoid',
       license='GPL v3.0',
       scripts=['pegamoid.py'],
       install_requires=['numpy (>=1.9.0)', 'h5py', 'VTK (>=8.1.0)', 'qtpy', 'future (>=0.15.2);python_version<"3.0"' ],
```

