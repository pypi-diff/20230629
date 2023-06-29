# Comparing `tmp/nuclia-1.0.3.tar.gz` & `tmp/nuclia-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.0.3.tar", last modified: Tue Jun 20 21:17:32 2023, max compression
+gzip compressed data, was "nuclia-1.0.4.tar", last modified: Thu Jun 29 07:30:18 2023, max compression
```

## Comparing `nuclia-1.0.3.tar` & `nuclia-1.0.4.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.232388 nuclia-1.0.3/
--rw-r--r--   0 ramon      (501) staff       (20)       34 2023-06-20 21:17:31.000000 nuclia-1.0.3/.gitignore
--rw-r--r--   0 ramon      (501) staff       (20)       10 2023-06-20 21:17:31.000000 nuclia-1.0.3/.python-version
--rw-r--r--   0 ramon      (501) staff       (20)       95 2023-06-20 21:17:31.000000 nuclia-1.0.3/CHANGELOG.md
--rw-r--r--   0 ramon      (501) staff       (20)     1063 2023-06-20 21:17:31.000000 nuclia-1.0.3/LICENSE
--rw-r--r--   0 ramon      (501) staff       (20)       83 2023-06-20 21:17:31.000000 nuclia-1.0.3/MANIFEST.in
--rw-r--r--   0 ramon      (501) staff       (20)      236 2023-06-20 21:17:31.000000 nuclia-1.0.3/Makefile
--rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-20 21:17:32.232483 nuclia-1.0.3/PKG-INFO
--rw-r--r--   0 ramon      (501) staff       (20)      847 2023-06-20 21:17:31.000000 nuclia-1.0.3/README.md
--rw-r--r--   0 ramon      (501) staff       (20)        6 2023-06-20 21:17:31.000000 nuclia-1.0.3/VERSION
--rw-r--r--   0 ramon      (501) staff       (20)       24 2023-06-20 21:17:31.000000 nuclia-1.0.3/code-requirements.txt
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.225529 nuclia-1.0.3/docs/
--rw-r--r--   0 ramon      (501) staff       (20)      941 2023-06-20 21:17:31.000000 nuclia-1.0.3/docs/AUTH.md
--rw-r--r--   0 ramon      (501) staff       (20)     1580 2023-06-20 21:17:31.000000 nuclia-1.0.3/docs/CONVERSATION.md
--rw-r--r--   0 ramon      (501) staff       (20)      892 2023-06-20 21:17:31.000000 nuclia-1.0.3/docs/DEFAULT.md
--rw-r--r--   0 ramon      (501) staff       (20)      648 2023-06-20 21:17:31.000000 nuclia-1.0.3/docs/README.md
--rw-r--r--   0 ramon      (501) staff       (20)     1036 2023-06-20 21:17:31.000000 nuclia-1.0.3/docs/SEARCH.md
--rw-r--r--   0 ramon      (501) staff       (20)     1319 2023-06-20 21:17:31.000000 nuclia-1.0.3/docs/UPLOAD.md
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.226349 nuclia-1.0.3/nuclia/
--rw-r--r--   0 ramon      (501) staff       (20)      303 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/__init__.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.228137 nuclia-1.0.3/nuclia/cli/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/cli/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      660 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/cli/run.py
--rw-r--r--   0 ramon      (501) staff       (20)      526 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/cli/utils.py
--rw-r--r--   0 ramon      (501) staff       (20)     6222 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/config.py
--rw-r--r--   0 ramon      (501) staff       (20)      739 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/data.py
--rw-r--r--   0 ramon      (501) staff       (20)     2569 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/decorators.py
--rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/exceptions.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.228788 nuclia-1.0.3/nuclia/lib/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/lib/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      253 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/lib/conversations.py
--rw-r--r--   0 ramon      (501) staff       (20)     5996 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/lib/kb.py
--rw-r--r--   0 ramon      (501) staff       (20)      791 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/lib/nua.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.231210 nuclia-1.0.3/nuclia/sdk/
--rw-r--r--   0 ramon      (501) staff       (20)      343 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      229 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/accounts.py
--rw-r--r--   0 ramon      (501) staff       (20)     7762 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/auth.py
--rw-r--r--   0 ramon      (501) staff       (20)     1075 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/kb.py
--rw-r--r--   0 ramon      (501) staff       (20)     2251 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/kbs.py
--rw-r--r--   0 ramon      (501) staff       (20)      410 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/nua.py
--rw-r--r--   0 ramon      (501) staff       (20)     1092 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/nuas.py
--rw-r--r--   0 ramon      (501) staff       (20)      427 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/predict.py
--rw-r--r--   0 ramon      (501) staff       (20)      190 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/process.py
--rw-r--r--   0 ramon      (501) staff       (20)     1968 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/search.py
--rw-r--r--   0 ramon      (501) staff       (20)      188 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/train.py
--rw-r--r--   0 ramon      (501) staff       (20)     4493 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/upload.py
--rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/sdk/zones.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.232040 nuclia-1.0.3/nuclia/tests/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/tests/__init__.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.232217 nuclia-1.0.3/nuclia/tests/assets/
--rw-r--r--   0 ramon      (501) staff       (20)      761 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ramon      (501) staff       (20)       50 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/tests/conftest.py
--rw-r--r--   0 ramon      (501) staff       (20)     1200 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/tests/fixtures.py
--rw-r--r--   0 ramon      (501) staff       (20)      431 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/tests/test_auth.py
--rw-r--r--   0 ramon      (501) staff       (20)      659 2023-06-20 21:17:31.000000 nuclia-1.0.3/nuclia/tests/test_conversation.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 21:17:32.227664 nuclia-1.0.3/nuclia.egg-info/
--rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ramon      (501) staff       (20)     1144 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ramon      (501) staff       (20)       47 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ramon      (501) staff       (20)       53 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/requires.txt
--rw-r--r--   0 ramon      (501) staff       (20)        7 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-20 21:17:32.000000 nuclia-1.0.3/nuclia.egg-info/zip-safe
--rw-r--r--   0 ramon      (501) staff       (20)       52 2023-06-20 21:17:31.000000 nuclia-1.0.3/requirements.txt
--rw-r--r--   0 ramon      (501) staff       (20)      204 2023-06-20 21:17:32.232908 nuclia-1.0.3/setup.cfg
--rw-r--r--   0 ramon      (501) staff       (20)     1946 2023-06-20 21:17:31.000000 nuclia-1.0.3/setup.py
--rw-r--r--   0 ramon      (501) staff       (20)       32 2023-06-20 21:17:31.000000 nuclia-1.0.3/test-requirements.txt
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.041690 nuclia-1.0.4/
+-rw-r--r--   0 ramon      (501) staff       (20)       39 2023-06-29 07:30:17.000000 nuclia-1.0.4/.gitignore
+-rw-r--r--   0 ramon      (501) staff       (20)       10 2023-06-29 07:30:17.000000 nuclia-1.0.4/.python-version
+-rw-r--r--   0 ramon      (501) staff       (20)      271 2023-06-29 07:30:17.000000 nuclia-1.0.4/CHANGELOG.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1063 2023-06-29 07:30:17.000000 nuclia-1.0.4/LICENSE
+-rw-r--r--   0 ramon      (501) staff       (20)       83 2023-06-29 07:30:17.000000 nuclia-1.0.4/MANIFEST.in
+-rw-r--r--   0 ramon      (501) staff       (20)      236 2023-06-29 07:30:17.000000 nuclia-1.0.4/Makefile
+-rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-29 07:30:18.041735 nuclia-1.0.4/PKG-INFO
+-rw-r--r--   0 ramon      (501) staff       (20)      847 2023-06-29 07:30:17.000000 nuclia-1.0.4/README.md
+-rw-r--r--   0 ramon      (501) staff       (20)        6 2023-06-29 07:30:17.000000 nuclia-1.0.4/VERSION
+-rw-r--r--   0 ramon      (501) staff       (20)       24 2023-06-29 07:30:17.000000 nuclia-1.0.4/code-requirements.txt
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.037909 nuclia-1.0.4/docs/
+-rw-r--r--   0 ramon      (501) staff       (20)      941 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/AUTH.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1580 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/CONVERSATION.md
+-rw-r--r--   0 ramon      (501) staff       (20)      892 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/DEFAULT.md
+-rw-r--r--   0 ramon      (501) staff       (20)      648 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/README.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1057 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/SEARCH.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1993 2023-06-29 07:30:17.000000 nuclia-1.0.4/docs/UPLOAD.md
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.038378 nuclia-1.0.4/nuclia/
+-rw-r--r--   0 ramon      (501) staff       (20)      303 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/__init__.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.039316 nuclia-1.0.4/nuclia/cli/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/cli/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      660 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/cli/run.py
+-rw-r--r--   0 ramon      (501) staff       (20)      526 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/cli/utils.py
+-rw-r--r--   0 ramon      (501) staff       (20)     6257 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/config.py
+-rw-r--r--   0 ramon      (501) staff       (20)      739 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/data.py
+-rw-r--r--   0 ramon      (501) staff       (20)     2569 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/decorators.py
+-rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/exceptions.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.039768 nuclia-1.0.4/nuclia/lib/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      253 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/conversations.py
+-rw-r--r--   0 ramon      (501) staff       (20)     5996 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/kb.py
+-rw-r--r--   0 ramon      (501) staff       (20)      868 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/nua.py
+-rw-r--r--   0 ramon      (501) staff       (20)      123 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/lib/nua_responses.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.040965 nuclia-1.0.4/nuclia/sdk/
+-rw-r--r--   0 ramon      (501) staff       (20)      343 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      229 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/accounts.py
+-rw-r--r--   0 ramon      (501) staff       (20)     7800 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/auth.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1075 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/kb.py
+-rw-r--r--   0 ramon      (501) staff       (20)     2251 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/kbs.py
+-rw-r--r--   0 ramon      (501) staff       (20)      410 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/nua.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1092 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/nuas.py
+-rw-r--r--   0 ramon      (501) staff       (20)      499 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/predict.py
+-rw-r--r--   0 ramon      (501) staff       (20)      190 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/process.py
+-rw-r--r--   0 ramon      (501) staff       (20)     2245 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/search.py
+-rw-r--r--   0 ramon      (501) staff       (20)      188 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/train.py
+-rw-r--r--   0 ramon      (501) staff       (20)     5846 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/upload.py
+-rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/sdk/zones.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.041503 nuclia-1.0.4/nuclia/tests/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/__init__.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.041601 nuclia-1.0.4/nuclia/tests/assets/
+-rw-r--r--   0 ramon      (501) staff       (20)      761 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ramon      (501) staff       (20)       50 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/conftest.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1200 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/fixtures.py
+-rw-r--r--   0 ramon      (501) staff       (20)      492 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/test_auth.py
+-rw-r--r--   0 ramon      (501) staff       (20)      659 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ramon      (501) staff       (20)      247 2023-06-29 07:30:17.000000 nuclia-1.0.4/nuclia/tests/test_predict.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-29 07:30:18.039046 nuclia-1.0.4/nuclia.egg-info/
+-rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ramon      (501) staff       (20)     1201 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ramon      (501) staff       (20)       47 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ramon      (501) staff       (20)      133 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        7 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-29 07:30:18.000000 nuclia-1.0.4/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ramon      (501) staff       (20)      132 2023-06-29 07:30:17.000000 nuclia-1.0.4/requirements.txt
+-rw-r--r--   0 ramon      (501) staff       (20)      204 2023-06-29 07:30:18.041931 nuclia-1.0.4/setup.cfg
+-rw-r--r--   0 ramon      (501) staff       (20)     1946 2023-06-29 07:30:17.000000 nuclia-1.0.4/setup.py
+-rw-r--r--   0 ramon      (501) staff       (20)       32 2023-06-29 07:30:17.000000 nuclia-1.0.4/test-requirements.txt
```

### Comparing `nuclia-1.0.3/LICENSE` & `nuclia-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/PKG-INFO` & `nuclia-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.0.3/README.md` & `nuclia-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/docs/AUTH.md` & `nuclia-1.0.4/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/docs/CONVERSATION.md` & `nuclia-1.0.4/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/docs/DEFAULT.md` & `nuclia-1.0.4/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/docs/README.md` & `nuclia-1.0.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/docs/SEARCH.md` & `nuclia-1.0.4/docs/SEARCH.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Search
 
 ## Search experience
 
 Its the most basic search experience at Nuclia. You can search resources and paragraphs that match a query by a fulltext match, a fuzzy match or a semantic match. The results will be ordered by each search using BM25, fuzzy distance and semantic distance.
 
 ```bash
-nuclia search --query="My search"
+nuclia search search --query="My search"
 ```
 
 ```python
 from nuclia import sdk
 search = sdk.NucliaSearch()
 search.search(query="My search")
 ```
 
 ## Find experience
 
 You get the list of paragraphs matching semantically and by keywords ordered together with a generic reranking strategy.
 
 ```bash
-nuclia find --query="My search"
+nuclia search find --query="My search"
 ```
 
 ```python
 from nuclia import sdk
 search = sdk.NucliaSearch()
 search.find(query="My search")
 ```
 
 ## Ask experience
 
 Based on the find experience we use a generative AI to answer the question based on the context without hallucinations and with the find result and relations
 
 ```bash
-nuclia ask --query="My search"
+nuclia search ask --query="My search"
 ```
 
 ```python
 from nuclia import sdk
 search = sdk.NucliaSearch()
 search.ask(query="My search")
 ```
