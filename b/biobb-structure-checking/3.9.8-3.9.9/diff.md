# Comparing `tmp/biobb_structure_checking-3.9.8.tar.gz` & `tmp/biobb_structure_checking-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_structure_checking-3.9.8.tar", last modified: Wed Jan 26 14:31:00 2022, max compression
+gzip compressed data, was "dist/biobb_structure_checking-3.9.9.tar", last modified: Wed Jan 26 14:35:38 2022, max compression
```

## Comparing `biobb_structure_checking-3.9.8.tar` & `biobb_structure_checking-3.9.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:31:00.000000 biobb_structure_checking-3.9.8/
--rw-r--r--   0 pau        (501) staff       (20)       65 2021-06-11 09:51:33.000000 biobb_structure_checking-3.9.8/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     4080 2022-01-26 14:31:00.000000 biobb_structure_checking-3.9.8/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     2818 2022-01-26 14:01:14.000000 biobb_structure_checking-3.9.8/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/
--rw-r--r--   0 pau        (501) staff       (20)     4176 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/PDBIO_extended.py
--rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-11 09:51:33.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)     1595 2022-01-18 14:00:47.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/check_structure.py
--rw-r--r--   0 pau        (501) staff       (20)    17727 2022-01-26 14:28:23.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/constants.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:31:00.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/dat/
--rw-r--r--   0 pau        (501) staff       (20)     3033 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/dat/ADT_prm.json
--rw-r--r--   0 pau        (501) staff       (20)     1279 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/dat/CMIP_prm.json
--rw-r--r--   0 pau        (501) staff       (20)   234678 2021-12-23 15:19:58.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/dat/all_residues.in
--rw-r--r--   0 pau        (501) staff       (20)     3732 2022-01-18 14:06:57.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/dat/commands.hlp
--rw-r--r--   0 pau        (501) staff       (20)    95116 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/dat/data_lib.json
--rw-r--r--   0 pau        (501) staff       (20)     6725 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/data_lib_manager.py
--rw-r--r--   0 pau        (501) staff       (20)     1253 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/json_writer.py
--rw-r--r--   0 pau        (501) staff       (20)     3565 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/mmb_server.py
--rw-r--r--   0 pau        (501) staff       (20)    34435 2022-01-18 14:00:47.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/model_utils.py
--rw-r--r--   0 pau        (501) staff       (20)     4936 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/modeller_manager.py
--rw-r--r--   0 pau        (501) staff       (20)     7049 2021-12-23 15:19:58.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/mutation_manager.py
--rw-r--r--   0 pau        (501) staff       (20)     9313 2022-01-18 14:36:15.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/param_input.py
--rw-r--r--   0 pau        (501) staff       (20)     2978 2021-07-01 09:43:57.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/residue_lib_manager.py
--rw-r--r--   0 pau        (501) staff       (20)    14388 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/sequence_manager.py
--rw-r--r--   0 pau        (501) staff       (20)    81328 2022-01-18 14:34:42.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/structure_checking.py
--rw-r--r--   0 pau        (501) staff       (20)    58628 2022-01-18 14:00:47.000000 biobb_structure_checking-3.9.8/biobb_structure_checking/structure_manager.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     4080 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     1177 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       83 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       29 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       25 2022-01-26 14:30:59.000000 biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2022-01-26 14:31:00.000000 biobb_structure_checking-3.9.8/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1392 2022-01-26 13:55:19.000000 biobb_structure_checking-3.9.8/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/
+-rw-r--r--   0 pau        (501) staff       (20)       65 2021-06-11 09:51:33.000000 biobb_structure_checking-3.9.9/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     4080 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     2818 2022-01-26 14:35:00.000000 biobb_structure_checking-3.9.9/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/
+-rw-r--r--   0 pau        (501) staff       (20)     4176 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/PDBIO_extended.py
+-rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-11 09:51:33.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     1595 2022-01-18 14:00:47.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/check_structure.py
+-rw-r--r--   0 pau        (501) staff       (20)    17744 2022-01-26 14:34:17.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/constants.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/dat/
+-rw-r--r--   0 pau        (501) staff       (20)     3033 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/dat/ADT_prm.json
+-rw-r--r--   0 pau        (501) staff       (20)     1279 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/dat/CMIP_prm.json
+-rw-r--r--   0 pau        (501) staff       (20)   234678 2021-12-23 15:19:58.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/dat/all_residues.in
+-rw-r--r--   0 pau        (501) staff       (20)     3734 2022-01-26 14:31:46.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/dat/commands.hlp
+-rw-r--r--   0 pau        (501) staff       (20)    95116 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/dat/data_lib.json
+-rw-r--r--   0 pau        (501) staff       (20)     6725 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/data_lib_manager.py
+-rw-r--r--   0 pau        (501) staff       (20)     1253 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/json_writer.py
+-rw-r--r--   0 pau        (501) staff       (20)     3565 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/mmb_server.py
+-rw-r--r--   0 pau        (501) staff       (20)    34435 2022-01-18 14:00:47.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/model_utils.py
+-rw-r--r--   0 pau        (501) staff       (20)     4936 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/modeller_manager.py
+-rw-r--r--   0 pau        (501) staff       (20)     7049 2021-12-23 15:19:58.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/mutation_manager.py
+-rw-r--r--   0 pau        (501) staff       (20)     9313 2022-01-18 14:36:15.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/param_input.py
+-rw-r--r--   0 pau        (501) staff       (20)     2978 2021-07-01 09:43:57.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/residue_lib_manager.py
+-rw-r--r--   0 pau        (501) staff       (20)    14388 2021-12-15 11:10:54.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/sequence_manager.py
+-rw-r--r--   0 pau        (501) staff       (20)    81453 2022-01-26 14:31:46.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/structure_checking.py
+-rw-r--r--   0 pau        (501) staff       (20)    58628 2022-01-18 14:00:47.000000 biobb_structure_checking-3.9.9/biobb_structure_checking/structure_manager.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     4080 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     1177 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       83 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       29 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       25 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2022-01-26 14:35:38.000000 biobb_structure_checking-3.9.9/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1392 2022-01-26 14:34:27.000000 biobb_structure_checking-3.9.9/setup.py
```

### Comparing `biobb_structure_checking-3.9.8/PKG-INFO` & `biobb_structure_checking-3.9.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_structure_checking
-Version: 3.9.8
+Version: 3.9.9
 Summary: BioBB_structure_checking performs MDWeb structure checking tool set as a command line utility.
 Home-page: https://github.com/bioexcel/biobb_structure_checking
 Author: Biobb developers
 Author-email: josep.gelpi@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://BioBB_structure_checking.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
