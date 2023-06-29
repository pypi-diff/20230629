# Comparing `tmp/fsrs4anki_optimizer-3.25.6.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.6.tar", last modified: Mon Jun 26 09:54:05 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.7.tar", last modified: Thu Jun 29 08:20:35 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.6.tar` & `fsrs4anki_optimizer-3.25.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44569 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:20:35.573447 fsrs4anki_optimizer-3.25.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 08:20:35.573447 fsrs4anki_optimizer-3.25.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:20:35.573447 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 08:20:22.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-29 08:20:22.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44686 2023-06-29 08:20:22.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:20:35.573447 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-29 08:20:35.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 08:20:35.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:20:35.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 08:20:35.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 08:20:35.000000 fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 08:20:22.000000 fsrs4anki_optimizer-3.25.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:20:35.573447 fsrs4anki_optimizer-3.25.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 08:20:22.000000 fsrs4anki_optimizer-3.25.7/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.7/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,23 @@
         elif os.path.isfile("collection.anki21"):
             con = sqlite3.connect("collection.anki21")
         elif os.path.isfile("collection.anki2"):
             con = sqlite3.connect("collection.anki2")
         else:
             raise Exception("Collection not exist!")
         cur = con.cursor()
-        res = cur.execute("SELECT * FROM revlog")
+        res = cur.execute("""
+        SELECT *
+        FROM revlog
+        WHERE cid IN (
+            SELECT id
+            FROM cards
+        )
+        """
+        )
         revlog = res.fetchall()
         if len(revlog) == 0:
             raise Exception("No review log found!")
         df = pd.DataFrame(revlog)
         df.columns = ['id', 'cid', 'usn', 'r', 'ivl', 'last_lvl', 'factor', 'time', 'type']
         df = df[(df['cid'] <= time.time() * 1000) &
                 (df['id'] <= time.time() * 1000) &
```

