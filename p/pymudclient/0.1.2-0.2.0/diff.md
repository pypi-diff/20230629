# Comparing `tmp/pymudclient-0.1.2.tar.gz` & `tmp/pymudclient-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymudclient-0.1.2.tar", last modified: Thu Jun 29 09:30:36 2023, max compression
+gzip compressed data, was "pymudclient-0.2.0.tar", last modified: Thu Jun 29 13:11:45 2023, max compression
```

## Comparing `pymudclient-0.1.2.tar` & `pymudclient-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.555102 pymudclient-0.1.2/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.1.2/LICENSE
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6688 2023-06-29 09:30:36.554631 pymudclient-0.1.2/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)     4776 2023-06-29 09:30:04.000000 pymudclient-0.1.2/README.md
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.545015 pymudclient-0.1.2/pymudclient/
--rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/display.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6030 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/input_cmd.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/kbhit.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.1.2/pymudclient/mud.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1906 2023-06-29 08:18:34.000000 pymudclient-0.1.2/pymudclient/recv.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/shared_data.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.553555 pymudclient-0.1.2/pymudclient/utils/
--rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/codec.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/colors.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/print.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pymudclient/utils/telnet.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:30:36.547438 pymudclient-0.1.2/pymudclient.egg-info/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6688 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/SOURCES.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/dependency_links.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/requires.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 09:30:36.000000 pymudclient-0.1.2/pymudclient.egg-info/top_level.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.1.2/pyproject.toml
--rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 09:30:36.555248 pymudclient-0.1.2/setup.cfg
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 09:30:29.000000 pymudclient-0.1.2/setup.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.281327 pymudclient-0.2.0/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.2.0/LICENSE
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     5580 2023-06-29 13:11:45.281006 pymudclient-0.2.0/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     4909 2023-06-29 13:06:30.000000 pymudclient-0.2.0/README.md
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.277569 pymudclient-0.2.0/pymudclient/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.2.0/pymudclient/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/display.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6122 2023-06-29 13:09:24.000000 pymudclient-0.2.0/pymudclient/input_cmd.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/kbhit.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.2.0/pymudclient/mud.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1888 2023-06-29 13:07:44.000000 pymudclient-0.2.0/pymudclient/recv.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/shared_data.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.280531 pymudclient-0.2.0/pymudclient/utils/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/codec.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/colors.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/print.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/telnet.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.279111 pymudclient-0.2.0/pymudclient.egg-info/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     5580 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/requires.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/top_level.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pyproject.toml
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 13:11:45.281444 pymudclient-0.2.0/setup.cfg
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 13:11:16.000000 pymudclient-0.2.0/setup.py
```

### Comparing `pymudclient-0.1.2/LICENSE` & `pymudclient-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/README.md` & `pymudclient-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     - [Trigger](#trigger)
       - [Trigger class 參數](#trigger-class-參數)
       - [使用範例](#使用範例-2)
     - [Timer](#timer)
       - [Timer class 參數](#timer-class-參數)
       - [使用範例](#使用範例-3)
   - [已知問題](#已知問題)
+  - [License](#license)
 
 ## 這是什麼？
 
 - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
 - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
 
 ## 已測試過環境
@@ -147,8 +148,12 @@
 ]
 ```
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
-- 部分中文字顯示會有不正確位置的換行。
+- ctrl-z 把 process 移到背景後，再 fg 切回前景，輸入會變得異常。
+
+## License
+
+- [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.1.2/pymudclient/input_cmd.py` & `pymudclient-0.2.0/pymudclient/input_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,14 @@
         g_input['input'] = (
             g_input['input'][:g_input['input_index'] - 1] + g_input['input'][g_input['input_index']:]
         )
         g_input['input_index'] -= 1
 
 
 def _alias_pattern_process(start_text, pattern, text):
-    text = text.replace(f'{start_text}', '', 1)
     split_text = text.split()
     params = {}
 
     # %0
     if '%0' in pattern:
         pattern = pattern.replace('%0', '{%0}')
         params['%0'] = text
@@ -149,15 +148,19 @@
         i += 1
 
     return pattern.format(**params)
 
 
 def _alias_function(text):
     for alias in alias_list:
-        if not text.startswith(alias.start_text):
+        if text == alias.start_text:
+            text = ''
+        elif text.startswith(alias.start_text + ' '):
+            text = text.replace(alias.start_text + ' ', '', 1)
+        else:
             continue
 
         if alias.pattern:
             return _alias_pattern_process(alias.start_text, alias.pattern, text)
         if alias.func:
             return alias.func(text)
```

### Comparing `pymudclient-0.1.2/pymudclient/kbhit.py` & `pymudclient-0.2.0/pymudclient/kbhit.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/pymudclient/mud.py` & `pymudclient-0.2.0/pymudclient/mud.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/pymudclient/recv.py` & `pymudclient-0.2.0/pymudclient/recv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import time
 
 from .display import show_input
 from .shared_data import (
     g_is_reconnect,
     g_is_running,
     g_tn,
 )
@@ -48,22 +49,23 @@
 def thread_job_recv(trigger_list):
     while g_is_running.get() and not g_is_reconnect.get():
         try:
             data = g_tn.get().read_very_eager()
             if not data:
                 continue
 
+            last_time = time.time()
+            while time.time() - last_time < 0.1:
+                data += g_tn.get().read_very_eager()
+                time.sleep(0.01)
+
             data = remove_strange_color_code(data)
             content_list = dec(data).split('\r\n')
 
             for content in content_list:
-                # TODO: 用 regex 取代這些無用的行
-                if content == '' or content == '\x1B[2;37;0m' or content == '\x1B[2;37;0m> ' or content == '> ':
-                    continue
-
                 content = dec(enc(content))
                 replace_line_print(content)
 
                 _triggers(trigger_list, content)
 
             show_input()
```

### Comparing `pymudclient-0.1.2/pymudclient/shared_data.py` & `pymudclient-0.2.0/pymudclient/shared_data.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/pymudclient/utils/colors.py` & `pymudclient-0.2.0/pymudclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/pymudclient/utils/print.py` & `pymudclient-0.2.0/pymudclient/utils/print.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/pymudclient.egg-info/SOURCES.txt` & `pymudclient-0.2.0/pymudclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/pyproject.toml` & `pymudclient-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.2/setup.py` & `pymudclient-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = 'pymudclient'
 AUTHOR = 'griiid'
 AUTHOR_EMAIL = 'gridwing@gmail.com'
 URL = 'https://github.com/griiid/PyMudClient'
 DOWNLOAD_URL = 'https://pypi.org/project/pymudclient/'
 
 LICENSE = 'MIT'
-VERSION = '0.1.2'
+VERSION = '0.2.0'
 DESCRIPTION = 'A MUD client core written in Python'
 LONG_DESCRIPTION = (HERE  / 'README.md').read_text(encoding='utf8')
 LONG_DESC_TYPE = 'text/markdown'
 
 requirements = (HERE / 'requirements.txt').read_text(encoding='utf8')
 INSTALL_REQUIRES = [s.strip() for s in requirements.split('\n')]
```