@@ -16,15 +16,15 @@
         
         The Biobb_structure_checking package provides a command line utility ([check_structure](https://biobb-structure-checking.readthedocs.io/en/latest/command_line_usage.html)) and a python [API](https://biobb-structure-checking.readthedocs.io/en/latest/biobb_structure_checking.html).
         
         The latest documentation of this package can be found in our readthedocs site:
         [latest package documentation](http://biobb_structure_checking.readthedocs.io/en/latest/).
         
         ### Version
-        v3.9.8 December 2021
+        v3.9.9 December 2021
         
         ### Requirements
         
         * Biopython
         ### Optional requirements
         * psutil (required for --debug, included in conda pkg.)
         * Modeller (required for some functionalities, not included in conda pkg.)
@@ -33,23 +33,23 @@
         ### Installation
         Using PIP:
         
         > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA.
         
         * Installation:
         
-                pip install "biobb_structure_checking>=3.9.8"
+                pip install "biobb_structure_checking>=3.9.9"
         
         * Usage: [Python API documentation](https://biobb_structure_checking.readthedocs.io/en/latest/modules.html).
         
         Using ANACONDA:
         
         * Installation:
         
-                conda install -c bioconda "biobb_structure_checking>=3.9.8"
+                conda install -c bioconda "biobb_structure_checking>=3.9.9"
         
         * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb_structure_checking.readthedocs.io/en/latest/modules.html) and the  [Command Line documentation](https://biobb_structure_checking.readthedocs.io/en/latest/command_line.html)
         
         ### Copyright & Licensing
         This software has been developed in the MMB group (http://mmb.irbbarcelona.org) at the
         BSC (https://www.bsc.es/) & IRB (https://www.irbbarcelona.org/) for the European BioExcel (https://bioexcel.eu/), funded by the European Commission
         (EU H2020 [675728](https://cordis.europa.eu/projects/675728)).
```

### Comparing `biobb_structure_checking-3.9.8/README.md` & `biobb_structure_checking-3.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 The Biobb_structure_checking package provides a command line utility ([check_structure](https://biobb-structure-checking.readthedocs.io/en/latest/command_line_usage.html)) and a python [API](https://biobb-structure-checking.readthedocs.io/en/latest/biobb_structure_checking.html).
 
 The latest documentation of this package can be found in our readthedocs site:
 [latest package documentation](http://biobb_structure_checking.readthedocs.io/en/latest/).
 
 ### Version
-v3.9.8 December 2021
+v3.9.9 December 2021
 
 ### Requirements
 
 * Biopython
 ### Optional requirements
 * psutil (required for --debug, included in conda pkg.)
 * Modeller (required for some functionalities, not included in conda pkg.)
@@ -23,23 +23,23 @@
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA.
 
 * Installation:
 
-        pip install "biobb_structure_checking>=3.9.8"
+        pip install "biobb_structure_checking>=3.9.9"
 
 * Usage: [Python API documentation](https://biobb_structure_checking.readthedocs.io/en/latest/modules.html).
 
 Using ANACONDA:
 
 * Installation:
 
-        conda install -c bioconda "biobb_structure_checking>=3.9.8"
+        conda install -c bioconda "biobb_structure_checking>=3.9.9"
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb_structure_checking.readthedocs.io/en/latest/modules.html) and the  [Command Line documentation](https://biobb_structure_checking.readthedocs.io/en/latest/command_line.html)
 
 ### Copyright & Licensing
 This software has been developed in the MMB group (http://mmb.irbbarcelona.org) at the
 BSC (https://www.bsc.es/) & IRB (https://www.irbbarcelona.org/) for the European BioExcel (https://bioexcel.eu/), funded by the European Commission
 (EU H2020 [675728](https://cordis.europa.eu/projects/675728)).
```

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/PDBIO_extended.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/PDBIO_extended.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/check_structure.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/check_structure.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/constants.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Global constants for structure_checking module
 """
 import argparse
 from os.path import join as opj
 from os.path import dirname
 from biobb_structure_checking.param_input import Dialog
 
-VERSION = '3.9.8'
+VERSION = '3.9.9'
 
 # Default locations and settings
 DATA_DIR_DEFAULT_PATH = 'dat'
 RES_LIBRARY_DEFAULT_PATH = 'all_residues.in'
 DATA_LIBRARY_DEFAULT_PATH = 'data_lib.json'
 CACHE_DIR_DEFAULT_PATH = 'tmpPDB'
 COMMANDS_HELP_PATH = 'commands.hlp'
@@ -281,15 +281,15 @@
 
 DIALOGS.add_entry('backbone', 'Checks and fixes several backbone issues')
 DIALOGS.add_option('backbone', '--fix_atoms', 'fix_atoms',\
     'Add missing Oxygen atoms to backbone (All | None | List)')
 DIALOGS.add_option('backbone', '--fix_chain', 'fix_chain',\
     'Fixes missing main chain segments (All | None | List)')
 DIALOGS.add_option('backbone', '--add_caps', 'add_caps',\
-    'Adds ACE and NME caps to missing main chain segments (All | None)')
+    'Adds ACE and NME caps to missing main chain segments (All | None | Breaks | Terms)')
 DIALOGS.add_option('backbone', '--no_check_clashes', 'no_check_clashes',\
     'Do not check for new clashes', 'bool')
 DIALOGS.add_option('backbone', '--extra_gap', 'extra_gap',\
     'Replace extra_gap additional flanking residues', int)
 DIALOGS.add_option('backbone', '--no_recheck', 'no_recheck',\
     'Do not re-check after modification', 'bool')
```

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/dat/ADT_prm.json` & `biobb_structure_checking-3.9.9/biobb_structure_checking/dat/ADT_prm.json`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/dat/CMIP_prm.json` & `biobb_structure_checking-3.9.9/biobb_structure_checking/dat/CMIP_prm.json`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/dat/all_residues.in` & `biobb_structure_checking-3.9.9/biobb_structure_checking/dat/all_residues.in`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/dat/commands.hlp` & `biobb_structure_checking-3.9.9/biobb_structure_checking/dat/commands.hlp`

 * *Files 8% similar despite different names*

```diff
@@ -52,22 +52,22 @@
     Detect/Fix Improper quirality
     Checks generated clashes unless --no_check_clashes set
 fixside [--fix All |None|Residue List] [--no_check_clashes]
     Complete side chains (heavy atoms, protein only)
     Checks generated clashes unless --no_check_clashes set
     --rebuild  Rebuild complete side chain using Modeller
 backbone [--fix_atoms All|None|Residue List]
-         [--fix_main All|None|Break list] 
+         [--fix_chain All|None|Break list] 
          [--add_caps All|None|Break list] 
          [--extra_gap]
          [--no_recheck]
          [--no_check_clashes]
     Analyze main chain missing atoms and fragments (protein only).
     --fix_atoms Missing O, OXT atoms can be fixed 
-    --fix_main Missing fragments filled using comparative modelling (Modeller License needed)
+    --fix_chain Missing fragments filled using comparative modelling (Modeller License needed)
     --add_caps Adds ACE and NME residues as necessary, preserving existing atoms
     --extra_gap Recovers additional residues from model either side of the break, helps to fix loop connections (experimental)
     Rechecks beckbone on each op unless --no_recheck is set.
     Generated clashes are checked unless --no_check_clashes
 
 
 3. Structure Warnings (no fix)
```

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/dat/data_lib.json` & `biobb_structure_checking-3.9.9/biobb_structure_checking/dat/data_lib.json`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/data_lib_manager.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/data_lib_manager.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/json_writer.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/json_writer.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/mmb_server.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/mmb_server.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/model_utils.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/model_utils.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/modeller_manager.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/modeller_manager.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/mutation_manager.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/mutation_manager.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/param_input.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/param_input.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/residue_lib_manager.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/residue_lib_manager.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/sequence_manager.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/sequence_manager.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/structure_checking.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/structure_checking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1594,20 +1594,22 @@
         Analyze/Fix main chain missing atoms and fragments (protein only). Check only with no options. Options accepted as command-line string, or python dictionary.
                 
         Args:
             opts (str | dict - Options dictionary):
                 * fix_atoms (str - Fix missing O, OXT backbone atoms):
                     * **all** - Fix all residues
                     * **residue List** - Fix indicated residues
-                * fix_main (str - Fix backbone main chain):
+                * fix_chain (str - Fix backbone main chain):
                     * **all** - All detected breaks
                     * **break list** - Indicated breaks
                 * add_caps (str - Add ACE and NME residues):
                     * **all** - All detected terminals
                     * **residue_list** - Indicated terminals
+                    * **breaks** - Add caps to backbone breaks
+                    * **terms** - Add caps to true terminals
                 * extra_gap (int) - ('0') Recover addiciontal residues from the model to improve match (experimental)
                 * no_recheck (bool) - (False) Do not recheck backbone after fixing 
                 * no_check_clashes (bool) - (False) Do not check for generated clashes
         """
         self._run_method('backbone', opts)
 
     def _backbone_check(self):
```

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking/structure_manager.py` & `biobb_structure_checking-3.9.9/biobb_structure_checking/structure_manager.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/PKG-INFO` & `biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-structure-checking
-Version: 3.9.8
+Version: 3.9.9
 Summary: BioBB_structure_checking performs MDWeb structure checking tool set as a command line utility.
 Home-page: https://github.com/bioexcel/biobb_structure_checking
 Author: Biobb developers
 Author-email: josep.gelpi@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://BioBB_structure_checking.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
@@ -16,15 +16,15 @@
         
         The Biobb_structure_checking package provides a command line utility ([check_structure](https://biobb-structure-checking.readthedocs.io/en/latest/command_line_usage.html)) and a python [API](https://biobb-structure-checking.readthedocs.io/en/latest/biobb_structure_checking.html).
         
         The latest documentation of this package can be found in our readthedocs site:
         [latest package documentation](http://biobb_structure_checking.readthedocs.io/en/latest/).
         
         ### Version
-        v3.9.8 December 2021
+        v3.9.9 December 2021
         
         ### Requirements
         
         * Biopython
         ### Optional requirements
         * psutil (required for --debug, included in conda pkg.)
         * Modeller (required for some functionalities, not included in conda pkg.)
@@ -33,23 +33,23 @@
         ### Installation
         Using PIP:
         
         > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA.
         
         * Installation:
         
-                pip install "biobb_structure_checking>=3.9.8"
+                pip install "biobb_structure_checking>=3.9.9"
         
         * Usage: [Python API documentation](https://biobb_structure_checking.readthedocs.io/en/latest/modules.html).
         
         Using ANACONDA:
         
         * Installation:
         
-                conda install -c bioconda "biobb_structure_checking>=3.9.8"
+                conda install -c bioconda "biobb_structure_checking>=3.9.9"
         
         * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb_structure_checking.readthedocs.io/en/latest/modules.html) and the  [Command Line documentation](https://biobb_structure_checking.readthedocs.io/en/latest/command_line.html)
         
         ### Copyright & Licensing
         This software has been developed in the MMB group (http://mmb.irbbarcelona.org) at the
         BSC (https://www.bsc.es/) & IRB (https://www.irbbarcelona.org/) for the European BioExcel (https://bioexcel.eu/), funded by the European Commission
         (EU H2020 [675728](https://cordis.europa.eu/projects/675728)).
```

### Comparing `biobb_structure_checking-3.9.8/biobb_structure_checking.egg-info/SOURCES.txt` & `biobb_structure_checking-3.9.9/biobb_structure_checking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_structure_checking-3.9.8/setup.py` & `biobb_structure_checking-3.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_structure_checking",
-    version="3.9.8",
+    version="3.9.9",
     author="Biobb developers",
     author_email="josep.gelpi@bsc.es",
     description="BioBB_structure_checking performs MDWeb structure checking tool set as a command line utility.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_structure_checking",
```

