# Comparing `tmp/enigmacrypt-0.0.1.tar.gz` & `tmp/enigmacrypt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmacrypt-0.0.1.tar", last modified: Thu Jun 29 20:09:20 2023, max compression
+gzip compressed data, was "enigmacrypt-0.0.2.tar", last modified: Thu Jun 29 20:42:26 2023, max compression
```

## Comparing `enigmacrypt-0.0.1.tar` & `enigmacrypt-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:09:20.471399 enigmacrypt-0.0.1/
--rw-rw-rw-   0        0        0     2398 2023-06-29 20:09:20.470402 enigmacrypt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2023-06-29 19:23:43.000000 enigmacrypt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:09:20.460831 enigmacrypt-0.0.1/app/
--rw-rw-rw-   0        0        0        0 2023-06-29 19:51:33.000000 enigmacrypt-0.0.1/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:09:20.461828 enigmacrypt-0.0.1/app/enigmacrypt/
--rw-rw-rw-   0        0        0       82 2023-06-29 20:06:55.000000 enigmacrypt-0.0.1/app/enigmacrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:09:20.469405 enigmacrypt-0.0.1/enigmacrypt.egg-info/
--rw-rw-rw-   0        0        0     2398 2023-06-29 20:09:20.000000 enigmacrypt-0.0.1/enigmacrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-29 20:09:20.000000 enigmacrypt-0.0.1/enigmacrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:09:20.000000 enigmacrypt-0.0.1/enigmacrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 20:09:20.000000 enigmacrypt-0.0.1/enigmacrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 20:09:20.000000 enigmacrypt-0.0.1/enigmacrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 20:09:20.471399 enigmacrypt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-06-29 19:57:14.000000 enigmacrypt-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.867506 enigmacrypt-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:14.000000 enigmacrypt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2510 2023-06-29 20:42:26.865508 enigmacrypt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:14.000000 enigmacrypt-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.851163 enigmacrypt-0.0.2/app/
+-rw-rw-rw-   0        0        0        0 2023-06-29 19:51:33.000000 enigmacrypt-0.0.2/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.852164 enigmacrypt-0.0.2/app/enigmacrypt/
+-rw-rw-rw-   0        0        0       82 2023-06-29 20:06:55.000000 enigmacrypt-0.0.2/app/enigmacrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.860445 enigmacrypt-0.0.2/enigmacrypt.egg-info/
+-rw-rw-rw-   0        0        0     2510 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:42:26.868503 enigmacrypt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-06-29 20:42:01.000000 enigmacrypt-0.0.2/setup.py
```

### Comparing `enigmacrypt-0.0.1/PKG-INFO` & `enigmacrypt-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
 Classifier: Development Status :: 1 - Planning
@@ -12,37 +12,41 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.07
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 # EnigmaCrypt
 EnigmaCrypt is a Python package that provides a simple and secure way to encrypt and decrypt strings. It uses a unique encryption algorithm and generates a key that can be used to decode the encrypted string.
 
 ## Installation
 To install EnigmaCrypt, you can use pip:
 
 ```pip install enigmacrypt```
 
 ## Usage
 Here's a simple example of how to use EnigmaCrypt to encrypt and decrypt a string:
 
 ```python
-from enigmacrypt import EnigmaCrypt
+from enigmacrypt import Encryption, Decryption
 
-# Create an instance of EnigmaCrypt
-crypt = EnigmaCrypt()
+# Create an instance of Encryption
+encryption = Encryption()
 
 # Encrypt a string
-encrypted_string, key = crypt.encrypt("Hello, World!")
+encrypted_string, key = encryption.encrypt("Hello, World!")
+
+# Create an instance of Decryption
+decryption = Decryption()
 
 # Decrypt the string using the generated key
-decrypted_string = crypt.decrypt(encrypted_string, key)
+decrypted_string = decryption.decrypt(encrypted_string, key)
 
 print(decrypted_string)  # Output: Hello, World!
 ```
 
 ## Contributing
 Contributions are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the GitHub repository. If you'd like to contribute code, you can fork the repository and create a pull request with your changes.
```

### Comparing `enigmacrypt-0.0.1/README.md` & `enigmacrypt-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 ```pip install enigmacrypt```
 
 ## Usage
 Here's a simple example of how to use EnigmaCrypt to encrypt and decrypt a string:
 
 ```python
-from enigmacrypt import EnigmaCrypt
+from enigmacrypt import Encryption, Decryption
 
-# Create an instance of EnigmaCrypt
-crypt = EnigmaCrypt()
+# Create an instance of Encryption
+encryption = Encryption()
 
 # Encrypt a string
-encrypted_string, key = crypt.encrypt("Hello, World!")
+encrypted_string, key = encryption.encrypt("Hello, World!")
+
+# Create an instance of Decryption
+decryption = Decryption()
 
 # Decrypt the string using the generated key
-decrypted_string = crypt.decrypt(encrypted_string, key)
+decrypted_string = decryption.decrypt(encrypted_string, key)
 
 print(decrypted_string)  # Output: Hello, World!
 ```
 
 ## Contributing
 Contributions are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the GitHub repository. If you'd like to contribute code, you can fork the repository and create a pull request with your changes.
```

### Comparing `enigmacrypt-0.0.1/enigmacrypt.egg-info/PKG-INFO` & `enigmacrypt-0.0.2/enigmacrypt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
 Classifier: Development Status :: 1 - Planning
@@ -12,37 +12,41 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.07
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 # EnigmaCrypt
 EnigmaCrypt is a Python package that provides a simple and secure way to encrypt and decrypt strings. It uses a unique encryption algorithm and generates a key that can be used to decode the encrypted string.
 
 ## Installation
 To install EnigmaCrypt, you can use pip:
 
 ```pip install enigmacrypt```
 
 ## Usage
 Here's a simple example of how to use EnigmaCrypt to encrypt and decrypt a string:
 
 ```python
-from enigmacrypt import EnigmaCrypt
+from enigmacrypt import Encryption, Decryption
 
-# Create an instance of EnigmaCrypt
-crypt = EnigmaCrypt()
+# Create an instance of Encryption
+encryption = Encryption()
 
 # Encrypt a string
-encrypted_string, key = crypt.encrypt("Hello, World!")
+encrypted_string, key = encryption.encrypt("Hello, World!")
+
+# Create an instance of Decryption
+decryption = Decryption()
 
 # Decrypt the string using the generated key
-decrypted_string = crypt.decrypt(encrypted_string, key)
+decrypted_string = decryption.decrypt(encrypted_string, key)
 
 print(decrypted_string)  # Output: Hello, World!
 ```
 
 ## Contributing
 Contributions are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the GitHub repository. If you'd like to contribute code, you can fork the repository and create a pull request with your changes.
```

### Comparing `enigmacrypt-0.0.1/setup.py` & `enigmacrypt-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Encoding and decoding strings using keys'
 
 # Setting up
 setup(
     name="enigmacrypt",
     version=VERSION,
     author="WooksCode (Wojciech Karwowski)",
```

