# Comparing `tmp/mkdocs-nbconvert-0.2.tar.gz` & `tmp/mkdocs-nbconvert-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-nbconvert-0.2.tar", last modified: Wed Jun 28 08:45:11 2023, max compression
+gzip compressed data, was "mkdocs-nbconvert-0.2.1.tar", last modified: Thu Jun 29 06:42:34 2023, max compression
```

## Comparing `mkdocs-nbconvert-0.2.tar` & `mkdocs-nbconvert-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 08:45:11.459754 mkdocs-nbconvert-0.2/
--rw-rw-rw-   0        0        0       52 2023-06-28 03:05:47.000000 mkdocs-nbconvert-0.2/AUTHORS.md
--rw-rw-rw-   0        0        0      737 2023-06-28 08:43:13.000000 mkdocs-nbconvert-0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0       16 2023-06-28 03:05:47.000000 mkdocs-nbconvert-0.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1304 2023-06-28 03:05:47.000000 mkdocs-nbconvert-0.2/LICENSE
--rw-rw-rw-   0        0        0      127 2023-06-28 08:42:45.000000 mkdocs-nbconvert-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1976 2023-06-28 08:45:11.458755 mkdocs-nbconvert-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-06-28 08:42:45.000000 mkdocs-nbconvert-0.2/README.md
--rw-rw-rw-   0        0        0     1343 2023-06-28 08:42:45.000000 mkdocs-nbconvert-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 08:45:11.459754 mkdocs-nbconvert-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 08:45:11.303756 mkdocs-nbconvert-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 08:45:11.345756 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert/
--rw-rw-rw-   0        0        0       88 2023-06-28 08:42:45.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert/__init__.py
--rw-rw-rw-   0        0        0     5962 2023-06-28 08:42:45.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert/plugin.py
--rw-rw-rw-   0        0        0      159 2023-06-28 08:45:06.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert/version.py
-drwxrwxrwx   0        0        0        0 2023-06-28 08:45:11.456753 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/
--rw-rw-rw-   0        0        0     1976 2023-06-28 08:45:07.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-06-28 08:45:11.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 08:45:07.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-28 08:45:07.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-28 08:45:07.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-28 08:45:07.000000 mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 06:42:34.870427 mkdocs-nbconvert-0.2.1/
+-rw-rw-rw-   0        0        0      183 2023-06-29 06:39:53.000000 mkdocs-nbconvert-0.2.1/AUTHORS.md
+-rw-rw-rw-   0        0        0      961 2023-06-29 06:40:13.000000 mkdocs-nbconvert-0.2.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0       15 2023-06-28 10:14:14.000000 mkdocs-nbconvert-0.2.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1295 2023-06-28 10:14:14.000000 mkdocs-nbconvert-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-06-28 10:14:14.000000 mkdocs-nbconvert-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1753 2023-06-29 06:42:34.869428 mkdocs-nbconvert-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-06-28 10:14:14.000000 mkdocs-nbconvert-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1349 2023-06-29 06:39:53.000000 mkdocs-nbconvert-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 06:42:34.870427 mkdocs-nbconvert-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 06:42:34.749309 mkdocs-nbconvert-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 06:42:34.775209 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert/
+-rw-rw-rw-   0        0        0       88 2023-06-28 10:14:14.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert/__init__.py
+-rw-rw-rw-   0        0        0     6912 2023-06-29 06:39:53.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert/plugin.py
+-rw-rw-rw-   0        0        0      164 2023-06-29 06:42:30.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert/version.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:42:34.867866 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/
+-rw-rw-rw-   0        0        0     1753 2023-06-29 06:42:30.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-06-29 06:42:34.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:42:30.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 06:42:30.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-29 06:42:30.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 06:42:30.000000 mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/top_level.txt
```

### Comparing `mkdocs-nbconvert-0.2/CHANGELOG.md` & `mkdocs-nbconvert-0.2.1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 # Changelog
 
+## v0.2.1
+
+Date: 2023-06-29
+
+- Release highlights:
+    - Add a new notebook execution configure: `exit_on_error`
+
+- Fixing:
+    - `mkdocs` and `nbconvert` dependent versions in `pyproject.toml`
+    - Typos
+
+- Docs:
+    - Edit usage notebook
+
 ## v0.2
 
 Date: 2023-06-28
 
 - Release highlights:
-  - Now the plugin can execute notebooks before convert
+    - Now the plugin can execute notebooks before convert
 
 - Break changes:
-  - No longer support for python earlier than 3.7
-  - Drop `setup.cfg`, only `pyproject.toml`
+    - No longer support for python earlier than 3.7
+    - Drop `setup.cfg`, only `pyproject.toml`
 
 - Library:
