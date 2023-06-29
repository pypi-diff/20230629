# Comparing `tmp/Geode_Explicit-4.0.2rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.0.2rc2-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2244070 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-Jun-27 20:18 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-Jun-27 20:18 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-27 20:18 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2251776 b- defN 23-Jun-27 20:19 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    34304 b- defN 23-Jun-27 20:19 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2072064 b- defN 23-Jun-27 20:19 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-27 20:19 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-Jun-27 20:19 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2392 b- defN 23-Jun-27 20:19 Geode_Explicit-4.0.2rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-27 20:19 Geode_Explicit-4.0.2rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-27 20:19 Geode_Explicit-4.0.2rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 23-Jun-27 20:19 Geode_Explicit-4.0.2rc1.dist-info/RECORD
-12 files, 4657919 bytes uncompressed, 2242146 bytes compressed:  51.9%
+Zip file size: 314096 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-29 12:51 geode_explicit/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Jun-29 12:51 geode_explicit/brep.py
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-29 12:51 geode_explicit/section.py
+-rwxr-xr-x  2.0 unx   171552 b- defN 23-Jun-29 12:51 geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   147016 b- defN 23-Jun-29 12:51 geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   374048 b- defN 23-Jun-29 12:51 geode_explicit/lib64/libGeode-Explicit_brep.so
+-rwxr-xr-x  2.0 unx    43592 b- defN 23-Jun-29 12:51 geode_explicit/lib64/libGeode-Explicit_common.so
+-rwxr-xr-x  2.0 unx    72752 b- defN 23-Jun-29 12:51 geode_explicit/lib64/libGeode-Explicit_section.so
+-rw-r--r--  2.0 unx     2332 b- defN 23-Jun-29 12:51 Geode_Explicit-4.0.2rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-29 12:51 Geode_Explicit-4.0.2rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 12:51 Geode_Explicit-4.0.2rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-29 12:51 Geode_Explicit-4.0.2rc2.dist-info/RECORD
+12 files, 813166 bytes uncompressed, 312092 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: geode_explicit/brep.py
 Comment: 
 
 Filename: geode_explicit/section.py
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_brep.dll
+Filename: geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_common.dll
+Filename: geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_section.dll
+Filename: geode_explicit/lib64/libGeode-Explicit_brep.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_common.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_section.so
 Comment: 
 
-Filename: Geode_Explicit-4.0.2rc1.dist-info/METADATA
+Filename: Geode_Explicit-4.0.2rc2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.0.2rc1.dist-info/WHEEL
+Filename: Geode_Explicit-4.0.2rc2.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.0.2rc1.dist-info/top_level.txt
+Filename: Geode_Explicit-4.0.2rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.0.2rc1.dist-info/RECORD
+Filename: Geode_Explicit-4.0.2rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .section import *
-from .brep import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .section import *
+from .brep import *
```

## geode_explicit/brep.py

```diff
@@ -1,12 +1,12 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_inspector
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_brep import *
-ExplicitBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_inspector
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_brep import *
+ExplicitBRepLibrary.initialize()
```

## geode_explicit/section.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_section import *
-ExplicitSectionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_section import *
+ExplicitSectionLibrary.initialize()
```

