# Comparing `tmp/cipher_kit-0.0.3.tar.gz` & `tmp/cipher_kit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipher_kit-0.0.3.tar", last modified: Wed Jun 21 07:56:49 2023, max compression
+gzip compressed data, was "cipher_kit-0.0.4.tar", last modified: Thu Jun 29 10:17:42 2023, max compression
```

## Comparing `cipher_kit-0.0.3.tar` & `cipher_kit-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.076026 cipher_kit-0.0.3/
--rw-rw-rw-   0        0        0     1082 2023-06-20 06:27:52.000000 cipher_kit-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1772 2023-06-21 07:56:49.074018 cipher_kit-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.048018 cipher_kit-0.0.3/app/
-drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.055020 cipher_kit-0.0.3/app/cipher_kit/
--rw-rw-rw-   0        0        0       34 2023-06-20 05:32:57.000000 cipher_kit-0.0.3/app/cipher_kit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.066027 cipher_kit-0.0.3/app/cipher_kit/src/
--rw-rw-rw-   0        0        0        0 2023-06-19 17:14:24.000000 cipher_kit-0.0.3/app/cipher_kit/src/__init__.py
--rw-rw-rw-   0        0        0     2475 2023-06-20 07:03:22.000000 cipher_kit-0.0.3/app/cipher_kit/src/cipher.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.071020 cipher_kit-0.0.3/app/cipher_kit/tests/
--rw-rw-rw-   0        0        0        0 2023-06-20 05:48:41.000000 cipher_kit-0.0.3/app/cipher_kit/tests/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-06-20 07:16:55.000000 cipher_kit-0.0.3/app/cipher_kit/tests/test_cipher.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:56:49.063022 cipher_kit-0.0.3/app/cipher_kit.egg-info/
--rw-rw-rw-   0        0        0     1772 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 07:56:48.000000 cipher_kit-0.0.3/app/cipher_kit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 07:56:49.076026 cipher_kit-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-06-21 07:45:14.000000 cipher_kit-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:17:42.937922 cipher_kit-0.0.4/
+-rw-rw-rw-   0        0        0     1082 2023-06-20 06:27:52.000000 cipher_kit-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1772 2023-06-29 10:17:42.935923 cipher_kit-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 10:17:42.917921 cipher_kit-0.0.4/app/
+drwxrwxrwx   0        0        0        0 2023-06-29 10:17:42.922924 cipher_kit-0.0.4/app/cipher_kit/
+-rw-rw-rw-   0        0        0       34 2023-06-20 05:32:57.000000 cipher_kit-0.0.4/app/cipher_kit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:17:42.931932 cipher_kit-0.0.4/app/cipher_kit/src/
+-rw-rw-rw-   0        0        0        0 2023-06-19 17:14:24.000000 cipher_kit-0.0.4/app/cipher_kit/src/__init__.py
+-rw-rw-rw-   0        0        0     2749 2023-06-29 10:09:54.000000 cipher_kit-0.0.4/app/cipher_kit/src/cipher.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:17:42.933925 cipher_kit-0.0.4/app/cipher_kit/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-20 05:48:41.000000 cipher_kit-0.0.4/app/cipher_kit/tests/__init__.py
+-rw-rw-rw-   0        0        0     3062 2023-06-29 10:09:54.000000 cipher_kit-0.0.4/app/cipher_kit/tests/test_cipher.py
+drwxrwxrwx   0        0        0        0 2023-06-29 10:17:42.928924 cipher_kit-0.0.4/app/cipher_kit.egg-info/
+-rw-rw-rw-   0        0        0     1772 2023-06-29 10:17:42.000000 cipher_kit-0.0.4/app/cipher_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-29 10:17:42.000000 cipher_kit-0.0.4/app/cipher_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 10:17:42.000000 cipher_kit-0.0.4/app/cipher_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 10:17:42.000000 cipher_kit-0.0.4/app/cipher_kit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 10:17:42.937922 cipher_kit-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-06-29 10:09:54.000000 cipher_kit-0.0.4/setup.py
```

### Comparing `cipher_kit-0.0.3/LICENSE.txt` & `cipher_kit-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cipher_kit-0.0.3/PKG-INFO` & `cipher_kit-0.0.4/app/cipher_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cipher_kit
-Version: 0.0.3
+Name: cipher-kit
+Version: 0.0.4
 Summary: Module which helps in encryption and decryption
 Home-page: https://github.com/PankajVishw50/cipher_kit
 Author: Pankaj
 Author-email: pankaj.vishw.dev@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cipher_kit-0.0.3/app/cipher_kit/src/cipher.py` & `cipher_kit-0.0.4/app/cipher_kit/src/cipher.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,20 @@
         index = 0
         length = len(key_list)
         new_data = str()
 
         text_list = [text[x:x + 2] for x in range(0, len(text), 2)]
 
         for letter in text_list:
