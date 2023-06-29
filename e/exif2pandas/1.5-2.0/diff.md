# Comparing `tmp/exif2pandas-1.5.tar.gz` & `tmp/exif2pandas-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exif2pandas-1.5.tar", last modified: Fri Feb 17 15:58:20 2023, max compression
+gzip compressed data, was "exif2pandas-2.0.tar", last modified: Thu Jun 29 20:48:41 2023, max compression
```

## Comparing `exif2pandas-1.5.tar` & `exif2pandas-2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-02-17 15:58:20.283398 exif2pandas-1.5/
--rw-r--r--   0 visgean    (501) staff       (20)     1064 2022-01-28 03:49:28.000000 exif2pandas-1.5/LICENSE
--rw-r--r--   0 visgean    (501) staff       (20)       34 2022-01-28 03:49:28.000000 exif2pandas-1.5/MANIFEST.in
--rw-r--r--   0 visgean    (501) staff       (20)     6817 2023-02-17 15:58:20.283252 exif2pandas-1.5/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)     5277 2022-01-28 03:49:28.000000 exif2pandas-1.5/README.md
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-02-17 15:58:20.282201 exif2pandas-1.5/exif2pandas/
--rw-r--r--   0 visgean    (501) staff       (20)        0 2022-01-28 03:49:28.000000 exif2pandas-1.5/exif2pandas/__init__.py
--rw-r--r--   0 visgean    (501) staff       (20)     1860 2022-01-28 03:58:49.000000 exif2pandas-1.5/exif2pandas/clean.py
--rw-r--r--   0 visgean    (501) staff       (20)     1429 2022-01-28 03:55:34.000000 exif2pandas-1.5/exif2pandas/gps_utils.py
--rwxr-xr-x   0 visgean    (501) staff       (20)     2370 2022-02-13 12:06:04.000000 exif2pandas-1.5/exif2pandas/main.py
--rw-r--r--   0 visgean    (501) staff       (20)     1768 2022-02-13 12:19:27.000000 exif2pandas-1.5/exif2pandas/utils.py
-drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-02-17 15:58:20.283005 exif2pandas-1.5/exif2pandas.egg-info/
--rw-r--r--   0 visgean    (501) staff       (20)     6817 2023-02-17 15:58:20.000000 exif2pandas-1.5/exif2pandas.egg-info/PKG-INFO
--rw-r--r--   0 visgean    (501) staff       (20)      361 2023-02-17 15:58:20.000000 exif2pandas-1.5/exif2pandas.egg-info/SOURCES.txt
--rw-r--r--   0 visgean    (501) staff       (20)        1 2023-02-17 15:58:20.000000 exif2pandas-1.5/exif2pandas.egg-info/dependency_links.txt
--rw-r--r--   0 visgean    (501) staff       (20)       55 2023-02-17 15:58:20.000000 exif2pandas-1.5/exif2pandas.egg-info/entry_points.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-02-17 15:58:20.000000 exif2pandas-1.5/exif2pandas.egg-info/requires.txt
--rw-r--r--   0 visgean    (501) staff       (20)       12 2023-02-17 15:58:20.000000 exif2pandas-1.5/exif2pandas.egg-info/top_level.txt
--rw-r--r--   0 visgean    (501) staff       (20)       38 2023-02-17 15:58:20.283441 exif2pandas-1.5/setup.cfg
--rw-r--r--   0 visgean    (501) staff       (20)     1057 2023-02-17 15:50:54.000000 exif2pandas-1.5/setup.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-29 20:48:41.863151 exif2pandas-2.0/
+-rw-r--r--   0 visgean    (501) staff       (20)     1064 2022-01-28 03:49:28.000000 exif2pandas-2.0/LICENSE
+-rw-r--r--   0 visgean    (501) staff       (20)       34 2022-01-28 03:49:28.000000 exif2pandas-2.0/MANIFEST.in
+-rw-r--r--   0 visgean    (501) staff       (20)     7280 2023-06-29 20:48:41.863022 exif2pandas-2.0/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)     5580 2023-06-29 20:34:34.000000 exif2pandas-2.0/README.md
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-29 20:48:41.862121 exif2pandas-2.0/exif2pandas/
+-rw-r--r--   0 visgean    (501) staff       (20)        0 2022-01-28 03:49:28.000000 exif2pandas-2.0/exif2pandas/__init__.py
+-rw-r--r--   0 visgean    (501) staff       (20)     2037 2023-06-29 20:42:14.000000 exif2pandas-2.0/exif2pandas/clean.py
+-rw-r--r--   0 visgean    (501) staff       (20)     2221 2023-06-29 20:44:01.000000 exif2pandas-2.0/exif2pandas/extract.py
+-rw-r--r--   0 visgean    (501) staff       (20)     1398 2023-06-29 20:37:48.000000 exif2pandas-2.0/exif2pandas/gps_utils.py
+-rwxr-xr-x   0 visgean    (501) staff       (20)     1655 2023-06-29 20:42:14.000000 exif2pandas-2.0/exif2pandas/main.py
+-rw-r--r--   0 visgean    (501) staff       (20)     1771 2023-06-29 20:42:13.000000 exif2pandas-2.0/exif2pandas/utils.py
+drwxr-xr-x   0 visgean    (501) staff       (20)        0 2023-06-29 20:48:41.862834 exif2pandas-2.0/exif2pandas.egg-info/
+-rw-r--r--   0 visgean    (501) staff       (20)     7280 2023-06-29 20:48:41.000000 exif2pandas-2.0/exif2pandas.egg-info/PKG-INFO
+-rw-r--r--   0 visgean    (501) staff       (20)      384 2023-06-29 20:48:41.000000 exif2pandas-2.0/exif2pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 visgean    (501) staff       (20)        1 2023-06-29 20:48:41.000000 exif2pandas-2.0/exif2pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       55 2023-06-29 20:48:41.000000 exif2pandas-2.0/exif2pandas.egg-info/entry_points.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-29 20:48:41.000000 exif2pandas-2.0/exif2pandas.egg-info/requires.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       12 2023-06-29 20:48:41.000000 exif2pandas-2.0/exif2pandas.egg-info/top_level.txt
+-rw-r--r--   0 visgean    (501) staff       (20)       38 2023-06-29 20:48:41.863194 exif2pandas-2.0/setup.cfg
+-rw-r--r--   0 visgean    (501) staff       (20)     1020 2023-06-29 20:47:06.000000 exif2pandas-2.0/setup.py
```

### Comparing `exif2pandas-1.5/LICENSE` & `exif2pandas-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exif2pandas-1.5/PKG-INFO` & `exif2pandas-2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exif2pandas
-Version: 1.5
+Version: 2.0
 Summary: Extract EXIF to pandas / SQL / Excel / Feather
 Home-page: https://github.com/visgean/exif2pandas
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Extract EXIF to pandas / SQL / Excel / Feather
         
