# Comparing `tmp/hmd_graphql_client-0.1.105-py3-none-any.whl.zip` & `tmp/hmd_graphql_client-0.1.98-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10737 bytes, number of entries: 12
--rw-rw-rw-  2.0 unx       40 b- defN 23-Apr-24 15:55 hmd_graphql_client/__init__.py
--rw-rw-rw-  2.0 unx      759 b- defN 23-Apr-24 15:55 hmd_graphql_client/hmd_base_auth_client.py
--rw-rw-rw-  2.0 unx     4274 b- defN 23-Apr-24 15:55 hmd_graphql_client/hmd_base_client.py
--rw-rw-rw-  2.0 unx     2538 b- defN 23-Apr-24 15:55 hmd_graphql_client/hmd_db_engine_client.py
--rw-rw-rw-  2.0 unx     5682 b- defN 23-Apr-24 15:55 hmd_graphql_client/hmd_lambda_client.py
--rw-rw-rw-  2.0 unx     7523 b- defN 23-Apr-24 15:55 hmd_graphql_client/hmd_memory_client.py
--rw-rw-rw-  2.0 unx     4876 b- defN 23-Apr-24 15:55 hmd_graphql_client/hmd_rest_client.py
--rw-rw-rw-  2.0 unx     3337 b- defN 23-Apr-24 15:55 hmd_graphql_client/relationship_support.py
--rw-rw-rw-  2.0 unx     2440 b- defN 23-Apr-24 15:55 hmd_graphql_client-0.1.105.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-24 15:55 hmd_graphql_client-0.1.105.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       19 b- defN 23-Apr-24 15:55 hmd_graphql_client-0.1.105.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1111 b- defN 23-Apr-24 15:55 hmd_graphql_client-0.1.105.dist-info/RECORD
-12 files, 32691 bytes uncompressed, 8827 bytes compressed:  73.0%
+Zip file size: 10726 bytes, number of entries: 12
+-rw-rw-rw-  2.0 unx       40 b- defN 23-Feb-28 20:08 hmd_graphql_client/__init__.py
+-rw-rw-rw-  2.0 unx      759 b- defN 23-Feb-28 20:08 hmd_graphql_client/hmd_base_auth_client.py
+-rw-rw-rw-  2.0 unx     4274 b- defN 23-Feb-28 20:08 hmd_graphql_client/hmd_base_client.py
+-rw-rw-rw-  2.0 unx     2538 b- defN 23-Feb-28 20:08 hmd_graphql_client/hmd_db_engine_client.py
+-rw-rw-rw-  2.0 unx     5682 b- defN 23-Feb-28 20:08 hmd_graphql_client/hmd_lambda_client.py
+-rw-rw-rw-  2.0 unx     7523 b- defN 23-Feb-28 20:08 hmd_graphql_client/hmd_memory_client.py
+-rw-rw-rw-  2.0 unx     4876 b- defN 23-Feb-28 20:08 hmd_graphql_client/hmd_rest_client.py
+-rw-rw-rw-  2.0 unx     3337 b- defN 23-Feb-28 20:08 hmd_graphql_client/relationship_support.py
+-rw-rw-rw-  2.0 unx     2439 b- defN 23-Feb-28 20:09 hmd_graphql_client-0.1.98.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Feb-28 20:09 hmd_graphql_client-0.1.98.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       19 b- defN 23-Feb-28 20:09 hmd_graphql_client-0.1.98.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1107 b- defN 23-Feb-28 20:09 hmd_graphql_client-0.1.98.dist-info/RECORD
+12 files, 32686 bytes uncompressed, 8824 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: hmd_graphql_client/hmd_rest_client.py
 Comment: 
 
 Filename: hmd_graphql_client/relationship_support.py
 Comment: 
 
-Filename: hmd_graphql_client-0.1.105.dist-info/METADATA
+Filename: hmd_graphql_client-0.1.98.dist-info/METADATA
 Comment: 
 
-Filename: hmd_graphql_client-0.1.105.dist-info/WHEEL
+Filename: hmd_graphql_client-0.1.98.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_graphql_client-0.1.105.dist-info/top_level.txt
+Filename: hmd_graphql_client-0.1.98.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_graphql_client-0.1.105.dist-info/RECORD
+Filename: hmd_graphql_client-0.1.98.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hmd_graphql_client-0.1.105.dist-info/METADATA` & `hmd_graphql_client-0.1.98.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-graphql-client
-Version: 0.1.105
+Version: 0.1.98
 Summary: A client for the graphql servers.
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: acachecontrol (==0.3.5)
@@ -25,17 +25,17 @@
 Requires-Dist: charset-normalizer (==2.0.12)
 Requires-Dist: decorator (==5.1.1)
 Requires-Dist: ecdsa (==0.17.0)
 Requires-Dist: frozenlist (==1.3.0)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
-Requires-Dist: hmd-cli-tools (~=1.1.228)
-Requires-Dist: hmd-entity-storage (~=0.1.223)
-Requires-Dist: hmd-lib-auth (~=0.1.75)
+Requires-Dist: hmd-cli-tools (~=1.1.227)
+Requires-Dist: hmd-entity-storage (~=0.1.216)
+Requires-Dist: hmd-lib-auth (~=0.1.67)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.34)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonschema (==4.4.0)
```

## Comparing `hmd_graphql_client-0.1.105.dist-info/RECORD` & `hmd_graphql_client-0.1.98.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 hmd_graphql_client/hmd_base_auth_client.py,sha256=j5QWaDOdYYYp4vvUej6MU0JAz1fdknSb0n3F8Kbb6Vw,759
 hmd_graphql_client/hmd_base_client.py,sha256=npZLchp4MX8nH8zeAf72oVeoKS4-cS7TGcPcdwBnH5o,4274
 hmd_graphql_client/hmd_db_engine_client.py,sha256=omJ7m89hjipAeJeoOqsgu7x88cehW1y0yDIPyKtd4A4,2538
 hmd_graphql_client/hmd_lambda_client.py,sha256=ozSXrU8_H9sftcIOaA2PrQiwGdw186rV7Q-EqPesHMo,5682
 hmd_graphql_client/hmd_memory_client.py,sha256=TRWrJ8L-SFmpjrfryi1vrHGtkVlsQn-1UprRbsuvVf8,7523
 hmd_graphql_client/hmd_rest_client.py,sha256=i1vhLErGmV_pplqSV0zACzGjyR3-3x53zaTQjZ8DX38,4876
 hmd_graphql_client/relationship_support.py,sha256=A4b8Y7cde2Kn27txjW-zetamsPyRVz6o8TEOWuitLBo,3337
-hmd_graphql_client-0.1.105.dist-info/METADATA,sha256=OapaoqWQduZcuhzLt7kONJbAFEDeNaA4pTociHUKggM,2440
-hmd_graphql_client-0.1.105.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_graphql_client-0.1.105.dist-info/top_level.txt,sha256=StgxSTi2IUD5DYygaMpd1K_Uy1P7UlN1aCEoTL-4m30,19
-hmd_graphql_client-0.1.105.dist-info/RECORD,,
+hmd_graphql_client-0.1.98.dist-info/METADATA,sha256=VlfT8se0IT5BJBJbTn4jbgDzPm6c29RSqIlCGHmxJ7M,2439
+hmd_graphql_client-0.1.98.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_graphql_client-0.1.98.dist-info/top_level.txt,sha256=StgxSTi2IUD5DYygaMpd1K_Uy1P7UlN1aCEoTL-4m30,19
+hmd_graphql_client-0.1.98.dist-info/RECORD,,
```

