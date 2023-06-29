# Comparing `tmp/pdocr_rpc-2023.6.14.tar.gz` & `tmp/pdocr_rpc-2023.6.29.tar.gz`

## Comparing `pdocr_rpc-2023.6.14.tar` & `pdocr_rpc-2023.6.29.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6441 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/conf.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pdocr_rpc/server.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/pyproject.toml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.14/PKG-INFO
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/pdocr_rpc/conf.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/pdocr_rpc/server.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/pyproject.toml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pdocr_rpc-2023.6.29/PKG-INFO
```

### Comparing `pdocr_rpc-2023.6.14/pdocr_rpc/__init__.py` & `pdocr_rpc-2023.6.29/pdocr_rpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # _*_ coding:utf-8 _*_
 """
 @Author: Mikigo
 @Date: 2022/5/25 0:03
 """
 import json
 import os
-from os import popen, environ
+from pprint import pprint
 from xmlrpc.client import Binary
 from xmlrpc.client import ServerProxy
 
 from pdocr_rpc.conf import setting
 
-environ["DISPLAY"] = ":0"
+os.environ["DISPLAY"] = ":0"
 
 if setting.IS_LINUX:
     import pyscreenshot as ImageGrab
 elif setting.IS_WINDOWS:
     from PIL import ImageGrab
 
 
@@ -29,15 +29,15 @@
         """
         if not picture_abspath:
             picture_abspath = setting.SCREEN_CACHE
             if setting.IS_X11:
                 ImageGrab.grab().save(os.path.expanduser(picture_abspath))
             else:
                 picture_abspath = (
-                    popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
+                    os.popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
                     .read()
                     .strip("\n")
                 )
         server = ServerProxy(
             f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True
         )
         put_handle = open(os.path.expanduser(picture_abspath), "rb")
@@ -161,12 +161,13 @@
                         n += 1
 
             if more_map:
                 print(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
                 return more_map
 
         print(f"未识别到字符{f'“{target_strings}”' or ''}")
+        pprint(results)
         return False
 
 
 if __name__ == "__main__":
-    print(ocr())
+    print(OCR.ocr())
```

### Comparing `pdocr_rpc-2023.6.14/pdocr_rpc/conf.py` & `pdocr_rpc-2023.6.29/pdocr_rpc/conf.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2023.6.14/pdocr_rpc/server.py` & `pdocr_rpc-2023.6.29/pdocr_rpc/server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2023.6.14/LICENSE` & `pdocr_rpc-2023.6.29/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2023.6.14/README.md` & `pdocr_rpc-2023.6.29/README.md`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2023.6.14/pyproject.toml` & `pdocr_rpc-2023.6.29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pdocr-rpc"
 authors = [
```

### Comparing `pdocr_rpc-2023.6.14/PKG-INFO` & `pdocr_rpc-2023.6.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 2023.6.14
+Version: 2023.6.29
 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/funny-dream/pdocr-rpc
 Project-URL: Documentation, https://funny-dream.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdocr-rpc Version: 2023.6.14 Summary: PaddleOCR-RPC
+Metadata-Version: 2.1 Name: pdocr-rpc Version: 2023.6.29 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/funny-dream/pdocr-rpc Project-URL:
 Documentation, https://funny-dream.github.io/pdocr-rpc Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Requires-Dist: pillow; sys_platform == 'win32' Requires-Dist: pyscreenshot;
 sys_platform == 'linux' Provides-Extra: doc Requires-Dist: mkdocs-material;
```

