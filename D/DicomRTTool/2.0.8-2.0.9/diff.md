# Comparing `tmp/DicomRTTool-2.0.8.tar.gz` & `tmp/DicomRTTool-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DicomRTTool-2.0.8.tar", last modified: Mon May  1 22:09:50 2023, max compression
+gzip compressed data, was "DicomRTTool-2.0.9.tar", last modified: Thu Jun 29 18:13:40 2023, max compression
```

## Comparing `DicomRTTool-2.0.8.tar` & `DicomRTTool-2.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.833644 DicomRTTool-2.0.8/DicomRTTool.egg-info/
--rw-rw-rw-   0        0        0     2890 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      239 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.833644 DicomRTTool-2.0.8/Images/
--rw-rw-rw-   0        0        0   587168 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/Images/multiple_rings.png
--rw-rw-rw-   0        0        0    35821 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      218 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2890 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2296 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-05-01 22:09:15.000000 DicomRTTool-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.849265 DicomRTTool-2.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/src/DicomRTTool/
--rw-rw-rw-   0        0        0    83848 2023-05-01 21:51:37.000000 DicomRTTool-2.0.8/src/DicomRTTool/ReaderWriter.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/src/DicomRTTool/Services/
--rw-rw-rw-   0        0        0     8964 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/Services/DicomBases.py
--rw-rw-rw-   0        0        0     1625 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/Services/StaticScripts.py
--rw-rw-rw-   0        0        0        0 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/Services/__init__.py
--rw-rw-rw-   0        0        0     1877 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/DicomRTTool/Viewer.py
--rw-rw-rw-   0        0        0      193 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/__init__.py
--rw-rw-rw-   0        0        0      156 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/DicomRTTool/key_list.txt
--rw-rw-rw-   0        0        0    17286 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/DicomRTTool/template_RS.dcm
--rw-rw-rw-   0        0        0     6133 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/Distribute_Train_Test_Validation.py
--rw-rw-rw-   0        0        0     1059 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/Main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:13:40.913617 DicomRTTool-2.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-29 18:13:40.857733 DicomRTTool-2.0.9/DicomRTTool.egg-info/
+-rw-rw-rw-   0        0        0     2890 2023-06-29 18:13:39.000000 DicomRTTool-2.0.9/DicomRTTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-29 18:13:39.000000 DicomRTTool-2.0.9/DicomRTTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:13:39.000000 DicomRTTool-2.0.9/DicomRTTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      239 2023-06-29 18:13:39.000000 DicomRTTool-2.0.9/DicomRTTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 18:13:39.000000 DicomRTTool-2.0.9/DicomRTTool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 18:13:40.865808 DicomRTTool-2.0.9/Images/
+-rw-rw-rw-   0        0        0   587168 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/Images/multiple_rings.png
+-rw-rw-rw-   0        0        0    35821 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      218 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2890 2023-06-29 18:13:40.912620 DicomRTTool-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2296 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:13:40.914615 DicomRTTool-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-06-29 18:09:30.000000 DicomRTTool-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:13:40.885692 DicomRTTool-2.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 18:13:40.902646 DicomRTTool-2.0.9/src/DicomRTTool/
+-rw-rw-rw-   0        0        0    83939 2023-06-27 16:48:53.000000 DicomRTTool-2.0.9/src/DicomRTTool/ReaderWriter.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:13:40.910625 DicomRTTool-2.0.9/src/DicomRTTool/Services/
+-rw-rw-rw-   0        0        0     8964 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/Services/DicomBases.py
+-rw-rw-rw-   0        0        0     1625 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/Services/StaticScripts.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/Services/__init__.py
+-rw-rw-rw-   0        0        0     1877 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/Viewer.py
+-rw-rw-rw-   0        0        0      193 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/key_list.txt
+-rw-rw-rw-   0        0        0    17286 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/DicomRTTool/template_RS.dcm
+-rw-rw-rw-   0        0        0     6133 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/Distribute_Train_Test_Validation.py
+-rw-rw-rw-   0        0        0     1059 2023-06-27 16:42:30.000000 DicomRTTool-2.0.9/src/Main.py
```

### Comparing `DicomRTTool-2.0.8/DicomRTTool.egg-info/PKG-INFO` & `DicomRTTool-2.0.9/DicomRTTool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DicomRTTool
-Version: 2.0.8
+Version: 2.0.9
 Summary: Services for reading dicom files, RT structures, and dose files, as well as tools for converting numpy prediction masks back to an RT structure
 Home-page: https://github.com/brianmanderson/Dicom_RT_and_Images_to_Mask
 Author: Brian Mark Anderson
 Author-email: b5anderson@health.ucsd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DicomRTTool-2.0.8/DicomRTTool.egg-info/SOURCES.txt` & `DicomRTTool-2.0.9/DicomRTTool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/Images/multiple_rings.png` & `DicomRTTool-2.0.9/Images/multiple_rings.png`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/LICENSE.txt` & `DicomRTTool-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/PKG-INFO` & `DicomRTTool-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DicomRTTool
-Version: 2.0.8
+Version: 2.0.9
 Summary: Services for reading dicom files, RT structures, and dose files, as well as tools for converting numpy prediction masks back to an RT structure
 Home-page: https://github.com/brianmanderson/Dicom_RT_and_Images_to_Mask
 Author: Brian Mark Anderson
 Author-email: b5anderson@health.ucsd.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DicomRTTool-2.0.8/README.md` & `DicomRTTool-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/setup.py` & `DicomRTTool-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='DicomRTTool',
     author='Brian Mark Anderson',
     author_email='b5anderson@health.ucsd.edu',
-    version='2.0.8',
+    version='2.0.9',
     description='Services for reading dicom files, RT structures, and dose files, as well as tools for '
                 'converting numpy prediction masks back to an RT structure',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={'DicomRTTool': 'src/DicomRTTool'},
     packages=['DicomRTTool'],
     include_package_data=True,
```

