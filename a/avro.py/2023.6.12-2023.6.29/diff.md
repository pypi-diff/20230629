# Comparing `tmp/avro.py-2023.6.12.tar.gz` & `tmp/avro.py-2023.6.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-2023.6.12.tar", last modified: Mon Jun 12 06:52:14 2023, max compression
+gzip compressed data, was "avro.py-2023.6.29.tar", last modified: Thu Jun 29 17:27:45 2023, max compression
```

## Comparing `avro.py-2023.6.12.tar` & `avro.py-2023.6.29.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 06:51:49.000000 avro.py-2023.6.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 06:51:49.000000 avro.py-2023.6.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-12 06:52:14.635330 avro.py-2023.6.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-12 06:51:49.000000 avro.py-2023.6.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.631330 avro.py-2023.6.12/avro/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11695 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59054 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/resources/avrodict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2814 2023-06-12 06:51:49.000000 avro.py-2023.6.12/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 06:52:14.000000 avro.py-2023.6.12/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 06:51:49.000000 avro.py-2023.6.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 06:52:14.635330 avro.py-2023.6.12/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-06-12 06:51:49.000000 avro.py-2023.6.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:52:14.635330 avro.py-2023.6.12/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5744 2023-06-12 06:51:49.000000 avro.py-2023.6.12/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-06-12 06:51:49.000000 avro.py-2023.6.12/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3750 2023-06-12 06:51:49.000000 avro.py-2023.6.12/tests/test_utils_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:27:45.372536 avro.py-2023.6.29/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 17:27:31.000000 avro.py-2023.6.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 17:27:31.000000 avro.py-2023.6.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-29 17:27:45.372536 avro.py-2023.6.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-29 17:27:31.000000 avro.py-2023.6.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:27:45.368536 avro.py-2023.6.29/avro/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      583 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10649 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:27:45.372536 avro.py-2023.6.29/avro/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32079 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/resources/avrodict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:27:45.372536 avro.py-2023.6.29/avro/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/utils/count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-06-29 17:27:31.000000 avro.py-2023.6.29/avro/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:27:45.372536 avro.py-2023.6.29/avro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-29 17:27:45.000000 avro.py-2023.6.29/avro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 17:27:45.000000 avro.py-2023.6.29/avro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:27:45.000000 avro.py-2023.6.29/avro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 17:27:45.000000 avro.py-2023.6.29/avro.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-29 17:27:31.000000 avro.py-2023.6.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:27:45.372536 avro.py-2023.6.29/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-06-29 17:27:31.000000 avro.py-2023.6.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:27:45.372536 avro.py-2023.6.29/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4658 2023-06-29 17:27:31.000000 avro.py-2023.6.29/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-06-29 17:27:31.000000 avro.py-2023.6.29/tests/test_utils_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2653 2023-06-29 17:27:31.000000 avro.py-2023.6.29/tests/test_utils_validate.py
```

### Comparing `avro.py-2023.6.12/LICENSE` & `avro.py-2023.6.29/LICENSE`

 * *Files identical despite different names*

### Comparing `avro.py-2023.6.12/PKG-INFO` & `avro.py-2023.6.29/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.6.12
+Version: 2023.6.29
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+<!-- SPDX-License-Identifier: MIT -->
+
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
 A modern Pythonic implementation of the popular Bengali phonetic-typing software **Avro Phonetic.**
 
 [![Downloads](https://static.pepy.tech/personalized-badge/avro-py?period=total&units=international_system&left_color=grey&right_color=black&left_text=Downloads)](https://pepy.tech/project/avro-py)
@@ -31,16 +33,15 @@
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
 <br>
 
 | Checks | Status | 
 |:---|---:|
 | usability | [![Unit Tests](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml) |
-| beauty | [![Linting](https://github.com/hitblast/avro.py/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/linting.yml) |
-| cleanliness | [![Format](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml) |
+| beauty | [![Style Check](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml) |
 
 <br>
 
 </div>
 
 ## Overview
```

### Comparing `avro.py-2023.6.12/README.md` & `avro.py-2023.6.29/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<!-- SPDX-License-Identifier: MIT -->
+
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
 A modern Pythonic implementation of the popular Bengali phonetic-typing software **Avro Phonetic.**
 
 [![Downloads](https://static.pepy.tech/personalized-badge/avro-py?period=total&units=international_system&left_color=grey&right_color=black&left_text=Downloads)](https://pepy.tech/project/avro-py)
@@ -9,16 +11,15 @@
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
 <br>
 
 | Checks | Status | 
 |:---|---:|
 | usability | [![Unit Tests](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml) |
-| beauty | [![Linting](https://github.com/hitblast/avro.py/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/linting.yml) |
-| cleanliness | [![Format](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml) |
+| beauty | [![Style Check](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml) |
 
 <br>
 
 </div>
 
 ## Overview
```

### Comparing `avro.py-2023.6.12/avro/main.py` & `avro.py-2023.6.29/avro/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,27 @@
-'''
+# SPDX-License-Identifier: MIT
 
-## A modern Pythonic implementation of Avro Phonetic.
-
----
-
-MIT License
-
-Copyright (c) 2022-present HitBlast
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the 'Software'), to deal
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
-'''
 
 # Import third-party modules.
 import re
+from functools import lru_cache
 from typing import Any, Dict, List, Optional, Union
 
 # Import local modules.
 from . import config
 from .utils import validate
 
 # Constants.
 PATTERNS: Any = config.AVRO_DICT['data']['patterns']
 NON_RULE_PATTERNS: list = [p for p in PATTERNS if 'rules' not in p]
 RULE_PATTERNS: list = [p for p in PATTERNS if 'rules' in p]
 
 
 # The primary parse function for the library.
+@lru_cache
 def parse(*texts: str, in_ascii: bool = False) -> Union[str, List[str]]:
     '''
     ### Parses input text, matches and replaces using avrodict.
 
     If a valid replacement is found, then it returns the replaced string.
     If no replacement is found, then it instead returns the input text.
 
@@ -126,14 +101,15 @@
         output.append(
             subparse(text) if not in_ascii else str(subparse(text).encode('ascii', errors='backslashreplace'))
         )
 
     return output[0] if len(output) == 1 else output
 
 
+@lru_cache
 def reverse(*texts: str) -> Union[str, List[str]]:
     '''
     ### Reverses input text to Roman script typed in English.
 
     If a valid replacement is found, then it returns the replaced string.
     If no replacement is found, then it instead returns the input text.
 
@@ -265,14 +241,15 @@
         for x in patterns
         if x.get('find', None)
         and (cur + len(x['find']) <= len(fixed_text))
         and x['find'] == fixed_text[cur : (cur + len(x['find']))]
     ]
 
 
+@lru_cache
 def reverse_with_rules(cursor: int, fixed_text: str, text_reversed: str) -> str:
     '''
     ### Enhances the word with rules for reverse-parsing.
     '''
 
     added_suffix = ''
```

### Comparing `avro.py-2023.6.12/avro.py.egg-info/PKG-INFO` & `avro.py-2023.6.29/avro.py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.6.12
+Version: 2023.6.29
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+<!-- SPDX-License-Identifier: MIT -->
+
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
 
 A modern Pythonic implementation of the popular Bengali phonetic-typing software **Avro Phonetic.**
 
 [![Downloads](https://static.pepy.tech/personalized-badge/avro-py?period=total&units=international_system&left_color=grey&right_color=black&left_text=Downloads)](https://pepy.tech/project/avro-py)
@@ -31,16 +33,15 @@
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
 <br>
 
 | Checks | Status | 
 |:---|---:|
 | usability | [![Unit Tests](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml) |
-| beauty | [![Linting](https://github.com/hitblast/avro.py/actions/workflows/linting.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/linting.yml) |
-| cleanliness | [![Format](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml) |
+| beauty | [![Style Check](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml) |
 
 <br>
 
 </div>
 
 ## Overview
```

### Comparing `avro.py-2023.6.12/setup.py` & `avro.py-2023.6.29/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# SPDX-License-Identifier: MIT
+
+
 # Import both local and third-party setup modules.
-import os
 import codecs
-from setuptools import setup, find_packages
+import os
+
+from setuptools import find_packages, setup
 
 # Import local modules to fetch version number.
 from avro import __version__
 
-
 # Constants.
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as fh:
     long_description = "\n" + fh.read()
```

