# Comparing `tmp/pysmart365-0.0.9.tar.gz` & `tmp/pysmart365-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.9.tar", last modified: Thu Jun 22 20:40:35 2023, max compression
+gzip compressed data, was "pysmart365-0.1.0.tar", last modified: Thu Jun 29 11:23:50 2023, max compression
```

## Comparing `pysmart365-0.0.9.tar` & `pysmart365-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 20:40:35.681004 pysmart365-0.0.9/
--rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      353 2023-06-22 20:40:35.680007 pysmart365-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-15 10:39:32.000000 pysmart365-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 20:40:35.670034 pysmart365-0.0.9/pysmart365/
--rw-rw-rw-   0        0        0     3489 2023-06-22 20:38:13.000000 pysmart365-0.0.9/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     1822 2023-06-15 10:30:41.000000 pysmart365-0.0.9/pysmart365/__init__.py
--rw-rw-rw-   0        0        0      635 2023-06-22 20:38:31.000000 pysmart365-0.0.9/pysmart365/modules.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:40:35.680007 pysmart365-0.0.9/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 20:40:35.681004 pysmart365-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-06-22 20:40:33.000000 pysmart365-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:23:50.283623 pysmart365-0.1.0/
+-rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-06-29 11:23:50.283623 pysmart365-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-06-29 11:21:53.000000 pysmart365-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 11:23:50.257692 pysmart365-0.1.0/pysmart365/
+-rw-rw-rw-   0        0        0     3102 2023-06-29 11:09:47.000000 pysmart365-0.1.0/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     2483 2023-06-29 11:13:27.000000 pysmart365-0.1.0/pysmart365/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-06-29 10:45:00.000000 pysmart365-0.1.0/pysmart365/modules.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:23:50.281666 pysmart365-0.1.0/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 11:23:50.283623 pysmart365-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-06-29 11:15:01.000000 pysmart365-0.1.0/setup.py
```

### Comparing `pysmart365-0.0.9/LICENSE` & `pysmart365-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.9/pysmart365/MicroSoftware.py` & `pysmart365-0.1.0/pysmart365/MicroSoftware.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,92 +10,79 @@
     view_time = datetime.now().strftime("%H:%M:%S")
     return view_time
 
 def view_date():
     view_date = datetime.now().strftime("%d/%m/%Y")
     return view_date
 
-def sleep(delay):
+def sleep(delay: str) -> None:
     if delay == '0' or delay is None:
         time.sleep(0)
     elif delay:
         time.sleep(delay)
-    else:
-        print("Error")
-
-class center_screen():
-    def __init__(self, width: int = None, height: int = None):
-        screen_width = Tk().winfo_screenwidth()
-        screen_height = Tk().winfo_screenheight()
-        x = (screen_width - width) // 2
-        y = (screen_height - height) // 2
-        self.geometry = f"{width}x{height}+{x}+{y}"
-
-class EXIT():
-    def __init__(self):
-        sys.exit()
 
 class wintools():
-    def mrt(self, secs: float) -> None:
+    def mrt() -> None:
         if os.path.exists(r"C:\Windows\System32\mrt.exe"):
             pyautogui.hotkey("winleft", "r")
             pyautogui.typewrite("mrt.exe")
             sleep(0.5)
             pyautogui.press("Enter")
         else:
             messagebox.showerror("Error not found", f"Program `mrt.exe` not found.")
 
-    def diskmgmt(self, secs: float) -> None:
+    def diskmgmt() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("diskmgmt.msc")
-        sleep(secs)
+        sleep(0.5)
         pyautogui.press("Enter")
 
-    def computermgmt(self, secs: float) -> None:
+    def computermgmt() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("compmgmt.msc")
-        sleep(secs)
+        sleep(0.5)
         pyautogui.press("Enter")
 
-    def notepad(self, secs: float) -> None:
+    def notepad() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("notepad.exe")
-        sleep(secs)
+        sleep(0.5)
         pyautogui.press("Enter")
 
-    def calculator(self, secs: float) -> None:
+    def calculator() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("calc.exe")
-        sleep(secs)
+        sleep(0.5)
         pyautogui.press("Enter")
 
-    def paint(self, secs: float) -> None:
+    def paint() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("mspaint.exe")
-        sleep(secs)
+        sleep(0.5)
+        pyautogui.press("Enter")
 
-    def taskmgr(self) -> None:
+    def taskmgr() -> None:
         pyautogui.hotkey("ctrl", "shift", "esc")
 
