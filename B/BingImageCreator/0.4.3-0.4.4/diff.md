# Comparing `tmp/BingImageCreator-0.4.3.tar.gz` & `tmp/BingImageCreator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.4.3.tar", last modified: Wed Jun 28 06:09:42 2023, max compression
+gzip compressed data, was "BingImageCreator-0.4.4.tar", last modified: Thu Jun 29 17:00:53 2023, max compression
```

## Comparing `BingImageCreator-0.4.3.tar` & `BingImageCreator-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:09:42.813960 BingImageCreator-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-28 06:09:21.000000 BingImageCreator-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-28 06:09:42.813960 BingImageCreator-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-28 06:09:21.000000 BingImageCreator-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-28 06:09:42.813960 BingImageCreator-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-28 06:09:21.000000 BingImageCreator-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:09:42.813960 BingImageCreator-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:09:42.813960 BingImageCreator-0.4.3/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-28 06:09:42.000000 BingImageCreator-0.4.3/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-28 06:09:42.000000 BingImageCreator-0.4.3/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 06:09:42.000000 BingImageCreator-0.4.3/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 06:09:42.000000 BingImageCreator-0.4.3/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 06:09:42.000000 BingImageCreator-0.4.3/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-06-28 06:09:21.000000 BingImageCreator-0.4.3/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:09:42.813960 BingImageCreator-0.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-28 06:09:21.000000 BingImageCreator-0.4.3/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:53.196152 BingImageCreator-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-29 17:00:31.000000 BingImageCreator-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-29 17:00:53.196152 BingImageCreator-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-29 17:00:31.000000 BingImageCreator-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 17:00:53.196152 BingImageCreator-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-29 17:00:31.000000 BingImageCreator-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:53.192152 BingImageCreator-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:53.196152 BingImageCreator-0.4.4/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-29 17:00:53.000000 BingImageCreator-0.4.4/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 17:00:53.000000 BingImageCreator-0.4.4/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:00:53.000000 BingImageCreator-0.4.4/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 17:00:53.000000 BingImageCreator-0.4.4/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 17:00:53.000000 BingImageCreator-0.4.4/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-29 17:00:31.000000 BingImageCreator-0.4.4/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:00:53.196152 BingImageCreator-0.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 17:00:31.000000 BingImageCreator-0.4.4/test/test_example.py
```

### Comparing `BingImageCreator-0.4.3/LICENSE` & `BingImageCreator-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.4.3/PKG-INFO` & `BingImageCreator-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.4.3
+Version: 0.4.4
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.4.3/README.md` & `BingImageCreator-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.4.3/setup.py` & `BingImageCreator-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.4.3",
+    version="0.4.4",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.4.3/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.4.4/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.4.3
+Version: 0.4.4
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.4.3/src/BingImageCreator.py` & `BingImageCreator-0.4.4/src/BingImageCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,21 @@
             if img in bad_images:
                 raise Exception("Bad images")
         # No images
         if not normal_image_links:
             raise Exception(error_no_images)
         return normal_image_links
 
-    def save_images(self, links: list, download_count: int, output_dir: str, file_name: str = None) -> None:
+    def save_images(
+        self,
+        links: list,
+        output_dir: str,
+        file_name: str = None,
+        download_count: int = None,
+    ) -> None:
         """
         Saves images to output directory
         Parameters:
             links: list[str]
             output_dir: str
             file_name: str
             download_count: int
@@ -198,22 +204,29 @@
             print(download_message)
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         try:
             fn = f"{file_name}_" if file_name else ""
             jpeg_index = 0
 
-            for link in links[:download_count]:
-                while os.path.exists(os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")):
+            if download_count:
+                links = links[:download_count]
+
+            for link in links:
+                while os.path.exists(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")
+                ):
                     jpeg_index += 1
                 response = self.session.get(link)
                 if response.status_code != 200:
                     raise Exception("Could not download image")
                 # save response to file
-                with open(os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb") as output_file:
+                with open(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb"
+                ) as output_file:
                     output_file.write(response.content)
                 jpeg_index += 1
 
         except requests.exceptions.MissingSchema as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt.",
             ) from url_exception
@@ -354,21 +367,25 @@
         with contextlib.suppress(FileExistsError):
             os.mkdir(output_dir)
         try:
             fn = f"{file_name}_" if file_name else ""
             jpeg_index = 0
 
             for link in links[:download_count]:
-                while os.path.exists(os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")):
+                while os.path.exists(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")
+                ):
                     jpeg_index += 1
                 response = await self.session.get(link)
                 if response.status_code != 200:
                     raise Exception("Could not download image")
                 # save response to file
-                with open(os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb") as output_file:
+                with open(
+                    os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb"
+                ) as output_file:
                     output_file.write(response.content)
                 jpeg_index += 1
         except httpx.InvalidURL as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt.",
             ) from url_exception
 
@@ -385,15 +402,17 @@
     async with ImageGenAsync(
         u_cookie,
         debug_file=debug_file,
         quiet=quiet,
         all_cookies=all_cookies,
     ) as image_generator:
         images = await image_generator.get_images(prompt)
-        await image_generator.save_images(images, output_dir=output_dir, download_count=download_count)
+        await image_generator.save_images(
+            images, output_dir=output_dir, download_count=download_count
+        )
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-U", help="Auth cookie from browser", type=str)
     parser.add_argument("--cookie-file", help="File containing auth cookie", type=str)
     parser.add_argument(
@@ -410,15 +429,15 @@
         default="./output",
     )
 
     parser.add_argument(
         "--download-count",
         help="Number of images to download, value must be less than five",
         type=int,
-        default=4
+        default=4,
     )
 
     parser.add_argument(
         "--debug-file",
         help="Path to the file where debug information will be written.",
         type=str,
     )
```

### Comparing `BingImageCreator-0.4.3/test/test_example.py` & `BingImageCreator-0.4.4/test/test_example.py`

 * *Files identical despite different names*