```

### Comparing `nuclia-1.0.3/docs/UPLOAD.md` & `nuclia-1.0.4/docs/UPLOAD.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # Upload use case
 
-All examples has assumed you [authenticated](AUTH.md) and defined a [default](DEFAULT.md) knowledgebox. In case you want to overwrite or define a one time knowledgebox you should add on any command/function the `url` and `api_key` parameter.
+All examples assume you [authenticated](AUTH.md) and defined a [default](DEFAULT.md) knowledgebox. In case you want to overwrite or define a one time knowledgebox you should add on any command/function the `url` and `api_key` parameter.
 
 ## Upload a file in a KnowledgeBox
 
-Pushing a file to a knowledgebox its easy as:
+Push a file to a knowledgebox:
 
 ```bash
 nuclia kb upload file --path=FILE_PATH
 ```
 
 ```python
 from nuclia import sdk
 upload = sdk.NucliaUpload()
 upload.file(FILE_PATH)
 ```
 
-
 ## Upload a file in an existing resource
 
-
 In case you want to upload a file inside a resource you can use:
 
 ```bash
 nuclia kb upload file --path=FILE_PATH  --rid=RESOURCE_ID --field=FIELD_ID
 ```
 
 In case that `FIELD_ID` is not defined filename will be used
@@ -42,14 +40,52 @@
 
 ```bash
 nuclia kb upload remote --origin=REMOTE_FILE_URL --rid=RESOURCE_ID --field=FIELD_ID
 ```
 
 In case that `FIELD_ID` is not defined filename will be used
 
