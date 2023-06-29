# Comparing `tmp/craft-providers-1.8.1.tar.gz` & `tmp/craft-providers-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-providers-1.8.1.tar", last modified: Fri Mar 10 21:19:51 2023, max compression
+gzip compressed data, was "craft-providers-1.9.0.tar", last modified: Mon Mar 20 15:39:26 2023, max compression
```

## Comparing `craft-providers-1.8.1.tar` & `craft-providers-1.9.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.639117 craft-providers-1.8.1/
--rw-rw-r--   0 developer  (1000) developer  (1000)     7652 2023-01-03 18:58:38.000000 craft-providers-1.8.1/LICENSE
--rw-rw-r--   0 developer  (1000) developer  (1000)     2152 2023-03-10 21:19:51.639117 craft-providers-1.8.1/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     1374 2023-03-06 20:53:11.000000 craft-providers-1.8.1/README.md
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.631117 craft-providers-1.8.1/craft_providers/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1031 2023-03-10 21:18:47.000000 craft-providers-1.8.1/craft_providers/__init__.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.631117 craft-providers-1.8.1/craft_providers/actions/
--rw-rw-r--   0 developer  (1000) developer  (1000)      734 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/actions/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    14015 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/actions/snap_installer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5231 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/base.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.631117 craft-providers-1.8.1/craft_providers/bases/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1092 2023-02-28 20:43:34.000000 craft-providers-1.8.1/craft_providers/bases/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    42539 2023-03-10 20:08:23.000000 craft-providers-1.8.1/craft_providers/bases/buildd.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1931 2023-03-02 01:31:24.000000 craft-providers-1.8.1/craft_providers/bases/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6206 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/bases/instance_config.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2699 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6055 2023-03-02 01:31:24.000000 craft-providers-1.8.1/craft_providers/executor.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.635117 craft-providers-1.8.1/craft_providers/lxd/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1600 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/lxd/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1894 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/lxd/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4306 2023-03-02 01:31:24.000000 craft-providers-1.8.1/craft_providers/lxd/installer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    21370 2023-03-10 20:08:23.000000 craft-providers-1.8.1/craft_providers/lxd/launcher.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    32652 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/lxd/lxc.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4127 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/lxd/lxd.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    19137 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/lxd/lxd_instance.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5399 2023-03-10 20:08:23.000000 craft-providers-1.8.1/craft_providers/lxd/lxd_provider.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3381 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/lxd/project.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6805 2023-03-10 20:08:23.000000 craft-providers-1.8.1/craft_providers/lxd/remotes.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.635117 craft-providers-1.8.1/craft_providers/multipass/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1463 2023-03-02 01:31:24.000000 craft-providers-1.8.1/craft_providers/multipass/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2645 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/multipass/_launch.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1814 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/multipass/_ready.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1498 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/multipass/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2813 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/multipass/installer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    18790 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/multipass/multipass.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    13846 2023-03-06 20:53:11.000000 craft-providers-1.8.1/craft_providers/multipass/multipass_instance.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4151 2023-03-10 20:08:23.000000 craft-providers-1.8.1/craft_providers/multipass/multipass_provider.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3343 2023-03-02 01:31:24.000000 craft-providers-1.8.1/craft_providers/provider.py
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/py.typed
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.639117 craft-providers-1.8.1/craft_providers/util/
--rw-rw-r--   0 developer  (1000) developer  (1000)      725 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/util/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1960 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/util/env_cmd.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2338 2023-03-08 20:34:44.000000 craft-providers-1.8.1/craft_providers/util/os_release.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3350 2023-01-03 18:58:38.000000 craft-providers-1.8.1/craft_providers/util/snap_cmd.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1462 2023-03-02 01:31:24.000000 craft-providers-1.8.1/craft_providers/util/temp_paths.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 21:19:51.631117 craft-providers-1.8.1/craft_providers.egg-info/
--rw-rw-r--   0 developer  (1000) developer  (1000)     2152 2023-03-10 21:19:51.000000 craft-providers-1.8.1/craft_providers.egg-info/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     1505 2023-03-10 21:19:51.000000 craft-providers-1.8.1/craft_providers.egg-info/SOURCES.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-03-10 21:19:51.000000 craft-providers-1.8.1/craft_providers.egg-info/dependency_links.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       61 2023-03-10 21:19:51.000000 craft-providers-1.8.1/craft_providers.egg-info/entry_points.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-01-04 15:11:16.000000 craft-providers-1.8.1/craft_providers.egg-info/not-zip-safe
--rw-rw-r--   0 developer  (1000) developer  (1000)      567 2023-03-10 21:19:51.000000 craft-providers-1.8.1/craft_providers.egg-info/requires.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       16 2023-03-10 21:19:51.000000 craft-providers-1.8.1/craft_providers.egg-info/top_level.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)      603 2023-03-06 20:53:11.000000 craft-providers-1.8.1/pyproject.toml
--rw-rw-r--   0 developer  (1000) developer  (1000)      592 2023-03-10 21:19:51.639117 craft-providers-1.8.1/setup.cfg
--rw-rw-r--   0 developer  (1000) developer  (1000)     2787 2023-03-10 21:18:47.000000 craft-providers-1.8.1/setup.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.576409 craft-providers-1.9.0/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7652 2023-01-03 18:58:38.000000 craft-providers-1.9.0/LICENSE
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2152 2023-03-20 15:39:26.576409 craft-providers-1.9.0/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1374 2023-03-14 16:37:15.000000 craft-providers-1.9.0/README.md
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.572409 craft-providers-1.9.0/craft_providers/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1031 2023-03-20 15:38:16.000000 craft-providers-1.9.0/craft_providers/__init__.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.572409 craft-providers-1.9.0/craft_providers/actions/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      734 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/actions/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    14015 2023-03-06 20:53:11.000000 craft-providers-1.9.0/craft_providers/actions/snap_installer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5231 2023-03-14 16:37:15.000000 craft-providers-1.9.0/craft_providers/base.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.572409 craft-providers-1.9.0/craft_providers/bases/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1092 2023-02-28 20:43:34.000000 craft-providers-1.9.0/craft_providers/bases/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    43818 2023-03-20 15:36:58.000000 craft-providers-1.9.0/craft_providers/bases/buildd.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1931 2023-03-02 01:31:24.000000 craft-providers-1.9.0/craft_providers/bases/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6206 2023-03-14 16:37:15.000000 craft-providers-1.9.0/craft_providers/bases/instance_config.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2699 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6055 2023-03-02 01:31:24.000000 craft-providers-1.9.0/craft_providers/executor.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.572409 craft-providers-1.9.0/craft_providers/lxd/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1600 2023-03-14 16:37:15.000000 craft-providers-1.9.0/craft_providers/lxd/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1894 2023-03-14 16:37:15.000000 craft-providers-1.9.0/craft_providers/lxd/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4306 2023-03-02 01:31:24.000000 craft-providers-1.9.0/craft_providers/lxd/installer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    21649 2023-03-20 12:33:12.000000 craft-providers-1.9.0/craft_providers/lxd/launcher.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    32652 2023-03-06 20:53:11.000000 craft-providers-1.9.0/craft_providers/lxd/lxc.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4127 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/lxd/lxd.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    19137 2023-03-06 20:53:11.000000 craft-providers-1.9.0/craft_providers/lxd/lxd_instance.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5401 2023-03-20 12:33:12.000000 craft-providers-1.9.0/craft_providers/lxd/lxd_provider.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3381 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/lxd/project.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6805 2023-03-14 16:37:18.000000 craft-providers-1.9.0/craft_providers/lxd/remotes.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.576409 craft-providers-1.9.0/craft_providers/multipass/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1463 2023-03-02 01:31:24.000000 craft-providers-1.9.0/craft_providers/multipass/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2645 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/multipass/_launch.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1814 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/multipass/_ready.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1498 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/multipass/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2813 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/multipass/installer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    18790 2023-03-06 20:53:11.000000 craft-providers-1.9.0/craft_providers/multipass/multipass.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    13846 2023-03-06 20:53:11.000000 craft-providers-1.9.0/craft_providers/multipass/multipass_instance.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4268 2023-03-20 12:33:12.000000 craft-providers-1.9.0/craft_providers/multipass/multipass_provider.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3451 2023-03-20 12:33:12.000000 craft-providers-1.9.0/craft_providers/provider.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/py.typed
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.576409 craft-providers-1.9.0/craft_providers/util/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      725 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/util/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1960 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/util/env_cmd.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2338 2023-03-08 20:34:44.000000 craft-providers-1.9.0/craft_providers/util/os_release.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3350 2023-01-03 18:58:38.000000 craft-providers-1.9.0/craft_providers/util/snap_cmd.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1462 2023-03-02 01:31:24.000000 craft-providers-1.9.0/craft_providers/util/temp_paths.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-20 15:39:26.572409 craft-providers-1.9.0/craft_providers.egg-info/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2152 2023-03-20 15:39:26.000000 craft-providers-1.9.0/craft_providers.egg-info/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1505 2023-03-20 15:39:26.000000 craft-providers-1.9.0/craft_providers.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-03-20 15:39:26.000000 craft-providers-1.9.0/craft_providers.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       61 2023-03-20 15:39:26.000000 craft-providers-1.9.0/craft_providers.egg-info/entry_points.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-01-04 15:11:16.000000 craft-providers-1.9.0/craft_providers.egg-info/not-zip-safe
+-rw-rw-r--   0 developer  (1000) developer  (1000)      567 2023-03-20 15:39:26.000000 craft-providers-1.9.0/craft_providers.egg-info/requires.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       16 2023-03-20 15:39:26.000000 craft-providers-1.9.0/craft_providers.egg-info/top_level.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)      603 2023-03-06 20:53:11.000000 craft-providers-1.9.0/pyproject.toml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      592 2023-03-20 15:39:26.576409 craft-providers-1.9.0/setup.cfg
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2787 2023-03-20 15:38:16.000000 craft-providers-1.9.0/setup.py
```

### Comparing `craft-providers-1.8.1/LICENSE` & `craft-providers-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/PKG-INFO` & `craft-providers-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-providers
-Version: 1.8.1
+Version: 1.9.0
 Summary: Craft provider tooling
 Home-page: https://github.com/canonical/craft-providers
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `craft-providers-1.8.1/README.md` & `craft-providers-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/__init__.py` & `craft-providers-1.9.0/craft_providers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 
 """Craft Providers base package."""
 
-__version__ = "1.8.1"  # noqa: F401
+__version__ = "1.9.0"  # noqa: F401
 
 from .base import Base  # noqa: F401
 from .errors import ProviderError  # noqa: F401
 from .executor import Executor  # noqa: F401
 from .provider import Provider  # noqa: f401
 
 __all__ = [
```

