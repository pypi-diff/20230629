# Comparing `tmp/hydrusvideodeduplicator-0.1.8.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.9.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.8.tar` & `hydrusvideodeduplicator-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    13565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/README.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/README.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 import hydrusvideodeduplicator.hydrus_api.utils
 from tqdm import tqdm
 from rich import print as rprint
 from sqlitedict import SqliteDict
 
 from .config import DEDUP_DATABASE_FILE, DEDUP_DATABASE_DIR, DEDUP_DATABASE_NAME
-from .dedup_util import find_tag_in_tags, get_file_names_hydrus
+from .dedup_util import find_tag_in_tags, get_file_names_hydrus, cleanup_defunct_processes
 from .vpdq import VPDQSignal
 
 from .vpdq_util import (
     VPDQ_QUERY_MATCH_THRESHOLD_PERCENT,
 )
 
 class HydrusVideoDeduplicator():
@@ -67,15 +67,15 @@
         if not skip_hashing:
             self._add_perceptual_hashes_to_db(overwrite=overwrite, custom_query=custom_query)
         else:
             rprint("[yellow] Skipping perceptual hashing")
 
         self._find_potential_duplicates()
         self.hydlog.info("Deduplication done.")
-    
+
     @classmethod
     # dir is where you're writing the video file
     def _add_perceptual_hash_to_db(cls, video_hash: str, video: str | bytes, video_dir: Path | str, db) -> None:
         with tempfile.NamedTemporaryFile(mode="w+b", dir=video_dir) as tmp_vid_file:
             # Write video to file to be able to calculate hash
             tmp_vid_file.write(video)
             tmp_vid_file.seek(0)
@@ -123,20 +123,21 @@
                         ]
 
                         # Execute the ffmpeg command
                         with open(os.devnull, "w") as devnull: subprocess.call(ffmpeg_cmd, stdout=devnull, stderr=devnull)
 
                         perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file_transcoded.name)
 
-                        print("[yellow] Fallback to transcode successful.")
+                        rprint("[yellow] Fallback to transcode successful.")
                 except:
-                    print("[red] Transcode and/or hashing the transcode failed.")
+                    rprint("[red] Transcode and/or hashing the transcode failed.")
             else:
                 perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
 
+            
             row = db.get(video_hash, {})
             row["perceptual_hash"] = perceptual_hash
             db[video_hash] = row
             cls.hydlog.debug(f"Perceptual hash calculated and added to DB.")
     
     # Add perceptual hash for videos to the database
     def _add_perceptual_hashes_to_db(self, overwrite: bool, custom_query: list | None = None) -> None:
@@ -152,15 +153,15 @@
             self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
 
         search_tags = ["system:filetype=video"]
         if custom_query is not None:
             custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
             search_tags.extend(custom_query)
         
-        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos") as hashdb:
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos",autocommit=True) as hashdb:
             print(f"Retrieving video file hashes...")
             all_video_hashes = self.client.search_files(search_tags, file_sort_type=hydrus_api.FileSortType.FILE_SIZE, return_hashes=True, file_sort_asc=True, return_file_ids=False)["hashes"]
             print("Calculating perceptual hashes:")
             with tqdm(dynamic_ncols=True, total=len(all_video_hashes), unit="video", colour="BLUE") as pbar:
                 with tempfile.TemporaryDirectory() as tmp_dir_name:
                     for chunk_video_hashes in hydrus_api.utils.yield_chunks(all_video_hashes, chunk_size=16):
                         for video_hash in chunk_video_hashes:
@@ -185,14 +186,18 @@
                                 return None
                             except:
                                 rprint("[red] Failed to calculate a perceptual hash.")
                                 self.hydlog.error(f"Errored file hash: {video_hash}")
                             
                         # Commit at the end of a chunk
                         hashdb.commit()
