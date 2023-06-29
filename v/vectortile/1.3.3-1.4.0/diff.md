# Comparing `tmp/vectortile-1.3.3.tar.gz` & `tmp/vectortile-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vectortile-1.3.3.tar", last modified: Wed May  6 08:13:04 2015, max compression
+gzip compressed data, was "vectortile-1.4.0.tar", last modified: Thu Jun 29 14:48:02 2023, max compression
```

## Comparing `vectortile-1.3.3.tar` & `vectortile-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2015-05-06 08:13:04.000000 vectortile-1.3.3/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2015-05-05 08:06:05.000000 vectortile-1.3.3/requirements.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6928 2015-05-06 08:13:04.000000 vectortile-1.3.3/PKG-INFO
--rw-r--r--   0 redhog    (1000) redhog    (1000)      898 2014-12-16 09:37:29.000000 vectortile-1.3.3/setup.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2015-05-06 08:13:04.000000 vectortile-1.3.3/vectortile/
--rw-r--r--   0 redhog    (1000) redhog    (1000)     1903 2014-11-18 12:45:26.000000 vectortile-1.3.3/vectortile/Tile.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1237 2015-05-05 08:06:05.000000 vectortile-1.3.3/vectortile/version.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)      184 2014-09-10 09:44:11.000000 vectortile-1.3.3/vectortile/__init__.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)     2041 2014-11-19 15:10:41.000000 vectortile-1.3.3/vectortile/Bbox.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)     6202 2014-10-22 11:08:51.000000 vectortile-1.3.3/vectortile/TypedMatrix.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)     3082 2014-09-10 08:29:19.000000 vectortile-1.3.3/vectortile/TileBounds.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2015-05-06 08:13:04.000000 vectortile-1.3.3/vectortile/tests/
--rw-r--r--   0 redhog    (1000) redhog    (1000)      685 2014-09-10 08:29:19.000000 vectortile-1.3.3/vectortile/tests/test_Tile.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)        0 2014-09-10 08:29:19.000000 vectortile-1.3.3/vectortile/tests/__init__.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)     2110 2014-09-10 08:29:19.000000 vectortile-1.3.3/vectortile/tests/test_TileBounds.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)     3872 2014-10-22 11:08:51.000000 vectortile-1.3.3/vectortile/tests/test_TypedMatrix.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)      411 2014-11-27 13:22:14.000000 vectortile-1.3.3/vectortile/tests/test_Bbox.py
--rw-r--r--   0 redhog    (1000) redhog    (1000)     4321 2014-11-27 13:22:35.000000 vectortile-1.3.3/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1075 2023-06-29 14:09:24.000000 vectortile-1.4.0/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       43 2023-06-29 14:09:24.000000 vectortile-1.4.0/MANIFEST.in
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     5902 2023-06-29 14:48:02.081652 vectortile-1.4.0/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     4321 2023-06-29 14:09:24.000000 vectortile-1.4.0/README.md
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2023-06-29 14:09:24.000000 vectortile-1.4.0/requirements.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-29 14:48:02.081652 vectortile-1.4.0/setup.cfg
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      975 2023-06-29 14:47:50.000000 vectortile-1.4.0/setup.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/vectortile/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2041 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/Bbox.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1903 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/Tile.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3083 2023-06-29 14:13:22.000000 vectortile-1.4.0/vectortile/TileBounds.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6202 2023-06-29 14:42:56.000000 vectortile-1.4.0/vectortile/TypedMatrix.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      195 2023-06-29 14:13:09.000000 vectortile-1.4.0/vectortile/__init__.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/vectortile/tests/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      411 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/test_Bbox.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      685 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/test_Tile.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2110 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/test_TileBounds.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3873 2023-06-29 14:42:21.000000 vectortile-1.4.0/vectortile/tests/test_TypedMatrix.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1276 2023-06-29 14:46:00.000000 vectortile-1.4.0/vectortile/version.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/vectortile.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     5902 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      520 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       11 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vectortile-1.3.3/PKG-INFO` & `vectortile-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,190 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: vectortile
-Version: 1.3.3
+Version: 1.4.0
 Summary: A set of classes for managing tiles of geospatial vector data