### Comparing `craft-providers-1.8.1/craft_providers/actions/__init__.py` & `craft-providers-1.9.0/craft_providers/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/actions/snap_installer.py` & `craft-providers-1.9.0/craft_providers/actions/snap_installer.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/base.py` & `craft-providers-1.9.0/craft_providers/base.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/bases/__init__.py` & `craft-providers-1.9.0/craft_providers/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/bases/buildd.py` & `craft-providers-1.9.0/craft_providers/bases/buildd.py`

 * *Files 2% similar despite different names*

```diff
@@ -995,30 +995,58 @@
         :param deadline: Optional time.time() deadline.
         :param codename: New codename to use in apt source config files (i.e. 'lunar')
         """
         _check_deadline(deadline)
 
         apt_source = "/etc/apt/sources.list"
         apt_source_dir = "/etc/apt/sources.list.d/"
+        cloud_config = "/etc/cloud/cloud.cfg"
 
         # get the current ubuntu codename
         os_release = self._get_os_release(executor=executor, deadline=deadline)
         version_codename = os_release.get("VERSION_CODENAME")
-        logger.debug("updating apt sources from %r to %r", version_codename, codename)
+        logger.debug("Updating apt sources from %r to %r.", version_codename, codename)
 
         # replace all occurrences of the codename in the `sources.list` file
         sed_command = ["sed", "-i", f"s/{version_codename}/{codename}/g"]
         try:
             _execute_run(executor, sed_command + [apt_source])
         except subprocess.CalledProcessError as error:
             raise BaseConfigurationError(
                 brief=f"Failed to update {apt_source!r}.",
                 details=errors.details_from_called_process_error(error),
             ) from error
 
+        # if cloud-init and cloud.cfg isn't present, then raise an error
+        try:
+            _execute_run(executor, ["test", "-s", cloud_config])
+        except subprocess.CalledProcessError as error:
+            raise BaseConfigurationError(
+                brief=(
+                    f"Could not update {cloud_config!r} because it is empty or "
+                    "does not exist."
+                ),
+                details=errors.details_from_called_process_error(error),
+            ) from error
+
+        # update cloud.cfg to prevent the sources.list file from being reset
+        logger.debug("Updating %r to preserve apt sources.", cloud_config)
+        try:
+            _execute_run(
+                executor,
+                # 'aapt' is not a typo, the first 'a' is the sed command to append
+                # this is a shlex-compatible way to append to a file
+                ["sed", "-i", "$ aapt_preserve_sources_list: true", cloud_config],
+            )
+        except subprocess.CalledProcessError as error:
+            raise BaseConfigurationError(
+                brief=f"Failed to update {cloud_config!r}.",
+                details=errors.details_from_called_process_error(error),
+            ) from error
+
         # running `find` and `sed` as two separate calls may appear unoptimized,
         # but these shell commands will pass through `shlex.join()` before being
         # executed, which means one-liners like `find -exec sed` or
         # `find | xargs sed` cannot be used
 
         try:
             additional_source_files = _execute_run(
```