### Comparing `DicomRTTool-2.0.8/src/DicomRTTool/ReaderWriter.py` & `DicomRTTool-2.0.9/src/DicomRTTool/ReaderWriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,20 +593,20 @@
     def __set_description__(self, description: str):
         self.desciption = description
 
     def __set_iteration__(self, iteration=0):
         self.iteration = str(iteration)
 
     def __check_contours_at_index__(self, index: int, RTs: List[RTBase] = None) -> None:
+        self.rois_in_loaded_index = []
         if self.series_instances_dictionary[index].path is None:
             return
         if RTs is None:
             RTs = self.series_instances_dictionary[index].RTs
         true_rois = []
-        self.rois_in_loaded_index = []
         for RT_key in RTs:
             RT = RTs[RT_key]
             for code_key in RT.CodeAssociations:
                 if code_key not in self.roi_groups:
                     self.roi_groups[code_key] = RT.CodeAssociations[code_key]
                 else:
                     self.roi_groups[code_key] = list(set(self.roi_groups[code_key] + RT.CodeAssociations[code_key]))
@@ -913,14 +913,15 @@
         if self.verbose or len(self.series_instances_dictionary) > 1:
             for key in self.series_instances_dictionary:
                 print('Index {}, description {} at {}'.format(key,
                                                               self.series_instances_dictionary[key].Description,
                                                               self.series_instances_dictionary[key].path))
             print('{} unique series IDs were found. Default is index 0, to change use '
                   'set_index(index)'.format(len(self.series_instances_dictionary)))
+            self.set_index(0)
         self.__check_if_all_contours_present__()
         return None
 
     def write_parallel(self, out_path: typing.Union[str, bytes, os.PathLike],
                        excel_file: typing.Union[str, bytes, os.PathLike],
                        thread_count=int(cpu_count() * 0.9 - 1)):
         if not os.path.exists(out_path):
@@ -1108,16 +1109,17 @@
             print('Index is not present in the dictionary! Set it using set_index(index)')
             return None
         index = self.index
         if self.dicom_handle_uid != self.series_instances_dictionary[index].SeriesInstanceUID:
             print('Loading images for index {}, since mask was requested but image loading was '
                   'previously different\n'.format(index))
             self.get_images()
-        if self.rd_study_instance_uid == self.series_instances_dictionary[index].StudyInstanceUID:  # Already loaded
-            return None
+        if self.rd_study_instance_uid is not None:
+            if self.rd_study_instance_uid == self.series_instances_dictionary[index].StudyInstanceUID:  # Already loaded
+                return None
         self.rd_study_instance_uid = self.series_instances_dictionary[index].StudyInstanceUID
         RDs = self.series_instances_dictionary[index].RDs
         reader = sitk.ImageFileReader()
         output, spacing, direction, origin = None, None, None, None
         self.dose = None
         for rd_series_instance_uid in RDs:
             rd = RDs[rd_series_instance_uid]
```

### Comparing `DicomRTTool-2.0.8/src/DicomRTTool/Services/DicomBases.py` & `DicomRTTool-2.0.9/src/DicomRTTool/Services/DicomBases.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/src/DicomRTTool/Services/StaticScripts.py` & `DicomRTTool-2.0.9/src/DicomRTTool/Services/StaticScripts.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/src/DicomRTTool/Viewer.py` & `DicomRTTool-2.0.9/src/DicomRTTool/Viewer.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/src/DicomRTTool/template_RS.dcm` & `DicomRTTool-2.0.9/src/DicomRTTool/template_RS.dcm`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/src/Distribute_Train_Test_Validation.py` & `DicomRTTool-2.0.9/src/Distribute_Train_Test_Validation.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.8/src/Main.py` & `DicomRTTool-2.0.9/src/Main.py`

 * *Files identical despite different names*

