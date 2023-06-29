# Comparing `tmp/recurtx-0.0.4.tar.gz` & `tmp/recurtx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurtx-0.0.4.tar", last modified: Mon Jun 26 05:02:58 2023, max compression
+gzip compressed data, was "dist/recurtx-0.0.5.tar", last modified: Thu Jun 29 07:48:32 2023, max compression
```

## Comparing `recurtx-0.0.4.tar` & `recurtx-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:02:58.920000 recurtx-0.0.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-25 15:44:44.000000 recurtx-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-26 05:02:58.920000 recurtx-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5715 2023-06-25 15:44:44.000000 recurtx-0.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-25 15:44:44.000000 recurtx-0.0.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:02:58.910000 recurtx-0.0.4/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 15:44:44.000000 recurtx-0.0.4/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-25 15:44:44.000000 recurtx-0.0.4/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6686 2023-06-26 04:47:34.000000 recurtx-0.0.4/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-06-26 04:53:15.000000 recurtx-0.0.4/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-25 15:44:44.000000 recurtx-0.0.4/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-26 03:53:38.000000 recurtx-0.0.4/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-25 15:44:45.000000 recurtx-0.0.4/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 05:02:58.920000 recurtx-0.0.4/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      252 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-26 05:02:58.000000 recurtx-0.0.4/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-26 05:02:58.920000 recurtx-0.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1562 2023-06-25 15:44:45.000000 recurtx-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:48:32.000000 recurtx-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-26 05:04:07.000000 recurtx-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-29 07:48:32.000000 recurtx-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-06-26 05:04:07.000000 recurtx-0.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 05:04:07.000000 recurtx-0.0.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:48:32.000000 recurtx-0.0.5/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 05:04:08.000000 recurtx-0.0.5/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-29 05:58:08.000000 recurtx-0.0.5/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4043 2023-06-29 07:43:05.000000 recurtx-0.0.5/recurtx/ll.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-06-27 14:45:56.000000 recurtx-0.0.5/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-06-27 14:46:00.000000 recurtx-0.0.5/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-06-29 02:59:29.000000 recurtx-0.0.5/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-26 05:04:08.000000 recurtx-0.0.5/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-28 13:50:26.000000 recurtx-0.0.5/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:48:32.000000 recurtx-0.0.5/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-29 07:48:32.000000 recurtx-0.0.5/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-29 07:48:32.000000 recurtx-0.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1596 2023-06-29 05:57:26.000000 recurtx-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `recurtx-0.0.4/LICENSE` & `recurtx-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.4/PKG-INFO` & `recurtx-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.4/README.md` & `recurtx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.4/recurtx/__main__.py` & `recurtx-0.0.5/recurtx/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import fire
 
+from .ll import ll
 from .pandas import pandas
 from .polars import polars
 from .recur import batch, under
 from .search import find, search
 
 
 def main():
     fire.Fire(
         dict(
             batch=batch,
             pandas=pandas,
             polars=polars,
             find=find,
             search=search,
+            stat=stat,
             under=under,
         )
     )
 
 
 def xpandas():
     fire.Fire(pandas)
@@ -39,15 +41,20 @@
     fire.Fire(find)
 
 
 def xsearch():
     fire.Fire(search)
 
 
+def xll():
+    fire.Fire(ll)
+
+
 if __name__ == "__main__":
     main()
     xpandas()
     xpolars()
     xbatch()
     xunder()
     xfind()
     xsearch()
+    xstat()
```

