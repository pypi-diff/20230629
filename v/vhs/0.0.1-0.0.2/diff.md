# Comparing `tmp/vhs-0.0.1.tar.gz` & `tmp/vhs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhs-0.0.1.tar", last modified: Tue Jun 27 16:39:10 2023, max compression
+gzip compressed data, was "vhs-0.0.2.tar", last modified: Thu Jun 29 13:17:22 2023, max compression
```

## Comparing `vhs-0.0.1.tar` & `vhs-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.882443 vhs-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.874443 vhs-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.878443 vhs-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-27 16:38:59.000000 vhs-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 16:38:59.000000 vhs-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 16:38:59.000000 vhs-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 16:38:59.000000 vhs-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-27 16:39:10.882443 vhs-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-27 16:38:59.000000 vhs-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.878443 vhs-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-27 16:38:59.000000 vhs-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-27 16:38:59.000000 vhs-0.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.878443 vhs-0.0.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.878443 vhs-0.0.1/docs/source/_extra/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 16:38:59.000000 vhs-0.0.1/docs/source/_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 16:38:59.000000 vhs-0.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 16:38:59.000000 vhs-0.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-27 16:38:59.000000 vhs-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:39:10.882443 vhs-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.878443 vhs-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 16:38:59.000000 vhs-0.0.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-27 16:38:59.000000 vhs-0.0.1/test/test_vhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.878443 vhs-0.0.1/vhs/
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-06-27 16:38:59.000000 vhs-0.0.1/vhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 16:39:10.000000 vhs-0.0.1/vhs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:38:59.000000 vhs-0.0.1/vhs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:39:10.882443 vhs-0.0.1/vhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-27 16:39:10.000000 vhs-0.0.1/vhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 16:39:10.000000 vhs-0.0.1/vhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:39:10.000000 vhs-0.0.1/vhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-27 16:39:10.000000 vhs-0.0.1/vhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 16:39:10.000000 vhs-0.0.1/vhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.101917 vhs-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.093917 vhs-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-29 13:17:11.000000 vhs-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 13:17:11.000000 vhs-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 13:17:11.000000 vhs-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 13:17:11.000000 vhs-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-29 13:17:22.097917 vhs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 13:17:11.000000 vhs-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/docs/source/_extra/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/source/_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 13:17:11.000000 vhs-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:17:22.101917 vhs-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 13:17:11.000000 vhs-0.0.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-29 13:17:11.000000 vhs-0.0.2/test/test_vhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/vhs/
+-rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-29 13:17:11.000000 vhs-0.0.2/vhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:17:21.000000 vhs-0.0.2/vhs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:11.000000 vhs-0.0.2/vhs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/vhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/top_level.txt
```

### Comparing `vhs-0.0.1/.github/workflows/ci.yaml` & `vhs-0.0.2/.github/workflows/ci.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -27,34 +27,35 @@
         os:
           - ubuntu-latest
         python-version:
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
-        include:
-          # GitHub windows runner seems to be hanging a lot; no idea why.
-          # - os: windows-latest
-          #   python-version: "3.11"
-          - os: macos-latest
-            python-version: "3.11"
+        # include:
+        #   - os: windows-latest
+        #     python-version: "3.11"
+        #   - os: macos-latest
+        #     python-version: "3.11"
     runs-on: ${{ matrix.os }}
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
       - name: Set up python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install package
         run: |
           python -m pip install --upgrade pip
           python -m pip install '.[test]'
       - name: Check codestyle
-        run: black --check .
+        run: |
+          black --check .
+          isort --check --diff .
       - run: |
           echo 'Type "true"' > _empty_vhs_tape.tape
       - name: Install VHS
         uses: charmbracelet/vhs-action@v1
         with:
           path: _empty_vhs_tape.tape
       - name: Test package
@@ -78,21 +79,20 @@
           python-version: 3.8
       - name: Install build
         run: |
           pip install build
       - name: Build project
         run: |
           python3 -m build .
