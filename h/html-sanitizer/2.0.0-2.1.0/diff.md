# Comparing `tmp/html_sanitizer-2.0.0.tar.gz` & `tmp/html_sanitizer-2.1.0.tar.gz`

## Comparing `html_sanitizer-2.0.0.tar` & `html_sanitizer-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/.editorconfig
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/tox.ini
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/html_sanitizer/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/html_sanitizer/__main__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/html_sanitizer/django.py
--rw-r--r--   0        0        0    13144 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/html_sanitizer/sanitizer.py
--rw-r--r--   0        0        0    23444 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/html_sanitizer/tests.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/.gitignore
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/LICENSE
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/README.rst
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 html_sanitizer-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.editorconfig
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/tox.ini
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/__main__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/django.py
+-rw-r--r--   0        0        0    13558 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/sanitizer.py
+-rw-r--r--   0        0        0    23857 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/html_sanitizer/tests.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/README.rst
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 html_sanitizer-2.1.0/PKG-INFO
```

### Comparing `html_sanitizer-2.0.0/.pre-commit-config.yaml` & `html_sanitizer-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.0.0/CHANGELOG.rst` & `html_sanitizer-2.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 ==========
 Change log
 ==========
 
-`Next version`_
-===============
+Next version
+============
+
+
+2.1 (2023-06-29)
+================
+
+- Added a test for a type of misconfiguration.
+- Changed the sanitizer configuration validation to not allow unexpected data
+  types in ``tags``, ``empty``, ``separate``, ``whitespace`` and
+  ``attributes``.
 
 
 2.0 (2023-06-28)
 ================
 
 - Raised the minimum Python version to 3.7. Added Python 3.10, 3.11.
 - Raised the minimum lxml version to the current 4.9.1.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_a61zs2n6_/tmp7vi1640w_TarContainer/0/2.rst", line 150, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_a61zs2n6_/tmp7vi1640w_TarContainer/0/2.rst", line 150, column 0: CDATA terminal not found*

```diff
@@ -1,9 +1,12 @@
-========== Change log ========== `Next version`_ =============== 2.0 (2023-06-
-28) ================ - Raised the minimum Python version to 3.7. Added Python
-3.10, 3.11. - Raised the minimum lxml version to the current 4.9.1. - Switched
-from Travis CI to GitHub actions. Added Python 3.9 to the CI matrix. - Renamed
-the main branch to main. - Switched to a declarative setup. - Fixed a
+========== Change log ========== Next version ============ 2.1 (2023-06-29)
+================ - Added a test for a type of misconfiguration. - Changed the
+sanitizer configuration validation to not allow unexpected data types in
+``tags``, ``empty``, ``separate``, ``whitespace`` and ``attributes``. 2.0
+(2023-06-28) ================ - Raised the minimum Python version to 3.7. Added
+Python 3.10, 3.11. - Raised the minimum lxml version to the current 4.9.1. -
+Switched from Travis CI to GitHub actions. Added Python 3.9 to the CI matrix. -
+Renamed the main branch to main. - Switched to a declarative setup. - Fixed a
 whitespace dependency in the testsuite. - Switched to hatchling and ruff. -
 Made behavior-altering arguments to ``normalize_overall_whitespace`` keyword-
 only. `1.9`_ (2020-01-20) =================== - Added Python 3.8 to the CI
 matrix. - Be able to keep the ``
```

### Comparing `html_sanitizer-2.0.0/.github/workflows/test.yml` & `html_sanitizer-2.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.0.0/html_sanitizer/django.py` & `html_sanitizer-2.1.0/html_sanitizer/django.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.0.0/html_sanitizer/sanitizer.py` & `html_sanitizer-2.1.0/html_sanitizer/sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,24 +169,36 @@
         target_blank_noopener,
         anchor_id_to_name,
     ],
     "element_postprocessors": [],
 }
 
 
+def coerce_to_set(value):
+    if isinstance(value, set):
+        return value
+    elif isinstance(value, (tuple, list)):
+        return set(value)
+    raise TypeError(f"Expected a set but got value {value!r} of type {type(value)}")
+
+
 class Sanitizer:
     def __init__(self, settings=None):
         self.__dict__.update(DEFAULT_SETTINGS)
         self.__dict__.update(settings or {})
 
         # Allow iterables of any kind, not just sets.
-        self.tags = set(self.tags)
-        self.empty = set(self.empty)
-        self.separate = set(self.separate)
-        self.whitespace = set(self.whitespace)
+        self.tags = coerce_to_set(self.tags)
+        self.empty = coerce_to_set(self.empty)
+        self.separate = coerce_to_set(self.separate)
+        self.whitespace = coerce_to_set(self.whitespace)
+        self.attributes = {
+            tag: coerce_to_set(attributes)
+            for tag, attributes in self.attributes.items()
+        }
 
         if self.keep_typographic_whitespace:
             re_whitespace = r"[^\S%s]" % typographic_whitespace
         else:
             re_whitespace = r"\s"
 
         self.only_whitespace_re = re.compile(rf"^{re_whitespace}*$")
```

### Comparing `html_sanitizer-2.0.0/html_sanitizer/tests.py` & `html_sanitizer-2.1.0/html_sanitizer/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,7 +586,17 @@
 
     def test_entities(self):
         self.run_tests(
             [
                 ("&lsquo;", "\u2018"),
             ],
         )
+
+    def test_invalid_attributes(self):
+        with self.assertRaisesRegex(TypeError, "Expected a set but got"):
+            Sanitizer({"attributes": {"p": ("class")}})
+
+        with self.assertRaisesRegex(TypeError, "Expected a set but got"):
+            Sanitizer({"tags": "blub"})
+
+        with self.assertRaisesRegex(TypeError, 'Tags in "empty", but not allowed:'):
+            Sanitizer({"tags": {"blub"}})
```

### Comparing `html_sanitizer-2.0.0/LICENSE` & `html_sanitizer-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.0.0/README.rst` & `html_sanitizer-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.0.0/pyproject.toml` & `html_sanitizer-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.0.0/PKG-INFO` & `html_sanitizer-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-sanitizer
-Version: 2.0.0
+Version: 2.1.0
 Summary: HTML sanitizer
 Project-URL: Homepage, https://github.com/matthiask/html-sanitizer/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

