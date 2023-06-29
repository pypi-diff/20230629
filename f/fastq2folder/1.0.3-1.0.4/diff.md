# Comparing `tmp/fastq2folder-1.0.3.tar.gz` & `tmp/fastq2folder-1.0.4.tar.gz`

## Comparing `fastq2folder-1.0.3.tar` & `fastq2folder-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.3/src/fastq2folder/__init__.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 fastq2folder-1.0.3/src/fastq2folder/fastq2folder.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.3/LICENSE
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.3/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastq2folder-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastq2folder-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/src/fastq2folder/__init__.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/src/fastq2folder/fastq2folder.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/LICENSE
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/PKG-INFO
```

### Comparing `fastq2folder-1.0.3/src/fastq2folder/fastq2folder.py` & `fastq2folder-1.0.4/src/fastq2folder/fastq2folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import gzip
 import shutil
 import pandas as pd
 from Bio import SeqIO
 from scipy import stats
 import numpy as np
+import seaborn as sns
 
 #Create a new folder for the unzipped and binned files to go
 #base_dir = r"C:\Users\egar1\OneDrive\Desktop"
 base_dir = input('Enter path to source directory: ')
 if os.path.isdir(base_dir):
     print('The directory exists')
 else:
```

### Comparing `fastq2folder-1.0.3/LICENSE` & `fastq2folder-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.3/README.md` & `fastq2folder-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.3/pyproject.toml` & `fastq2folder-1.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "pandas", "Bio", "scipy", "numpy", "matplotlib"]
+requires = ["hatchling", "pandas", "Bio", "scipy", "numpy", "matplotlib", "seaborn"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastq2folder"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Elizabeth Gardner", email="egar18111@gmail.com" },
 ]
 description = "Script to process fastq files before epi2me analysis"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `fastq2folder-1.0.3/PKG-INFO` & `fastq2folder-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastq2folder
-Version: 1.0.3
+Version: 1.0.4
 Summary: Script to process fastq files before epi2me analysis
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Elizabeth Gardner <egar18111@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

