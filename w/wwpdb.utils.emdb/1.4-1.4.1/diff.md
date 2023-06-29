# Comparing `tmp/wwpdb.utils.emdb-1.4.tar.gz` & `tmp/wwpdb.utils.emdb-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.4.tar", last modified: Tue Jun 27 11:53:16 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.4.1.tar", last modified: Thu Jun 29 11:56:32 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.4.tar` & `wwpdb.utils.emdb-1.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11264 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   668369 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2286661 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)      389 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   219336 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      975 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 11:53:00.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.131426 wwpdb.utils.emdb-1.4.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-06-29 11:56:32.131426 wwpdb.utils.emdb-1.4.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-29 11:56:32.135427 wwpdb.utils.emdb-1.4.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.123426 wwpdb.utils.emdb-1.4.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.123426 wwpdb.utils.emdb-1.4.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.123426 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.127426 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11264 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.131426 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   667859 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2283184 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      389 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.131426 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   217727 2023-06-29 11:55:33.000000 wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 11:56:32.123426 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-06-29 11:56:32.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      975 2023-06-29 11:56:32.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-29 11:56:32.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-06-29 11:56:32.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-29 11:56:12.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-06-29 11:56:32.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-29 11:56:32.000000 wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.4/PKG-INFO` & `wwpdb.utils.emdb-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.4
+Version: 1.4.1
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.4/setup.py` & `wwpdb.utils.emdb-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.4.1"
+        XML_OUT_VERSION = "3.0.4.0"
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
         EM_DEPUI = "em_depui"
@@ -588,15 +588,14 @@
             "_em_map.pixel_spacing_z": '<xs:element name="z" type="pixel_spacing_type"/>',
             "_em_particle_selection.reference_model": '<xs:element name="reference_model" type="xs:token" minOccurs="0"/>',
             "_em_particle_selection.method": '<xs:element name="method" type="xs:string" minOccurs="0"/>',
             "_em_particle_selection.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_em_particle_selection.num_particles_selected": '<xs:element name="number_selected" type="xs:positiveInteger" minOccurs="0"/>',
             "_em_software.name": '<xs:element name="name" type="xs:token" minOccurs="0"/>',
             "_em_software.version": '<xs:element name="version" type="xs:token" minOccurs="0"/>',
-            "_em_software.category": '<xs:element name="category" type="xs:token" minOccurs="0"/>',
             "_em_software.details": '<xs:element name="processing_details" type="xs:string" minOccurs="0"/>',
             "_em_specimen.concentration": '<xs:element name="concentration" minOccurs="0">',
             "_em_specimen.id": '<xs:element name="specimen_preparation_id" type="xs:positiveInteger"/>',
             "_em_specimen.details": '<xs:element name="details" type="xs:string" minOccurs="0">',
             "_em_staining.type": '<xs:element name="type">',
             "_em_staining.material": '<xs:element name="material" type="xs:token">',
             "_em_staining.details": '<xs:element name="details" type="xs:string" minOccurs="0">',
@@ -1801,35 +1800,26 @@
                 def set_el_version(soft, soft_in):
                     """
                     XSD: <xs:element name="version" type="xs:token" minOccurs="0"/>
                     CIF: _em_software.version
                     """
                     set_cif_value(soft.set_version, "version", const.EM_SOFTWARE, cif_list=soft_in)
 
-                def set_el_category(soft, soft_in):
-                    """
-                    XSD: <xs:element name="category" type="xs:token" minOccurs="0"/>
-                    CIF: _em_software.category
-                    """
-                    set_cif_value(soft.set_category, "category", const.EM_SOFTWARE, cif_list=soft_in)
-
                 def set_el_processing_details(soft, soft_in):
                     """
                     XSD: <xs:element name="processing_details" type="xs:string" minOccurs="0"/>
                     CIF: _em_software.details
                     """
                     set_cif_value(soft.set_processing_details, "details", const.EM_SOFTWARE, cif_list=soft_in)
 
                 # element 1
                 set_el_name(soft, soft_in)
                 # element 2
                 set_el_version(soft, soft_in)
                 # element 3
-                set_el_category(soft, soft_in)
-                # element 4
                 set_el_processing_details(soft, soft_in)
 
             if software_category in category_dict:
                 soft_list = emdb.software_list_type()
                 for soft_in in category_dict[software_category]:
                     soft = emdb.software_type()
                     set_software_type(software_category, soft, soft_in)
