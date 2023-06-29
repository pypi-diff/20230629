# Comparing `tmp/reait-0.0.7.tar.gz` & `tmp/reait-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reait-0.0.7.tar", last modified: Wed Nov 16 14:22:33 2022, max compression
+gzip compressed data, was "reait-0.0.9.tar", last modified: Thu Nov 17 14:50:29 2022, max compression
```

## Comparing `reait-0.0.7.tar` & `reait-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-11-16 14:22:33.030590 reait-0.0.7/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2022-11-11 16:03:01.000000 reait-0.0.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2884 2022-11-16 14:22:33.030590 reait-0.0.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2237 2022-11-15 09:43:09.000000 reait-0.0.7/README.md
--rw-r--r--   0 user      (1000) user      (1000)      791 2022-11-16 14:21:42.000000 reait-0.0.7/pyproject.toml
--rwxr-xr-x   0 user      (1000) user      (1000)     6192 2022-11-16 14:21:23.000000 reait-0.0.7/reait
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-11-16 14:22:33.020591 reait-0.0.7/reait.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2884 2022-11-16 14:22:32.000000 reait-0.0.7/reait.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      191 2022-11-16 14:22:33.000000 reait-0.0.7/reait.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-11-16 14:22:32.000000 reait-0.0.7/reait.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       34 2022-11-16 14:22:32.000000 reait-0.0.7/reait.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-11-16 14:22:32.000000 reait-0.0.7/reait.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-11-16 14:22:33.030590 reait-0.0.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      704 2022-11-16 14:21:31.000000 reait-0.0.7/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-11-17 14:50:29.874474 reait-0.0.9/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2022-11-11 16:03:01.000000 reait-0.0.9/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3378 2022-11-17 14:50:29.874474 reait-0.0.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2714 2022-11-17 13:53:04.000000 reait-0.0.9/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      844 2022-11-17 13:43:01.000000 reait-0.0.9/pyproject.toml
+-rwxr-xr-x   0 user      (1000) user      (1000)     7799 2022-11-17 13:43:01.000000 reait-0.0.9/reait
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-11-17 14:50:29.874474 reait-0.0.9/reait.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3378 2022-11-17 14:50:29.000000 reait-0.0.9/reait.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      191 2022-11-17 14:50:29.000000 reait-0.0.9/reait.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2022-11-17 14:50:29.000000 reait-0.0.9/reait.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       34 2022-11-17 14:50:29.000000 reait-0.0.9/reait.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2022-11-17 14:50:29.000000 reait-0.0.9/reait.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2022-11-17 14:50:29.874474 reait-0.0.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      734 2022-11-17 13:43:01.000000 reait-0.0.9/setup.py
```

### Comparing `reait-0.0.7/LICENSE` & `reait-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reait-0.0.7/PKG-INFO` & `reait-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: reait
-Version: 0.0.7
+Version: 0.0.9
 Home-page: https://github.com/RevEng-AI/reait
 Project-URL: Homepage, https://github.com/RevEng-AI/reait
 Project-URL: Bug Tracker, https://github.com/RevEng-AI/reait/issues
 Project-URL: Organisation Homepage, https://reveng.ai
 Project-URL: Documentation, https://docs.reveng.ai
-Keywords: reverse,engineering,reveng.ai,reveng,machine,learning,binary,analysis,ml,ai
+Keywords: reverse,engineering,reveng.ai,reveng,machine,learning,binary,analysis,ml,ai,vector,embedding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # reait
@@ -52,14 +52,22 @@
 ### Search for similar symbols based on JSON embedding file
 To query our database of similar symbols based on an embedding, use `-n` to search using Approximate Nearest Neighbours. The `--nns` allows you to specify the number of results returned. A list of symbol names and the distance between each vector is returned. 
 
 `reait -e embedding.json -n`
 
 NB: A smaller distance indicates a higher degree of similarity.
 
+#### Limited Search
+To search for the most similar symbols found in a binary to a specific embedding, use the `--found-in` option with a path to the executable.
+
+`reait -n --embedding /tmp/sha256_init.json --found-in ~/malware.exe` 
+
+This downloads embeddings from `malware.exe` and computes the cosine similarity between all symbols and `sha256_init.json`. The returned results lists the most similar results by cosine similarity score (1.0 most similar, -1.0, dissimilar).
+
+
 ## Configuration
 
 `reait` reads the config file stored at `~/.reait.toml`. An example config file looks like:
 
 ```
 apikey = "l1br3"
 host = "https://api.reveng.ai"
```

### Comparing `reait-0.0.7/README.md` & `reait-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,22 @@
 ### Search for similar symbols based on JSON embedding file
 To query our database of similar symbols based on an embedding, use `-n` to search using Approximate Nearest Neighbours. The `--nns` allows you to specify the number of results returned. A list of symbol names and the distance between each vector is returned. 
 
 `reait -e embedding.json -n`
 
 NB: A smaller distance indicates a higher degree of similarity.
 
