# Comparing `tmp/pycatsearch-5.1.7.tar.gz` & `tmp/pycatsearch-5.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.7.tar", last modified: Thu Jun 22 09:24:14 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.8.tar", last modified: Thu Jun 29 18:59:49 2023, max compression
```

## Comparing `pycatsearch-5.1.7.tar` & `pycatsearch-5.1.8.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    45337 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    25354 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.197547 pycatsearch-5.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.197547 pycatsearch-5.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.197547 pycatsearch-5.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.201547 pycatsearch-5.1.8/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45716 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/url_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.201547 pycatsearch-5.1.8/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/updater.py
```

### Comparing `pycatsearch-5.1.7/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/LICENSE.md` & `pycatsearch-5.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/PKG-INFO` & `pycatsearch-5.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.7
+Version: 5.1.8
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -81,14 +81,15 @@
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
   any_name: str = '',
   any_formula: str = '',
   any_name_or_formula: str = '',
+  anything: str = '',
   species_tag: int = 0,
   inchi: str = '',
   trivial_name: str = '',
   structural_formula: str = '',
   name: str = '',
   stoichiometric_formula: str = '',
   isotopolog: str = '',
@@ -102,14 +103,15 @@
     - `float max_intensity`: the maximal intensity \[log10(nm²×MHz)\] to take, use to avoid meta-stable substances.
     - `float temperature`: the temperature to calculate the line intensity at,
       use the catalog intensity if not set.
     - `str any_name`: a string to match the ``trivialname`` or the ``name`` field.
     - `str any_formula`: a string to match the ``structuralformula``, ``moleculesymbol``,
       ``stoichiometricformula``, or ``isotopolog`` field.
     - `str any_name_or_formula`: a string to match any field used by `any_name` and `any_formula`.
+    - `str anything`: a string to match any field at all.
     - `int species_tag`: a number to match the ``speciestag`` field.
     - `str inchi`: a string to match the ``inchikey`` field.
       See https://iupac.org/who-we-are/divisions/division-details/inchi/ for more.
     - `str trivial_name`: a string to match the ``trivialname`` field.
     - `str structural_formula`: a string to match the ``structuralformula`` field.
     - `str name`: a string to match the ``name`` field.
     - `str stoichiometric_formula`: a string to match the ``stoichiometricformula`` field.
```

### Comparing `pycatsearch-5.1.7/README.md` & `pycatsearch-5.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
   any_name: str = '',
   any_formula: str = '',
   any_name_or_formula: str = '',
+  anything: str = '',
   species_tag: int = 0,
   inchi: str = '',
   trivial_name: str = '',
   structural_formula: str = '',
   name: str = '',
   stoichiometric_formula: str = '',
   isotopolog: str = '',
@@ -70,14 +71,15 @@
     - `float max_intensity`: the maximal intensity \[log10(nm²×MHz)\] to take, use to avoid meta-stable substances.
     - `float temperature`: the temperature to calculate the line intensity at,
       use the catalog intensity if not set.
     - `str any_name`: a string to match the ``trivialname`` or the ``name`` field.
     - `str any_formula`: a string to match the ``structuralformula``, ``moleculesymbol``,
       ``stoichiometricformula``, or ``isotopolog`` field.
     - `str any_name_or_formula`: a string to match any field used by `any_name` and `any_formula`.
+    - `str anything`: a string to match any field at all.
     - `int species_tag`: a number to match the ``speciestag`` field.
     - `str inchi`: a string to match the ``inchikey`` field.
       See https://iupac.org/who-we-are/divisions/division-details/inchi/ for more.
     - `str trivial_name`: a string to match the ``trivialname`` field.
     - `str structural_formula`: a string to match the ``structuralformula`` field.
     - `str name`: a string to match the ``name`` field.
     - `str stoichiometric_formula`: a string to match the ``stoichiometricformula`` field.
```

### Comparing `pycatsearch-5.1.7/main.py` & `pycatsearch-5.1.8/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/pyproject.toml` & `pycatsearch-5.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/setup.py` & `pycatsearch-5.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.8/src/pycatsearch/async_downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/catalog.py` & `pycatsearch-5.1.8/src/pycatsearch/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -206,16 +206,17 @@
                max_frequency: float = math.inf,
                min_intensity: float = -math.inf,
                max_intensity: float = math.inf,
                temperature: float = -math.inf,
                any_name: str = '',
                any_formula: str = '',
                any_name_or_formula: str = '',
+               anything: str = '',
                species_tag: int = 0,
-               inchi: str = '',
+               inchi_key: str = '',
                trivial_name: str = '',
                structural_formula: str = '',
                name: str = '',
                stoichiometric_formula: str = '',
                isotopolog: str = '',
                state: str = '',
                degrees_of_freedom: Optional[int] = None,
@@ -230,17 +231,18 @@
         :param float max_intensity: the maximal intensity [log10(nm²×MHz)] to take, use to avoid meta-stable substances.
         :param float temperature: the temperature to calculate the line intensity at,
                                   use the catalog intensity if not set.
         :param str any_name: a string to match the ``trivialname`` or the ``name`` field.
         :param str any_formula: a string to match the ``structuralformula``, ``moleculesymbol``,
                                 ``stoichiometricformula``, or ``isotopolog`` field.
         :param str any_name_or_formula: a string to match any field used by :param:any_name and :param:any_formula.
+        :param str anything: a string to match any field at all.
         :param int species_tag: a number to match the ``speciestag`` field.
-        :param str inchi: a string to match the ``inchikey`` field.
-                          See https://iupac.org/who-we-are/divisions/division-details/inchi/ for more.
+        :param str inchi_key: a string to match the ``inchikey`` field.
+                              See https://iupac.org/who-we-are/divisions/division-details/inchi/ for more.
         :param str trivial_name: a string to match the ``trivialname`` field.
         :param str structural_formula: a string to match the ``structuralformula`` field.
         :param str name: a string to match the ``name`` field.
         :param str stoichiometric_formula: a string to match the ``stoichiometricformula`` field.
         :param str isotopolog: a string to match the ``isotopolog`` field.
         :param str state: a string to match the ``state`` or the ``state_html`` field.
         :param int degrees_of_freedom: 0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules.
@@ -274,60 +276,65 @@
             return new_catalog_entry
 
         if (min_frequency > max_frequency
                 or min_frequency > self.max_frequency
                 or max_frequency < self.min_frequency):
             return []
         start_time: float = time.monotonic()
