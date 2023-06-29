# Comparing `tmp/croqueta-0.2.2.tar.gz` & `tmp/croqueta-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croqueta-0.2.2.tar", last modified: Sat Jun 17 16:23:06 2023, max compression
+gzip compressed data, was "croqueta-0.2.3.tar", last modified: Thu Jun 29 16:47:46 2023, max compression
```

## Comparing `croqueta-0.2.2.tar` & `croqueta-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 16:23:06.957148 croqueta-0.2.2/
--rw-r--r--   0 juanluis   (502) staff       (20)    11357 2022-03-30 10:50:05.000000 croqueta-0.2.2/LICENSE
--rw-r--r--   0 juanluis   (502) staff       (20)      588 2023-06-17 16:23:06.957217 croqueta-0.2.2/PKG-INFO
--rw-r--r--   0 juanluis   (502) staff       (20)      254 2023-06-17 16:17:55.000000 croqueta-0.2.2/README.md
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 16:23:06.956399 croqueta-0.2.2/croqueta/
--rw-r--r--   0 juanluis   (502) staff       (20)      215 2023-06-17 16:07:12.000000 croqueta-0.2.2/croqueta/__init__.py
--rw-r--r--   0 juanluis   (502) staff       (20)      879 2023-06-17 16:06:27.000000 croqueta-0.2.2/croqueta/maps.py
--rw-r--r--   0 juanluis   (502) staff       (20)     1321 2023-06-17 09:24:30.000000 croqueta-0.2.2/croqueta/obj.py
--rw-r--r--   0 juanluis   (502) staff       (20)     9806 2023-06-17 16:21:30.000000 croqueta-0.2.2/croqueta/pd.py
--rw-r--r--   0 juanluis   (502) staff       (20)      764 2023-06-17 09:39:27.000000 croqueta-0.2.2/croqueta/str.py
--rw-r--r--   0 juanluis   (502) staff       (20)     1162 2023-06-17 15:19:25.000000 croqueta-0.2.2/croqueta/viz.py
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 16:23:06.957039 croqueta-0.2.2/croqueta.egg-info/
--rw-r--r--   0 juanluis   (502) staff       (20)      588 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/PKG-INFO
--rw-r--r--   0 juanluis   (502) staff       (20)      265 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/SOURCES.txt
--rw-r--r--   0 juanluis   (502) staff       (20)        1 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/dependency_links.txt
--rw-r--r--   0 juanluis   (502) staff       (20)        9 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/top_level.txt
--rw-r--r--   0 juanluis   (502) staff       (20)      103 2023-06-17 16:23:06.957474 croqueta-0.2.2/setup.cfg
--rw-r--r--   0 juanluis   (502) staff       (20)      673 2023-06-17 16:07:46.000000 croqueta-0.2.2/setup.py
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-29 16:47:46.545122 croqueta-0.2.3/
+-rw-r--r--   0 juanluis   (502) staff       (20)    11357 2022-03-30 10:50:05.000000 croqueta-0.2.3/LICENSE
+-rw-r--r--   0 juanluis   (502) staff       (20)      551 2023-06-29 16:47:46.545183 croqueta-0.2.3/PKG-INFO
+-rw-r--r--   0 juanluis   (502) staff       (20)      254 2023-06-17 16:17:55.000000 croqueta-0.2.3/README.md
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-29 16:47:46.544344 croqueta-0.2.3/croqueta/
+-rw-r--r--   0 juanluis   (502) staff       (20)      215 2023-06-17 16:07:12.000000 croqueta-0.2.3/croqueta/__init__.py
+-rw-r--r--   0 juanluis   (502) staff       (20)      879 2023-06-17 16:40:20.000000 croqueta-0.2.3/croqueta/maps.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     1321 2023-06-17 09:24:30.000000 croqueta-0.2.3/croqueta/obj.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     9792 2023-06-29 16:46:21.000000 croqueta-0.2.3/croqueta/pd.py
+-rw-r--r--   0 juanluis   (502) staff       (20)      765 2023-06-17 17:00:12.000000 croqueta-0.2.3/croqueta/str.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     1153 2023-06-17 17:03:01.000000 croqueta-0.2.3/croqueta/viz.py
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-29 16:47:46.545015 croqueta-0.2.3/croqueta.egg-info/
+-rw-r--r--   0 juanluis   (502) staff       (20)      551 2023-06-29 16:47:46.000000 croqueta-0.2.3/croqueta.egg-info/PKG-INFO
+-rw-r--r--   0 juanluis   (502) staff       (20)      265 2023-06-29 16:47:46.000000 croqueta-0.2.3/croqueta.egg-info/SOURCES.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)        1 2023-06-29 16:47:46.000000 croqueta-0.2.3/croqueta.egg-info/dependency_links.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)        9 2023-06-29 16:47:46.000000 croqueta-0.2.3/croqueta.egg-info/top_level.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)      103 2023-06-29 16:47:46.545503 croqueta-0.2.3/setup.cfg
+-rw-r--r--   0 juanluis   (502) staff       (20)      673 2023-06-29 16:47:12.000000 croqueta-0.2.3/setup.py
```

### Comparing `croqueta-0.2.2/LICENSE` & `croqueta-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `croqueta-0.2.2/croqueta/maps.py` & `croqueta-0.2.3/croqueta/maps.py`

 * *Files identical despite different names*