## Comparing `Geode_Explicit-4.0.2rc1.dist-info/METADATA` & `Geode_Explicit-4.0.2rc2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-Metadata-Version: 2.1
-Name: Geode-Explicit
-Version: 4.0.2rc1
-Summary: Geode-solutions OpenGeode module for building explicit models
-Home-page: https://github.com/Geode-solutions/Geode-Explicit
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-background (==7.*,>=7.3.0rc1)
-Requires-Dist: geode-common (==26.*,>=26.1.2rc1)
-Requires-Dist: geode-conversion (==5.*,>=5.0.8)
-Requires-Dist: opengeode-core (==14.*,>=14.3.4rc1)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.12)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.5)
-Requires-Dist: opengeode-inspector (==3.*,>=3.0.6)
-Requires-Dist: opengeode-io (==6.*,>=6.0.8)
-
-<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Explicit
+Version: 4.0.2rc2
+Summary: Geode-solutions OpenGeode module for building explicit models
+Home-page: https://github.com/Geode-solutions/Geode-Explicit
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-background (==7.*,>=7.3.0rc1)
+Requires-Dist: geode-common (==26.*,>=26.1.2rc2)
+Requires-Dist: geode-conversion (==5.*,>=5.0.8)
+Requires-Dist: opengeode-core (==14.*,>=14.4.0rc2)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.12)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.6rc1)
+Requires-Dist: opengeode-inspector (==3.*,>=3.0.6)
+Requires-Dist: opengeode-io (==6.*,>=6.0.9rc1)
+
+<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.2rc1 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.2rc2 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.3.0rc1)
-Requires-Dist: geode-common (==26.*,>=26.1.2rc1) Requires-Dist: geode-
-conversion (==5.*,>=5.0.8) Requires-Dist: opengeode-core (==14.*,>=14.3.4rc1)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.12) Requires-Dist: opengeode-
-geosciencesio (==4.*,>=4.1.5) Requires-Dist: opengeode-inspector
-(==3.*,>=3.0.6) Requires-Dist: opengeode-io (==6.*,>=6.0.8)
+contact@geode-solutions.com License: Proprietary Description-Content-Type:
+text/markdown Requires-Dist: geode-background (==7.*,>=7.3.0rc1) Requires-Dist:
+geode-common (==26.*,>=26.1.2rc2) Requires-Dist: geode-conversion
+(==5.*,>=5.0.8) Requires-Dist: opengeode-core (==14.*,>=14.4.0rc2) Requires-
+Dist: opengeode-geosciences (==7.*,>=7.0.12) Requires-Dist: opengeode-
+geosciencesio (==4.*,>=4.1.6rc1) Requires-Dist: opengeode-inspector
+(==3.*,>=3.0.6) Requires-Dist: opengeode-io (==6.*,>=6.0.9rc1)
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Explicit-4.0.2rc1.dist-info/RECORD` & `Geode_Explicit-4.0.2rc2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-geode_explicit/__init__.py,sha256=-1Ma-Q_qKho5-HJywdEjGH_v91Dp0h8zchFCzKp7ADk,194
-geode_explicit/brep.py,sha256=5gXUGyujJVK7W7i2Zoqb5_9Mb5jPPZLiYZX9piVVUGY,271
-geode_explicit/section.py,sha256=diHY0-G0OXfICdOX3HSTnwrdrW3WOsct7GAT4rECQb4,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=G4eIR1zNFKbKXXuHIFRUnrFAYeOrVZxAMdJ67cmwpaE,2251776
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=0dBPRhV4Lk2Oyi_LkUCorynr_bdEaI9CBhsaQTo4jFA,34304
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=a23YOn8_W2-eC_gTiwLC5EhLY0ct30CkMNZpmMg7GJ0,2072064
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=p5euvLLcm9usPvJfIJ4lymqtBix_uSGlI5h7jUhD0_s,153600
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=BZgXNXLfGqd_kS-McAv-K27ppbwTBUGLrGILMiCAGzM,141824
-Geode_Explicit-4.0.2rc1.dist-info/METADATA,sha256=KBHNUhrT_sUJCRO7-G8ooQ73pMOoEsxhqDB3TCCR9aY,2392
-Geode_Explicit-4.0.2rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Explicit-4.0.2rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.0.2rc1.dist-info/RECORD,,
+geode_explicit/__init__.py,sha256=qYVdapUcPygn4JqOdtOMwy1qRD1BU5CbzlIv70VBZ24,89
+geode_explicit/brep.py,sha256=9ME2IUcanxZ1JaatGcKcuYUDCtIz6n99vUqRU9iMRac,261
+geode_explicit/section.py,sha256=sBEpKD71oVuLW7omi2OIBCgS0p8RZTLAcH7XEpo7OjQ,240
+geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so,sha256=2rnUzYxoKxFpcO-hoL2RfXSUVK8dsFWvNeJ9M0v1ij8,171552
+geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so,sha256=bJXXio7cBHbdbPGDWHHEem8BejgNsTNWTA-5JASAk50,147016
+geode_explicit/lib64/libGeode-Explicit_brep.so,sha256=jqL_135Fs_GREuTMHt6dKG6Mbint2_iAe9UqaH8b_aM,374048
+geode_explicit/lib64/libGeode-Explicit_common.so,sha256=fpIWurLbsAzw_-0YM4-d1Ld-er_uhiItnFMDMUjazDg,43592
+geode_explicit/lib64/libGeode-Explicit_section.so,sha256=4p00hEtyNstjd-hnvybi-USnkZOc_BdzeIc42JGe0OM,72752
+Geode_Explicit-4.0.2rc2.dist-info/METADATA,sha256=6FdPSEch0mqt1Kvs_OZpJDz00I3RhbWp3fwWjdFILHU,2332
+Geode_Explicit-4.0.2rc2.dist-info/WHEEL,sha256=3s2LSuQQhT9U1Dyv6MxBd72puf_ocSkY6hn5h0Kjf-o,103
+Geode_Explicit-4.0.2rc2.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.0.2rc2.dist-info/RECORD,,
```

