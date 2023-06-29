# Comparing `tmp/addons_installer-3.0.0.tar.gz` & `tmp/addons_installer-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addons_installer-3.0.0.tar", last modified: Thu May  4 14:52:13 2023, max compression
+gzip compressed data, was "addons_installer-3.1.1.tar", last modified: Thu Jun 29 19:32:20 2023, max compression
```

## Comparing `addons_installer-3.0.0.tar` & `addons_installer-3.1.1.tar`

### file list

```diff
@@ -1,22 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.614966 addons_installer-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-04 14:52:13.614966 addons_installer-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5014 2023-05-02 13:47:14.000000 addons_installer-3.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-05-02 13:47:14.000000 addons_installer-3.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 14:52:13.614966 addons_installer-3.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.610966 addons_installer-3.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.610966 addons_installer-3.0.0/src/addons_installer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 13:47:14.000000 addons_installer-3.0.0/src/addons_installer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2023-05-02 13:47:14.000000 addons_installer-3.0.0/src/addons_installer/addons_installer.py
--rw-rw-rw-   0 root         (0) root         (0)     5139 2023-05-03 09:51:05.000000 addons_installer-3.0.0/src/addons_installer/api.py
--rw-rw-rw-   0 root         (0) root         (0)     7097 2023-05-03 09:51:05.000000 addons_installer-3.0.0/src/addons_installer/git_addons.py
--rw-rw-rw-   0 root         (0) root         (0)     1231 2023-05-03 09:51:05.000000 addons_installer-3.0.0/src/addons_installer/local_addons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.610966 addons_installer-3.0.0/src/addons_installer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-04 14:52:13.000000 addons_installer-3.0.0/src/addons_installer.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 14:52:13.614966 addons_installer-3.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-05-03 09:51:05.000000 addons_installer-3.0.0/tests/test_addons_finder.py
--rw-rw-rw-   0 root         (0) root         (0)     8632 2023-05-02 13:47:14.000000 addons_installer-3.0.0/tests/test_git_addons.py
--rw-rw-rw-   0 root         (0) root         (0)     7323 2023-05-03 09:51:05.000000 addons_installer-3.0.0/tests/test_local_addons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.120553 addons_installer-3.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-06-29 19:28:50.000000 addons_installer-3.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.112553 addons_installer-3.1.1/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-29 19:28:50.000000 addons_installer-3.1.1/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-29 19:28:50.000000 addons_installer-3.1.1/.idea/ruff.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.116553 addons_installer-3.1.1/.idea/runConfigurations/
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/runConfigurations/Python_all_tests.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/runConfigurations/Python_tests_in_test_addons_finder_py.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/runConfigurations/Python_tests_in_test_git_addons_py.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/runConfigurations/Python_tests_in_test_local_addons_py.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-29 19:28:50.000000 addons_installer-3.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 19:22:54.000000 addons_installer-3.1.1/.ruff
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-29 19:32:20.120553 addons_installer-3.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-06-29 19:28:50.000000 addons_installer-3.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-29 19:22:54.000000 addons_installer-3.1.1/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-29 19:28:50.000000 addons_installer-3.1.1/addons_installer.iml
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-29 19:22:54.000000 addons_installer-3.1.1/flake8-plugins.txt
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-06-29 19:28:50.000000 addons_installer-3.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 19:32:20.120553 addons_installer-3.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.112553 addons_installer-3.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.116553 addons_installer-3.1.1/src/addons_installer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 19:22:54.000000 addons_installer-3.1.1/src/addons_installer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-29 19:28:50.000000 addons_installer-3.1.1/src/addons_installer/addons_installer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-06-29 19:22:54.000000 addons_installer-3.1.1/src/addons_installer/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2023-06-29 19:28:50.000000 addons_installer-3.1.1/src/addons_installer/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     7138 2023-06-29 19:28:50.000000 addons_installer-3.1.1/src/addons_installer/git_addons.py
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-06-29 19:22:54.000000 addons_installer-3.1.1/src/addons_installer/local_addons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.116553 addons_installer-3.1.1/src/addons_installer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 19:32:20.000000 addons_installer-3.1.1/src/addons_installer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.120553 addons_installer-3.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 19:22:54.000000 addons_installer-3.1.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:32:20.120553 addons_installer-3.1.1/tests/profiles/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-29 19:22:54.000000 addons_installer-3.1.1/tests/profiles/test_profile1
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-29 19:22:54.000000 addons_installer-3.1.1/tests/profiles/test_profile2
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-29 19:22:54.000000 addons_installer-3.1.1/tests/profiles/test_profile3
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-06-29 19:28:50.000000 addons_installer-3.1.1/tests/test_addons_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)    11838 2023-06-29 19:28:50.000000 addons_installer-3.1.1/tests/test_addons_installer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8632 2023-06-29 19:22:54.000000 addons_installer-3.1.1/tests/test_git_addons.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2023-06-29 19:22:54.000000 addons_installer-3.1.1/tests/test_local_addons.py
```

### Comparing `addons_installer-3.0.0/README.md` & `addons_installer-3.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -127,7 +127,24 @@
 1.  `ADDONS_LOCAL_PATH1="/src/path1"`
 2.  `ADDONS_LOCAL_PATH2="/src/path2"`
 3.  `ADDONS_LOCAL_PATH3="/other/sub/path2"`
 
 ### ADDONS_GIT_SUBDIR_OF and ADDONS_LOCAL_SUBDIR_OF
 
 TODO: Explain this feat