+## Upload a text in a KnowledgeBox
+
+Push a text to a knowledgebox:
+
+```bash
+nuclia kb upload text --path=FILE_PATH
+```
+
+```python
+from nuclia import sdk
+upload = sdk.NucliaUpload()
+upload.text(FILE_PATH)
+```
+
+Pass the text from standard input:
+
+```bash
+echo "This is a message" | nuclia kb upload text --stdin
+```
+
+Set a specific format (default is `PLAIN`):
+
+```bash
+nuclia kb upload text --path=FILE_PATH --format=MARKDOWN
+```
+
+Define a slug for the resource:
+
+```bash
+nuclia kb upload text --path=FILE_PATH --slug=SLUG
+```
+
+Pass `origin` or `extra` metadata:
+
+```bash
+nuclia kb upload text --path=FILE_PATH --origin='{"url":"https://somwhere.com"}' --extra='{"metadata":{"whatever":42}}'
+```
+
 ## List resources on a kb
 
 ```bash
 nuclia kb list
 ```
 
 ## Delete a resource on a kb
```

### Comparing `nuclia-1.0.3/nuclia/cli/run.py` & `nuclia-1.0.4/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/cli/utils.py` & `nuclia-1.0.4/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/config.py` & `nuclia-1.0.4/nuclia/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 
     def __str__(self):
         return f"{self.id:36} -> {'(' + self.account + ')' if self.account else ''} {self.title}"
 
 
 class NuaKey(BaseModel):
     client_id: str
