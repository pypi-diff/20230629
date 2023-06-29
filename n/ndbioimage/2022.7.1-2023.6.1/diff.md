# Comparing `tmp/ndbioimage-2022.7.1.tar.gz` & `tmp/ndbioimage-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2022.7.1.tar", last modified: Sun Jul 17 10:14:51 2022, max compression
+gzip compressed data, was "ndbioimage-2023.6.1.tar", max compression
```

## Comparing `ndbioimage-2022.7.1.tar` & `ndbioimage-2023.6.1.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-07-17 10:14:51.164398 ndbioimage-2022.7.1/
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)    35149 2022-07-15 11:39:50.000000 ndbioimage-2022.7.1/LICENSE
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     3436 2022-07-17 10:14:51.164398 ndbioimage-2022.7.1/PKG-INFO
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     2906 2022-07-15 12:18:39.000000 ndbioimage-2022.7.1/README.md
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-07-17 10:14:51.164398 ndbioimage-2022.7.1/ndbioimage/
--rwxr-xr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)    60547 2022-07-17 09:21:39.000000 ndbioimage-2022.7.1/ndbioimage/__init__.py
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)       57 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage/_version.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     1563 2022-07-15 09:29:04.000000 ndbioimage-2022.7.1/ndbioimage/jvm.py
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-07-17 10:14:51.164398 ndbioimage-2022.7.1/ndbioimage/readers/
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      194 2022-07-15 08:43:29.000000 ndbioimage-2022.7.1/ndbioimage/readers/__init__.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     3830 2022-07-15 09:08:56.000000 ndbioimage-2022.7.1/ndbioimage/readers/bfread.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     6082 2022-07-17 10:14:28.000000 ndbioimage-2022.7.1/ndbioimage/readers/cziread.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      805 2022-07-15 09:34:15.000000 ndbioimage-2022.7.1/ndbioimage/readers/ndread.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     3459 2022-07-15 08:51:59.000000 ndbioimage-2022.7.1/ndbioimage/readers/seqread.py
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     1696 2022-07-15 08:51:59.000000 ndbioimage-2022.7.1/ndbioimage/readers/tifread.py
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      187 2022-07-15 08:02:04.000000 ndbioimage-2022.7.1/ndbioimage/transform.txt
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     9146 2022-07-17 08:56:50.000000 ndbioimage-2022.7.1/ndbioimage/transforms.py
-drwxrwxr-x   0 w.pomp   (1262200273) w.pomp   (1262200273)        0 2022-07-17 10:14:51.164398 ndbioimage-2022.7.1/ndbioimage.egg-info/
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     3436 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage.egg-info/PKG-INFO
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      525 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage.egg-info/SOURCES.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)        1 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage.egg-info/dependency_links.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)       58 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage.egg-info/entry_points.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)      161 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage.egg-info/requires.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)       11 2022-07-17 10:14:51.000000 ndbioimage-2022.7.1/ndbioimage.egg-info/top_level.txt
--rw-rw-r--   0 w.pomp   (1262200273) w.pomp   (1262200273)       38 2022-07-17 10:14:51.164398 ndbioimage-2022.7.1/setup.cfg
--rw-r--r--   0 w.pomp   (1262200273) w.pomp   (1262200273)     1740 2022-07-17 10:13:14.000000 ndbioimage-2022.7.1/setup.py
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.6.1/LICENSE
+-rw-r--r--   0        0        0     2418 2023-06-29 12:27:04.230942 ndbioimage-2023.6.1/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.6.1/ndbioimage/.DS_Store
+-rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.6.1/ndbioimage/AiryScan.xml
+-rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.6.1/ndbioimage/Elyra_test.xml
+-rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.6.1/ndbioimage/Elyra_test2.xml
+-rwxr-xr-x   0        0        0    55945 2023-06-29 12:01:13.598678 ndbioimage-2023.6.1/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.6.1/ndbioimage/bf.py
+-rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.6.1/ndbioimage/jvm.py
+-rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.6.1/ndbioimage/ntransforms.py
+-rw-r--r--   0        0        0      146 2023-05-25 09:20:54.527861 ndbioimage-2023.6.1/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8187 2023-06-29 12:01:13.546678 ndbioimage-2023.6.1/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    22889 2023-05-26 07:14:19.001535 ndbioimage-2023.6.1/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.6.1/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     5302 2023-05-25 14:09:31.628409 ndbioimage-2023.6.1/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.6.1/ndbioimage/readers/tifread.py
+-rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.6.1/ndbioimage/test.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.6.1/ndbioimage/transform.txt
+-rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.6.1/ndbioimage/transforms.py
+-rw-r--r--   0        0        0      805 2023-06-29 12:31:28.546990 ndbioimage-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 ndbioimage-2023.6.1/PKG-INFO
```

### Comparing `ndbioimage-2022.7.1/LICENSE` & `ndbioimage-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2022.7.1/PKG-INFO` & `ndbioimage-2023.6.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,108 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2022.7.1
+Version: 2023.6.1
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
-Author: Wim Pomp
+License: GPLv3
+Keywords: bioformats,imread,numpy,metadata
+Author: W. Pomp
 Author-email: w.pomp@nki.nl
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: test
+Requires-Dist: JPype1
+Requires-Dist: SimpleITK-SimpleElastix
+Requires-Dist: czifile
+Requires-Dist: lxml
+Requires-Dist: numpy
+Requires-Dist: ome-types
+Requires-Dist: pandas
+Requires-Dist: parfor
+Requires-Dist: pint
+Requires-Dist: pytest
+Requires-Dist: pyyaml
+Requires-Dist: tifffile
+Requires-Dist: tiffwrite
+Requires-Dist: tqdm
+Project-URL: Repository, https://github.com/wimpomp/ndbioimage
 Description-Content-Type: text/markdown
-Provides-Extra: transforms
-Provides-Extra: bioformats
-License-File: LICENSE
-
-# ndbioimage
-
-Exposes (bio) images as a numpy ndarray like object, but without loading the whole
-image into memory, reading from the file only when needed. Some metadata is read
-and exposed as attributes to the Imread object (TODO: structure data in OME format).
-Additionally, it can automatically calculate an affine transform that corrects for
-chromatic abberrations etc. and apply it on the fly to the image.
+
+# ndbioimage - Work in progress
+
+Exposes (bio) images as a numpy ndarray-like-object, but without loading the whole
+image into memory, reading from the file only when needed. Some metadata is read and
+and stored in an ome structure. Additionally, it can automatically calculate an affine
+transform that corrects for chromatic abberrations etc. and apply it on the fly to the image.
 
 Currently supports imagej tif files, czi files, micromanager tif sequences and anything
 bioformats can handle. 
 
 ## Installation
 
     pip install ndbioimage@git+https://github.com/wimpomp/ndbioimage.git
 
-### With bioformats (if java is properly installed)
-
-    pip install ndbioimage[bioformats]@git+https://github.com/wimpomp/ndbioimage.git
-
-### With affine transforms (only for python 3.8, 3.9 and 3.10)
-
-    pip install ndbioimage[transforms]@git+https://github.com/wimpomp/ndbioimage.git
 
 ## Usage
 
 - Reading an image file and plotting the frame at channel=2, time=1
 
 
     import matplotlib.pyplot as plt
-    from ndbioimage import imread
-    with imread('image_file.tif', axes='ctxy', dtype=int) as im:
+    from ndbioimage import Imread
+    with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
         plt.imshow(im[2, 1])
 
 - Showing some image metadata
 
 
-    from ndbioimage import imread
+    from ndbioimage import Imread
     from pprint import pprint
-    with imread('image_file.tif') as im:
+    with Imread('image_file.tif') as im:
         pprint(im)
 
 - Slicing the image without loading the image into memory
 
 
-    from ndbioimage import imread
-    with imread('image_file.tif', axes='cztxy') as im:
+    from ndbioimage import Imread
+    with Imread('image_file.tif', axes='cztxy') as im:
         sliced_im = im[1, :, :, 100:200, 100:200]
 
-sliced_im is an instance of imread which will load any image data from file only when needed
+sliced_im is an instance of Imread which will load any image data from file only when needed
 
 
 - Converting (part) of the image to a numpy ndarray
 
 
-    from ndbioimage import imread
+    from ndbioimage import Imread
     import numpy as np
-    with imread('image_file.tif', axes='cztxy') as im:
+    with Imread('image_file.tif', axes='cztxy') as im:
         array = np.asarray(im[0, 0])
 
 ## Adding more formats
 Readers for image formats subclass Imread. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 subclass Imread and are required to implement the following methods:
 
 - staticmethod _can_open(path): return True if path can be opened by this reader
-- \_\_metadata__(self): reads metadata from file and adds them to self as attributes,
-  - the shape of the data in the file needs to be set as self.shape = (X, Y, C, Z, T)
-  - other attributes like pxsize, acquisitiontime and title can be set here as well
+- property ome: reads metadata from file and adds them to an OME object imported
+from the ome-types library 
 - \_\_frame__(self, c, z, t): return the frame at channel=c, z-slice=z, time=t from the file
 
 Optional methods:
 - open(self): maybe open some file
 - close(self): close any file handles
 
 Optional fields:
 - priority (int): Imread will try readers with a lower number first, default: 99
 - do_not_pickle (strings): any attributes that should not be included when the object is pickled,
 for example: any file handles
 
 # TODO
-- structure the metadata in OME format tree
+- more image formats
 - re-implement transforms 
+
```

### Comparing `ndbioimage-2022.7.1/README.md` & `ndbioimage-2023.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,73 @@
-# ndbioimage
+# ndbioimage - Work in progress
 