-  - Update to latest mkdocs
+    - Update to latest mkdocs
 
 - Docs
-  - Update to latest mkdocs-material and re-build doc-site
+    - Update to latest mkdocs-material and re-build doc-site
 
 - CI
-  - Many pre-commit checks
+    - Many pre-commit checks
 
 ## v0.1.3
 
 Date: 2022-04-18
 
 - Changes:
-  - Switch to BSD 2-Clause License, and add the license file to repo.
-  - Drop supports of old python (<=3.6))
-  - Change the package's build system to PEP517
+    - Switch to BSD 2-Clause License, and add the license file to repo.
+    - Drop supports of old python (<=3.6))
+    - Change the package's build system to PEP517
 
 ## v0.1.2
 
-- Date: 2020-07-17
+Date: 2020-07-17
 
-  - New documentation site
-  - `kwargs` to plugin method
+- New documentation site
 
 ## v0.1
 
-- Date: 2020-01-16
+Date: 2020-01-16
 
 A very early alpha version, not for production.
```

### Comparing `mkdocs-nbconvert-0.2/LICENSE` & `mkdocs-nbconvert-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright 2019-present, Liu Xue Yan. All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright 2019-present, Liu Xue Yan. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `mkdocs-nbconvert-0.2/PKG-INFO` & `mkdocs-nbconvert-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mkdocs-nbconvert
-Version: 0.2
+Version: 0.2.1
 Summary: A MkDocs plug-in provides a source parser for *.ipynb Jupyter notebook files, base on nbconvert.
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://tanbro.github.io/mkdocs-nbconvert
-Project-URL: Repository, https://github.com/tanbro/mkdocs_nbconvert.git
+Project-URL: Repository, https://github.com/tanbro/mkdocs-nbconvert
 Project-URL: Documentation, https://tanbro.github.io/mkdocs-nbconvert
 Keywords: mkdocs,mkdocs-plugin,jupyter,notebook,jupyter-notebook,markdown,md,nbconvert
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Documentation
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -17,17 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # mkdocs-nbconvert
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Status](https://img.shields.io/pypi/status/mkdocs-nbconvert)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Format](https://img.shields.io/pypi/format/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
+[![GitHub tag (latest SemVer pre-release)](https://img.shields.io/github/v/tag/tanbro/mkdocs-nbconvert)](https://github.com/tanbro/mkdocs-nbconvert)
 
 A [MkDocs][] plug-in provides a source parser for `*.ipynb` [Jupyter][] Notebook files, base on [nbconvert][].
 
 ## References
 
 - <https://tanbro.github.io/mkdocs-nbconvert/>
 - <https://www.mkdocs.org/user-guide/plugins/>
```