-    title: Optional[str]
+    account_type: Optional[str]
     region: str
     account: str
     token: str
 
     def __str__(self):
-        return f"{self.client_id} {self.account} {self.title:30}"
+        return f"{self.client_id} {self.account} {self.account_type:30}"
 
 
 class Zone(BaseModel):
     id: str
     title: str
     slug: Optional[str] = None
 
@@ -97,27 +97,27 @@
 
     def set_nua_token(
         self,
         client_id: str,
         account: str,
         region: str,
         token: str,
-        title: Optional[str] = None,
+        account_type: Optional[str] = None,
     ):
         if self.nuas_token is None:
             self.nuas_token = []
         try:
             nua_obj = next(filter(lambda x: x.client_id == client_id, self.nuas_token))
             self.nuas_token.remove(nua_obj)
         except StopIteration:
             pass
 
         self.nuas_token.append(
             NuaKey(
-                title=title,
+                account_type=account_type,
                 account=account,
                 region=region,
                 token=token,
                 client_id=client_id,
             )
         )
         self.save()
```

### Comparing `nuclia-1.0.3/nuclia/data.py` & `nuclia-1.0.4/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/decorators.py` & `nuclia-1.0.4/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/lib/kb.py` & `nuclia-1.0.4/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/lib/nua.py` & `nuclia-1.0.4/nuclia/lib/nua.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Optional
 
 import requests
 
 from nuclia import REGIONAL
 from nuclia.exceptions import NuaAPIException