```

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Wed May 24 20:24:21 2023 by generateDS.py version 2.41.5.
+# Generated Tue May 23 14:21:39 2023 by generateDS.py version 2.41.5.
 # Python 3.9.5 (default, May 18 2021, 12:31:01)  [Clang 10.0.0 ]
 #
 # Command line options:
 #   ('--root-element', 'emd')
 #   ('-f', '')
-#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.py')
+#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.py')
 #   ('--no-warnings', '')
 #   ('--external-encoding', 'utf-8')
 #
 # Command line arguments:
-#   emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.xsd
+#   emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.xsd
 #
 # Command line:
-#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.xsd
+#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_4_0/emdb.xsd
 #
 # Current working directory (os.getcwd()):
 #   IdeaProjects
 #
 
 import sys
 try:
@@ -1145,37 +1145,14 @@
     CCD='CCD'
     CMOS='CMOS'
     DIRECTELECTRONDETECTOR='DIRECT ELECTRON DETECTOR'
     STORAGEPHOSPORIMAGEPLATES='STORAGE PHOSPOR (IMAGE PLATES)'
     FILM='FILM'
 
 
-class categoryType44(str, Enum):
-    CLASSIFICATION='CLASSIFICATION'
-    CRYSTALLOGRAPHYMERGING='CRYSTALLOGRAPHY MERGING'
-    CTFCORRECTION='CTF CORRECTION'
-    DIFFRACTIONINDEXING='DIFFRACTION INDEXING'
-    EWALDSPHERECORRECTION='EWALD SPHERE CORRECTION'
-    FINALEULERASSIGNMENT='FINAL EULER ASSIGNMENT'
-    IMAGEACQUISITION='IMAGE ACQUISITION'
-    INITIALEULERASSIGNMENT='INITIAL EULER ASSIGNMENT'
-    LATTICEDISTORTIONCORRECTION='LATTICE DISTORTION CORRECTION'
-    LAYERLINEINDEXING='LAYERLINE INDEXING'
-    MASKING='MASKING'
-    MODELFITTING='MODEL FITTING'
-    MODELREFINEMENT='MODEL REFINEMENT'
-    MOLECULARREPLACEMENT='MOLECULAR REPLACEMENT'
-    OTHER='OTHER'
-    PARTICLESELECTION='PARTICLE SELECTION'
-    RECONSTRUCTION='RECONSTRUCTION'
-    SERIESALIGNMENT='SERIES ALIGNMENT'
-    SYMMETRYDETERMINATION='SYMMETRY DETERMINATION'
-    VOLUMESELECTION='VOLUME SELECTION'
-
-
 class classificationType(str, Enum):
     DNA='DNA'
 
 
 class classificationType32(str, Enum):
     MESSENGER='MESSENGER'
     TRANSFER='TRANSFER'
@@ -1699,15 +1676,15 @@
     ISSN='ISSN'
     CAS='CAS'
     CSD='CSD'
     MEDLINE='MEDLINE'
     ASTM='ASTM'
 
 
-class typeType57(str, Enum):
+class typeType56(str, Enum):
     ANGULARRECONSTITUTION='ANGULAR RECONSTITUTION'
     COMMONLINE='COMMON LINE'
     NOTAPPLICABLE='NOT APPLICABLE'
     OTHER='OTHER'
     PROJECTIONMATCHING='PROJECTION MATCHING'
     RANDOMASSIGNMENT='RANDOM ASSIGNMENT'
     MAXIMUMLIKELIHOOD='MAXIMUM LIKELIHOOD'
@@ -1741,30 +1718,30 @@
 
 class unitsType40(str, Enum):
     MINUTE='MINUTE'
     HOUR='HOUR'
     DAY='DAY'
 
 
-class unitsType48(str, Enum):
+class unitsType47(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
-class unitsType50(str, Enum):
+class unitsType49(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
-class unitsType52(str, Enum):
+class unitsType51(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
-class unitsType53(str, Enum):
+class unitsType52(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
 class virus_isolateType(str, Enum):
     OTHER='OTHER'
     SEROCOMPLEX='SEROCOMPLEX'
@@ -1782,15 +1759,15 @@
     VIRUSLIKEPARTICLE='VIRUS-LIKE PARTICLE'
 
 
 class entry_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, emdb_id=None, version='3.0.4.2', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
+    def __init__(self, emdb_id=None, version='3.0.4.0', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.emdb_id = _cast(None, emdb_id)
         self.emdb_id_nsprefix_ = None
@@ -1908,15 +1885,15 @@
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='entry_type'):
         if self.emdb_id is not None and 'emdb_id' not in already_processed:
             already_processed.add('emdb_id')
             outfile.write(' emdb_id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.emdb_id), input_name='emdb_id')), ))
-        if self.version != "3.0.4.2" and 'version' not in already_processed:
+        if self.version != "3.0.4.0" and 'version' not in already_processed:
             already_processed.add('version')
             outfile.write(' version=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.version), input_name='version')), ))
     def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='entry_type', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -15106,27 +15083,24 @@
 # end class software_list_type
 
 
 class software_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, name=None, version=None, category=None, processing_details=None, gds_collector_=None, **kwargs_):
+    def __init__(self, name=None, version=None, processing_details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.name = name
         self.name_nsprefix_ = None
         self.version = version
         self.version_nsprefix_ = None
-        self.category = category
-        self.validate_categoryType44(self.category)
-        self.category_nsprefix_ = None
         self.processing_details = processing_details
         self.processing_details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, software_type)
             if subclass is not None:
@@ -15144,42 +15118,22 @@
         return self.name
     def set_name(self, name):
         self.name = name
     def get_version(self):
         return self.version
     def set_version(self, version):
         self.version = version
-    def get_category(self):
-        return self.category
-    def set_category(self, category):
-        self.category = category
     def get_processing_details(self):
         return self.processing_details
     def set_processing_details(self, processing_details):
         self.processing_details = processing_details
-    def validate_categoryType44(self, value):
-        result = True
-        # Validate type categoryType44, a restriction on xs:token.
-        if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
-            if not isinstance(value, str):
-                lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
-                return False
-            value = value
-            enumerations = ['CLASSIFICATION', 'CRYSTALLOGRAPHY MERGING', 'CTF CORRECTION', 'DIFFRACTION INDEXING', 'EWALD SPHERE CORRECTION', 'FINAL EULER ASSIGNMENT', 'IMAGE ACQUISITION', 'INITIAL EULER ASSIGNMENT', 'LATTICE DISTORTION CORRECTION', 'LAYERLINE INDEXING', 'MASKING', 'MODEL FITTING', 'MODEL REFINEMENT', 'MOLECULAR REPLACEMENT', 'OTHER', 'PARTICLE SELECTION', 'RECONSTRUCTION', 'SERIES ALIGNMENT', 'SYMMETRY DETERMINATION', 'VOLUME SELECTION']
-            if value not in enumerations:
-                lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on categoryType44' % {"value" : encode_str_2_3(value), "lineno": lineno} )
-                result = False
-        return result
     def has__content(self):
         if (
             self.name is not None or
             self.version is not None or
-            self.category is not None or
             self.processing_details is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='software_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('software_type')
@@ -15215,18 +15169,14 @@
             namespaceprefix_ = self.name_nsprefix_ + ':' if (UseCapturedNS_ and self.name_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.name), input_name='name')), namespaceprefix_ , eol_))
         if self.version is not None:
             namespaceprefix_ = self.version_nsprefix_ + ':' if (UseCapturedNS_ and self.version_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sversion>%s</%sversion>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.version), input_name='version')), namespaceprefix_ , eol_))
-        if self.category is not None:
-            namespaceprefix_ = self.category_nsprefix_ + ':' if (UseCapturedNS_ and self.category_nsprefix_) else ''
-            showIndent(outfile, level, pretty_print)
-            outfile.write('<%scategory>%s</%scategory>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.category), input_name='category')), namespaceprefix_ , eol_))
         if self.processing_details is not None:
             namespaceprefix_ = self.processing_details_nsprefix_ + ':' if (UseCapturedNS_ and self.processing_details_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sprocessing_details>%s</%sprocessing_details>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.processing_details), input_name='processing_details')), namespaceprefix_ , eol_))
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
@@ -15257,26 +15207,14 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'version')
             value_ = self.gds_validate_string(value_, node, 'version')
             self.version = value_
             self.version_nsprefix_ = child_.prefix
-        elif nodeName_ == 'category':
-            value_ = child_.text
-            if value_:
-                value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
-            else:
-                value_ = ""
-            value_ = self.gds_parse_string(value_, node, 'category')
-            value_ = self.gds_validate_string(value_, node, 'category')
-            self.category = value_
-            self.category_nsprefix_ = child_.prefix
-            # validate type categoryType44
-            self.validate_categoryType44(self.category)
         elif nodeName_ == 'processing_details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'processing_details')
             value_ = self.gds_validate_string(value_, node, 'processing_details')
             self.processing_details = value_
             self.processing_details_nsprefix_ = child_.prefix
 # end class software_type
@@ -16751,15 +16689,15 @@
             obj_.original_tagname_ = 'sharpening'
         elif nodeName_ == 'b-factorSharpening':
             obj_ = b_factorSharpeningType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.b_factorSharpening = obj_
             obj_.original_tagname_ = 'b-factorSharpening'
         elif nodeName_ == 'other':
-            obj_ = otherType46.factory(parent_object_=self)
+            obj_ = otherType45.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.other = obj_
             obj_.original_tagname_ = 'other'
 # end class reconstruction_filtering_type
 
 
 class background_masked_type(GeneratedsSuper):
@@ -16904,15 +16842,15 @@
             value_ = self.gds_parse_string(value_, node, 'geometrical_shape')
             value_ = self.gds_validate_string(value_, node, 'geometrical_shape')
             self.geometrical_shape = value_
             self.geometrical_shape_nsprefix_ = child_.prefix
             # validate type geometrical_shapeType
             self.validate_geometrical_shapeType(self.geometrical_shape)
         elif nodeName_ == 'dimensions':
-            obj_ = dimensionsType47.factory(parent_object_=self)
+            obj_ = dimensionsType46.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.dimensions = obj_
             obj_.original_tagname_ = 'dimensions'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.software_list = obj_
@@ -18551,15 +18489,15 @@
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'phase_error_rejection_criteria')
             value_ = self.gds_validate_string(value_, node, 'phase_error_rejection_criteria')
             self.phase_error_rejection_criteria = value_
             self.phase_error_rejection_criteria_nsprefix_ = child_.prefix
         elif nodeName_ == 'high_resolution':
-            obj_ = high_resolutionType54.factory(parent_object_=self)
+            obj_ = high_resolutionType53.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.high_resolution = obj_
             obj_.original_tagname_ = 'high_resolution'
         elif nodeName_ == 'shell_list':
             obj_ = shell_listType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.shell_list = obj_
@@ -19365,15 +19303,15 @@
     def __init__(self, type_=None, projection_matching_processing=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.type_ = type_
-        self.validate_typeType57(self.type_)
+        self.validate_typeType56(self.type_)
         self.type__nsprefix_ = None
         self.projection_matching_processing = projection_matching_processing
         self.projection_matching_processing_nsprefix_ = None
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
@@ -19404,27 +19342,27 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def validate_typeType57(self, value):
+    def validate_typeType56(self, value):
         result = True
-        # Validate type typeType57, a restriction on xs:token.
+        # Validate type typeType56, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['ANGULAR RECONSTITUTION', 'COMMON LINE', 'NOT APPLICABLE', 'OTHER', 'PROJECTION MATCHING', 'RANDOM ASSIGNMENT', 'MAXIMUM LIKELIHOOD']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType57' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType56' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
     def has__content(self):
         if (
             self.type_ is not None or
             self.projection_matching_processing is not None or
             self.software_list is not None or
@@ -19497,16 +19435,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'type')
             value_ = self.gds_validate_string(value_, node, 'type')
             self.type_ = value_
             self.type_nsprefix_ = child_.prefix
-            # validate type typeType57
-            self.validate_typeType57(self.type_)
+            # validate type typeType56
+            self.validate_typeType56(self.type_)
         elif nodeName_ == 'projection_matching_processing':
             obj_ = projection_matching_processingType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.projection_matching_processing = obj_
             obj_.original_tagname_ = 'projection_matching_processing'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
@@ -20246,15 +20184,15 @@
             obj_.original_tagname_ = 'extraction'
         elif nodeName_ == 'ctf_correction':
             obj_ = ctf_correction_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.ctf_correction = obj_
             obj_.original_tagname_ = 'ctf_correction'
         elif nodeName_ == 'final_multi_reference_alignment':
-            obj_ = final_multi_reference_alignmentType61.factory(parent_object_=self)
+            obj_ = final_multi_reference_alignmentType60.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.final_multi_reference_alignment = obj_
             obj_.original_tagname_ = 'final_multi_reference_alignment'
         elif nodeName_ == 'final_three_d_classification':
             obj_ = classification_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.final_three_d_classification = obj_
@@ -21850,15 +21788,15 @@
     def __init__(self, file=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.file = file
-        self.validate_fileType66(self.file)
+        self.validate_fileType65(self.file)
         self.file_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, figure_type)
@@ -21877,28 +21815,28 @@
         return self.file
     def set_file(self, file):
         self.file = file
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def validate_fileType66(self, value):
+    def validate_fileType65(self, value):
         result = True
-        # Validate type fileType66, a restriction on xs:token.
+        # Validate type fileType65, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_fileType66_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType66_patterns_, ))
+                    self.validate_fileType65_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType65_patterns_, ))
                 result = False
         return result
-    validate_fileType66_patterns_ = [['^(emd_\\d{4,}.+)$']]
+    validate_fileType65_patterns_ = [['^(emd_\\d{4,}.+)$']]
     def has__content(self):
         if (
             self.file is not None or
             self.details is not None
         ):
             return True
         else:
@@ -21961,16 +21899,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'file')
             value_ = self.gds_validate_string(value_, node, 'file')
             self.file = value_
             self.file_nsprefix_ = child_.prefix
-            # validate type fileType66
-            self.validate_fileType66(self.file)
+            # validate type fileType65
+            self.validate_fileType65(self.file)
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class figure_type
@@ -21983,15 +21921,15 @@
     def __init__(self, file=None, details=None, extensiontype_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.file = file
-        self.validate_fileType67(self.file)
+        self.validate_fileType66(self.file)
         self.file_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
         self.extensiontype_ = extensiontype_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
@@ -22013,28 +21951,28 @@
         self.file = file
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
-    def validate_fileType67(self, value):
+    def validate_fileType66(self, value):
         result = True
-        # Validate type fileType67, a restriction on xs:token.
+        # Validate type fileType66, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_fileType67_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType67_patterns_, ))
+                    self.validate_fileType66_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType66_patterns_, ))
                 result = False
         return result
-    validate_fileType67_patterns_ = [['^(emd_\\d{4,}_fsc(_[1-9]{1,})*.xml)$']]
+    validate_fileType66_patterns_ = [['^(emd_\\d{4,}_fsc(_[1-9]{1,})*.xml)$']]
     def has__content(self):
         if (
             self.file is not None or
             self.details is not None
         ):
             return True
         else:
@@ -22108,16 +22046,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'file')
             value_ = self.gds_validate_string(value_, node, 'file')
             self.file = value_
             self.file_nsprefix_ = child_.prefix
-            # validate type fileType67
-            self.validate_fileType67(self.file)
+            # validate type fileType66
+            self.validate_fileType66(self.file)
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class validation_type
@@ -34878,29 +34816,29 @@
         self.angle = angle
     def add_angle(self, value):
         self.angle.append(value)
     def insert_angle_at(self, index, value):
         self.angle.insert(index, value)
     def replace_angle_at(self, index, value):
         self.angle[index] = value
-    def validate_angleType45(self, value):
+    def validate_angleType44(self, value):
         result = True
-        # Validate type angleType45, a restriction on xs:float.
+        # Validate type angleType44, a restriction on xs:float.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, float):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value < -70:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on angleType45' % {"value": value, "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on angleType44' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 70:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on angleType45' % {"value": value, "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on angleType44' % {"value": value, "lineno": lineno} )
                 result = False
         return result
     def has__content(self):
         if (
             self.angle
         ):
             return True
@@ -34956,16 +34894,16 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'angle' and child_.text:
             sval_ = child_.text
             fval_ = self.gds_parse_float(sval_, node, 'angle')
             fval_ = self.gds_validate_float(fval_, node, 'angle')
             self.angle.append(fval_)
             self.angle_nsprefix_ = child_.prefix
-            # validate type angleType45
-            self.validate_angleType45(self.angle[-1])
+            # validate type angleType44
+            self.validate_angleType44(self.angle[-1])
 # end class tilt_listType
 
 
 class axis2Type(axis_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = axis_type
@@ -36352,15 +36290,15 @@
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class _brestoreType
 
 
-class otherType46(GeneratedsSuper):
+class otherType45(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36369,21 +36307,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, otherType46)
+                CurrentSubclassModule_, otherType45)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if otherType46.subclass:
-            return otherType46.subclass(*args_, **kwargs_)
+        if otherType45.subclass:
+            return otherType45.subclass(*args_, **kwargs_)
         else:
-            return otherType46(*args_, **kwargs_)
+            return otherType45(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_software_list(self):
         return self.software_list
@@ -36397,40 +36335,40 @@
         if (
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType46', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('otherType46')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType45', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('otherType45')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'otherType46':
+        if self.original_tagname_ is not None and name_ == 'otherType45':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='otherType46')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='otherType45')
         if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='otherType46', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='otherType45', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='otherType46'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='otherType45'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType46', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType45', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.software_list is not None:
             namespaceprefix_ = self.software_list_nsprefix_ + ':' if (UseCapturedNS_ and self.software_list_nsprefix_) else ''
             self.software_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='software_list', pretty_print=pretty_print)
@@ -36459,18 +36397,18 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class otherType46
+# end class otherType45
 
 
-class dimensionsType47(GeneratedsSuper):
+class dimensionsType46(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, radius=None, width=None, height=None, depth=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36483,21 +36421,21 @@
         self.height = height
         self.height_nsprefix_ = None
         self.depth = depth
         self.depth_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, dimensionsType47)
+                CurrentSubclassModule_, dimensionsType46)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if dimensionsType47.subclass:
-            return dimensionsType47.subclass(*args_, **kwargs_)
+        if dimensionsType46.subclass:
+            return dimensionsType46.subclass(*args_, **kwargs_)
         else:
-            return dimensionsType47(*args_, **kwargs_)
+            return dimensionsType46(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_radius(self):
         return self.radius
@@ -36521,40 +36459,40 @@
             self.width is not None or
             self.height is not None or
             self.depth is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType47', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('dimensionsType47')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType46', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('dimensionsType46')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'dimensionsType47':
+        if self.original_tagname_ is not None and name_ == 'dimensionsType46':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='dimensionsType47')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='dimensionsType46')
         if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='dimensionsType47', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='dimensionsType46', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='dimensionsType47'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='dimensionsType46'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType47', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType46', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.radius is not None:
             namespaceprefix_ = self.radius_nsprefix_ + ':' if (UseCapturedNS_ and self.radius_nsprefix_) else ''
             self.radius.export(outfile, level, namespaceprefix_, namespacedef_='', name_='radius', pretty_print=pretty_print)
@@ -36583,29 +36521,29 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'radius':
             obj_ = radiusType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.radius = obj_
             obj_.original_tagname_ = 'radius'
         elif nodeName_ == 'width':
-            obj_ = widthType49.factory(parent_object_=self)
+            obj_ = widthType48.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.width = obj_
             obj_.original_tagname_ = 'width'
         elif nodeName_ == 'height':
-            obj_ = heightType51.factory(parent_object_=self)
+            obj_ = heightType50.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.height = obj_
             obj_.original_tagname_ = 'height'
         elif nodeName_ == 'depth':
             obj_ = depthType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.depth = obj_
             obj_.original_tagname_ = 'depth'
-# end class dimensionsType47
+# end class dimensionsType46
 
 
 class radiusType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
@@ -36634,26 +36572,26 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType48(self, value):
-        # Validate type unitsType48, a restriction on xs:token.
+    def validate_unitsType47(self, value):
+        # Validate type unitsType47, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType48' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType47' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
@@ -36698,21 +36636,21 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType48(self.units)    # validate type unitsType48
+            self.validate_unitsType47(self.units)    # validate type unitsType47
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class radiusType
 
 
-class widthType49(GeneratedsSuper):
+class widthType48(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36720,77 +36658,77 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, widthType49)
+                CurrentSubclassModule_, widthType48)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if widthType49.subclass:
-            return widthType49.subclass(*args_, **kwargs_)
+        if widthType48.subclass:
+            return widthType48.subclass(*args_, **kwargs_)
         else:
-            return widthType49(*args_, **kwargs_)
+            return widthType48(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType50(self, value):
-        # Validate type unitsType50, a restriction on xs:token.
+    def validate_unitsType49(self, value):
+        # Validate type unitsType49, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType50' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType49' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType49', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('widthType49')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType48', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('widthType48')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'widthType49':
+        if self.original_tagname_ is not None and name_ == 'widthType48':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='widthType49')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='widthType48')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='widthType49'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='widthType48'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType49', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType48', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -36802,21 +36740,21 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType50(self.units)    # validate type unitsType50
+            self.validate_unitsType49(self.units)    # validate type unitsType49
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class widthType49
+# end class widthType48
 
 
-class heightType51(GeneratedsSuper):
+class heightType50(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36824,77 +36762,77 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, heightType51)
+                CurrentSubclassModule_, heightType50)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if heightType51.subclass:
-            return heightType51.subclass(*args_, **kwargs_)
+        if heightType50.subclass:
+            return heightType50.subclass(*args_, **kwargs_)
         else:
-            return heightType51(*args_, **kwargs_)
+            return heightType50(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType52(self, value):
-        # Validate type unitsType52, a restriction on xs:token.
+    def validate_unitsType51(self, value):
+        # Validate type unitsType51, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType52' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType51' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType51', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('heightType51')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType50', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('heightType50')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'heightType51':
+        if self.original_tagname_ is not None and name_ == 'heightType50':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='heightType51')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='heightType50')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='heightType51'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='heightType50'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType51', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType50', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -36906,18 +36844,18 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType52(self.units)    # validate type unitsType52
+            self.validate_unitsType51(self.units)    # validate type unitsType51
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class heightType51
+# end class heightType50
 
 
 class depthType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
@@ -36946,26 +36884,26 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType53(self, value):
-        # Validate type unitsType53, a restriction on xs:token.
+    def validate_unitsType52(self, value):
+        # Validate type unitsType52, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType53' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType52' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
@@ -37010,15 +36948,15 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType53(self.units)    # validate type unitsType53
+            self.validate_unitsType52(self.units)    # validate type unitsType52
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class depthType
 
 
 class random_conical_tiltType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
@@ -38354,15 +38292,15 @@
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class low_resolutionType
 
 
-class high_resolutionType54(GeneratedsSuper):
+class high_resolutionType53(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38370,21 +38308,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, high_resolutionType54)
+                CurrentSubclassModule_, high_resolutionType53)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if high_resolutionType54.subclass:
-            return high_resolutionType54.subclass(*args_, **kwargs_)
+        if high_resolutionType53.subclass:
+            return high_resolutionType53.subclass(*args_, **kwargs_)
         else:
-            return high_resolutionType54(*args_, **kwargs_)
+            return high_resolutionType53(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -38408,39 +38346,39 @@
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType54')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType53', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType53')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'high_resolutionType54':
+        if self.original_tagname_ is not None and name_ == 'high_resolutionType53':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType54')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType53')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType54'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType53'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType53', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -38454,15 +38392,15 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class high_resolutionType54
+# end class high_resolutionType53
 
 
 class shell_listType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, shell=None, gds_collector_=None, **kwargs_):
@@ -38712,20 +38650,20 @@
         if value is not None and 'shell_id' not in already_processed:
             already_processed.add('shell_id')
             self.shell_id = self.gds_parse_integer(value, node, 'shell_id')
             if self.shell_id <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'high_resolution':
-            obj_ = high_resolutionType55.factory(parent_object_=self)
+            obj_ = high_resolutionType54.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.high_resolution = obj_
             obj_.original_tagname_ = 'high_resolution'
         elif nodeName_ == 'low_resolution':
-            obj_ = low_resolutionType56.factory(parent_object_=self)
+            obj_ = low_resolutionType55.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.low_resolution = obj_
             obj_.original_tagname_ = 'low_resolution'
         elif nodeName_ == 'number_structure_factors' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'number_structure_factors')
             if ival_ <= 0:
@@ -38750,15 +38688,15 @@
             fval_ = self.gds_parse_float(sval_, node, 'multiplicity')
             fval_ = self.gds_validate_float(fval_, node, 'multiplicity')
             self.multiplicity = fval_
             self.multiplicity_nsprefix_ = child_.prefix
 # end class shellType
 
 
-class high_resolutionType55(GeneratedsSuper):
+class high_resolutionType54(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38766,21 +38704,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, high_resolutionType55)
+                CurrentSubclassModule_, high_resolutionType54)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if high_resolutionType55.subclass:
-            return high_resolutionType55.subclass(*args_, **kwargs_)
+        if high_resolutionType54.subclass:
+            return high_resolutionType54.subclass(*args_, **kwargs_)
         else:
-            return high_resolutionType55(*args_, **kwargs_)
+            return high_resolutionType54(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -38804,39 +38742,39 @@
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType55', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType55')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType54')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'high_resolutionType55':
+        if self.original_tagname_ is not None and name_ == 'high_resolutionType54':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType55')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType54')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType55'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType54'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType55', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -38850,18 +38788,18 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class high_resolutionType55
+# end class high_resolutionType54
 
 
-class low_resolutionType56(GeneratedsSuper):
+class low_resolutionType55(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38869,21 +38807,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, low_resolutionType56)
+                CurrentSubclassModule_, low_resolutionType55)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if low_resolutionType56.subclass:
-            return low_resolutionType56.subclass(*args_, **kwargs_)
+        if low_resolutionType55.subclass:
+            return low_resolutionType55.subclass(*args_, **kwargs_)
         else:
-            return low_resolutionType56(*args_, **kwargs_)
+            return low_resolutionType55(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -38907,39 +38845,39 @@
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType56', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('low_resolutionType56')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType55', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('low_resolutionType55')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'low_resolutionType56':
+        if self.original_tagname_ is not None and name_ == 'low_resolutionType55':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='low_resolutionType56')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='low_resolutionType55')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='low_resolutionType56'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='low_resolutionType55'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType56', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType55', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -38953,15 +38891,15 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class low_resolutionType56
+# end class low_resolutionType55
 
 
 class segment_lengthType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
@@ -40202,15 +40140,15 @@
         elif nodeName_ == 'merit_function':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'merit_function')
             value_ = self.gds_validate_string(value_, node, 'merit_function')
             self.merit_function = value_
             self.merit_function_nsprefix_ = child_.prefix
         elif nodeName_ == 'angular_sampling':
-            obj_ = angular_samplingType58.factory(parent_object_=self)
+            obj_ = angular_samplingType57.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.angular_sampling = obj_
             obj_.original_tagname_ = 'angular_sampling'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.software_list = obj_
@@ -40220,15 +40158,15 @@
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class final_multi_reference_alignmentType
 
 
-class angular_samplingType58(GeneratedsSuper):
+class angular_samplingType57(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='degrees', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40236,21 +40174,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, angular_samplingType58)
+                CurrentSubclassModule_, angular_samplingType57)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if angular_samplingType58.subclass:
-            return angular_samplingType58.subclass(*args_, **kwargs_)
+        if angular_samplingType57.subclass:
+            return angular_samplingType57.subclass(*args_, **kwargs_)
         else:
-            return angular_samplingType58(*args_, **kwargs_)
+            return angular_samplingType57(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -40274,39 +40212,39 @@
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType58', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType58')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType57', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType57')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'angular_samplingType58':
+        if self.original_tagname_ is not None and name_ == 'angular_samplingType57':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType58')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType57')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType58'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType57'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType58', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType57', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -40320,18 +40258,18 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class angular_samplingType58
+# end class angular_samplingType57
 
 
-class final_multi_reference_alignmentType59(GeneratedsSuper):
+class final_multi_reference_alignmentType58(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_reference_projections=None, merit_function=None, angular_sampling=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40346,21 +40284,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, final_multi_reference_alignmentType59)
+                CurrentSubclassModule_, final_multi_reference_alignmentType58)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if final_multi_reference_alignmentType59.subclass:
-            return final_multi_reference_alignmentType59.subclass(*args_, **kwargs_)
+        if final_multi_reference_alignmentType58.subclass:
+            return final_multi_reference_alignmentType58.subclass(*args_, **kwargs_)
         else:
-            return final_multi_reference_alignmentType59(*args_, **kwargs_)
+            return final_multi_reference_alignmentType58(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_reference_projections(self):
         return self.number_reference_projections
@@ -40389,40 +40327,40 @@
             self.angular_sampling is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType59', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType59')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType58', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType58')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType59':
+        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType58':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType59')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType58')
         if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType59', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType58', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType59'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType58'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType59', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType58', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_reference_projections is not None:
             namespaceprefix_ = self.number_reference_projections_nsprefix_ + ':' if (UseCapturedNS_ and self.number_reference_projections_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40466,33 +40404,33 @@
         elif nodeName_ == 'merit_function':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'merit_function')
             value_ = self.gds_validate_string(value_, node, 'merit_function')
             self.merit_function = value_
             self.merit_function_nsprefix_ = child_.prefix
         elif nodeName_ == 'angular_sampling':
-            obj_ = angular_samplingType60.factory(parent_object_=self)
+            obj_ = angular_samplingType59.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.angular_sampling = obj_
             obj_.original_tagname_ = 'angular_sampling'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.software_list = obj_
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class final_multi_reference_alignmentType59
+# end class final_multi_reference_alignmentType58
 
 
-class angular_samplingType60(GeneratedsSuper):
+class angular_samplingType59(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='degrees', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40500,21 +40438,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, angular_samplingType60)
+                CurrentSubclassModule_, angular_samplingType59)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if angular_samplingType60.subclass:
-            return angular_samplingType60.subclass(*args_, **kwargs_)
+        if angular_samplingType59.subclass:
+            return angular_samplingType59.subclass(*args_, **kwargs_)
         else:
-            return angular_samplingType60(*args_, **kwargs_)
+            return angular_samplingType59(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -40538,39 +40476,39 @@
     def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType60', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType60')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType59', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType59')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'angular_samplingType60':
+        if self.original_tagname_ is not None and name_ == 'angular_samplingType59':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType60')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType59')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType60'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType59'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType60', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType59', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -40584,15 +40522,15 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class angular_samplingType60
+# end class angular_samplingType59
 
 
 class extractionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_tomograms=None, number_images_used=None, reference_model=None, method=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
@@ -40773,15 +40711,15 @@
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class extractionType
 
 
-class final_multi_reference_alignmentType61(GeneratedsSuper):
+class final_multi_reference_alignmentType60(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_reference_projections=None, merit_function=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40794,21 +40732,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, final_multi_reference_alignmentType61)
+                CurrentSubclassModule_, final_multi_reference_alignmentType60)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if final_multi_reference_alignmentType61.subclass:
-            return final_multi_reference_alignmentType61.subclass(*args_, **kwargs_)
+        if final_multi_reference_alignmentType60.subclass:
+            return final_multi_reference_alignmentType60.subclass(*args_, **kwargs_)
         else:
-            return final_multi_reference_alignmentType61(*args_, **kwargs_)
+            return final_multi_reference_alignmentType60(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_reference_projections(self):
         return self.number_reference_projections
@@ -40832,40 +40770,40 @@
             self.merit_function is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType61', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType61')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType60', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType60')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType61':
+        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType60':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType61')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType60')
         if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType61', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType60', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType61'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType60'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType61', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType60', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_reference_projections is not None:
             namespaceprefix_ = self.number_reference_projections_nsprefix_ + ':' if (UseCapturedNS_ and self.number_reference_projections_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40916,18 +40854,18 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class final_multi_reference_alignmentType61
+# end class final_multi_reference_alignmentType60
 
 
-class extractionType62(GeneratedsSuper):
+class extractionType61(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_tomograms=None, number_images_used=None, reference_model=None, method=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40944,21 +40882,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, extractionType62)
+                CurrentSubclassModule_, extractionType61)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if extractionType62.subclass:
-            return extractionType62.subclass(*args_, **kwargs_)
+        if extractionType61.subclass:
+            return extractionType61.subclass(*args_, **kwargs_)
         else:
-            return extractionType62(*args_, **kwargs_)
+            return extractionType61(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_tomograms(self):
         return self.number_tomograms
@@ -40992,40 +40930,40 @@
             self.method is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType62', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('extractionType62')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType61', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('extractionType61')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'extractionType62':
+        if self.original_tagname_ is not None and name_ == 'extractionType61':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='extractionType62')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='extractionType61')
         if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='extractionType62', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='extractionType61', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='extractionType62'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='extractionType61'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType62', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType61', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_tomograms is not None:
             namespaceprefix_ = self.number_tomograms_nsprefix_ + ':' if (UseCapturedNS_ and self.number_tomograms_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41102,18 +41040,18 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class extractionType62
+# end class extractionType61
 
 
-class final_multi_reference_alignmentType63(GeneratedsSuper):
+class final_multi_reference_alignmentType62(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_reference_projections=None, merit_function=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -41126,21 +41064,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, final_multi_reference_alignmentType63)
+                CurrentSubclassModule_, final_multi_reference_alignmentType62)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if final_multi_reference_alignmentType63.subclass:
-            return final_multi_reference_alignmentType63.subclass(*args_, **kwargs_)
+        if final_multi_reference_alignmentType62.subclass:
+            return final_multi_reference_alignmentType62.subclass(*args_, **kwargs_)
         else:
-            return final_multi_reference_alignmentType63(*args_, **kwargs_)
+            return final_multi_reference_alignmentType62(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_reference_projections(self):
         return self.number_reference_projections
@@ -41164,40 +41102,40 @@
             self.merit_function is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType63', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType63')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType62', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType62')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType63':
+        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType62':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType63')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType62')
         if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType63', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType62', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType63'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType62'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType63', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType62', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_reference_projections is not None:
             namespaceprefix_ = self.number_reference_projections_nsprefix_ + ':' if (UseCapturedNS_ and self.number_reference_projections_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41248,15 +41186,15 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class final_multi_reference_alignmentType63
+# end class final_multi_reference_alignmentType62
 
 
 class resolutionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', res_type=None, valueOf_=None, gds_collector_=None, **kwargs_):
@@ -42698,15 +42636,15 @@
     def __init__(self, file=None, details=None, mask_details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.file = file
-        self.validate_fileType64(self.file)
+        self.validate_fileType63(self.file)
         self.file_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
         self.mask_details = mask_details
         self.mask_details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
@@ -42731,28 +42669,28 @@
         return self.details
     def set_details(self, details):
         self.details = details
     def get_mask_details(self):
         return self.mask_details
     def set_mask_details(self, mask_details):
         self.mask_details = mask_details
-    def validate_fileType64(self, value):
+    def validate_fileType63(self, value):
         result = True
-        # Validate type fileType64, a restriction on xs:token.
+        # Validate type fileType63, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_fileType64_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType64_patterns_, ))
+                    self.validate_fileType63_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType63_patterns_, ))
                 result = False
         return result
-    validate_fileType64_patterns_ = [['^([emd_\\d{4,}]+.*)$']]
+    validate_fileType63_patterns_ = [['^([emd_\\d{4,}]+.*)$']]
     def has__content(self):
         if (
             self.file is not None or
             self.details is not None or
             self.mask_details is not None
         ):
             return True
@@ -42819,16 +42757,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'file')
             value_ = self.gds_validate_string(value_, node, 'file')
             self.file = value_
             self.file_nsprefix_ = child_.prefix
-            # validate type fileType64
-            self.validate_fileType64(self.file)
+            # validate type fileType63
+            self.validate_fileType63(self.file)
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
         elif nodeName_ == 'mask_details':
@@ -43285,15 +43223,15 @@
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.chain_id = chain_id
         self.chain_id_nsprefix_ = None
         self.residue_range = residue_range
-        self.validate_residue_rangeType65(self.residue_range)
+        self.validate_residue_rangeType64(self.residue_range)
         self.residue_range_nsprefix_ = None
         self.number_of_copies_in_final_model = number_of_copies_in_final_model
         self.number_of_copies_in_final_model_nsprefix_ = None
         self.source_name = source_name
         self.validate_source_nameType(self.source_name)
         self.source_name_nsprefix_ = None
         self.initial_model_type = initial_model_type
@@ -43330,28 +43268,28 @@
         return self.source_name
     def set_source_name(self, source_name):
         self.source_name = source_name
     def get_initial_model_type(self):
         return self.initial_model_type
     def set_initial_model_type(self, initial_model_type):
         self.initial_model_type = initial_model_type
-    def validate_residue_rangeType65(self, value):
+    def validate_residue_rangeType64(self, value):
         result = True
-        # Validate type residue_rangeType65, a restriction on xs:token.
+        # Validate type residue_rangeType64, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_residue_rangeType65_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_residue_rangeType65_patterns_, ))
+                    self.validate_residue_rangeType64_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_residue_rangeType64_patterns_, ))
                 result = False
         return result
-    validate_residue_rangeType65_patterns_ = [['^(\\d+-\\d+)$']]
+    validate_residue_rangeType64_patterns_ = [['^(\\d+-\\d+)$']]
     def validate_source_nameType(self, value):
         result = True
         # Validate type source_nameType, a restriction on xs:string.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
@@ -43469,16 +43407,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'residue_range')
             value_ = self.gds_validate_string(value_, node, 'residue_range')
             self.residue_range = value_
             self.residue_range_nsprefix_ = child_.prefix
-            # validate type residue_rangeType65
-            self.validate_residue_rangeType65(self.residue_range)
+            # validate type residue_rangeType64
+            self.validate_residue_rangeType64(self.residue_range)
         elif nodeName_ == 'number_of_copies_in_final_model' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'number_of_copies_in_final_model')
             if ival_ <= 0:
                 raise_parse_error(child_, 'requires positiveInteger')
             ival_ = self.gds_validate_integer(ival_, node, 'number_of_copies_in_final_model')
             self.number_of_copies_in_final_model = ival_
@@ -44253,16 +44191,16 @@
     "admin_type",
     "alignment_procedureType",
     "amplitude_correctionType",
     "angleType",
     "angle_assignment_type",
     "angle_incrementType",
     "angular_samplingType",
-    "angular_samplingType58",
-    "angular_samplingType60",
+    "angular_samplingType57",
+    "angular_samplingType59",
     "annotatorType",
     "applied_symmetry_type",
     "author_ORCID_type",
     "author_order_type",
     "authors_listType",
     "auxiliary_link_listType",
     "auxiliary_link_type",
@@ -44326,15 +44264,15 @@
     "data_completeness",
     "delta_phiType",
     "delta_zType",
     "depthType",
     "diameterType",
     "digitization_detailsType",
     "dimensionsType",
-    "dimensionsType47",
+    "dimensionsType46",
     "discrepancy_listType",
     "discrepancy_listType19",
     "discrepancy_listType23",
     "discrepancy_listType28",
     "dna_macromolecule_type",
     "em_label_macromolecule_type",
     "emdb_cross_reference_list_type",
@@ -44348,15 +44286,15 @@
     "external_referencesType16",
     "external_referencesType21",
     "external_referencesType25",
     "external_referencesType30",
     "external_referencesType35",
     "external_referencesType4",
     "extractionType",
-    "extractionType62",
+    "extractionType61",
     "fib_current_type",
     "fib_dose_rate_type",
     "fib_duration_type",
     "fib_final_thickness_type",
     "fib_initial_thickness_type",
     "fib_voltage_type",
     "fiducial_marker_diameter_type",
@@ -44365,52 +44303,52 @@
     "figure_listType",
     "figure_type",
     "film_or_detector_modelType",
     "film_thicknessType",
     "film_type",
     "final_modelType",
     "final_multi_reference_alignmentType",
-    "final_multi_reference_alignmentType59",
-    "final_multi_reference_alignmentType61",
-    "final_multi_reference_alignmentType63",
+    "final_multi_reference_alignmentType58",
+    "final_multi_reference_alignmentType60",
+    "final_multi_reference_alignmentType62",
     "final_reconstruction_type",
     "focused_ion_beamType",
     "fsc_curve_validation_type",
     "grant_reference_type",
     "grant_supportType",
     "grid_pretreatment_type",
     "grid_type",
     "half_map_listType",
     "heightType",
-    "heightType51",
+    "heightType50",
     "helical_microscopy_type",
     "helical_parameters_type",
     "helical_preparation_type",
     "helical_processing_type",
     "helix_lengthType",
     "high_frequency_cutoffType",
     "high_pressure_freezingType",
     "high_resolutionType",
+    "high_resolutionType53",
     "high_resolutionType54",
-    "high_resolutionType55",
     "image_recordingType",
     "image_recording_listType",
     "indexingType",
     "initial_modelType",
     "integer_vector_map_type",
     "interpretation_type",
     "journal_citation",
     "key_datesType",
     "layer_lines_type",
     "layer_lines_validation_type",
     "legacyType",
     "ligand_macromolecule_type",
     "low_frequency_cutoffType",
     "low_resolutionType",
-    "low_resolutionType56",
+    "low_resolutionType55",
     "lower_energy_thresholdType",
     "macromoleculeType",
     "macromolecule_listType",
     "macromolecule_list_type",
     "macromolecule_source_type",
     "macromolecules_and_complexes_type",
     "map_statistics_type",
@@ -44439,15 +44377,15 @@
     "organelle_or_cellular_component_supramolecule_type",
     "organelle_source_type",
     "organism_type",
     "organizationType",
     "originType",
     "orthogonal_tiltType",
     "otherType",
-    "otherType46",
+    "otherType45",
     "other_macromolecule_type",
     "parallel_resolution",
     "particle_selection_type",
     "pdb_cross_reference_list_type",
     "pdb_cross_reference_type",
     "pdb_model_type",
     "perpendicular_resolution",
@@ -44547,10 +44485,10 @@
     "virus_shellType",
     "virus_species_name_type",
     "virus_supramolecule_type",
     "vitrification_type",
     "weighted_phase_residual",
     "weighted_r_factor",
     "widthType",
-    "widthType49",
+    "widthType48",
     "zemlin_tableauType"
 ]
```

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 1% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.4.1/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.4.1"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.4.0"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -2509,40 +2509,14 @@
       <xs:element name="software" type="software_type" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="software_type">
     <xs:sequence>
       <xs:element name="name" type="xs:token" minOccurs="0"/>
       <xs:element name="version" type="xs:token" minOccurs="0"/>
