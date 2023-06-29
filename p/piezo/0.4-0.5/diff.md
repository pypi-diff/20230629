# Comparing `tmp/piezo-0.4.tar.gz` & `tmp/piezo-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piezo-0.4.tar", last modified: Wed Mar 22 11:59:54 2023, max compression
+gzip compressed data, was "piezo-0.5.tar", last modified: Thu Jun 29 15:52:33 2023, max compression
```

## Comparing `piezo-0.4.tar` & `piezo-0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:59:54.130151 piezo-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-03-22 11:59:28.000000 piezo-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-22 11:59:54.130151 piezo-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-03-22 11:59:28.000000 piezo-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-22 11:59:28.000000 piezo-0.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:59:54.126151 piezo-0.4/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-22 11:59:28.000000 piezo-0.4/bin/piezo-predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:59:54.126151 piezo-0.4/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-22 11:59:28.000000 piezo-0.4/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-03-22 11:59:28.000000 piezo-0.4/piezo/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-03-22 11:59:28.000000 piezo-0.4/piezo/grammar_GARC1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:59:54.126151 piezo-0.4/piezo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-22 11:59:54.000000 piezo-0.4/piezo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-22 11:59:54.000000 piezo-0.4/piezo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:59:54.000000 piezo-0.4/piezo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:59:33.000000 piezo-0.4/piezo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-22 11:59:54.000000 piezo-0.4/piezo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 11:59:54.000000 piezo-0.4/piezo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-22 11:59:28.000000 piezo-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-22 11:59:54.130151 piezo-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:59:54.130151 piezo-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-03-22 11:59:28.000000 piezo-0.4/tests/test_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.199128 piezo-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-29 15:52:03.000000 piezo-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-29 15:52:33.199128 piezo-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-29 15:52:03.000000 piezo-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 15:52:03.000000 piezo-0.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.195128 piezo-0.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 15:52:03.000000 piezo-0.5/bin/piezo-predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.195128 piezo-0.5/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 15:52:03.000000 piezo-0.5/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-29 15:52:03.000000 piezo-0.5/piezo/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-06-29 15:52:03.000000 piezo-0.5/piezo/grammar_GARC1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.199128 piezo-0.5/piezo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:52:12.000000 piezo-0.5/piezo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 15:52:03.000000 piezo-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-29 15:52:33.199128 piezo-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.199128 piezo-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-29 15:52:03.000000 piezo-0.5/tests/test_catalogue.py
```

### Comparing `piezo-0.4/LICENSE` & `piezo-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `piezo-0.4/PKG-INFO` & `piezo-0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piezo
-Version: 0.4
+Version: 0.5
 Summary: Predicting the effect of an antibiotic from gene mutations
 Home-page: https://github.com/oxfordmmm/piezo
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 [![Tests](https://github.com/oxfordmmm/piezo/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/piezo/actions/workflows/tests.yaml)
 [![codecov](https://codecov.io/gh/oxfordmmm/piezo/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/piezo)
-[![Documentation Status](https://readthedocs.org/projects/piezo/badge/?version=latest)](https://piezo.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/piezo.svg)](https://badge.fury.io/py/piezo)
+[![Docs](https://github.com/oxfordmmm/piezo/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/piezo/)
+[![PyPI version](https://badge.fury.io/py/piezo.svg)](https://badge.fury.io/py/piezo)
 
 # piezo
 
 Predict the effect of a genetic mutation on the effect of an antibiotic using a supplied AMR catalogue.
 
 This code was developed as part of the [CRyPTIC](http://www.crypticproject.org) international tuberculosis consortium. If you would like to use the software commercially, please consult the LICENCE file.
 
@@ -41,14 +42,17 @@
 ```
 git clone https://github.com/oxfordmmm/piezo
 cd piezo
 pip install .
 ```
 The pre-requisites are all fairly standard and are listed in `setup.cfg` so will be automatically installed.
 
+## Documentation
+API documentation for developers can be found here: https://oxfordmmm.github.io/piezo/
+
 ## Included files
 
 ```
 $ ls tests/test-catalogue/
 NC_004148.2.gbk                    NC_004148.2_TEST_GM1_RFUS_v1.0.csv
 ```
 NC_004148 is the reference genome of the human metapneumovirus and is used primarily for unit testing since it is small and fast to parse.
```