+
+
+Cli
+===
+The Cli gives an entrypoint called `addons-installer`
+The Cli can be used to perform the installation of all addons declared in ENV vars, to specify which addons should be installed, or to retrieve the installing command without actually performing it.
+We can use the `--profiles` option to pass profiles files that contains ENV var declaration
+`addons-installer -help` to get usage
+
+Developper local usage
+======================
+The library can be installed with ` pip install -e .`
+Tests can be run with `python -m unittest discover`
+Cli can be used with
+```
+export ADDONS_GIT_DEFAULT_SERVER="gitlab.com"; export ADDONS_GIT_MY_PROJECT="my-project"; export ADDONS_GIT_MY_PROJECT_PROTOCOLE="public";addons-installer -install --profiles toto,truc -i my_project --cmd-only
+```
```

### Comparing `addons_installer-3.0.0/pyproject.toml` & `addons_installer-3.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools_scm[toml]>=7.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "addons_installer"
-
-version = "3.0.0"
+dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
     "typing==3.10.0.0;python_version<='3'",
+    "python-dotenv==1.0.0",
 ]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
 description = "Allow to find Odoo addons from Environment Variables"
 
-#[project.scripts]
-#odoo-env2config = "odoo_env_config.cli:env_to_config"
-#[tool.setuptools]
+[project.scripts]
+addons-installer = "addons_installer.cli:install_from_env"
+
+[tool.setuptools]
+include-package-data = true
 #packages = ["addons_installer"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools_scm]
+write_to = "src/addons_installer/_version.py"
+
 [tool.bdist_wheel]
 python-tag = "py3"
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-
 [tool.ruff]
 line-length = 120
+
+[tool.isort]
+profile = "black"
```

### Comparing `addons_installer-3.0.0/src/addons_installer/addons_installer.py` & `addons_installer-3.1.1/src/addons_installer/addons_installer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import subprocess
 import sys
 import warnings
 from os.path import exists as path_exists
 from os.path import join as path_join
-from typing import Dict, Set, Union, List, Type
+from typing import Dict, List, Set, Type, Union
 
-from .api import OdooAddonsDef, AddonsSuffix
+from .api import AddonsSuffix, OdooAddonsDef
 from .git_addons import GitOdooAddons, GitSubDirOdooAddons
 from .local_addons import LocalOdooAddons, LocalSubDirOdooAddons
 
 _logger = logging.getLogger("install_addons")
 _logger.setLevel(logging.INFO)
 
 