+#### Limited Search
+To search for the most similar symbols found in a binary to a specific embedding, use the `--found-in` option with a path to the executable.
+
+`reait -n --embedding /tmp/sha256_init.json --found-in ~/malware.exe` 
+
+This downloads embeddings from `malware.exe` and computes the cosine similarity between all symbols and `sha256_init.json`. The returned results lists the most similar results by cosine similarity score (1.0 most similar, -1.0, dissimilar).
+
+
 ## Configuration
 
 `reait` reads the config file stored at `~/.reait.toml`. An example config file looks like:
 
 ```
 apikey = "l1br3"
 host = "https://api.reveng.ai"
```

### Comparing `reait-0.0.7/pyproject.toml` & `reait-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
-requires = ["setuptools >= 40.9.0", "tqdm", "argparse", "requests", "rich", "tomli"]
+requires = ["setuptools >= 40.9.0", "tqdm", "argparse", "requests", "rich", "tomli", "sklearn", "pandas", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reait"
-version = "0.0.7"
+version = "0.0.9"
 readme = "README.md"
 classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent"
 ]
 dependencies = [
     "tqdm",
     "requests",
     "rich",
     "argparse",
     "tomli"
 ]
-keywords = ["reverse", "engineering", "reveng.ai", "reveng", "machine", "learning", "binary", "analysis", "ml", "ai"]
+keywords = ["reverse", "engineering", "reveng.ai", "reveng", "machine", "learning", "binary", "analysis", "ml", "ai", "vector", "embedding"]
 
 [project.urls]
 "Homepage" = "https://github.com/RevEng-AI/reait"
 "Bug Tracker" = "https://github.com/RevEng-AI/reait/issues"
 "Organisation Homepage" = "https://reveng.ai"
 "Documentation" = "https://docs.reveng.ai"
```

### Comparing `reait-0.0.7/reait` & `reait-0.0.9/reait`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from json import dumps
 from os import system
 from tqdm import tqdm 
 from hashlib import sha256
 from rich import print_json
+from sklearn.metrics.pairwise import cosine_similarity
 import os
 from argparse import ArgumentParser
-import traceback
-from IPython import embed
 import requests
+import numpy as np
+import pandas as pd
 import json
 import tomli
 from os.path import isfile
 from sys import exit
+# from IPython import embed
 
-__version__ = "0.0.7"
+__version__ = "0.0.9"
 
 re_conf = {
     'apikey' : 'l1br3', 
     'host' : 'https://api.reveng.ai'
 }
 
 def reveng_req(r: requests.request, end_point: str, data=None, ex_headers: dict = None, params=None):
@@ -69,16 +71,15 @@
     """
     res = reveng_req(requests.get, f"embeddings/{binary_id(fpath)}")
     if res.status_code == 425:
         print(f"[-] Analysis for {binary_id(fpath)} still in progress. Please check the logs (-l) and try again later.")
         return
 
     res.raise_for_status()
-    embeddings = res.json()
-    print_json(data=embeddings)
+    return res.json()
 
 
 def RE_logs(fpath: str):
     """
         Delete analysis results for Binary ID in command
     """
     bin_id = binary_id(fpath)
@@ -89,20 +90,42 @@
     elif res.status_code == 404:
         print(f"[!] Error, binary analysis for {bin_id} not found.")
         return
 
     res.raise_for_status()
 
 
+def RE_compute_distance(embedding: list, fpath_source: str, nns: int = 5):
+    """
+        Comput ecosine distance between source embedding and embeddinsg from binary
+    """
+    embeddings = RE_embeddings(fpath_source)
+    df = pd.DataFrame(data=embeddings)
+    np_embedding = np.array(embedding).reshape(1, -1)
+    source_embeddings = np.vstack(df['embedding'].values)
+    closest = cosine_similarity(source_embeddings, np_embedding).squeeze().argsort()[::-1][:nns]
+    distances = cosine_similarity(source_embeddings[closest], np_embedding)
+    # match closest embeddings with similarity
+    closest_df = df.iloc[closest]
+    # create json similarity object
+    similarities = list(zip(distances, closest_df.index.tolist()))
+    json_sims = [{'similaritiy': d[0], 'vaddr': v} for d, v in similarities]
+    return json_sims
+
+
 def RE_nearest_symbols(embedding: list, nns: int = 5):
     """
         Get function name suggestions for an embedding
         :param nns: Number of nearest neighbors
+        :param source: Binary file to search embeddings from
     """
-    res = reveng_req(requests.post, "ann", data=json.dumps(embedding), params={'nns': nns})
+    params={'nns': nns}
+    if source:
+        params['source'] = source
+    res = reveng_req(requests.post, "ann", data=json.dumps(embedding), params=params)
     res.raise_for_status()
     f_suggestions = res.json()
     print_json(data=f_suggestions)
 
 def binary_id(path: str):
     """Take the SHA-256 hash of binary file"""
     hf = sha256()
@@ -134,22 +157,23 @@
 
 if __name__ == '__main__':
     parse_config()
     parser = ArgumentParser()
     parser.add_argument("-b", "--binary", default="", help="Path on binary to analyse")
     parser.add_argument("-a", "--analyse", action='store_true', help="Analyse new binary")
     parser.add_argument("-n", "--ann", action='store_true', help="Fetch Approximate Nearest Neighbours (ANNs) for embedding")
-    parser.add_argument("-e", "--embedding", help="Path of JSON file containing a BinNet embedding")
-    parser.add_argument("-m", "--model", default="BinNet", help="AI model used to generate embeddings")
+    parser.add_argument("--embedding", help="Path of JSON file containing a BinNet embedding")
+    parser.add_argument("--nns", default="5", help="Number of approximate nearest neighbors to fetch")
+    parser.add_argument("--found-in", help="ANN flag to limit to embeddings returned to those found in specific binary")
+    # parser.add_argument("-m", "--model", default="BinNet", help="AI model used to generate embeddings")
     parser.add_argument("-x", "--extract", action='store_true', help="Fetch embeddings for binary")
     parser.add_argument("-l", "--logs", action='store_true', help="Fetch analysis log file for binary")
     parser.add_argument("-d", "--delete", action='store_true', help="Securely delete all analyses and metadata associated with binary")
     parser.add_argument("-k", "--apikey", help="RevEng.AI API key")
     parser.add_argument("-s", "--host", help="Analysis Host. Defaults to https://api.reveng.ai")
-    parser.add_argument("--nns", default="5", help="Number of approximate nearest neighbors to fetch")
     parser.add_argument("-v", "--version", action="store_true", help="Display version information")
     args = parser.parse_args()
 
     if args.apikey:
         re_conf['apikey'] = args.apikey
     if args.host:
         re_conf['host'] = args.host
@@ -166,25 +190,36 @@
             parser.print_help()
             exit(-1)
 
     if args.analyse:
         RE_analyse(args.binary)
 
     elif args.extract:
-        RE_embeddings(args.binary)
+        embeddings = RE_embeddings(args.binary)
+        print_json(data=embeddings)
 
     elif args.ann:
+        source = None
         # parse embedding json file
         if not isfile(args.embedding):
             print("[!] Error, please supply a valid embedding JSON file using '-e'")
             parser.print_help()
             exit(-1)
 
         embedding = json.loads(open(args.embedding, 'r').read())
-        RE_nearest_symbols(embedding, int(args.nns))
+
+        if args.found_in:
+            if not os.path.isfile(args.found_in):
+                print("[!] Error, --found-in flag requires a path to a binary to search from")
+                exit(-1)
+            print(f"[+] Searching for symbols similar to embedding in binary {args.found_in}")
+            res = RE_compute_distance(embedding, args.found_in, int(args.nns))
+            print_json(data=res)
+        else:
+            RE_nearest_symbols(embedding, int(args.nns))
 
     elif args.logs:
         RE_logs(args.binary)
 
     elif args.delete:
         RE_delete(args.binary)
```

