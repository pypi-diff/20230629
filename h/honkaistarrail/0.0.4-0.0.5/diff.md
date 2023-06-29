# Comparing `tmp/honkaistarrail-0.0.4.tar.gz` & `tmp/honkaistarrail-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkaistarrail-0.0.4.tar", max compression
+gzip compressed data, was "honkaistarrail-0.0.5.tar", max compression
```

## Comparing `honkaistarrail-0.0.4.tar` & `honkaistarrail-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.4/honkaistarrail/calculator.py
--rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.4/honkaistarrail/modal.py
--rw-r--r--   0        0        0    29135 2023-05-04 13:30:29.205747 honkaistarrail-0.0.4/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
--rw-r--r--   0        0        0    38022 2023-05-04 13:30:26.497309 honkaistarrail-0.0.4/honkaistarrail/src/data/gacha/gacha_data.py
--rw-r--r--   0        0        0     6977 2023-05-29 19:55:18.822822 honkaistarrail-0.0.4/honkaistarrail/starrail.py
--rw-r--r--   0        0        0      480 2023-05-29 19:56:15.501740 honkaistarrail-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.4/README.md
--rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.4/setup.py
--rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.5/honkaistarrail/calculator.py
+-rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.5/honkaistarrail/modal.py
+-rw-r--r--   0        0        0    22251 2023-06-29 12:55:21.035102 honkaistarrail-0.0.5/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
+-rw-r--r--   0        0        0    29820 2023-06-29 12:52:34.916622 honkaistarrail-0.0.5/honkaistarrail/src/data/gacha/gacha_data.py
+-rw-r--r--   0        0        0     7122 2023-06-29 12:56:03.490223 honkaistarrail-0.0.5/honkaistarrail/starrail.py
+-rw-r--r--   0        0        0      480 2023-06-29 12:56:24.023694 honkaistarrail-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.5/README.md
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.5/setup.py
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.5/PKG-INFO
```

### Comparing `honkaistarrail-0.0.4/honkaistarrail/calculator.py` & `honkaistarrail-0.0.5/honkaistarrail/calculator.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.4/honkaistarrail/modal.py` & `honkaistarrail-0.0.5/honkaistarrail/modal.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.4/honkaistarrail/starrail.py` & `honkaistarrail-0.0.5/honkaistarrail/starrail.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 class Jump:
     def __init__(self, link = "", banner = 1, lang = "en",limit = 0,reg = "os") -> None:
 
         examination(lang,banner)
         self.link = link
         if self.link == "":
             self.get_auto_link(reg=reg)
+        print(self.link)
         self.limit = limit
         self.lang = lang
         self.banner = str(banner)
         if self.link != "-":
             data = self.set_parameters()
 
             if data.authkey == None:
@@ -70,17 +71,17 @@
 
 
             self.history = []
             self.response = None
 
     def get_auto_link(self, reg = "os"):
         if reg.lower() == "os":
-            cmd = ['powershell', '-Command', 'Invoke-Expression (New-Object Net.WebClient).DownloadString("https://gist.githubusercontent.com/DEViantUA/d5b77400c5d710e4260474afa5011d17/raw/bd8c200f7906fb005d4d11097a8f95e4feb8823f/HonkaiStarRailJump.ps1")'] 
+            cmd = ['powershell', '-Command', 'Invoke-Expression (New-Object Net.WebClient).DownloadString("https://gist.githubusercontent.com/DEViantUA/79d635767620951128a967bf8cfc9049/raw/29b02aa151fa9978c69cda2d5ea9bf06ff416182/HSR_OS.ps1")'] 
         elif reg.lower() == "cn":
-            cmd = ['powershell', '-Command', 'Invoke-Expression (New-Object Net.WebClient).DownloadString("https://gist.githubusercontent.com/DEViantUA/19d224c9c13e6f6b1cc62a12fc0e8a9d/raw/9dcd08b8033d9e60921e216c7219354e863e13b5/HonkaiStarRailJump_CN.ps1")'] 
+            cmd = ['powershell', '-Command', 'Invoke-Expression (New-Object Net.WebClient).DownloadString("https://gist.githubusercontent.com/DEViantUA/61f9d4d8f762467923b5000fbe6bbdc6/raw/71802147293fd29f8162bc2c537bbda7481dad8c/HSR_CN.ps1")'] 
         else:
             raise ValueError('The reg parameter takes values: os or cn')
         result = subprocess.run(cmd, capture_output=True, text=True)
         if result.returncode == 0:
             self.link = next(filter(None, map(str.strip, reversed(result.stdout.splitlines()))))
         elif result.returncode == 1:
             raise ValueError('Try changing reg to ch or os')
@@ -154,7 +155,14 @@
     
     async def get_gacha(self):
         items = []
         async for key in self.get_history(gacha=True):
             items.extend(key)
         return await get_result(items)
 
+
+class HoYoLab:
+    def __init__(self,lang = "en",reg = "os") -> None:
+        self.lang = lang
+        self.reg = reg
+        pass
+
```

### Comparing `honkaistarrail-0.0.4/README.md` & `honkaistarrail-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.4/setup.py` & `honkaistarrail-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['honkaistarrail', 'honkaistarrail.src.data.gacha']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkaistarrail',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Asynchronous module for working with API Honkai: Star Rail',
     'long_description': '<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/HSR-BANNER.png" />\n</p>\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install honkaistarrail\n```\nPyPi: [OPEN](https://pypi.org/project/honkaistarrail/)\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n### ID Banned:\n``1`` - Event Banner\n``2`` - Light Cone\n``3`` - Standart Banner\n\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom honkaistarrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link = link,banner = 1,lang = "en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\n\n# In developing:\n\n1. Automatic code redemption.\n2. Automatic collection of daily marks on HoYoLab.\n\n___\n<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/%D0%91%D0%B5%D0%B7-%D0%B8%D0%BC%D0%B5%D0%BD%D0%B8-1.png" />\n</p>\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiStarRail.py',
```

### Comparing `honkaistarrail-0.0.4/PKG-INFO` & `honkaistarrail-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honkaistarrail
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asynchronous module for working with API Honkai: Star Rail
 Home-page: https://github.com/DEViantUA/HonkaiStarRail.py
 Author: None
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