@@ -31,15 +31,15 @@
         GitSubDirOdooAddons,
         LocalSubDirOdooAddons,
         GitOdooAddons,
         LocalOdooAddons,
     ]
 
     @staticmethod
-    def get_addons(env_vars: Dict[str, str] = None):
+    def get_addons(env_vars: Dict[str, str] = None) -> Set[AddonsSuffix]:
         founded = {}
         for env_key in sorted(env_vars.keys()):
             addon = AddonsFinder.try_parse_key(env_key)
             if addon and env_vars.get(env_key) != str(False):
                 _logger.info("Found depends %s from %s", addon, addon.identifier)
                 founded[addon.identifier] = addon
         return set(founded.values())
@@ -91,60 +91,81 @@
 class AddonsRegistry(AddonsFinder):
     """
     Compatibility with 1.5.0
     @see AddonsFinder
     """
 
     def __init__(self):
-        warnings.warn("Depcrecated, use AddonsFinder insted. will be removed in 2.0.0", DeprecationWarning)
+        warnings.warn("Deprecated, use AddonsFinder insted. will be removed in 2.0.0", DeprecationWarning)
         super(AddonsRegistry, self).__init__()
 
 
 class OdooAddonsDefInstaller(OdooAddonsDef):
     def install(self):
         AddonsInstaller.install(self)
 
 
 class AddonsInstaller:
     @staticmethod
-    def exec_cmd(cmd: List[str], force_log=True):
+    def exec_cmd(cmd: List[str], force_log=True) -> int:
         if not cmd:
             return 0
         if force_log:
             _logger.info(" ".join(cmd))
         return AddonsInstaller.exit_if_error(subprocess.Popen(cmd).wait())
 
     @staticmethod
     def exit_if_error(error_no: int) -> int:
         if error_no:
             sys.exit(error_no)
         return error_no
 
     @staticmethod
-    def install_py_requirements(path_depot: str):
+    def install_py_requirements(path_depot: str, return_cmd: bool = False) -> List[str]:
         path_requirements = path_join(path_depot, "requirements.txt")
         if path_exists(path_requirements):
-            AddonsInstaller.exec_cmd(
-                [sys.executable, "-m", "pip", "install", "-q", "--no-input", "-r", path_requirements], True
-            )
+            cmd = [sys.executable, "-m", "pip", "install", "-q", "--no-input", "-r", path_requirements]
+            if not return_cmd:
+                AddonsInstaller.exec_cmd(cmd, True)
+            else:
+                return cmd
         else:
             _logger.debug("No requirements.txt founded in %s", path_requirements)
 
     @staticmethod
-    def install_npm_package(path_depot: str):
+    def install_npm_package(path_depot: str, return_cmd: bool = False) -> List[str]:
         path_npm = path_join(path_depot, "package.json")
         if path_exists(path_npm):
-            AddonsInstaller.exec_cmd(["npm", "install", "-g", path_npm], True)
+            cmd = ["npm", "install", "-g", path_npm]
+            if not return_cmd:
+                AddonsInstaller.exec_cmd(cmd, True)
+            else:
+                return cmd
         else:
             _logger.debug("No package.json founded in %s", path_npm)
 
     @staticmethod
-    def install(addons: OdooAddonsDef):
+    def install(addons: OdooAddonsDef, return_cmd: bool = False) -> List[List[str]]:
+        """
+        Clone the given addons and install required dependencies
+        Sys Exit with error code when errors
+        Args:
+            addons: The list of addons to install
+            return_cmd: if True, does not perform actual cloning, return only the commands to perform it
+
+        Returns:
+
+        """
         _logger.info("install %s", addons)
+        cmd_list = []
         try:
             for cmd in addons.install_cmd():