### Comparing `craft-providers-1.8.1/craft_providers/bases/errors.py` & `craft-providers-1.9.0/craft_providers/bases/errors.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/bases/instance_config.py` & `craft-providers-1.9.0/craft_providers/bases/instance_config.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/errors.py` & `craft-providers-1.9.0/craft_providers/errors.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/executor.py` & `craft-providers-1.9.0/craft_providers/executor.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/__init__.py` & `craft-providers-1.9.0/craft_providers/lxd/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/errors.py` & `craft-providers-1.9.0/craft_providers/lxd/errors.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/installer.py` & `craft-providers-1.9.0/craft_providers/lxd/installer.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/launcher.py` & `craft-providers-1.9.0/craft_providers/lxd/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,23 @@
             source_remote=remote,
             source_instance_name=instance.instance_name,
             destination_remote=remote,
             destination_instance_name=base_instance.instance_name,
             project=project,
         )
 
+        # set the full instance name as image description
+        lxc.config_set(
+            instance_name=base_instance.instance_name,
+            key="image.description",
+            value=base_instance.name,
+            project=project,
+            remote=remote,
+        )
+
     # after creating the base instance, the id map can be set
     if map_user_uid:
         _set_id_map(instance=instance, lxc=lxc, project=project, remote=remote, uid=uid)
 
     # now restart and wait for the instance to be ready
     instance.start()
     base_configuration.wait_until_ready(executor=instance)
