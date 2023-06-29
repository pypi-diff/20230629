# Comparing `tmp/sbom4python-0.9.1-py2.py3-none-any.whl.zip` & `tmp/sbom4python-0.9.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 40715 bytes, number of entries: 14
+Zip file size: 40793 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:00 sbom4python/__init__.py
 -rw-r--r--  2.0 unx     4573 b- defN 23-Mar-26 14:18 sbom4python/cli.py
 -rw-r--r--  2.0 unx     1820 b- defN 23-Jan-11 12:22 sbom4python/license.py
--rw-r--r--  2.0 unx     9607 b- defN 23-Apr-13 13:20 sbom4python/scanner.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:34 sbom4python/version.py
+-rw-r--r--  2.0 unx     9793 b- defN 23-Apr-14 15:58 sbom4python/scanner.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-29 16:49 sbom4python/version.py
 -rw-r--r--  2.0 unx   222585 b- defN 22-Oct-14 16:39 sbom4python/license_data/spdx_licenses.json
 -rw-r--r--  2.0 unx       75 b- defN 23-Mar-21 14:58 test/__init__.py
 -rw-r--r--  2.0 unx     1976 b- defN 23-Mar-21 16:30 test/test_license.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6301 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1146 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/RECORD
-14 files, 259791 bytes uncompressed, 38811 bytes compressed:  85.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-29 16:54 sbom4python-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6301 b- defN 23-Jun-29 16:54 sbom4python-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 16:54 sbom4python-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-29 16:54 sbom4python-0.9.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-29 16:54 sbom4python-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1146 b- defN 23-Jun-29 16:54 sbom4python-0.9.2.dist-info/RECORD
+14 files, 259977 bytes uncompressed, 38889 bytes compressed:  85.0%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_license.py
 Comment: 
 
-Filename: sbom4python-0.9.1.dist-info/LICENSE
+Filename: sbom4python-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: sbom4python-0.9.1.dist-info/METADATA
+Filename: sbom4python-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: sbom4python-0.9.1.dist-info/WHEEL
+Filename: sbom4python-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: sbom4python-0.9.1.dist-info/entry_points.txt
+Filename: sbom4python-0.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom4python-0.9.1.dist-info/top_level.txt
+Filename: sbom4python-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom4python-0.9.1.dist-info/RECORD
+Filename: sbom4python-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom4python/scanner.py

```diff
@@ -68,23 +68,25 @@
             supplier = supplier + "(" + emails[-1] + ")"
         return re.sub(" +", " ", supplier.strip())
 
     def process_module(self, module, parent="-"):
         if self.debug:
             print(f"Process Module {module}")
         out = self.run_program(f"pip show {module}")
-        # If module not found, no metadata returned
+        # If: module not found, no metadata returned
         if len(out) > 0:
             self.metadata = {}
             for line in out:
                 entry = line.split(":")
-                # store all data after keyword
-                self.metadata[entry[0]] = (
-                    line.split(f"{entry[0]}:", 1)[1].strip().rstrip("\n")
-                )
+                # If: this line contain an non empty entry delimited by ':'
+                if ((len(entry) == 2) and
+                        (entry[1] and not (entry[1].isspace()))):
+                    # then: store all data after keyword
+                    self.metadata[entry[0]] = (
+                        line.split(f"{entry[0]}:", 1)[1].strip().rstrip("\n"))
             if self.debug:
                 print(f"Metadata for {module}\n{self.metadata}")
             self.sbom_package.initialise()
             package = self.get("Name").lower().replace("_", "-")
             version = self.get("Version")
             self.sbom_package.set_name(package)
             self.sbom_package.set_version(version)
```

## sbom4python/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.9.1"
+VERSION: str = "0.9.2"
```

## Comparing `sbom4python-0.9.1.dist-info/LICENSE` & `sbom4python-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom4python-0.9.1.dist-info/METADATA` & `sbom4python-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom4python
-Version: 0.9.1
+Version: 0.9.2
 Summary: SBOM generator for Python modules
 Home-page: https://github.com/anthonyharrison/sbom4python
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lib4sbom (>=0.3.1)
-Requires-Dist: sbom4files (>=0.2.2)
 Requires-Dist: sbom2dot
+Requires-Dist: sbom4files (>=0.2.2)
 
 # SBOM4Python
 
 The SBOM4Python is a free, open source tool to generate a
 SBOM (Software Bill of Materials) for an installed Python module in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 It identifies all of the dependent components which are
```

## Comparing `sbom4python-0.9.1.dist-info/RECORD` & `sbom4python-0.9.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 sbom4python/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 sbom4python/cli.py,sha256=qu34b36ENBKAMFS835ArVhu7pjpqHznK8wdtQKucwME,4573
 sbom4python/license.py,sha256=5XRAwuvRNd4nt2T7shMQr3jUo9dEMstZF5Hov3IzvIw,1820
-sbom4python/scanner.py,sha256=Ub0gyH-pg-YBopfBvesJuGUqfgAHKPxpktF-WnYLrbY,9607
-sbom4python/version.py,sha256=yepdnyC7o4OD8LXWeMAliMLJmFekDrf4Yw5jUW-0KGs,100
+sbom4python/scanner.py,sha256=cHIPqWnHy8jqkodHn_PmR4TUb0gK3vTIm3sCYuomEdg,9793
+sbom4python/version.py,sha256=2fVLva60JTI60pUvuaiN-RZfJOIR_Blw7040wWu4IEQ,100
 sbom4python/license_data/spdx_licenses.json,sha256=mj836L9ndKZMZBORMqUkjzP0n23RRhleuBdXlER0pVE,222585
 test/__init__.py,sha256=Jdm3si-iktHDtKWwHpYgVfLYF-l1bE6TQDJASgkVpQU,75
 test/test_license.py,sha256=stWDum_UwVGZZsTyjrVICgBh3Azb6dUqZIMK_DUQe4s,1976
-sbom4python-0.9.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbom4python-0.9.1.dist-info/METADATA,sha256=FZFSmh6NzSk_lvqQZ6X9ZPloKcR47uLqbiUZKfIll68,6301
-sbom4python-0.9.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom4python-0.9.1.dist-info/entry_points.txt,sha256=_83UfxTjM06vaj0t1XlOO3YmniXkM1jsyvTdkee7tmk,53
-sbom4python-0.9.1.dist-info/top_level.txt,sha256=udvkgWvzv7RUbiqpZ-ANkgXwwk5fFhl2LiQkh8dJGQg,12
-sbom4python-0.9.1.dist-info/RECORD,,
+sbom4python-0.9.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbom4python-0.9.2.dist-info/METADATA,sha256=gXyGXoNHZa6d6x-R8Y5IdygYq8Rb3uSURATlSXAnQus,6301
+sbom4python-0.9.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom4python-0.9.2.dist-info/entry_points.txt,sha256=_83UfxTjM06vaj0t1XlOO3YmniXkM1jsyvTdkee7tmk,53
+sbom4python-0.9.2.dist-info/top_level.txt,sha256=udvkgWvzv7RUbiqpZ-ANkgXwwk5fFhl2LiQkh8dJGQg,12
+sbom4python-0.9.2.dist-info/RECORD,,
```

