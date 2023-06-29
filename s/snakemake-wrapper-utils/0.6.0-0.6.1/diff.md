# Comparing `tmp/snakemake_wrapper_utils-0.6.0.tar.gz` & `tmp/snakemake_wrapper_utils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_wrapper_utils-0.6.0.tar", max compression
+gzip compressed data, was "snakemake_wrapper_utils-0.6.1.tar", max compression
```

## Comparing `snakemake_wrapper_utils-0.6.0.tar` & `snakemake_wrapper_utils-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1090 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/LICENSE.md
--rw-r--r--   0        0        0      434 2023-06-21 13:15:47.388283 snakemake_wrapper_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/__init__.py
--rw-r--r--   0        0        0     5076 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/bcftools.py
--rw-r--r--   0        0        0     1638 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/java.py
--rw-r--r--   0        0        0     2761 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/samtools.py
--rw-r--r--   0        0        0      747 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/snakemake.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 snakemake_wrapper_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-29 10:07:06.035309 snakemake_wrapper_utils-0.6.1/LICENSE.md
+-rw-r--r--   0        0        0      434 2023-06-29 10:07:20.091279 snakemake_wrapper_utils-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-29 10:07:06.035309 snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/__init__.py
+-rw-r--r--   0        0        0     5076 2023-06-29 10:07:06.035309 snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/bcftools.py
+-rw-r--r--   0        0        0     1638 2023-06-29 10:07:06.035309 snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/java.py
+-rw-r--r--   0        0        0     2761 2023-06-29 10:07:06.035309 snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/samtools.py
+-rw-r--r--   0        0        0      751 2023-06-29 10:07:06.035309 snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/snakemake.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 snakemake_wrapper_utils-0.6.1/PKG-INFO
```

### Comparing `snakemake_wrapper_utils-0.6.0/LICENSE.md` & `snakemake_wrapper_utils-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/bcftools.py` & `snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/bcftools.py`

 * *Files identical despite different names*

### Comparing `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/java.py` & `snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/java.py`

 * *Files identical despite different names*

### Comparing `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/samtools.py` & `snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/samtools.py`

 * *Files identical despite different names*

### Comparing `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/snakemake.py` & `snakemake_wrapper_utils-0.6.1/snakemake_wrapper_utils/snakemake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 def get_mem(snakemake, out_unit="MiB"):
     """
     Obtain requested memory (from resources) and return in given units.
     If no memory resources found, return 0.
     """
 
     # Store memory in MiB
-    mem_mb = snakemake.resources.get("mem_gb", 0) * 1024
+    mem_mb = snakemake.resources.get("mem_gb", 0.2) * 1024
     if not mem_mb:
-        mem_mb = snakemake.resources.get("mem_mb", 0)
+        mem_mb = snakemake.resources.get("mem_mb", 205)
 
     if out_unit == "KiB":
         return mem_mb * 1024
     elif out_unit == "MiB":
         return mem_mb
     elif out_unit == "GiB":
         return mem_mb / 1024
```

### Comparing `snakemake_wrapper_utils-0.6.0/PKG-INFO` & `snakemake_wrapper_utils-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-wrapper-utils
-Version: 0.6.0
+Version: 0.6.1
 Summary: A collection of utils for Snakemake wrappers.
 License: MIT
 Author: Johannes Köster
 Author-email: johannes.koester@tu-dortmund.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

