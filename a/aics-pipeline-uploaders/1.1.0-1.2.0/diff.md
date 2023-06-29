# Comparing `tmp/aics_pipeline_uploaders-1.1.0.tar.gz` & `tmp/aics_pipeline_uploaders-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aics_pipeline_uploaders-1.1.0.tar", last modified: Wed Jan 11 22:13:17 2023, max compression
+gzip compressed data, was "aics_pipeline_uploaders-1.2.0.tar", last modified: Thu Jun 29 21:02:32 2023, max compression
```

## Comparing `aics_pipeline_uploaders-1.1.0.tar` & `aics_pipeline_uploaders-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.713113 aics_pipeline_uploaders-1.1.0/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     1951 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.1.0/LICENSE
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)       34 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.1.0/MANIFEST.in
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     3325 2023-01-11 22:13:17.714759 aics_pipeline_uploaders-1.1.0/PKG-INFO
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     2794 2023-01-11 22:12:16.000000 aics_pipeline_uploaders-1.1.0/README.md
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.591152 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)      494 2023-01-11 22:12:16.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/__init__.py
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.654942 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/bin/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)       78 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/bin/__init__.py
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     1236 2023-01-11 22:12:16.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/celigo_uploader.py
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)      930 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/drug_uploader.py
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)    13098 2023-01-06 20:51:45.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/emt_uploader.py
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     7541 2023-01-06 20:47:04.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/fms_uploader.py
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.665655 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/tests/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)       78 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/tests/__init__.py
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.685406 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)       31 2023-01-10 18:56:39.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/__init__.py
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     2099 2023-01-11 22:12:16.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/celigo.py
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.704961 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/test/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-10 18:56:39.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/test/__init__.py
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     3077 2023-01-11 22:12:16.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/test/test_celigo.py
-drwxrwxrwx   0 brian.whitney (20256) domain users (10513)        0 2023-01-11 22:13:17.643324 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     3325 2023-01-11 22:13:17.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/PKG-INFO
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)      745 2023-01-11 22:13:17.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/SOURCES.txt
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)        1 2023-01-11 22:13:17.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/dependency_links.txt
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)      379 2023-01-11 22:13:17.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/requires.txt
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)       24 2023-01-11 22:13:17.000000 aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/top_level.txt
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     1353 2023-01-11 22:12:16.000000 aics_pipeline_uploaders-1.1.0/pyproject.toml
--rwxrwxrwx   0 brian.whitney (20256) domain users (10513)     1026 2023-01-11 22:13:17.723703 aics_pipeline_uploaders-1.1.0/setup.cfg
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.557146 aics_pipeline_uploaders-1.2.0/
+----------   0 brian.whitney (20256) domain users (10513)     1951 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.2.0/LICENSE
+----------   0 brian.whitney (20256) domain users (10513)       34 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.2.0/MANIFEST.in
+----------   0 brian.whitney (20256) domain users (10513)     3325 2023-06-29 21:02:32.562017 aics_pipeline_uploaders-1.2.0/PKG-INFO
+----------   0 brian.whitney (20256) domain users (10513)     2794 2023-06-29 20:51:42.000000 aics_pipeline_uploaders-1.2.0/README.md
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.255710 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/
+----------   0 brian.whitney (20256) domain users (10513)      524 2023-06-29 20:51:42.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/__init__.py
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.416622 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/bin/
+----------   0 brian.whitney (20256) domain users (10513)       78 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/bin/__init__.py
+----------   0 brian.whitney (20256) domain users (10513)     1133 2023-06-29 20:43:36.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/celigo_uploader.py
+----------   0 brian.whitney (20256) domain users (10513)      930 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/drug_uploader.py
+----------   0 brian.whitney (20256) domain users (10513)    13276 2023-01-13 22:33:16.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/emt_uploader.py
+----------   0 brian.whitney (20256) domain users (10513)     7725 2023-01-13 22:27:08.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/fms_uploader.py
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.440108 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/tests/
+----------   0 brian.whitney (20256) domain users (10513)       78 2022-09-30 18:52:07.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/tests/__init__.py
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.486714 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/
+----------   0 brian.whitney (20256) domain users (10513)       31 2023-01-10 18:56:39.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/__init__.py
+----------   0 brian.whitney (20256) domain users (10513)     2636 2023-01-13 22:21:32.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/celigo.py
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.535572 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/test/
+----------   0 brian.whitney (20256) domain users (10513)        0 2023-01-10 18:56:39.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/test/__init__.py
+----------   0 brian.whitney (20256) domain users (10513)     5014 2023-01-13 22:23:48.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/test/test_celigo.py
+d---------   0 brian.whitney (20256) domain users (10513)        0 2023-06-29 21:02:32.386744 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/
+----------   0 brian.whitney (20256) domain users (10513)     3325 2023-06-29 21:02:31.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/PKG-INFO
+----------   0 brian.whitney (20256) domain users (10513)      745 2023-06-29 21:02:31.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/SOURCES.txt
+----------   0 brian.whitney (20256) domain users (10513)        1 2023-06-29 21:02:31.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/dependency_links.txt
+----------   0 brian.whitney (20256) domain users (10513)      379 2023-06-29 21:02:31.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/requires.txt
+----------   0 brian.whitney (20256) domain users (10513)       24 2023-06-29 21:02:31.000000 aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/top_level.txt
+----------   0 brian.whitney (20256) domain users (10513)     1353 2023-06-29 21:01:38.000000 aics_pipeline_uploaders-1.2.0/pyproject.toml
+----------   0 brian.whitney (20256) domain users (10513)     1026 2023-06-29 21:02:32.580066 aics_pipeline_uploaders-1.2.0/setup.cfg
```

### Comparing `aics_pipeline_uploaders-1.1.0/LICENSE` & `aics_pipeline_uploaders-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aics_pipeline_uploaders-1.1.0/PKG-INFO` & `aics_pipeline_uploaders-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aics_pipeline_uploaders
-Version: 1.1.0
+Version: 1.2.0
 Summary: This package contains resources for uploading pipeline data to FMS
 Author-email: AICS <!AICS_SW@alleninstitute.org>
 Project-URL: homepage, https://github.com/aics-int/aics_pipeline_uploaders
 Project-URL: documentation, https://aics-int.github.io/aics_pipeline_uploaders
 Project-URL: repository, https://github.com/aics-int/aics_pipeline_uploaders
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 [![Build Status](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/workflows/Build%20Main/badge.svg)](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/actions)
 [![Documentation](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/workflows/Documentation/badge.svg)](https://BrianWhitneyAI.github.io/aics_pipeline_uploaders/)
 [![Code Coverage](https://codecov.io/gh/BrianWhitneyAI/aics_pipeline_uploaders/branch/main/graph/badge.svg)](https://codecov.io/gh/BrianWhitneyAI/aics_pipeline_uploaders)
 
 This package contains resources for uploading pipeline data to FMS
 
-aics_pipeline_uploaders==1.1.0
+aics_pipeline_uploaders==1.2.0
 ---
 ## Features
 
 -   Store values and retain the prior value in memory
 -   ... some other functionality
 
 ## Installation
```

### Comparing `aics_pipeline_uploaders-1.1.0/README.md` & `aics_pipeline_uploaders-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![Build Status](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/workflows/Build%20Main/badge.svg)](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/actions)
 [![Documentation](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/workflows/Documentation/badge.svg)](https://BrianWhitneyAI.github.io/aics_pipeline_uploaders/)
 [![Code Coverage](https://codecov.io/gh/BrianWhitneyAI/aics_pipeline_uploaders/branch/main/graph/badge.svg)](https://codecov.io/gh/BrianWhitneyAI/aics_pipeline_uploaders)
 
 This package contains resources for uploading pipeline data to FMS
 
-aics_pipeline_uploaders==1.1.0
+aics_pipeline_uploaders==1.2.0
 ---
 ## Features
 
 -   Store values and retain the prior value in memory
 -   ... some other functionality
 
 ## Installation
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/celigo_uploader.py` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/celigo_uploader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from pathlib import Path
-
-from aicsfiles import FileManagementSystem
+from typing import Literal
 
 from .fms_uploader import FMSUploader
 from .util.celigo import CeligoUtil
 
 # Example file name "3500001609_Scan_1-12-2018-6-03-16-AM_Well_F5_Ch1_-1um.tiff"
 
 
 class CeligoUploader(FMSUploader):
-    def __init__(self, file_path: str, file_type: str, env: str = "stg"):
+    def __init__(
+        self, file_path: str, file_type: str, env: Literal["prod", "stg", "dev"] = "stg"
+    ):
 
-        self.file_path = Path(file_path)
-        self.file_type = file_type
-        self.file_name = self.file_path.name
+        super().__init__(file_path=file_path, file_type=file_type, env=env)
 
         # Get Metadata from filename
-        util = CeligoUtil(env)
+        util = CeligoUtil(self.env)
+
         (
             self.plate_barcode,
             self.well_name,
             self.scan_date,
             self.scan_timeutil,
         ) = util.parse_filename(self.file_name)
         self.well_id = util.lookup_well_id(self.plate_barcode, self.well_name)
 
-        # Build fms object
-        fms = FileManagementSystem()
-        builder = fms.create_file_metadata_builder()
+        builder = self.fms.create_file_metadata_builder()
         builder.add_annotation("Well", self.well_id).add_annotation(
             "Plate Barcode", self.plate_barcode
         ).add_annotation("Celigo Scan Time", self.scan_timeutil).add_annotation(
             "Celigo Scan Date", self.scan_date
         )
 
         self.metadata = builder.build()
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/drug_uploader.py` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/drug_uploader.py`

 * *Files identical despite different names*

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/emt_uploader.py` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/emt_uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import List
+from typing import List, Literal
 import xml.etree.ElementTree as ET
 from xml.etree.ElementTree import (
     tostring as xml_to_string,
 )
 
 from aicsfiles import FileManagementSystem
 from aicsimageio import AICSImage
@@ -23,15 +23,15 @@
 
         NOTE: Super class for uploaders
         NOTE: look into helper constructor
 """
 
 
 class EMTUploader:
-    def __init__(self, dir_path: str, env="stg"):
+    def __init__(self, dir_path: str, env: Literal["prod", "stg", "dev"] = "stg"):
 
         BLOCK = "AcquisitionBlock"
         self.env = env
         self.barcode = int(
             Path(dir_path).name.split("_")[0]
         )  # this is oversimplified at moment
         self.files = []  # This is where files + metadata go
@@ -176,19 +176,19 @@
 
     @staticmethod
     def block_metadata_formatter(
         barcode: int,
         filename: str,
         file_type: str,
         well_ids: List[int],
-        env: str,
         imaging_date: str,
         scene_map: List[str],
         optical_control_id: str,
         timepoint: int,
+        env: Literal["prod", "stg", "dev"] = "stg",
     ):
 
         fms = FileManagementSystem(env="stg")
         builder = fms.create_file_metadata_builder()
         builder.add_annotation("Well", well_ids).add_annotation(
             "Plate Barcode", barcode
         ).add_annotation("Optical Control ID", optical_control_id).add_annotation(
@@ -218,18 +218,18 @@
 
     @staticmethod
     def wellscan_metadata_formatter(
         barcode: int,
         filename: str,
         file_type: str,
         well_ids: List[int],
-        env: str,
         imaging_date: str,
         scene_map: List[str],
         optical_control_id: str,
+        env: Literal["prod", "stg", "dev"] = "stg",
     ):
 
         fms = FileManagementSystem(env="stg")
         builder = fms.create_file_metadata_builder()
         builder.add_annotation("Well", well_ids).add_annotation(
             "Plate Barcode", barcode
         ).add_annotation("Optical Control ID", optical_control_id)
@@ -257,17 +257,17 @@
 
     @staticmethod
     def czmbi_metadata_formatter(
         barcode: int,
         filename: str,
         file_type: str,
         well_ids: List[int],
-        env: str,
         imaging_date: str,
         scene_map: List[str],
+        env: Literal["prod", "stg", "dev"] = "stg",
     ):
 
         fms = FileManagementSystem(env="stg")
         builder = fms.create_file_metadata_builder()
         builder.add_annotation("Well", well_ids).add_annotation(
             "Plate Barcode", barcode
         )
@@ -295,17 +295,17 @@
 
     @staticmethod
     def czexp_metadata_formatter(
         barcode: int,
         filename: str,
         file_type: str,
         well_ids: List[int],
-        env: str,
         imaging_date: str,
         scene_map: List[str],
+        env: Literal["prod", "stg", "dev"] = "stg",
     ):
 
         fms = FileManagementSystem(env="stg")
         builder = fms.create_file_metadata_builder()
         builder.add_annotation("Well", well_ids).add_annotation(
             "Plate Barcode", barcode
         )
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/fms_uploader.py` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/fms_uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import os
 from pathlib import Path
 import subprocess
+from typing import Literal
 import xml.etree.ElementTree as ET
 from xml.etree.ElementTree import (
     tostring as xml_to_string,
 )
 
 from aicsfiles import FileManagementSystem
 from aicsimageio import AICSImage
@@ -40,31 +41,37 @@
     "ZSD2": "ZSD-2",
     "ZSD3": "ZSD-3"
     # More systems ...
 }
 
 
 class FMSUploader:
-    def __init__(self, file_path: str, file_type: str, metadata: dict, env="stg"):
+    def __init__(
+        self,
+        file_path: str,
+        file_type: str,
+        metadata: dict = None,
+        env: Literal["prod", "stg", "dev"] = "stg",
+    ):
 
         self.env = env
         self.file_path = Path(file_path)
         self.file_type = file_type
         self.metadata = metadata
+        self.file_name = self.file_path.name
+        self.fms = FileManagementSystem.from_env(env=self.env)
 
     def upload(self):
-        fms = FileManagementSystem(env=self.env)
-
         run_count = 0
         while run_count < 3:
             try:
-                fms_file = fms.upload_v2_file(
+                fms_file = self.fms.upload_file(
                     file_reference=self.file_path,
                     file_type=self.file_type,
-                    metadata=self.metadata,
+                    annotations=self.metadata,
                 )
                 self.fms_ID = fms_file.id
                 run_count = 3
             except requests.exceptions.ReadTimeout:
                 print("ReadTimeout, retrying")
                 run_count = run_count + 1
                 continue
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/celigo.py` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/celigo.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,21 +16,33 @@
     def __init__(self, env: str = "stg"):
         self.env = env
 
     def lookup_well_id(self, plate_barcode, well_name):
         url = ENV_SERVICE_MAP[self.env][SERVICE_MMS][MMS_RESOURCE_PLATE_INFO] + str(
             plate_barcode
         )
-        well_info_response = requests.get(url)
-        well_info = well_info_response.json()
-        if len(well_info["data"]) > 1:
-            raise Exception(f"Barcode {plate_barcode} is used by more than one plate.")
-        well_name_lookup = well_info["data"][0]["wellNameLookup"]
-
-        return well_name_lookup[well_name]["wellId"]
+        response: requests.Response = requests.get(url)
+        if response.status_code == 404:
+            return None
+        elif response.status_code == 200:
+            barcode_info = response.json()
+            if len(barcode_info["data"]) > 1:
+                raise BarcodeException(
+                    f"Barcode {plate_barcode} is used by more than one plate."
+                )
+            well_name_lookup = barcode_info["data"][0]["wellNameLookup"]
+            if well_name in well_name_lookup:
+                well_id = well_name_lookup[well_name]["wellId"]
+            else:
+                well_id = None
+            return well_id
+        else:
+            raise MMSException(
+                f"Error requesting barcode info from MMS: {response.status_code}"
+            )
 
     def parse_filename(self, file_name):
         raw_metadata = file_name.split("_")
         plate_barcode = int(raw_metadata[0])
         well_name = raw_metadata[4]
         scan_date_time_parts = raw_metadata[2].split("-")
         hours = int(scan_date_time_parts[3])
@@ -49,7 +61,15 @@
         standardized_scan_date_time_parts = scan_date_time.isoformat(
             timespec="auto"
         ).split("T")
         scan_time = standardized_scan_date_time_parts[1]
         scan_date = standardized_scan_date_time_parts[0]
 
         return plate_barcode, well_name, scan_date, scan_time
+
+
+class BarcodeException(Exception):
+    pass
+
+
+class MMSException(Exception):
+    pass
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders/util/test/test_celigo.py` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders/util/test/test_celigo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import json
 
 import pytest
 import requests_mock
 
+from aics_pipeline_uploaders.util.celigo import (
+    BarcodeException,
+    MMSException,
+)
+
 from ...util import CeligoUtil
 
 
 def test_parse_filename() -> None:
     util = CeligoUtil("stg")
     filename = "3500001609_Scan_1-12-2018-6-03-16-AM_Well_F5_Ch1_-1um.tiff"
     plate_barcode, well_name, scan_date, scan_time = util.parse_filename(filename)
     assert plate_barcode == 3500001609
     assert well_name == "F5"
     assert scan_date == "2018-01-12"
     assert scan_time == "06:03:16"
 
 
-def test_lookup_well_id_raises() -> None:
+def test_lookup_well_id_multiple_plates() -> None:
     util = CeligoUtil("stg")
 
     with requests_mock.Mocker() as mock_request:
         mms_url = "http://stg-aics-api.corp.alleninstitute.org/metadata-management-service/1.0/plate/query?barcode=9999999999"  # noqa: E501
         mms_resp = {
             "data": [
                 {
@@ -54,19 +59,38 @@
                             "solutions": [],
                         },
                     },
                 },
             ]
         }
         mock_request.get(mms_url, text=json.dumps(mms_resp))
-        with pytest.raises(Exception):
-            util.lookup_well_id("3500001609", "A5")
+        with pytest.raises(BarcodeException):
+            util.lookup_well_id("9999999999", "A5")
 
 
-def test_lookup_well_id() -> None:
+def test_lookup_well_id_404() -> None:
+    util = CeligoUtil("stg")
+
+    with requests_mock.Mocker() as mock_request:
+        mms_url = "http://stg-aics-api.corp.alleninstitute.org/metadata-management-service/1.0/plate/query?barcode=9999999999"  # noqa: E501
+        mock_request.get(mms_url, status_code=404)
+        assert None is util.lookup_well_id("9999999999", "A5")
+
+
+def test_lookup_well_id_500() -> None:
+    util = CeligoUtil("stg")
+
+    with requests_mock.Mocker() as mock_request:
+        mms_url = "http://stg-aics-api.corp.alleninstitute.org/metadata-management-service/1.0/plate/query?barcode=9999999999"  # noqa: E501
+        mock_request.get(mms_url, status_code=500)
+        with pytest.raises(MMSException):
+            util.lookup_well_id("9999999999", "A5")
+
+
+def test_lookup_well_id_success() -> None:
     util = CeligoUtil("stg")
     mms_url = "http://stg-aics-api.corp.alleninstitute.org/metadata-management-service/1.0/plate/query?barcode=9999999999"  # noqa: E501
     mms_resp = {
         "data": [
             {
                 "wellNameLookup": {
                     "A6": {
@@ -87,7 +111,38 @@
             }
         ]
     }
     with requests_mock.Mocker() as mock_request:
         mock_request.get(mms_url, text=json.dumps(mms_resp))
         well_id = util.lookup_well_id("9999999999", "A5")
         assert well_id == 10
+
+
+def test_lookup_well_id_no_well_name() -> None:
+    util = CeligoUtil("stg")
+    mms_url = "http://stg-aics-api.corp.alleninstitute.org/metadata-management-service/1.0/plate/query?barcode=9999999999"  # noqa: E501
+    mms_resp = {
+        "data": [
+            {
+                "wellNameLookup": {
+                    "A6": {
+                        "wellId": 10,
+                        "row": 0,
+                        "col": 5,
+                        "cellPopulations": [],
+                        "solutions": [],
+                    },
+                    "A5": {
+                        "wellId": 11,
+                        "row": 0,
+                        "col": 4,
+                        "cellPopulations": [],
+                        "solutions": [],
+                    },
+                }
+            }
+        ]
+    }
+    with requests_mock.Mocker() as mock_request:
+        mock_request.get(mms_url, text=json.dumps(mms_resp))
+        well_id = util.lookup_well_id("9999999999", "A99")
+        assert well_id is None
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/PKG-INFO` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aics-pipeline-uploaders
-Version: 1.1.0
+Version: 1.2.0
 Summary: This package contains resources for uploading pipeline data to FMS
 Author-email: AICS <!AICS_SW@alleninstitute.org>
 Project-URL: homepage, https://github.com/aics-int/aics_pipeline_uploaders
 Project-URL: documentation, https://aics-int.github.io/aics_pipeline_uploaders
 Project-URL: repository, https://github.com/aics-int/aics_pipeline_uploaders
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 [![Build Status](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/workflows/Build%20Main/badge.svg)](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/actions)
 [![Documentation](https://github.com/BrianWhitneyAI/aics_pipeline_uploaders/workflows/Documentation/badge.svg)](https://BrianWhitneyAI.github.io/aics_pipeline_uploaders/)
 [![Code Coverage](https://codecov.io/gh/BrianWhitneyAI/aics_pipeline_uploaders/branch/main/graph/badge.svg)](https://codecov.io/gh/BrianWhitneyAI/aics_pipeline_uploaders)
 
 This package contains resources for uploading pipeline data to FMS
 
-aics_pipeline_uploaders==1.1.0
+aics_pipeline_uploaders==1.2.0
 ---
 ## Features
 
 -   Store values and retain the prior value in memory
 -   ... some other functionality
 
 ## Installation
```

### Comparing `aics_pipeline_uploaders-1.1.0/aics_pipeline_uploaders.egg-info/SOURCES.txt` & `aics_pipeline_uploaders-1.2.0/aics_pipeline_uploaders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aics_pipeline_uploaders-1.1.0/pyproject.toml` & `aics_pipeline_uploaders-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [project]
 name = "aics_pipeline_uploaders"
-version = "1.1.0"  # Do not edit manually; managed by bumpversion
+version = "1.2.0"  # Do not edit manually; managed by bumpversion
 description = "This package contains resources for uploading pipeline data to FMS"
 authors = [
     {name = "AICS", email="!AICS_SW@alleninstitute.org"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.9.2"
 
 dependencies = [
     "aicsimageio ~= 4.9.2",
     "aicsimageio[czi] ~= 4.4",
-    "aicsfiles ~=5.1.0",
+    "aicsfiles ~=7.0.0",
     "lkaccess ~= 1.4.25",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black == 22.8.0",
     "build == 0.7.0",
-    "bump2version ~= 1.1.0",
+    "bump2version ~= 0.5.4",
     "flake8 ~= 5.0.4",
     "furo == 2022.9.29",
     "isort ~= 5.9",
     "m2r2 ~= 0.3.3",
     "mypy == 0.982",
     "numpy ~= 1.23.4",
     "pre-commit ~= 2.20.0",
```

### Comparing `aics_pipeline_uploaders-1.1.0/setup.cfg` & `aics_pipeline_uploaders-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.0
+current_version = 1.2.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.((?P<release>[a-z]*)(?P<devbuild>\d*)))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{devbuild}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
```

