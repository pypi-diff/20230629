# Comparing `tmp/katalytic_images-0.6.0.tar.gz` & `tmp/katalytic_images-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_images-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_images-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic_images-0.6.0.tar` & `katalytic_images-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.6.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.6.0/.gitignore
--rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.6.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     3500 2023-06-26 19:15:12.396704 katalytic_images-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.6.0/README.md
--rw-r--r--   0        0        0     1549 2023-06-26 19:15:12.396704 katalytic_images-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    23183 2023-06-26 19:10:26.536185 katalytic_images-0.6.0/src/katalytic/images.py
--rw-r--r--   0        0        0    16722 2023-06-26 19:11:21.424280 katalytic_images-0.6.0/tests/test_images.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.7.0/.gitignore
+-rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.7.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3831 2023-06-29 18:12:27.326416 katalytic_images-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.7.0/README.md
+-rw-r--r--   0        0        0     1549 2023-06-29 18:12:27.326416 katalytic_images-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    23618 2023-06-29 18:06:33.150349 katalytic_images-0.7.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    18056 2023-06-29 18:05:45.304863 katalytic_images-0.7.0/tests/test_images.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.7.0/PKG-INFO
```

### Comparing `katalytic_images-0.6.0/.gitignore` & `katalytic_images-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.6.0/.gitlab-ci.yml` & `katalytic_images-0.7.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.6.0/CHANGELOG.md` & `katalytic_images-0.7.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 0.7.0 (2023-06-29)
+### feat
+- [[`1783c35`](https://gitlab.com/katalytic/katalytic-images/commit/1783c354f5a1da45b5784d065481ef568b80a8a7)] warn when using the wrong saver/loader
+### fix
+- [[`1f2e027`](https://gitlab.com/katalytic/katalytic-images/commit/1f2e02761af8ee18199841432f2e41af4e9248a6)] some edge case import issues
+
+
 ## 0.6.0 (2023-06-26)
 ### feat
 - [[`7baa7e9`](https://gitlab.com/katalytic/katalytic-images/commit/7baa7e94f5786d23f6f87051e8c87c4cdfec1407)] when passing a PIL.Image to draw() or load_image(), return another PIL.Image
 ### refactor
 - [[`eaa3cc6`](https://gitlab.com/katalytic/katalytic-images/commit/eaa3cc61705170539ec7076e63d86395ba57bf19)] make condition more explicit
 - [[`0d16675`](https://gitlab.com/katalytic/katalytic-images/commit/0d16675d3075eae62f31560c1e326a18057009a6)] use errno codes instead of hardcoded numbers
```

### Comparing `katalytic_images-0.6.0/LICENSE.txt` & `katalytic_images-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.6.0/README.md` & `katalytic_images-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.6.0/pyproject.toml` & `katalytic_images-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.6.0"
+version = "0.7.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic_images-0.6.0/src/katalytic/images.py` & `katalytic_images-0.7.0/src/katalytic/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import errno
 from pathlib import Path
 
 import cv2
+# noinspection PyProtectedMember
 from cv2 import (
     imwrite as __cv2_imwrite,
     cvtColor as __cv2_cvtColor
 )
 
 import numpy as np
 from numpy import (
@@ -13,18 +14,17 @@
     ndarray as __np_ndarray
 )
 
 import PIL.Image
 __PIL_Image_open = PIL.Image.open
 __PIL_Image_Image = PIL.Image.Image
 
-from katalytic.files import copy_file
-from katalytic.files import make_dir
-from katalytic.data.checks import is_iterable, is_number, is_sequence
+# noinspection PyProtectedMember
 from katalytic.data import _UNDEFINED
+from katalytic.data.checks import is_iterable, is_number, is_sequence
 from katalytic.pkg import get_version, mark
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def bhwc(arr):
     """
@@ -279,19 +279,23 @@
         **kwargs
     }
 
 
 def draw(image, data):
     """Draws shapes on a copy of the input image
 
-    This function takes an image and an collection specifying the shapes to be drawn on the image. The shapes can include lines, circles, rectangles, text, masks, and polylines. The function iterates over the collection in order and calls the corresponding drawing functions to draw each shape on the image.
+    This function takes an image and an collection specifying the shapes to be drawn on the image.
+    The shapes can include lines, circles, rectangles, text, masks, and polylines.
+    The calls the corresponding drawing functions for each shape in the order it appears in the collection.
 
     Parameters:
         image: a numpy array representing the image on which the shapes will be drawn.
-        data: The shapes to be drawn. It can be either a dictionary representing a single shape or a list of dictionaries representing multiple shapes.
+        data:
+            The shapes to be drawn. It can be either a dictionary representing a single shape
+            or a list of dictionaries representing multiple shapes.
 
     Raises:
         TypeError: If the 'data' parameter is not an iterable of shapes or a dict
         KeyError: If the 'type' key is missing in any shape dictionary.
         ValueError: If the 'type' key in any shape dictionary has an invalid value.
         ValueError: If the 'pts' key in a mask or polylines shape dictionary has an invalid format.
 
@@ -310,15 +314,17 @@
     else:
         return new_image
 
 
 def draw_inplace(image, data):
     """Draws shapes on the input image by modifying it in-place
 
-    This function takes an image and an collection specifying the shapes to be drawn on the image. The shapes can include lines, circles, rectangles, text, masks, and polylines. The function iterates over the collection in order and calls the corresponding drawing functions to draw each shape on the image.
+    This function takes an image and an collection specifying the shapes to be drawn on the image.
+    The shapes can include lines, circles, rectangles, text, masks, and polylines.
+    The calls the corresponding drawing functions for each shape in the order it appears in the collection.
 
     Parameters:
         image: a numpy array representing the image on which the shapes will be drawn.
         data: The shapes to be drawn. It can be either a dictionary representing a single shape or a list of dictionaries representing multiple shapes.
 
     Raises:
         TypeError: If the 'data' parameter is not an iterable of shapes or a dict
@@ -474,14 +480,16 @@
         TypeError: If the 'image' parameter has an unsupported type.
 
     """
     if not(mode is None or isinstance(mode, str)):
         raise TypeError(f'mode expected None or str. Got {type(mode)!r}')
 
     if isinstance(image, (str, Path)):
+        from katalytic.files import _warn_if_another_function_should_be_used, _load_funcs
+        _warn_if_another_function_should_be_used(str(image), _load_funcs)
         if not Path(image).exists() and default is not _UNDEFINED:
             return default
         else:
             return __np_array(__PIL_Image_open(image))
     elif isinstance(image, __PIL_Image_Image):
         return image.copy()
     elif isinstance(image, __np_ndarray):
@@ -542,14 +550,15 @@
     image_2 = load_image(image_2)
 
     if image_1.shape != image_2.shape:
         return False
     elif check_type and image_1.dtype != image_2.dtype:
         return False
     else:
+        # noinspection PyUnresolvedReferences
         return (image_1 == image_2).all()
 
 
 @mark('save::png')
 @mark('save::jpg')
 @mark('save::jpeg')
 def save_image(image, path, *, exists='replace', make_dirs=True, mode='RGB'):
@@ -581,24 +590,27 @@
 
     """
     if not isinstance(mode, str):
         raise TypeError(f'type(mode) = {type(mode)!r}')
     elif exists not in ('error', 'skip', 'replace'):
         raise ValueError(f'exists must be one of \'error\', \'skip\', \'replace\'. Got {exists!r}')
 
+    from katalytic.files import _warn_if_another_function_should_be_used, _save_funcs
+    _warn_if_another_function_should_be_used(str(path), _save_funcs)
     if Path(path).exists():
         if exists == 'error':
             raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
         elif exists == 'replace':
             pass  # continue executing
         elif exists == 'skip':
             return
 
     dest_dir = Path(path).parent
     if make_dirs:
+        from katalytic.files import make_dir
         make_dir(dest_dir, create_parents=True, exists_ok=True)
     elif not dest_dir.exists():
         raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
     elif dest_dir.is_file():
         raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
 
     if isinstance(image, __PIL_Image_Image):
@@ -606,10 +618,11 @@
 
     if isinstance(image, __np_ndarray):
         if mode != 'BGR':
             image = convert_image(image, mode, 'BGR')
 
         __cv2_imwrite(str(path), image)
     elif isinstance(image, (str, Path)):
+        from katalytic.files import copy_file
         copy_file(image, path, exists=exists)
     else:
         raise TypeError(f'type(image) = {type(image)!r}')
```

### Comparing `katalytic_images-0.6.0/tests/test_images.py` & `katalytic_images-0.7.0/tests/test_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import cv2
 import numpy as np
 import PIL.Image
 import pytest
 from PIL import Image
 
 from katalytic.data import all_types_besides
-from katalytic.files import get_unique_path, load, move_file, save
+from katalytic.files import get_unique_path, load, load_csv, load_json, load_text, move_file, save, save_csv, save_json, save_text
 from katalytic.images import bhwc, convert_image, create_circle, create_line, create_mask, create_polylines, create_rectangle, create_text, draw, hw, hwc, are_arrays_equal, load_image, save_image
 
 
 def _create_RGB(dtype=np.uint8):
     return np.array([
         [[255, 0, 0], [0, 255, 0], [0, 0, 255]],        # RGB
         [[0, 255, 255], [255, 0, 255], [255, 255, 0]],  # CMY
@@ -128,19 +128,21 @@
         img = np.array([[[0, 0, 0], [255, 255, 255]]])
         with pytest.raises(ValueError):
             _ = convert_image(img, 'unknown', 'RGB')
 
     @pytest.mark.parametrize('before', all_types_besides('str'))
     def test_save_raises_TypeError_for_before(self, before):
         with pytest.raises(TypeError):
+            # noinspection PyTypeChecker
             convert_image(_create_RGB(), before, 'RGB')
 
     @pytest.mark.parametrize('after', all_types_besides('str'))
     def test_save_raises_TypeError_for_after(self, after):
         with pytest.raises(TypeError):
+            # noinspection PyTypeChecker
             convert_image(_create_RGB(), 'RGB', after)
 
 
 class Test_draw:
     @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
@@ -317,14 +319,41 @@
             _create_RGB(np.float32),
             _create_RGB(np.uint8),
             check_type=True
         )
 
 
 class Test_load_and_save:
+    # noinspection PyBroadException
+    @pytest.mark.parametrize('ext, wrong_load, correct_load', [
+        ('jpeg', load_csv, 'load_image'),
+        ('jpg', load_json, 'load_image'),
+        ('png', load_text, 'load_image'),
+    ])
+    def test_using_the_wrong_loader_should_always_warn(self, ext, wrong_load, correct_load):
+        # The warning should be triggered regardless of whether the file exists or not.
+        with pytest.warns(UserWarning, match=f'Use "{correct_load}" for ".{ext}" files.'):
+            try:
+                wrong_load(get_unique_path('{}.' + ext))
+            except Exception:
+                pass
+
+    # noinspection PyBroadException
+    @pytest.mark.parametrize('ext, wrong_save, correct_save', [
+        ('jpeg', save_csv, 'save_image'),
+        ('jpg', save_json, 'save_image'),
+        ('png', save_text, 'save_image'),
+    ])
+    def test_using_the_wrong_saver_should_always_warn(self, ext, wrong_save, correct_save):
+        with pytest.warns(UserWarning, match=f'Use "{correct_save}" for ".{ext}" files.'):
+            try:
+                wrong_save(_create_RGB(), get_unique_path('{}.' + ext))
+            except Exception:
+                pass
+
     def test_str(self):
         image_1 = _create_RGB()
         path = get_unique_path('{}.png')
         save_image(image_1, path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_Path(self):
@@ -396,26 +425,26 @@
     def test_default(self):
         path = get_unique_path('{}.png')
         img = load_image(path, default=_create_RGB())
         assert are_arrays_equal(img, _create_RGB())
 
     def test_make_dirs_False(self):
         img = _create_RGB()
-        path = get_unique_path('{}/data.csv')
+        path = get_unique_path('{}/data.png')
         with pytest.raises(FileNotFoundError):
             save_image(img, path, make_dirs=False)
 
         # save image, then move it to a filename without extension
         path = get_unique_path('{}/data')
         save_image(img, f'{path}.png', make_dirs=True)
         move_file(f'{path}.png', path)
 
         # then try to use that filename as a directory
         with pytest.raises(NotADirectoryError):
-            save_image(img, f'{path}/x.csv', make_dirs=False)
+            save_image(img, f'{path}/x.png', make_dirs=False)
 
     @pytest.mark.parametrize('img', [1, True, None, [], {}, (), object()])
     def test_load_raises_TypeError_for_image(self, img):
         with pytest.raises(TypeError):
             load_image(img)
 
     @pytest.mark.parametrize('mode', [1, True, [], {}, (), object()])
```

### Comparing `katalytic_images-0.6.0/PKG-INFO` & `katalytic_images-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.6.0
+Version: 0.7.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

