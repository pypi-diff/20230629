# Comparing `tmp/LogTranslate-1.1.tar.gz` & `tmp/LogTranslate-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.1.tar", last modified: Wed Jun 28 15:57:11 2023, max compression
+gzip compressed data, was "LogTranslate-1.2.tar", last modified: Thu Jun 29 14:55:03 2023, max compression
```

## Comparing `LogTranslate-1.1.tar` & `LogTranslate-1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 15:57:11.797219 LogTranslate-1.1/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-28 15:57:11.778278 LogTranslate-1.1/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3181 2023-06-28 15:57:11.000000 LogTranslate-1.1/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-06-28 15:57:11.000000 LogTranslate-1.1/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 15:57:11.000000 LogTranslate-1.1/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-28 15:57:11.000000 LogTranslate-1.1/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-28 15:57:11.000000 LogTranslate-1.1/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3181 2023-06-28 15:57:11.796279 LogTranslate-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 15:57:11.789245 LogTranslate-1.1/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:57:11.793270 LogTranslate-1.1/log_translate/business/
--rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0     3848 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/config_default.py
--rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/data_struct.py
--rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/gloable.py
--rw-rw-rw-   0        0        0     4362 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:57:11.795226 LogTranslate-1.1/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.1/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     7111 2023-06-28 15:47:22.000000 LogTranslate-1.1/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7099 2023-06-28 15:47:22.000000 LogTranslate-1.1/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 15:57:11.797219 LogTranslate-1.1/setup.cfg
--rw-rw-rw-   0        0        0     2165 2023-06-28 15:52:11.000000 LogTranslate-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:55:03.000116 LogTranslate-1.2/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 14:55:02.988156 LogTranslate-1.2/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3181 2023-06-29 14:55:02.000000 LogTranslate-1.2/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-06-29 14:55:02.000000 LogTranslate-1.2/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:55:02.000000 LogTranslate-1.2/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-29 14:55:02.000000 LogTranslate-1.2/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 14:55:02.000000 LogTranslate-1.2/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3181 2023-06-29 14:55:02.999120 LogTranslate-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:55:02.996130 LogTranslate-1.2/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:55:02.998123 LogTranslate-1.2/log_translate/business/
+-rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0     3848 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4443 2023-06-29 14:49:11.000000 LogTranslate-1.2/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:55:02.999120 LogTranslate-1.2/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     7386 2023-06-29 14:53:32.000000 LogTranslate-1.2/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7374 2023-06-29 14:53:32.000000 LogTranslate-1.2/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:55:03.000116 LogTranslate-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2197 2023-06-29 14:54:53.000000 LogTranslate-1.2/setup.py
```

### Comparing `LogTranslate-1.1/LICENSE.txt` & `LogTranslate-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.2/LogTranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.1
+Version: 1.2
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.1/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.2/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/PKG-INFO` & `LogTranslate-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.1
+Version: 1.2
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.1/README.md` & `LogTranslate-1.2/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.2/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.2/log_translate/business/bluetooth_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/log_translate/data_struct.py` & `LogTranslate-1.2/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/log_translate/log_translator.py` & `LogTranslate-1.2/log_translate/log_translator.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # :param pattern_translators 是数据[tag,fun(tag, msg)] fun参数必须是(tag, msg)
 class TagPatternTranslator(object):
     def __init__(self, pattern_translators):
         self.pattern_translators = pattern_translators
 
     def translate(self, tag, msg):
         for pattern in self.pattern_translators:
-            match = re.compile(pattern, re.IGNORECASE).match(tag)
+            match = re.compile(pattern, re.IGNORECASE).fullmatch(tag)
             if match:
                 translator = self.pattern_translators[pattern]
                 if callable(translator):
                     return translator(tag, msg)
                 else:
                     return translator.translate(tag, msg)
         return None
@@ -34,29 +34,29 @@
             if callable(translator):
                 return translator(msg)
             else:
                 return translator.translate(msg)
         return None
 
 
-class SecStrTagTranslator(TagStrTranslator):
+class SubTagTranslator(TagPatternTranslator):
     """
     :param father表示上一级tag
     :param tag_from_str_fun 从字符串解析tag的方法
     :param tag_translators 用来解析二级tag的translator 是个数组必须是TagStrTranslator|TagPatternTranslator
     """
 
     def __init__(self, father, tag_from_str_fun, tag_translators):
         super().__init__({
-            father: self.translate_new_tag
+            father: self.translate_sub_tag
         })
         self.tag_from_str_fun = tag_from_str_fun
         self.tag_translators = tag_translators
 
-    def translate_new_tag(self, msg):
+    def translate_sub_tag(self, msg):
         log = self.tag_from_str_fun(msg)
         if log:
             sec_tag = log.group("tag")
             sec_msg = log.group("msg")
             for translator in self.tag_translators:
                 result = translator.translate(sec_tag, sec_msg)
                 if result:
@@ -120,7 +120,9 @@
     #
     print(result.group())
 
     str = "04-29 10:01:16.788935  1848  2303 D OGG_Detector: D:done mCurrStatus: 0"
     f = re.search(r"(?P<time>\d+.*\.\d{3,}) +(?P<pid>\d+).* [A-Z] (?P<tag>.*?) *:(?P<msg>.*)", str)
     print(f.group("pid"))
     print(f.group("tag"))