### Comparing `piezo-0.4/README.md` & `piezo-0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Tests](https://github.com/oxfordmmm/piezo/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/piezo/actions/workflows/tests.yaml)
 [![codecov](https://codecov.io/gh/oxfordmmm/piezo/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/piezo)
-[![Documentation Status](https://readthedocs.org/projects/piezo/badge/?version=latest)](https://piezo.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/piezo.svg)](https://badge.fury.io/py/piezo)
+[![Docs](https://github.com/oxfordmmm/piezo/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/piezo/)
+[![PyPI version](https://badge.fury.io/py/piezo.svg)](https://badge.fury.io/py/piezo)
 
 # piezo
 
 Predict the effect of a genetic mutation on the effect of an antibiotic using a supplied AMR catalogue.
 
 This code was developed as part of the [CRyPTIC](http://www.crypticproject.org) international tuberculosis consortium. If you would like to use the software commercially, please consult the LICENCE file.
 
@@ -25,14 +26,17 @@
 ```
 git clone https://github.com/oxfordmmm/piezo
 cd piezo
 pip install .
 ```
 The pre-requisites are all fairly standard and are listed in `setup.cfg` so will be automatically installed.
 
+## Documentation
+API documentation for developers can be found here: https://oxfordmmm.github.io/piezo/
+
 ## Included files
 
 ```
 $ ls tests/test-catalogue/
 NC_004148.2.gbk                    NC_004148.2_TEST_GM1_RFUS_v1.0.csv
 ```
 NC_004148 is the reference genome of the human metapneumovirus and is used primarily for unit testing since it is small and fast to parse.
```

### Comparing `piezo-0.4/bin/piezo-predict.py` & `piezo-0.5/bin/piezo-predict.py`

 * *Files identical despite different names*

### Comparing `piezo-0.4/piezo/catalogue.py` & `piezo-0.5/piezo/catalogue.py`

 * *Files identical despite different names*

### Comparing `piezo-0.4/piezo/grammar_GARC1.py` & `piezo-0.5/piezo/grammar_GARC1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #! /usr/bin/env python
 '''All logic required to parse and generate predictions from a catalogue in GARC1
 '''
 
 import collections
+import re
 
 import pandas
 
 
 def split_mutation(row: pandas.Series) -> pandas.Series:
     '''Take a row of the catalogue and get info about the mutation from it.
     This includes the type, ref, alt, position and minor populations
@@ -68,27 +69,40 @@
         except:
             position=cols[0][:-1]
             if position[0]=="-":
                 mutation_affects="PROM"
 
     elif len(cols) in [2,3]:
         mutation_type="INDEL"
-        mutation_affects="CDS"
-        position=cols[0]
-        try:
-            if int(position)<0:
-                mutation_affects="PROM"
-            elif int(position)==0:
-                valid = False
-        except:
+        percentage = False
+        if len(cols) == 2:
+            #Checking for percentage deletions (of form "del_<percent>")
+            try:
+                float(cols[1])
+                percentage = True
+            except ValueError:
+                percentage = False
+            if percentage:
+                position = None
+        if percentage:
+            mutation_affects = "GENE"
+        else:
+            mutation_affects = "CDS"
+            position=cols[0]
             try:
-                if position[0]=="-":
+                if int(position)<0:
                     mutation_affects="PROM"
+                elif int(position)==0:
+                    valid = False
             except:
-                valid = False
+                try:
+                    if position[0]=="-":
+                        mutation_affects="PROM"
+                except:
+                    valid = False
 
     else:
         raise ValueError("Badly formed mutation: "+row["MUTATION"])
     
     if not valid:
         #Valid mutation not found, so complain
         raise ValueError("Badly formed mutation: "+row['MUTATION'])
@@ -346,33 +360,76 @@
             assert int(priority) in range (1,11), 'priority must be an integer in range 1,2..10'
             if values.index(row['PREDICTION']) < values.index(pred):
                 #This row's prediction is more important than the current, so check for minors and prioritise
                 if minor is None and row['MINOR'] == '':
                     #Neither are minor populations so act normally
                     pred = row['PREDICTION']
 
-                elif row['MINOR'] != '' and minor < 1 and float(row['MINOR']) < 1:
+                elif minor is not None and row['MINOR'] != '' and minor < 1 and float(row['MINOR']) < 1:
                     #We have FRS
                     if minor >= float(row['MINOR']):
                         #Match
                         pred = row['PREDICTION']
 
-                elif row['MINOR'] != '' and minor >= 1 and float(row['MINOR']) >= 1:
+                elif minor is not None and row['MINOR'] != '' and minor >= 1 and float(row['MINOR']) >= 1:
                     #We have COV
                     if minor >= float(row['MINOR']):
                         #Match
                         pred = row['PREDICTION']
 
                 else:
                     #Mismatch, so only give a match for defaults
                     if "*" in row['MUTATION']:
                         pred = row['PREDICTION']
     if pred:
         predictions[int(priority)] = str(pred)
 
+def large_del(predictions: {int: str}, rules: pandas.DataFrame, size: float, minor: float) -> None:
+    '''Row prediction, but specifically for large deletions
+
+    Args:
+        predictions ({int: str}): Predictions dictionary
+        rules (pandas.DataFrame): Rules from the catalogue
+        size (float): Percentage of the gene deleted (as a decimal)
+        minor (float): Minors (if existing)
+    '''
+    pred = None
+    current = -1
+    #Find which rules are large deletions and see if the mutation is >= rule
+    deletion = re.compile(r"""del_([01]\.[0-9]+)""")
+    for _, rule in rules.iterrows():
+        if deletion.fullmatch(rule['MUTATION']):
+            percentage = float(deletion.fullmatch(rule['MUTATION']).groups()[0])
+            if size >= percentage and percentage > current:
+                #Match!
+                if minor is None and rule['MINOR'] == '':
+                    #Neither are minor populations so act normally
+                    pred = rule['PREDICTION']
+                    current = percentage
+                elif minor is not None and rule['MINOR'] != '' and minor < 1 and float(rule['MINOR']) < 1:
+                    #We have FRS
+                    if minor >= float(rule['MINOR']):
+                        #Match
+                        pred = rule['PREDICTION']
+                        current = percentage
+
+                elif minor is not None and rule['MINOR'] != '' and minor >= 1 and float(rule['MINOR']) >= 1:
+                    #We have COV
+                    if minor >= float(rule['MINOR']):
+                        #Match
+                        pred = rule['PREDICTION']
+                        current = percentage
+                else:
+                    #Mismatch so only match default
+                    if rule['MUTATION'] == "del_0.0":
+                        pred = rule['PREDICTION']
+                        current = percentage
+    if pred:
+        predictions[1] = str(pred)
+
 
 def process_snp_variants(mutation_affects: str,
                          predictions: {int: str},
                          before: str, after: str,
                          mutation: str,
                          rules: pandas.DataFrame,
                          rules_mutation_type_vector: pandas.Series,
@@ -489,14 +546,17 @@
         rules_position_vector (pandas.Series): Series for the rules which refer to this position
         indel_length (int): Length of the indel
         indel_type (str): Type of the indel. i.e ins/del/fs/indel
         indel_bases (str): Bases inserted/deleted (if applicable)
         position (int): Position of the indel
         minor (float): Float for supporting evidence of minor populations (or None if not a minor population)
     '''
+    if mutation_affects == "GENE":
+        #Large deletions are priority 1
+        large_del(predictions, rules.loc[rules_mutation_type_vector], indel_length, minor)
 
     # PRIORITY 1: any insertion or deletion in the CDS or PROM (e.g. rpoB_*_indel or rpoB_-*_indel)
     if mutation_affects == "CDS":
         row=rules.loc[rules_mutation_type_vector & (rules.MUTATION=="*_indel")]
     else:
         row=rules.loc[rules_mutation_type_vector & (rules.MUTATION=="-*_indel")]
     #any insertion or deletion in the CDS or PROM
@@ -597,37 +657,51 @@
 
         mutation_affects=infer_mutation_affects(position)
 
         before=mutation[0]
         after=mutation[-1]
 
     elif len(cols) in [2,3]:
-
         mutation_type="INDEL"
-
-        position=int(cols[0])
-
-        mutation_affects=infer_mutation_affects(position)
-
-        # the third element is one of indel, ins, del or the special case fs
-        indel_type=cols[1]
-
-        assert indel_type in ['indel','ins','del','fs'], "form of indel not recognised: "+indel_type
-
-        # if there is a fourth and final element to an INDEL it is either _4 or _ctgc
-        if len(cols)==3:
-            assert indel_type in ['ins','del'], "form of indel does not make sense when length or bases specified!: "+indel_type
+        #Checking for large deletions
+        percentage = False
+        if cols[0] == "del":
             try:
-                indel_length=int(cols[2])
-            except:
-                indel_length=len(cols[2])
-                indel_bases=cols[2]
-                assert 0 not in [c in ['a','t','c','g','z','x'] for c in indel_bases], "only nucleotides of a,t,c,g,z,x are allowed!"
+                float(cols[1])
+                percentage = True
+            except ValueError:
+                percentage = False
+
+        if percentage:
+            mutation_affects = "GENE"
+            indel_type = "del"
+            indel_length = float(cols[1])
+        else:
+            try:
+                position = int(cols[0])
+            except ValueError:
+                assert False, "Invalid mutation: " + mutation
+            mutation_affects=infer_mutation_affects(position)
+
+            # the third element is one of indel, ins, del or the special case fs
+            indel_type=cols[1]
+
+            assert indel_type in ['indel','ins','del','fs'], "form of indel not recognised: "+indel_type
+
+            # if there is a fourth and final element to an INDEL it is either _4 or _ctgc
+            if len(cols)==3:
+                assert indel_type in ['ins','del'], "form of indel does not make sense when length or bases specified!: "+indel_type
+                try:
+                    indel_length=int(cols[2])
+                except:
+                    indel_length=len(cols[2])
+                    indel_bases=cols[2]
+                    assert 0 not in [c in ['a','t','c','g','z','x'] for c in indel_bases], "only nucleotides of a,t,c,g,z,x are allowed!"
 
-            assert indel_length>0, "makes no sense to have a negative indel length! "+cols[2]
+                assert indel_length>0, "makes no sense to have a negative indel length! "+cols[2]
 
     assert mutation_type in ['INDEL','SNP'], "form of mutation_type not recognised: "+mutation_type
 
     # insist we've been given an amino acid or a wildcard only
     if mutation_type=="SNP":
         sanity_check_snp(before,after)
```

### Comparing `piezo-0.4/piezo.egg-info/PKG-INFO` & `piezo-0.5/piezo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piezo
-Version: 0.4
+Version: 0.5
 Summary: Predicting the effect of an antibiotic from gene mutations
 Home-page: https://github.com/oxfordmmm/piezo
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 [![Tests](https://github.com/oxfordmmm/piezo/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/piezo/actions/workflows/tests.yaml)
 [![codecov](https://codecov.io/gh/oxfordmmm/piezo/branch/master/graph/badge.svg)](https://codecov.io/gh/oxfordmmm/piezo)
-[![Documentation Status](https://readthedocs.org/projects/piezo/badge/?version=latest)](https://piezo.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/piezo.svg)](https://badge.fury.io/py/piezo)
+[![Docs](https://github.com/oxfordmmm/piezo/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/piezo/)
+[![PyPI version](https://badge.fury.io/py/piezo.svg)](https://badge.fury.io/py/piezo)
 
 # piezo
 
 Predict the effect of a genetic mutation on the effect of an antibiotic using a supplied AMR catalogue.
 
 This code was developed as part of the [CRyPTIC](http://www.crypticproject.org) international tuberculosis consortium. If you would like to use the software commercially, please consult the LICENCE file.
 
@@ -41,14 +42,17 @@
 ```
 git clone https://github.com/oxfordmmm/piezo
 cd piezo
 pip install .
 ```
 The pre-requisites are all fairly standard and are listed in `setup.cfg` so will be automatically installed.
 
+## Documentation
+API documentation for developers can be found here: https://oxfordmmm.github.io/piezo/
+
 ## Included files
 
 ```
 $ ls tests/test-catalogue/
 NC_004148.2.gbk                    NC_004148.2_TEST_GM1_RFUS_v1.0.csv
 ```
 NC_004148 is the reference genome of the human metapneumovirus and is used primarily for unit testing since it is small and fast to parse.
```

### Comparing `piezo-0.4/setup.cfg` & `piezo-0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `piezo-0.4/tests/test_catalogue.py` & `piezo-0.5/tests/test_catalogue.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     assert test_catalogue.catalogue.version=="v1.0"
 
     assert test_catalogue.catalogue.values==["R","F","U","S"]
 
     assert test_catalogue.catalogue.grammar=="GARC1"
 
-    assert test_catalogue.catalogue.number_rows == 42
+    assert test_catalogue.catalogue.number_rows == 45
 
     assert test_catalogue.catalogue.drugs==['DRUG_A','DRUG_B']
 
     #Ordering of lists is annoying here, so sort both
     genes = sorted(genes)
     assert sorted(test_catalogue.catalogue.genes) == genes
 
@@ -91,14 +91,25 @@
     assert test_catalogue.predict("M2@t-15o")=={'DRUG_A': 'F', 'DRUG_B': 'S'}
 
     assert test_catalogue.predict("M2@t-15x")=={'DRUG_A': 'F', 'DRUG_B': 'S'}
 
     # check that a gene not in the catalogue simply returns an "S"
     assert test_catalogue.predict("N1@S2T")=="S"
 
+    #Checking large deletions
+    assert test_catalogue.predict("M2@del_1.0") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.9") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.85") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.8") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.7") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.5") == {"DRUG_A": "U", "DRUG_B": "U"}
+
+    with pytest.raises(Exception):
+        assert test_catalogue.predict("M2@del_0.5s") == {"DRUG_A": "U", "DRUG_B": "U"}
+
     # bad prediction
     with pytest.raises(Exception):
         assert test_catalogue.predict("M2@L73P")=={'DRUG_A': 'R', 'DRUG_B': 'R'}
 
     # incorrect amino acid in the alt position
     with pytest.raises(Exception):
         assert test_catalogue.predict("M2@L73B")
@@ -264,9 +275,26 @@
 
     with pytest.raises(ValueError):
         piezo.ResistanceCatalogue("tests/test-catalogue/broken-catalogue6.csv")
     
     #Checking for deprication warnings
     with pytest.warns(UserWarning):
         test_catalogue.predict("M2@L73P", verbose=True)
+    
+    #Minor edge cases of large dels
+    test_catalogue = piezo.ResistanceCatalogue("tests/test-catalogue/NC_004148.2_TEST_v1.0_GARC1_RFUS-minor-COV.csv")
+    assert test_catalogue.predict("M2@del_1.0") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.9:3") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.85:10") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.8:1") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.7") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.5") == {"DRUG_A": "U", "DRUG_B": "U"}
+
+    test_catalogue = piezo.ResistanceCatalogue("tests/test-catalogue/NC_004148.2_TEST_v1.0_GARC1_RFUS-minor-FRS.csv")
+    assert test_catalogue.predict("M2@del_1.0") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.9:0.3") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.85:0.99") == {"DRUG_A": "R", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.8:0.01") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.7") == {"DRUG_A": "U", "DRUG_B": "U"}
+    assert test_catalogue.predict("M2@del_0.5:0.03") == {"DRUG_A": "U", "DRUG_B": "U"}
```