+from nuclia.lib.nua_responses import Sentence
 
 SENTENCE_PREDICT = "/api/v1/predict/sentence"
 
 
 class NuaClient:
     def __init__(self, region: str, account: str, token: str):
         self.region = region
         self.account = account
         self.token = token
         self.url = REGIONAL.format(region=region).strip("/")
         self.headers = {"X-STF-NUAKEY": f"Bearer {token}"}
 
-    def sentence_predict(self, text: str, model: Optional[str] = None):
+    def sentence_predict(self, text: str, model: Optional[str] = None) -> Sentence:
         resp = requests.get(
-            f"{self.url}{SENTENCE_PREDICT}?query={text}&model={model}",
+            f"{self.url}{SENTENCE_PREDICT}?text={text}&model={model}",
             headers=self.headers,
         )
         if resp.status_code == 200:
-            return resp.json()
+            return Sentence.parse_obj(resp.json())
         else:
             raise NuaAPIException()
```

### Comparing `nuclia-1.0.3/nuclia/sdk/auth.py` & `nuclia-1.0.4/nuclia/sdk/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import json
 import readline  # noqa
 import webbrowser
 from typing import Dict, List, Optional, Tuple
 
 import requests
 
-from nuclia import BASE, get_global_url, get_regional_url
+from nuclia import BASE, get_global_url
 from nuclia.cli.utils import yes_no
 from nuclia.config import Account, Config, KnowledgeBox, Zone
 from nuclia.exceptions import NeedUserToken, UserTokenExpired
 
 USER = f"{BASE}/api/v1/user/welcome"
 MEMBER = f"{BASE}/api/v1/user"
 ACCOUNTS = f"{BASE}/api/v1/accounts"
 ZONES = f"{BASE}/api/v1/zones"
 LIST_KBS = BASE + "/api/v1/account/{account}/kbs"
