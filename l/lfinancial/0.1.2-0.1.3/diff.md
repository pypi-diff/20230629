# Comparing `tmp/lfinancial-0.1.2.tar.gz` & `tmp/lfinancial-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.1.2.tar", last modified: Tue Jun 27 12:37:04 2023, max compression
+gzip compressed data, was "lfinancial-0.1.3.tar", last modified: Wed Jun 28 15:32:41 2023, max compression
```

## Comparing `lfinancial-0.1.2.tar` & `lfinancial-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 12:36:43.000000 lfinancial-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-27 12:37:04.785813 lfinancial-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-27 12:36:43.000000 lfinancial-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 12:36:43.000000 lfinancial-0.1.2/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-27 12:36:43.000000 lfinancial-0.1.2/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-27 12:36:43.000000 lfinancial-0.1.2/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 12:37:04.000000 lfinancial-0.1.2/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:37:04.785813 lfinancial-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-27 12:36:43.000000 lfinancial-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:37:04.785813 lfinancial-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 12:36:43.000000 lfinancial-0.1.2/tests/test_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:32:41.331862 lfinancial-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-28 15:32:21.000000 lfinancial-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-28 15:32:41.331862 lfinancial-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-28 15:32:21.000000 lfinancial-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:32:41.331862 lfinancial-0.1.3/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 15:32:21.000000 lfinancial-0.1.3/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-28 15:32:21.000000 lfinancial-0.1.3/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-28 15:32:21.000000 lfinancial-0.1.3/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:32:41.331862 lfinancial-0.1.3/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-28 15:32:41.000000 lfinancial-0.1.3/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-28 15:32:41.000000 lfinancial-0.1.3/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:32:41.000000 lfinancial-0.1.3/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 15:32:41.000000 lfinancial-0.1.3/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:32:41.331862 lfinancial-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-28 15:32:21.000000 lfinancial-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:32:41.331862 lfinancial-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-28 15:32:21.000000 lfinancial-0.1.3/tests/test_document.py
```

### Comparing `lfinancial-0.1.2/LICENSE.txt` & `lfinancial-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.1.2/PKG-INFO` & `lfinancial-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -60,8 +60,14 @@
 # Baviv
 
 f.last_name()
 # Hucacuqa
 
 f.kana_name()
 # ハジ
+
+f.cellphone()
+# 13851695115
+
+f.area_code()
+# +86
 ```
```

### Comparing `lfinancial-0.1.2/README.md` & `lfinancial-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -48,8 +48,14 @@
 # Baviv
 
 f.last_name()
 # Hucacuqa
 
 f.kana_name()
 # ハジ
+
+f.cellphone()
+# 13851695115
+
+f.area_code()
+# +86
 ```
```

### Comparing `lfinancial-0.1.2/lfinancial/factory.py` & `lfinancial-0.1.3/lfinancial/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from lfinancial.generators.document_type import IDCodeGenerator
+from lfinancial.generators.document import IDCodeGenerator
 from lfinancial.generators.name import NameGenerator
+from lfinancial.generators.phone import PhoneGenerator
 
 
 class GeneratorFactory:
     def __init__(self):
         self.generators = {
             "SSN": IDCodeGenerator(),
             "IDCard": IDCodeGenerator(),
             "Passport": IDCodeGenerator(),
             "NRIC": IDCodeGenerator(),
             "MyNumber": IDCodeGenerator(),
             "first_name": NameGenerator(),
             "middle_name": NameGenerator(),
             "last_name": NameGenerator(),
             "cn_name": NameGenerator(),
-            "kana_name": NameGenerator()
+            "kana_name": NameGenerator(),
+            "cellphone": PhoneGenerator(),
+            "area_code": PhoneGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.1.2/lfinancial/financial.py` & `lfinancial-0.1.3/lfinancial/financial.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,20 +35,28 @@
 
     def cn_name(self, country=None):
         return self._generate("cn_name", country)
 
     def kana_name(self, country=None):
         return self._generate("kana_name", country)
 
+    def cellphone(self, country=None):
+        return self._generate("cellphone", country)
+
+    def area_code(self, country=None):
+        return self._generate("area_code", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
     print(f.my_number())
     print(f.first_name())
     print(f.middle_name())
     print(f.last_name())
     print(f.kana_name())
     print(f.cn_name())
+    print(f.cellphone())
+    print(f.area_code())
```

### Comparing `lfinancial-0.1.2/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.1.3/lfinancial.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -60,8 +60,14 @@
 # Baviv
 
 f.last_name()
 # Hucacuqa
 
 f.kana_name()
 # ハジ
+
+f.cellphone()
+# 13851695115
+
+f.area_code()
+# +86
 ```
```

### Comparing `lfinancial-0.1.2/setup.py` & `lfinancial-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='lfinancial',
-    version='0.1.2',
+    version='0.1.3',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=['lfinancial'],
```

