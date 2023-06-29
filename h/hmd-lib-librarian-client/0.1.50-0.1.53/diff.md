# Comparing `tmp/hmd_lib_librarian_client-0.1.50-py3-none-any.whl.zip` & `tmp/hmd_lib_librarian_client-0.1.53-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8142 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-02 13:42 hmd_lib_librarian_client/__init__.py
--rw-rw-rw-  2.0 unx     5142 b- defN 23-Mar-02 13:42 hmd_lib_librarian_client/artifact_tools.py
--rw-rw-rw-  2.0 unx     6166 b- defN 23-Mar-02 13:42 hmd_lib_librarian_client/file_uploader.py
--rw-rw-rw-  2.0 unx     8494 b- defN 23-Mar-02 13:42 hmd_lib_librarian_client/hmd_lib_librarian_client.py
--rw-rw-rw-  2.0 unx     2456 b- defN 23-Mar-02 13:43 hmd_lib_librarian_client-0.1.50.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Mar-02 13:43 hmd_lib_librarian_client-0.1.50.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       25 b- defN 23-Mar-02 13:43 hmd_lib_librarian_client-0.1.50.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-Mar-02 13:43 hmd_lib_librarian_client-0.1.50.dist-info/RECORD
-8 files, 23141 bytes uncompressed, 6770 bytes compressed:  70.7%
+Zip file size: 8141 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Apr-27 12:47 hmd_lib_librarian_client/__init__.py
+-rw-rw-rw-  2.0 unx     5142 b- defN 23-Apr-27 12:47 hmd_lib_librarian_client/artifact_tools.py
+-rw-rw-rw-  2.0 unx     6166 b- defN 23-Apr-27 12:47 hmd_lib_librarian_client/file_uploader.py
+-rw-rw-rw-  2.0 unx     8494 b- defN 23-Apr-27 12:47 hmd_lib_librarian_client/hmd_lib_librarian_client.py
+-rw-rw-rw-  2.0 unx     2457 b- defN 23-Apr-27 12:48 hmd_lib_librarian_client-0.1.53.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-27 12:48 hmd_lib_librarian_client-0.1.53.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       25 b- defN 23-Apr-27 12:48 hmd_lib_librarian_client-0.1.53.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-Apr-27 12:48 hmd_lib_librarian_client-0.1.53.dist-info/RECORD
+8 files, 23142 bytes uncompressed, 6769 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: hmd_lib_librarian_client/file_uploader.py
 Comment: 
 
 Filename: hmd_lib_librarian_client/hmd_lib_librarian_client.py
 Comment: 
 
-Filename: hmd_lib_librarian_client-0.1.50.dist-info/METADATA
+Filename: hmd_lib_librarian_client-0.1.53.dist-info/METADATA
 Comment: 
 
-Filename: hmd_lib_librarian_client-0.1.50.dist-info/WHEEL
+Filename: hmd_lib_librarian_client-0.1.53.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_lib_librarian_client-0.1.50.dist-info/top_level.txt
+Filename: hmd_lib_librarian_client-0.1.53.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_lib_librarian_client-0.1.50.dist-info/RECORD
+Filename: hmd_lib_librarian_client-0.1.53.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hmd_lib_librarian_client-0.1.50.dist-info/METADATA` & `hmd_lib_librarian_client-0.1.53.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-lib-librarian-client
-Version: 0.1.50
+Version: 0.1.53
 Summary: A client library to interface with librarian.
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Requires-Dist: acachecontrol (==0.3.5)
 Requires-Dist: aenum (==2.2.6)
 Requires-Dist: aiohttp (==3.8.1)
@@ -23,18 +23,18 @@
 Requires-Dist: charset-normalizer (==2.0.12)
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
-Requires-Dist: hmd-cli-tools (~=1.1.227)
-Requires-Dist: hmd-entity-storage (~=0.1.216)
-Requires-Dist: hmd-graphql-client (~=0.1.98)
-Requires-Dist: hmd-lib-auth (~=0.1.67)
+Requires-Dist: hmd-cli-tools (~=1.1.228)
+Requires-Dist: hmd-entity-storage (~=0.1.223)
+Requires-Dist: hmd-graphql-client (~=0.1.105)
+Requires-Dist: hmd-lib-auth (~=0.1.75)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonschema (==4.4.0)
```

## Comparing `hmd_lib_librarian_client-0.1.50.dist-info/RECORD` & `hmd_lib_librarian_client-0.1.53.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 hmd_lib_librarian_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hmd_lib_librarian_client/artifact_tools.py,sha256=yBuody3VaUTZ7j4xJwTbIHZSq0gngDsFHdx2FV2AydM,5142
 hmd_lib_librarian_client/file_uploader.py,sha256=8B0O94pwfW-KSlj4GLgaFM38-F4TfJqpwMos5XUCWEE,6166
 hmd_lib_librarian_client/hmd_lib_librarian_client.py,sha256=zVeBwxZLneNCEFs53YMCGprNpgFxcOFMW-EkVDUVhZU,8494
-hmd_lib_librarian_client-0.1.50.dist-info/METADATA,sha256=ZliB8AbmKMk_X7vs4ClMAHhHKE_0y4RHwWRifyAaB4M,2456
-hmd_lib_librarian_client-0.1.50.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_lib_librarian_client-0.1.50.dist-info/top_level.txt,sha256=6wwN9CnhhFuOkx0ERY0wh60ovSL6Rc3kuekH80pJIYE,25
-hmd_lib_librarian_client-0.1.50.dist-info/RECORD,,
+hmd_lib_librarian_client-0.1.53.dist-info/METADATA,sha256=9gw26UJcDkMvlZv_6183w7WPbGnjvHNJJFmCXTvtVVs,2457
+hmd_lib_librarian_client-0.1.53.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_lib_librarian_client-0.1.53.dist-info/top_level.txt,sha256=6wwN9CnhhFuOkx0ERY0wh60ovSL6Rc3kuekH80pJIYE,25
+hmd_lib_librarian_client-0.1.53.dist-info/RECORD,,
```

