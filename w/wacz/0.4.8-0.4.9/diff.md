# Comparing `tmp/wacz-0.4.8.tar.gz` & `tmp/wacz-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wacz-0.4.8.tar", last modified: Fri Feb 24 03:10:15 2023, max compression
+gzip compressed data, was "wacz-0.4.9.tar", last modified: Thu Jun 29 16:42:54 2023, max compression
```

## Comparing `wacz-0.4.8.tar` & `wacz-0.4.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:10:15.035038 wacz-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-24 03:10:07.000000 wacz-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-02-24 03:10:15.035038 wacz-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-02-24 03:10:07.000000 wacz-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 03:10:15.035038 wacz-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-24 03:10:07.000000 wacz-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:10:15.035038 wacz-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_create_wacz.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_create_wacz_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_optional_flags_wacz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_validate_wacz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_verify_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-24 03:10:07.000000 wacz-0.4.8/tests/test_wacz_indexer_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:10:15.035038 wacz-0.4.8/wacz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 03:10:07.000000 wacz-0.4.8/wacz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-24 03:10:07.000000 wacz-0.4.8/wacz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-02-24 03:10:07.000000 wacz-0.4.8/wacz/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-24 03:10:07.000000 wacz-0.4.8/wacz/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-02-24 03:10:07.000000 wacz-0.4.8/wacz/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-02-24 03:10:07.000000 wacz-0.4.8/wacz/waczindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 03:10:15.035038 wacz-0.4.8/wacz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-02-24 03:10:14.000000 wacz-0.4.8/wacz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-24 03:10:15.000000 wacz-0.4.8/wacz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 03:10:14.000000 wacz-0.4.8/wacz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 03:10:14.000000 wacz-0.4.8/wacz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-24 03:10:14.000000 wacz-0.4.8/wacz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 03:10:14.000000 wacz-0.4.8/wacz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 03:10:14.000000 wacz-0.4.8/wacz.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.841309 wacz-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 16:42:43.000000 wacz-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-29 16:42:54.841309 wacz-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-29 16:42:43.000000 wacz-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:42:54.841309 wacz-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-29 16:42:43.000000 wacz-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.837309 wacz-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_create_wacz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_create_wacz_hash_in_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_create_wacz_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_optional_flags_wacz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_validate_wacz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_verify_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_wacz_indexer_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.841309 wacz-0.4.9/wacz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/waczindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.841309 wacz-0.4.9/wacz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/zip-safe
```

### Comparing `wacz-0.4.8/LICENSE` & `wacz-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/PKG-INFO` & `wacz-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wacz
-Version: 0.4.8
+Version: 0.4.9
 Summary: WACZ Format Tools
 Home-page: https://github.com/webrecorder/py-wacz
 Author: Ilya Kreymer, Emma Dickson
 Author-email: info@webrecorder.net
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -88,14 +88,22 @@
 
 You can add a full text index by including the --text tag.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl --text
 ```
 
+### -l --log-directory
+
+Adds log files in specified directory to WACZ
+
+```
+wacz create tests/fixtures/example-collection.warc -l tests/fixtures/logs
+```
+
 ### --ts
 
 Overrides the ts metadata value in the datapackage.json file.
 
 ```
 wacz create tests/fixtures/example-collection.warc --ts TIMESTAMP
 ```
@@ -163,15 +171,15 @@
 
 ### --verify-auth
 
 New option in 0.4.0, this option also verifies the WACZ is signed, using [authsign](https://github.com/webrecorder/authsign)
 
 The verification can be done locally, or via remote signing/verification server.
 
-To use remote server, add `--verify-url` which should be a URL pointing to the authsign `/verify` endpoint.
+To use remote server, add `--verifier-url` which should be a URL pointing to the authsign `/verify` endpoint.
 
 To run locally, the `authsign` must be installed, which can be done by running `pip install wacz[signing]`.
 
 See [WACZ Authentication Spec](https://github.com/webrecorder/wacz-auth-spec) on WACZ authentication.
 
 This feature and the specification are still in development (alpha-quality) and are subject to change.
```

