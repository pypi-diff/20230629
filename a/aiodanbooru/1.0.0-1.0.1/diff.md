# Comparing `tmp/aiodanbooru-1.0.0.tar.gz` & `tmp/aiodanbooru-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.0.tar", last modified: Thu Jun 29 11:10:19 2023, max compression
+gzip compressed data, was "aiodanbooru-1.0.1.tar", last modified: Thu Jun 29 11:18:21 2023, max compression
```

## Comparing `aiodanbooru-1.0.0.tar` & `aiodanbooru-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 11:10:19.007569 aiodanbooru-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      822 2023-06-29 11:10:19.007569 aiodanbooru-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2011 2023-06-29 10:56:09.000000 aiodanbooru-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 11:10:18.992544 aiodanbooru-1.0.0/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.0/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-06-29 10:39:15.000000 aiodanbooru-1.0.0/aiodanbooru/api.py
--rw-rw-rw-   0        0        0     1916 2023-06-29 10:09:01.000000 aiodanbooru-1.0.0/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:10:19.005058 aiodanbooru-1.0.0/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0      822 2023-06-29 11:10:18.000000 aiodanbooru-1.0.0/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-29 11:10:18.000000 aiodanbooru-1.0.0/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 11:10:18.000000 aiodanbooru-1.0.0/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 11:10:18.000000 aiodanbooru-1.0.0/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 11:10:18.000000 aiodanbooru-1.0.0/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 11:10:19.007569 aiodanbooru-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-29 10:58:45.000000 aiodanbooru-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:10:19.006563 aiodanbooru-1.0.0/tests/
--rw-rw-rw-   0        0        0     1466 2023-06-29 10:45:36.000000 aiodanbooru-1.0.0/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.944836 aiodanbooru-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-06-29 11:18:21.943832 aiodanbooru-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.916307 aiodanbooru-1.0.1/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.1/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1523 2023-06-29 10:39:15.000000 aiodanbooru-1.0.1/aiodanbooru/api.py
+-rw-rw-rw-   0        0        0     1916 2023-06-29 10:09:01.000000 aiodanbooru-1.0.1/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.941313 aiodanbooru-1.0.1/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 11:18:21.000000 aiodanbooru-1.0.1/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 11:18:21.944836 aiodanbooru-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-06-29 11:14:00.000000 aiodanbooru-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:18:21.941313 aiodanbooru-1.0.1/tests/
+-rw-rw-rw-   0        0        0     1466 2023-06-29 10:45:36.000000 aiodanbooru-1.0.1/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.0/LICENSE` & `aiodanbooru-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.0/README.md` & `aiodanbooru-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Danbooru
 
 [![PyPI](https://img.shields.io/pypi/v/aiodanbooru.svg)](https://pypi.org/project/aiodanbooru/)
-[![License](https://img.shields.io/pypi/l/aiodanbooru.svg)](https://https://github.com/lrdcxdes/aiodanbooru/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/aiodanbooru.svg)](https://github.com/lrdcxdes/aiodanbooru/blob/main/LICENSE)
 
 Danbooru is a Python library that provides an easy-to-use interface for interacting with the Danbooru API. It allows you to search for posts, retrieve post details, and download media files from the Danbooru image board.
 
 ## Features
 
 - Simple and intuitive API for interacting with the Danbooru API
 - Retrieve posts based on tags and limit
@@ -42,14 +42,14 @@
 if __name__ == "__main__":
     import asyncio
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
-For more details and advanced usage examples, please refer to the [**documentation**](https://aiodanbooru.readthedocs.io/en/latest/).
+For more details and advanced usage examples, please refer to the **[documentation](https://aiodanbooru.readthedocs.io/en/latest/)**.
 
 ## Contributing
-Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue on the [**GitHub repository**](https://github.com/lrdcxdes/danbooru). Feel free to submit pull requests with improvements or fixes.
+Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue on the **[GitHub repository](https://github.com/lrdcxdes/danbooru)**. Feel free to submit pull requests with improvements or fixes.
 
 ## License
-This project is licensed under the MIT License. See the [**LICENSE**](https://github.com/lrdcxdes/aiodanbooru/blob/main/LICENSE) file for more information.
+This project is licensed under the MIT License. See the **[LICENSE](https://github.com/lrdcxdes/aiodanbooru/blob/main/LICENSE)** file for more information.
```

### Comparing `aiodanbooru-1.0.0/aiodanbooru/api.py` & `aiodanbooru-1.0.1/aiodanbooru/api.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.0/aiodanbooru/models.py` & `aiodanbooru-1.0.1/aiodanbooru/models.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.0/setup.py` & `aiodanbooru-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.0",
+    version="1.0.1",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic",
@@ -24,8 +24,9 @@
     ],
     python_requires=">=3.7",
     project_urls={
         "Source": "https://github.com/lrdcxdes/aiodanbooru",
         "Bug Reports": "https://github.com/lrdcxdes/aiodanbooru/issues",
     },
     long_description=open("LONG.rst").read(),
+    license="MIT",
 )
```

### Comparing `aiodanbooru-1.0.0/tests/test_api.py` & `aiodanbooru-1.0.1/tests/test_api.py`

 * *Files identical despite different names*

