# Comparing `tmp/talk_codebase-0.1.33.tar.gz` & `tmp/talk_codebase-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.33.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.34.tar", max compression
```

## Comparing `talk_codebase-0.1.33.tar` & `talk_codebase-0.1.34.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2874 2023-06-29 02:14:56.244210 talk_codebase-0.1.33/README.md
--rw-r--r--   0        0        0      896 2023-06-29 02:14:56.248210 talk_codebase-0.1.33/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 02:14:56.248210 talk_codebase-0.1.33/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2898 2023-06-29 02:14:56.248210 talk_codebase-0.1.33/talk_codebase/cli.py
--rw-r--r--   0        0        0     1615 2023-06-29 02:14:56.248210 talk_codebase-0.1.33/talk_codebase/consts.py
--rw-r--r--   0        0        0     4855 2023-06-29 02:14:56.248210 talk_codebase-0.1.33/talk_codebase/llm.py
--rw-r--r--   0        0        0     2346 2023-06-29 02:14:56.248210 talk_codebase-0.1.33/talk_codebase/utils.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0     2874 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/README.md
+-rw-r--r--   0        0        0      896 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1615 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/consts.py
+-rw-r--r--   0        0        0     4777 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2278 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.34/PKG-INFO
```

### Comparing `talk_codebase-0.1.33/README.md` & `talk_codebase-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.33/pyproject.toml` & `talk_codebase-0.1.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.33"
+version = "0.1.34"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.33/talk_codebase/cli.py` & `talk_codebase-0.1.34/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.33/talk_codebase/consts.py` & `talk_codebase-0.1.34/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.33/talk_codebase/llm.py` & `talk_codebase-0.1.34/talk_codebase/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,28 +70,28 @@
             exit(0)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=int(self.config.get("chunk_size")),
                                                        chunk_overlap=int(self.config.get("chunk_overlap")))
         texts = text_splitter.split_documents(docs)
         if index == MODEL_TYPES["OPENAI"]:
             cost = calculate_cost(docs, self.config.get("model_name"))
             approve = questionary.select(
-                f"Creating a vector store for {len(docs)} documents will cost ~${cost:.5f}. Do you want to continue?",
+                f"Creating a vector store will cost ~${cost:.5f}. Do you want to continue?",
                 choices=[
                     {"name": "Yes", "value": True},
                     {"name": "No", "value": False},
                 ]
             ).ask()
             if not approve:
                 exit(0)
 
-        spinners = Halo(text=f"Creating vector store for {len(docs)} documents", spinner='dots').start()
+        spinners = Halo(text=f"Creating vector store", spinner='dots').start()
         db = FAISS.from_documents(texts, embeddings)
         db.add_documents(texts)
         db.save_local(index_path)
-        spinners.succeed(f"Created vector store for {len(docs)} documents")
+        spinners.succeed(f"Created vector store")
         return db
 
 
 class LocalLLM(BaseLLM):
 
     def _create_store(self, root_dir: str) -> Optional[FAISS]:
         embeddings = HuggingFaceEmbeddings(model_name='all-MiniLM-L6-v2')
```

### Comparing `talk_codebase-0.1.33/talk_codebase/utils.py` & `talk_codebase-0.1.34/talk_codebase/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,33 +40,31 @@
     def on_llm_end(self, response, **kwargs):
         sys.stdout.write("\n")
         sys.stdout.flush()
 
 
 def load_files(root_dir):
     num_cpus = multiprocessing.cpu_count()
-    loaded_files = []
     with multiprocessing.Pool(num_cpus) as pool:
         futures = []
         for file_path in glob.glob(os.path.join(root_dir, '**/*'), recursive=True):
-            print('\r' + f'📂 Loading files: {file_path}')
             if is_ignored(file_path, root_dir):
                 continue
             if any(
                     file_path.endswith(exclude_file) for exclude_file in EXCLUDE_FILES):
                 continue
             for ext in LOADER_MAPPING:
                 if file_path.endswith(ext):
+                    print('\r' + f'📂 Loading files: {file_path}')
                     args = LOADER_MAPPING[ext]['args']
                     loader = LOADER_MAPPING[ext]['loader'](file_path, *args)
                     futures.append(pool.apply_async(loader.load))
-                    loaded_files.append(file_path)
         docs = []
         for future in futures:
-            docs.append(future.get()[0])
+            docs.extend(future.get())
     return docs
 
 
 def calculate_cost(texts, model_name):
     enc = tiktoken.encoding_for_model(model_name)
     all_text = ''.join([text.page_content for text in texts])
     tokens = enc.encode(all_text)
```

### Comparing `talk_codebase-0.1.33/PKG-INFO` & `talk_codebase-0.1.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.33
+Version: 0.1.34
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