-Exposes (bio) images as a numpy ndarray like object, but without loading the whole
-image into memory, reading from the file only when needed. Some metadata is read
-and exposed as attributes to the Imread object (TODO: structure data in OME format).
-Additionally, it can automatically calculate an affine transform that corrects for
-chromatic abberrations etc. and apply it on the fly to the image.
+Exposes (bio) images as a numpy ndarray-like-object, but without loading the whole
+image into memory, reading from the file only when needed. Some metadata is read and
+and stored in an ome structure. Additionally, it can automatically calculate an affine
+transform that corrects for chromatic abberrations etc. and apply it on the fly to the image.
 
 Currently supports imagej tif files, czi files, micromanager tif sequences and anything
 bioformats can handle. 
 
 ## Installation
 
     pip install ndbioimage@git+https://github.com/wimpomp/ndbioimage.git
 
-### With bioformats (if java is properly installed)
-
-    pip install ndbioimage[bioformats]@git+https://github.com/wimpomp/ndbioimage.git
-
-### With affine transforms (only for python 3.8, 3.9 and 3.10)
-
-    pip install ndbioimage[transforms]@git+https://github.com/wimpomp/ndbioimage.git
 
 ## Usage
 
 - Reading an image file and plotting the frame at channel=2, time=1
 
 
     import matplotlib.pyplot as plt
-    from ndbioimage import imread
-    with imread('image_file.tif', axes='ctxy', dtype=int) as im:
+    from ndbioimage import Imread
+    with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
         plt.imshow(im[2, 1])
 
 - Showing some image metadata
 
 
-    from ndbioimage import imread
+    from ndbioimage import Imread
     from pprint import pprint
-    with imread('image_file.tif') as im:
+    with Imread('image_file.tif') as im:
         pprint(im)
 
 - Slicing the image without loading the image into memory
 
 
-    from ndbioimage import imread
-    with imread('image_file.tif', axes='cztxy') as im:
+    from ndbioimage import Imread
+    with Imread('image_file.tif', axes='cztxy') as im:
         sliced_im = im[1, :, :, 100:200, 100:200]
 
-sliced_im is an instance of imread which will load any image data from file only when needed
+sliced_im is an instance of Imread which will load any image data from file only when needed
 
 
 - Converting (part) of the image to a numpy ndarray
 
 
-    from ndbioimage import imread
+    from ndbioimage import Imread
     import numpy as np
-    with imread('image_file.tif', axes='cztxy') as im:
+    with Imread('image_file.tif', axes='cztxy') as im:
         array = np.asarray(im[0, 0])
 
 ## Adding more formats
 Readers for image formats subclass Imread. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 subclass Imread and are required to implement the following methods:
 
 - staticmethod _can_open(path): return True if path can be opened by this reader
-- \_\_metadata__(self): reads metadata from file and adds them to self as attributes,
-  - the shape of the data in the file needs to be set as self.shape = (X, Y, C, Z, T)
-  - other attributes like pxsize, acquisitiontime and title can be set here as well
+- property ome: reads metadata from file and adds them to an OME object imported
+from the ome-types library 
 - \_\_frame__(self, c, z, t): return the frame at channel=c, z-slice=z, time=t from the file
 
 Optional methods:
 - open(self): maybe open some file
 - close(self): close any file handles
 
 Optional fields:
 - priority (int): Imread will try readers with a lower number first, default: 99
 - do_not_pickle (strings): any attributes that should not be included when the object is pickled,
 for example: any file handles
 
 # TODO
-- structure the metadata in OME format tree
+- more image formats
 - re-implement transforms
```

### Comparing `ndbioimage-2022.7.1/ndbioimage/__init__.py` & `ndbioimage-2023.6.1/ndbioimage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,202 +1,211 @@
-import os
 import re
 import inspect
 import pandas
 import yaml
 import numpy as np
+import multiprocessing
+import ome_types
+from ome_types import ureg, model
+from pint import set_application_registry
 from datetime import datetime
 from tqdm.auto import tqdm
 from itertools import product
 from collections import OrderedDict
 from abc import ABCMeta, abstractmethod
 from functools import cached_property
 from parfor import parfor
 from tiffwrite import IJTiffFile
 from numbers import Number
 from argparse import ArgumentParser
-from warnings import warn
 from ndbioimage.transforms import Transform, Transforms
 from ndbioimage.jvm import JVM
-from ndbioimage._version import __version__, __git_commit_hash__
-
-
-class ImTransformsBase(Transforms):
-    def coords(self, array, colums=None):
-        if isinstance(array, pandas.DataFrame):
-            return pandas.concat([self(int(row['C']), int(row['T'])).coords(row, colums)
-                                  for _, row in array.iterrows()], axis=1).T
-        elif isinstance(array, pandas.Series):
-            return self(int(array['C']), int(array['T'])).coords(array, colums)
-        else:
-            raise TypeError('Not a pandas DataFrame or Series.')
-
-
-class ImTransforms(ImTransformsBase):
-    """ Transforms class with methods to calculate channel transforms from bead files etc.
-    """
-    def __init__(self, path, cyllens, tracks=None, detectors=None, file=None, transforms=None):
+from typing import List
+from pathlib import Path
+from importlib.metadata import version
+from traceback import print_exc
+
+
+try:
+    __version__ = version(Path(__file__).parent.name)
+except (Exception,):
+    __version__ = 'unknown'
+
+try:
+    with open(Path(__file__).parent.parent / '.git' / 'HEAD') as g:
+        head = g.read().split(':')[1].strip()
+    with open(Path(__file__).parent.parent / '.git' / head) as h:
+        __git_commit_hash__ = h.read().rstrip('\n')
+except (Exception,):
+    __git_commit_hash__ = 'unknown'
+
+ureg.default_format = '~P'
+set_application_registry(ureg)
+
+
+class ImTransforms(Transforms):
+    """ Transforms class with methods to calculate channel transforms from bead files etc. """
+    def __init__(self, path, cyllens, file=None, transforms=None):
         super().__init__()
         self.cyllens = cyllens
-        self.tracks = tracks
-        self.detectors = detectors
         if transforms is None:
             # TODO: check this
-            if re.search(r'^Pos\d+', os.path.basename(path.rstrip(os.path.sep))):
-                self.path = os.path.dirname(os.path.dirname(path))
+            if re.search(r'^Pos\d+', path.name):
+                self.path = path.parent.parent
             else:
-                self.path = os.path.dirname(path)
+                self.path = path.parent
             if file is not None:
                 if isinstance(file, str) and file.lower().endswith('.yml'):
                     self.ymlpath = file
                     self.beadfile = None
                 else:
-                    self.ymlpath = os.path.join(self.path, 'transform.yml')
+                    self.ymlpath = self.path / 'transform.yml'
                     self.beadfile = file
             else:
-                self.ymlpath = os.path.join(self.path, 'transform.yml')
+                self.ymlpath = self.path / 'transform.yml'
                 self.beadfile = None
-            self.tifpath = self.ymlpath[:-3] + 'tif'
+            self.tifpath = self.ymlpath.with_suffix('.tif')
             try:
                 self.load(self.ymlpath)
-            except Exception:
+            except (Exception,):
                 print('No transform file found, trying to generate one.')
                 if not self.files:
                     raise FileNotFoundError('No bead files found to calculate the transform from.')
                 self.calculate_transforms()
                 self.save(self.ymlpath)
                 self.save_transform_tiff()
                 print(f'Saving transform in {self.ymlpath}.')
                 print(f'Please check the transform in {self.tifpath}.')
         else:  # load from dict transforms
             self.path = path
             self.beadfile = file
-            for key, value in transforms.items():
-                self[tuple([int(i) for i in key.split(':')])] = Transform(value)
+            for i, (key, value) in enumerate(transforms.items()):
+                self[key] = Transform(value)
+
+    def coords_pandas(self, array, cnamelist, colums=None):
+        if isinstance(array, pandas.DataFrame):
+            return pandas.concat([self[(cnamelist[int(row['C'])],)].coords(row, colums)
+                                  for _, row in array.iterrows()], axis=1).T
+        elif isinstance(array, pandas.Series):
+            return self[(cnamelist[int(array['C'])],)].coords(array, colums)
+        else:
+            raise TypeError('Not a pandas DataFrame or Series.')
 
     @cached_property
     def files(self):
         try:
             if self.beadfile is None:
                 files = self.get_bead_files()
             else:
                 files = self.beadfile
             if isinstance(files, str):
+                files = (Path(files),)
+            elif isinstance(files, Path):
                 files = (files,)
             return files
-        except Exception:
+        except (Exception,):
             return ()
 
-    def __reduce__(self):
-        return self.__class__, (self.path, self.cyllens, self.tracks, self.detectors, self.files, self.asdict())
-
-    def __call__(self, channel, time=None, tracks=None, detectors=None):
-        tracks = tracks or self.tracks
-        detectors = detectors or self.detectors
-        return super().__call__(channel, time, tracks, detectors)
-
     def get_bead_files(self):
-        files = sorted([os.path.join(self.path, f) for f in os.listdir(self.path) if f.lower().startswith('beads')
-                        and not f.lower().endswith('.pdf') and not f.lower().endswith('pkl')])
+        files = sorted([f for f in self.path.parent.iterdir() if f.name.lower().startswith('beads')
+                        and not f.suffix.lower() == '.pdf' and not f.suffix.lower() == 'pkl'])
         if not files:
             raise Exception('No bead file found!')
-        Files = []
+        checked_files = []
         for file in files:
             try:
-                if os.path.isdir(file):
-                    file = os.path.join(file, 'Pos0')
-                with Imread(file) as im:  # check for errors opening the file
-                    pass
-                Files.append(file)
-            except Exception:
+                if file.is_dir():
+                    file /= 'Pos0'
+                with Imread(file):  # check for errors opening the file
+                    checked_files.append(file)
+            except (Exception,):
                 continue
-        if not Files:
+        if not checked_files:
             raise Exception('No bead file found!')