-      <xs:element name="category" minOccurs="0">
-        <xs:simpleType>
-          <xs:restriction base="xs:token">
-            <xs:enumeration value="CLASSIFICATION"/>
-            <xs:enumeration value="CRYSTALLOGRAPHY MERGING"/>
-            <xs:enumeration value="CTF CORRECTION"/>
-            <xs:enumeration value="DIFFRACTION INDEXING"/>
-            <xs:enumeration value="EWALD SPHERE CORRECTION"/>
-            <xs:enumeration value="FINAL EULER ASSIGNMENT"/>
-            <xs:enumeration value="IMAGE ACQUISITION"/>
-            <xs:enumeration value="INITIAL EULER ASSIGNMENT"/>
-            <xs:enumeration value="LATTICE DISTORTION CORRECTION"/>
-            <xs:enumeration value="LAYERLINE INDEXING"/>
-            <xs:enumeration value="MASKING"/>
-            <xs:enumeration value="MODEL FITTING"/>
-            <xs:enumeration value="MODEL REFINEMENT"/>
-            <xs:enumeration value="MOLECULAR REPLACEMENT"/>
-            <xs:enumeration value="OTHER"/>
-            <xs:enumeration value="PARTICLE SELECTION"/>
-            <xs:enumeration value="RECONSTRUCTION"/>
-            <xs:enumeration value="SERIES ALIGNMENT"/>
-            <xs:enumeration value="SYMMETRY DETERMINATION"/>
-            <xs:enumeration value="VOLUME SELECTION"/>
-          </xs:restriction>
-        </xs:simpleType>
-      </xs:element>
       <xs:element name="processing_details" type="xs:string" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
   <xs:simpleType name="allowed_film_or_detector_model">
     <xs:restriction base="xs:token">
       <xs:enumeration value="AGFA SCIENTA FILM"/>
       <xs:enumeration value="DIRECT ELECTRON APOLLO (4k x 4k)"/>
```

### Comparing `wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.4
+Version: 1.4.1
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.4.1/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