### Comparing `reait-0.0.7/reait.egg-info/PKG-INFO` & `reait-0.0.9/reait.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: reait
-Version: 0.0.7
+Version: 0.0.9
 Home-page: https://github.com/RevEng-AI/reait
 Project-URL: Homepage, https://github.com/RevEng-AI/reait
 Project-URL: Bug Tracker, https://github.com/RevEng-AI/reait/issues
 Project-URL: Organisation Homepage, https://reveng.ai
 Project-URL: Documentation, https://docs.reveng.ai
-Keywords: reverse,engineering,reveng.ai,reveng,machine,learning,binary,analysis,ml,ai
+Keywords: reverse,engineering,reveng.ai,reveng,machine,learning,binary,analysis,ml,ai,vector,embedding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # reait
@@ -52,14 +52,22 @@
 ### Search for similar symbols based on JSON embedding file
 To query our database of similar symbols based on an embedding, use `-n` to search using Approximate Nearest Neighbours. The `--nns` allows you to specify the number of results returned. A list of symbol names and the distance between each vector is returned. 
 
 `reait -e embedding.json -n`
 
 NB: A smaller distance indicates a higher degree of similarity.
 
+#### Limited Search
+To search for the most similar symbols found in a binary to a specific embedding, use the `--found-in` option with a path to the executable.
+
+`reait -n --embedding /tmp/sha256_init.json --found-in ~/malware.exe` 
+
+This downloads embeddings from `malware.exe` and computes the cosine similarity between all symbols and `sha256_init.json`. The returned results lists the most similar results by cosine similarity score (1.0 most similar, -1.0, dissimilar).
+
+
 ## Configuration
 
 `reait` reads the config file stored at `~/.reait.toml`. An example config file looks like:
 
 ```
 apikey = "l1br3"
 host = "https://api.reveng.ai"
```

### Comparing `reait-0.0.7/setup.py` & `reait-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
         name="reait",
-        version="0.0.7",
+        version="0.0.9",
         scripts=['reait'],
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/RevEng-AI/reait",
         packages=setuptools.find_packages(),
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
             "Operating System :: OS Independent"
             ],
         install_requires=[
-                'tqdm', 'argparse', 'requests', 'rich', 'tomli'
+                'tqdm', 'argparse', 'requests', 'rich', 'tomli', 'sklearn', 'pandas', 'numpy'
             ]
         )
```