@@ -22,24 +22,44 @@
         
         and anything else that [Pandas supports](https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html).
         
         
         ## Installation
         
         ```
-            $ pip install exif2pandas --user
+            $ pip3 install exif2pandas --user
         ```
         
         To export the dataframe you will need one of these modules:
         
-         - SQLite: ``pip install --user SQLAlchemy`` 
-         - Feather: ``pip install --user pyarrow`` 
-         - Excel: ``pip install --user xlsxwriter``
+         - SQLite: ``pip3 install --user SQLAlchemy`` 
+         - Feather: ``pip3 install --user pyarrow`` 
+         - Excel: ``pip3 install --user xlsxwriter``
+        
+        # Python module usage:
+        
+        ```python
+        from exif2pandas import extract
+        from pathlib import Path
+        
+        
+        df = extract.extract_feather(
+            feather_path=Path('photos.feather').resolve(),
+            pictures_root=[
+                Path('/Users/visgean/Dropbox/Photos').resolve(),
+            ],
+            processes=5
+        )
         
-        # Usage
+        
+        ```
+        
+        
+        
+        # Command line usage:
         
         ```
         usage: exif2pandas [-h] [-s SQLITE] [-f FEATHER] [-e EXCEL] [-p PROCESSES]
                            picture_folders [picture_folders ...]
         
         Generate sql database with exif data.
```

