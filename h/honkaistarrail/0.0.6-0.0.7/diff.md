# Comparing `tmp/honkaistarrail-0.0.6.tar.gz` & `tmp/honkaistarrail-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkaistarrail-0.0.6.tar", max compression
+gzip compressed data, was "honkaistarrail-0.0.7.tar", max compression
```

## Comparing `honkaistarrail-0.0.6.tar` & `honkaistarrail-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.6/honkaistarrail/calculator.py
--rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.6/honkaistarrail/modal.py
--rw-r--r--   0        0        0    16020 2023-06-29 13:08:01.698918 honkaistarrail-0.0.6/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
--rw-r--r--   0        0        0    19055 2023-06-29 13:07:56.646895 honkaistarrail-0.0.6/honkaistarrail/src/data/gacha/gacha_data.py
--rw-r--r--   0        0        0     7096 2023-06-29 13:04:23.019999 honkaistarrail-0.0.6/honkaistarrail/starrail.py
--rw-r--r--   0        0        0      480 2023-06-29 13:08:23.922647 honkaistarrail-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.6/README.md
--rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.6/setup.py
--rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.7/honkaistarrail/calculator.py
+-rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.7/honkaistarrail/modal.py
+-rw-r--r--   0        0        0    16020 2023-06-29 13:08:01.698918 honkaistarrail-0.0.7/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
+-rw-r--r--   0        0        0    19055 2023-06-29 13:07:56.646895 honkaistarrail-0.0.7/honkaistarrail/src/data/gacha/gacha_data.py
+-rw-r--r--   0        0        0     7097 2023-06-29 13:15:22.981460 honkaistarrail-0.0.7/honkaistarrail/starrail.py
+-rw-r--r--   0        0        0      480 2023-06-29 13:15:32.091773 honkaistarrail-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.7/README.md
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.7/setup.py
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.7/PKG-INFO
```

### Comparing `honkaistarrail-0.0.6/honkaistarrail/calculator.py` & `honkaistarrail-0.0.7/honkaistarrail/calculator.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.6/honkaistarrail/modal.py` & `honkaistarrail-0.0.7/honkaistarrail/modal.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.6/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc` & `honkaistarrail-0.0.7/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.6/honkaistarrail/src/data/gacha/gacha_data.py` & `honkaistarrail-0.0.7/honkaistarrail/src/data/gacha/gacha_data.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.6/honkaistarrail/starrail.py` & `honkaistarrail-0.0.7/honkaistarrail/starrail.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     
     async def get_images(self, itmes_id):
         items = gacha_data.items.get(str(itmes_id), None)
         if items == None:
             raise ValueError('Information not found in the database, try updating the module version.')
         
         
-        keys_image_mini = items.get("icon","a30bc8cb7d4bed2a72c52b43949ac07e010f3ba1c5f6fe05c70d7f31feb234f1")
-        keys_image_full = items.get("splashIcon","a30bc8cb7d4bed2a72c52b43949ac07e010f3ba1c5f6fe05c70d7f31feb234f1")
+        keys_image_mini = items.get("artPath","a30bc8cb7d4bed2a72c52b43949ac07e010f3ba1c5f6fe05c70d7f31feb234f1")
+        keys_image_full = items.get("iconPath","a30bc8cb7d4bed2a72c52b43949ac07e010f3ba1c5f6fe05c70d7f31feb234f1")
         
         return ImageGacha(icon = _LINK_DATA_IMAGE.format(keys = keys_image_mini), full =  _LINK_DATA_IMAGE.format(keys = keys_image_full))
 
 
 
     def set_parameters(self):
         params = urllib.parse.parse_qs(urllib.parse.urlparse(self.link).query)
```

### Comparing `honkaistarrail-0.0.6/README.md` & `honkaistarrail-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.6/setup.py` & `honkaistarrail-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['honkaistarrail', 'honkaistarrail.src.data.gacha']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkaistarrail',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Asynchronous module for working with API Honkai: Star Rail',
     'long_description': '<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/HSR-BANNER.png" />\n</p>\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install honkaistarrail\n```\nPyPi: [OPEN](https://pypi.org/project/honkaistarrail/)\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n### ID Banned:\n``1`` - Event Banner\n``2`` - Light Cone\n``3`` - Standart Banner\n\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom honkaistarrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link = link,banner = 1,lang = "en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\n\n# In developing:\n\n1. Automatic code redemption.\n2. Automatic collection of daily marks on HoYoLab.\n\n___\n<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/%D0%91%D0%B5%D0%B7-%D0%B8%D0%BC%D0%B5%D0%BD%D0%B8-1.png" />\n</p>\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiStarRail.py',
```

### Comparing `honkaistarrail-0.0.6/PKG-INFO` & `honkaistarrail-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honkaistarrail
-Version: 0.0.6
+Version: 0.0.7
 Summary: Asynchronous module for working with API Honkai: Star Rail
 Home-page: https://github.com/DEViantUA/HonkaiStarRail.py
 Author: None
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