-        return Files
+        return checked_files
 
     def calculate_transform(self, file):
         """ When no channel is not transformed by a cylindrical lens, assume that the image is scaled by a factor 1.162
-            in the horizontal direction
-        """
-        with Imread(file) as im:
-            ims = [im.max(c) for c in range(im.shape[2])]
-            goodch = [c for c in range(im.shape[2]) if not im.isnoise(im.max(c))]
-            untransformed = [c for c in range(im.shape[2]) if self.cyllens[im.detector[c]].lower() == 'none']
+            in the horizontal direction """
+        with Imread(file, axes='zcxy') as im:
+            max_ims = im.max('z')
+            goodch = [c for c, max_im in enumerate(max_ims) if not im.is_noise(max_im)]
+            if not goodch:
+                goodch = list(range(len(max_ims)))
+            untransformed = [c for c in range(im.shape['c']) if self.cyllens[im.detector[c]].lower() == 'none']
 
             good_and_untrans = sorted(set(goodch) & set(untransformed))
             if good_and_untrans:
                 masterch = good_and_untrans[0]
             else:
                 masterch = goodch[0]
-            print(f'{untransformed = }, {masterch = }, {goodch = }')
-            C = Transform()
+            transform = Transform()
             if not np.any(good_and_untrans):
-                M = C.matrix
-                M[0, 0] = 0.86
-                C.matrix = M
-            Tr = Transforms()
+                matrix = transform.matrix
+                matrix[0, 0] = 0.86
+                transform.matrix = matrix
+            transforms = Transforms()
             for c in tqdm(goodch):
                 if c == masterch:
-                    Tr[im.track[c], im.detector[c]] = C
+                    transforms[(im.cnamelist[c],)] = transform
                 else:
-                    Tr[im.track[c], im.detector[c]] = Transform(ims[masterch], ims[c]) * C
-        return Tr
+                    transforms[(im.cnamelist[c],)] = Transform(max_ims[masterch], max_ims[c]) * transform
+        return transforms
 
     def calculate_transforms(self):
-        Tq = [self.calculate_transform(file) for file in self.files]
-        for key in set([key for t in Tq for key in t.keys()]):
-            T = [t[key] for t in Tq if key in t]
-            if len(T) == 1:
-                self[key] = T[0]
+        transforms = [self.calculate_transform(file) for file in self.files]
+        for key in set([key for transform in transforms for key in transform.keys()]):
+            new_transforms = [transform[key] for transform in transforms if key in transform]
+            if len(new_transforms) == 1:
+                self[key] = new_transforms[0]
             else:
                 self[key] = Transform()
-                self[key].parameters = np.mean([t.parameters for t in T], 0)
-                self[key].dparameters = (np.std([t.parameters for t in T], 0) / np.sqrt(len(T))).tolist()
+                self[key].parameters = np.mean([t.parameters for t in new_transforms], 0)
+                self[key].dparameters = (np.std([t.parameters for t in new_transforms], 0) /
+                                         np.sqrt(len(new_transforms))).tolist()
 
     def save_transform_tiff(self):
-        C = 0
+        n_channels = 0
         for file in self.files:
             with Imread(file) as im:
-                C = max(C, im.shape[2])
-        with IJTiffFile(self.tifpath, (C, 1, len(self.files))) as tif:
+                n_channels = max(n_channels, im.shape['c'])
+        with IJTiffFile(self.tifpath, (n_channels, 1, len(self.files))) as tif:
             for t, file in enumerate(self.files):
                 with Imread(file) as im:
                     with Imread(file, transform=True) as jm:
-                        for c in range(im.shape[2]):
-                            tif.save(np.hstack((im.max(c), jm.max(c))), c, 0, t)
+                        for c in range(im.shape['c']):
+                            tif.save(np.hstack((im(c=c, t=0).max('z'), jm(c=c, t=0).max('z'))), c, 0, t)
 
 
-class ImShiftTransforms(ImTransformsBase):
+class ImShiftTransforms(Transforms):
     """ Class to handle drift in xy. The image this is applied to must have a channeltransform already, which is then
