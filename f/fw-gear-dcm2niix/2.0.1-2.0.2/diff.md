# Comparing `tmp/fw_gear_dcm2niix-2.0.1-py3-none-any.whl.zip` & `tmp/fw_gear_dcm2niix-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25338 bytes, number of entries: 15
+Zip file size: 25483 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/__init__.py
 -rw-r--r--  2.0 unx    14361 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/arrange.py
 -rw-r--r--  2.0 unx     7642 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py
 -rw-r--r--  2.0 unx     5646 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_utils.py
--rw-r--r--  2.0 unx     3528 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/interfaces.py
+-rw-r--r--  2.0 unx     3542 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/interfaces.py
 -rw-r--r--  2.0 unx     1240 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/prepare.py
 -rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/__init__.py
 -rw-r--r--  2.0 unx    15016 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/metadata.py
 -rw-r--r--  2.0 unx     7078 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/parse_config.py
 -rw-r--r--  2.0 unx     6904 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/resolve.py
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13774 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1354 b- defN 16-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/RECORD
-15 files, 77966 bytes uncompressed, 23062 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14183 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx     1354 b- defN 16-Jan-01 00:00 fw_gear_dcm2niix-2.0.2.dist-info/RECORD
+15 files, 78389 bytes uncompressed, 23207 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: fw_gear_dcm2niix/utils/parse_config.py
 Comment: 
 
 Filename: fw_gear_dcm2niix/utils/resolve.py
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.1.dist-info/LICENSE
+Filename: fw_gear_dcm2niix-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.1.dist-info/METADATA
+Filename: fw_gear_dcm2niix-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.1.dist-info/WHEEL
+Filename: fw_gear_dcm2niix-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.1.dist-info/RECORD
+Filename: fw_gear_dcm2niix-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gear_dcm2niix/dcm2niix/interfaces.py

```diff
@@ -63,15 +63,15 @@
             if val:
                 spec.argstr += " y"
             else:
                 spec.argstr += " n"
                 val = True
         if opt == "source_names":
             return spec.argstr % (os.path.dirname(val[0]) or ".")
-        return super()._format_arg(opt, spec, val)
+        return super(Dcm2niix, self)._format_arg(opt, spec, val)
 
     def _parse_files(self, filenames):
         """Adds mvec to filetypes"""
         outfiles, bvals, bvecs, mvecs, bids = [], [], [], [], []
         outtypes = [".bval", ".bvec", ".mvec", ".json", ".txt"]
         if self.inputs.to_nrrd:
             outtypes += [".nrrd", ".nhdr", ".raw.gz"]
```

## Comparing `fw_gear_dcm2niix-2.0.1.dist-info/LICENSE` & `fw_gear_dcm2niix-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gear_dcm2niix-2.0.1.dist-info/METADATA` & `fw_gear_dcm2niix-2.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-gear-dcm2niix
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Flywheel Gear for implementing Chris Rorden's dcm2niix for converting DICOM (or PAR/REC) to NIfTI (or NRRD).
 Home-page: https://gitlab.com/flywheel-io/scientific-solutions/gears/dcm2niix/
 License: Other
 Keywords: Flywheel,Gears
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.9,<4.0
@@ -323,14 +323,22 @@
 * NumberOfEchos, tag(2001,1014)
 * NumberOfSlices, tag(2001,1018)
 * NumberOfTemporalPositions
 
 All metadata applied to the output files from the dcm2niix Gear are extracted from the
 raw DICOM tags. As such, the units of measurement remain consistent with the DICOM standard.
 
+##### Tags
+If a value is provided in the "tag" config option, that tag will be added to the input file on completion of the gear execution.
+
+If the "tag_on_failure" config option is checked, the tag "dcm2niix-failure" will be added to the input file
+if the gear does not complete successfully. 
+
+The gear will REMOVE a "dcm2niix-failure" tag from a file if it is present and the gear completes successfully.
+
 ### Workflow
 
 ```mermaid
 graph LR
     dz["dicom.zip"] --> A[One Required] ===> dcm[dcm2niix_input]
     dt["dicom.tgz"] --> A
     pz["parrec.zip"] --> A
```

## Comparing `fw_gear_dcm2niix-2.0.1.dist-info/RECORD` & `fw_gear_dcm2niix-2.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 fw_gear_dcm2niix/__init__.py,sha256=YaB4aZxevqASxeO3okRaTHvCQVY6DS7BEGVymPgO2dQ,192
 fw_gear_dcm2niix/dcm2niix/__init__.py,sha256=gD5DzU4HJdzPQrsVL3sChft0ymhmdyDtqaPrG2AcX4U,27
 fw_gear_dcm2niix/dcm2niix/arrange.py,sha256=VwfF52hYLsAM5m-UaVoQ098VoTclGpr8vp6ksZHCWvE,14361
 fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py,sha256=GMl_YzdPglMiWb_DRXD7bXqSCKtTXhw5Y2igtwJJAGY,7642
 fw_gear_dcm2niix/dcm2niix/dcm2niix_utils.py,sha256=Bi7FVy2B4qeUJr_57FAM9OjizTRYeDDuLIvzoVEDpf8,5646
-fw_gear_dcm2niix/dcm2niix/interfaces.py,sha256=f-cFwE-W9WAbvXaVptrapXmMgnpXgI0yk7J92d_hUwM,3528
+fw_gear_dcm2niix/dcm2niix/interfaces.py,sha256=e_p9hf2G-fR94R8O_sgCN9PGgiLRvZWZhRkge5FgI34,3542
 fw_gear_dcm2niix/dcm2niix/prepare.py,sha256=SXB0Hglz6Y8L0yJ1h61YBFtAZMVtht1c59Iltz3O4II,1240
 fw_gear_dcm2niix/utils/__init__.py,sha256=JqFj1MIfZbijg-OcS_ho5QzMfpHEy2G-Pn95dFTlioM,24
 fw_gear_dcm2niix/utils/metadata.py,sha256=ipjsjmZke3xubty-AT73RmaeCOEnIPTTumA-epeBE7k,15016
 fw_gear_dcm2niix/utils/parse_config.py,sha256=Q1AJcBS0rE0FouFVtfun6l627uBUPAI5EQOL2lXdBS4,7078
 fw_gear_dcm2niix/utils/resolve.py,sha256=geyQqxyA_U2LFK1pvZj-l5-g0E0WZrnOH9NBH4ywMNA,6904
-fw_gear_dcm2niix-2.0.1.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
-fw_gear_dcm2niix-2.0.1.dist-info/METADATA,sha256=WP5zrLhFW1XmxANnyi0LsEuoK9DEDuRYtWwdKStWRS4,13774
-fw_gear_dcm2niix-2.0.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-fw_gear_dcm2niix-2.0.1.dist-info/RECORD,,
+fw_gear_dcm2niix-2.0.2.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+fw_gear_dcm2niix-2.0.2.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
+fw_gear_dcm2niix-2.0.2.dist-info/METADATA,sha256=G3h5qsq1ii5gaDEm0DkZcuAB8ZpjJBPZMuAUorKa8mA,14183
+fw_gear_dcm2niix-2.0.2.dist-info/RECORD,,
```

