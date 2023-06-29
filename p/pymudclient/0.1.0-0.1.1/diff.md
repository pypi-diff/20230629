# Comparing `tmp/pymudclient-0.1.0.tar.gz` & `tmp/pymudclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymudclient-0.1.0.tar", last modified: Thu Jun 29 08:01:58 2023, max compression
+gzip compressed data, was "pymudclient-0.1.1.tar", last modified: Thu Jun 29 09:18:43 2023, max compression
```

## Comparing `pymudclient-0.1.0.tar` & `pymudclient-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 08:01:58.868203 pymudclient-0.1.0/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.1.0/LICENSE
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6212 2023-06-29 08:01:58.867933 pymudclient-0.1.0/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)     4428 2023-06-29 07:55:53.000000 pymudclient-0.1.0/README.md
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 08:01:58.864075 pymudclient-0.1.0/pymudclient/
--rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/display.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6030 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/input_cmd.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/kbhit.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/mud.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1906 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/recv.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/shared_data.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 08:01:58.867394 pymudclient-0.1.0/pymudclient/utils/
--rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/utils/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/utils/codec.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/utils/colors.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/utils/print.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pymudclient/utils/telnet.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 08:01:58.865787 pymudclient-0.1.0/pymudclient.egg-info/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6212 2023-06-29 08:01:58.000000 pymudclient-0.1.0/pymudclient.egg-info/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 08:01:58.000000 pymudclient-0.1.0/pymudclient.egg-info/SOURCES.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 08:01:58.000000 pymudclient-0.1.0/pymudclient.egg-info/dependency_links.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 08:01:58.000000 pymudclient-0.1.0/pymudclient.egg-info/requires.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 08:01:58.000000 pymudclient-0.1.0/pymudclient.egg-info/top_level.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.1.0/pyproject.toml
--rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 08:01:58.868293 pymudclient-0.1.0/setup.cfg
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 07:55:53.000000 pymudclient-0.1.0/setup.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.360463 pymudclient-0.1.1/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.1.1/LICENSE
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6700 2023-06-29 09:18:43.360054 pymudclient-0.1.1/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     4788 2023-06-29 09:16:59.000000 pymudclient-0.1.1/README.md
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.354297 pymudclient-0.1.1/pymudclient/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/display.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6030 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/input_cmd.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/kbhit.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.1.1/pymudclient/mud.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1906 2023-06-29 08:18:34.000000 pymudclient-0.1.1/pymudclient/recv.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/shared_data.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.359299 pymudclient-0.1.1/pymudclient/utils/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/codec.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/colors.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/print.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pymudclient/utils/telnet.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 09:18:43.356949 pymudclient-0.1.1/pymudclient.egg-info/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6700 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/requires.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 09:18:43.000000 pymudclient-0.1.1/pymudclient.egg-info/top_level.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.1.1/pyproject.toml
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 09:18:43.360600 pymudclient-0.1.1/setup.cfg
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 08:59:30.000000 pymudclient-0.1.1/setup.py
```

### Comparing `pymudclient-0.1.0/LICENSE` & `pymudclient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/PKG-INFO` & `pymudclient-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/pymudclient/
 Description: # pymudclient: 用 Python 開發的 MUD Client 核心
         
         - [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
           - [這是什麼？](#這是什麼)
           - [已測試過環境](#已測試過環境)
           - [功能說明](#功能說明)
+          - [安裝](#安裝)
           - [使用範例](#使用範例)
           - [功能說明](#功能說明-1)
             - [mud_run](#mud_run)
             - [Alias](#alias)
               - [Alias class 參數](#alias-class-參數)
               - [使用範例](#使用範例-1)
             - [Trigger](#trigger)
               - [Trigger class 參數](#trigger-class-參數)
               - [使用範例](#使用範例-2)
             - [Timer](#timer)
               - [Timer class 參數](#timer-class-參數)
               - [使用範例](#使用範例-3)
+          - [已知問題](#已知問題)
         
         ## 這是什麼？
         
         - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
         - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
         
         ## 已測試過環境
@@ -37,21 +39,27 @@
         - GNU/Linux 5.15.0-1032-raspi aarch64
         
         ## 功能說明
         
         - 連線：根據輸入的 host 跟 port 進行連線。
         - 斷線重連：發生異常、server 重新啟動導致的斷線，會等待 3 秒後重新連線。
         - 顯示：顯示 server 回傳的內容。
+          - 有處理 big5 中文顯示的問題。
+          - 只針對萬王之王 (kk.muds.idv.tw:4000) 進行測試過。
         - 輸入介面：在最後一行顯示輸入的文字；送出的文字還沒有改動時按下 Enter 會再送一次。
         
+        ## 安裝
+        
+        `pip install pymudclient`
+        
         ## 使用範例
         
         ```py
         from aliases import ALIAS_LIST
-        import mud
+        import pymudclient
         from settings import (
             HOST,
             PORT,
         )
         from timers import TIMER_LIST
         from triggers import TRIGGER_LIST
         
@@ -87,15 +95,15 @@
         - func `function`: (optional) 要呼叫的 function，會傳一個 `text` 參數，會把除了 start_text 外的後面的文字全部傳入；如果 function 有回傳文字，會傳給 host。
         
         pattern 跟 func 2 選 1。
         
         #### 使用範例
         
         ```py
-        from mud import Alias
+        from pymudclient import Alias
         
         ALIAS_LIST = [
             Alias('kk', pattern='kingdom %0'),
             Alias('c', pattern='cast %1 on %2'),
             Alias('draw', pattern='draw %1 %-1'),
         ]
         ```
@@ -111,14 +119,16 @@
         - pattern `string`: 觸發的 pattern，使用 regex。
         - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
         - func `function`: (optional) 要呼叫的 function，會傳一個 `match` 參數，會把 regex match 到的 `match.groups()` 傳入；如果 function 有回傳文字，會傳給 host。
         
         #### 使用範例
         
         ```py
+        from pymudclient import Trigger
+        
         def summon(match):
             return f'summon {match[0]}'
         
         TRIGGER_LIST = [
             Trigger(r"^您的英文名字\(新人物請輸入\'new\'\) :$", data=USER),
             Trigger(r"^請輸入密碼﹕$", data=PW),
             Trigger(r'\(([a-zA-Z]+)\)告訴你﹕sum$', func=summon),
@@ -135,21 +145,27 @@
         - seconds `number`: 多久執行一次，單位是秒。
         - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
         - func `function`: (optional) 要呼叫的 function；如果 function 有回傳文字，會傳給 host。
         
         #### 使用範例
         
         ```py
+        from pymudclient import Timer
+        
         TIMER_LIST = [
             Timer(900, data='save'),
         ]
         ```
         
         - 每 900 秒傳送一個 `save` 到 host。
         
+        ## 已知問題
+        
+        - 部分中文字顯示會有不正確位置的換行。
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pymudclient-0.1.0/README.md` & `pymudclient-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # pymudclient: 用 Python 開發的 MUD Client 核心
 
 - [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
   - [功能說明](#功能說明)
+  - [安裝](#安裝)
   - [使用範例](#使用範例)
   - [功能說明](#功能說明-1)
     - [mud_run](#mud_run)
     - [Alias](#alias)
       - [Alias class 參數](#alias-class-參數)
       - [使用範例](#使用範例-1)
     - [Trigger](#trigger)
       - [Trigger class 參數](#trigger-class-參數)
       - [使用範例](#使用範例-2)
     - [Timer](#timer)
       - [Timer class 參數](#timer-class-參數)
       - [使用範例](#使用範例-3)
+  - [已知問題](#已知問題)
 
 ## 這是什麼？
 
 - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
 - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
 
 ## 已測試過環境
@@ -28,21 +30,27 @@
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
 ## 功能說明
 
 - 連線：根據輸入的 host 跟 port 進行連線。
 - 斷線重連：發生異常、server 重新啟動導致的斷線，會等待 3 秒後重新連線。
 - 顯示：顯示 server 回傳的內容。
+  - 有處理 big5 中文顯示的問題。
+  - 只針對萬王之王 (kk.muds.idv.tw:4000) 進行測試過。
 - 輸入介面：在最後一行顯示輸入的文字；送出的文字還沒有改動時按下 Enter 會再送一次。
 
+## 安裝
+
+`pip install pymudclient`
+
 ## 使用範例
 
 ```py
 from aliases import ALIAS_LIST
-import mud
+import pymudclient
 from settings import (
     HOST,
     PORT,
 )
 from timers import TIMER_LIST
 from triggers import TRIGGER_LIST
 
@@ -78,15 +86,15 @@
 - func `function`: (optional) 要呼叫的 function，會傳一個 `text` 參數，會把除了 start_text 外的後面的文字全部傳入；如果 function 有回傳文字，會傳給 host。
 
 pattern 跟 func 2 選 1。
 
 #### 使用範例
 
 ```py
-from mud import Alias
+from pymudclient import Alias
 
 ALIAS_LIST = [
     Alias('kk', pattern='kingdom %0'),
     Alias('c', pattern='cast %1 on %2'),
     Alias('draw', pattern='draw %1 %-1'),
 ]
 ```
@@ -102,14 +110,16 @@
 - pattern `string`: 觸發的 pattern，使用 regex。
 - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
 - func `function`: (optional) 要呼叫的 function，會傳一個 `match` 參數，會把 regex match 到的 `match.groups()` 傳入；如果 function 有回傳文字，會傳給 host。
 
 #### 使用範例
 
 ```py
+from pymudclient import Trigger
+
 def summon(match):
     return f'summon {match[0]}'
 
 TRIGGER_LIST = [
     Trigger(r"^您的英文名字\(新人物請輸入\'new\'\) :$", data=USER),
     Trigger(r"^請輸入密碼﹕$", data=PW),
     Trigger(r'\(([a-zA-Z]+)\)告訴你﹕sum$', func=summon),
@@ -126,13 +136,19 @@
 - seconds `number`: 多久執行一次，單位是秒。
 - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
 - func `function`: (optional) 要呼叫的 function；如果 function 有回傳文字，會傳給 host。
 
 #### 使用範例
 
 ```py
+from pymudclient import Timer
+
 TIMER_LIST = [
     Timer(900, data='save'),
 ]
 ```
 
 - 每 900 秒傳送一個 `save` 到 host。
+
+## 已知問題
+
+- 部分中文字顯示會有不正確位置的換行。
```

### Comparing `pymudclient-0.1.0/pymudclient/input_cmd.py` & `pymudclient-0.1.1/pymudclient/input_cmd.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient/kbhit.py` & `pymudclient-0.1.1/pymudclient/kbhit.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient/mud.py` & `pymudclient-0.1.1/pymudclient/mud.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient/recv.py` & `pymudclient-0.1.1/pymudclient/recv.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient/shared_data.py` & `pymudclient-0.1.1/pymudclient/shared_data.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient/utils/colors.py` & `pymudclient-0.1.1/pymudclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient/utils/print.py` & `pymudclient-0.1.1/pymudclient/utils/print.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pymudclient.egg-info/PKG-INFO` & `pymudclient-0.1.1/pymudclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/pymudclient/
 Description: # pymudclient: 用 Python 開發的 MUD Client 核心
         
         - [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
           - [這是什麼？](#這是什麼)
           - [已測試過環境](#已測試過環境)
           - [功能說明](#功能說明)
+          - [安裝](#安裝)
           - [使用範例](#使用範例)
           - [功能說明](#功能說明-1)
             - [mud_run](#mud_run)
             - [Alias](#alias)
               - [Alias class 參數](#alias-class-參數)
               - [使用範例](#使用範例-1)
             - [Trigger](#trigger)
               - [Trigger class 參數](#trigger-class-參數)
               - [使用範例](#使用範例-2)
             - [Timer](#timer)
               - [Timer class 參數](#timer-class-參數)
               - [使用範例](#使用範例-3)
+          - [已知問題](#已知問題)
         
         ## 這是什麼？
         
         - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
         - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
         
         ## 已測試過環境
@@ -37,21 +39,27 @@
         - GNU/Linux 5.15.0-1032-raspi aarch64
         
         ## 功能說明
         
         - 連線：根據輸入的 host 跟 port 進行連線。
         - 斷線重連：發生異常、server 重新啟動導致的斷線，會等待 3 秒後重新連線。
         - 顯示：顯示 server 回傳的內容。
+          - 有處理 big5 中文顯示的問題。
+          - 只針對萬王之王 (kk.muds.idv.tw:4000) 進行測試過。
         - 輸入介面：在最後一行顯示輸入的文字；送出的文字還沒有改動時按下 Enter 會再送一次。
         
+        ## 安裝
+        
+        `pip install pymudclient`
+        
         ## 使用範例
         
         ```py
         from aliases import ALIAS_LIST
-        import mud
+        import pymudclient
         from settings import (
             HOST,
             PORT,
         )
         from timers import TIMER_LIST
         from triggers import TRIGGER_LIST
         
@@ -87,15 +95,15 @@
         - func `function`: (optional) 要呼叫的 function，會傳一個 `text` 參數，會把除了 start_text 外的後面的文字全部傳入；如果 function 有回傳文字，會傳給 host。
         
         pattern 跟 func 2 選 1。
         
         #### 使用範例
         
         ```py
-        from mud import Alias
+        from pymudclient import Alias
         
         ALIAS_LIST = [
             Alias('kk', pattern='kingdom %0'),
             Alias('c', pattern='cast %1 on %2'),
             Alias('draw', pattern='draw %1 %-1'),
         ]
         ```
@@ -111,14 +119,16 @@
         - pattern `string`: 觸發的 pattern，使用 regex。
         - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
         - func `function`: (optional) 要呼叫的 function，會傳一個 `match` 參數，會把 regex match 到的 `match.groups()` 傳入；如果 function 有回傳文字，會傳給 host。
         
         #### 使用範例
         
         ```py
+        from pymudclient import Trigger
+        
         def summon(match):
             return f'summon {match[0]}'
         
         TRIGGER_LIST = [
             Trigger(r"^您的英文名字\(新人物請輸入\'new\'\) :$", data=USER),
             Trigger(r"^請輸入密碼﹕$", data=PW),
             Trigger(r'\(([a-zA-Z]+)\)告訴你﹕sum$', func=summon),
@@ -135,21 +145,27 @@
         - seconds `number`: 多久執行一次，單位是秒。
         - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
         - func `function`: (optional) 要呼叫的 function；如果 function 有回傳文字，會傳給 host。
         
         #### 使用範例
         
         ```py
+        from pymudclient import Timer
+        
         TIMER_LIST = [
             Timer(900, data='save'),
         ]
         ```
         
         - 每 900 秒傳送一個 `save` 到 host。
         
+        ## 已知問題
+        
+        - 部分中文字顯示會有不正確位置的換行。
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pymudclient-0.1.0/pymudclient.egg-info/SOURCES.txt` & `pymudclient-0.1.1/pymudclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/pyproject.toml` & `pymudclient-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymudclient-0.1.0/setup.py` & `pymudclient-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = 'pymudclient'
 AUTHOR = 'griiid'
 AUTHOR_EMAIL = 'gridwing@gmail.com'
 URL = 'https://github.com/griiid/PyMudClient'
 DOWNLOAD_URL = 'https://pypi.org/project/pymudclient/'
 
 LICENSE = 'MIT'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A MUD client core written in Python'
 LONG_DESCRIPTION = (HERE  / 'README.md').read_text(encoding='utf8')
 LONG_DESC_TYPE = 'text/markdown'
 
 requirements = (HERE / 'requirements.txt').read_text(encoding='utf8')
 INSTALL_REQUIRES = [s.strip() for s in requirements.split('\n')]
```