-Home-page: https://github.com/SkyTruth/vectortile
-Author: Paul Woods
-Author-email: paul@skytruth.org
+Home-page: https://github.com/emerald-geomodelling/vectortile
+Author: Paul Woods, Egil Moeller
+Author-email: paul@skytruth.org, em@emrld.no
 License: The MIT License (MIT)
-
-Copyright (c) 2014 SkyTruth
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-Description: Vector Tile Tools
-        =================
-        A set of classes for managing tiles of geospatial vector data
-        
-        ![Build Status](https://travis-ci.org/SkyTruth/vectortile.svg)
-        
-        
-        Installation and Unittests
-        --------------------------
-        Install via pip:
-        
-            pip install vectortile
-        
-        Source:
-            
-            $ git clone https://github.com/SkyTruth/vectortile.git
-            $ cd vectortile
-            $ pip install -r requirements.txt
-            $ nosetests
-            $ python setup.py install
-        
-        
-        TypedMatrix
-        -----------
-        TypedMatrix is a binary coded format optimized for delivering large amounts of
-        tabular data from a web server to a javascript client without the need for
-        parsing in javascript on the client side.
-        
-        The vectortile.TypedMatrix module provides functions to read and write
-        typed-matrix formatted strings.
-        
-        
-        ### Format Details ###
-        A TypedMatrix is a packed 2 dimensional array of typed values suitable for
-        typecasting to a set of javascript arrays.  Currently two fundamental data
-        types are supported:
-        
-        - Int32
-        - Float32
-        
-        Special handling is provided for converting datetime values to Float32.  The
-        format includes a header containing a json object, which can contain arbitrary
-        content.  The header must contain at least:
         
-        - length: indicated the number of rows in the data section
-        - cols: an array of column definitions.  The length of this array indicates the number of columns in each row
+        Copyright (c) 2014 SkyTruth
         
-        For example, a TypedMatrix with 2 rows and 3 columns:
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Vector Tile Tools
+=================
+A set of classes for managing tiles of geospatial vector data
+
+![Build Status](https://travis-ci.org/SkyTruth/vectortile.svg)
+
+
+Installation and Unittests
+--------------------------
+Install via pip:
+
+    pip install vectortile
+
+Source:
+    
+    $ git clone https://github.com/SkyTruth/vectortile.git
+    $ cd vectortile
+    $ pip install -r requirements.txt
+    $ nosetests
+    $ python setup.py install
+
+
+TypedMatrix
+-----------
+TypedMatrix is a binary coded format optimized for delivering large amounts of
+tabular data from a web server to a javascript client without the need for
+parsing in javascript on the client side.
+
+The vectortile.TypedMatrix module provides functions to read and write
+typed-matrix formatted strings.
+
+
+### Format Details ###
+A TypedMatrix is a packed 2 dimensional array of typed values suitable for
+typecasting to a set of javascript arrays.  Currently two fundamental data
+types are supported:
+
+- Int32
+- Float32
+
+Special handling is provided for converting datetime values to Float32.  The
+format includes a header containing a json object, which can contain arbitrary
+content.  The header must contain at least:
+
+- length: indicated the number of rows in the data section
+- cols: an array of column definitions.  The length of this array indicates the number of columns in each row
+
+For example, a TypedMatrix with 2 rows and 3 columns:
+
+    {
+        'length': 2,
+        'cols': [
+            {
+                'type': 'Float32',
+                'name': 'float'
+            },
+            {
+                'type': 'Int32',
+                'name': 'int'
+            },
             {
-                'length': 2,
-                'cols': [
-                    {
-                        'type': 'Float32',
-                        'name': 'float'
-                    },
-                    {
-                        'type': 'Int32',
-                        'name': 'int'
-                    },
-                    {
-                        'type': 'Float32',
-                        'name': 'timestamp'
-                    }
-                ]
+                'type': 'Float32',
+                'name': 'timestamp'
             }
-        
-        
-        ### Usage Examples ###
-        
-            >>> from vectortile import TypedMatrix
-            >>> from datetime import datetime
-            >>> from pprint import pprint
-        
-            # Create two rows of 3 columns each: int, float and datetime
-            >>> data = [{'int':1, 'float':1.0, 'timestamp': datetime(2014,1,1)}]
-            >>> data.append ({'int':2, 'float':2.0, 'timestamp':datetime(2014,1,2)})
-            >>> t_str = TypedMatrix.pack(data)
-        
-            # Typedmatrix is now coded as a binary string, packed row-wise
-            >>> t_str
-            'tmtx\x01\x00\x00\x00r\x89\x00\x00\x00{"length": 2, "cols": [{"type": "Float32", "name": "float"}, {"type": "Int32", "name": "int"}, {"type": "Float32", "name": "timestamp"}]}\x00\x00\x80?\x01\x00\x00\x00\x8d\xa5\xa1S\x00\x00\x00@\x02\x00\x00\x00 \xa8\xa1S'
-            
-            >>> header, data = TypedMatrix.unpack(t_str)
-            >>> pprint(header)
-            {
-                'cols': [
-                    {
-                        'name': 'float',
-                        'type': 'Float32'
-                    },
-                    {
-                        'name': 'int',
-                        'type': 'Int32'
-                    },
-                    {
-                        'name': 'timestamp',
-                        'type': 'Float32'
-                    }
-                ],
-                'length': 2
+        ]
+    }
+
+
+### Usage Examples ###
+
+    >>> from vectortile import TypedMatrix
+    >>> from datetime import datetime
+    >>> from pprint import pprint
+
+    # Create two rows of 3 columns each: int, float and datetime
+    >>> data = [{'int':1, 'float':1.0, 'timestamp': datetime(2014,1,1)}]
+    >>> data.append ({'int':2, 'float':2.0, 'timestamp':datetime(2014,1,2)})
+    >>> t_str = TypedMatrix.pack(data)
+
+    # Typedmatrix is now coded as a binary string, packed row-wise
+    >>> t_str
+    'tmtx\x01\x00\x00\x00r\x89\x00\x00\x00{"length": 2, "cols": [{"type": "Float32", "name": "float"}, {"type": "Int32", "name": "int"}, {"type": "Float32", "name": "timestamp"}]}\x00\x00\x80?\x01\x00\x00\x00\x8d\xa5\xa1S\x00\x00\x00@\x02\x00\x00\x00 \xa8\xa1S'
+    
+    >>> header, data = TypedMatrix.unpack(t_str)
+    >>> pprint(header)
+    {
+        'cols': [
+            {
+                'name': 'float',
+                'type': 'Float32'
+            },
+            {
+                'name': 'int',
+                'type': 'Int32'
+            },
+            {
+                'name': 'timestamp',
+                'type': 'Float32'
             }
-            
-            >>> pprint(data)
-            [
-                {
-                    'float': 1.0,
-                    'int': 1,
-                    'timestamp': 1388534431744.0
-                },
-                {
-                    'float': 2.0,
-                    'int': 2,
-                    'timestamp': 1388620808192.0
-                }
-            ]
-        
-            # Pack data column-wise
-            >>> TypedMatrix.pack(data,orientation='columnwise')
-            'tmtx\x01\x00\x00\x00c\x89\x00\x00\x00{"length": 2, "cols": [{"type": "Float32", "name": "float"}, {"type": "Int32", "name": "int"}, {"type": "Float32", "name": "timestamp"}]}\x00\x00\x80?\x00\x00\x00@\x01\x00\x00\x00\x02\x00\x00\x00\x8d\xa5\xa1S \xa8\xa1S'
-            
-            >>> header, data = TypedMatrix.unpack(t_str)
-            >>> pprint(header)
-            {
-                'cols': [
-                    {
-                        'name': 'float',
-                        'type': 'Float32'
-                    },
-                    {
-                        'name': 'int',
-                        'type': 'Int32'
-                    },
-                    {
-                        'name': 'timestamp',
-                        'type': 'Float32'
-                    }
-                ],
-                'length': 2
+        ],
+        'length': 2
+    }
+    
+    >>> pprint(data)
+    [
+        {
+            'float': 1.0,
+            'int': 1,
+            'timestamp': 1388534431744.0
+        },
+        {
+            'float': 2.0,
+            'int': 2,
+            'timestamp': 1388620808192.0
+        }
+    ]
+
+    # Pack data column-wise
+    >>> TypedMatrix.pack(data,orientation='columnwise')
+    'tmtx\x01\x00\x00\x00c\x89\x00\x00\x00{"length": 2, "cols": [{"type": "Float32", "name": "float"}, {"type": "Int32", "name": "int"}, {"type": "Float32", "name": "timestamp"}]}\x00\x00\x80?\x00\x00\x00@\x01\x00\x00\x00\x02\x00\x00\x00\x8d\xa5\xa1S \xa8\xa1S'
+    
+    >>> header, data = TypedMatrix.unpack(t_str)
+    >>> pprint(header)
+    {
+        'cols': [
+            {
+                'name': 'float',
+                'type': 'Float32'
+            },
+            {
+                'name': 'int',
+                'type': 'Int32'
+            },
+            {
+                'name': 'timestamp',
+                'type': 'Float32'
             }
-            
-            >>> pprint(data)
-            [
-                {
-                    'float': 1.0,
-                    'int': 1,
-                    'timestamp': 1388534431744.0
-                },
-                {
-                    'float': 2.0,
-                    'int': 2,
-                    'timestamp': 1388620808192.0
-                }
-            ]
-        
-        
-        ### Javascript Example ###
-        See [data-visualization-tools](https://github.com/SkyTruth/data-visualization-tools)
-        
-Platform: UNKNOWN
+        ],
+        'length': 2
+    }
+    
+    >>> pprint(data)
+    [
+        {
+            'float': 1.0,
+            'int': 1,
+            'timestamp': 1388534431744.0
+        },
+        {
+            'float': 2.0,
+            'int': 2,
+            'timestamp': 1388620808192.0
+        }
+    ]
+
+
+### Javascript Example ###
+See [data-visualization-tools](https://github.com/SkyTruth/data-visualization-tools)
```

### Comparing `vectortile-1.3.3/vectortile/Tile.py` & `vectortile-1.4.0/vectortile/Tile.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.3.3/vectortile/version.py` & `vectortile-1.4.0/vectortile/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-__version__ = '1.3.3'
-__author__ = 'Paul Woods'
-__author_email__ = 'paul@skytruth.org'
-__source__ = 'https://github.com/SkyTruth/vectortile'
+__version__ = '1.4.0'
+__author__ = 'Paul Woods, Egil Moeller'
+__author_email__ = 'paul@skytruth.org, em@emrld.no'
+__source__ = 'https://github.com/emerald-geomodelling/vectortile'
 __license__ = """The MIT License (MIT)
 
 Copyright (c) 2014 SkyTruth
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `vectortile-1.3.3/vectortile/Bbox.py` & `vectortile-1.4.0/vectortile/Bbox.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.3.3/vectortile/TypedMatrix.py` & `vectortile-1.4.0/vectortile/TypedMatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 TypedMatrix.py - read/write TypedMatrix format
 """
 
-magic = 'tmtx' # Must be four bytes long!
+magic = b'tmtx' # Must be four bytes long!
 version = 2
 
-import StringIO
+import io
 import struct
 import json
 import calendar
 from datetime import datetime
 
 # Header Structure
 # {
@@ -39,22 +39,22 @@
     """
     # make data iterable
     if type(data) is dict:
         data = [data]
 
     cols = {}
     for i, d in enumerate(data):
-        for key, value in d.iteritems():
+        for key, value in d.items():
             t = type(value)
             if t not in typemap:
                 raise TypeError ('TypedMatrix: "%s" is not a supported type in field "%s"' % (type(value), key))
             if key not in cols:
                 cols[key] = {'name': key, 'type': typemap[t]}
-    cols = cols.values()
-    cols.sort(lambda a, b: cmp(a['name'], b['name']))
+    cols = list(cols.values())
+    cols.sort(key=lambda a: a['name'])
     return cols
 
 
 def _datetime2timestamp(dt):
     return calendar.timegm(dt.utctimetuple()) * 1000.0
 
 
@@ -109,22 +109,22 @@
                 col.update(colsByName[col['name']])
 
     header['version'] = version
     if orientation is None:
         raise ValueError ('TypedMatrix: unknown orientation %s' % orientation)
     header['orientation'] = orientation
 
-    f = StringIO.StringIO()
-    headerstr = json.dumps(header)
+    f = io.BytesIO()
+    headerstr = json.dumps(header).encode("utf-8")
     paddinglen = (4 - len(headerstr) % 4) % 4
-    headerstr += (" " * paddinglen)
+    headerstr += (b" " * paddinglen)
 
 
     # write "magic" file format token at the start
-    f.write(struct.pack('<%sc' % len(magic), *magic))
+    f.write(struct.pack('<%ss' % len(magic), magic))
     f.write(struct.pack("<i", len(headerstr)))
     f.write(headerstr)
 
     colspecs = [{'name': col['name'], 'type': col['type'], 'default': typedefaultmap[col['type']]} for col in columns]
 
     if orientation == 'rowwise':
         for d in data:
@@ -151,22 +151,22 @@
 
 
 def unpack(packed_str):
     """
     Unpack a binary packed string containing a TypedMatrix.   Returns a tuple of header and data
     header is a dict and data is a list of dicts
     """
-    f = StringIO.StringIO(packed_str)
+    f = io.BytesIO(packed_str)
 
     # read "magic" file format token
-    token = ''.join(_struct_read(f, 'c', len(magic)))
+    token = b''.join(_struct_read(f, 'c', len(magic)))
     assert(token == magic)
 
     header_len = _struct_read(f,'i')
-    header = json.loads(f.read(header_len))
+    header = json.loads(f.read(header_len).decode("utf-8"))
 
     assert (header['version'] == version)  # only supports one version right now
 
     if header['orientation'] == 'rowwise':
         fmt = row_fmt(header['cols'])
         data = []
         col_names = [col['name'] for col in header['cols']]
@@ -176,15 +176,15 @@
         col_data = []
         col_names = [col['name'] for col in header['cols']]
         length = header['length']
         for col in header['cols']:
             col_data.append(_struct_read(f, typeformatmap[col['type']], length))
         col_indexes = range(0, len(col_names))
         if length > 1:
-            data = [dict(zip(col_names, [col_data[c][i] for c in col_indexes])) for i in xrange(0, length)]
+            data = [dict(zip(col_names, [col_data[c][i] for c in col_indexes])) for i in range(0, length)]
         elif length == 1:
             data = [dict(zip(col_names, [col_data[c] for c in col_indexes]))]
         else:
             data = []
     else:
         raise Exception("Unsupported orientation")
```

### Comparing `vectortile-1.3.3/vectortile/TileBounds.py` & `vectortile-1.4.0/vectortile/TileBounds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import quadtree
 
-from Bbox import Bbox
+from .Bbox import Bbox
 
 class TileBounds(object):
     maxzoom = 21
     worldwidth = 360.0
     worldheight = 180.0
     min_tile_width = worldwidth / pow(2, maxzoom)
     min_tile_height = worldheight / pow(2, maxzoom)
```

### Comparing `vectortile-1.3.3/vectortile/tests/test_Tile.py` & `vectortile-1.4.0/vectortile/tests/test_Tile.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.3.3/vectortile/tests/test_TileBounds.py` & `vectortile-1.4.0/vectortile/tests/test_TileBounds.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.3.3/vectortile/tests/test_TypedMatrix.py` & `vectortile-1.4.0/vectortile/tests/test_TypedMatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.assertDictEqual(data[0], data_out)
 
     def test_unsupported_type(self):
         data_in = dict(I=1, F=2.0, D=datetime(2014, 1, 1), unsupported=timedelta(1))
         self.assertRaises(TypeError, TypedMatrix.pack, data_in)
 
     def test_bad_format(self):
-        self.assertRaises(AssertionError, TypedMatrix.unpack, packed_str='not valid')
+        self.assertRaises(AssertionError, TypedMatrix.unpack, packed_str=b'not valid')
 
     def test_columnwise(self):
         data_in = [{'A': 1, 'B': 2}, {'A': 11, 'B': 22}, {'A': 111, 'B': 222}]
         packed_str = TypedMatrix.pack(data_in, orientation='columnwise')
         header, data_out = TypedMatrix.unpack(packed_str)
         self.assertEqual(3, header['length'])
         self.assertListEqual(data_in, data_out)
```

### Comparing `vectortile-1.3.3/README.md` & `vectortile-1.4.0/README.md`

 * *Files identical despite different names*

