# Comparing `tmp/concept_x_converter-0.3.0-cp37-abi3-win_amd64.whl.zip` & `tmp/concept_x_converter-0.3.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 225072 bytes, number of entries: 5
--rw-r--r--  4.6 unx     2212 b- defN 23-Jun-29 19:31 concept_x_converter-0.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-29 19:31 concept_x_converter-0.3.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      159 b- defN 23-Jun-29 19:31 concept_x_converter/__init__.py
--rwxr-xr-x  4.6 unx   510976 b- defN 23-Jun-29 19:31 concept_x_converter/concept_x_converter.pyd
--rw-r--r--  4.6 unx      431 b- defN 23-Jun-29 19:31 concept_x_converter-0.3.0.dist-info/RECORD
-5 files, 513874 bytes uncompressed, 224268 bytes compressed:  56.4%
+Zip file size: 223650 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2212 b- defN 23-Jun-29 20:44 concept_x_converter-0.3.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-29 20:44 concept_x_converter-0.3.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx      159 b- defN 23-Jun-29 20:44 concept_x_converter/__init__.py
+-rwxr-xr-x  4.6 unx   508416 b- defN 23-Jun-29 20:44 concept_x_converter/concept_x_converter.pyd
+-rw-r--r--  4.6 unx      431 b- defN 23-Jun-29 20:44 concept_x_converter-0.3.1.dist-info/RECORD
+5 files, 511314 bytes uncompressed, 222846 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: concept_x_converter-0.3.0.dist-info/METADATA
+Filename: concept_x_converter-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: concept_x_converter-0.3.0.dist-info/WHEEL
+Filename: concept_x_converter-0.3.1.dist-info/WHEEL
 Comment: 
 
 Filename: concept_x_converter/__init__.py
 Comment: 
 
 Filename: concept_x_converter/concept_x_converter.pyd
 Comment: 
 
-Filename: concept_x_converter-0.3.0.dist-info/RECORD
+Filename: concept_x_converter-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `concept_x_converter-0.3.0.dist-info/METADATA` & `concept_x_converter-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concept_x_converter
-Version: 0.3.0
+Version: 0.3.1
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ConecptX_Converter
 
 This tool is designed for converting [ConceptX](https://github.com/hsajjad/ConceptX) activation files into Word2Vec format. The resulting Word2Vec file can be used with gensim library in Python to find **semantically** similar words.
 <br><br>
 This tool could be built as a binary file, or it could be run as a cargo project. The following sections describe how to build and run the tool.
```