### Comparing `recurtx-0.0.4/recurtx/pandas.py` & `recurtx-0.0.5/recurtx/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from pathlib import Path
 from typing import List
 
 from .utils import infer_type, stdout_lines
 
 DATA_TYPES = {
     "pickle",
```

### Comparing `recurtx-0.0.4/recurtx/polars.py` & `recurtx-0.0.5/recurtx/polars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from pathlib import Path
 from typing import List
 
 from .utils import infer_type, stdout_lines
 
 DATA_TYPES = {
     "csv",
```

### Comparing `recurtx-0.0.4/recurtx/recur.py` & `recurtx-0.0.5/recurtx/recur.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import sys
 from pathlib import Path
 
 from .utils import get_exception_msg, subprocess_run, upath
 
 
 def recur(
-    kind: str,
     path: str,
     *scripts: str,
     **kwargs: str,
 ):
     glob = kwargs.pop("glob", "**/*")
     regex = kwargs.pop(
         "regex",
         r"^(?!.*(\.git\/|__pycache__\/|\.ipynb_checkpoints\/|\.pytest_cache\/|\.vscode\/|\.idea\/|\.DS_Store)).*$",
     )
-    reverse = kwargs.pop("reverse", False)
+    type = kwargs.pop("type", "file")
+    sort_paths = kwargs.pop("sort_paths", "asc")
     replace_str = kwargs.pop("replace_str", "@@")
     show_paths = kwargs.pop("show_paths", False)
     show_scripts = kwargs.pop("show_scripts", False)
 
     if regex:
         rx = re.compile(regex)
     else:
@@ -53,89 +53,83 @@
 
     path = Path(upath(path))
     assert path.exists(), str(path.resolve()) + " does not exist."
 
     if path.is_file():
         path_ls = [str(path)]
     else:
-        path_ls = [str(p) for p in path.glob(glob) if p.is_file()]
+        path_ls = [str(p) for p in path.glob(glob) if getattr(p, "is_" + type)()]
         if rx:
             path_ls = [p for p in path_ls if rx.match(p)]
-        path_ls.sort(reverse=reverse)
+        if sort_paths:
+            assert isinstance(sort_paths, str), sort_paths
+            path_ls.sort(reverse=(sort_paths.lower().startswith("desc")))
 
     if show_paths:
         sys.stdout.write(
             "[Searching files]\n" + str("\n".join(["    " + p for p in path_ls]) + "\n")
         )
-
-    running_scripts = scripts
-    if kind == "under":
-        for p in path_ls:
-            try:
-                if replace_str:
-                    running_scripts = [
-                        script.replace(replace_str, p)
-                        if isinstance(script, str)
-                        else script
-                        for script in scripts
-                    ]
-                if len(running_scripts) == 1:
-                    running_scripts = running_scripts[0]
-                subprocess_run(running_scripts, show_scripts)
-            except Exception:
-                msg = get_exception_msg()
-                sys.stdout.write(msg)
-                continue
-
-    elif kind == "batch":
-        if len(scripts) == 1:
-            running_scripts = scripts[0]
-            if replace_str:
-                running_scripts = running_scripts.replace(
-                    replace_str, " ".join(path_ls)
-                )
-        else:
-            running_scripts = []
-            for script in scripts:
-                if replace_str and (script == replace_str):
-                    running_scripts.extend(path_ls)
-                else:
-                    running_scripts.append(script)
-        try:
-            subprocess_run(running_scripts, show_scripts)
-        except Exception:
-            msg = get_exception_msg()
-            sys.stdout.write(msg)
-    else:
-        raise NotImplementedError()
+    return path_ls, scripts, replace_str, show_scripts
 
 
 def under(
     path: str,
     *scripts: str,
     **kwargs: str,
 ):
     """Run any scripts for each file under a directory recursively."""
 
-    kind = "under"
-    recur(
-        kind,
+    path_ls, scripts, replace_str, show_scripts = recur(
         path,
         *scripts,
         **kwargs,
     )
 
+    running_scripts = scripts
+    for p in path_ls:
+        try:
+            if replace_str:
+                running_scripts = [
+                    script.replace(replace_str, p)
+                    if isinstance(script, str)
+                    else script
+                    for script in scripts
+                ]
+            if len(running_scripts) == 1:
+                running_scripts = running_scripts[0]
+            subprocess_run(running_scripts, show_scripts)
+        except Exception:
+            msg = get_exception_msg()
+            sys.stdout.write(msg)
+            continue
+
 
 def batch(
     path: str,
     *scripts: str,
     **kwargs: str,
 ):
     """Run any scripts for a batch of files in a directory recursively."""
 
-    kind = "batch"
-    recur(
-        kind,
+    path_ls, scripts, replace_str, show_scripts = recur(
         path,
         *scripts,
         **kwargs,
     )
+
+    running_scripts = scripts
+    if len(scripts) == 1:
+        running_scripts = scripts[0]
+        if replace_str:
+            running_scripts = running_scripts.replace(replace_str, " ".join(path_ls))
+    else:
+        running_scripts = []
+        for script in scripts:
+            if replace_str and (script == replace_str):
+                running_scripts.extend(path_ls)
+            else:
+                running_scripts.append(script)
+    try:
+        subprocess_run(running_scripts, show_scripts)
+    except Exception:
+        msg = get_exception_msg()
+        sys.stdout.write(msg)
```

### Comparing `recurtx-0.0.4/recurtx/search.py` & `recurtx-0.0.5/recurtx/search.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.4/recurtx/utils.py` & `recurtx-0.0.5/recurtx/utils.py`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.4/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.5/recurtx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.4/setup.py` & `recurtx-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "recurtx = recurtx.__main__:main",
     "xpandas = recurtx.__main__:xpandas",
     "xpolars = recurtx.__main__:xpolars",
     "xunder = recurtx.__main__:xunder",
     "xbatch = recurtx.__main__:xbatch",
     "xsearch = recurtx.__main__:xsearch",
     "xfind = recurtx.__main__:xfind",
+    "xll = recurtx.__main__:xll",
 ]
 
 
 with open("requirements.txt", encoding="utf-8") as f:
     requires = []
     for line in f:
         req = line.split("#", 1)[0].strip()
@@ -21,15 +22,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": console_scripts},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