### Comparing `mkdocs-nbconvert-0.2/README.md` & `mkdocs-nbconvert-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # mkdocs-nbconvert
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Status](https://img.shields.io/pypi/status/mkdocs-nbconvert)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Format](https://img.shields.io/pypi/format/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
+[![GitHub tag (latest SemVer pre-release)](https://img.shields.io/github/v/tag/tanbro/mkdocs-nbconvert)](https://github.com/tanbro/mkdocs-nbconvert)
 
 A [MkDocs][] plug-in provides a source parser for `*.ipynb` [Jupyter][] Notebook files, base on [nbconvert][].
 
 ## References
 
 - <https://tanbro.github.io/mkdocs-nbconvert/>
 - <https://www.mkdocs.org/user-guide/plugins/>
```

### Comparing `mkdocs-nbconvert-0.2/pyproject.toml` & `mkdocs-nbconvert-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,20 +19,20 @@
   "Programming Language :: Python",
 ]
 dynamic = ["version"]
 
 # requires python version
 requires-python = ">=3.7"
 # requires
-dependencies = ["mkdocs", "nbconvert"]
+dependencies = ["mkdocs>=1.4", "nbconvert>=4.2"]
 
 # Project links
 [project.urls]
 Homepage = "https://tanbro.github.io/mkdocs-nbconvert"
-Repository = "https://github.com/tanbro/mkdocs_nbconvert.git"
+Repository = "https://github.com/tanbro/mkdocs-nbconvert"
 Documentation = "https://tanbro.github.io/mkdocs-nbconvert"
 
 [project.entry-points."mkdocs.plugins"]
 nbconvert = "mkdocs_nbconvert:NbConvertPlugin"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `mkdocs-nbconvert-0.2/src/mkdocs_nbconvert/plugin.py` & `mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,137 @@
+import asyncio
+import platform
 from glob import iglob
 from os import makedirs, path, remove, removedirs
 from pprint import pformat
 from time import time
 
 import nbformat
 from mkdocs.config import base, config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import File
 from mkdocs.utils import log
 from nbconvert import MarkdownExporter
-from nbconvert.preprocessors import ExecutePreprocessor  # type: ignore
+from nbconvert.preprocessors import CellExecutionError, ExecutePreprocessor  # pyright: ignore[reportPrivateImportUsage]
+
 
 __all__ = ["NbConvertPlugin"]
 
 
 class _ExecuteOptions(base.Config):
     run_path = config_options.Optional(config_options.Dir())
     kernel_name = config_options.Optional(config_options.Type(str))
     timeout = config_options.Optional(config_options.Type(int))
-    write_back = config_options.Optional(config_options.Type(bool))
+    write_back = config_options.Type(bool, default=False)
+    exit_on_error = config_options.Type(bool, default=True)
 
 
-class NbConvertPluginConfig(base.Config):
+class _PluginConfig(base.Config):
     input_dir = config_options.Dir(exists=True, default="notebooks")
     output_dir = config_options.Type(str, default="notebooks")
     recursive = config_options.Type(bool, default=True)
     execute_enabled = config_options.Type(bool, default=False)
     execute_options = config_options.SubConfig(_ExecuteOptions)
 
 
-class NbConvertPlugin(BasePlugin[NbConvertPluginConfig]):
+class NbConvertPlugin(BasePlugin[_PluginConfig]):
     def on_files(self, files, config, **kwargs):
         log.debug("[NbConvertPlugin] config: %s", pformat(self.config))
         self._src_files = []
         # deal with dirs
         config_file_dir = path.dirname(config["config_file_path"])
         input_dir = path.normpath(self.config["input_dir"])
         output_dir = path.realpath(path.join(config["docs_dir"], path.normpath(self.config["output_dir"])))
         if not path.isabs(input_dir):
             input_dir = path.realpath(path.join(config_file_dir, input_dir))
         # glob match
         nb_finder = iglob(path.join(config_file_dir, input_dir, "**", "*.ipynb"), recursive=self.config["recursive"])
         # Exporter
         exporter = MarkdownExporter()
+        # Pre-execute args
+        exe_opts = exe_path = exe_save = exe_exit_on_error = None
+        if self.config.get("execute_enabled"):
+            _opts = self.config.get("execute_options") or {}
+            exe_opts = {k: v for k, v in _opts.items() if k in ("timeout", "kernel_name") and v is not None}
+            exe_path, exe_save, exe_exit_on_error = (_opts.get(a) for a in ("run_path", "write_back", "exit_on_error"))
+            # On windows:
+            #   Proactor event loop does not implement add_reader family of methods required for zmq.
+            #   Registering an additional selector thread for add_reader support via tornado.
+            #   Use `asyncio.set_event_loop_policy(WindowsSelectorEventLoopPolicy())` to avoid this warning.
+            if platform.system() == "Windows":
+                asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
         # Converting
         for i, nb_path in enumerate(nb_finder, 1):
             # Prepare output file/dir
             nb_dirname, nb_basename = path.split(nb_path)
             nb_basename_root, _ = path.splitext(nb_basename)
             nb_subdir = path.relpath(nb_dirname, input_dir)
             md_dir = path.join(output_dir, nb_subdir)
             md_basename = f"{nb_basename_root}.md"
             md_path = path.join(md_dir, md_basename)
             md_rel_dir = path.relpath(md_dir, config["docs_dir"])
             md_rel_path = path.join(md_rel_dir, md_basename)
+            file_obj = File(
+                path=md_rel_path,
+                src_dir=config["docs_dir"],
+                dest_dir=config["site_dir"],
+                use_directory_urls=config["use_directory_urls"],
+            )
             #
-            log.debug("[NbConvertPlugin] (%d) %r => %r", i, nb_path, md_path)
-            # run nbconvert ...
+            log.info("[NbConvertPlugin] (%d) %r => %r", i, nb_path, file_obj)
+            # read out
             with open(nb_path, encoding="utf-8") as fp:
                 nb = nbformat.read(fp, nbformat.NO_CONVERT)
             # pre-execute
-            if self.config.get("execute_enabled"):
-                log.debug("[NbConvertPlugin] (%d) execution start: %r", i, nb_path)
+            if exe_opts is not None:
+                log.debug("[NbConvertPlugin] (%d) notebook execution start", i)
                 ts = time()
-                opts = self.config.get("execute_options") or {}
-                ep = ExecutePreprocessor(**{k: v for k, v in opts.items() if v is not None and k in ("timeout", "kernel_name")})
-                run_path = opts.get("run_path")
-                if run_path:
-                    resources = {"metadata": {"path": "run_path"}}
+                exe_completed = False
+                ep = ExecutePreprocessor(**exe_opts)
+                try:
+                    ep.preprocess(nb, {"metadata": {"path": exe_path if exe_path else input_dir}})
+                except CellExecutionError as err:
+                    if exe_exit_on_error:
+                        raise
+                    exe_completed = True
+                    log.error("[NbConvertPlugin] (%d) notebook execution error(%.3fs): %s", i, time() - ts, err)
                 else:
-                    resources = {"metadata": {"path": input_dir}}
-                ep.preprocess(nb, resources)
-                log.debug("[NbConvertPlugin] (%d) execution finished(%.2f sec): %r", i, time() - ts, nb_path)
-                if opts.get("write_back"):
-                    log.debug("[NbConvertPlugin] (%d) save: %r", i, nb_path)
-                    with open(nb_path, "w", encoding="utf-8") as fp:
-                        nbformat.write(nb, fp)
+                    exe_completed = True
+                    log.debug("[NbConvertPlugin] (%d) notebook execution finish(%.3fs)", i, time() - ts)
+                finally:
+                    if exe_save and exe_completed:
+                        log.debug("[NbConvertPlugin] (%d) save notebook", i)
+                        with open(nb_path, "w", encoding="utf-8") as fp:
+                            nbformat.write(nb, fp)
             # convert
             body, resources = exporter.from_notebook_node(nb)
             # save exported
             makedirs(md_dir, exist_ok=True)
             with open(md_path, "w", encoding="utf-8") as fp:
                 fp.write(body)
-            file_obj = File(
-                path=md_rel_path,
-                src_dir=config["docs_dir"],
-                dest_dir=config["site_dir"],
-                use_directory_urls=config["use_directory_urls"],
-            )
-
             for resource_name, resource_data in resources["outputs"].items():
                 resource_src_dir = path.dirname(file_obj.abs_src_path)
                 resource_src_path = path.join(resource_src_dir, resource_name)
-                if not path.isdir(resource_src_dir):
-                    makedirs(resource_src_dir)
+                makedirs(resource_src_dir, exist_ok=True)
                 with open(resource_src_path, "wb") as fp:
                     fp.write(resource_data)
                 self._src_files.append(resource_src_path)
                 resource_dest_dir = path.dirname(file_obj.abs_dest_path)
                 resource_dest_path = path.join(resource_dest_dir, resource_name)
                 log.debug(
                     "[NbConvertPlugin] (%d) resource output(%dBytes): %s => %s",
                     i,
                     len(resource_data),
                     resource_name,
                     resource_dest_path,
                 )
-                if not path.isdir(resource_dest_dir):
-                    makedirs(resource_dest_dir)
+                makedirs(resource_dest_dir, exist_ok=True)
                 with open(resource_dest_path, "wb") as fp:
                     fp.write(resource_data)
 
-            log.debug("[NbConvertPlugin] (%d) %r", i, file_obj)
             self._src_files.append(file_obj.abs_src_path)
             files.append(file_obj)
         return files
 
     def on_post_build(self, config, **kwargs):
         for file in self._src_files:
             log.debug("[NbConvertPlugin] remove: %r", file)
```

### Comparing `mkdocs-nbconvert-0.2/src/mkdocs_nbconvert.egg-info/PKG-INFO` & `mkdocs-nbconvert-0.2.1/src/mkdocs_nbconvert.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mkdocs-nbconvert
-Version: 0.2
+Version: 0.2.1
 Summary: A MkDocs plug-in provides a source parser for *.ipynb Jupyter notebook files, base on nbconvert.
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://tanbro.github.io/mkdocs-nbconvert
-Project-URL: Repository, https://github.com/tanbro/mkdocs_nbconvert.git
+Project-URL: Repository, https://github.com/tanbro/mkdocs-nbconvert
 Project-URL: Documentation, https://tanbro.github.io/mkdocs-nbconvert
 Keywords: mkdocs,mkdocs-plugin,jupyter,notebook,jupyter-notebook,markdown,md,nbconvert
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Documentation
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -17,17 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # mkdocs-nbconvert
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Status](https://img.shields.io/pypi/status/mkdocs-nbconvert)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
-[![PyPI - Format](https://img.shields.io/pypi/format/mkdocs-nbconvert.svg)](https://pypi.org/project/mkdocs-nbconvert/)
+[![GitHub tag (latest SemVer pre-release)](https://img.shields.io/github/v/tag/tanbro/mkdocs-nbconvert)](https://github.com/tanbro/mkdocs-nbconvert)
 
 A [MkDocs][] plug-in provides a source parser for `*.ipynb` [Jupyter][] Notebook files, base on [nbconvert][].
 
 ## References
 
 - <https://tanbro.github.io/mkdocs-nbconvert/>
 - <https://www.mkdocs.org/user-guide/plugins/>
```