-VERIFY_NUA = "/api/v1/nua/verify"
+VERIFY_NUA = "/api/authorizer/info"
 
 
 class NucliaAuth:
     _inner_config: Optional[Config] = None
 
     @property
     def _config(self) -> Config:
@@ -81,41 +81,41 @@
                 pass
 
             self._config.set_kb_token(url=url, token=token, title=title, kbid=kbid)
         else:
             print("Invalid service token")
 
     def nua(self, region: str, token: str) -> Optional[str]:
-        client_id, title, account = self.validate_nua(region, token)
+        client_id, account_type, account = self.validate_nua(token, region)
         if account is not None and client_id is not None:
             print("Validated")
             self._config.set_nua_token(
                 client_id=client_id,
-                title=title,
+                account_type=account_type,
                 account=account,
                 region=region,
                 token=token,
             )
             return client_id
         else:
             print("Invalid service token")
             return None
 
     def validate_nua(
-        self, region: str, token: str
+        self, token: str, region: Optional[str] = None
     ) -> Tuple[Optional[str], Optional[str], Optional[str]]:
         # Validate the code is ok
-        url = get_regional_url(region, VERIFY_NUA)
+        url = get_global_url(VERIFY_NUA)
         resp = requests.get(
             url,
-            headers={"X-STF-NUA": f"Bearer {token}"},
+            headers={"x-nuclia-nuakey": f"Bearer {token}"},
         )
         if resp.status_code == 200:
-            data = resp.json()
-            return data.get("client_id"), data.get("title"), data.get("account")
+            data = resp.json().get("user")
+            return data.get("user_id"), data.get("account_type"), data.get("account_id")
         else:
             return None, None, None
 
     def validate_kb(self, url: str, token: str) -> Tuple[Optional[str], Optional[str]]:
         # Validate the code is ok
         resp = requests.get(
             url,
```

### Comparing `nuclia-1.0.3/nuclia/sdk/kb.py` & `nuclia-1.0.4/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/sdk/kbs.py` & `nuclia-1.0.4/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/sdk/nuas.py` & `nuclia-1.0.4/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/sdk/search.py` & `nuclia-1.0.4/nuclia/sdk/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional, Union
 
 from nucliadb_models.search import (
     ChatRequest,
     FindRequest,
     KnowledgeboxFindResults,
     Relations,
+    SearchRequest,
 )
 
 from nuclia.data import get_auth
 from nuclia.decorators import kb
 from nuclia.lib.kb import NucliaDBClient
 from nuclia.sdk.auth import NucliaAuth
 
@@ -29,14 +30,23 @@
 class NucliaSearch:
     @property
     def _auth(self) -> NucliaAuth:
         auth = get_auth()
         return auth
 
     @kb
+    def search(self, *, ndb: NucliaDBClient, query: Union[str, SearchRequest]):
+        if isinstance(query, str):
+            req = SearchRequest(query=query)
+        else:
+            req = query
+
+        return ndb.ndb.search(req, kbid=ndb.kbid)
+
+    @kb
     def find(self, *, ndb: NucliaDBClient, query: Union[str, FindRequest]):
         if isinstance(query, str):
             req = FindRequest(query=query)
         else:
             req = query
 
         return ndb.ndb.find(req, kbid=ndb.kbid)
```

### Comparing `nuclia-1.0.3/nuclia/sdk/upload.py` & `nuclia-1.0.4/nuclia/sdk/upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
 import mimetypes
 import os
+import sys
 from datetime import datetime
+from pathlib import Path
 from typing import Optional
 from uuid import uuid4
 
 import requests
+from nucliadb_models.metadata import Extra, Origin
+from nucliadb_models.text import TextFormat
 from tqdm import tqdm
 
 from nuclia.data import get_auth
 from nuclia.decorators import kb
 from nuclia.lib.conversations import Conversations
 from nuclia.lib.kb import NucliaDBClient
 from nuclia.sdk.auth import NucliaAuth
@@ -96,14 +100,55 @@
                             for message in conversation.messages
                         ]
                     }
                 },
             )
 
     @kb