### Comparing `exif2pandas-1.5/README.md` & `exif2pandas-2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,44 @@
 
 and anything else that [Pandas supports](https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html).
 
 
 ## Installation
 
 ```
-    $ pip install exif2pandas --user
+    $ pip3 install exif2pandas --user
 ```
 
 To export the dataframe you will need one of these modules:
 
- - SQLite: ``pip install --user SQLAlchemy`` 
- - Feather: ``pip install --user pyarrow`` 
- - Excel: ``pip install --user xlsxwriter``
+ - SQLite: ``pip3 install --user SQLAlchemy`` 
+ - Feather: ``pip3 install --user pyarrow`` 
+ - Excel: ``pip3 install --user xlsxwriter``
+
+# Python module usage:
+
+```python
+from exif2pandas import extract
+from pathlib import Path
+
+
+df = extract.extract_feather(
+    feather_path=Path('photos.feather').resolve(),
+    pictures_root=[
+        Path('/Users/visgean/Dropbox/Photos').resolve(),
+    ],
+    processes=5
+)
 
-# Usage
+
+```
+
+
+
+# Command line usage:
 
 ```
 usage: exif2pandas [-h] [-s SQLITE] [-f FEATHER] [-e EXCEL] [-p PROCESSES]
                    picture_folders [picture_folders ...]
 
 Generate sql database with exif data.
```

### Comparing `exif2pandas-1.5/exif2pandas/clean.py` & `exif2pandas-2.0/exif2pandas/clean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,71 @@
+import logging
 import os
 
 from datetime import datetime
 from typing import Optional
 from fractions import Fraction
 from slugify import slugify
 
 from .gps_utils import get_exif_location
 
 IGNORE_STARTSWITH = (
-    'MakerNote Tag',
-    'Thumbnail',
-    'Image Tag',
-    'Image PrintIM',
-    'MakerNote Internal',
-    'EXIF MakerNote',
-    'JPEGThumbnail',
+    "MakerNote Tag",
+    "Thumbnail",
+    "Image Tag",
+    "Image PrintIM",
+    "MakerNote Internal",
+    "EXIF MakerNote",
+    "JPEGThumbnail",
 )
 
 
 def parse_exif_date(dt) -> Optional[datetime]:
     try:
-        return datetime.strptime(str(dt.values), '%Y:%m:%d %H:%M:%S')
+        return datetime.strptime(str(dt.values), "%Y:%m:%d %H:%M:%S")
     except ValueError:
         return None
 
 
 def parse_date(exif_info) -> Optional[datetime]:
-    if 'Image DateTimeOriginal' in exif_info:
-        return parse_exif_date(exif_info['Image DateTimeOriginal'])
-    if 'Image DateTime' in exif_info:
-        return parse_exif_date(exif_info['Image DateTime'])
+    if "Image DateTimeOriginal" in exif_info:
+        return parse_exif_date(exif_info["Image DateTimeOriginal"])
+    if "Image DateTime" in exif_info:
+        return parse_exif_date(exif_info["Image DateTime"])
 
 
 def clean_exif_data(path, data, ignore_keys=IGNORE_STARTSWITH) -> dict:
     """
     Cleans exif data for each picture
     """
-    lat, lon = get_exif_location(data)
-    size = os.path.getsize(path) / 1024 ** 2
+    try:
+        lat, lon = get_exif_location(data)
+    except Exception as e:
+        logging.error(f"Could not get exif for {path}", exc_info=e)
+        lat, lon = None, None
+
+    size = os.path.getsize(path) / 1024**2
 
     cleaned_data = {
-        'filename': str(path),
-        'cleaned_latitude': lat,
-        'cleaned_longitude': lon,
-        'size_megabytes': size,
-        'cleaned_date': parse_date(data)
+        "filename": str(path),
+        "cleaned_latitude": lat,
+        "cleaned_longitude": lon,
+        "size_megabytes": size,
+        "cleaned_date": parse_date(data),
     }
 
     for key, tag in data.items():
         if not any([key.startswith(prefix) for prefix in ignore_keys]):
             if tag and tag.values and len(tag.values) == 1:
                 cleaned_val = tag.values[0]
                 if isinstance(cleaned_val, Fraction):
