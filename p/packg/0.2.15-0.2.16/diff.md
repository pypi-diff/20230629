# Comparing `tmp/packg-0.2.15.tar.gz` & `tmp/packg-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.15.tar", last modified: Thu Jun 29 10:46:38 2023, max compression
+gzip compressed data, was "packg-0.2.16.tar", last modified: Thu Jun 29 13:21:09 2023, max compression
```

## Comparing `packg-0.2.15.tar` & `packg-0.2.16.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 10:46:38.585045 packg-0.2.15/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.15/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2102 2023-06-29 10:46:38.585045 packg-0.2.15/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1306 2023-06-29 10:46:26.000000 packg-0.2.15/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2317 2023-06-21 09:57:15.000000 packg-0.2.15/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       87 2023-06-29 10:46:26.000000 packg-0.2.15/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-29 10:46:38.589045 packg-0.2.15/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 10:46:38.509043 packg-0.2.15/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 10:46:38.545044 packg-0.2.15/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      130 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 10:46:38.581045 packg-0.2.15/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      525 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/iotools/compressed.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4735 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4317 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2678 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/paths.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-06-29 10:46:26.000000 packg-0.2.15/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 10:46:38.565044 packg-0.2.15/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2102 2023-06-29 10:46:38.000000 packg-0.2.15/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      657 2023-06-29 10:46:38.000000 packg-0.2.15/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-29 10:46:38.000000 packg-0.2.15/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       87 2023-06-29 10:46:38.000000 packg-0.2.15/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-06-29 10:46:38.000000 packg-0.2.15/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.15/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.899574 packg-0.2.16/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.16/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-06-29 13:21:09.899574 packg-0.2.16/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-06-29 13:20:48.000000 packg-0.2.16/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2317 2023-06-21 09:57:15.000000 packg-0.2.16/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       87 2023-06-29 13:20:48.000000 packg-0.2.16/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-29 13:21:09.903574 packg-0.2.16/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.803572 packg-0.2.16/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.855573 packg-0.2.16/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      130 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.895574 packg-0.2.16/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      525 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/compressed.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4735 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4317 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2678 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/paths.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5458 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/strings.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-06-29 13:20:48.000000 packg-0.2.16/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-29 13:21:09.879574 packg-0.2.16/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      678 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       87 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-06-29 13:21:09.000000 packg-0.2.16/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.16/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.15/LICENSE` & `packg-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/PKG-INFO` & `packg-0.2.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.15
+Version: 0.2.16
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -55,13 +55,13 @@
 ## Dev install
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint packg
 
-# run tests
 python -m pytest --cov
+
+pylint packg
 pylint tests
 ~~~
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.15 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.16 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -11,9 +11,9 @@
 Content-Type: text/markdown License-File: LICENSE # packg
           [build_3.7_status] [build_3.9_status] [coverage] [version]
 Collection of utilities used in other python projects. ## Features * `caching`:
 Cache objects to disk / to memory * `Const`: Base class for defining constants,
 as alternative to `enum.Enum` * `typext`: Type definitions * etc ## Install
 Requires `python>=3.7` ```bash pip install packg ``` ## Dev install Clone
 repository and cd into, then: ~~~bash pip install -e . pip install pytest
-pytest-cov pylint pytest-lazy-fixture pylint packg # run tests python -m pytest
---cov pylint tests ~~~
+pytest-cov pylint pytest-lazy-fixture python -m pytest --cov pylint packg
+pylint tests ~~~
```

### Comparing `packg-0.2.15/README.md` & `packg-0.2.16/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 ## Dev install
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint packg
 
-# run tests
 python -m pytest --cov
+
+pylint packg
 pylint tests
 ~~~
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # packg
           [build_3.7_status] [build_3.9_status] [coverage] [version]
 Collection of utilities used in other python projects. ## Features * `caching`:
 Cache objects to disk / to memory * `Const`: Base class for defining constants,
 as alternative to `enum.Enum` * `typext`: Type definitions * etc ## Install
 Requires `python>=3.7` ```bash pip install packg ``` ## Dev install Clone
 repository and cd into, then: ~~~bash pip install -e . pip install pytest
-pytest-cov pylint pytest-lazy-fixture pylint packg # run tests python -m pytest
---cov pylint tests ~~~
+pytest-cov pylint pytest-lazy-fixture python -m pytest --cov pylint packg
+pylint tests ~~~
```

### Comparing `packg-0.2.15/pyproject.toml` & `packg-0.2.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/caching.py` & `packg-0.2.16/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/constclass.py` & `packg-0.2.16/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/import_from_source.py` & `packg-0.2.16/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/iotools/__init__.py` & `packg-0.2.16/src/packg/iotools/__init__.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/iotools/jsonext.py` & `packg-0.2.16/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.16/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/iotools/misc.py` & `packg-0.2.16/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/iotools/yamlext.py` & `packg-0.2.16/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/log.py` & `packg-0.2.16/src/packg/log.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/paths.py` & `packg-0.2.16/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/system.py` & `packg-0.2.16/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/tensors.py` & `packg-0.2.16/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg/typext.py` & `packg-0.2.16/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.15/src/packg.egg-info/PKG-INFO` & `packg-0.2.16/src/packg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.15
+Version: 0.2.16
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -55,13 +55,13 @@
 ## Dev install
 
 Clone repository and cd into, then:
 
 ~~~bash
 pip install -e .
 pip install pytest pytest-cov pylint pytest-lazy-fixture
-pylint packg
 
-# run tests
 python -m pytest --cov
+
+pylint packg
 pylint tests
 ~~~
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.15 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.16 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -11,9 +11,9 @@
 Content-Type: text/markdown License-File: LICENSE # packg
           [build_3.7_status] [build_3.9_status] [coverage] [version]
 Collection of utilities used in other python projects. ## Features * `caching`:
 Cache objects to disk / to memory * `Const`: Base class for defining constants,
 as alternative to `enum.Enum` * `typext`: Type definitions * etc ## Install
 Requires `python>=3.7` ```bash pip install packg ``` ## Dev install Clone
 repository and cd into, then: ~~~bash pip install -e . pip install pytest
-pytest-cov pylint pytest-lazy-fixture pylint packg # run tests python -m pytest
---cov pylint tests ~~~
+pytest-cov pylint pytest-lazy-fixture python -m pytest --cov pylint packg
+pylint tests ~~~
```

### Comparing `packg-0.2.15/src/packg.egg-info/SOURCES.txt` & `packg-0.2.16/src/packg.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/packg/caching.py
 src/packg/constclass.py
 src/packg/dtime.py
 src/packg/import_from_source.py
 src/packg/log.py
 src/packg/misc.py
 src/packg/paths.py
+src/packg/strings.py
 src/packg/system.py
 src/packg/tensors.py
 src/packg/typext.py
 src/packg.egg-info/PKG-INFO
 src/packg.egg-info/SOURCES.txt
 src/packg.egg-info/dependency_links.txt
 src/packg.egg-info/requires.txt
```