-    def explorer(self) -> None:
+    def explorer() -> None:
         pyautogui.hotkey("winleft", "e")
 
-    def cmd(self, secs: float) -> None:
+    def cmd() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("cmd.exe")
-        sleep(secs)
+        sleep()
         pyautogui.press("Enter")
 
-    def settings(self, secs: float) -> None:
+    def settings() -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("ms-settings:")
         sleep(0.5)
         pyautogui.press("Enter")
 
-    def ms_store(self, secs: float) -> None:
+    def ms_store() -> None:
         def check_microsoft_store():
             try:
                 app = Application(backend='uia').start("ms-windows-store://")
                 app.kill()
                 return True
             except Exception:
                 return False
@@ -108,7 +95,12 @@
         else:
             messagebox.showerror("Error not found", "Microsoft Store not found.")
     def runner(command) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite(command)
         time.sleep(0.5)
         pyautogui.press("Enter")
+    def clenmgr():
+        pyautogui.hotkey("Winleft", "r")
+        pyautogui.typewrite("cleanmgr")
+        time.sleep(0.5)
+        pyautogui.press("Enter")
```

### Comparing `pysmart365-0.0.9/pysmart365/__init__.py` & `pysmart365-0.1.0/pysmart365/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 AUTHOR = 'Runkang'
 COPYRIGHT = '© Copyright 2023 Informatic365 - SmartSoft - MicroSoftware'
-
 import subprocess
 import platform
 from customtkinter import *
 from tkinter import messagebox
 import sys
 
 def turn_off(time: float) -> None:
@@ -33,21 +32,38 @@
         subprocess.run(['shutdown', '-r', '-o', '-t', f'{time}'])
 def turn_off_with_gui():
     '''
     Turn Off pc with gui available on Windows 10 and 11 or successive version.
     '''
     check_windows_version = platform.win32_ver()[0]
     if check_windows_version == '7' or '8':
-        pass
+        subprocess.run(['slidetoshutdown'])
     else:
         subprocess.run(['slidetoshutdown'])
-def copyright_view(year, company):
+def set_copyright(year, company):
     '''
     Enter the copyright text that will be displayed with the name that you can customize and the year using the attribute 'company' for the name and 'year' for the year.
     Example if i write copyright_view(year='2022 - 2023', company= 'Informatic365')
     then displays "© Copyright 2022 - 2023 Informatic365".
     '''
     get = f'© Copyright {year} {company}'
     return get
 class close():
     def __init__(self) -> None:
-        sys.exit()
+        sys.exit()
+
+class wincenter():
+    def __init__(self, width, height) -> None:
+        swidth = CTk().winfo_screenwidth()
+        sheight = CTk().winfo_screenheight()
+        x = (swidth - width) // 2
+        y = (sheight - height) // 2
+        
+        self.set = f"{width}x{height}+{x}+{y}"
+
+class msbox():
+    def showinfo(self, title, message) -> None:
+        messagebox.showinfo(title=title, message=message)
+    def showerror(self, title, message) -> None:
+        messagebox.showerror(title=title, message=message)
+    def show_warning(self, title, message):
+        messagebox.showwarning(title=title, message=message)
```

### Comparing `pysmart365-0.0.9/pysmart365/modules.py` & `pysmart365-0.1.0/pysmart365/modules.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 import flask
 from flask import Flask, views, app, config, globals, helpers, logging, cli, ctx, sessions, debughelpers, testing, wrappers, blueprints, scaffold
 from ttkbootstrap import *
 from flask import *
 import random
 import string
 from customtkinter import *
-import pywinauto
+import pywinauto
```

### Comparing `pysmart365-0.0.9/setup.py` & `pysmart365-0.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import *
+import webbrowser
 setup(
     author="Runkang",
     author_email="informatic3650@gmail.com",
     name="pysmart365",
     packages=['pysmart365'],
-    version='0.0.9',
+    version='0.1.0',
     long_description='''This module is to simplify the functions of MicroSoftware and SmartSoft.''',
     description='This module is to simplify the functions of MicroSoftware and SmartSoft.',
     install_requires=[
         'screeninfo',
         'pandas',
         'pyautogui',
         'pytube',
@@ -18,9 +19,10 @@
         'requests',
         'flask',
         'ttkbootstrap',
         'configparse',
         'pywinauto',
         'jsonschema'
         ],
-    url="https://github.com/informatic365/PySmart365/"
-)
+    url="https://github.com/informatic365/PySmart365/",
+    download_url="https://pypi.org/project/pysmart365/"
+)
```

