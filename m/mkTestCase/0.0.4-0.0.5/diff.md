# Comparing `tmp/mkTestCase-0.0.4.tar.gz` & `tmp/mkTestCase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkTestCase-0.0.4.tar", last modified: Thu Jun 29 02:29:49 2023, max compression
+gzip compressed data, was "mkTestCase-0.0.5.tar", last modified: Thu Jun 29 07:31:49 2023, max compression
```

## Comparing `mkTestCase-0.0.4.tar` & `mkTestCase-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 02:29:49.261788 mkTestCase-0.0.4/
--rw-r--r--   0 yangqing   (501) staff       (20)     1066 2023-03-03 07:16:54.000000 mkTestCase-0.0.4/LICENSE
--rw-r--r--   0 yangqing   (501) staff       (20)       40 2023-06-28 07:23:33.000000 mkTestCase-0.0.4/MANIFEST.in
--rw-r--r--   0 yangqing   (501) staff       (20)     2209 2023-06-29 02:29:49.261309 mkTestCase-0.0.4/PKG-INFO
--rw-r--r--   0 yangqing   (501) staff       (20)     1548 2023-06-05 08:46:44.000000 mkTestCase-0.0.4/README.md
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 02:29:49.257521 mkTestCase-0.0.4/mkTestCase/
--rw-r--r--   0 yangqing   (501) staff       (20)      141 2023-06-26 06:18:54.000000 mkTestCase-0.0.4/mkTestCase/__init__.py
--rw-r--r--   0 yangqing   (501) staff       (20)     2869 2023-06-29 01:54:04.000000 mkTestCase-0.0.4/mkTestCase/mkTestCase.py
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 02:29:49.260390 mkTestCase-0.0.4/mkTestCase/testcases/
--rw-r--r--   0 yangqing   (501) staff       (20)     1155 2023-06-29 01:50:49.000000 mkTestCase-0.0.4/mkTestCase/testcases/form.yml
--rw-r--r--   0 yangqing   (501) staff       (20)     1034 2023-06-29 01:56:22.000000 mkTestCase-0.0.4/mkTestCase/testcases/page.yml
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 02:29:49.259269 mkTestCase-0.0.4/mkTestCase.egg-info/
--rw-r--r--   0 yangqing   (501) staff       (20)     2209 2023-06-29 02:29:49.000000 mkTestCase-0.0.4/mkTestCase.egg-info/PKG-INFO
--rw-r--r--   0 yangqing   (501) staff       (20)      315 2023-06-29 02:29:49.000000 mkTestCase-0.0.4/mkTestCase.egg-info/SOURCES.txt
--rw-r--r--   0 yangqing   (501) staff       (20)        1 2023-06-29 02:29:49.000000 mkTestCase-0.0.4/mkTestCase.egg-info/dependency_links.txt
--rw-r--r--   0 yangqing   (501) staff       (20)        9 2023-06-29 02:29:49.000000 mkTestCase-0.0.4/mkTestCase.egg-info/requires.txt
--rw-r--r--   0 yangqing   (501) staff       (20)       11 2023-06-29 02:29:49.000000 mkTestCase-0.0.4/mkTestCase.egg-info/top_level.txt
--rw-r--r--   0 yangqing   (501) staff       (20)       38 2023-06-29 02:29:49.261917 mkTestCase-0.0.4/setup.cfg
--rw-r--r--   0 yangqing   (501) staff       (20)     1184 2023-06-29 01:59:11.000000 mkTestCase-0.0.4/setup.py
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 07:31:49.180988 mkTestCase-0.0.5/
+-rw-r--r--   0 yangqing   (501) staff       (20)     1066 2023-03-03 07:16:54.000000 mkTestCase-0.0.5/LICENSE
+-rw-r--r--   0 yangqing   (501) staff       (20)       40 2023-06-28 07:23:33.000000 mkTestCase-0.0.5/MANIFEST.in
+-rw-r--r--   0 yangqing   (501) staff       (20)     2209 2023-06-29 07:31:49.180586 mkTestCase-0.0.5/PKG-INFO
+-rw-r--r--   0 yangqing   (501) staff       (20)     1548 2023-06-05 08:46:44.000000 mkTestCase-0.0.5/README.md
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 07:31:49.176461 mkTestCase-0.0.5/mkTestCase/
+-rw-r--r--   0 yangqing   (501) staff       (20)      141 2023-06-26 06:18:54.000000 mkTestCase-0.0.5/mkTestCase/__init__.py
+-rw-r--r--   0 yangqing   (501) staff       (20)     2931 2023-06-29 07:27:19.000000 mkTestCase-0.0.5/mkTestCase/mkTestCase.py
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 07:31:49.179662 mkTestCase-0.0.5/mkTestCase/testcases/
+-rw-r--r--   0 yangqing   (501) staff       (20)     1155 2023-06-29 01:50:49.000000 mkTestCase-0.0.5/mkTestCase/testcases/form.yml
+-rw-r--r--   0 yangqing   (501) staff       (20)     1034 2023-06-29 01:56:22.000000 mkTestCase-0.0.5/mkTestCase/testcases/page.yml
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-29 07:31:49.178520 mkTestCase-0.0.5/mkTestCase.egg-info/
+-rw-r--r--   0 yangqing   (501) staff       (20)     2209 2023-06-29 07:31:49.000000 mkTestCase-0.0.5/mkTestCase.egg-info/PKG-INFO
+-rw-r--r--   0 yangqing   (501) staff       (20)      315 2023-06-29 07:31:49.000000 mkTestCase-0.0.5/mkTestCase.egg-info/SOURCES.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)        1 2023-06-29 07:31:49.000000 mkTestCase-0.0.5/mkTestCase.egg-info/dependency_links.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)        9 2023-06-29 07:31:49.000000 mkTestCase-0.0.5/mkTestCase.egg-info/requires.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)       11 2023-06-29 07:31:49.000000 mkTestCase-0.0.5/mkTestCase.egg-info/top_level.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)       38 2023-06-29 07:31:49.181122 mkTestCase-0.0.5/setup.cfg
+-rw-r--r--   0 yangqing   (501) staff       (20)     1184 2023-06-29 07:27:42.000000 mkTestCase-0.0.5/setup.py
```

### Comparing `mkTestCase-0.0.4/LICENSE` & `mkTestCase-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkTestCase-0.0.4/PKG-INFO` & `mkTestCase-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkTestCase
-Version: 0.0.4
+Version: 0.0.5
 Summary: Write test cases like building blocks
 Home-page: https://github.com/yongchin0821/mkTestCase
 Author: Yongchin
 Author-email: yongchin39@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yongchin0821/mkTestCase/issues
 Keywords: testcase,automatically generate test cases,automated test
