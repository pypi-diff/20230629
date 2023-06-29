# Comparing `tmp/pgml-0.7.0-cp39-none-win_amd64.whl.zip` & `tmp/pgml-0.7.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 2231000 bytes, number of entries: 6
--rw-r--r--  4.6 unx    17316 b- defN 23-Jun-20 00:11 pgml-0.7.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jun-20 00:11 pgml-0.7.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     1577 b- defN 23-Jun-20 00:11 pgml/pgml.pyi
--rw-r--r--  4.6 unx      107 b- defN 23-Jun-20 00:11 pgml/__init__.py
--rwxr-xr-x  4.6 unx  5925376 b- defN 23-Jun-20 00:11 pgml/pgml.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      428 b- defN 23-Jun-20 00:11 pgml-0.7.0.dist-info/RECORD
-6 files, 5944898 bytes uncompressed, 2230244 bytes compressed:  62.5%
+Zip file size: 1908690 bytes, number of entries: 5
+-rw-r--r--  4.6 unx    17320 b- defN 23-Jun-29 19:32 pgml-0.7.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-29 19:32 pgml-0.7.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx      107 b- defN 23-Jun-29 19:32 pgml/__init__.py
+-rwxr-xr-x  4.6 unx  4852736 b- defN 23-Jun-29 19:32 pgml/pgml.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      358 b- defN 23-Jun-29 19:32 pgml-0.7.1.dist-info/RECORD
+5 files, 4870615 bytes uncompressed, 1908036 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
-Filename: pgml-0.7.0.dist-info/METADATA
+Filename: pgml-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: pgml-0.7.0.dist-info/WHEEL
-Comment: 
-
-Filename: pgml/pgml.pyi
+Filename: pgml-0.7.1.dist-info/WHEEL
 Comment: 
 
 Filename: pgml/__init__.py
 Comment: 
 
 Filename: pgml/pgml.cp39-win_amd64.pyd
 Comment: 
 
-Filename: pgml-0.7.0.dist-info/RECORD
+Filename: pgml-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pgml-0.7.0.dist-info/METADATA` & `pgml-0.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgml
-Version: 0.7.0
+Version: 0.7.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python SDK is designed to facilitate the development of scalable vector search applications on PostgreSQL databases.
 Keywords: postgres,machine learning,vector databases,embeddings
 Author-email: PostgresML <team@postgresml.org>
 Requires-Python: >=3.7
@@ -262,15 +262,15 @@
 ```
 
 This function allows for the registration of a model in a database, creating a record if it does not already exist. `model_name` is the name of the open source HuggingFace model being registered and `model_params` is a dictionary containing parameters for configuring the model. It can be empty if no parameters are needed.
 
 #### Register Text Splitter
 
 ```python
-await collection.register_text_splitter(splitter_name="recursive_character",splitter_params={"chunk_size": 100,"chunk_overlap": 20})
+await collection.register_text_splitter(splitter_name="recursive_character",splitter_params={"chunk_size": "100","chunk_overlap": "20"})
 ```
 
 This function allows for the registration of a text spliter in a database, creating a record if it doesn't already exist. Following [LangChain](https://python.langchain.com/en/latest/reference/modules/text_splitter.html) splitters are supported.
 
 ```
 SPLITTERS = {
     "character": CharacterTextSplitter,
```

