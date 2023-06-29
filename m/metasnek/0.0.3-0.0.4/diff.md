# Comparing `tmp/metasnek-0.0.3.tar.gz` & `tmp/metasnek-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasnek-0.0.3.tar", last modified: Thu Jun 22 01:31:22 2023, max compression
+gzip compressed data, was "metasnek-0.0.4.tar", last modified: Thu Jun 29 08:28:54 2023, max compression
```

## Comparing `metasnek-0.0.3.tar` & `metasnek-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 01:31:13.000000 metasnek-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 01:31:13.000000 metasnek-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-22 01:31:22.862733 metasnek-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-22 01:31:13.000000 metasnek-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 01:31:13.000000 metasnek-0.0.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/metasnek/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 01:31:13.000000 metasnek-0.0.3/metasnek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-22 01:31:13.000000 metasnek-0.0.3/metasnek/fastq_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/metasnek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 01:31:22.000000 metasnek-0.0.3/metasnek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:31:22.862733 metasnek-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-22 01:31:13.000000 metasnek-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:31:22.862733 metasnek-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-22 01:31:13.000000 metasnek-0.0.3/tests/test_fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 08:28:40.000000 metasnek-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:28:40.000000 metasnek-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-29 08:28:54.032666 metasnek-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-29 08:28:40.000000 metasnek-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 08:28:40.000000 metasnek-0.0.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/metasnek/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:28:40.000000 metasnek-0.0.4/metasnek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-29 08:28:40.000000 metasnek-0.0.4/metasnek/fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/metasnek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:28:54.032666 metasnek-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-29 08:28:40.000000 metasnek-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-29 08:28:40.000000 metasnek-0.0.4/tests/test_fastq_finder.py
```

### Comparing `metasnek-0.0.3/LICENSE` & `metasnek-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.3/PKG-INFO` & `metasnek-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: metasnek
-Version: 0.0.3
+Version: 0.0.4
 Summary: Misc functions for metagenomics pipelines
 Home-page: https://github.com/beardymcjohnface/metasnek
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MetaSnek
 
 [![](https://img.shields.io/static/v1?label=Licence&message=MIT&color=black)](https://opensource.org/license/mit/)
 [![install with PyPI](https://img.shields.io/badge/Install%20with-PyPI-brightgreen.svg?style=flat-square)](https://pypi.org/project/metasnek/)
```

### Comparing `metasnek-0.0.3/README.md` & `metasnek-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.3/metasnek/fastq_finder.py` & `metasnek-0.0.4/metasnek/fastq_finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             sample_name = row[0].strip()
             r1_file = row[1].strip()
             r2_file = row[2].strip() if len(row) >= 3 else None
 
             if not os.path.isfile(r1_file):
                 raise FileNotFoundError(f"R1 file '{r1_file}' does not exist.")
 
-            if r2_file and not os.path.isfile(r2_file):
+            if r2_file and not os.path.isfile(r2_file) and not r2_file.lower() in ["none", "null"]:
                 raise FileNotFoundError(f"R2 file '{r2_file}' does not exist.")
 
             if r2_file:
                 paired_reads.add((sample_name, r1_file, r2_file))
             else:
                 unpaired_reads.add((sample_name, r1_file))
 
@@ -168,8 +168,11 @@
                 - R1 (str): filepath of R1 reads file
                 - R2 (str): filepath of R2 reads file or None for unpaired
         output_file (str): filepath of output file for writing
     """
 
     with open(output_file, "w") as out:
         for sample in dictionary.keys():
-            out.write(f"{sample}\t{dictionary[sample]['R1']}\t{dictionary[sample]['R2']}\n")
+            if dictionary[sample]['R2'] is not None and dictionary[sample]['R2'].lower() not in ["none", "null"]:
+                out.write(f"{sample}\t{dictionary[sample]['R1']}\t{dictionary[sample]['R2']}\n")
+            else:
+                out.write(f"{sample}\t{dictionary[sample]['R1']}\n")
```

### Comparing `metasnek-0.0.3/metasnek.egg-info/PKG-INFO` & `metasnek-0.0.4/metasnek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: metasnek
-Version: 0.0.3
+Version: 0.0.4
 Summary: Misc functions for metagenomics pipelines
 Home-page: https://github.com/beardymcjohnface/metasnek
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MetaSnek
 
 [![](https://img.shields.io/static/v1?label=Licence&message=MIT&color=black)](https://opensource.org/license/mit/)
 [![install with PyPI](https://img.shields.io/badge/Install%20with-PyPI-brightgreen.svg?style=flat-square)](https://pypi.org/project/metasnek/)
```

### Comparing `metasnek-0.0.3/setup.py` & `metasnek-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     "Environment :: Console",
     "Environment :: MacOS X",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT license",
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 
 
 setup(
     name="metasnek",
     url="https://github.com/beardymcjohnface/metasnek",
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     description="Misc functions for metagenomics pipelines",
     long_description=get_description(),
     long_description_content_type="text/markdown",
     version=get_version(),
     author="Michael Roach",
     author_email="beardymcjohnface@gmail.com",
 )
```

### Comparing `metasnek-0.0.3/tests/test_fastq_finder.py` & `metasnek-0.0.4/tests/test_fastq_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,14 @@
 
     with open(output_file, "r") as file:
         content = file.read()
 
     expected_content = (
         "sample1\t" + os.path.join(temp_directory, "sample1_R1.fastq") + "\t" + os.path.join(temp_directory, "sample1_R2.fastq") + "\n"
         "sample2\t" + os.path.join(temp_directory, "sample2_R1_001.fastq.gz") + "\t" + os.path.join(temp_directory, "sample2_R2_001.fastq.gz") + "\n"
-        "sample3\t" + os.path.join(temp_directory, "sample3.fastq") + "\tNone\n"
-        "sample4_R2\t" + os.path.join(temp_directory, "sample4_R2.fastq") + "\tNone\n"
-        "sample5\t" + os.path.join(temp_directory, "sample5.fasta.gz") + "\tNone\n"
-        "sample6\t" + os.path.join(temp_directory, "sample6.fastq.gz") + "\tNone\n"
+        "sample3\t" + os.path.join(temp_directory, "sample3.fastq") + "\n"
+        "sample4_R2\t" + os.path.join(temp_directory, "sample4_R2.fastq") + "\n"
+        "sample5\t" + os.path.join(temp_directory, "sample5.fasta.gz") + "\n"
+        "sample6\t" + os.path.join(temp_directory, "sample6.fastq.gz") + "\n"
     )
 
     assert content == expected_content
```