-                AddonsInstaller.exec_cmd(cmd, True)
-            AddonsInstaller.install_py_requirements(addons.addons_path)
-            AddonsInstaller.install_npm_package(addons.addons_path)
+                if not return_cmd:
+                    AddonsInstaller.exec_cmd(cmd, force_log=True)
+                else:
+                    cmd_list.append(cmd)
+            cmd_list.append(AddonsInstaller.install_py_requirements(addons.addons_path, return_cmd=return_cmd))
+            cmd_list.append(AddonsInstaller.install_npm_package(addons.addons_path, return_cmd=return_cmd))
+            return [cmd for cmd in cmd_list if cmd]  # remove None and empty
         except Exception as e:
             _logger.exception("Error", exc_info=e)
             sys.exit(1)
```

### Comparing `addons_installer-3.0.0/src/addons_installer/api.py` & `addons_installer-3.1.1/src/addons_installer/api.py`

 * *Files identical despite different names*

### Comparing `addons_installer-3.0.0/src/addons_installer/git_addons.py` & `addons_installer-3.1.1/src/addons_installer/git_addons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 from __future__ import annotations
+
 import logging
 from os.path import exists as path_exists
 from os.path import expanduser
 from os.path import join as path_join
 from typing import Dict, List
-from .api import ABCSubDirAddons, AddonsSuffix, BaseAddonsResult, OdooAddonsDef, KeySuffix
+
+from .api import (
+    ABCSubDirAddons,
+    AddonsSuffix,
+    BaseAddonsResult,
+    KeySuffix,
+    OdooAddonsDef,
+)
 
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.INFO)
 
 
 class GitOdooAddons(AddonsSuffix):
     """
     Represent a Git remote url to clone to get Odoo Addons.
 
     """
 
-    PROTOCLE_HTTPS = "https"
-    PROTOCLE_SSH = "ssh"
-    PROTOCLE_PUBLIC = "public"
+    PROTOCOLE_HTTPS = "https"
+    PROTOCOLE_SSH = "ssh"
+    PROTOCOLE_PUBLIC = "public"
     FORMAT_GIT_CLONE = {
-        PROTOCLE_HTTPS: "https://%(login)s:%(password)s@%(server)s/%(git_path)s.git",
-        PROTOCLE_SSH: "git@%(server)s:%(git_path)s.git",
-        PROTOCLE_PUBLIC: "https://%(server)s/%(git_path)s.git",
+        PROTOCOLE_HTTPS: "https://%(login)s:%(password)s@%(server)s/%(git_path)s.git",
+        PROTOCOLE_SSH: "git@%(server)s:%(git_path)s.git",
+        PROTOCOLE_PUBLIC: "https://%(server)s/%(git_path)s.git",
     }
 
     def __init__(self, base_key):
         super(GitOdooAddons, self).__init__(base_key)
         self.BRANCH = self.create_key("BRANCH", default="master")
         self.CLONE_PATH = self.create_key("CLONE_PATH")
         self.PULL_OPTIONS = self.create_key("PULL_OPTIONS", default="--depth=1,--quiet,--single-branch")
         self.HTTPS_LOGIN = self.create_key("HTTPS_LOGIN")
         self.HTTPS_PASSWORD = self.create_key("HTTPS_PASSWORD")
-        self.PROTOCOLE = self.create_key("PROTOCOLE", default=self.PROTOCLE_PUBLIC)
+        self.PROTOCOLE = self.create_key("PROTOCOLE", default=self.PROTOCOLE_PUBLIC)
         self.SERVER = self.create_key("SERVER")
 
     @property
     def prefix(self):
         return "ADDONS_GIT"
 
     def extract(self, env_vars: Dict[str, str]) -> GitOdooAddonsResult:
         res = self.to_dict(env_vars)
-        # Remove de '/' at the end and the beginning of the name '/p1/p2' become 'p1/p2'
         self._apply_check(env_vars, res)
 
+        # Remove the '/' at the end and the beginning of the name '/p1/p2' become 'p1/p2'
         res[self.NAME] = res[self.NAME].strip("/")
 
         protocole = self._get_protocole(env_vars, res)
         clone_path = self._get_clone_path(env_vars, res)
         pull_option = self._get_pull_option(res)
 
