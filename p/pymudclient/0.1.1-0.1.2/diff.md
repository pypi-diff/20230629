# Comparing `tmp/pymudclient-0.1.1.tar.gz` & `tmp/pymudclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymudclient-0.1.1.tar", last modified: Thu Jun 29 09:18:43 2023, max compression
+gzip compressed data, was "pymudclient-0.1.2.tar", last modified: Thu Jun 29 09:30:36 2023, max compression
```

## Comparing `pymudclient-0.1.1.tar` & `pymudclient-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.360463 pymudclient-0.1.1/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.1.1/LICENSE
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6700 2023-06-29 09:18:43.360054 pymudclient-0.1.1/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)     4788 2023-06-29 09:16:59.000000 pymudclient-0.1.1/README.md
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.354297 pymudclient-0.1.1/pymudclient/
--rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/display.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6030 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/input_cmd.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/kbhit.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.1.1/pymudclient/mud.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1906 2023-06-29 08:18:34.000000 pymudclient-0.1.1/pymudclient/recv.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/shared_data.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.359299 pymudclient-0.1.1/pymudclient/utils/
--rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/codec.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/colors.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/print.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/telnet.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.356949 pymudclient-0.1.1/pymudclient.egg-info/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6700 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/SOURCES.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/dependency_links.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/requires.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/top_level.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pyproject.toml
--rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 09:18:43.360600 pymudclient-0.1.1/setup.cfg
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 08:59:30.000000 pymudclient-0.1.1/setup.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.555102 pymudclient-0.1.2/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.1.2/LICENSE
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6688 2023-06-29 09:30:36.554631 pymudclient-0.1.2/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     4776 2023-06-29 09:30:04.000000 pymudclient-0.1.2/README.md
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.545015 pymudclient-0.1.2/pymudclient/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/display.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6030 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/input_cmd.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/kbhit.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.1.2/pymudclient/mud.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1906 2023-06-29 08:18:34.000000 pymudclient-0.1.2/pymudclient/recv.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/shared_data.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.553555 pymudclient-0.1.2/pymudclient/utils/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/codec.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/colors.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/print.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/telnet.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.547438 pymudclient-0.1.2/pymudclient.egg-info/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6688 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/requires.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/top_level.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pyproject.toml
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 09:30:36.555248 pymudclient-0.1.2/setup.cfg
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 09:30:29.000000 pymudclient-0.1.2/setup.py
```

### Comparing `pymudclient-0.1.1/LICENSE` & `pymudclient-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/PKG-INFO` & `pymudclient-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/pymudclient/
 Description: # pymudclient: 用 Python 開發的 MUD Client 核心
@@ -12,15 +12,15 @@
         - [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
           - [這是什麼？](#這是什麼)
           - [已測試過環境](#已測試過環境)
           - [功能說明](#功能說明)
           - [安裝](#安裝)
           - [使用範例](#使用範例)
           - [功能說明](#功能說明-1)
-            - [mud_run](#mud_run)
+            - [run](#run)
             - [Alias](#alias)
               - [Alias class 參數](#alias-class-參數)
               - [使用範例](#使用範例-1)
             - [Trigger](#trigger)
               - [Trigger class 參數](#trigger-class-參數)
               - [使用範例](#使用範例-2)
             - [Timer](#timer)
@@ -70,15 +70,15 @@
             trigger_list=TRIGGER_LIST,
             timer_list=TIMER_LIST,
         )
         ```
         
         ## 功能說明
         
-        ### mud_run
+        ### run
         
         ```py
         run(host, port, alias_list=None, trigger_list=None, timer_list=None)
         ```
         
         - host `string`: 連線的主機網址或 IP。
         - port `number`: 連線的主機 port。
```

### Comparing `pymudclient-0.1.1/README.md` & `pymudclient-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 - [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
   - [功能說明](#功能說明)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
   - [功能說明](#功能說明-1)
-    - [mud_run](#mud_run)
+    - [run](#run)
     - [Alias](#alias)
       - [Alias class 參數](#alias-class-參數)
       - [使用範例](#使用範例-1)
     - [Trigger](#trigger)
       - [Trigger class 參數](#trigger-class-參數)
       - [使用範例](#使用範例-2)
     - [Timer](#timer)
@@ -61,15 +61,15 @@
     trigger_list=TRIGGER_LIST,
     timer_list=TIMER_LIST,
 )
 ```
 
 ## 功能說明
 
-### mud_run
+### run
 
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
 ```
 
 - host `string`: 連線的主機網址或 IP。
 - port `number`: 連線的主機 port。
```

### Comparing `pymudclient-0.1.1/pymudclient/input_cmd.py` & `pymudclient-0.1.2/pymudclient/input_cmd.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient/kbhit.py` & `pymudclient-0.1.2/pymudclient/kbhit.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient/mud.py` & `pymudclient-0.1.2/pymudclient/mud.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient/recv.py` & `pymudclient-0.1.2/pymudclient/recv.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient/shared_data.py` & `pymudclient-0.1.2/pymudclient/shared_data.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient/utils/colors.py` & `pymudclient-0.1.2/pymudclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient/utils/print.py` & `pymudclient-0.1.2/pymudclient/utils/print.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pymudclient.egg-info/PKG-INFO` & `pymudclient-0.1.2/pymudclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/pymudclient/
 Description: # pymudclient: 用 Python 開發的 MUD Client 核心
@@ -12,15 +12,15 @@
         - [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
           - [這是什麼？](#這是什麼)
           - [已測試過環境](#已測試過環境)
           - [功能說明](#功能說明)
           - [安裝](#安裝)
           - [使用範例](#使用範例)
           - [功能說明](#功能說明-1)
-            - [mud_run](#mud_run)
+            - [run](#run)
             - [Alias](#alias)
               - [Alias class 參數](#alias-class-參數)
               - [使用範例](#使用範例-1)
             - [Trigger](#trigger)
               - [Trigger class 參數](#trigger-class-參數)
               - [使用範例](#使用範例-2)
             - [Timer](#timer)
@@ -70,15 +70,15 @@
             trigger_list=TRIGGER_LIST,
             timer_list=TIMER_LIST,
         )
         ```
         
         ## 功能說明
         
-        ### mud_run
+        ### run
         
         ```py
         run(host, port, alias_list=None, trigger_list=None, timer_list=None)
         ```
         
         - host `string`: 連線的主機網址或 IP。
         - port `number`: 連線的主機 port。
```

### Comparing `pymudclient-0.1.1/pymudclient.egg-info/SOURCES.txt` & `pymudclient-0.1.2/pymudclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/pyproject.toml` & `pymudclient-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.1/setup.py` & `pymudclient-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = 'pymudclient'
 AUTHOR = 'griiid'
 AUTHOR_EMAIL = 'gridwing@gmail.com'
 URL = 'https://github.com/griiid/PyMudClient'
 DOWNLOAD_URL = 'https://pypi.org/project/pymudclient/'
 
 LICENSE = 'MIT'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A MUD client core written in Python'
 LONG_DESCRIPTION = (HERE  / 'README.md').read_text(encoding='utf8')
 LONG_DESC_TYPE = 'text/markdown'
 
 requirements = (HERE / 'requirements.txt').read_text(encoding='utf8')
 INSTALL_REQUIRES = [s.strip() for s in requirements.split('\n')]
```