### Comparing `croqueta-0.2.2/croqueta/obj.py` & `croqueta-0.2.3/croqueta/obj.py`

 * *Files identical despite different names*

### Comparing `croqueta-0.2.2/croqueta/pd.py` & `croqueta-0.2.3/croqueta/pd.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,37 +12,37 @@
     Filter a dataframe with a dictionary of filters.
 
     Args:
         df (pandas.DataFrame): The dataframe to be filtered.
         filter_dict (dict): A dictionary of filters, where the keys represent the column names
             and the values represent the filter values.
         filter_type (str, optional): The type of filter to apply. Valid values are 'and' (default) and 'or'.
-        filter_iterable_values (bool, optional): Determines whether iterable values should be treated as
-            multiple filter values. Defaults to True.
+        filter_iterable_values (bool, optional): If a filter value is an iterable, create one filter for each
+        element in the iterable. Defaults to True.
 
     Returns:
         pandas.DataFrame: The filtered dataframe.
 
     Example:
         df = pd.DataFrame({'A': [1, 2, 3, 4], 'B': ['x', 'y', 'z', 'w']})
         filters = {'A': [2, 3], 'B': 'x'}
         filtered_df = filter_df(df, filters, filter_type = "or")
     """
     views = []
     for key, value in filter_dict.items():
         if filter_iterable_values and not isinstance(value, str) and isinstance(value, Iterable):
-            views.append(df[df[key].isin(value)])
+            views.append(df[key].isin(value))
         else:
-            views.append(df[df[key] == value])
+            views.append(df[key] == value)
     
     if filter_type == "and":
         index = reduce(lambda x, y : x.index.intersection(y.index), views)   
     elif filter_type == "or":
         index = reduce(lambda x, y : x.index.union(y.index), views)
-        
+
     if len(index) > 0:
         return df.loc[index]
 
 def generate_fake_df(n_rows, cols, col_names = None, intervals = None, seed = None):
     """
     Generate a DataFrame with dummy data in a controlled manner.
     Supported datatypes for the columns are int, float, date and categorical.
```

### Comparing `croqueta-0.2.2/croqueta/str.py` & `croqueta-0.2.3/croqueta/str.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
 import string
 import hashlib
 
 def hash_string_to_n_digits(s, n = 10):
-    """Hash a string to a number with n digits."""
+    """Hash a string to a number with n digits.""" 
 
     assert n > 0, "Number of digits must be a positive integer"
 
     # Create a SHA256 hash object
     hasher = hashlib.sha256()
 
     # Encode the input string and hash it
```

### Comparing `croqueta-0.2.2/croqueta/viz.py` & `croqueta-0.2.3/croqueta/viz.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from matplotlib.axes import Axes
 from pathlib import Path
 
-def savefig(fig, filename : str, path = None, size = None, dpi: int =300):
+def savefig(fig, filename : str, path = None, size = None, dpi: int = 300):
     """
     Save a figure to a file.
 
     Parameters:
         - fig: The figure or axes object to save.
         - filename: The filename to save the figure as.
         - path: Optional. The directory path to save the figure in.
@@ -26,9 +26,8 @@
         path = Path()
     elif isinstance(path,str):
         path = Path(path)
     if not filename.endswith('.png'):
         filename = filename + '.png'
     if isinstance(size, tuple):
         fig.set_size_inches(size)
-    fig.set_dpi(dpi)
-    fig.savefig(path / filename) 
+    fig.savefig(path / filename, dpi = dpi)
```

### Comparing `croqueta-0.2.2/setup.py` & `croqueta-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="croqueta", # Replace with your own username
-    version="0.2.2",
+    version="0.2.3",
     author="juanluisrto",
     author_email="juanluis.rto@gmail.com",
     description="A bunch of utilities to code even faster.",
     url="https://github.com/juanluisrto/croqueta",
     packages= setuptools.find_packages(),
     python_requires='>=3.8',
     include_package_data=True,
```