+                        
+                        # Each call to vpdq causes a defunct process because they didn't clean up the FFmpeg command in C++
+                        # Otherwise, the program will fill with zombie processes
+                        cleanup_defunct_processes()
 
             # Commit at the end of all processing
             hashdb.commit()
             
         rprint("[green] Finished perceptual hash processing.\n")
     
     def get_potential_duplicate_count_hydrus(self) -> int:
@@ -240,17 +245,17 @@
                         video2_phash = hashdb[video2_hash]["perceptual_hash"]
                         
                         similar = HydrusVideoDeduplicator.is_similar(video_phash, video2_phash, self.threshold)
                         
                         if similar:
                             similar_files_found_count += 1
                             if self._DEBUG:
-                                file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
-                                self.hydlog.info(f"Duplicates filenames: {file_names}")
-                                #self.hydlog.info(f"\"Duplicates hashes: {video_hash}\" and \"{video2_hash}\"")
+                                #file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
+                                #self.hydlog.info(f"Duplicates filenames: {file_names}")
+                                self.hydlog.info(f"\"Duplicates hashes: {video_hash}\" and \"{video2_hash}\"")
                             
                             new_relationship = {
                                 "hash_a": str(video_hash),
                                 "hash_b": str(video2_hash),
                                 "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
                                 "do_default_content_merge": True,
                             }
```

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from datetime import datetime
 import time
+import os
 
 from hydrusvideodeduplicator.hydrus_api import Client
  
 # Given a lexicographically SORTED list of tags, find the tag given a namespace
 # TODO: Do binary search since the tags are sorted
 def find_tag_in_tags(target_tag_namespace: str, tags: list) -> str:
     namespace_len = len(target_tag_namespace)
@@ -17,34 +18,32 @@
 # This is just used for debugging.
 # TODO: Clean this up it's a mess
 def get_file_names_hydrus(client: Client, file_hashes: list[str]) -> list[str]:
     err_msg = "Cannot get file name from Hydrus."
     result = []
     files_metadata = client.get_file_metadata(hashes=file_hashes, only_return_basic_information=False)
     all_known_tags = "all known tags".encode("utf-8").hex()
-    for file_metadata in files_metadata["metadata"]:
+    for file_metadata in files_metadata.get("metadata", []):
         # Try to get file extension
         try:
             ext = file_metadata["ext"]
         except KeyError:
             ext = ""
             
         # Try to get the file name
+        tag = ""
         try:
             tag_services = file_metadata["tags"]
-        except KeyError:
-            logging.warning(f"{err_msg} Hash: {file_metadata['hash']}")
-        else:
             tags = tag_services[all_known_tags]["storage_tags"]["0"]
             tag = find_tag_in_tags(target_tag_namespace="filename:", tags=tags)
             # Don't show extension if filename doesn't exist
             if tag != "":
                 tag = f"{tag}{ext}"
-            else:
-                logging.warning(f"{err_msg} Hash: {file_metadata['hash']}")
+        except:
+            logging.warning(f"{err_msg} Hash: {file_metadata['hash']}")
 
         result.append(tag)
 
     return result
 
 # Get the oldest file by import time in list of file_metadata 
 def get_oldest_imported_file_time(all_files_metadata: list) -> int:
@@ -107,8 +106,17 @@
     return {
         'years': int(years()[0]),
         'days': int(days()[0]),
         'hours': int(hours()[0]),
         'minutes': int(minutes()[0]),
         'seconds': int(seconds()),
         'default': totalDuration()
-    }[interval]        
+    }[interval]        
+
+def cleanup_defunct_processes():
+    while True:
+        try:
+            pid, status = os.waitpid(-1, os.WNOHANG)
+            if pid == 0:  # No more defunct processes
+                break
+        except ChildProcessError:
+            break  # No more child processes
```

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/.gitignore` & `hydrusvideodeduplicator-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/LICENSE` & `hydrusvideodeduplicator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/README.md` & `hydrusvideodeduplicator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/pyproject.toml` & `hydrusvideodeduplicator-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.8/PKG-INFO` & `hydrusvideodeduplicator-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
```