-        replaced by this class.
-    """
+        replaced by this class. """
     def __init__(self, im, shifts=None):
         """ im:                     Calculate shifts from channel-transformed images
             im, t x 2 array         Sets shifts from array, one row per frame
             im, dict {frame: shift} Sets shifts from dict, each key is a frame number from where a new shift is applied
-            im, file                Loads shifts from a saved file
-        """
+            im, file                Loads shifts from a saved file """
         super().__init__()
         with (Imread(im, transform=True, drift=False) if isinstance(im, str)
                                                       else im.new(transform=True, drift=False)) as im:
             self.impath = im.path
-            self.path = os.path.splitext(self.impath)[0] + '_shifts.txt'
+            self.path = self.impath.parent / self.impath.stem + '_shifts.txt'
             self.tracks, self.detectors, self.files = im.track, im.detector, im.beadfile
             if shifts is not None:
                 if isinstance(shifts, np.ndarray):
                     self.shifts = shifts
                     self.shifts2transforms(im)
                 elif isinstance(shifts, dict):
-                    self.shifts = np.zeros((im.shape[4], 2))
+                    self.shifts = np.zeros((im.shape['t'], 2))
                     for k in sorted(shifts.keys()):
                         self.shifts[k:] = shifts[k]
                     self.shifts2transforms(im)
                 elif isinstance(shifts, str):
                     self.load(im, shifts)
-            elif os.path.exists(self.path):
+            elif self.path.exists():
                 self.load(im, self.path)
             else:
                 self.calulate_shifts(im)
                 self.save()
 
     def __call__(self, channel, time, tracks=None, detectors=None):
         tracks = tracks or self.tracks
@@ -205,51 +214,57 @@
         if (track, detector, time) in self:
             return self[track, detector, time]
         elif (0, detector, time) in self:
             return self[0, detector, time]
         else:
             return Transform()
 
-    def __reduce__(self):
-        return self.__class__, (self.impath, self.shifts)
-
     def load(self, im, file):
         self.shifts = np.loadtxt(file)
         self.shifts2transforms(im)
 
     def save(self, file=None):
         self.path = file or self.path
         np.savetxt(self.path, self.shifts)
 
+    def coords(self, array, colums=None):
+        if isinstance(array, pandas.DataFrame):
+            return pandas.concat([self(int(row['C']), int(row['T'])).coords(row, colums)
+                                  for _, row in array.iterrows()], axis=1).T
+        elif isinstance(array, pandas.Series):
+            return self(int(array['C']), int(array['T'])).coords(array, colums)
+        else:
+            raise TypeError('Not a pandas DataFrame or Series.')
+
     def calulate_shifts0(self, im):
         """ Calculate shifts relative to the first frame """
         im0 = im[:, 0, 0].squeeze().transpose(2, 0, 1)
 
-        @parfor(range(1, im.shape[4]), (im, im0), desc='Calculating image shifts.')
+        @parfor(range(1, im.shape['t']), (im, im0), desc='Calculating image shifts.')
         def fun(t, im, im0):
             return Transform(im0, im[:, 0, t].squeeze().transpose(2, 0, 1), 'translation')
         transforms = [Transform()] + fun
         self.shifts = np.array([t.parameters[4:] for t in transforms])
-        self.setTransforms(transforms, im.transform)
+        self.set_transforms(transforms, im.transform)
 
     def calulate_shifts(self, im):
         """ Calculate shifts relative to the previous frame """
-        @parfor(range(1, im.shape[4]), (im,), desc='Calculating image shifts.')
+        @parfor(range(1, im.shape['t']), (im,), desc='Calculating image shifts.')
         def fun(t, im):
             return Transform(im[:, 0, t-1].squeeze().transpose(2, 0, 1), im[:, 0, t].squeeze().transpose(2, 0, 1),
                              'translation')
         transforms = [Transform()] + fun
         self.shifts = np.cumsum([t.parameters[4:] for t in transforms])
-        self.setTransforms(transforms, im.transform)
+        self.set_transforms(transforms, im.transform)
 
     def shifts2transforms(self, im):
-        self.setTransforms([Transform(np.array(((1, 0, s[0]), (0, 1, s[1]), (0, 0, 1))))
-                            for s in self.shifts], im.transform)
+        self.set_transforms([Transform(np.array(((1, 0, s[0]), (0, 1, s[1]), (0, 0, 1))))
+                             for s in self.shifts], im.transform)
 
-    def setTransforms(self, shift_transforms, channel_transforms):
+    def set_transforms(self, shift_transforms, channel_transforms):
         for key, value in channel_transforms.items():
             for t, T in enumerate(shift_transforms):
                 self[key[0], key[1], t] = T * channel_transforms[key]
 
 
 class DequeDict(OrderedDict):
     def __init__(self, maxlen=None, *args, **kwargs):
@@ -266,28 +281,71 @@
         self.__truncate__()
 
     def update(self, *args, **kwargs):
         super().update(*args, **kwargs)
         self.__truncate__()
 
 
-def tolist(item):
-    if isinstance(item, XmlData):
-        return [item]
-    elif hasattr(item, 'items'):
+def tolist(item) -> List:
+    if hasattr(item, 'items'):
         return item
     elif isinstance(item, str):
         return [item]
     try:
         iter(item)
         return list(item)
     except TypeError:
         return list((item,))
 
 
+def find(obj, **kwargs):
+    for item in obj:
+        if all([getattr(item, key) == value for key, value in kwargs.items()]):
+            return item
+
+
+def find_rec(obj, **kwargs):
+    if isinstance(obj, list):
+        for item in obj:
+            ans = find_rec(item, **kwargs)
+            if ans:
+                return ans
+    elif isinstance(obj, ome_types._base_type.OMEType):
+        if all([hasattr(obj, key) for key in kwargs.keys()]) and all(
+                [getattr(obj, key) == value for key, value in kwargs.items()]):
+            return obj
+        for k, v in obj.__dict__.items():
+            ans = find_rec(v, **kwargs)
+            if ans:
+                return ans
+
+
+def try_default(fun, default, *args, **kwargs):
+    try:
+        return fun(*args, **kwargs)
+    except (Exception,):
+        return default
+
+
+def ome_subprocess(path):
+    try:
+        jvm = JVM()
+        ome_meta = jvm.metadata_tools.createOMEXMLMetadata()
+        reader = jvm.image_reader()
+        reader.setMetadataStore(ome_meta)
+        reader.setId(str(path))
+        ome = ome_types.from_xml(str(ome_meta.dumpXML()), parser='lxml')
+    except (Exception,):
+        print_exc()
+        ome = model.OME()
+    finally:
+        jvm.kill_vm()
+    return ome
+
+
 class Shape(tuple):
     def __new__(cls, shape, axes='xyczt'):
         instance = super().__new__(cls, shape)
         instance.axes = axes.lower()
         return instance
 
     def __getitem__(self, n):
@@ -299,193 +357,14 @@
         return super().__getitem__(n)
 
     @cached_property
     def xyczt(self):
         return tuple(self[i] for i in 'xyczt')
 
 
-class XmlData(OrderedDict):
-    def __init__(self, elem=None):
-        super(XmlData, self).__init__()
-        if elem:
-            if isinstance(elem, dict):
-                self.update(elem)
-            else:
-                self.update(XmlData._todict(elem)[1])
-
-    def re_search(self, reg, default=None, *args, **kwargs):
-        return tolist(XmlData._output(XmlData._search(self, reg, True, default, *args, **kwargs)[1]))
-
-    def search(self, key, default=None):
-        return tolist(XmlData._output(XmlData._search(self, key, False, default)[1]))
-
-    def re_search_all(self, reg, *args, **kwargs):
-        K, V = XmlData._search_all(self, reg, True, *args, **kwargs)
-        return {k: XmlData._output(v) for k, v in zip(K, V)}
-
-    def search_all(self, key):
-        K, V = XmlData._search_all(self, key, False)
-        return {k: XmlData._output(v) for k, v in zip(K, V)}
-
-    @staticmethod
-    def _search(d, key, regex=False, default=None, *args, **kwargs):
-        if isinstance(key, (list, tuple)):
-            if len(key) == 1:
-                key = key[0]
-            else:
-                for v in XmlData._search_all(d, key[0], regex, *args, **kwargs)[1]:
-                    found, value = XmlData._search(v, key[1:], regex, default, *args, **kwargs)
-                    if found:
-                        return True, value
-                return False, default
-
-        if hasattr(d, 'items'):
-            for k, v in d.items():
-                if isinstance(k, str):
-                    if (not regex and k == key) or (regex and re.findall(key, k, *args, **kwargs)):
-                        return True, v
-                    elif isinstance(v, dict):
-                        found, value = XmlData._search(v, key, regex, default, *args, **kwargs)
-                        if found:
-                            return True, value
-                    elif isinstance(v, (list, tuple)):
-                        for w in v:
-                            found, value = XmlData._search(w, key, regex, default, *args, **kwargs)
-                            if found:
-                                return True, value
-                else:
-                    found, value = XmlData._search(v, key, regex, default, *args, **kwargs)
-                    if found:
-                        return True, value
-        return False, default
-
-    @staticmethod
-    def _search_all(d, key, regex=False, *args, **kwargs):
-        K = []
-        V = []
-        if hasattr(d, 'items'):
-            for k, v in d.items():
-                if isinstance(k, str):
-                    if (not regex and k == key) or (regex and re.findall(key, k, *args, **kwargs)):
-                        K.append(k)
-                        V.append(v)
-                    elif isinstance(v, dict):
-                        q, w = XmlData._search_all(v, key, regex, *args, **kwargs)
-                        K.extend([str(k) + '|' + i for i in q])
-                        V.extend(w)
-                    elif isinstance(v, (list, tuple)):
-                        for j, val in enumerate(v):
-                            q, w = XmlData._search_all(val, key, regex, *args, **kwargs)
-                            K.extend([str(k) + '|' + str(j) + '|' + i for i in q])
-                            V.extend(w)
-                else:
-                    q, w = XmlData._search_all(v, key, regex, *args, **kwargs)
-                    K.extend([str(k) + '|' + i for i in q])
-                    V.extend(w)
-        return K, V
-
-    @staticmethod
-    def _enumdict(d):
-        d2 = {}
-        for k, v in d.items():
-            idx = [int(i) for i in re.findall(r'(?<=:)\d+$', k)]
-            if idx:
-                key = re.findall(r'^.*(?=:\d+$)', k)[0]
-                if key not in d2:
-                    d2[key] = {}
-                d2[key][idx[0]] = d['{}:{}'.format(key, idx[0])]
-            else:
-                d2[k] = v
-        rec = False
-        for k, v in d2.items():
-            if [int(i) for i in re.findall(r'(?<=:)\d+$', k)]:
-                rec = True
-                break
-        if rec:
-            return XmlData._enumdict(d2)
-        else:
-            return d2
-
-    @staticmethod
-    def _unique_children(l):
-        if l:
-            keys, values = zip(*l)
-            d = {}
-            for k in set(keys):
-                value = [v for m, v in zip(keys, values) if k == m]
-                if len(value) == 1:
-                    d[k] = value[0]
-                else:
-                    d[k] = value
-            return d
-        else:
-            return {}
-
-    @staticmethod
-    def _todict(elem):
-        d = {}
-        if hasattr(elem, 'Key') and hasattr(elem, 'Value'):
-            name = elem.Key.cdata
-            d = elem.Value.cdata
-            return name, d
-
-        if hasattr(elem, '_attributes') and elem._attributes is not None and 'ID' in elem._attributes:
-            name = elem._attributes['ID']
-            elem._attributes.pop('ID')
-        elif hasattr(elem, '_name'):
-            name = elem._name
-        else:
-            name = 'none'
-
-        if name == 'Value':
-            if hasattr(elem, 'children') and len(elem.children):
-                return XmlData._todict(elem.children[0])
-
-        if hasattr(elem, 'children'):
-            children = [XmlData._todict(child) for child in elem.children]
-            children = XmlData._unique_children(children)
-            if children:
-                d = OrderedDict(d, **children)
-        if hasattr(elem, '_attributes'):
-            children = elem._attributes
-            if children:
-                d = OrderedDict(d, **children)
-        if not len(d.keys()) and hasattr(elem, 'cdata'):
-            return name, elem.cdata
-
-        return name, XmlData._enumdict(d)
-
-    @staticmethod
-    def _output(s):
-        if isinstance(s, dict):
-            return XmlData(s)
-        elif isinstance(s, (tuple, list)):
-            return [XmlData._output(i) for i in s]
-        elif not isinstance(s, str):
-            return s
-        elif len(s) > 1 and s[0] == '[' and s[-1] == ']':
-            return [XmlData._output(i) for i in s[1:-1].split(', ')]
-        elif re.search(r'^[-+]?\d+$', s):
-            return int(s)
-        elif re.search(r'^[-+]?\d?\d*\.?\d+([eE][-+]?\d+)?$', s):
-            return float(s)
-        elif s.lower() == 'true':
-            return True
-        elif s.lower() == 'false':
-            return False
-        elif s.lower() == 'none':
-            return None
-        else:
-            return s
-
-    def __getitem__(self, item):
-        value = super().__getitem__(item)
-        return XmlData(value) if isinstance(value, dict) else value
-
-
 class Imread(np.lib.mixins.NDArrayOperatorsMixin, metaclass=ABCMeta):
     """ class to read image files, while taking good care of important metadata,
             currently optimized for .czi files, but can open anything that bioformats can handle
         path: path to the image file
         optional:
         series: in case multiple experiments are saved in one file, like in .lif files
         transform: automatically correct warping between channels, need transforms.py among others
@@ -531,165 +410,216 @@
                 staticmethod _can_open(path): returns True when the subclass can open the image in path
                 __metadata__(self): pulls some metadata from the file and do other format specific things, it needs to
                                     define a few properties, like shape, etc.
                 __frame__(self, c, z, t): this should return a single frame at channel c, slice z and time t
                 optional close(self): close the file in a proper way
                 optional field priority: subclasses with lower priority will be tried first, default = 99
                 Any other method can be overridden as needed
-        wp@tl2019-2021
-    """
+        wp@tl2019-2023 """
 
     # TODO: more numpy.ndarray methods as needed
     # TODO: imread.std
     # TODO: metadata in OME format tree
 
     priority = 99
     do_not_pickle = 'base', 'copies', 'cache'
     do_not_copy = 'extrametadata'
+    ureg = ureg
 
     @staticmethod
     @abstractmethod
     def _can_open(path):  # Override this method, and return true when the subclass can open the file
         return False
 
     @abstractmethod
-    def __metadata__(self):
-        return
-
-    @abstractmethod
     def __frame__(self, c, z, t):  # Override this, return the frame at c, z, t
         return np.random.randint(0, 255, self.shape['xy'])
 
+    @cached_property
+    def ome(self):
+        return self.get_ome(self.path)
+
     def open(self):  # Optionally override this, open file handles etc.
         """ filehandles cannot be pickled and should be marked such by setting do_not_pickle = 'file_handle_name' """
         return
 
     def close(self):  # Optionally override this, close file handles etc.
         return
 
+    @staticmethod
+    def get_ome(path):
+        """ Use java BioFormats to make an ome metadata structure. """
+        with multiprocessing.get_context('spawn').Pool(1) as pool:
+            ome = pool.map(ome_subprocess, (path,))[0]
+            return ome
+
     def __new__(cls, path=None, *args, **kwargs):
         if cls is not Imread:
             return super().__new__(cls)
         if len(cls.__subclasses__()) == 0:
             raise Exception('Restart python kernel please!')
         if isinstance(path, Imread):
             return path
