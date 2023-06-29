# Comparing `tmp/nc_py_api-0.0.10.tar.gz` & `tmp/nc_py_api-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.10.tar", last modified: Sat Jan 14 11:22:01 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.11.tar", last modified: Wed Mar 22 16:52:12 2023, max compression
```

## Comparing `nc_py_api-0.0.10.tar` & `nc_py_api-0.0.11.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 11:22:01.473364 nc_py_api-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-01-14 11:22:01.473364 nc_py_api-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 11:22:01.473364 nc_py_api-0.0.10/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/db_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/db_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/db_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/db_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/occ.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/nc_py_api/signal_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 11:22:01.473364 nc_py_api-0.0.10/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-01-14 11:22:01.000000 nc_py_api-0.0.10/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-01-14 11:22:01.000000 nc_py_api-0.0.10/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 11:22:01.000000 nc_py_api-0.0.10/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 11:21:52.000000 nc_py_api-0.0.10/nc_py_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-14 11:22:01.000000 nc_py_api-0.0.10/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-14 11:22:01.000000 nc_py_api-0.0.10/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-14 11:22:01.477364 nc_py_api-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-14 11:21:40.000000 nc_py_api-0.0.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/occ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:52:02.000000 nc_py_api-0.0.11/nc_py_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/setup.py
```

### Comparing `nc_py_api-0.0.10/LICENSE` & `nc_py_api-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/PKG-INFO` & `nc_py_api-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc_py_api
-Version: 0.0.10
+Version: 0.0.11
 Summary: Backend API for Python 3.9+ to work with Nextcloud
 Home-page: https://github.com/cloud-py-api/cloud-py-api
 Author: Alexander Piskun
 Author-email: bigcat88@users.noreply.github.com
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/cloud-py-api
 Keywords: nextcloud,api,framework
```

### Comparing `nc_py_api-0.0.10/README.md` & `nc_py_api-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/nc_py_api/config.py` & `nc_py_api-0.0.11/nc_py_api/config.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/nc_py_api/db_api.py` & `nc_py_api-0.0.11/nc_py_api/db_api.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/nc_py_api/db_connectors.py` & `nc_py_api-0.0.11/nc_py_api/db_connectors.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/nc_py_api/db_misc.py` & `nc_py_api-0.0.11/nc_py_api/db_misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         return CONFIG["dbtprefix"] + "filecache"
 
     @property
     def mimetypes(self) -> str:
         return CONFIG["dbtprefix"] + "mimetypes"
 
     @property
+    def users(self) -> str:
+        return CONFIG["dbtprefix"] + "users"
+
+    @property
     def settings(self) -> str:
         return CONFIG["dbtprefix"] + "cloud_py_api_settings"
 
 
 TABLES = Tables()
```

### Comparing `nc_py_api-0.0.10/nc_py_api/db_requests.py` & `nc_py_api-0.0.11/nc_py_api/db_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,7 +117,22 @@
 
 def get_non_direct_access_filesize_limit() -> int:
     query = f"SELECT value FROM {TABLES.settings} WHERE name='remote_filesize_limit';"
     result = execute_fetchall(query)
     if not result:
         return 256 * 1024 * 1024
     return int(result[0]["value"])
+
+
+def get_users() -> list[dict]:
+    """Returns `users` table as a list of dictionaries."""
+
+    return execute_fetchall(f"SELECT * FROM {TABLES.users};")
+
+
+def get_user(uid_lower: str) -> dict:
+    """Returns `user` table record as a dictionary."""
+
+    result = execute_fetchall(f"SELECT * FROM {TABLES.users} WHERE uid_lower='{uid_lower}';")
+    if result:
+        return result[0]
+    return {}
```

### Comparing `nc_py_api-0.0.10/nc_py_api/files.py` & `nc_py_api-0.0.11/nc_py_api/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,39 +48,46 @@
 
 USER_ID = environ.get("USER_ID", "")
 STORAGES_INFO = get_storages_info()
 ND_ACCESS_LIMIT = get_non_direct_access_filesize_limit()
 """A value from the config that defines the maximum file size allowed to be requested from php."""
 
 
