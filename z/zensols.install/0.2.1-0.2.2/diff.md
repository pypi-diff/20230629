# Comparing `tmp/zensols.install-0.2.1-py3-none-any.whl.zip` & `tmp/zensols.install-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11435 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      224 b- defN 23-Apr-06 00:52 zensols/install/__init__.py
--rw-rw-r--  2.0 unx     4945 b- defN 23-Apr-06 00:52 zensols/install/download.py
--rw-rw-r--  2.0 unx    10081 b- defN 23-Apr-06 00:52 zensols/install/installer.py
--rw-rw-r--  2.0 unx    11222 b- defN 23-Apr-06 00:52 zensols/install/resource.py
--rw-rw-r--  2.0 unx     4560 b- defN 23-Apr-06 00:52 zensols.install-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-06 00:52 zensols.install-0.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-06 00:52 zensols.install-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      668 b- defN 23-Apr-06 00:52 zensols.install-0.2.1.dist-info/RECORD
-8 files, 31808 bytes uncompressed, 10267 bytes compressed:  67.7%
+Zip file size: 11708 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      224 b- defN 23-Jun-29 17:06 zensols/install/__init__.py
+-rw-rw-r--  2.0 unx     4945 b- defN 23-Jun-29 17:06 zensols/install/download.py
+-rw-rw-r--  2.0 unx    10396 b- defN 23-Jun-29 17:06 zensols/install/installer.py
+-rw-rw-r--  2.0 unx    11191 b- defN 23-Jun-29 17:06 zensols/install/resource.py
+-rw-rw-r--  2.0 unx     5134 b- defN 23-Jun-29 17:06 zensols.install-0.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-29 17:06 zensols.install-0.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Jun-29 17:06 zensols.install-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      668 b- defN 23-Jun-29 17:06 zensols.install-0.2.2.dist-info/RECORD
+8 files, 32666 bytes uncompressed, 10540 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: zensols/install/installer.py
 Comment: 
 
 Filename: zensols/install/resource.py
 Comment: 
 
-Filename: zensols.install-0.2.1.dist-info/METADATA
+Filename: zensols.install-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: zensols.install-0.2.1.dist-info/WHEEL
+Filename: zensols.install-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: zensols.install-0.2.1.dist-info/top_level.txt
+Filename: zensols.install-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zensols.install-0.2.1.dist-info/RECORD
+Filename: zensols.install-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zensols/install/installer.py

```diff
@@ -103,15 +103,15 @@
         if self.base_directory is None:
             self.base_directory = self._get_default_base()
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f'resolved base directory: {self.base_directory}')
         if self.sub_directory is not None:
             self.base_directory = self.base_directory / self.sub_directory
         if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f'resolbed base directory: {self.base_directory}')
+            logger.debug(f'install base directory: {self.base_directory}')
 
     def _get_default_base(self) -> Path:
         existing = tuple(filter(lambda p: p.is_dir(),
                                 map(lambda p: Path(p).expanduser(),
                                     self.DEFAULT_BASE_DIRECTORIES)))
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f'existing default base directories: {existing}')
@@ -205,24 +205,30 @@
         :return: a list of statuses for each resource downloaded
 
         """
         statuses: List[Status] = []
         res: Resource
         for res in self.resources:
             local_path: Path = self.get_path(res, False)
+            check_path: Path = None
             status: Status = None
-            # we can skip installation if we already find it on the file
-            # system; however, we have to re-check compressed files in cases
-            # where we've downloaded by not uncompressed between life-cycles
+            if res.check_path is not None:
+                check_path = self.base_directory / res.check_path
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f'local path: {local_path}, ' +
-                             f'check path: {res.check_path}, ' +
+                             f'check path: {check_path}, ' +
+                             f'res check path: {res.check_path}, ' +
                              f'compressed: {res.is_compressed}')
-            if local_path.exists() and not \
-               (res.is_compressed and res.check_path is not None):
+            # we can skip installation if we already find it on the file system;
+            # however, we have to re-check compressed files in cases where we've
+            # downloaded by not uncompressed between life-cycles (ie raised
+            # exceptions)
+            if (check_path is not None and check_path.exists()) or \
+               (local_path.exists() and not
+               (res.is_compressed and res.check_path is not None)):
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f'found: {local_path}--skipping')
                 comp_path = self.get_path(res, True)
                 status = Status(res, None, comp_path, False)
             else:
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f'missing {local_path}')
```

## zensols/install/resource.py

```diff
@@ -1,13 +1,13 @@
-from __future__ import annotations
 """Installable resource.
 
 """
-__author__ = 'Paul Landes'
 
+from __future__ import annotations
+__author__ = 'Paul Landes'
 from typing import Sequence, Union
 from dataclasses import dataclass, field
 from abc import ABCMeta, abstractmethod
 import logging
 import re
 import urllib
 import shutil
@@ -55,15 +55,15 @@
     def _format_str(self, context: FileSystemUpdateContext, val: str) -> str:
         return val.format(**context.asdict())
 
     def _format_path(self, context: FileSystemUpdateContext,
                      attr: str, make_path: bool = True) -> \
             Union[Path, str]:
         val: str = getattr(self, attr)
-        path_str: str = self._format_str(context, val)#val.format(**context.asdict())
+        path_str: str = self._format_str(context, val)
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f'{attr}({val}) -> {path_str}')
         return Path(path_str) if make_path else path_str
 
     @abstractmethod
     def invoke(self, context: FileSystemUpdateContext):
         pass
```