-                    cleaned_data[slugify(f'{key}-float')] = (
+                    cleaned_data[slugify(f"{key}-float")] = (
                         cleaned_val.numerator / cleaned_val.denominator
-                        if cleaned_val.denominator != 0 else 0.0
+                        if cleaned_val.denominator != 0
+                        else 0.0
                     )
                     cleaned_val = tag.printable
             else:
                 cleaned_val = tag.printable
 
             cleaned_data[slugify(key)] = cleaned_val
```

### Comparing `exif2pandas-1.5/exif2pandas/gps_utils.py` & `exif2pandas-2.0/exif2pandas/gps_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,26 +17,23 @@
 
 
 def get_exif_location(exif_data):
     """
     Returns the latitude and longitude, if available, from the provided exif_data
     (obtained through get_exif_data above)
     """
-    lat = None
-    lon = None
-
-    gps_latitude = exif_data.get('GPS GPSLatitude')
-    gps_latitude_ref = exif_data.get('GPS GPSLatitudeRef')
-    gps_longitude = exif_data.get('GPS GPSLongitude')
-    gps_longitude_ref = exif_data.get('GPS GPSLongitudeRef')
+    gps_latitude = exif_data.get("GPS GPSLatitude")
+    gps_latitude_ref = exif_data.get("GPS GPSLatitudeRef")
+    gps_longitude = exif_data.get("GPS GPSLongitude")
+    gps_longitude_ref = exif_data.get("GPS GPSLongitudeRef")
 
     if gps_latitude and gps_latitude_ref and gps_longitude and gps_longitude_ref:
         lat = convert_to_degress(gps_latitude)
-        if gps_latitude_ref.values[0] != 'N':
+        if gps_latitude_ref.values[0] != "N":
             lat = round(0 - lat, 6)
 
         lon = convert_to_degress(gps_longitude)
-        if gps_longitude_ref.values[0] != 'E':
+        if gps_longitude_ref.values[0] != "E":
             lon = round(0 - lon, 6)
         return lat, lon
 
     return None, None
```

### Comparing `exif2pandas-1.5/exif2pandas/utils.py` & `exif2pandas-2.0/exif2pandas/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import pandas as pd
 import exifread
 import os
+import logging
 
 from pathlib import Path
 from typing import List
 from multiprocessing import Pool
 from .clean import clean_exif_data
 
-picture_globs = ['*.jpg', '*.jpeg', '*.png', '*.JPG', '*.JPEG', '*.PNG']
+
+picture_globs = ["*.jpg", "*.jpeg", "*.png", "*.JPG", "*.JPEG", "*.PNG"]
 
 PROCESSES_DEFAULT = 5
 
 
 def get_extension(filename):
     filename, file_extension = os.path.splitext(filename)
     return file_extension.lower()
@@ -21,49 +23,42 @@
     pics = []
     for glob in picture_globs:
         pics.extend(directory.rglob(glob))
     return pics
 
 
 def get_exif(path):
-    with open(path, 'rb') as f:
+    with open(path, "rb") as f:
         return clean_exif_data(path, exifread.process_file(f))
 
 
 def simple_extract_exif(fnames: List[Path]):
-    return [
-        get_exif(f)
-        for f in fnames
-    ]
+    return [get_exif(f) for f in fnames]
 
 
 def multiprocess_extract_exif(fnames: List[Path], processes: int):
     with Pool(processes) as pool:
         return pool.map(get_exif, fnames)
 
 
 def get_panda_df(folder_names, processes=PROCESSES_DEFAULT, existing_df=None):
     pics_filenames = []
     for folder in folder_names:
         abs_path = Path(folder).resolve()
         pics_filenames.extend(get_pictures(abs_path))
 
     if existing_df is not None:
-        existing_rows = set([Path(p) for p in  existing_df['filename'].values])
+        existing_rows = set([Path(p) for p in existing_df["filename"].values])
         pics_filenames = list(set(pics_filenames) - set(existing_rows))
 
     imgs_to_scan = len(pics_filenames)
 
-    print(f'Scanning {imgs_to_scan} new photos')
+    logging.info(f"Scanning {imgs_to_scan} new photos")
     if imgs_to_scan > 1000:
-        print(f'Using {processes} processes. ')
+        logging.info(f"Using {processes} processes. ")
         cleaned_data = multiprocess_extract_exif(pics_filenames, processes)
     else:
         cleaned_data = simple_extract_exif(pics_filenames)
 
     if existing_df is not None:
-        cleaned_data.extend(existing_df.to_dict(orient='records'))
+        cleaned_data.extend(existing_df.to_dict(orient="records"))
     return pd.DataFrame(cleaned_data)
-
-
-
-
```

### Comparing `exif2pandas-1.5/exif2pandas.egg-info/PKG-INFO` & `exif2pandas-2.0/exif2pandas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exif2pandas
-Version: 1.5
+Version: 2.0
 Summary: Extract EXIF to pandas / SQL / Excel / Feather
 Home-page: https://github.com/visgean/exif2pandas
 Author: Visgean
 Author-email: visgean@gmail.com
 License: MIT
 Description: # Extract EXIF to pandas / SQL / Excel / Feather
         
@@ -22,24 +22,44 @@
         
         and anything else that [Pandas supports](https://pandas.pydata.org/pandas-docs/stable/user_guide/io.html).
         
         
         ## Installation
         
         ```
-            $ pip install exif2pandas --user
+            $ pip3 install exif2pandas --user
         ```
         
         To export the dataframe you will need one of these modules:
         
-         - SQLite: ``pip install --user SQLAlchemy`` 
-         - Feather: ``pip install --user pyarrow`` 
-         - Excel: ``pip install --user xlsxwriter``
+         - SQLite: ``pip3 install --user SQLAlchemy`` 
+         - Feather: ``pip3 install --user pyarrow`` 
+         - Excel: ``pip3 install --user xlsxwriter``
+        
+        # Python module usage:
+        
+        ```python
+        from exif2pandas import extract
+        from pathlib import Path
+        
+        
+        df = extract.extract_feather(
+            feather_path=Path('photos.feather').resolve(),
+            pictures_root=[
+                Path('/Users/visgean/Dropbox/Photos').resolve(),
+            ],
+            processes=5
+        )
         
-        # Usage
+        
+        ```
+        
+        
+        
+        # Command line usage:
         
         ```
         usage: exif2pandas [-h] [-s SQLITE] [-f FEATHER] [-e EXCEL] [-p PROCESSES]
                            picture_folders [picture_folders ...]
         
         Generate sql database with exif data.
```

### Comparing `exif2pandas-1.5/setup.py` & `exif2pandas-2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,39 +8,33 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
-    name='exif2pandas',
-    version='1.5',
-
+    name="exif2pandas",
+    version="2.0",
     description="Extract EXIF to pandas / SQL / Excel / Feather",
     long_description=long_description,
     long_description_content_type="text/markdown",
-
     author="Visgean",
-    author_email='visgean@gmail.com',
-    url='https://github.com/visgean/exif2pandas',
+    author_email="visgean@gmail.com",
+    url="https://github.com/visgean/exif2pandas",
     packages=[
-        'exif2pandas',
+        "exif2pandas",
     ],
-    package_dir={'exif2pandas': 'exif2pandas'},
+    package_dir={"exif2pandas": "exif2pandas"},
     license="MIT",
-    keywords='exif sql',
+    keywords="exif sql",
     classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
     ],
     install_requires=[
-        'exifread==2.3.2',
-        'pandas',
-        'python-slugify',
+        "exifread==2.3.2",
+        "pandas",
+        "python-slugify",
     ],
-    entry_points={
-        'console_scripts': [
-            'exif2pandas = exif2pandas.main:main'
-        ]
-    },
-)
+    entry_points={"console_scripts": ["exif2pandas = exif2pandas.main:main"]},
+)
```