+    def text(
+        self,
+        *,
+        ndb: NucliaDBClient,
+        format: TextFormat = TextFormat.PLAIN,
+        path: Optional[str] = None,
+        stdin: Optional[bool] = False,
+        slug: Optional[str] = None,
+        origin: Optional[Origin] = None,
+        extra: Optional[Extra] = None,
+    ):
+        """Option to upload a text from filesystem to a Nuclia KnowledgeBox"""
+        if path is None and not stdin:
+            raise ValueError("Either path or stdin must be provided")
+        if path:
+            text = Path(path).resolve().open().read()
+        else:
+            text = sys.stdin.read()
+        rid = slug if slug is not None else uuid4().hex
+        icon = "text/plain"
+        if format == "HTML":
+            icon = "text/html"
+        elif format == "MARKDOWN":
+            icon = "text/markdown"
+        elif format == "RST":
+            icon = "text/x-rst"
+        ndb.ndb.create_resource(
+            kbid=ndb.kbid,
+            slug=rid,
+            icon=icon,
+            origin=origin,
+            extra=extra,
+            texts={
+                rid: {
+                    "body": text,
+                    "format": format,
+                }
+            },
+        )
+
+    @kb
     def remote(
         self,
         *,
         ndb: NucliaDBClient,
         origin: str,
         rid: Optional[str] = None,
         field: Optional[str] = "file",
```

### Comparing `nuclia-1.0.3/nuclia/tests/assets/conversation.json` & `nuclia-1.0.4/nuclia/tests/assets/conversation.json`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/tests/fixtures.py` & `nuclia-1.0.4/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia/tests/test_conversation.py` & `nuclia-1.0.4/nuclia/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.3/nuclia.egg-info/PKG-INFO` & `nuclia-1.0.4/nuclia.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.0.3/nuclia.egg-info/SOURCES.txt` & `nuclia-1.0.4/nuclia.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 nuclia/cli/__init__.py
 nuclia/cli/run.py
 nuclia/cli/utils.py
 nuclia/lib/__init__.py
 nuclia/lib/conversations.py
 nuclia/lib/kb.py
 nuclia/lib/nua.py
+nuclia/lib/nua_responses.py
 nuclia/sdk/__init__.py
 nuclia/sdk/accounts.py
 nuclia/sdk/auth.py
 nuclia/sdk/kb.py
 nuclia/sdk/kbs.py
 nuclia/sdk/nua.py
 nuclia/sdk/nuas.py
@@ -50,8 +51,9 @@
 nuclia/sdk/upload.py
 nuclia/sdk/zones.py
 nuclia/tests/__init__.py
 nuclia/tests/conftest.py
 nuclia/tests/fixtures.py
 nuclia/tests/test_auth.py
 nuclia/tests/test_conversation.py
+nuclia/tests/test_predict.py
 nuclia/tests/assets/conversation.json
```

### Comparing `nuclia-1.0.3/setup.py` & `nuclia-1.0.4/setup.py`

 * *Files identical despite different names*