-#      - name: Publish to test pypi
-#        uses: pypa/gh-action-pypi-publish@release/v1
-#        with:
-#          password: ${{ secrets.TEST_PYPI_PASSWORD }}
-#          repository-url: https://test.pypi.org/legacy/
+      - name: Publish to test pypi
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.TEST_PYPI_PASSWORD }}
+          repository-url: https://test.pypi.org/legacy/
       - name: Publish to pypi
-        if: ${{ !contains(github.event.ref, '.dev') }}  # don't upload dev releases to prod pypi
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_PASSWORD }}
 
   # Builds sphinx documentation.
   #
   # Runs on all events except when closing a pull request.
```

### Comparing `vhs-0.0.1/.gitignore` & `vhs-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vhs-0.0.1/LICENSE` & `vhs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vhs-0.0.1/PKG-INFO` & `vhs-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vhs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Write terminal GIFs as code for integration testing and demoing your CLI tools, now with python
 Author-email: Tamika Nomara <taminomara@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tamika Nomara
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://python-vhs.readthedocs.io/en/stable/
-Project-URL: Issues, https://github.com/taminomara/python-vhs/issues
+Project-URL: Documentation, https://taminomara.github.io/python-vhs/
+Project-URL: Issues, https://github.com/taminomara/python-vhs/issues/
 Project-URL: Source, https://github.com/taminomara/python-vhs/
 Project-URL: Changelog, https://github.com/taminomara/python-vhs/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -56,9 +56,9 @@
 [charm]: https://charm.sh/
 
 ## Resources
 
 - [Documentation](https://taminomara.github.io/python-vhs/)
 - [Issues](https://github.com/taminomara/python-vhs/issues)
 - [Source](https://github.com/taminomara/python-vhs/)
-- [PyPi](https://pypi.org/project/python-vhs/)
+- [PyPi](https://pypi.org/project/vhs/)
 - [Changelog](https://github.com/taminomara/python-vhs/blob/main/CHANGELOG.md)
```

### Comparing `vhs-0.0.1/README.md` & `vhs-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 [charm]: https://charm.sh/
 
 ## Resources
 
 - [Documentation](https://taminomara.github.io/python-vhs/)
 - [Issues](https://github.com/taminomara/python-vhs/issues)
 - [Source](https://github.com/taminomara/python-vhs/)
-- [PyPi](https://pypi.org/project/python-vhs/)
+- [PyPi](https://pypi.org/project/vhs/)
 - [Changelog](https://github.com/taminomara/python-vhs/blob/main/CHANGELOG.md)
```

### Comparing `vhs-0.0.1/docs/Makefile` & `vhs-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vhs-0.0.1/docs/make.bat` & `vhs-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vhs-0.0.1/docs/source/conf.py` & `vhs-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vhs-0.0.1/pyproject.toml` & `vhs-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "vhs"
 authors = [{name = "Tamika Nomara", email = "taminomara@gmail.com"}]
 description = "Write terminal GIFs as code for integration testing and demoing your CLI tools, now with python"
+dynamic = ["version"]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -14,35 +15,35 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
     "Typing :: Typed",
 ]
-dynamic = ["version"]
 dependencies = [
     "PyGithub~=1.59.0",
     "requests~=2.31.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest~=7.0",
     "pytest-mypy~=0.10.3",
     "black~=23.0",
+    "isort~=5.12.0",
     "types-requests",
 ]
 doc = [
     "sphinx>=6.0.0",
     "sphinx-rtd-theme~=1.2.2",
 ]
 
 [project.urls]
-Documentation = "https://python-vhs.readthedocs.io/en/stable/"
-Issues = "https://github.com/taminomara/python-vhs/issues"
+Documentation = "https://taminomara.github.io/python-vhs/"
+Issues = "https://github.com/taminomara/python-vhs/issues/"
 Source = "https://github.com/taminomara/python-vhs/"
 Changelog = "https://github.com/taminomara/python-vhs/blob/main/CHANGELOG.md"
 
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2", "wheel>=0.40"]
 
 [tool.setuptools_scm]
```

### Comparing `vhs-0.0.1/test/test_vhs.py` & `vhs-0.0.2/test/test_vhs.py`

 * *Files identical despite different names*

### Comparing `vhs-0.0.1/vhs/__init__.py` & `vhs-0.0.2/vhs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,31 +61,30 @@
 .. autoclass:: ProgressReporter
    :members:
 
 .. autoclass:: DefaultProgressReporter
 
 """
 import datetime
-
-import requests
-import requests.adapters
 import logging
 import os
 import pathlib
 import platform
 import re
 import shutil
 import signal
 import stat
 import subprocess
 import sys
 import tempfile
 import typing as _t
 
 import github
+import requests
+import requests.adapters
 import urllib3
 
 _logger = logging.getLogger("vhs")
 
 try:
     from vhs._version import __version__, __version_tuple__
 except ImportError:
@@ -303,15 +302,15 @@
         :param speed:
             when the installer downloads files, this number indicates
             current downloading speed, in bytes per second. Otherwise,
             it is set to zero.
 
         """
 
-    def finish(self):
+    def finish(self, exc_type, exc_val, exc_tb):
         """
         Called when installation finishes.
 
         """
 
 
 class DefaultProgressReporter(ProgressReporter):
@@ -322,27 +321,43 @@
 
     _prev_len = 0
 
     def __init__(self, stream: _t.Optional[_t.TextIO] = None):
         self.stream = stream or sys.stderr
 
     def progress(self, desc: str, dl_size: int, total_size: int, speed: float, /):
+        desc = self.format_desc(desc)
+
         if total_size:
-            dl_size_mb = dl_size / 1024**2
-            total_size_mb = total_size / 1024**2
-            speed_mb = speed / 1024**2
-            desc += f": {dl_size_mb:.1f}/{total_size_mb:.1f}MB - {speed_mb:.2f}MB/s"
+            desc += self.format_progress(dl_size, total_size, speed)
 
-        self.stream.write(desc.ljust(self._prev_len) + "\r")
-        self.stream.flush()
+        self.write(desc.ljust(self._prev_len) + "\r")
 
         self._prev_len = len(desc)
 
-    def finish(self):
-        self.stream.write(f"vhs installed\n")
+    def finish(self, exc_type, exc_val, exc_tb):
+        if exc_val:
+            self.progress(f"vhs installation failed: {exc_val}", 0, 0, 0)
+            self.write("\n")
+        elif self._prev_len > 0:
+            self.progress(f"vhs installed", 0, 0, 0)
+            self.write("\n")
+
+    def format_desc(self, desc: str) -> str:
+        return desc
+
+    def format_progress(self, dl_size: int, total_size: int, speed: float) -> str:
+        dl_size_mb = dl_size / 1024**2
+        total_size_mb = total_size / 1024**2
+        speed_mb = speed / 1024**2
+
+        return f": {dl_size_mb:.1f}/{total_size_mb:.1f}MB - {speed_mb:.2f}MB/s"
+
+    def write(self, msg: str):
+        self.stream.write(msg)
         self.stream.flush()
 
 
 def resolve(
     *,
     cache_path: _t.Optional[pathlib.Path] = None,
     min_version: str = "0.5.0",
@@ -394,24 +409,26 @@
     """
 
     if cache_path is None:
         cache_path = pathlib.Path(tempfile.gettempdir()) / "python_vhs_cache"
     else:
         cache_path = pathlib.Path(cache_path)
 
+    _logger.debug("using vhs cache path: %s", cache_path)
+
     if retry is None:
         retry = urllib3.Retry(10, backoff_factor=0.1)
 
     reporter.start()
     try:
         vhs_path, path = _check_and_install(
             min_version, cache_path, _get_path(env), install, reporter, timeout, retry
         )
     finally:
-        reporter.finish()
+        reporter.finish(*sys.exc_info())
 
     return Vhs(
         _vhs_path=vhs_path,
         _path=path,
         _quiet=quiet,
         _env=env,
         _cwd=cwd,
@@ -448,26 +465,30 @@
 
     repo = api.get_repo(repo_name)
 
     for release in repo.get_releases():
         if release.draft or release.prerelease:
             continue
 
+        _logger.debug("found %s release %s", name, release.tag_name)
+
         for asset in release.assets:
             if filter(asset.name):
+                _logger.debug("found %s asset %s", name, asset.name)
+                basename = asset.name
                 browser_download_url = asset.browser_download_url
                 break
         else:
             raise VhsError(f"unable to find {name} release for platform {sys.platform}")
 
         break
     else:
         raise VhsError(f"unable to find latest {name} release")
 
-    basename = browser_download_url.rstrip("/").rsplit("/", maxsplit=1)[1]
+    _logger.debug("downloading %s from %s", name, browser_download_url)
 
     with requests.Session() as session:
         adapter = requests.adapters.HTTPAdapter(max_retries=retry)
         session.mount("https://", adapter)
         session.mount("http://", adapter)
 
         with requests.get(browser_download_url, stream=True, timeout=timeout) as stream:
@@ -523,19 +544,23 @@
                 tmp_dir,
                 filter,
                 reporter,
             )
 
             reporter.progress(f"processing vhs", 0, 0, 0)
 
+            _logger.debug("unpacking vhs")
+
             shutil.unpack_archive(tmp_file, tmp_dir)
 
             src = tmp_dir / "vhs"
             dst = bin_path / "vhs"
 
+            _logger.debug("copying %s -> %s", src, dst)
+
             os.replace(src, dst)
             dst.chmod(dst.stat().st_mode | stat.S_IEXEC)
         except Exception as e:
             raise VhsError(f"vhs install failed: {e}")
 
 
 def _install_ttyd(
@@ -555,14 +580,16 @@
                 api, timeout, retry, "ttyd", "tsl0922/ttyd", tmp_dir, filter, reporter
             )
 
             reporter.progress(f"processing ttyd", 0, 0, 0)
 
             dst = bin_path / "ttyd"
 
+            _logger.debug("copying %s -> %s", tmp_file, dst)
+
             os.replace(tmp_file, dst)
             dst.chmod(dst.stat().st_mode | stat.S_IEXEC)
         except Exception as e:
             raise VhsError(f"ttyd install failed: {e}") from e
 
 
 def _install_ffmpeg(
@@ -595,19 +622,23 @@
             if archive_basename.endswith(".zip"):
                 archive_basename = archive_basename[: -len(".zip")]
             elif archive_basename.endswith(".tar.gz"):
                 archive_basename = archive_basename[: -len(".tar.gz")]
             elif archive_basename.endswith(".tar.xz"):
                 archive_basename = archive_basename[: -len(".tar.xz")]
 
+            _logger.debug("unpacking ffmpeg")
+
             shutil.unpack_archive(tmp_file, tmp_dir)
 
             for src in (tmp_dir / archive_basename / "bin").iterdir():
                 dst = bin_path / src.name
 
+                _logger.debug("copying %s -> %s", src, dst)
+
                 os.replace(src, dst)
                 dst.chmod(dst.stat().st_mode | stat.S_IEXEC)
 
         except Exception as e:
             raise VhsError(f"ffmpeg install failed: {e}")
```

### Comparing `vhs-0.0.1/vhs.egg-info/PKG-INFO` & `vhs-0.0.2/vhs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vhs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Write terminal GIFs as code for integration testing and demoing your CLI tools, now with python
 Author-email: Tamika Nomara <taminomara@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tamika Nomara
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://python-vhs.readthedocs.io/en/stable/
-Project-URL: Issues, https://github.com/taminomara/python-vhs/issues
+Project-URL: Documentation, https://taminomara.github.io/python-vhs/
+Project-URL: Issues, https://github.com/taminomara/python-vhs/issues/
 Project-URL: Source, https://github.com/taminomara/python-vhs/
 Project-URL: Changelog, https://github.com/taminomara/python-vhs/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -56,9 +56,9 @@
 [charm]: https://charm.sh/
 
 ## Resources
 
 - [Documentation](https://taminomara.github.io/python-vhs/)
 - [Issues](https://github.com/taminomara/python-vhs/issues)
 - [Source](https://github.com/taminomara/python-vhs/)
-- [PyPi](https://pypi.org/project/python-vhs/)
+- [PyPi](https://pypi.org/project/vhs/)
 - [Changelog](https://github.com/taminomara/python-vhs/blob/main/CHANGELOG.md)
```