-        for subclass in sorted(cls.__subclasses__(), key=lambda subclass: subclass.priority):
+        path, _ = Imread.split_path_series(path)
+        for subclass in sorted(cls.__subclasses__(), key=lambda subclass_: subclass_.priority):
             if subclass._can_open(path):
                 do_not_pickle = (cls.do_not_pickle,) if isinstance(cls.do_not_pickle, str) else cls.do_not_pickle
                 subclass_do_not_pickle = (subclass.do_not_pickle,) if isinstance(subclass.do_not_pickle, str) \
                     else subclass.do_not_pickle if hasattr(subclass, 'do_not_pickle') else ()
                 subclass.do_not_pickle = set(do_not_pickle).union(set(subclass_do_not_pickle))
 
                 do_not_copy = (cls.do_not_copy,) if isinstance(cls.do_not_copy, str) else cls.do_not_copy
                 subclass_do_not_copy = (subclass.do_not_copy,) if isinstance(subclass.do_not_copy, str) \
                     else subclass.do_not_copy if hasattr(subclass, 'do_not_copy') else ()
                 subclass.do_not_copy = set(do_not_copy).union(set(subclass_do_not_copy))
 
                 return super().__new__(subclass)
 
-    def __init__(self, path, series=0, transform=False, drift=False, beadfile=None, sigma=None, dtype=None,
-                 axes='cztxy'):
+    @staticmethod
+    def split_path_series(path):
+        if isinstance(path, str):
+            path = Path(path)
+        if isinstance(path, Path) and path.name.startswith('Pos'):
+            return path.parent, int(path.name.lstrip('Pos'))
+        return path, 0
+
+    def __init__(self, path, transform=False, drift=False, beadfile=None, dtype=None, axes=None):
         if isinstance(path, Imread):
             return
         self.isclosed = False
         self._shape = Shape((0, 0, 0, 0, 0))
         self.base = None
         self.copies = []
         if isinstance(path, str):
-            self.path = os.path.abspath(path)
-            self.title = os.path.splitext(os.path.basename(self.path))[0]
-            self.acquisitiondate = datetime.fromtimestamp(os.path.getmtime(self.path)).strftime('%y-%m-%dT%H:%M:%S')
-        else:
-            self.path = path  # ndarray
+            path = Path(path)
+        self.path, self.series = self.split_path_series(path)
+        if isinstance(path, Path):
+            self.title = self.path.name
+            self.acquisitiondate = datetime.fromtimestamp(self.path.stat().st_mtime).strftime('%y-%m-%dT%H:%M:%S')
+        else:  # ndarray
+            self.title = 'ndarray'
+            self.acquisitiondate = 'now'
         self.transform = transform
         self.drift = drift
         self.beadfile = beadfile
         self.dtype = dtype
-        self.series = series
-        self.pxsize = 1e-1
-        self.settimeinterval = 0
-        self.pxsizecam = 0
-        self.magnification = 0
-        self.exposuretime = (0,)
-        self.deltaz = 1
-        self.pcf = (1, 1)
-        self.laserwavelengths = [[]]
-        self.laserpowers = [[]]
-        self.powermode = 'normal'
-        self.optovar = (1,)
-        self.binning = 1
-        self.collimator = (1,)
-        self.tirfangle = (0,)
-        self.gain = (100, 100)
-        self.objective = 'unknown'
-        self.filter = 'unknown'
-        self.NA = 1
+        self.reader = None
+
+        self.pcf = None
+        self.powermode = None
+        self.collimator = None
+        self.tirfangle = None
         self.cyllens = ['None', 'None']
         self.duolink = 'None'
         self.detector = [0, 1]
         self.track = [0]
-        self.metadata = {}
         self.cache = DequeDict(16)
         self._frame_decorator = None
         self.frameoffset = 0, 0  # how far apart the centers of frame and sensor are
 
         self.open()
-        self.__metadata__()
+
+        # extract some metadata from ome
+        instrument = self.ome.instruments[0]
+        image = self.ome.images[0]
+        pixels = image.pixels
+        self.shape = pixels.size_x, pixels.size_y, pixels.size_c, pixels.size_z, pixels.size_t
+        self.pxsize = pixels.physical_size_x_quantity
+        self.exposuretime = tuple(find(image.pixels.planes, the_c=c).exposure_time_quantity
+                                  for c in range(self.shape['c']))
+        if self.zstack:
+            self.deltaz = image.pixels.physical_size_z_quantity
+            self.deltaz_um = None if self.deltaz is None else self.deltaz.to(self.ureg.um).m
+        else:
+            self.deltaz = self.deltaz_um = None
+        if self.ome.images[0].objective_settings:
+            self.objective = find(instrument.objectives, id=self.ome.images[0].objective_settings.id)
+        else:
+            self.objective = None
+        self.timeval = [find(image.pixels.planes, the_c=0, the_t=t, the_z=0).delta_t for t in range(self.shape['t'])]
+        self.timeinterval = np.diff(self.timeval).mean() if len(self.timeval) > 1 else 0
+        try:
+            self.binning = [int(i) for i in image.pixels.channels[0].detector_settings.binning.value.split('x')]
+        except (Exception,):
+            self.binning = None
+        self.cnamelist = [channel.name for channel in image.pixels.channels]
+        optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
+        if len(optovars) == 0:
+            self.tubelens = None
+        else:
+            self.tubelens = optovars[0]
+        if self.objective:
+            if self.tubelens:
+                self.magnification = self.objective.nominal_magnification * self.tubelens.nominal_magnification
+            else:
+                self.magnification = self.objective.nominal_magnification
+            self.NA = self.objective.lens_na
+        else:
+            self.magnification = None
+            self.NA = None
+
+        self.gain = [find(instrument.detectors, id=channel.detector_settings.id).amplification_gain
+                     for channel in image.pixels.channels
+                     if channel.detector_settings
+                     and find(instrument.detectors, id=channel.detector_settings.id).amplification_gain]
+        self.laserwavelengths = [(channel.emission_wavelength_quantity.to(self.ureg.nm).m,)
+                                 for channel in pixels.channels if channel.emission_wavelength_quantity]
+        self.laserpowers = try_default(lambda channel: [(1 - channel.light_source_settings.attenuation,)
+                                                        for channel in pixels.channels], [])
+        self.filter = try_default(lambda: [find(instrument.filter_sets, id=channel.filter_set_ref.id).model
+                                           for channel in image.pixels.channels], None)
+        self.pxsize_um = None if self.pxsize is None else self.pxsize.to(self.ureg.um).m
+        self.exposuretime_s = [None if i is None else i.to(self.ureg.s).m for i in self.exposuretime]
         self.file_shape = self.shape.xyczt
 
-        if axes.lower() == 'squeeze':
+        if axes is None:
             self.axes = ''.join(i for i in 'cztxy' if self.shape[i] > 1)
         elif axes.lower() == 'full':
             self.axes = 'cztxy'
         else:
             self.axes = axes
         self.slice = [np.arange(s, dtype=int) for s in self.shape.xyczt]
 
-        if not hasattr(self, 'cnamelist'):
-            self.cnamelist = 'abcdefghijklmnopqrstuvwxyz'[:self.shape['c']]
-
         m = self.extrametadata
         if m is not None:
             try:
                 self.cyllens = m['CylLens']
                 self.duolink = m['DLFilterSet'].split(' & ')[m['DLFilterChannel']]
                 if 'FeedbackChannels' in m:
                     self.feedback = m['FeedbackChannels']
                 else:
                     self.feedback = m['FeedbackChannel']
-            except Exception:
+            except (Exception,):
                 self.cyllens = ['None', 'None']
                 self.duolink = 'None'
                 self.feedback = []
         try:
             self.cyllenschannels = np.where([self.cyllens[self.detector[c]].lower() != 'none'
                                              for c in range(self.shape['c'])])[0].tolist()
-        except Exception:
+        except (Exception,):
             pass
         self.set_transform()
         try:
-            s = int(re.findall(r'_(\d{3})_', self.duolink)[0])
-        except Exception:
-            s = 561
-        if sigma is None:
-            try:
-                sigma = []
-                for t, d in zip(self.track, self.detector):
-                    l = np.array(self.laserwavelengths[t]) + 22
-                    sigma.append([l[l > s].max(initial=0), l[l < s].max(initial=0)][d])
-                sigma = np.array(sigma)
-                sigma[sigma == 0] = 600
-                sigma /= 2 * self.NA * self.pxsize * 1000
-                self.sigma = sigma.tolist()
-            except Exception:
-                self.sigma = [2] * self.shape['c']
-        else:
-            self.sigma = sigma
-        if 1.5 < self.NA:
+            s = int(re.findall(r'_(\d{3})_', self.duolink)[0]) * ureg.nm
+        except (Exception,):
+            s = 561 * ureg.nm
+        try:
+            sigma = []
+            for c, d in enumerate(self.detector):
+                emission = np.hstack(self.laserwavelengths[c]) + 22 * ureg.nm
+                sigma.append([emission[emission > s].max(initial=0), emission[emission < s].max(initial=0)][d])
+            sigma = np.hstack(sigma)
+            sigma[sigma == 0] = 600 * ureg.nm
+            sigma /= 2 * self.NA * self.pxsize
+            self.sigma = sigma.magnitude.tolist()
+        except (Exception,):
+            self.sigma = [2] * self.shape['c']
+        if not self.NA:
+            self.immersionN = 1
+        elif 1.5 < self.NA:
             self.immersionN = 1.661
         elif 1.3 < self.NA < 1.5:
             self.immersionN = 1.518
         elif 1 < self.NA < 1.3:
             self.immersionN = 1.33
         else:
             self.immersionN = 1
@@ -707,17 +637,17 @@
         if self.transform is False or self.transform is None:
             self.transform = None
         else:
             if isinstance(self.transform, Transforms):
                 self.transform = self.transform
             else:
                 if isinstance(self.transform, str):
-                    self.transform = ImTransforms(self.path, self.cyllens, self.track, self.detector, self.transform)
+                    self.transform = ImTransforms(self.path, self.cyllens, self.transform)
                 else:
-                    self.transform = ImTransforms(self.path, self.cyllens, self.track, self.detector, self.beadfile)
+                    self.transform = ImTransforms(self.path, self.cyllens, self.beadfile)
                 if self.drift is True:
                     self.transform = ImShiftTransforms(self)
                 elif not (self.drift is False or self.drift is None):
                     self.transform = ImShiftTransforms(self, self.drift)
             self.transform.adapt(self.frameoffset, self.shape.xyczt)
             self.beadfile = self.transform.files
 