+            if len(letter) != 2:
+                # This block will only be true when have text which is not encrypted by Cipher.encrypt or
+                # text is corrupted
+                # In either case method should not raise any error
+                continue
+
             value = ord(letter[0])
             remainder = ord(letter[1])
 
             value = (value * 2) + remainder
             value //= key_list[index]
 
             new_data += chr(value)
```

### Comparing `cipher_kit-0.0.3/app/cipher_kit/tests/test_cipher.py` & `cipher_kit-0.0.4/app/cipher_kit/tests/test_cipher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import json
 
 from .. import Cipher
 
 
 class TestCipher:
 
-    def test_one(self):
+    def test_basic(self):
         data = "My name is Subhash and i work on great projects"
         key = "9d3f90jfi39320820932jkj302932290i0jiofjijfw0932iifjeojf3"
 
         encrypted_data = Cipher.encrypt(data, key)
 
         assert encrypted_data != data
 
         decrypted_data = Cipher.decrypt(encrypted_data, key)
 
         assert decrypted_data == data
 
-    def in_development_test_two(self):
+    def unfixed_key_value_0(self):
+        """
+        Will generate error due to key being 0
+        Will fix in the future.
+        """
+
         data = """
         Once upon a time, in a small village, a curious cat named Whiskers embarked on a quest to find 
         the legendary Golden Fish. Along the way, Whiskers encountered talking trees, mischievous squirrels, 
         and a wise old owl. With courage and determination, 
         Whiskers discovered that the real treasure was the journey itself.
         """
+
         key = "\x00"
 
         encrypted_data = Cipher.encrypt(data, key)
 
         assert encrypted_data != data
 
         decrypted_data = Cipher.decrypt(encrypted_data, key)
 
         assert decrypted_data == data
 
-    def test_three(self):
+    def test_json_data(self):
         """ Testing if it can encrypt and decrypt json """
         data = {
             "name": "Neha",
             "age": 23,
             "bachelor": True,
             "height": 5.4
         }
@@ -56,26 +62,43 @@
 
         assert decrypted_json == json_data
 
         obj_data = json.loads(decrypted_json)
 
         assert data == obj_data
 
-    def in_development_test_four(self):
+    def test_various_keys(self):
         data = "Who knows what can happen"
         key = "#StrongPassword_1000x"
 
         encrypted_data = Cipher.encrypt(data, key)
 
         assert encrypted_data != data
 
-        decrypted_data_with_wrong_key = Cipher.decrypt(data, "#StrongPassword_999x")
+        decrypted_data_with_wrong_key = Cipher.decrypt(encrypted_data, "#StrongPassword_999x")
 
         assert decrypted_data_with_wrong_key != data
 
-        decrypted_data_with_different_case_letter = Cipher.decrypt(data, "#strongPassword_1000x")
+        decrypted_data_with_different_case_letter = Cipher.decrypt(encrypted_data, "#strongPassword_1000x")
 
         assert decrypted_data_with_different_case_letter != data
 
-        decrypted_data = Cipher.decrypt(data, key)
+        decrypted_data = Cipher.decrypt(encrypted_data, key)
+
+        assert decrypted_data == data
+
+    def test_unencrypted_data(self):
+        """
+        In this test we are providing non encrypted data to see how
+        our module handles it.
+        """
+        data = "Who knows what can happen"
+        key = "Very strong key"
+
+        encrypted_data = Cipher.encrypt(data, key)
+        assert encrypted_data != data
 
+        decrypted_data_with_non_encrypted_data = Cipher.decrypt(data, key)
+        assert decrypted_data_with_non_encrypted_data != data
+
+        decrypted_data = Cipher.decrypt(encrypted_data, key)
         assert decrypted_data == data
```

### Comparing `cipher_kit-0.0.3/app/cipher_kit.egg-info/PKG-INFO` & `cipher_kit-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cipher-kit
-Version: 0.0.3
+Name: cipher_kit
+Version: 0.0.4
 Summary: Module which helps in encryption and decryption
 Home-page: https://github.com/PankajVishw50/cipher_kit
 Author: Pankaj
 Author-email: pankaj.vishw.dev@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cipher_kit-0.0.3/setup.py` & `cipher_kit-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("app/Readme.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="cipher_kit",
-    version="0.0.3",
+    version="0.0.4",
     description="Module which helps in encryption and decryption",
     author="Pankaj",
     author_email="pankaj.vishw.dev@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PankajVishw50/cipher_kit",
     packages=find_packages("app"),
     package_dir={"": "app"},
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 ",
-        "License :: OSI Approved :: MIT License"
+         "License :: OSI Approved :: MIT License"
 
     ],
     extra_requires={
         "dev": [
             "pytest>=7.0.0",
         ]
     }
```