-def fs_node_info(obj: Union[list[int], int, str], user_id=USER_ID) -> Union[list[FsNodeInfo], Optional[FsNodeInfo]]:
-    """Gets `FsNodeInfo` by list of ids, id or path.
+def fs_node_info(obj: Union[int, str], user_id=USER_ID) -> Optional[FsNodeInfo]:
+    """Gets `FsNodeInfo` by `fileid` or path.
 
-    :param obj: for the list of ints or one int it is a `fileid` value. For ``str`` type it is the
-    relative path to file/directory. `path` field from NC DB, without `files/` prefix.
+    :param obj: `fileid` value or ``str`` type if it is the
+    relative path to file/directory(`path` field from NC DB, without `files/` prefix).
     :param user_id: `uid` of user. Optional, in most cases you should not specify it.
 
-    :returns: list of :py:data:`FsNodeInfo`, :py:data:`FsNodeInfo` or None in case of error.
-     Depends on the type of `obj` parameter."""
+    :returns: :py:data:`FsNodeInfo` or None in case of error."""
 
-    if isinstance(obj, list):
-        return [db_record_to_fs_node(i) for i in get_fileids_info(obj)]
     if isinstance(obj, int):
         raw_result = get_fileid_info(obj)
     else:
         numeric_id = get_storage_by_user_id(user_id).get("numeric_id", 0)
         if not numeric_id:
             log.debug("can not find storage for specified user: %s", user_id)
             return None
         raw_result = get_fs_obj_info_by_path(path.join("files", obj.lstrip("/")).rstrip("/"), numeric_id)
     if raw_result:
         return db_record_to_fs_node(raw_result)
     return None
 
 
+def fs_nodes_info(file_ids: list[int]) -> list[FsNodeInfo]:
+    """Gets list of `FsNodeInfo` by list of file ids.
+
+    :param file_ids: list of `fileid`s for which get info.
+
+    :returns: list of :py:data:`FsNodeInfo`."""
+
+    return [db_record_to_fs_node(i) for i in get_fileids_info(file_ids)]
+
+
 def fs_list_directory(file_id: Optional[Union[int, FsNodeInfo]] = None, user_id=USER_ID) -> list[FsNodeInfo]:
     """Gets listing of the directory.
 
     :param file_id: `fileid` or :py:data:`FsNodeInfo` of the directory. Can be `None` to list `root` directory.
     :param user_id: `uid` of user. Optional, in most cases you should not specify it.
 
     :returns: list of :py:data:`FsNodeInfo` dictionaries."""
@@ -103,60 +110,87 @@
     if storage_id and internal_path:
         file_mounts = get_mounts_to(storage_id, internal_path)
     raw_result = get_directory_list(file_id, file_mounts)
     return [db_record_to_fs_node(i) for i in raw_result]
 
 
 def fs_apply_exclude_lists(fs_objs: list[FsNodeInfo], excl_file_ids: list[int], excl_mask: list[str]) -> None:
-    """Purge all records according to exclude_(mask/fileid) from `where_to_purge`(or from fs_records)."""
+    """Purge all records according to exclude_(mask/fileid).
+
+    :param fs_objs: list of :py:data:`FsNodeInfo` to which exclusion lists apply.
+    :param excl_file_ids: list of int, representing exclude masks fileids.
+    :param excl_mask: list of str, representing exclude masks. Comparison done using `fnmatch`."""
 
     indexes_to_purge = []
     for index, fs_obj in enumerate(fs_objs):
         if fs_obj["id"] in excl_file_ids:
             indexes_to_purge.append(index)
         elif is_path_in_exclude(fs_obj["internal_path"], excl_mask):
             indexes_to_purge.append(index)
     for index in reversed(indexes_to_purge):
         del fs_objs[index]
 
 
 def fs_extract_sub_dirs(fs_objs: list[FsNodeInfo]) -> list[FsNodeInfo]:
+    """Extracts and return all records with ``mimetype`` equal to ``DIR``.
+
+    :param fs_objs: list of :py:data:`FsNodeInfo` from which extract directory records. Will be edite in place.
+    :return: list of :py:data:`FsNodeInfo` that are directories."""
+
     sub_dirs = []
     indexes_to_purge = []
     for index, fs_obj in enumerate(fs_objs):
         if fs_obj["mimetype"] == mimetype.DIR:
             sub_dirs.append(fs_obj)
             indexes_to_purge.append(index)
     for index in reversed(indexes_to_purge):
         del fs_objs[index]
     return sub_dirs
 
 
 def fs_apply_ignore_flags(fs_objs: list[FsNodeInfo]) -> None:
+    """Check for ``.noimage``/``.nomedia`` flag and removes all records with `mimetype` equal to ``IMAGE/VIDEO``.
+
+    The flag also will be removed. The list will be edited in place.
+
+    :param fs_objs: list of :py:data:`FsNodeInfo`."""
+
     ignore_flag = any(fs_obj["name"] in (".noimage", ".nomedia") for fs_obj in fs_objs)
     if ignore_flag:
         fs_filter_by(fs_objs, "mimepart", [mimetype.IMAGE, mimetype.VIDEO], reverse_filter=True)
         fs_apply_exclude_lists(fs_objs, [], [".noimage", ".nomedia"])
 
 
 def fs_filter_by(fs_objs: list[FsNodeInfo], field: FsNodeInfoField, values: list, reverse_filter=False) -> None:
+    """Filter elements in FS list(in-place) by specified mask.
+
+    :param fs_objs: directory listing returned by :py:func:`~nc_py_api.fs_list_directory`.
+    :param field: value from :py:data:`FsNodeInfoField` on which the filter will be applied.
+    :param values: list of values to compare.
+    :param reverse_filter: a boolean indicating that the entry should be filtered if the value is present."""
+
     indexes_to_purge = []
     if reverse_filter:
         for index, fs_obj in enumerate(fs_objs):
             if fs_obj[field] in values:
                 indexes_to_purge.append(index)
     else:
         for index, fs_obj in enumerate(fs_objs):
             if fs_obj[field] not in values:
                 indexes_to_purge.append(index)
     for index in reversed(indexes_to_purge):
         del fs_objs[index]
 
 
 def fs_sort_by_id(fs_objs: list[FsNodeInfo]) -> list[FsNodeInfo]:
+    """Helper function, to sort list of `FsNodeInfo` in ascending order by `fileid`.
+
+    :param fs_objs: list of :py:data:`FsNodeInfo`.
+    :return: list of :py:data:`FsNodeInfo`."""
+
     return sorted(fs_objs, key=lambda i: i["id"])
 
 
 def fs_file_data(file_info: FsNodeInfo) -> bytes:
     if file_info["direct_access"]:
         try:
             with open(file_info["abs_path"], "rb") as h_file:
```

### Comparing `nc_py_api-0.0.10/nc_py_api/occ.py` & `nc_py_api-0.0.11/nc_py_api/occ.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.11/nc_py_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc-py-api
-Version: 0.0.10
+Version: 0.0.11
 Summary: Backend API for Python 3.9+ to work with Nextcloud
 Home-page: https://github.com/cloud-py-api/cloud-py-api
 Author: Alexander Piskun
 Author-email: bigcat88@users.noreply.github.com
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/cloud-py-api
 Keywords: nextcloud,api,framework
```

### Comparing `nc_py_api-0.0.10/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.11/nc_py_api.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 nc_py_api/db_misc.py
 nc_py_api/db_requests.py
 nc_py_api/files.py
 nc_py_api/log.py
 nc_py_api/mimetype.py
 nc_py_api/occ.py
 nc_py_api/signal_handler.py
+nc_py_api/users.py
 nc_py_api.egg-info/PKG-INFO
 nc_py_api.egg-info/SOURCES.txt
 nc_py_api.egg-info/dependency_links.txt
 nc_py_api.egg-info/not-zip-safe
 nc_py_api.egg-info/requires.txt
 nc_py_api.egg-info/top_level.txt
```

### Comparing `nc_py_api-0.0.10/pyproject.toml` & `nc_py_api-0.0.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.10/setup.cfg` & `nc_py_api-0.0.11/setup.cfg`

 * *Files identical despite different names*