```

### Comparing `mkTestCase-0.0.4/README.md` & `mkTestCase-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mkTestCase-0.0.4/mkTestCase/mkTestCase.py` & `mkTestCase-0.0.5/mkTestCase/mkTestCase.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,17 @@
             if count > self.m_count:
                 self.m_count = count
 
         # 拆解数据
         for data in datas:
             self.mk_row(data)
 
-        return self.rows
+        result = copy.deepcopy(self.rows)
+        self.rows = []
+        return result
 
     def mk_testcase(self, output_path):
         wb = Workbook()
         ws = wb.active
         lowercase = string.ascii_lowercase
         title_prefix = []
         for i in range(self.m_count):
```

### Comparing `mkTestCase-0.0.4/mkTestCase/testcases/form.yml` & `mkTestCase-0.0.5/mkTestCase/testcases/form.yml`

 * *Files identical despite different names*

### Comparing `mkTestCase-0.0.4/mkTestCase/testcases/page.yml` & `mkTestCase-0.0.5/mkTestCase/testcases/page.yml`

 * *Files identical despite different names*

### Comparing `mkTestCase-0.0.4/mkTestCase.egg-info/PKG-INFO` & `mkTestCase-0.0.5/mkTestCase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkTestCase
-Version: 0.0.4
+Version: 0.0.5
 Summary: Write test cases like building blocks
 Home-page: https://github.com/yongchin0821/mkTestCase
 Author: Yongchin
 Author-email: yongchin39@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yongchin0821/mkTestCase/issues
 Keywords: testcase,automatically generate test cases,automated test
```

### Comparing `mkTestCase-0.0.4/setup.py` & `mkTestCase-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mkTestCase",
-    version="0.0.4",
+    version="0.0.5",
     author="Yongchin",
     author_email="yongchin39@qq.com",
     license="MIT",
     description="Write test cases like building blocks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["testcase", "automatically generate test cases", "automated test"],
```

