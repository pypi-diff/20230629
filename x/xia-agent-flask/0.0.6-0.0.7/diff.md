# Comparing `tmp/xia_agent_flask-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent_flask-0.0.7-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2741 bytes, number of entries: 7
--rw-r--r--  2.0 unx      251 b- defN 23-Jun-29 20:33 xia_agent_flask/__init__.py
--rw-r--r--  2.0 unx     1888 b- defN 23-Jun-29 20:32 xia_agent_flask/api.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:34 xia_agent_flask-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      755 b- defN 23-Jun-29 20:34 xia_agent_flask-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:34 xia_agent_flask-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:34 xia_agent_flask-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      590 b- defN 23-Jun-29 20:34 xia_agent_flask-0.0.6.dist-info/RECORD
-7 files, 3750 bytes uncompressed, 1683 bytes compressed:  55.1%
+Zip file size: 2752 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      251 b- defN 23-Jun-29 20:36 xia_agent_flask/__init__.py
+-rw-r--r--  2.0 unx     1888 b- defN 23-Jun-29 20:33 xia_agent_flask/api.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:36 xia_agent_flask-0.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      755 b- defN 23-Jun-29 20:36 xia_agent_flask-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:36 xia_agent_flask-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:36 xia_agent_flask-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      591 b- defN 23-Jun-29 20:36 xia_agent_flask-0.0.7.dist-info/RECORD
+7 files, 3760 bytes uncompressed, 1694 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent_flask/__init__.py
 Comment: 
 
 Filename: xia_agent_flask/api.py
 Comment: 
 
-Filename: xia_agent_flask-0.0.6.dist-info/LICENSE.txt
+Filename: xia_agent_flask-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent_flask-0.0.6.dist-info/METADATA
+Filename: xia_agent_flask-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent_flask-0.0.6.dist-info/WHEEL
+Filename: xia_agent_flask-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent_flask-0.0.6.dist-info/top_level.txt
+Filename: xia_agent_flask-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent_flask-0.0.6.dist-info/RECORD
+Filename: xia_agent_flask-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent_flask/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
    "AgentFunctionApi",
    "FlaskRequestParser", "GcpLogParser", "PubsubLogParser"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

## Comparing `xia_agent_flask-0.0.6.dist-info/METADATA` & `xia_agent_flask-0.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-agent-flask
-Version: 0.0.6
+Version: 0.0.7
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-agent-flask/0.0.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-agent-flask/0.0.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