+
+    print(re.compile("testb", re.IGNORECASE).fullmatch("testb").group())
```

### Comparing `LogTranslate-1.1/log_translate/read_log_file.py` & `LogTranslate-1.2/log_translate/read_log_file.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/log_translate/res/log_logo.ico` & `LogTranslate-1.2/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.1/log_translate/ui_pyqt6.py` & `LogTranslate-1.2/log_translate/ui_pyqt6.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         filter_action.setShortcut('Ctrl+E')
         filter_action.triggered.connect(self.filter_logs_e)
         action.addAction(filter_action)
 
         keyboard.add_hotkey('Ctrl+O', self.log_show_origin)
         keyboard.add_hotkey('Ctrl+Up', self.font_zoom_in)
         keyboard.add_hotkey('Ctrl+Down', self.font_zoom_out)
+        keyboard.add_hotkey('Ctrl+R', self.log_clear)
 
     def dragEnterEvent(self, event):
         if event.mimeData().hasUrls():
             if not self.isMaximized():
                 self.showMaximized()
             event.accept()
         else:
@@ -125,36 +126,45 @@
     def filter_logs_e(self):
         self.filter_logs(Level.e)
 
     def log_show_origin(self):
         self.show_origin = not self.show_origin
         self.filter_logs(Level(self.show_level))
 
+    def filter_logs(self, level: Level):
+        self.show_level = level.value
+        first = self.list_widget.item(0).text()
+        self.list_widget.clear()
+        self.list_widget.addItem(first)
+        show_logs = self.data_item_logs[self.show_level]
+        for log in show_logs:
+            self.list_widget.addItem(self.log_to_list_item(log))
+
     # 字体缩小
     def font_zoom_out(self):
         font: QFont = self.list_widget.font()
         new_font = QFont()
         new_font.setPointSize(font.pointSize() - 1)
         self.list_widget.setFont(new_font)
 
     # 字体放大
     def font_zoom_in(self):
         font: QFont = self.list_widget.font()
         new_font = QFont()
         new_font.setPointSize(font.pointSize() + 1)
         self.list_widget.setFont(new_font)
 
-    def filter_logs(self, level: Level):
-        self.show_level = level.value
-        first = self.list_widget.item(0).text()
-        self.list_widget.clear()
-        self.list_widget.addItem(first)
-        show_logs = self.data_item_logs[self.show_level]
-        for log in show_logs:
-            self.list_widget.addItem(self.log_to_list_item(log))
+    # 清空缓存
+    def log_clear(self):
+        self.data_item_logs = {
+            Level.d.value: [],
+            Level.i.value: [],
+            Level.w.value: [],
+            Level.e.value: [],
+        }
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
     window = PyQt6Window()
     window.show()
     sys.exit(app.exec())
```

### Comparing `LogTranslate-1.1/log_translate/ui_pyside2.py` & `LogTranslate-1.2/log_translate/ui_pyside2.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         filter_action.setShortcut('Ctrl+E')
         filter_action.triggered.connect(self.filter_logs_e)
         action.addAction(filter_action)
 
         keyboard.add_hotkey('Ctrl+O', self.log_show_origin)
         keyboard.add_hotkey('Ctrl+Up', self.font_zoom_in)
         keyboard.add_hotkey('Ctrl+Down', self.font_zoom_out)
+        keyboard.add_hotkey('Ctrl+R', self.log_clear)
 
     def dragEnterEvent(self, event):
         if event.mimeData().hasUrls():
             if not self.isMaximized():
                 self.showMaximized()
             event.accept()
         else:
@@ -125,36 +126,45 @@
     def filter_logs_e(self):
         self.filter_logs(Level.e)
 
     def log_show_origin(self):
         self.show_origin = not self.show_origin
         self.filter_logs(Level(self.show_level))
 
+    def filter_logs(self, level: Level):
+        self.show_level = level.value
+        first = self.list_widget.item(0).text()
+        self.list_widget.clear()
+        self.list_widget.addItem(first)
+        show_logs = self.data_item_logs[self.show_level]
+        for log in show_logs:
+            self.list_widget.addItem(self.log_to_list_item(log))
+
     # 字体缩小
     def font_zoom_out(self):
         font: QFont = self.list_widget.font()
         new_font = QFont()
         new_font.setPointSize(font.pointSize() - 1)
         self.list_widget.setFont(new_font)
 
     # 字体放大
     def font_zoom_in(self):
         font: QFont = self.list_widget.font()
         new_font = QFont()
         new_font.setPointSize(font.pointSize() + 1)
         self.list_widget.setFont(new_font)
 
-    def filter_logs(self, level: Level):
-        self.show_level = level.value
-        first = self.list_widget.item(0).text()
-        self.list_widget.clear()
-        self.list_widget.addItem(first)
-        show_logs = self.data_item_logs[self.show_level]
-        for log in show_logs:
-            self.list_widget.addItem(self.log_to_list_item(log))
+    # 清空缓存
+    def log_clear(self):
+        self.data_item_logs = {
+            Level.d.value: [],
+            Level.i.value: [],
+            Level.w.value: [],
+            Level.e.value: [],
+        }
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
     window = PySide6Window()
     window.show()
     sys.exit(app.exec())
```

### Comparing `LogTranslate-1.1/setup.py` & `LogTranslate-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
 ICON_PATH = 'res/*.ico'
 
 setup(
     name='LogTranslate',
-    version='1.1',
+    version='1.2',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
@@ -43,12 +43,13 @@
     ],
     keywords='tools log translate',
     url='https://github.com/5hmlA/PyTools',
     description='A Python library for translate log from log files'
 )
 
 # python -m pip install --upgrade twine
+# pip install wheel setuptools
 # python setup.py sdist bdist_wheel
 
 # 发布到测试地址
 # twine upload --repository testpypi dist/*
 # twine upload dist/*
```

