# Comparing `tmp/fw_file-2.2.0-py3-none-any.whl.zip` & `tmp/fw_file-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 211221 bytes, number of entries: 31
+Zip file size: 211560 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      229 b- defN 80-Jan-01 00:00 fw_file/__init__.py
 -rw-r--r--  2.0 unx     8377 b- defN 80-Jan-01 00:00 fw_file/base.py
 -rw-r--r--  2.0 unx     3184 b- defN 80-Jan-01 00:00 fw_file/bruker.py
 -rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 fw_file/dicom/__init__.py
 -rw-r--r--  2.0 unx     4912 b- defN 80-Jan-01 00:00 fw_file/dicom/config.py
 -rw-r--r--  2.0 unx    44285 b- defN 80-Jan-01 00:00 fw_file/dicom/dcmdict.py
 -rw-r--r--  2.0 unx    17527 b- defN 80-Jan-01 00:00 fw_file/dicom/dicom.py
--rw-r--r--  2.0 unx    16940 b- defN 80-Jan-01 00:00 fw_file/dicom/fixers.py
+-rw-r--r--  2.0 unx    18392 b- defN 80-Jan-01 00:00 fw_file/dicom/fixers.py
 -rw-r--r--  2.0 unx    17330 b- defN 80-Jan-01 00:00 fw_file/dicom/reader.py
 -rw-r--r--  2.0 unx    27641 b- defN 80-Jan-01 00:00 fw_file/dicom/series.py
 -rw-r--r--  2.0 unx   421033 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/dict_info.json
 -rw-r--r--  2.0 unx   188832 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/iod_info.json
 -rw-r--r--  2.0 unx   528709 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/module_info.json
 -rw-r--r--  2.0 unx    31221 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/uid_info.json
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/version
@@ -22,12 +22,12 @@
 -rw-r--r--  2.0 unx      778 b- defN 80-Jan-01 00:00 fw_file/jpg.py
 -rw-r--r--  2.0 unx     2186 b- defN 80-Jan-01 00:00 fw_file/json.py
 -rw-r--r--  2.0 unx     1440 b- defN 80-Jan-01 00:00 fw_file/nifti.py
 -rw-r--r--  2.0 unx     5265 b- defN 80-Jan-01 00:00 fw_file/philips.py
 -rw-r--r--  2.0 unx     8385 b- defN 80-Jan-01 00:00 fw_file/png.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_file/py.typed
 -rw-r--r--  2.0 unx    10521 b- defN 80-Jan-01 00:00 fw_file/siemens.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_file-2.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8486 b- defN 80-Jan-01 00:00 fw_file-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_file-2.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2509 b- defN 16-Jan-01 00:00 fw_file-2.2.0.dist-info/RECORD
-31 files, 1384172 bytes uncompressed, 207257 bytes compressed:  85.0%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_file-2.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8486 b- defN 80-Jan-01 00:00 fw_file-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_file-2.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2509 b- defN 16-Jan-01 00:00 fw_file-2.3.0.dist-info/RECORD
+31 files, 1385624 bytes uncompressed, 207596 bytes compressed:  85.0%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: fw_file/py.typed
 Comment: 
 
 Filename: fw_file/siemens.py
 Comment: 
 
-Filename: fw_file-2.2.0.dist-info/LICENSE
+Filename: fw_file-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_file-2.2.0.dist-info/METADATA
+Filename: fw_file-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_file-2.2.0.dist-info/WHEEL
+Filename: fw_file-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_file-2.2.0.dist-info/RECORD
+Filename: fw_file-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_file/dicom/fixers.py

```diff
@@ -66,22 +66,27 @@
     VR = raw.VR
     # After this, VR is guaranteed to be string, not None
     if not VR:
         VR = "UN"
     try:
         VR = dictionary_VR(raw.tag)
     except KeyError:
+        # Only set private tag VR if it is known in the private tag dictionary,
+        # AND if the found VR is _unknown_. Later in convert_exception_fixer, we
+        # will override the found VR with the dictionary VR but only if there is
+        # a converter exception trying to read the value given the VR in the
+        # dicom.
         if raw.tag.is_private:
             # VRs for private tags see PS3.5, 6.2.2
             new_VR = private_vr_for_tag(dataset, raw.tag)
             # Python 3.11 changed enums returning the enum type instead of string value
             new_VR = getattr(new_VR, "value", new_VR)
             # private_vr_for_tag returns UN if nothing found.
             # only update VR if something is found
-            if new_VR != "UN":
+            if new_VR != "UN" and VR == "UN":
                 VR = new_VR
         # group length tag implied in versions < 3.0
         elif raw.tag.element == 0:
             VR = "UL"
         else:
             VR = "UN"
     if VR != raw.VR:
@@ -187,14 +192,33 @@
         #
         # DA VR class instantiated:
         # https://github.com/pydicom/pydicom/blob/v2.2.2/pydicom/dataelem.py#L543
 
         value = convert_value(VR, raw, encoding)
         DataElement(raw.tag, VR, value, validation_mode=2)
     except (ValueError, OverflowError):
+        # Only attempt to apply dictionary VR for a private tag if initial value
+        # conversion didn't work. Private tag dictionary VRs don't seem to
+        # always be accurate, and in fact there is nothing stopping
+        # manufacturers from changing their internal "VR" for this field. So we
+        # should only rely on the dictionary as a last resort to give us a hint
+        # what the field should be if we can't decode it at first
+        if raw.tag.is_private:
+            # VRs for private tags see PS3.5, 6.2.2
+            new_VR = private_vr_for_tag(dataset, raw.tag)
+            # Python 3.11 changed enums returning the enum type instead of string value
+            new_VR = getattr(new_VR, "value", new_VR)
+            # private_vr_for_tag returns UN if nothing found.
+            # only update VR if something is found
+            if new_VR != "UN" and new_VR != VR:
+                # If we found a new VR, try converting again
+                VR = new_VR
+                raw = raw._replace(VR=new_VR)
+                return convert_exception_fixer(raw, encoding, dataset)
+
         # If we get a value error, it could be caused by either validate_value
         # or convert_value. Regardless, something is wrong with the value, so we
         # attempt to fix it.
         fixed_val = fix_invalid_VR_value(VR, raw, encoding=encoding, dataset=dataset)
         try:
             # Avoid calling TrackedRawDataElement._replace here since we
             # don't want this value change tracked
```