## Comparing `zensols.install-0.2.1.dist-info/METADATA` & `zensols.install-0.2.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: zensols.install
-Version: 0.2.1
+Version: 0.2.2
 Summary: Downloads and installs (optionally compressed) files.
 Home-page: https://github.com/plandes/install
-Download-URL: https://github.com/plandes/install/releases/download/v0.2.1/zensols.install-0.2.1-py3-none-any.whl
+Download-URL: https://github.com/plandes/install/releases/download/v0.2.2/zensols.install-0.2.2-py3-none-any.whl
 Author: Paul Landes
 Author-email: landes@mailc.net
 Keywords: tooling
 Description-Content-Type: text/markdown
 Requires-Dist: patool (~=1.12)
 Requires-Dist: tqdm
 Requires-Dist: zensols.util (~=1.12.2)
@@ -17,15 +17,25 @@
 [![PyPI][pypi-badge]][pypi-link]
 [![Python 3.9][python39-badge]][python39-link]
 [![Python 3.10][python310-badge]][python310-link]
 [![Build Status][build-badge]][build-link]
 
 Simple light API to download and install files.  If the file appears to be a
 compressed file by ending with `zip`, `tar.gz`, `tgz` etc, then also un-compress
-the file after it is downloaded.
+the file after it is downloaded.  The process flow follows:
+
+1. Check to see if the installed file exists.  If not download it.
+1. Otherwise, if the file has been downloaded uncompress it.
+1. If the file could not be downloaded, uncompressed, or a file from the
+   uncompressed file isn't found an error is thrown.
+
+A destination location can be specified in the configuration.  It is also
+possible to install it in the `~/.cache/<package name>` where *package name* is
+the name the installed package.  For example, that would be `zensols.install`
+for the package installed for this repository.
 
 
 ## Documentation
 
 * [Full documentation](https://plandes.github.io/install/index.html)
 * [API reference](https://plandes.github.io/install/api.html)
 
@@ -80,15 +90,16 @@
 logging.basicConfig(level=logging.INFO)
 fac = ImportConfigFactory(IniConfig('install.conf'))
 installer: Installer = fac.instance('installer')
 installer.install()
 ```
 
 This code creates a new directory with the un-zipped files in `install_dir`:
-```bash
+
+```readline-config
 INFO:zensols.install.installer:installing zenbuild-general_build to install_dir/zenbuild-general_build
 INFO:zensols.install.download:creating directory: install_dir
 INFO:zensols.install.download:downloading https://github.com/plandes/zenbuild/archive/refs/tags/general_build.zip to install_dir/zenbuild-general_build.zip
 general_build.zip: 16.4kB [00:00, 40.1kB/s]
 INFO:zensols.install.installer:uncompressing install_dir/zenbuild-general_build.zip to install_dir
 patool: Extracting install_dir/zenbuild-general_build.zip ...
 patool: ... install_dir/zenbuild-general_build.zip extracted to `install_dir'.
```

## Comparing `zensols.install-0.2.1.dist-info/RECORD` & `zensols.install-0.2.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 zensols/install/__init__.py,sha256=8eXzuKzRzbVLQSK-Lr1Vznhb9cAoo_zDMeMpraqLy_I,224
 zensols/install/download.py,sha256=lh-nTVUBBuh80X2Xg1JoO1A49POScd66ubtlOK_LKII,4945
-zensols/install/installer.py,sha256=E0_x1scMlQYdT6W73A_fXH_wv_TGWoz3xfIujhy3sRE,10081
-zensols/install/resource.py,sha256=CsWyh-JjblnjEaq1A_ebEYvX35p6Xd8HsvVs3UjxfCs,11222
-zensols.install-0.2.1.dist-info/METADATA,sha256=VBnnFlFQWjW_rbja5zrRaf82sjNMTCCcGMp0_pDTN5E,4560
-zensols.install-0.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-zensols.install-0.2.1.dist-info/top_level.txt,sha256=lwLzgW4KCTZCqSzGcrARKMfprcfBgmpsc21niNiTKf0,16
-zensols.install-0.2.1.dist-info/RECORD,,
+zensols/install/installer.py,sha256=ITFsMcAcrSMwhYksAbBvl6oYFJZPXwRm4AhcArhVFGc,10396
+zensols/install/resource.py,sha256=gg5FJxTRDYSf11ShCMCmT64WZudWg6DO51Nw9M2ZADE,11191
+zensols.install-0.2.2.dist-info/METADATA,sha256=nl5k8zQzRD_CN8PyTqXAVP8SUSgiNRuR_fNfuQWUI50,5134
+zensols.install-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+zensols.install-0.2.2.dist-info/top_level.txt,sha256=lwLzgW4KCTZCqSzGcrARKMfprcfBgmpsc21niNiTKf0,16
+zensols.install-0.2.2.dist-info/RECORD,,
```