-        if self.PROTOCLE_HTTPS != protocole:
+        if self.PROTOCOLE_HTTPS != protocole:
             res.pop(self.HTTPS_LOGIN, False)
             res.pop(self.HTTPS_PASSWORD, False)
 
         return GitOdooAddonsResult(
             name=self.identifier,
             git_path=res[self.NAME],
             branch=res[self.BRANCH],
@@ -68,39 +76,39 @@
 
     def _get_protocole(self, env_vars: Dict[str, str], res: Dict[KeySuffix, str]):
         if (
             not self.PROTOCOLE.get_value(env_vars, with_default=False)
             and res[self.HTTPS_LOGIN]
             and res[self.HTTPS_PASSWORD]
         ):
-            return self.PROTOCLE_HTTPS
+            return self.PROTOCOLE_HTTPS
         return res[self.PROTOCOLE]
 
     def _apply_check(self, env_vars: Dict[str, str], res: Dict[KeySuffix, str]):
         if not res[self.SERVER]:
             raise ValueError(
                 "Not git server is provided, key [%s] or [%s]" % (self.SERVER.full_key, self.SERVER.default_key)
             )
         if res[self.PROTOCOLE] not in self.FORMAT_GIT_CLONE.keys():
             raise ValueError(
                 "The selected protocole %s is not supported, possible values are %s"
                 % (res[self.PROTOCOLE], sorted(list(self.FORMAT_GIT_CLONE.keys())))
             )
-        if self.PROTOCLE_SSH == res[self.PROTOCOLE]:
-            raise ValueError("Protocole [%s] not supported for the moment" % self.PROTOCLE_SSH)
+        if self.PROTOCOLE_SSH == res[self.PROTOCOLE]:
+            raise ValueError("Protocole [%s] not supported for the moment" % self.PROTOCOLE_SSH)
 
         protocole = self._get_protocole(env_vars, res)
-        if self.PROTOCLE_HTTPS == protocole:
+        if self.PROTOCOLE_HTTPS == protocole:
             if not res[self.HTTPS_LOGIN] or not res[self.HTTPS_PASSWORD]:
                 raise ValueError(
                     "Please add %s and %s var in your environment when you use [%s] has git protocole"
                     % (
                         self.HTTPS_LOGIN.full_key,
                         self.HTTPS_PASSWORD.full_key,
-                        self.PROTOCLE_HTTPS,
+                        self.PROTOCOLE_HTTPS,
                     )
                 )
 
     def _get_clone_path(self, env_vars, res):
         # type: (Dict[str, str], Dict[KeySuffix, str]) -> str
         if self.CLONE_PATH.default_key in env_vars and self.CLONE_PATH.full_key not in env_vars:
             # If default key in env_vars but not dedicated key then we add identifier in lower case to the clone path
```

### Comparing `addons_installer-3.0.0/src/addons_installer/local_addons.py` & `addons_installer-3.1.1/src/addons_installer/local_addons.py`

 * *Files identical despite different names*

### Comparing `addons_installer-3.0.0/tests/test_addons_finder.py` & `addons_installer-3.1.1/tests/test_addons_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
+from addons_installer.addons_installer import AddonsFinder
+from addons_installer.api import BaseAddonsResult, OdooAddonsDef
 from addons_installer.git_addons import GitOdooAddons, GitOdooAddonsResult
 from addons_installer.local_addons import LocalOdooAddons
-from addons_installer.addons_installer import AddonsFinder
-from addons_installer.api import OdooAddonsDef, BaseAddonsResult
 
 
 class TestAddonsFinder(unittest.TestCase):
     def setUp(self):
         self.registry = AddonsFinder()
 
     def test_try_parse_key_local(self):
```

### Comparing `addons_installer-3.0.0/tests/test_git_addons.py` & `addons_installer-3.1.1/tests/test_git_addons.py`

 * *Files identical despite different names*

### Comparing `addons_installer-3.0.0/tests/test_local_addons.py` & `addons_installer-3.1.1/tests/test_local_addons.py`

 * *Files identical despite different names*