-        if (species_tag or inchi or trivial_name or structural_formula or name or stoichiometric_formula
-                or isotopolog or state or degrees_of_freedom or any_name or any_formula or any_name_or_formula):
-            selected_entries = []
+        if (species_tag or inchi_key or trivial_name or structural_formula or name or stoichiometric_formula
+                or isotopolog or state or degrees_of_freedom or any_name or any_formula or any_name_or_formula
+                or anything):
+            trivial_name: str = trivial_name.casefold()
+            name: str = name.casefold()
+            any_name: str = any_name.casefold()
+            any_name_or_formula_lowercase: str = any_name_or_formula.casefold()
+            anything_lowercase: str = anything.casefold()
+            selected_entries: list[CatalogEntryType] = []
             for entry in self.catalog:
                 if timeout is not None and 0.0 < timeout <= time.monotonic() - start_time:
                     break
-                if ((not species_tag or (SPECIES_TAG in entry and entry[SPECIES_TAG] == species_tag))
-                        and (not inchi or (INCHI_KEY in entry and entry[INCHI_KEY] == inchi))
-                        and (not trivial_name
-                             or (TRIVIAL_NAME in entry and entry[TRIVIAL_NAME].casefold() == trivial_name.casefold()))
-                        and (not structural_formula
-                             or (STRUCTURAL_FORMULA in entry and entry[STRUCTURAL_FORMULA] == structural_formula))
-                        and (not name or (NAME in entry and entry[NAME].casefold() == name.casefold()))
+                if ((not species_tag or entry.get(SPECIES_TAG, 0) == species_tag)
+                        and (not inchi_key or entry.get(INCHI_KEY, '') == inchi_key)
+                        and (not trivial_name or entry.get(TRIVIAL_NAME, '').casefold() == trivial_name)
+                        and (not structural_formula or entry.get(STRUCTURAL_FORMULA, '') == structural_formula)
+                        and (not name or entry.get(NAME, '').casefold() == name)
                         and (not stoichiometric_formula
-                             or (STOICHIOMETRIC_FORMULA in entry
-                                 and entry[STOICHIOMETRIC_FORMULA] == stoichiometric_formula))
-                        and (not isotopolog or (ISOTOPOLOG in entry and entry[ISOTOPOLOG] == isotopolog))
-                        and (not state
-                             or (STATE in entry and entry[STATE] == state)
-                             or (STATE_HTML in entry and entry[STATE_HTML] == state))
-                        and (degrees_of_freedom is None
-                             or (DEGREES_OF_FREEDOM in entry and entry[DEGREES_OF_FREEDOM] == degrees_of_freedom))
+                             or entry.get(STOICHIOMETRIC_FORMULA, '') == stoichiometric_formula)
+                        and (not isotopolog or entry.get(ISOTOPOLOG, '') == isotopolog)
+                        and (not state or state in (entry.get(STATE, ''), entry.get(STATE_HTML, '')))
+                        and (degrees_of_freedom is None or entry.get(DEGREES_OF_FREEDOM, -1) == degrees_of_freedom)
                         and (not any_name
-                             or (TRIVIAL_NAME in entry and entry[TRIVIAL_NAME].casefold() == any_name.casefold())
-                             or (NAME in entry and entry[NAME].casefold() == any_name.casefold()))
+                             or any_name in (entry.get(TRIVIAL_NAME, '').casefold(),
+                                             entry.get(NAME, '').casefold(),))
                         and (not any_formula
-                             or (STRUCTURAL_FORMULA in entry and entry[STRUCTURAL_FORMULA] == any_formula)
-                             or (MOLECULE_SYMBOL in entry and entry[MOLECULE_SYMBOL] == any_formula)
-                             or (STOICHIOMETRIC_FORMULA in entry and entry[STOICHIOMETRIC_FORMULA] == any_formula)
-                             or (ISOTOPOLOG in entry and entry[ISOTOPOLOG] == any_formula))
+                             or any_formula in (entry.get(STRUCTURAL_FORMULA, ''),
+                                                entry.get(MOLECULE_SYMBOL, ''),
+                                                entry.get(STOICHIOMETRIC_FORMULA, ''),
+                                                entry.get(ISOTOPOLOG, ''),))
                         and (not any_name_or_formula
-                             or (TRIVIAL_NAME in entry
-                                 and entry[TRIVIAL_NAME].casefold() == any_name_or_formula.casefold())
-                             or (NAME in entry and entry[NAME].casefold() == any_name_or_formula.casefold())
-                             or (STRUCTURAL_FORMULA in entry and entry[STRUCTURAL_FORMULA] == any_name_or_formula)
-                             or (MOLECULE_SYMBOL in entry and entry[MOLECULE_SYMBOL] == any_name_or_formula)
-                             or (STOICHIOMETRIC_FORMULA in entry
-                                 and entry[STOICHIOMETRIC_FORMULA] == any_name_or_formula)
-                             or (ISOTOPOLOG in entry and entry[ISOTOPOLOG] == any_name_or_formula))):
-                    filtered_entry = filter_by_frequency_and_intensity(entry)
+                             or any_name_or_formula_lowercase in (entry.get(TRIVIAL_NAME, '').casefold(),
+                                                                  entry.get(NAME, '').casefold(),)
+                             or any_name_or_formula in (entry.get(STRUCTURAL_FORMULA, ''),
+                                                        entry.get(MOLECULE_SYMBOL, ''),
+                                                        entry.get(STOICHIOMETRIC_FORMULA, ''),
+                                                        entry.get(ISOTOPOLOG, ''),))
+                        and (not anything
+                             or anything in (str(entry[key]) for key in entry if key != LINES)
+                             or anything_lowercase in (entry.get(TRIVIAL_NAME, '').casefold(),
+                                                       entry.get(NAME, '').casefold(),))
+                ):
+                    filtered_entry: CatalogEntryType = filter_by_frequency_and_intensity(entry)
                     if filtered_entry[LINES]:
                         selected_entries.append(filtered_entry)
         else:
-            filtered_entries = [filter_by_frequency_and_intensity(entry)
-                                for entry in self._data.catalog
-                                if timeout is None or (timeout > 0.0 and timeout >= time.monotonic() - start_time)]
+            filtered_entries: list[CatalogEntryType] = [
+                filter_by_frequency_and_intensity(entry)
+                for entry in self._data.catalog
+                if timeout is None or (timeout > 0.0 and timeout >= time.monotonic() - start_time)
+            ]
             selected_entries = [entry for entry in filtered_entries if entry[LINES]]
         return selected_entries
 
     def print(self, **kwargs: None | int | float | str) -> None:
         """
         Print a table of the filtered catalog entries
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.8/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/downloader.py` & `pycatsearch-5.1.8/src/pycatsearch/downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/__init__.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/catalog_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def rowCount(self, parent: QModelIndex | QPersistentModelIndex = QModelIndex()) -> int:
         return len(self._data)
 
     def columnCount(self, parent: QModelIndex | QPersistentModelIndex = QModelIndex()) -> int:
         return 1 if all(info.build_datetime is None for info in self._data) else 2
 
-    def data(self, index: QModelIndex, role: int = Qt.ItemDataRole.DisplayRole) -> str | None:
+    def data(self, index: QModelIndex | QPersistentModelIndex, role: int = Qt.ItemDataRole.DisplayRole) -> str | None:
         if index.isValid() and role == Qt.ItemDataRole.DisplayRole:
             if index.column() == 0:
                 return self._data[index.row()].filename
             if index.column() == 1:
                 info: CatalogSourceInfo = self._data[index.row()]
                 if info.build_datetime is None:
                     return None
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/frequency_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/preferences.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,34 +16,39 @@
 
 
 class PreferencesPage(QWidget):
     """ A page of the Preferences dialog """
 
     def __init__(self, value: dict[str, (Settings.CallbackOnly
                                          | Settings.SpinboxAndCallback
-                                         | Settings.ComboboxAndCallback)],
+                                         | Settings.ComboboxAndCallback
+                                         | Settings.EditableComboboxAndCallback)],
                  settings: Settings, parent: QWidget | None = None) -> None:
         super().__init__(parent)
 
         self.settings: Settings = settings
         logger: logging.Logger = logging.getLogger('preferences')
 
         if not (isinstance(value, dict) and value):
             raise TypeError(f'Invalid type: {type(value)}')
         layout: QFormLayout = QFormLayout(self)
         key2: str
-        value2: Settings.CallbackOnly | Settings.SpinboxAndCallback | Settings.ComboboxAndCallback
+        value2: (Settings.CallbackOnly
+                 | Settings.SpinboxAndCallback
+                 | Settings.ComboboxAndCallback
+                 | Settings.EditableComboboxAndCallback)
 
         check_box: QCheckBox
         spin_box: QSpinBox | QDoubleSpinBox
+        combo_box: QComboBox
 
         for key2, value2 in value.items():
             if isinstance(value2, Settings.CallbackOnly):
                 if isinstance(getattr(self.settings, value2.callback), bool):
-                    check_box: QCheckBox = QCheckBox(self.tr(key2), self)
+                    check_box = QCheckBox(self.tr(key2), self)
                     setattr(check_box, 'callback', value2.callback)
                     check_box.setChecked(getattr(self.settings, value2.callback))
                     check_box.toggled.connect(partial(self._on_event, sender=check_box))
                     layout.addWidget(check_box)
                 else:
                     logger.error(f'The type of {value2.callback!r} is not supported')
             elif isinstance(value2, Settings.SpinboxAndCallback):
@@ -56,32 +61,46 @@
                 spin_box.setSingleStep(value2.range.step or 1)
                 spin_box.setPrefix(value2.prefix_and_suffix[0])
                 spin_box.setSuffix(value2.prefix_and_suffix[1])
                 setattr(spin_box, 'callback', value2.callback)
                 spin_box.valueChanged.connect(partial(self._on_event, sender=spin_box))
                 layout.addRow(key2, spin_box)
             elif isinstance(value2, Settings.ComboboxAndCallback):
-                combo_box: QComboBox = QComboBox(self)
+                combo_box = QComboBox(self)
                 setattr(combo_box, 'callback', value2.callback)
                 combobox_data: dict[Hashable, str]
                 if isinstance(value2.combobox_data, dict):
                     combobox_data = value2.combobox_data
                 else:
                     combobox_data = dict(enumerate(value2.combobox_data))
                 for index, (data, item) in enumerate(combobox_data.items()):
                     combo_box.addItem(self.tr(item), data)
+                combo_box.setEditable(False)
                 combo_box.setCurrentText(combobox_data[getattr(self.settings, value2.callback)])
                 combo_box.currentIndexChanged.connect(
                     partial(self._on_combo_box_current_index_changed, sender=combo_box))
                 layout.addRow(self.tr(key2), combo_box)
+            elif isinstance(value2, Settings.EditableComboboxAndCallback):
+                combo_box = QComboBox(self)
+                setattr(combo_box, 'callback', value2.callback)
+                combo_box.addItems(value2.combobox_items)
+                current_text: str = getattr(self.settings, value2.callback)
+                if current_text in value2.combobox_items:
+                    combo_box.setCurrentIndex(value2.combobox_items.index(current_text))
+                else:
+                    combo_box.insertItem(0, current_text)
+                    combo_box.setCurrentIndex(0)
+                combo_box.setEditable(True)
+                combo_box.currentTextChanged.connect(partial(self._on_event, sender=combo_box))
+                layout.addRow(self.tr(key2), combo_box)
             else:
                 logger.error(f'{value2!r} is not supported')
 
     # https://forum.qt.io/post/671245
-    def _on_event(self, x: bool | int | float, sender: QWidget) -> None:
+    def _on_event(self, x: bool | int | float | str, sender: QWidget) -> None:
         setattr(self.settings, getattr(sender, 'callback'), x)
 
     def _on_combo_box_current_index_changed(self, _: int, sender: QComboBox) -> None:
         setattr(self.settings, getattr(sender, 'callback'), sender.currentData())
 
 
 class PreferencesBody(QScrollArea):
@@ -104,15 +123,16 @@
 
         layout: QHBoxLayout = QHBoxLayout(widget)
         content: QListWidget = QListWidget(widget)
         stack: QStackedWidget = QStackedWidget(widget)
         key: str | tuple[str, tuple[str, ...]] | tuple[str, tuple[str, ...], tuple[tuple[str, Any], ...]]
         value: dict[str, (Settings.CallbackOnly
                           | Settings.SpinboxAndCallback
-                          | Settings.ComboboxAndCallback)]
+                          | Settings.ComboboxAndCallback
+                          | Settings.EditableComboboxAndCallback)]
         for key, value in self.settings.dialog.items():
             if not (isinstance(value, dict) and value):
                 logger.error(f'Invalid value of {key!r}')
                 continue
             new_item: QListWidgetItem
             if isinstance(key, str):
                 new_item = QListWidgetItem(key)
@@ -153,15 +173,15 @@
         self.setWindowTitle(self.tr('Preferences'))
         if parent is not None:
             self.setWindowIcon(parent.windowIcon())
 
         layout: QVBoxLayout = QVBoxLayout(self)
         layout.addWidget(PreferencesBody(settings=settings, parent=parent))
         buttons: QDialogButtonBox = QDialogButtonBox(QDialogButtonBox.StandardButton.Close, self)
-        buttons.rejected.connect(self.reject)
+        buttons.rejected.connect(self.close)
         layout.addWidget(buttons)
 
         self.settings.beginGroup('PreferencesDialog')
         self.restoreGeometry(cast(QByteArray, self.settings.value('windowGeometry', QByteArray())))
         self.settings.endGroup()
 
     def closeEvent(self, event: QCloseEvent) -> None:
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
-from typing import Any, Callable, Final, Hashable, Iterable, NamedTuple
+from typing import Any, Callable, Final, Hashable, Iterable, NamedTuple, Sequence
 
 from qtpy.QtCore import QObject, QSettings
 
 from ..utils import *
 
 __all__ = ['Settings']
 
@@ -22,14 +22,18 @@
         prefix_and_suffix: tuple[str, str]
         callback: str
 
     class ComboboxAndCallback(NamedTuple):
         combobox_data: Iterable[str] | dict[Hashable, str]
         callback: str
 
+    class EditableComboboxAndCallback(NamedTuple):
+        combobox_items: Sequence[str]
+        callback: str
+
     TO_MHZ: Final[list[Callable[[float], float]]] = [lambda x: x, ghz_to_mhz, rec_cm_to_mhz, nm_to_mhz]
     FROM_MHZ: Final[list[Callable[[float], float]]] = [lambda x: x, mhz_to_ghz, mhz_to_rec_cm, mhz_to_nm]
 
     TO_LOG10_SQ_NM_MHZ: Final[list[Callable[[float], float]]] = [
         lambda x: x,
         sq_nm_mhz_to_log10_sq_nm_mhz,
         log10_cm_per_molecule_to_log10_sq_nm_mhz,
@@ -52,14 +56,24 @@
         rec_cm_to_meV,
         rec_cm_to_j
     ]
 
     TO_K: Final[list[Callable[[float], float]]] = [lambda x: x, lambda x: x + 273.15]
     FROM_K: Final[list[Callable[[float], float]]] = [lambda x: x, lambda x: x - 273.15]
 
+    INCHI_KEY_SEARCH_PROVIDERS: Final[list[str]] = [
+        'https://pubchem.ncbi.nlm.nih.gov/#query={InChIKey}',
+        'https://www.ebi.ac.uk/unichem/compoundsources?type=inchikey&compound={InChIKey}',
+        'https://webbook.nist.gov/cgi/cbook.cgi?InChI={InChIKey}',
+        'https://www.spectrabase.com/search?q={InChIKey}',
+        'https://www.google.com/search?q={InChIKey}',
+        'http://gmd.mpimp-golm.mpg.de/search.aspx?query={InChIKey}',
+        'http://www.chemspider.com/InChIKey/{InChIKey}',
+    ]
+
     def __init__(self, organization: str, application: str, parent: QObject | None = None) -> None:
         super().__init__(organization, application, parent)
 
         # for some reason, the dicts are not being translated when used as class variables
         self.LINE_ENDS: Final[dict[str, str]] = {
             '\n': self.tr(r'Line Feed (\n)'),
             '\r': self.tr(r'Carriage Return (\r)'),
@@ -78,17 +92,17 @@
         self.ENERGY_UNITS: Final[list[str]] = [self.tr('cm⁻¹'), self.tr('meV'), self.tr('J')]
         self.TEMPERATURE_UNITS: Final[list[str]] = [self.tr('K'), self.tr('°C')]
 
     @property
     def dialog(self) -> (dict[(str
                                | tuple[str, tuple[str, ...]]
                                | tuple[str, tuple[str, ...], tuple[tuple[str, Any], ...]]),
-                              dict[str, (Settings.CallbackOnly
-                                         | Settings.SpinboxAndCallback
-                                         | Settings.ComboboxAndCallback)]]):
+    dict[str, (Settings.CallbackOnly
+               | Settings.SpinboxAndCallback
+               | Settings.ComboboxAndCallback)]]):
         return {
             (self.tr('When the program starts'), ('mdi6.rocket-launch',)): {
                 self.tr('Load catalogs'): Settings.CallbackOnly('load_last_catalogs'),
                 self.tr('Check for update'): Settings.CallbackOnly('check_updates'),
             },
             (self.tr('Display'), ('mdi6.binoculars',)): {
                 self.tr('Allow rich text in formulas'): Settings.CallbackOnly('rich_text_in_formulas'),
@@ -102,15 +116,23 @@
                 self.tr('Energy:'): Settings.ComboboxAndCallback(self.ENERGY_UNITS, 'energy_unit'),
                 self.tr('Temperature:'): Settings.ComboboxAndCallback(self.TEMPERATURE_UNITS, 'temperature_unit'),
             },
             (self.tr('Export'), ('mdi6.file-export',)): {
                 self.tr('With units'): Settings.CallbackOnly('with_units'),
                 self.tr('Line ending:'): Settings.ComboboxAndCallback(self.LINE_ENDS, 'line_end'),
                 self.tr('CSV separator:'): Settings.ComboboxAndCallback(self.CSV_SEPARATORS, 'csv_separator'),
-            }
+            },
+            (
+                self.tr('Info'),
+                ('mdi6.flask-empty-outline', 'mdi6.information-variant'),
+                (('options', ((), (('scale_factor', 0.5),))),)
+            ): {
+                self.tr('InChI key search URL:'): Settings.EditableComboboxAndCallback(self.INCHI_KEY_SEARCH_PROVIDERS,
+                                                                                       'inchi_key_search_url_template'),
+            },
         }
 
     @property
     def frequency_unit(self) -> int:
         self.beginGroup('frequency')
         v: int = self.value('unit', 0, int)
         self.endGroup()
@@ -352,7 +374,20 @@
         return v
 
     @ignored_version.setter
     def ignored_version(self, new_value: str) -> None:
         self.beginGroup('update')
         self.setValue('ignoredVersion', new_value)
         self.endGroup()
+
+    @property
+    def inchi_key_search_url_template(self) -> str:
+        self.beginGroup('info')
+        v: str = self.value('InChIKeySearchURLTemplate', 'https://pubchem.ncbi.nlm.nih.gov/#query={InChIKey}', str)
+        self.endGroup()
+        return v
+
+    @inchi_key_search_url_template.setter
+    def inchi_key_search_url_template(self, new_value: str) -> None:
+        self.beginGroup('info')
+        self.setValue('InChIKeySearchURLTemplate', new_value)
+        self.endGroup()
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/substance_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from typing import Collection
 
 from qtpy.QtCore import QModelIndex, Qt, Slot
 from qtpy.QtWidgets import (QDialog, QDialogButtonBox, QFormLayout, QLabel, QListWidget, QListWidgetItem, QVBoxLayout,
                             QWidget)
 
 from .selectable_label import SelectableLabel
+from .url_label import URLLabel
 from ..catalog import Catalog
 from ..utils import *
 
 __all__ = ['SubstanceInfoSelector', 'SubstanceInfo']
 
 
 class SubstanceInfoSelector(QDialog):
     def __init__(self, catalog: Catalog, entry_ids: Collection[int],
-                 allow_html: bool = True, parent: QWidget | None = None) -> None:
+                 allow_html: bool = True, inchi_key_search_url_template: str = '',
+                 parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self._catalog: Catalog = catalog
+        self._inchi_key_search_url_template: str = inchi_key_search_url_template
         self.setModal(True)
         self.setWindowTitle(self.tr('Select Substance'))
         if parent is not None:
             self.setWindowIcon(parent.windowIcon())
         layout: QVBoxLayout = QVBoxLayout(self)
         self._list_box: QListWidget = QListWidget(self)
         self._list_box.itemSelectionChanged.connect(self._on_list_selection_changed)
@@ -51,52 +54,64 @@
     def _on_list_selection_changed(self) -> None:
         self._buttons.button(QDialogButtonBox.StandardButton.Ok).setEnabled(bool(self._list_box.selectedIndexes()))
 
     @Slot(QModelIndex)
     def _on_list_double_clicked(self, index: QModelIndex) -> None:
         self.hide()
         item: QListWidgetItem = self._list_box.item(index.row())
-        syn: SubstanceInfo = SubstanceInfo(self._catalog, item.data(Qt.ItemDataRole.UserRole), self.parent())
+        syn: SubstanceInfo = SubstanceInfo(self._catalog, item.data(Qt.ItemDataRole.UserRole),
+                                           inchi_key_search_url_template=self._inchi_key_search_url_template,
+                                           parent=self.parent())
         syn.exec()
         self.accept()
 
     @Slot()
     def _on_accept(self) -> None:
         selected_items: list[QListWidgetItem] = self._list_box.selectedItems()
         if not selected_items:
             return
         self.hide()
         item: QListWidgetItem = selected_items.pop()
-        syn: SubstanceInfo = SubstanceInfo(self._catalog, item.data(Qt.ItemDataRole.UserRole), self.parent())
+        syn: SubstanceInfo = SubstanceInfo(self._catalog, item.data(Qt.ItemDataRole.UserRole),
+                                           inchi_key_search_url_template=self._inchi_key_search_url_template,
+                                           parent=self.parent())
         syn.exec()
         self.accept()
 
 
 class SubstanceInfo(QDialog):
     """ A simple dialog that displays the information about a substance from the loaded catalog """
 
-    def __init__(self, catalog: Catalog, entry_id: int, parent: QWidget | None = None) -> None:
+    def __init__(self, catalog: Catalog, entry_id: int, inchi_key_search_url_template: str = '',
+                 parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.setModal(True)
         self.setWindowTitle(self.tr('Substance Info'))
         if parent is not None:
             self.setWindowIcon(parent.windowIcon())
         layout: QFormLayout = QFormLayout(self)
         label: SelectableLabel
         for entry in catalog.catalog:
             if entry[ID] == entry_id:
                 for key in entry:
                     if key == LINES:
                         continue
+                    elif key == ID:
+                        label = URLLabel(
+                            url=f'https://cdms.astro.uni-koeln.de/cdms/portal/catalog/{entry[key]}/',
+                            text=f'{entry[key]}',
+                            parent=self)
+                        label.setOpenExternalLinks(True)
                     elif key == STATE_HTML:
                         label = SelectableLabel(chem_html(str(entry[key])), self)
-                    elif key == INCHI_KEY:
-                        label = SelectableLabel(
-                            f'<a href="https://pubchem.ncbi.nlm.nih.gov/#query={entry[key]}">{entry[key]}</a>',
-                            self)
+                    elif key == INCHI_KEY and inchi_key_search_url_template:
+                        label = URLLabel(
+                            url=inchi_key_search_url_template.format(InChIKey=entry[key]),
+                            text=entry[key],
+                            parent=self)
                         label.setOpenExternalLinks(True)
                     else:
                         label = SelectableLabel(str(entry[key]), self)
                     layout.addRow(self.tr(HUMAN_READABLE[key]), label)
                 break
         buttons: QDialogButtonBox = QDialogButtonBox(QDialogButtonBox.StandardButton.Close, self)
         buttons.rejected.connect(self.reject)
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/substances_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,18 +93,29 @@
                     if (name_key in entry
                             and (filter_text in plain_text_name
                                  or (name_key in (NAME, TRIVIAL_NAME)
                                      and filter_text_lowercase in plain_text_name.casefold()))):
                         if plain_text_name not in list_items:
                             list_items[plain_text_name] = set()
                         list_items[plain_text_name].add(entry[ID])
+            # species tag suspected
             if filter_text.isdecimal():
                 for entry in self._catalog.catalog:
-                    plain_text_name = str(entry[SPECIES_TAG])
-                    if SPECIES_TAG in entry and plain_text_name.startswith(filter_text):
+                    plain_text_name = str(entry.get(SPECIES_TAG, ''))
+                    if plain_text_name.startswith(filter_text):
+                        if plain_text_name not in list_items:
+                            list_items[plain_text_name] = set()
+                        list_items[plain_text_name].add(entry[ID])
+            # InChI Key match, see https://en.wikipedia.org/wiki/International_Chemical_Identifier#InChIKey
+            if (len(filter_text) == 27
+                    and filter_text[14] == '-' and filter_text[25] == '-'
+                    and filter_text.count('-') == 2):
+                for entry in self._catalog.catalog:
+                    plain_text_name = str(entry.get(INCHI_KEY, ''))
+                    if plain_text_name == filter_text:
                         if plain_text_name not in list_items:
                             list_items[plain_text_name] = set()
                         list_items[plain_text_name].add(entry[ID])
         else:
             for name_key in (ISOTOPOLOG, NAME, STRUCTURAL_FORMULA,
                              STOICHIOMETRIC_FORMULA, TRIVIAL_NAME):
                 for entry in self._catalog.catalog:
@@ -148,20 +159,26 @@
         for i in range(self._list_substance.count()):
             self._list_substance.item(i).setCheckState(Qt.CheckState.Unchecked)
         self._selected_substances.clear()
 
     @Slot(QModelIndex)
     def _on_list_substance_double_clicked(self, index: QModelIndex) -> None:
         item: QListWidgetItem = self._list_substance.item(index.row())
-        ids: set[int] = item.data(Qt.ItemDataRole.UserRole)
+        ids: set[int] = item.data(Qt.ItemDataRole.UserRole).copy()
         if len(ids) > 1:
-            sis: SubstanceInfoSelector = SubstanceInfoSelector(self.catalog, ids, parent=self)
+            sis: SubstanceInfoSelector = SubstanceInfoSelector(
+                self.catalog, ids,
+                inchi_key_search_url_template=self._settings.inchi_key_search_url_template,
+                parent=self)
             sis.exec()
         elif ids:  # if not empty
-            syn: SubstanceInfo = SubstanceInfo(self.catalog, ids.pop(), parent=self)
+            syn: SubstanceInfo = SubstanceInfo(
+                self.catalog, ids.pop(),
+                inchi_key_search_url_template=self._settings.inchi_key_search_url_template,
+                parent=self)
             syn.exec()
 
     def load_settings(self) -> None:
         self._settings.beginGroup('search')
         self._settings.beginGroup('selection')
         self._text_substance.setText(self._settings.value('filter', self._text_substance.text(), str))
         self._check_keep_selection.setChecked(self._settings.value('isPersistent', False, bool))
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import math
 from typing import Any, Callable, Final, final
 
-from qtpy.QtCore import (QAbstractTableModel, QByteArray, QItemSelection, QMimeData, QModelIndex, QPoint, QPointF,
-                         QRect, QSize, Qt, Slot)
+from qtpy.QtCore import (QAbstractTableModel, QByteArray, QItemSelection, QMimeData, QModelIndex, QPersistentModelIndex,
+                         QPoint, QPointF, QRect, QSize, Qt, Slot)
 from qtpy.QtGui import (QAbstractTextDocumentLayout, QClipboard, QCloseEvent, QCursor, QIcon, QPainter, QPixmap,
                         QScreen, QTextDocument)
 from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QHeaderView,
                             QMainWindow, QMessageBox, QPushButton, QSplitter, QStatusBar, QStyle, QStyleOptionViewItem,
                             QStyledItemDelegate, QTableView, QVBoxLayout, QWidget)
 from qtpy.compat import getopenfilenames
 
@@ -55,15 +55,15 @@
     @staticmethod
     def anchorAt(html: str, point: QPoint | QPointF) -> str:
         doc: QTextDocument = QTextDocument()
         doc.setHtml(html)
         text_layout: QAbstractTextDocumentLayout = doc.documentLayout()
         return text_layout.anchorAt(point)
 
-    def paint(self, painter: QPainter, option: QStyleOptionViewItem, index: QModelIndex) -> None:
+    def paint(self, painter: QPainter, option: QStyleOptionViewItem, index: QModelIndex | QPersistentModelIndex) -> None:
         self.initStyleOption(option, index)
         style: QStyle
         if option.widget:
             style = option.widget.style()
         else:
             style = QApplication.style()
         doc: QTextDocument = QTextDocument()
@@ -75,15 +75,15 @@
         painter.save()
         painter.translate(text_rect.topLeft())
         painter.setClipRect(text_rect.translated(-text_rect.topLeft()))
         painter.translate(0, 0.5 * (option.rect.height() - doc.size().height()))
         doc.documentLayout().draw(painter, ctx)
         painter.restore()
 
-    def sizeHint(self, option: QStyleOptionViewItem | None, index: QModelIndex) -> QSize:
+    def sizeHint(self, option: QStyleOptionViewItem | None, index: QModelIndex | QPersistentModelIndex) -> QSize:
         options: QStyleOptionViewItem = QStyleOptionViewItem(option)
         self.initStyleOption(options, index)
         doc: QTextDocument = QTextDocument()
         doc.setHtml(options.text)
         doc.setTextWidth(options.rect.width())
         return QSize(round(doc.idealWidth()), round(doc.size().height()))
 
@@ -108,14 +108,16 @@
             self.frequency: float = frequency
             self.intensity_str: str = intensity_str
             self.intensity: float = intensity
             self.lower_state_energy_str: str = lower_state_energy_str
             self.lower_state_energy: float = lower_state_energy
 
         def __eq__(self, other: LinesListModel.DataType) -> int:
+            if not isinstance(other, LinesListModel.DataType):
+                return NotImplemented
             return (self.id == other.id
                     and self.frequency == other.frequency
                     and self.intensity == other.intensity
                     and self.lower_state_energy == other.lower_state_energy)
 
         def __hash__(self) -> int:
             return hash(self.id) ^ hash(self.frequency) ^ hash(self.lower_state_energy)
@@ -137,21 +139,21 @@
 
     def update_units(self) -> None:
         unit_format: Final[str] = self.tr('{0} [{1}]', 'unit format')
         self._header[1] = substitute(unit_format, self.tr("Frequency"), self._settings.frequency_unit_str)
         self._header[2] = substitute(unit_format, self.tr("Intensity"), self._settings.intensity_unit_str)
         self._header[3] = substitute(unit_format, self.tr("Lower state energy"), self._settings.energy_unit_str)
 
-    def rowCount(self, parent: QModelIndex = ...) -> int:
+    def rowCount(self, parent: QModelIndex | QPersistentModelIndex = ...) -> int:
         return min(len(self._data), self._rows_loaded)
 
-    def columnCount(self, parent: QModelIndex = ...) -> int:
+    def columnCount(self, parent: QModelIndex | QPersistentModelIndex = ...) -> int:
         return len(self._header)
 
-    def data(self, index: QModelIndex, role: int = Qt.ItemDataRole.DisplayRole) -> str | None:
+    def data(self, index: QModelIndex | QPersistentModelIndex, role: int = Qt.ItemDataRole.DisplayRole) -> str | None:
         if index.isValid():
             if role == Qt.ItemDataRole.DisplayRole:
                 item: LinesListModel.DataType = self._data[index.row()]
                 column_index: int = index.column()
                 if column_index == 0:
                     return item.name
                 if column_index == 1:
@@ -256,18 +258,18 @@
             1: (lambda l: (l.frequency, l.intensity, l.name, l.lower_state_energy)),
             2: (lambda l: (l.intensity, l.frequency, l.name, l.lower_state_energy)),
             3: (lambda l: (l.lower_state_energy, l.intensity, l.frequency, l.name))
         }[column]
         self._data.sort(key=key, reverse=bool(order != Qt.SortOrder.AscendingOrder))
         self.endResetModel()
 
-    def canFetchMore(self, index: QModelIndex = QModelIndex()) -> bool:
+    def canFetchMore(self, index: QModelIndex | QPersistentModelIndex = QModelIndex()) -> bool:
         return len(self._data) > self._rows_loaded
 
-    def fetchMore(self, index: QModelIndex = QModelIndex()) -> None:
+    def fetchMore(self, index: QModelIndex | QPersistentModelIndex = QModelIndex()) -> None:
         # https://sateeshkumarb.wordpress.com/2012/04/01/paginated-display-of-table-data-in-pyqt/
         remainder: int = len(self._data) - self._rows_loaded
         items_to_fetch: int = min(remainder, LinesListModel.ROW_BATCH_COUNT)
         self.beginInsertRows(QModelIndex(), self._rows_loaded, self._rows_loaded + items_to_fetch - 1)
         self._rows_loaded += items_to_fetch
         self.endInsertRows()
 
@@ -680,15 +682,16 @@
 
     @Slot()
     def _on_action_substance_info_triggered(self) -> None:
         if self.results_table.selectionModel().selectedRows():
             syn: SubstanceInfo = SubstanceInfo(
                 self.catalog,
                 self.results_model.row(self.results_table.selectionModel().selectedRows()[0].row()).id,
-                self)
+                inchi_key_search_url_template=self.settings.inchi_key_search_url_template,
+                parent=self)
             syn.exec()
 
     def toggle_results_table_column_visibility(self, column: int, is_visible: bool) -> None:
         if is_visible != self.results_table.isColumnHidden(column):
             return
         if is_visible:
             self.results_table.showColumn(column)
@@ -883,15 +886,15 @@
 
         entries: list[dict[str, int | str | list[dict[str, float]]]] = \
             (sum(
                 (
                     self.catalog.filter(min_frequency=self.box_frequency.min_frequency,
                                         max_frequency=self.box_frequency.max_frequency,
                                         min_intensity=self.minimal_intensity,
-                                        any_name_or_formula=name,
+                                        anything=name,
                                         temperature=self.temperature,
                                         timeout=self.settings.timeout)
                     for name in self.box_substance.selected_substances
                 ),
                 []
             ) if self.box_substance.selected_substances and self.box_substance.isChecked()
              else self.catalog.filter(min_frequency=self.box_frequency.min_frequency,
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.8/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.7/src/pycatsearch/utils.py` & `pycatsearch-5.1.8/src/pycatsearch/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-import builtins
 import html
 import html.entities
 import itertools
 import math
 import os
 import sys
 from numbers import Real
@@ -29,16 +28,15 @@
            'sq_nm_mhz_to_log10_sq_nm_mhz',
            'log10_cm_per_molecule_to_log10_sq_nm_mhz',
            'cm_per_molecule_to_log10_sq_nm_mhz',
            'sort_unique', 'merge_sorted', 'search_sorted',
            'within', 'chem_html', 'best_name', 'remove_html', 'wrap_in_html',
            'ensure_prefix', 'all_cases',
            'save_catalog_to_file',
-           'ReleaseInfo', 'latest_release', 'update_with_pip',
-           'zip']
+           'ReleaseInfo', 'latest_release', 'update_with_pip']
 
 M_LOG10E: Final[float] = math.log10(math.e)
 
 T0: Final[float] = 300.00  # [K], see https://spec.jpl.nasa.gov/ftp/pub/catalog/doc/catdoc.pdf
 k: Final[float] = 1.380649000e-23  # [J/K],  see https://physics.nist.gov/cgi-bin/cuu/Value?k
 h: Final[float] = 6.626070150e-34  # [J/Hz], see https://physics.nist.gov/cgi-bin/cuu/Value?h
 e: Final[float] = 1.602176634e-19  # [C],    see https://physics.nist.gov/cgi-bin/cuu/Value?e
@@ -91,15 +89,15 @@
     LOWER_STATE_ENERGY: 'Lower state energy',
 }
 
 
 def within(x: float, limits: tuple[float, float] | tuple[tuple[float, float], ...]) -> bool:
     if len(limits) < 2:
         raise ValueError('Invalid limits')
-    if all(isinstance(cast(float, limit), Real) for limit in limits):
+    if all(isinstance(limit, Real) for limit in limits):
         return min(limits) <= x <= max(limits)
     elif all(isinstance(limit, tuple) for limit in limits):
         return any(min(limit) <= x <= max(limit) for limit in limits)
     else:
         raise TypeError('Invalid limits type')
 
 
@@ -468,59 +466,59 @@
     """ Basic check that all tags are sound """
     _1, _2, _3 = text.count('<'), text.count('>'), 2 * text.count('</')
     return _1 == _2 and _1 == _3
 
 
 def best_name(entry: dict[str, int | str | list[dict[str, float]]],
               allow_html: bool = True) -> str:
-    last: str = best_name.__dict__.get('last', dict()).get(entry[SPECIES_TAG], dict()).get(allow_html, '')
+    species_tag: int = cast(int, entry.get(SPECIES_TAG, 0))
+    last: str = best_name.__dict__.get('last', dict()).get(species_tag, dict()).get(allow_html, '')
     if last:
         return last
 
     def _best_name() -> str:
-        if allow_html and ISOTOPOLOG in entry and entry[ISOTOPOLOG]:
+        if isotopolog := entry.get(ISOTOPOLOG, ''):
             if allow_html:
-                if (is_good_html(str(entry[MOLECULE_SYMBOL]))
-                        and ((STRUCTURAL_FORMULA in entry and entry[STRUCTURAL_FORMULA] == entry[ISOTOPOLOG])
-                             or (STOICHIOMETRIC_FORMULA in entry
-                                 and entry[STOICHIOMETRIC_FORMULA] == entry[ISOTOPOLOG]))):
-                    if STATE_HTML in entry and entry[STATE_HTML]:
+                if (is_good_html(str(molecule_symbol := entry[MOLECULE_SYMBOL]))
+                        and (entry.get(STRUCTURAL_FORMULA, '') == isotopolog
+                             or entry.get(STOICHIOMETRIC_FORMULA, '') == isotopolog)):
+                    if state_html := cast(str, entry.get(STATE_HTML, '')):
                         # span tags are needed when the molecule symbol is malformed
-                        return f'<span>{entry[MOLECULE_SYMBOL]}</span>, ' \
-                               f'{chem_html(tex_to_html_entity(str(entry[STATE_HTML])))}'
-                    return str(entry[MOLECULE_SYMBOL])
+                        return f'<span>{molecule_symbol}</span>, ' \
+                               f'{chem_html(tex_to_html_entity(str(state_html)))}'
+                    return str(molecule_symbol)
                 else:
-                    if STATE_HTML in entry and entry[STATE_HTML]:
-                        return f'{chem_html(str(entry[ISOTOPOLOG]))}, ' \
-                               f'{chem_html(tex_to_html_entity(str(entry[STATE_HTML])))}'
-                    return chem_html(str(entry[ISOTOPOLOG]))
+                    if state_html := cast(str, entry.get(STATE_HTML, '')):
+                        return f'{chem_html(str(isotopolog))}, ' \
+                               f'{chem_html(tex_to_html_entity(str(state_html)))}'
+                    return chem_html(str(isotopolog))
             else:
-                if STATE_HTML in entry and entry[STATE_HTML]:
-                    return f'{entry[ISOTOPOLOG]}, {remove_html(tex_to_html_entity(entry[STATE_HTML]))}'
-                if STATE in entry and entry[STATE]:
-                    return f'{entry[ISOTOPOLOG]}, {remove_html(tex_to_html_entity(entry[STATE].strip("$")))}'
-                return entry[ISOTOPOLOG]
+                if state_html := cast(str, entry.get(STATE_HTML, '')):
+                    return f'{isotopolog}, {remove_html(tex_to_html_entity(state_html))}'
+                if state := cast(str, entry.get(STATE, '')):
+                    return f'{isotopolog}, {remove_html(tex_to_html_entity(state.strip("$")))}'
+                return isotopolog
 
         for key in (NAME, STRUCTURAL_FORMULA, STOICHIOMETRIC_FORMULA):
-            if key in entry and entry[key]:
-                return chem_html(str(entry[key])) if allow_html else str(entry[key])
-        if TRIVIAL_NAME in entry and entry[TRIVIAL_NAME]:
-            return str(entry[TRIVIAL_NAME])
-        if SPECIES_TAG in entry and entry[SPECIES_TAG]:
-            return str(entry[SPECIES_TAG])
+            if candidate := entry.get(key, ''):
+                return chem_html(str(candidate)) if allow_html else str(candidate)
+        if trivial_name := entry.get(TRIVIAL_NAME, ''):
+            return str(trivial_name)
+        if species_tag:
+            return str(species_tag)
         return 'no name'
 
     res: str = _best_name()
-    if SPECIES_TAG not in entry:
+    if not species_tag:
         return res
     if 'last' not in best_name.__dict__:
         best_name.__dict__['last'] = dict()
-    if entry[SPECIES_TAG] not in best_name.__dict__['last']:
-        best_name.__dict__['last'][entry[SPECIES_TAG]] = dict()
-    best_name.__dict__['last'][entry[SPECIES_TAG]][allow_html] = res
+    if species_tag not in best_name.__dict__['last']:
+        best_name.__dict__['last'][species_tag] = dict()
+    best_name.__dict__['last'][species_tag][allow_html] = res
     return res
 
 
 def remove_html(line: str) -> str:
     """ removes HTML tags and decodes HTML entities """
     if not is_good_html(line):
         return html.unescape(line)
@@ -585,15 +583,15 @@
     for combination in itertools.product(*variants):
         yield ''.join(combination)
 
 
 def save_catalog_to_file(filename: str | Path,
                          catalog: list[dict[str, int | str | list[dict[str, float]]]],
                          frequency_limits: tuple[float, float]) -> bool:
-    from catalog import Catalog
+    from .catalog import Catalog
 
     if not catalog:
         return False
     Catalog.save(filename=filename, catalog=catalog, frequency_limits=frequency_limits)
     return True
 
 
@@ -624,14 +622,16 @@
                         return int(i_digits) < int(j_digits)
                     else:
                         return i_digits < j_digits
                 return i < j
         return False
 
     def __eq__(self, other: str | ReleaseInfo) -> bool:
+        if not isinstance(other, (str, ReleaseInfo)):
+            return NotImplemented
         if isinstance(other, str):
             other = ReleaseInfo(version=other)
         return self.version == other.version
 
 
 def latest_release() -> ReleaseInfo:
     import urllib.request
@@ -686,14 +686,18 @@
         sys.executable, '-c',
         f'''import sys, subprocess, time; time.sleep(2);\
         subprocess.run(args=[sys.executable, '-m', 'pip', 'install', '-U', {__original_name__!r}]);\
         subprocess.Popen(args=[sys.executable, '-m', {__original_name__!r}])'''])
     sys.exit(0)
 
 
-# noinspection PyShadowingBuiltins
-def zip(*iterables: Iterable[Any], strict: bool = False) -> builtins.zip:
-    """ Intentionally override `builtins.zip` to ignore `strict` parameter in Python < 3.10 """
-    if sys.version_info < (3, 10):
+if sys.version_info < (3, 10):
+    import builtins
+
+
+    # noinspection PyShadowingBuiltins, PyUnusedLocal
+    def zip(*iterables: Iterable[Any], strict: bool = False) -> builtins.zip:
+        """ Intentionally override `builtins.zip` to ignore `strict` parameter in Python < 3.10 """
         return builtins.zip(*iterables)
-    else:
-        return builtins.zip(*iterables, strict=strict)
+
+
+    __all__.append('zip')
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.8/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.7
+Version: 5.1.8
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -81,14 +81,15 @@
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
   any_name: str = '',
   any_formula: str = '',
   any_name_or_formula: str = '',
+  anything: str = '',
   species_tag: int = 0,
   inchi: str = '',
   trivial_name: str = '',
   structural_formula: str = '',
   name: str = '',
   stoichiometric_formula: str = '',
   isotopolog: str = '',
@@ -102,14 +103,15 @@
     - `float max_intensity`: the maximal intensity \[log10(nm²×MHz)\] to take, use to avoid meta-stable substances.
     - `float temperature`: the temperature to calculate the line intensity at,
       use the catalog intensity if not set.
     - `str any_name`: a string to match the ``trivialname`` or the ``name`` field.
     - `str any_formula`: a string to match the ``structuralformula``, ``moleculesymbol``,
       ``stoichiometricformula``, or ``isotopolog`` field.
     - `str any_name_or_formula`: a string to match any field used by `any_name` and `any_formula`.
+    - `str anything`: a string to match any field at all.
     - `int species_tag`: a number to match the ``speciestag`` field.
     - `str inchi`: a string to match the ``inchikey`` field.
       See https://iupac.org/who-we-are/divisions/division-details/inchi/ for more.
     - `str trivial_name`: a string to match the ``trivialname`` field.
     - `str structural_formula`: a string to match the ``structuralformula`` field.
     - `str name`: a string to match the ``name`` field.
     - `str stoichiometric_formula`: a string to match the ``stoichiometricformula`` field.
```

### Comparing `pycatsearch-5.1.7/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.8/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 src/pycatsearch/gui/preferences.py
 src/pycatsearch/gui/selectable_label.py
 src/pycatsearch/gui/settings.py
 src/pycatsearch/gui/substance_info.py
 src/pycatsearch/gui/substances_box.py
 src/pycatsearch/gui/titled_list_widget.py
 src/pycatsearch/gui/ui.py
+src/pycatsearch/gui/url_label.py
 src/pycatsearch/gui/waiting_screen.py
```

### Comparing `pycatsearch-5.1.7/updater.py` & `pycatsearch-5.1.8/updater.py`

 * *Files identical despite different names*

