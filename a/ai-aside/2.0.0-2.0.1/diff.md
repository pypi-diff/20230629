# Comparing `tmp/ai-aside-2.0.0.tar.gz` & `tmp/ai-aside-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-aside-2.0.0.tar", last modified: Wed Jun 28 13:34:29 2023, max compression
+gzip compressed data, was "ai-aside-2.0.1.tar", last modified: Thu Jun 29 16:16:40 2023, max compression
```

## Comparing `ai-aside-2.0.0.tar` & `ai-aside-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      953 2023-06-28 13:34:25.000000 ai-aside-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-28 13:34:25.000000 ai-aside-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-28 13:34:25.000000 ai-aside-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-06-28 13:34:29.925830 ai-aside-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-06-28 13:34:25.000000 ai-aside-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/ai_aside/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/ai_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/ai_aside/summaryhook_aside/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     7412 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/ai_aside/summaryhook_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-06-28 13:34:25.000000 ai-aside-2.0.0/ai_aside/summaryhook_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/ai_aside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-28 13:34:29.000000 ai-aside-2.0.0/ai_aside.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-06-28 13:34:25.000000 ai-aside-2.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-28 13:34:25.000000 ai-aside-2.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-28 13:34:29.925830 ai-aside-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5399 2023-06-28 13:34:25.000000 ai-aside-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 13:34:29.925830 ai-aside-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-28 13:34:25.000000 ai-aside-2.0.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-29 16:16:35.000000 ai-aside-2.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-29 16:16:35.000000 ai-aside-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-29 16:16:35.000000 ai-aside-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7691 2023-06-29 16:16:40.246649 ai-aside-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-06-29 16:16:35.000000 ai-aside-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/summaryhook_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-06-29 16:16:35.000000 ai-aside-2.0.1/ai_aside/summaryhook_aside/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/ai_aside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7691 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 16:16:40.000000 ai-aside-2.0.1/ai_aside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-06-29 16:16:35.000000 ai-aside-2.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-29 16:16:35.000000 ai-aside-2.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-29 16:16:40.246649 ai-aside-2.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5399 2023-06-29 16:16:35.000000 ai-aside-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 16:16:40.242649 ai-aside-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-29 16:16:35.000000 ai-aside-2.0.1/tests/test_placeholder.py
```

### Comparing `ai-aside-2.0.0/CHANGELOG.rst` & `ai-aside-2.0.1/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+2.0.1 – 2023-06-29
+**********************************************
+
+Fix
+=====
+
+* Fix transcript format request and conversion
+
+
 2.0.0 – 2023-06-28
 **********************************************
 
 Added
 =====
 
 * Adds a handler endpoint to provide summarizable content
```

### Comparing `ai-aside-2.0.0/LICENSE.txt` & `ai-aside-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/PKG-INFO` & `ai-aside-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 2.0.0
+Version: 2.0.1
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -196,14 +196,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+2.0.1 – 2023-06-29
+**********************************************
+
+Fix
+=====
+
+* Fix transcript format request and conversion
+
+
 2.0.0 – 2023-06-28
 **********************************************
 
 Added
 =====
 
 * Adds a handler endpoint to provide summarizable content
```

### Comparing `ai-aside-2.0.0/README.rst` & `ai-aside-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/ai_aside/apps.py` & `ai-aside-2.0.1/ai_aside/apps.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/ai_aside/summaryhook_aside/apps.py` & `ai-aside-2.0.1/ai_aside/summaryhook_aside/apps.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/ai_aside/summaryhook_aside/block.py` & `ai-aside-2.0.1/ai_aside/summaryhook_aside/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,34 +49,31 @@
 def _extract_child_contents(child, category):
     """
     Process the child contents based on its category.
     """
 
     try:
         # pylint: disable=import-outside-toplevel
-        from xmodule.video_block.transcripts_utils import Transcript, get_transcript
+        from xmodule.video_block.transcripts_utils import get_transcript
     except ImportError:
         return None
 
     if category == 'html':
         try:
             content_html = child.get_html()
             text = html_to_text(content_html)
 
             return text
         except AttributeError:
             return None
 
     if category == 'video':
         try:
-            transcript = get_transcript(child)[0]
-            transcript_format = child.transcript_download_format
-            text = Transcript.convert(transcript, transcript_format, 'txt')
-
-            return text
+            transcript, _, _ = get_transcript(child, output_format='txt')
+            return transcript
         except AttributeError:
             return None
 
     return None
 
 
 def _parse_children_contents(block):
```

### Comparing `ai-aside-2.0.0/ai_aside/summaryhook_aside/settings/devstack.py` & `ai-aside-2.0.1/ai_aside/summaryhook_aside/settings/devstack.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/ai_aside/summaryhook_aside/text_utils.py` & `ai-aside-2.0.1/ai_aside/summaryhook_aside/text_utils.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/ai_aside/summaryhook_aside/waffle.py` & `ai-aside-2.0.1/ai_aside/summaryhook_aside/waffle.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/ai_aside.egg-info/PKG-INFO` & `ai-aside-2.0.1/ai_aside.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 2.0.0
+Version: 2.0.1
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -196,14 +196,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+2.0.1 – 2023-06-29
+**********************************************
+
+Fix
+=====
+
+* Fix transcript format request and conversion
+
+
 2.0.0 – 2023-06-28
 **********************************************
 
 Added
 =====
 
 * Adds a handler endpoint to provide summarizable content
```

### Comparing `ai-aside-2.0.0/ai_aside.egg-info/SOURCES.txt` & `ai-aside-2.0.1/ai_aside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/requirements/constraints.txt` & `ai-aside-2.0.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.0/setup.py` & `ai-aside-2.0.1/setup.py`

 * *Files identical despite different names*