@@ -730,16 +660,15 @@
         new_kwargs = {key: value for key, value in zip(inspect.getfullargspec(c).args[1:], a)}
         for key, value in kwargs.items():
             new_kwargs[key] = value
         return c(**new_kwargs)
 
     @staticmethod
     def get_config(file):
-        """ Open a yml parameter file
-        """
+        """ Open a yml config file """
         loader = yaml.SafeLoader
         loader.add_implicit_resolver(
             r'tag:yaml.org,2002:float',
             re.compile(r'''^(?:
              [-+]?(?:[0-9][0-9_]*)\.[0-9_]*(?:[eE][-+]?[0-9]+)?
             |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
             |\.[0-9_]+(?:[eE][-+][0-9]+)?
@@ -759,93 +688,92 @@
         return self._frame_decorator
 
     @frame_decorator.setter
     def frame_decorator(self, decorator):
         self._frame_decorator = decorator
         self.cache = DequeDict(self.cache.maxlen)
 
-    def __repr__(self):
-        """ gives a helpful summary of the recorded experiment
-        """
-        s = [100 * '#']
-        s.append('path/filename: {}'.format(self.path))
-        s.append('shape ({}): '.format(self.axes) + ' ' * (5 - self.ndim) +
-                 ' x '.join(('{}',) * self.ndim).format(*self.shape))
-        s.append('pixelsize:     {:.2f} nm'.format(self.pxsize * 1000))
-        if self.zstack:
-            s.append('z-interval:    {:.2f} nm'.format(self.deltaz * 1000))
-        s.append('Exposuretime:  ' + ('{:.2f} ' * len(self.exposuretime)).format(
-            *(np.array(self.exposuretime) * 1000)) + 'ms')
-        if self.timeseries:
-            if self.timeval and np.diff(self.timeval).shape[0]:
-                s.append('t-interval:    {:.3f} ± {:.3f} s'.format(
-                    np.diff(self.timeval).mean(), np.diff(self.timeval).std()))
-            else:
-                s.append('t-interval:    {:.2f} s'.format(self.settimeinterval))
-        s.append('binning:       {}x{}'.format(self.binning, self.binning))
-        s.append('laser colors:  ' + ' | '.join([' & '.join(len(l)*('{:.0f}',)).format(*l)
-                                                 for l in self.laserwavelengths]) + ' nm')
-        s.append('laser powers:  ' + ' | '.join([' & '.join(len(l)*('{}',)).format(*[100 * i for i in l])
-                                                 for l in self.laserpowers]) + ' %')
-        s.append('objective:     {}'.format(self.objective))
-        s.append('magnification: {}x'.format(self.magnification))
-        s.append('optovar:      ' + (' {}' * len(self.optovar)).format(*self.optovar) + 'x')
-        s.append('filterset:     {}'.format(self.filter))
-        s.append('powermode:     {}'.format(self.powermode))
-        s.append('collimator:   ' + (' {}' * len(self.collimator)).format(*self.collimator))
-        s.append('TIRF angle:   ' + (' {:.2f}°' * len(self.tirfangle)).format(*self.tirfangle))
-        s.append('gain:         ' + (' {:.0f}' * len(self.gain)).format(*self.gain))
-        s.append('pcf:          ' + (' {:.2f}' * len(self.pcf)).format(*self.pcf))
+    @property
+    def summary(self):
+        """ gives a helpful summary of the recorded experiment """
+        s = [f"path/filename: {self.path}",
+             f"reader:        {self.__class__.__module__.split('.')[-1]}",
+             f"shape ({self.axes}):".ljust(15) + f"{' x '.join(str(i) for i in self.shape)}"]
+        if self.pxsize_um:
+            s.append(f'pixel size:    {1000 * self.pxsize_um:.2f} nm')
+        if self.zstack and self.deltaz_um:
+            s.append(f'z-interval:    {1000 * self.deltaz_um:.2f} nm')
+        if self.exposuretime_s[0]:
+            s.append(f'exposuretime:  {self.exposuretime_s[0]:.2f} s')
+        if self.timeseries and self.timeinterval:
+            s.append(f'time interval: {self.timeinterval:.3f} s')
+        if self.binning:
+            s.append('binning:       {}x{}'.format(*self.binning))
+        if self.laserwavelengths:
+            s.append('laser colors:  ' + ' | '.join([' & '.join(len(w)*('{:.0f}',)).format(*w)
+                                                     for w in self.laserwavelengths]) + ' nm')
+        if self.laserpowers:
+            s.append('laser powers:  ' + ' | '.join([' & '.join(len(p)*('{:.3g}',)).format(*[100 * i for i in p])
+                                                     for p in self.laserpowers]) + ' %')
+        if self.objective:
+            s.append('objective:     {}'.format(self.objective.model))
+        if self.magnification:
+            s.append('magnification: {}x'.format(self.magnification))
+        if self.tubelens:
+            s.append('tubelens:      {}'.format(self.tubelens.model))
+        if self.filter:
+            s.append('filterset:     {}'.format(self.filter))
+        if self.powermode:
+            s.append('powermode:     {}'.format(self.powermode))
+        if self.collimator:
+            s.append('collimator:   ' + (' {}' * len(self.collimator)).format(*self.collimator))
+        if self.tirfangle:
+            s.append('TIRF angle:   ' + (' {:.2f}°' * len(self.tirfangle)).format(*self.tirfangle))
+        if self.gain:
+            s.append('gain:         ' + (' {:.0f}' * len(self.gain)).format(*self.gain))
+        if self.pcf:
+            s.append('pcf:          ' + (' {:.2f}' * len(self.pcf)).format(*self.pcf))
         return '\n'.join(s)
 
     def __str__(self):
-        return self.path
+        return str(self.path)
 
     def __len__(self):
         return self.shape[0]
 
-    def __call__(self, *n):
-        """ returns single 2D frame
-            im(n):     index linearly in czt order
-            im(c,z):   return im(c,z,t=0)
-            im(c,z,t): return im(c,z,t)
-        """
-        if len(n) == 1:
-            n = self.get_channel(n[0])
-            c = int(n % self.shape['c'])
-            z = int((n // self.shape['c']) % self.shape['z'])
-            t = int((n // (self.shape['c'] * self.shape['z'])) % self.shape['t'])
-            return self.frame(c, z, t)
-        else:
-            return self.frame(*[int(i) for i in n])
+    def __call__(self, c=None, z=None, t=None, x=None, y=None):
+        """ same as im[] but allowing keyword axes, but slices need to made with slice() or np.s_ """
+        return self[{k: slice(v) if v is None else v for k, v in dict(c=c, z=z, t=t, x=x, y=y).items()}]
 
     def __getitem__(self, n):
-        # None = :
-        if isinstance(n, (slice, Number)):
+        """ slice like a numpy array but return an Imread instance """
+        if isinstance(n, (slice, Number)):  # None = :
             n = (n,)
         elif isinstance(n, type(Ellipsis)):
             n = (None,) * len(self.axes)
+        elif isinstance(n, dict):  # allow im[dict(z=0)] etc.
+            n = [n.get(i, slice(None)) for i in self.axes]
         n = list(n)
 
         # deal with ...
         ell = [i for i, e in enumerate(n) if isinstance(e, type(Ellipsis))]
         if len(ell) > 1:
-            raise IndexError("an index can only have a single ellipsis (...)")
+            raise IndexError('an index can only have a single ellipsis (...)')
         if len(ell):
             if len(n) > self.ndim:
                 n.remove(Ellipsis)
             else:
                 n[ell[0]] = None
                 while len(n) < self.ndim:
                     n.insert(ell[0], None)
         while len(n) < self.ndim:
             n.append(None)
 
-        T = [self.shape.axes.find(i) for i in 'xyczt']
-        n = [n[j] if 0 <= j < len(n) else None for j in T]  # reorder n
+        axes_idx = [self.shape.axes.find(i) for i in 'xyczt']
+        n = [n[j] if 0 <= j < len(n) else None for j in axes_idx]  # reorder n
 
         new_slice = []
         for s, e in zip(self.slice, n):
             if e is None:
                 new_slice.append(s)
             else:
                 new_slice.append(s[e])
@@ -858,39 +786,39 @@
             new.slice = new_slice
             new._shape = Shape([1 if isinstance(s, Number) else len(s) for s in new_slice])
             new.axes = ''.join(j for j in self.axes if j in [i for i, s in zip('xyczt', new_slice)
                                                              if not isinstance(s, Number)])
             return new
 
     def __contains__(self, item):
-        def unique_yield(l, i):
-            for k in l:
+        def unique_yield(a, b):
+            for k in a:
                 yield k
-            for k in i:
-                if k not in l:
+            for k in b:
+                if k not in a:
                     yield k
         for idx in unique_yield(list(self.cache.keys()),
                                 product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t']))):
             xyczt = (slice(None), slice(None)) + idx
             in_idx = tuple(xyczt['xyczt'.find(i)] for i in self.axes)
             if item in np.asarray(self[in_idx]):
                 return True
         return False
 
     def __array__(self, dtype=None):
         block = self.block(*self.slice)
-        T = [self.shape.axes.find(i) for i in 'xyczt']
-        S = tuple({i for i, j in enumerate(T) if j == -1}.union(
+        axes_idx = [self.shape.axes.find(i) for i in 'xyczt']
+        axes_squeeze = tuple({i for i, j in enumerate(axes_idx) if j == -1}.union(
             {i for i, j in enumerate(self.slice) if isinstance(j, Number)}))
-        block = block.squeeze(S)
+        block = block.squeeze(axes_squeeze)
         if dtype is not None:
             block = block.astype(dtype)
         if block.ndim == 0:
             return block.item()
-        axes = ''.join(j for i, j in enumerate('xyczt') if i not in S)
+        axes = ''.join(j for i, j in enumerate('xyczt') if i not in axes_squeeze)
         return block.transpose([axes.find(i) for i in self.shape.axes if i in axes])
 
     def asarray(self):
         return self.__array__()
 
     def astype(self, dtype):
         new = self.copy()
@@ -921,15 +849,15 @@
     def __setstate__(self, state):
         """ What happens during unpickling """
         self.__dict__.update(state)
         self.open()
         self.copies = []
         self.cache = DequeDict(16)
 
-    # TODO: this is causing problems when multiprocessing
+    # TODO: this is causing problems when multiprocessing and doesn't work anyway
     # def __del__(self):
     #     if not self.copies:
     #         if self.base is None:
     #             self.__exit__()
     #         else:
     #             self.base.copies.remove(self)
 
@@ -937,15 +865,15 @@
         return self.copy()
 
     def copy(self):
         new = Imread.__new__(self.__class__)
         new.copies = []
         new.base = self
         for key, value in self.__dict__.items():
-            if not key in self.do_not_copy and not hasattr(new, key):
+            if key not in self.do_not_copy and not hasattr(new, key):
                 new.__dict__[key] = value
         self.copies.append(new)
         return new
 
     @property
     def shape(self):
         return self._shape
@@ -1004,54 +932,19 @@
         axes[axis1], axes[axis2] = axes[axis2], axes[axis1]
         new.axes = axes
         return new
 
     def moveaxis(self, source, destination):
         raise NotImplementedError('moveaxis it not implemented')
 
-    def czt(self, n):
-        """ returns indices c, z, t used when calling im(n)
-        """
-        if not isinstance(n, tuple):
-            c = n % self.shape['c']
-            z = (n // self.shape['c']) % self.shape['z']
-            t = (n // (self.shape['c'] * self.shape['z'])) % self.shape['t']
-            return c, z, t
-        n = list(n)
-        if len(n) == 2 or len(n) == 4:
-            n.append(slice(0, -1, 1))
-        if len(n) == 3:
-            n = list(n)
-            for i, (ax, e) in enumerate(zip('czt', n)):
-                if isinstance(e, slice):
-                    a = [e.start, e.stop, e.step]
-                    if a[0] is None:
-                        a[0] = 0
-                    if a[1] is None:
-                        a[1] = -1
-                    if a[2] is None:
-                        a[2] = 1
-                    for j in range(2):
-                        if a[j] < 0:
-                            a[j] %= self.shape[ax]
-                            a[j] += 1
-                    n[i] = np.arange(*a)
-            n = [np.array(i) for i in n]
-            return tuple(n)
-        if len(n) == 5:
-            return tuple(n[2:5])
-
-    def czt2n(self, c, z, t):
-        return c + z * self.shape['c'] + t * self.shape['c'] * self.shape['z']
-
     def transform_frame(self, frame, c, t=0):
         if self.transform is None:
             return frame
         else:
-            return self.transform(c, t, self.track, self.detector).frame(frame)
+            return self.transform[(self.cnamelist[c],)].frame(frame)
 
     def get_czt(self, c, z, t):
         czt = []
         for i, n in zip('czt', (c, z, t)):
             if n is None:
                 czt.append(list(range(self.shape[i])))
             elif isinstance(n, range):
@@ -1064,43 +957,14 @@
                 czt.append(list(range(n.start % self.shape[i], stop, n.step)))
             elif isinstance(n, Number):
                 czt.append([n % self.shape[i]])
             else:
                 czt.append([k % self.shape[i] for k in n])
         return [self.get_channel(c) for c in czt[0]], *czt[1:]
 
-    def _stats(self, fun, c=None, z=None, t=None, ffun=None):
-        """ fun = np.min, np.max, np.sum or their nan varieties """
-        warn('Warning: _stats is deprecated.')
-        c, z, t = self.get_czt(c, z, t)
-        if fun in (np.min, np.nanmin):
-            val = np.inf
-        elif fun in (np.max, np.nanmax):
-            val = -np.inf
-        else:
-            val = 0
-        if ffun is None:
-            ffun = lambda im: im
-        T = np.full(self.shape['xy'], val, self.dtype)
-        for ic in c:
-            m = np.full(self.shape['xy'], val, self.dtype)
-            if isinstance(self.transform, ImShiftTransforms):
-                for it in t:
-                    n = np.full(self.shape['xy'], val, self.dtype)
-                    for iz in z:
-                        n = fun((n, ffun(self.__frame__(ic, iz, it))), 0)
-                    m = self.transform_frame(n, ic, it)
-            else:
-                for it, iz in product(t, z):
-                    m = fun((m, ffun(self.__frame__(ic, iz, it))), 0)
-                if isinstance(self.transform, ImTransforms):
-                    m = self.transform_frame(m, ic, 0)
-            T = fun((T, m), 0)
-        return T
-
     @staticmethod
     def __array_arg_fun__(self, fun, axis=None, out=None):
         """ frame-wise application of np.argmin and np.argmax """
         if axis is None:
             value = arg = None
             for idx in product(range(self.shape['c']), range(self.shape['z']), range(self.shape['t'])):
                 xyczt = (slice(None), slice(None)) + idx
@@ -1163,17 +1027,18 @@
     def argmin(self, *args, **kwargs):
         return Imread.__array_arg_fun__(self, np.argmin, *args, **kwargs)
 
     def argmax(self, *args, **kwargs):
         return Imread.__array_arg_fun__(self, np.argmax, *args, **kwargs)
 
     def __array_fun__(self, fun, axis=None, dtype=None, out=None, keepdims=False, initial=None, where=True, ffun=None):
-        """ frame-wise application of np.min, np.max, np.sum, np.mean and theis nan equivalents """
+        """ frame-wise application of np.min, np.max, np.sum, np.mean and their nan equivalents """
         if ffun is None:
-            ffun = lambda im: im
+            def ffun(im):
+                return im
         if dtype is None:
             dtype = self.dtype if out is None else out.dtype
 
         # TODO: smarter transforms
         if where is not True:
             raise NotImplementedError('Argument where != True is not implemented.')
         if axis is None:
@@ -1271,20 +1136,21 @@
             else:
                 res /= self.sum(axis, None, keepdims=keepdims, where=where, ffun=lambda x: np.invert(np.isnan(x)))
             return res.astype(out.dtype, copy=False)
 
     def reshape(self, *args, **kwargs):
         return np.asarray(self).reshape(*args, **kwargs)
 
-    @property
-    def is_noise(self):
+    def is_noise(self, volume=None):
         """ True if volume only has noise """
-        F = np.fft.fftn(self)
-        S = np.fft.fftshift(np.fft.ifftn(F * F.conj()).real / np.sum(self ** 2))
-        return -np.log(1 - S[tuple([0] * S.ndim)]) > 5
+        if volume is None:
+            volume = self
+        fft = np.fft.fftn(volume)
+        corr = np.fft.fftshift(np.fft.ifftn(fft * fft.conj()).real / np.sum(volume ** 2))
+        return -np.log(1 - corr[tuple([0] * corr.ndim)]) > 5
 
     @property
     def dtype(self):
         return self._dtype
 
     @dtype.setter
     def dtype(self, value):
@@ -1296,16 +1162,15 @@
         else:
             c = [i for i, c in enumerate(self.cnamelist) if c.lower().startswith(channel_name.lower())]
             assert len(c) > 0, 'Channel {} not found in {}'.format(c, self.cnamelist)
             assert len(c) < 2, 'Channel {} not unique in {}'.format(c, self.cnamelist)
             return c[0]
 
     def frame(self, c=0, z=0, t=0):
-        """ returns single 2D frame
-        """
+        """ returns single 2D frame """
         c = self.get_channel(c)
         c %= self.file_shape[2]
         z %= self.file_shape[3]
         t %= self.file_shape[4]
 
         # cache last n (default 16) frames in memory for speed (~250x faster)
         if (c, z, t) in self.cache:
@@ -1318,47 +1183,30 @@
             self.cache[(c, z, t)] = f
         if self.dtype is not None:
             return f.copy().astype(self.dtype)
         else:
             return f.copy()
 
     def data(self, c=0, z=0, t=0):
-        """ returns 3D stack of frames
-        """
+        """ returns 3D stack of frames """
         c, z, t = [np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1) for i, e in zip('czt', (c, z, t))]
         return np.dstack([self.frame(ci, zi, ti) for ci, zi, ti in product(c, z, t)])
 
     def block(self, x=None, y=None, c=None, z=None, t=None):
-        """ returns 5D block of frames
-        """
+        """ returns 5D block of frames """
         x, y, c, z, t = [np.arange(self.shape[i]) if e is None else np.array(e, ndmin=1)
                          for i, e in zip('xyczt', (x, y, c, z, t))]
         d = np.full((len(x), len(y), len(c), len(z), len(t)), np.nan, self.dtype)
         for (ci, cj), (zi, zj), (ti, tj) in product(enumerate(c), enumerate(z), enumerate(t)):
             d[:, :, ci, zi, ti] = self.frame(cj, zj, tj)[x][:, y]
         return d
 
     @cached_property
-    def timeval(self):
-        if hasattr(self, 'metadata') and isinstance(self.metadata, XmlData):
-            image = self.metadata.search('Image')
-            if (isinstance(image, dict) and self.series in image) or (isinstance(image, list) and len(image)):
-                image = XmlData(image[0])
-            return sorted(np.unique(image.search_all('DeltaT').values()))[:self.shape['t']]
-        else:
-            return (np.arange(self.shape['t']) * self.settimeinterval).tolist()
-
-    @cached_property
-    def timeinterval(self):
-        return float(np.diff(self.timeval).mean()) if len(self.timeval) > 1 else 1
-
-    @cached_property
     def piezoval(self):
-        """ gives the height of the piezo and focus motor, only available when CylLensGUI was used
-        """
+        """ gives the height of the piezo and focus motor, only available when CylLensGUI was used """
         def upack(idx):
             time = list()
             val = list()
             if len(idx) == 0:
                 return time, val
             for i in idx:
                 time.append(int(re.search(r'\d+', n[i]).group(0)))
@@ -1403,87 +1251,83 @@
 
         # remove duplicates
         df = df[~df.duplicated('frame', 'last')]
         return df
 
     @cached_property
     def extrametadata(self):
-        if isinstance(self.path, str) and len(self.path) > 3:
-            if os.path.isfile(self.path[:-3] + 'pzl2'):
-                pname = self.path[:-3] + 'pzl2'
-            elif os.path.isfile(self.path[:-3] + 'pzl'):
-                pname = self.path[:-3] + 'pzl'
+        if isinstance(self.path, Path):
+            if self.path.with_suffix('.pzl2').exists():
+                pname = self.path.with_suffix('.pzl2')
+            elif self.path.with_suffix('.pzl').exists():
+                pname = self.path.with_suffix('.pzl')
             else:
                 return
             try:
                 return self.get_config(pname)
-            except Exception:
+            except (Exception,):
                 return
         return
 
     def save_as_tiff(self, fname=None, c=None, z=None, t=None, split=False, bar=True, pixel_type='uint16'):
         """ saves the image as a tiff-file
-            split: split channels into different files
-        """
+            split: split channels into different files """
         if fname is None:
-            if isinstance(self.path, str):
-                fname = self.path[:-3] + 'tif'
-            else:
-                raise Exception('No filename given.')
-        elif not fname[-3:] == 'tif':
-            fname += '.tif'
+            fname = self.path.with_suffix('.tif')
+            if fname == self.path:
+                raise FileExistsError(f'File {fname} exists already.')
+        if not isinstance(fname, Path):
+            fname = Path(fname)
         if split:
             for i in range(self.shape['c']):
                 if self.timeseries:
-                    self.save_as_tiff(fname[:-3] + '_C{:01d}.tif'.format(i), i, 0, None, False, bar, pixel_type)
+                    self.save_as_tiff(fname.with_name(f'{fname.stem}_C{i:01d}').with_suffix('.tif'), i, 0, None, False,
+                                      bar, pixel_type)
                 else:
-                    self.save_as_tiff(fname[:-3] + '_C{:01d}.tif'.format(i), i, None, 0, False, bar, pixel_type)
+                    self.save_as_tiff(fname.with_name(f'{fname.stem}_C{i:01d}').with_suffix('.tif'), i, None, 0, False,
+                                      bar, pixel_type)
         else:
             n = [c, z, t]
             for i, ax in enumerate('czt'):
                 if n[i] is None:
                     n[i] = range(self.shape[ax])
                 elif not isinstance(n[i], (tuple, list)):
                     n[i] = (n[i],)
 
             shape = [len(i) for i in n]
             at_least_one = False
-            with IJTiffFile(fname, shape, pixel_type, pxsize=self.pxsize, deltaz=self.deltaz) as tif:
+            with IJTiffFile(fname.with_suffix('.tif'), shape, pixel_type,
+                            pxsize=self.pxsize_um, deltaz=self.deltaz_um) as tif:
                 for i, m in tqdm(zip(product(*[range(s) for s in shape]), product(*n)),
                                  total=np.prod(shape), desc='Saving tiff', disable=not bar):
                     if np.any(self(*m)) or not at_least_one:
                         tif.save(self(*m), *i)
                         at_least_one = True
 
-    @cached_property
-    def summary(self):
-        return self.__repr__()
+    def __repr__(self):
+        return self.summary
 
 
 def main():
     parser = ArgumentParser(description='Display info and save as tif')
     parser.add_argument('file', help='image_file')
     parser.add_argument('out', help='path to tif out', type=str, default=None, nargs='?')
     parser.add_argument('-r', '--register', help='register channels', action='store_true')
     parser.add_argument('-c', '--channel', help='channel', type=int, default=None)
     parser.add_argument('-z', '--zslice', help='z-slice', type=int, default=None)
     parser.add_argument('-t', '--time', help='time', type=int, default=None)
     parser.add_argument('-s', '--split', help='split channels', action='store_true')
     parser.add_argument('-f', '--force', help='force overwrite', action='store_true')
     args = parser.parse_args()
 
-    if os.path.exists(args.file):
-        with Imread(args.file, transform=args.register) as im:
-            print(im.summary)
-            if args.out:
-                out = os.path.abspath(args.out)
-                if not os.path.exists(os.path.dirname(out)):
-                    os.makedirs(os.path.dirname(out))
-                if os.path.exists(out) and not args.force:
-                    print('File {} exists already, add the -f flag if you want to overwrite it.'.format(args.out))
-                else:
-                    im.save_as_tiff(out, args.channel, args.zslice, args.time, args.split)
-    else:
-        print('File does not exist.')
+    with Imread(args.file, transform=args.register) as im:
+        print(im.summary)
+        if args.out:
+            out = Path(args.out).absolute()
+            out.parent.mkdir(parents=True, exist_ok=True)
+            if out.exists() and not args.force:
+                print('File {} exists already, add the -f flag if you want to overwrite it.'.format(args.out))
+            else:
+                im.save_as_tiff(out, args.channel, args.zslice, args.time, args.split)
 
 
 from ndbioimage.readers import *
```

### Comparing `ndbioimage-2022.7.1/ndbioimage/transforms.py` & `ndbioimage-2023.6.1/ndbioimage/ntransforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,38 @@
 import yaml
-import os
 import numpy as np
 from copy import deepcopy
-from collections import OrderedDict
+from numbers import Number
+from pathlib import Path
 
 try:
     # best if SimpleElastix is installed: https://simpleelastix.readthedocs.io/GettingStarted.html
     import SimpleITK as sitk
     installed = True
 except ImportError:
     installed = False
 
 try:
     pp = True
     from pandas import DataFrame, Series
 except ImportError:
     pp = False
 
-
 if hasattr(yaml, 'full_load'):
     yamlload = yaml.full_load
 else:
     yamlload = yaml.load
 
 
-class Transforms(OrderedDict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args[1:], **kwargs)
-        if len(args):
-            self.load(args[0])
-
-    def asdict(self):
-        return {f'{key[0]:.0f}:{key[1]:.0f}': value.asdict() for key, value in self.items()}
-
-    def load(self, file):
-        if isinstance(file, dict):
-            d = file
-        else:
-            if not file[-3:] == 'yml':
-                file += '.yml'
-            with open(file, 'r') as f:
-                d = yamlload(f)
-        for key, value in d.items():
-            self[tuple([int(k) for k in key.split(':')])] = Transform(value)
-
-    def __call__(self, channel, time, tracks, detectors):
-        track, detector = tracks[channel], detectors[channel]
-        if (track, detector) in self:
-            return self[track, detector]
-        elif (0, detector) in self:
-            return self[0, detector]
-        else:
-            return Transform()
-
-    def __reduce__(self):
-        return self.__class__, (self.asdict(),)
-
-    def save(self, file):
-        if not file[-3:] == 'yml':
-            file += '.yml'
-        with open(file, 'w') as f:
-            yaml.safe_dump(self.asdict(), f, default_flow_style=None)
-
-    def copy(self):
-        return deepcopy(self)
-
-    def adapt(self, origin, shape):
-        for value in self.values():
-            value.adapt(origin, shape)
-
-    @property
-    def inverse(self):
-        inverse = self.copy()
-        for key, value in self.items():
-            inverse[key] = value.inverse
-        return inverse
-
-
 class Transform:
     def __init__(self, *args):
         if not installed:
-            raise ImportError('SimpleElastix is not installed: https://simpleelastix.readthedocs.io/GettingStarted.html')
-        self.transform = sitk.ReadTransform(os.path.join(os.path.dirname(__file__), 'transform.txt'))
+            raise ImportError('SimpleElastix is not installed:'
+                              ' https://simpleelastix.readthedocs.io/GettingStarted.html')
+        self.transform = sitk.ReadTransform(str(Path(__file__).parent / 'transform.txt'))
         self.dparameters = (0, 0, 0, 0, 0, 0)
         self.shape = (512, 512)
         self.origin = (255.5, 255.5)
         if len(args) == 1:  # load from file or dict
             if isinstance(args[0], np.ndarray):
                 self.matrix = args[0]
             else:
@@ -253,9 +200,44 @@
             self.shape = [float(t) for t in transform['Size']]
             self.origin = [float(t) for t in transform['CenterOfRotationPoint']]
         elif kind == 'translation':
             self.parameters = [1.0, 0.0, 0.0, 1.0] + [float(t) for t in transform['TransformParameters']]
             self.shape = [float(t) for t in transform['Size']]
             self.origin = [(t - 1) / 2 for t in self.shape]
         else:
-            raise NotImplementedError(f'{kind} tranforms not implemented (yet)')
+            raise NotImplementedError(f'{kind} transforms not implemented (yet)')
         self.dparameters = 6 * [np.nan]
+
+
+class Transforms(dict):
+    def __init__(self, d=None, **kwargs):
+        super().__init__()
+        if d is not None:
+            for key, value in d.items():
+                self[key] = value
+        for key, value in kwargs.items():
+            self[key] = value
+
+    def __contains__(self, item):
+        for key in self.keys():
+            if all([i == j or j is None or i in j for i, j in zip(item, key)]):
+                return True
+        return False
+
+    def __getitem__(self, item):
+        for key, value in self.items():
+            if all([i == j or j is None or i in j for i, j in zip(item, key)]):
+                return value
+        raise KeyError(f'{item}')
+
+    def __setitem__(self, key, value):
+        super().__setitem__(tuple((i,) if isinstance(i, Number) else i for i in key), value)
+
+    def get(self, item, default=None):
+        try:
+            return self[item]
+        except KeyError:
+            return default
+
+    def asdict(self):
+        return {':'.join(str(i) for i in key): value.asdict() for key, value in self.items()}
+
```