```

### Comparing `craft-providers-1.8.1/craft_providers/lxd/lxc.py` & `craft-providers-1.9.0/craft_providers/lxd/lxc.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/lxd.py` & `craft-providers-1.9.0/craft_providers/lxd/lxd.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/lxd_instance.py` & `craft-providers-1.9.0/craft_providers/lxd/lxd_instance.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/lxd_provider.py` & `craft-providers-1.9.0/craft_providers/lxd/lxd_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,17 @@
         use `create_environment()` instead.
 
         :param project_name: Name of project.
         :param project_path: Path to project.
         :param base_configuration: Base configuration to apply to instance.
         :param build_base: Base to build from.
         :param instance_name: Name of the instance to launch.
-        :param allow_unstable: If true, allow unstable images to be launched
+        :param allow_unstable: If true, allow unstable images to be launched.
 
-        :raises LXDError: if instance cannot be configured and launched
+        :raises LXDError: if instance cannot be configured and launched.
         """
         image = get_remote_image(build_base)
         image.add_remote(lxc=self.lxc)
 
         # only allow launching unstable images when opted-in with `allow_unstable`
         if not image.is_stable and not allow_unstable:
             raise LXDUnstableImageError(
```

### Comparing `craft-providers-1.8.1/craft_providers/lxd/project.py` & `craft-providers-1.9.0/craft_providers/lxd/project.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/lxd/remotes.py` & `craft-providers-1.9.0/craft_providers/lxd/remotes.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/__init__.py` & `craft-providers-1.9.0/craft_providers/multipass/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/_launch.py` & `craft-providers-1.9.0/craft_providers/multipass/_launch.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/_ready.py` & `craft-providers-1.9.0/craft_providers/multipass/_ready.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/errors.py` & `craft-providers-1.9.0/craft_providers/multipass/errors.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/installer.py` & `craft-providers-1.9.0/craft_providers/multipass/installer.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/multipass.py` & `craft-providers-1.9.0/craft_providers/multipass/multipass.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/multipass_instance.py` & `craft-providers-1.9.0/craft_providers/multipass/multipass_instance.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/multipass/multipass_provider.py` & `craft-providers-1.9.0/craft_providers/multipass/multipass_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,26 +86,28 @@
         self,
         *,
         project_name: str,
         project_path: pathlib.Path,
         base_configuration: base.Base,
         build_base: str,
         instance_name: str,
+        allow_unstable: bool = False,
     ) -> Generator[Executor, None, None]:
         """Configure and launch environment for specified base.
 
         When this method loses context, all directories are unmounted and the
         environment is stopped. For more control of environment setup and teardown,
         use `create_environment()` instead.
 
         :param project_name: Name of the project.
         :param project_path: Path to project.
         :param base_configuration: Base configuration to apply to instance.
         :param build_base: Base to build from.
         :param instance_name: Name of the instance to launch.