## Comparing `fw_file-2.2.0.dist-info/LICENSE` & `fw_file-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_file-2.2.0.dist-info/METADATA` & `fw_file-2.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-file
-Version: 2.2.0
+Version: 2.3.0
 Summary: Unified data-file interface
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-file
 License: MIT
 Keywords: Flywheel,parse,medical,file,metadata,extract,DICOM,RAW,MR,CT,PET,NIfTI,JPG,JPEG,PNG,Bruker,ParaVision,GE,PFile,Philips,PARREC,Siemens,PTD
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_file-2.2.0.dist-info/RECORD` & `fw_file-2.3.0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 fw_file/__init__.py,sha256=T3Tnv5R3uXDGZ-lp03D4noosiBfs9Bu6GzvDUUltgTg,229
 fw_file/base.py,sha256=skak6Ex5bfSPwzN48F5dsJvfEz-vcg-Kn84SkfhhHzI,8377
 fw_file/bruker.py,sha256=yM_xq-cdgJ8zPKjhHBBQ8YrJRvj1U3JHmzMj8MR3oUA,3184
 fw_file/dicom/__init__.py,sha256=Dh7WgsG2PoelxuqtM5-_5C0dbAi_CG_TW35_N5aRBxY,1515
 fw_file/dicom/config.py,sha256=fbbVedvpRcyWl_ehcHmYQimNU-HozLEsBj4SyUfDFw4,4912
 fw_file/dicom/dcmdict.py,sha256=y_NpdECSc-klhPnf69qpYbjwy_TsI2ikXwLckZIDVcA,44285
 fw_file/dicom/dicom.py,sha256=FspnCMXey-etyz9QGla9_QjmrBACe6ChtMH15YEHjzU,17527
-fw_file/dicom/fixers.py,sha256=MUyzotTps-O_PzZcenQjUqcz_ghdOQW4hG1d-6s5yu0,16940
+fw_file/dicom/fixers.py,sha256=_cPToJhNej7QDmYMtBAwZaRlR7JPABIPzZXOIN02CRU,18392
 fw_file/dicom/reader.py,sha256=WOhltexJvpI3Aeh64wrIWMkqUXpScf5zSu9uo_duk3I,17330
 fw_file/dicom/series.py,sha256=VGp5rmCMwo7mFfq9Dc5P54z-H0FoZff0j-oNkpynQnM,27641
 fw_file/dicom/standard/2023b/json/dict_info.json,sha256=G57E1IYRQssb6NVgA6hRA-qgrTAk-b_JgP7QUBjym1k,421033
 fw_file/dicom/standard/2023b/json/iod_info.json,sha256=kOR8UWIR7Gyut7WVGHmEXTJymjF8XYty6lqJWsoTwMs,188832
 fw_file/dicom/standard/2023b/json/module_info.json,sha256=juOJ1KQVVhL0J24fzGDl2joL6MtsBf223_PpkSvfwS8,528709
 fw_file/dicom/standard/2023b/json/uid_info.json,sha256=tkQbqwXGQO6_WsPxbNwf4eHQ8tdANM_PisWW8zqc864,31221
 fw_file/dicom/standard/2023b/json/version,sha256=uPt4p7NTFCveH-UkqLcBd1htCl0u6YAhWEHipHmPbBs,5
@@ -21,11 +21,11 @@
 fw_file/jpg.py,sha256=3qLSgZztivZ3so1CYD-CBC-x59kahOZO5Y5PIbVDX10,778
 fw_file/json.py,sha256=ufQ2YnNsyWocsB1yrTFEncHCKmIr7OeiwEUqOm3n3VY,2186
 fw_file/nifti.py,sha256=hKjKGhUUTrqIv6QsPe2qWJqteLbZPHZ52yWPf788iOQ,1440
 fw_file/philips.py,sha256=E9gyia6ZpyTg2RYktYFFDBNaI-plmYSVunhhWgfR_GA,5265
 fw_file/png.py,sha256=dqpSGSPg7Ox_B4JOFcSD2Uy5y0fXhM5O2tZgI-aZ4kU,8385
 fw_file/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_file/siemens.py,sha256=IYUQkiEJs9_25hb50NgdoHM8cw-l5iATlI1V1EdQwpc,10521
-fw_file-2.2.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_file-2.2.0.dist-info/METADATA,sha256=nItLch7QDGeuEw-8tQtMRfwoGMXD8gTcNtJ1vdfPflI,8486
-fw_file-2.2.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_file-2.2.0.dist-info/RECORD,,
+fw_file-2.3.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_file-2.3.0.dist-info/METADATA,sha256=QWxNeeagcxvKUUj3JASrgvufqTVCrv8B--Mb_QaX7XA,8486
+fw_file-2.3.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_file-2.3.0.dist-info/RECORD,,
```

