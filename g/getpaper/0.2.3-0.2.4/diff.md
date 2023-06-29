# Comparing `tmp/getpaper-0.2.3.tar.gz` & `tmp/getpaper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.2.3.tar", last modified: Thu Jun 29 11:13:22 2023, max compression
+gzip compressed data, was "getpaper-0.2.4.tar", last modified: Thu Jun 29 13:17:31 2023, max compression
```

## Comparing `getpaper-0.2.3.tar` & `getpaper-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 11:13:22.457812 getpaper-0.2.3/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.2.3/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5155 2023-06-29 11:13:22.457812 getpaper-0.2.3/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4540 2023-06-29 07:41:46.000000 getpaper-0.2.3/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 11:13:22.457812 getpaper-0.2.3/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.2.3/getpaper/__init__.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.2.3/getpaper/clean.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1020 2023-06-29 07:49:25.000000 getpaper-0.2.3/getpaper/config.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12419 2023-06-29 11:13:03.000000 getpaper-0.2.3/getpaper/download.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6845 2023-06-29 10:57:47.000000 getpaper-0.2.3/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12854 2023-06-29 07:52:58.000000 getpaper-0.2.3/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5052 2023-06-29 10:54:05.000000 getpaper-0.2.3/getpaper/splitting.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 11:13:22.457812 getpaper-0.2.3/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5155 2023-06-29 11:13:22.000000 getpaper-0.2.3/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-06-29 11:13:22.000000 getpaper-0.2.3/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-29 11:13:22.000000 getpaper-0.2.3/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-29 11:13:22.000000 getpaper-0.2.3/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      233 2023-06-29 11:13:22.000000 getpaper-0.2.3/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-29 11:13:22.000000 getpaper-0.2.3/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-29 11:13:22.457812 getpaper-0.2.3/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1627 2023-06-29 10:58:29.000000 getpaper-0.2.3/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 13:17:31.175314 getpaper-0.2.4/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.2.4/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5155 2023-06-29 13:17:31.175314 getpaper-0.2.4/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4540 2023-06-29 07:41:46.000000 getpaper-0.2.4/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 13:17:31.175314 getpaper-0.2.4/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.2.4/getpaper/__init__.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.2.4/getpaper/clean.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1020 2023-06-29 07:49:25.000000 getpaper-0.2.4/getpaper/config.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12926 2023-06-29 13:16:29.000000 getpaper-0.2.4/getpaper/download.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6845 2023-06-29 10:57:47.000000 getpaper-0.2.4/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12854 2023-06-29 07:52:58.000000 getpaper-0.2.4/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5052 2023-06-29 10:54:05.000000 getpaper-0.2.4/getpaper/splitting.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-29 13:17:31.175314 getpaper-0.2.4/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5155 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      233 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-29 13:17:31.000000 getpaper-0.2.4/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-29 13:17:31.175314 getpaper-0.2.4/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1627 2023-06-29 12:53:37.000000 getpaper-0.2.4/setup.py
```

### Comparing `getpaper-0.2.3/LICENSE` & `getpaper-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/PKG-INFO` & `getpaper-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.2.3
+Version: 0.2.4
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.2.3/README.md` & `getpaper-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/getpaper/clean.py` & `getpaper-0.2.4/getpaper/clean.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/getpaper/config.py` & `getpaper-0.2.4/getpaper/config.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/getpaper/download.py` & `getpaper-0.2.4/getpaper/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -237,23 +237,41 @@
 def download_pubmed_command(pubmed: str, folder: str, skip_existing: bool, name: Optional[str]):
     where = Path(folder)
     where.mkdir(exist_ok=True, parents=True)
     custom_name = pubmed if name == "pmid" or name == "PMID" else name
     return download_pubmed(pubmed, where, skip_existing, custom_name)
 
 
+def get_access(
+        sch: SemanticScholar,
+        paper_ids: List[str],
+        fields: Optional[List[str]] = None
+) -> List[dict]:
+    if fields is None:
+        fields = ["externalIds", "isOpenAccess", "openAccessPdf", "title", "year"]
+
+    url = f'{sch.api_url}/paper/batch'
+
+    fields = ','.join(fields)
+    parameters = f'&fields={fields}'
+    payload = { "ids": paper_ids }
+
+    data = sch._requester.get_data(url, parameters, sch.auth_header, payload)
+    return [item for item in data if item is not None]
+
+
 def check_access(dois: List[str]) ->(List[Paper], List[Paper]):
     sch = SemanticScholar()
-    fetched = sch.get_papers(dois, ["openAccessPdf"])
-    logger.info(f"FETCHED {fetched}")
-    papers = seq(sch.get_papers(dois, ["openAccessPdf"]))
-    result = papers.partition(lambda p: "openAccessPdf" in p.raw_data and p.raw_data["openAccessPdf"] is not None and "url" in p.raw_data["openAccessPdf"]).to_list()
+    papers_list = get_access(sch, dois)
+    papers = seq(papers_list)
+    result = papers.partition(lambda p: "openAccessPdf" in p and p["openAccessPdf"] is not None and "url" in p["openAccessPdf"])
     opened = result[0].to_list()
     closed = result[1].to_list()
-    logger.info(f"{len(result[0].to_list())} papers out of {len(papers.to_list())}")
+    failed = len(dois) - len(papers_list)
+    logger.info(f"{len(result[0].to_list())} papers out of {len(dois)}{' out of which ' + str(failed) + ' were not found' if failed >0 else ''}")
     return opened, closed
 
 @app.command("access")
 @click.option('--dois', multiple=True)
 @click.option('--log_level', type=click.Choice(LOG_LEVELS, case_sensitive=False), default="debug", help="logging level")
 def check_access_command(dois: List[str],  log_level: str):
     configure_logger(log_level)
```

### Comparing `getpaper-0.2.3/getpaper/index.py` & `getpaper-0.2.4/getpaper/index.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/getpaper/parse.py` & `getpaper-0.2.4/getpaper/parse.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/getpaper/splitting.py` & `getpaper-0.2.4/getpaper/splitting.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.3/getpaper.egg-info/PKG-INFO` & `getpaper-0.2.4/getpaper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.2.3
+Version: 0.2.4
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.2.3/setup.py` & `getpaper-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

