# Comparing `tmp/katalytic-pkg-0.4.0.tar.gz` & `tmp/katalytic_pkg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.4.0.tar", last modified: Tue May  2 05:42:16 2023, max compression
+gzip compressed data, was "katalytic_pkg-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic-pkg-0.4.0.tar` & `katalytic_pkg-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic-pkg-0.4.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-pkg-0.4.0/.gitignore
--rw-r--r--   0        0        0     3258 2023-04-30 14:18:45.239106 katalytic-pkg-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2085 2023-05-02 05:41:51.432198 katalytic-pkg-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic-pkg-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1507 2023-04-30 14:21:04.979530 katalytic-pkg-0.4.0/README.md
--rw-r--r--   0        0        0     1119 2023-05-02 05:41:51.432198 katalytic-pkg-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4757 2023-05-02 05:32:43.902113 katalytic-pkg-0.4.0/src/katalytic/pkg.py
--rw-r--r--   0        0        0     2829 2023-04-28 10:02:55.132516 katalytic-pkg-0.4.0/tests/test_pkg.py
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 katalytic-pkg-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic_pkg-0.4.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_pkg-0.4.1/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_pkg-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2564 2023-06-29 17:28:54.379685 katalytic_pkg-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic_pkg-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     1537 2023-05-14 08:37:36.967341 katalytic_pkg-0.4.1/README.md
+-rw-r--r--   0        0        0     1119 2023-06-29 17:28:54.379685 katalytic_pkg-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6150 2023-06-29 17:14:46.039481 katalytic_pkg-0.4.1/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2914 2023-06-29 17:26:02.006220 katalytic_pkg-0.4.1/tests/test_pkg.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 katalytic_pkg-0.4.1/PKG-INFO
```

### Comparing `katalytic-pkg-0.4.0/.gitignore` & `katalytic_pkg-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.4.0/.gitlab-ci.yml` & `katalytic_pkg-0.4.1/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 include:
 - template: Security/SAST.gitlab-ci.yml
 
-image: python:3.9
+image: python:3.6
 
 stages:
   - coverage
   - test
   - security
   - release
 
 variables:
-  TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
 coverage:
   image: python:3.6
   stage: coverage
   script:
```

### Comparing `katalytic-pkg-0.4.0/CHANGELOG.md` & `katalytic_pkg-0.4.1/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.4.1 (2023-06-29)
+### refactor
+- [[`eb5f392`](https://gitlab.com/katalytic/katalytic-pkg/commit/eb5f3921112948dd1c7e6c8c954e18e7907f6076)] rename get_functions_in_group() -> find_functions_marked_with()
+- [[`852af88`](https://gitlab.com/katalytic/katalytic-pkg/commit/852af883b95eb4a314750fbda2b4f58f862cbc07)] rename get_functions_in_group() -> find_functions_marked_with() --- See previous commit. I made this change because the merge commit will not trigger the rebuild
+
+
 ## 0.4.0 (2023-05-02)
 ### feat
 - [[`1afcf66`](https://gitlab.com/katalytic/katalytic-pkg/commit/1afcf66f65a6a208039af7929da42a2dc1fcef24)] **get_version:** support subpackages
 
 
 ## 0.3.0 (2023-04-28)
 ### feat
```

### Comparing `katalytic-pkg-0.4.0/LICENSE.txt` & `katalytic_pkg-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.4.0/README.md` & `katalytic_pkg-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-pkg)](https://pypi.org/project/katalytic-pkg/)
 [![tests](https://gitlab.com/katalytic/katalytic-pkg/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-pkg/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
```

### Comparing `katalytic-pkg-0.4.0/pyproject.toml` & `katalytic_pkg-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-pkg"
-version = "0.4.0"
+version = "0.4.1"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-pkg-0.4.0/tests/test_pkg.py` & `katalytic_pkg-0.4.1/tests/test_pkg.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import sys
-
 import pytest
 
-from katalytic.pkg import _check, get_functions_in_group, get_modules, get_version, mark
+# noinspection PyProtectedMember
+from katalytic.pkg import _check, find_functions_marked_with, get_modules, get_version, mark
 from katalytic.pkg import __version__ as pkg_version
 
 
 class Test_check:
     def test_all(self):
         assert _check(None, '') is False
         assert _check('load', 'save') is False
@@ -30,61 +29,61 @@
         @mark('_test_group-1')
         def f3(): pass
 
         assert not hasattr(f1, '__katalytic_marks__')
         assert f2.__katalytic_marks__ == ('_test_group-1', )
         assert f3.__katalytic_marks__ == ('_test_group-2', '_test_group-1')
 
-
     @pytest.mark.parametrize('group', [0, None, {}, True])
     def test_TypeError(self, group):
         with pytest.raises(TypeError):
+            # noinspection PyTypeChecker
             @mark(group)
             def f1(): pass
 
-
     @pytest.mark.parametrize('group', ['', ' ', ' \n ', '\t \t', 'no \t tabs', 'no \n newlines'])
     def test_ValueError(self, group):
         with pytest.raises(ValueError):
             @mark(group)
             def f1(): pass
 
 
-class Test_get_modules:
-    def test_all(self):
-        modules = get_modules()
-        assert 'katalytic.pkg' in [m.__name__ for m in modules]
-        assert all(m.__name__.startswith('katalytic') for m in modules)
-
-
 class Test_get_functions_in_group:
     def test_empty(self):
-        assert get_functions_in_group('__not-used') == []
-        assert get_functions_in_group('__test_3') == []
+        assert find_functions_marked_with('__not-used') == []
+        assert find_functions_marked_with('__test_3') == []
 
     def test_pattern(self):
-        found = get_functions_in_group('__test_3*')
+        found = find_functions_marked_with('__test_3*')
         found = [(name, groups) for name, _, groups in found]
         assert found == [
             ('__test', ['__test_300']),
             ('__test_2', ['__test_3::a', '__test_3::b'])
         ]
 
     def test_exact(self):
-        found = get_functions_in_group('__test_1')
+        found = find_functions_marked_with('__test_1')
         found = [(name, groups) for name, _, groups in found]
         assert found == [('__test', ['__test_1'])]
 
-        found = get_functions_in_group('__test_2')
+        found = find_functions_marked_with('__test_2')
         found = [(name, groups) for name, _, groups in found]
         assert found == [
             ('__test', ['__test_2']),
             ('__test_2', ['__test_2'])
         ]
 
+
+class Test_get_modules:
+    def test_all(self):
+        modules = get_modules()
+        assert 'katalytic.pkg' in [m.__name__ for m in modules]
+        assert all(m.__name__.startswith('katalytic') for m in modules)
+
+
 class Test_version:
     def test_is_ok(self):
         v, v_info = get_version('katalytic.pkg')
 
         assert pkg_version is not None
         assert v is not None
         assert v_info is not None
```

### Comparing `katalytic-pkg-0.4.0/PKG-INFO` & `katalytic_pkg-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.4.0
+Version: 0.4.1
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Keywords: high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,16 @@
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-pkg.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-pkg.git
 Provides-Extra: dev
 
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-pkg)](https://pypi.org/project/katalytic-pkg/)
 [![tests](https://gitlab.com/katalytic/katalytic-pkg/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-pkg/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-pkg/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
```