+        :param allow_unstable: Unused - unstable images are not yet supported.
         """
         try:
             instance = launch(
                 name=instance_name,
                 base_configuration=base_configuration,
                 image_name=PROVIDER_BASE_TO_MULTIPASS_BASE[build_base],
                 cpus=2,
```

### Comparing `craft-providers-1.8.1/craft_providers/provider.py` & `craft-providers-1.9.0/craft_providers/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,20 +83,22 @@
         self,
         *,
         project_name: str,
         project_path: pathlib.Path,
         base_configuration: Base,
         build_base: str,
         instance_name: str,
+        allow_unstable: bool,
     ) -> Generator[Executor, None, None]:
         """Configure and launch environment for specified base.
 
         When this method loses context, all directories are unmounted and the
         environment is stopped. For more control of environment setup and teardown,
         use `create_environment()` instead.
 
         :param project_name: Name of project.
         :param project_path: Path to project.
         :param base_configuration: Base configuration to apply to instance.
         :param build_base: Base to build from.
         :param instance_name: Name of the instance to launch.
+        :param allow_unstable: If true, allow unstable images to be launched.
         """
```

### Comparing `craft-providers-1.8.1/craft_providers/util/__init__.py` & `craft-providers-1.9.0/craft_providers/util/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/util/env_cmd.py` & `craft-providers-1.9.0/craft_providers/util/env_cmd.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/util/os_release.py` & `craft-providers-1.9.0/craft_providers/util/os_release.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/util/snap_cmd.py` & `craft-providers-1.9.0/craft_providers/util/snap_cmd.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers/util/temp_paths.py` & `craft-providers-1.9.0/craft_providers/util/temp_paths.py`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers.egg-info/PKG-INFO` & `craft-providers-1.9.0/craft_providers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-providers
-Version: 1.8.1
+Version: 1.9.0
 Summary: Craft provider tooling
 Home-page: https://github.com/canonical/craft-providers
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `craft-providers-1.8.1/craft_providers.egg-info/SOURCES.txt` & `craft-providers-1.9.0/craft_providers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/craft_providers.egg-info/requires.txt` & `craft-providers-1.9.0/craft_providers.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/pyproject.toml` & `craft-providers-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/setup.cfg` & `craft-providers-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `craft-providers-1.8.1/setup.py` & `craft-providers-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "dev": dev_requires + test_requires,
     "doc": doc_requires,
     "test": test_requires,
 }
 
 setup(
     name="craft-providers",
-    version="1.8.1",
+    version="1.9.0",
     description="Craft provider tooling",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Canonical Ltd.",
     author_email="snapcraft@lists.snapcraft.io",
     url="https://github.com/canonical/craft-providers",
     classifiers=[
```