### Comparing `wacz-0.4.8/README.md` & `wacz-0.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,22 @@
 
 You can add a full text index by including the --text tag.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl --text
 ```
 
+### -l --log-directory
+
+Adds log files in specified directory to WACZ
+
+```
+wacz create tests/fixtures/example-collection.warc -l tests/fixtures/logs
+```
+
 ### --ts
 
 Overrides the ts metadata value in the datapackage.json file.
 
 ```
 wacz create tests/fixtures/example-collection.warc --ts TIMESTAMP
 ```
@@ -150,15 +158,15 @@
 
 ### --verify-auth
 
 New option in 0.4.0, this option also verifies the WACZ is signed, using [authsign](https://github.com/webrecorder/authsign)
 
 The verification can be done locally, or via remote signing/verification server.
 
-To use remote server, add `--verify-url` which should be a URL pointing to the authsign `/verify` endpoint.
+To use remote server, add `--verifier-url` which should be a URL pointing to the authsign `/verify` endpoint.
 
 To run locally, the `authsign` must be installed, which can be done by running `pip install wacz[signing]`.
 
 See [WACZ Authentication Spec](https://github.com/webrecorder/wacz-auth-spec) on WACZ authentication.
 
 This feature and the specification are still in development (alpha-quality) and are subject to change.
```

### Comparing `wacz-0.4.8/setup.py` & `wacz-0.4.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # vim: set sw=4 et:
 from setuptools import setup, find_packages
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 def load_requirements(filename):
     with open(filename, "rt") as fh:
         return fh.read().rstrip().split("\n")
 
 def long_description():
     with open("README.md") as f:
```

### Comparing `wacz-0.4.8/tests/test_create_wacz.py` & `wacz-0.4.9/tests/test_create_wacz.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/tests/test_create_wacz_indexing.py` & `wacz-0.4.9/tests/test_create_wacz_indexing.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/tests/test_optional_flags_wacz.py` & `wacz-0.4.9/tests/test_optional_flags_wacz.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/tests/test_util.py` & `wacz-0.4.9/tests/test_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         test_hash = "md5:%s" % hashlib.md5("test".encode("utf-8")).hexdigest()
         bytes_, hash_ = hash_stream("md5", BytesIO("test".encode("utf-8")))
         self.assertEqual(bytes_, 4)
         self.assertEqual(hash_, test_hash)
 
     def test_util_validate_json_succeed(self):
-        """validate json method should succed with valid json"""
+        """validate json method should succeed with valid json"""
         self.assertTrue(validateJSON('{"test": "test"}'))
 
     def test_util_validate_json_fail(self):
         """validate json method should fail with valid json"""
         self.assertFalse(validateJSON('test": "test"}'))
```

### Comparing `wacz-0.4.8/tests/test_validate_wacz.py` & `wacz-0.4.9/tests/test_validate_wacz.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/tests/test_verify_signed.py` & `wacz-0.4.9/tests/test_verify_signed.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/tests/test_wacz_indexer_functions.py` & `wacz-0.4.9/tests/test_wacz_indexer_functions.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/wacz/main.py` & `wacz-0.4.9/wacz/main.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/wacz/util.py` & `wacz-0.4.9/wacz/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,18 +68,19 @@
             page_dict = json.loads(page_data)
         except:
             print("Warning: Skipping invalid page {0}".format(page_data))
             continue
 
         # Skip the file's header if it's been set
         if "format" not in page_dict:
-            url = page_dict.pop("url", "")
+            url = page_dict.get("url", "")
 
-            # Set the default key as url
-            key = url
+            # Set the default key as url, but without hashtag, as will match pages
+            # to URLs without hashtag, but keep hashtag on page list
+            key = url.split("#", 1)[0]
 
             # If timestamp is present overwrite the key to be 'ts/url'
             if "ts" in page_dict:
                 key = iso_date_to_timestamp(page_dict.pop("ts")) + "/" + url
 
             # Add the key to the dictionary with remaining data
             passed_pages_dict[key] = page_dict
```

### Comparing `wacz-0.4.8/wacz/validate.py` & `wacz-0.4.9/wacz/validate.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.8/wacz/waczindexer.py` & `wacz-0.4.9/wacz/waczindexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,27 +201,25 @@
 
         # if id_ in self.passed_pages_dict:
         #    matched_id = id_
 
         matched_id = check_http_and_https(url, ts, self.passed_pages_dict)
         # If we find a match build a record
         if matched_id:
-            new_page = {"timestamp": ts, "url": url, "title": url}
-            input_page = self.passed_pages_dict[matched_id]
+            page_data = self.passed_pages_dict[matched_id]
+            page_data["timestamp"] = ts
+            if "url" not in page_data:
+                page_data["url"] = url
+            if "title" not in page_data:
+                page_data["title"] = url
 
-            # Add title and text if they've been provided
-            if "title" in input_page:
-                new_page["title"] = input_page["title"]
-            if "text" in self.passed_pages_dict[matched_id]:
-                new_page["text"] = input_page["text"]
-
-            if self.split_seeds and not input_page.get("seed"):
-                self.extra_pages[matched_id] = new_page
+            if self.split_seeds and not page_data.get("seed"):
+                self.extra_pages[matched_id] = page_data
             else:
-                self.pages[matched_id] = new_page
+                self.pages[matched_id] = page_data
 
             # Delete the entry from our pages_dict so we can't match it again
             del self.passed_pages_dict[matched_id]
 
         if (
             self.main_url
             and self.main_url == url
@@ -330,28 +328,22 @@
 
         if has_text:
             page_header["hasText"] = True
 
         yield json.dumps(page_header) + "\n"
 
         for line in pages:
-            ts = timestamp_to_iso_date(line["timestamp"])
-            page_title = line.get("title")
-
-            uid = line.get("id") or line.get("page_id") or shortuuid.uuid()
-
-            data = {"id": uid, "url": line["url"], "ts": ts}
-
-            if page_title:
-                data["title"] = page_title
+            if "ts" not in line and "timestamp" in line:
+                ts = timestamp_to_iso_date(line["timestamp"])
+                line["ts"] = ts
+                del line["timestamp"]
 
-            if "text" in line:
-                data["text"] = line["text"]
+            line["id"] = line.get("id") or line.get("page_id") or shortuuid.uuid()
 
-            yield json.dumps(data) + "\n"
+            yield json.dumps(line) + "\n"
 
     def generate_datapackage(self, res, wacz):
         package_dict = {}
 
         package_dict["profile"] = "data-package"
 
         resources = []
```

### Comparing `wacz-0.4.8/wacz.egg-info/PKG-INFO` & `wacz-0.4.9/wacz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wacz
-Version: 0.4.8
+Version: 0.4.9
 Summary: WACZ Format Tools
 Home-page: https://github.com/webrecorder/py-wacz
 Author: Ilya Kreymer, Emma Dickson
 Author-email: info@webrecorder.net
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -88,14 +88,22 @@
 
 You can add a full text index by including the --text tag.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl --text
 ```
 
+### -l --log-directory
+
+Adds log files in specified directory to WACZ
+
+```
+wacz create tests/fixtures/example-collection.warc -l tests/fixtures/logs
+```
+
 ### --ts
 
 Overrides the ts metadata value in the datapackage.json file.
 
 ```
 wacz create tests/fixtures/example-collection.warc --ts TIMESTAMP
 ```
@@ -163,15 +171,15 @@
 
 ### --verify-auth
 
 New option in 0.4.0, this option also verifies the WACZ is signed, using [authsign](https://github.com/webrecorder/authsign)
 
 The verification can be done locally, or via remote signing/verification server.
 
-To use remote server, add `--verify-url` which should be a URL pointing to the authsign `/verify` endpoint.
+To use remote server, add `--verifier-url` which should be a URL pointing to the authsign `/verify` endpoint.
 
 To run locally, the `authsign` must be installed, which can be done by running `pip install wacz[signing]`.
 
 See [WACZ Authentication Spec](https://github.com/webrecorder/wacz-auth-spec) on WACZ authentication.
 
 This feature and the specification are still in development (alpha-quality) and are subject to change.
```

### Comparing `wacz-0.4.8/wacz.egg-info/SOURCES.txt` & `wacz-0.4.9/wacz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/test_create_wacz.py
+tests/test_create_wacz_hash_in_page.py
 tests/test_create_wacz_indexing.py
 tests/test_optional_flags_wacz.py
 tests/test_util.py
 tests/test_validate_wacz.py
 tests/test_verify_signed.py
 tests/test_wacz_indexer_functions.py
 wacz/__init__.py
```

