# Comparing `tmp/slap_cli-1.9.7.tar.gz` & `tmp/slap_cli-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slap_cli-1.9.7.tar", max compression
+gzip compressed data, was "slap_cli-1.9.8.tar", max compression
```

## Comparing `slap_cli-1.9.7.tar` & `slap_cli-1.9.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1002 2023-06-20 13:32:58.376097 slap_cli-1.9.7/LICENSE
--rw-r--r--   0        0        0     4981 2023-06-20 13:36:00.993760 slap_cli-1.9.7/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-20 13:36:00.993967 slap_cli-1.9.7/src/slap/__init__.py
--rw-r--r--   0        0        0      122 2023-06-20 13:32:58.383372 slap_cli-1.9.7/src/slap/__main__.py
--rw-r--r--   0        0        0    13007 2023-06-20 13:32:58.383633 slap_cli-1.9.7/src/slap/application.py
--rw-r--r--   0        0        0     9163 2023-06-20 13:32:58.383917 slap_cli-1.9.7/src/slap/changelog.py
--rw-r--r--   0        0        0     3353 2023-06-20 13:32:58.384178 slap_cli-1.9.7/src/slap/check.py
--rw-r--r--   0        0        0     2533 2023-06-20 13:32:58.384343 slap_cli-1.9.7/src/slap/configuration.py
--rw-r--r--   0        0        0     5337 2023-06-20 13:32:58.384694 slap_cli-1.9.7/src/slap/ext/application/add.py
--rw-r--r--   0        0        0    27292 2023-06-20 13:32:58.384909 slap_cli-1.9.7/src/slap/ext/application/changelog.py
--rw-r--r--   0        0        0     6330 2023-06-20 13:32:58.385071 slap_cli-1.9.7/src/slap/ext/application/check.py
--rw-r--r--   0        0        0     3177 2023-06-20 13:32:58.385320 slap_cli-1.9.7/src/slap/ext/application/info.py
--rw-r--r--   0        0        0     4976 2023-06-20 13:35:56.901718 slap_cli-1.9.7/src/slap/ext/application/init.py
--rw-r--r--   0        0        0    13694 2023-06-20 13:32:58.385666 slap_cli-1.9.7/src/slap/ext/application/install.py
--rw-r--r--   0        0        0     5982 2023-06-20 13:32:58.385828 slap_cli-1.9.7/src/slap/ext/application/link.py
--rw-r--r--   0        0        0     4230 2023-06-20 13:32:58.385968 slap_cli-1.9.7/src/slap/ext/application/publish.py
--rw-r--r--   0        0        0    21667 2023-06-20 13:32:58.386154 slap_cli-1.9.7/src/slap/ext/application/release.py
--rw-r--r--   0        0        0     3243 2023-06-20 13:32:58.386321 slap_cli-1.9.7/src/slap/ext/application/report.py
--rw-r--r--   0        0        0     3555 2023-06-20 13:32:58.386460 slap_cli-1.9.7/src/slap/ext/application/run.py
--rw-r--r--   0        0        0     8129 2023-06-20 13:32:58.386638 slap_cli-1.9.7/src/slap/ext/application/test.py
--rw-r--r--   0        0        0    19880 2023-06-20 13:32:58.386830 slap_cli-1.9.7/src/slap/ext/application/venv.py
--rw-r--r--   0        0        0     2075 2023-06-20 13:32:58.387077 slap_cli-1.9.7/src/slap/ext/checks/changelog.py
--rw-r--r--   0        0        0     2215 2023-06-20 13:32:58.387231 slap_cli-1.9.7/src/slap/ext/checks/general.py
--rw-r--r--   0        0        0     6060 2023-06-20 13:32:58.387435 slap_cli-1.9.7/src/slap/ext/checks/poetry.py
--rw-r--r--   0        0        0     2815 2023-06-20 13:32:58.387611 slap_cli-1.9.7/src/slap/ext/checks/release.py
--rw-r--r--   0        0        0     8491 2023-06-20 13:32:58.387962 slap_cli-1.9.7/src/slap/ext/project_handlers/base.py
--rw-r--r--   0        0        0     3799 2023-06-20 13:32:58.388144 slap_cli-1.9.7/src/slap/ext/project_handlers/flit.py
--rw-r--r--   0        0        0     6462 2023-06-20 13:32:58.388289 slap_cli-1.9.7/src/slap/ext/project_handlers/poetry.py
--rw-r--r--   0        0        0     5751 2023-06-20 13:32:58.388545 slap_cli-1.9.7/src/slap/ext/project_handlers/setuptools.py
--rw-r--r--   0        0        0     1208 2023-06-20 13:32:58.388913 slap_cli-1.9.7/src/slap/ext/release/changelog.py
--rw-r--r--   0        0        0     2046 2023-06-20 13:32:58.389104 slap_cli-1.9.7/src/slap/ext/release/source_code_version.py
--rw-r--r--   0        0        0    16205 2023-06-20 13:32:58.389458 slap_cli-1.9.7/src/slap/ext/repository_ci/github_actions.py
--rw-r--r--   0        0        0     4065 2023-06-20 13:32:58.389756 slap_cli-1.9.7/src/slap/ext/repository_handlers/default.py
--rw-r--r--   0        0        0     4479 2023-06-20 13:32:58.390092 slap_cli-1.9.7/src/slap/ext/repository_hosts/github.py
--rw-r--r--   0        0        0     1357 2023-06-20 13:32:58.390281 slap_cli-1.9.7/src/slap/ext/version_incrementing_rule.py
--rw-r--r--   0        0        0    10869 2023-06-20 13:32:58.390802 slap_cli-1.9.7/src/slap/install/installer.py
--rw-r--r--   0        0        0     8308 2023-06-20 13:32:58.391026 slap_cli-1.9.7/src/slap/plugins.py
--rw-r--r--   0        0        0     8623 2023-06-20 13:32:58.391199 slap_cli-1.9.7/src/slap/project.py
--rw-r--r--   0        0        0        0 2023-06-20 13:32:58.391288 slap_cli-1.9.7/src/slap/py.typed
--rw-r--r--   0        0        0    14965 2023-06-20 13:32:58.391567 slap_cli-1.9.7/src/slap/python/dependency.py
--rw-r--r--   0        0        0     9711 2023-06-20 13:32:58.391728 slap_cli-1.9.7/src/slap/python/environment.py
--rw-r--r--   0        0        0     6833 2023-06-20 13:32:58.391915 slap_cli-1.9.7/src/slap/python/pep508.py
--rw-r--r--   0        0        0     2535 2023-06-20 13:32:58.392086 slap_cli-1.9.7/src/slap/release.py
--rw-r--r--   0        0        0     5629 2023-06-20 13:32:58.392231 slap_cli-1.9.7/src/slap/repository.py
--rw-r--r--   0        0        0     1091 2023-06-20 13:32:58.392906 slap_cli-1.9.7/src/slap/templates/github/.github/workflows/changelog.yaml
--rw-r--r--   0        0        0      972 2023-06-20 13:32:58.393041 slap_cli-1.9.7/src/slap/templates/github/.github/workflows/python.yaml
--rw-r--r--   0        0        0      246 2023-06-20 13:32:58.393303 slap_cli-1.9.7/src/slap/templates/poetry/.flake8
--rw-r--r--   0        0        0       78 2023-06-20 13:32:58.393479 slap_cli-1.9.7/src/slap/templates/poetry/.gitignore
--rw-r--r--   0        0        0        0 2023-06-20 13:32:58.393569 slap_cli-1.9.7/src/slap/templates/poetry/LICENSE
--rw-r--r--   0        0        0        9 2023-06-20 13:32:58.393696 slap_cli-1.9.7/src/slap/templates/poetry/README.md
--rw-r--r--   0        0        0     1472 2023-06-20 13:32:58.393819 slap_cli-1.9.7/src/slap/templates/poetry/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-20 13:32:58.394288 slap_cli-1.9.7/src/slap/templates/poetry/src/{path}/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 13:32:58.394392 slap_cli-1.9.7/src/slap/templates/poetry/src/{path}/py.typed
--rw-r--r--   0        0        0       67 2023-06-20 13:32:58.394614 slap_cli-1.9.7/src/slap/templates/poetry/tests/test_import.py
--rw-r--r--   0        0        0     1847 2023-06-20 13:32:58.394937 slap_cli-1.9.7/src/slap/util/cleo.py
--rw-r--r--   0        0        0     4309 2023-06-20 13:32:58.395513 slap_cli-1.9.7/src/slap/util/external/licenses.py
--rw-r--r--   0        0        0     2172 2023-06-20 13:32:58.395768 slap_cli-1.9.7/src/slap/util/external/pypi_classifiers.py
--rw-r--r--   0        0        0      418 2023-06-20 13:32:58.395903 slap_cli-1.9.7/src/slap/util/pygments.py
--rw-r--r--   0        0        0      114 2023-06-20 13:32:58.396186 slap_cli-1.9.7/src/slap/util/strings.py
--rw-r--r--   0        0        0     2113 2023-06-20 13:32:58.396434 slap_cli-1.9.7/src/slap/util/toml_file.py
--rw-r--r--   0        0        0     7363 2023-06-20 13:32:58.396668 slap_cli-1.9.7/src/slap/util/vcs.py
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-05-13 10:33:37.160056 slap_cli-1.9.8/LICENSE
+-rw-r--r--   0        0        0     4981 2023-06-29 21:46:46.271570 slap_cli-1.9.8/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-29 21:46:46.271570 slap_cli-1.9.8/src/slap/__init__.py
+-rw-r--r--   0        0        0      122 2023-06-29 21:41:59.971654 slap_cli-1.9.8/src/slap/__main__.py
+-rw-r--r--   0        0        0    13007 2023-06-29 21:41:59.971654 slap_cli-1.9.8/src/slap/application.py
+-rw-r--r--   0        0        0     9163 2023-05-13 10:33:37.164056 slap_cli-1.9.8/src/slap/changelog.py
+-rw-r--r--   0        0        0     3353 2023-05-13 10:33:37.164056 slap_cli-1.9.8/src/slap/check.py
+-rw-r--r--   0        0        0     2533 2023-06-29 21:41:59.971654 slap_cli-1.9.8/src/slap/configuration.py
+-rw-r--r--   0        0        0     5337 2023-05-13 10:33:37.164056 slap_cli-1.9.8/src/slap/ext/application/add.py
+-rw-r--r--   0        0        0    27292 2023-05-13 10:33:37.164056 slap_cli-1.9.8/src/slap/ext/application/changelog.py
+-rw-r--r--   0        0        0     6330 2023-06-29 21:41:59.971654 slap_cli-1.9.8/src/slap/ext/application/check.py
+-rw-r--r--   0        0        0     3177 2023-06-29 21:41:59.971654 slap_cli-1.9.8/src/slap/ext/application/info.py
+-rw-r--r--   0        0        0     4976 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/init.py
+-rw-r--r--   0        0        0    13694 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/install.py
+-rw-r--r--   0        0        0     5982 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/link.py
+-rw-r--r--   0        0        0     4230 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/publish.py
+-rw-r--r--   0        0        0    22457 2023-06-29 21:41:59.979654 slap_cli-1.9.8/src/slap/ext/application/release.py
+-rw-r--r--   0        0        0     3243 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/report.py
+-rw-r--r--   0        0        0     3555 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/run.py
+-rw-r--r--   0        0        0     8129 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/test.py
+-rw-r--r--   0        0        0    19880 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/application/venv.py
+-rw-r--r--   0        0        0     2075 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/checks/changelog.py
+-rw-r--r--   0        0        0     2215 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/checks/general.py
+-rw-r--r--   0        0        0     6060 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/checks/poetry.py
+-rw-r--r--   0        0        0     2815 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/ext/checks/release.py
+-rw-r--r--   0        0        0     8491 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/project_handlers/base.py
+-rw-r--r--   0        0        0     3799 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/project_handlers/flit.py
+-rw-r--r--   0        0        0     6462 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/project_handlers/poetry.py
+-rw-r--r--   0        0        0     5751 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/project_handlers/setuptools.py
+-rw-r--r--   0        0        0     1208 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/release/changelog.py
+-rw-r--r--   0        0        0     2046 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/release/source_code_version.py
+-rw-r--r--   0        0        0    16205 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/ext/repository_ci/github_actions.py
+-rw-r--r--   0        0        0     4065 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/repository_handlers/default.py
+-rw-r--r--   0        0        0     4479 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/repository_hosts/github.py
+-rw-r--r--   0        0        0     1357 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/ext/version_incrementing_rule.py
+-rw-r--r--   0        0        0    10869 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/install/installer.py
+-rw-r--r--   0        0        0     8308 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/plugins.py
+-rw-r--r--   0        0        0     8623 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/project.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/py.typed
+-rw-r--r--   0        0        0    14965 2023-05-13 18:23:43.419460 slap_cli-1.9.8/src/slap/python/dependency.py
+-rw-r--r--   0        0        0     9711 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/python/environment.py
+-rw-r--r--   0        0        0     6833 2023-06-29 21:45:30.045723 slap_cli-1.9.8/src/slap/python/pep508.py
+-rw-r--r--   0        0        0     2535 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/release.py
+-rw-r--r--   0        0        0     5651 2023-06-29 21:41:59.979654 slap_cli-1.9.8/src/slap/repository.py
+-rw-r--r--   0        0        0     1091 2023-05-13 18:54:04.063864 slap_cli-1.9.8/src/slap/templates/github/.github/workflows/changelog.yaml
+-rw-r--r--   0        0        0      972 2023-05-13 18:53:05.709519 slap_cli-1.9.8/src/slap/templates/github/.github/workflows/python.yaml
+-rw-r--r--   0        0        0      246 2023-05-13 18:23:57.759054 slap_cli-1.9.8/src/slap/templates/poetry/.flake8
+-rw-r--r--   0        0        0       78 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/templates/poetry/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/templates/poetry/LICENSE
+-rw-r--r--   0        0        0        9 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/templates/poetry/README.md
+-rw-r--r--   0        0        0     1472 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/templates/poetry/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/templates/poetry/src/{path}/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/templates/poetry/src/{path}/py.typed
+-rw-r--r--   0        0        0       67 2023-05-13 17:02:56.460903 slap_cli-1.9.8/src/slap/templates/poetry/tests/test_import.py
+-rw-r--r--   0        0        0     1847 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/util/cleo.py
+-rw-r--r--   0        0        0     4309 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/util/external/licenses.py
+-rw-r--r--   0        0        0     2172 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/util/external/pypi_classifiers.py
+-rw-r--r--   0        0        0      418 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/util/pygments.py
+-rw-r--r--   0        0        0      114 2023-06-29 21:41:59.975654 slap_cli-1.9.8/src/slap/util/strings.py
+-rw-r--r--   0        0        0     2113 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/util/toml_file.py
+-rw-r--r--   0        0        0     7363 2023-05-13 10:33:37.168056 slap_cli-1.9.8/src/slap/util/vcs.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.8/PKG-INFO
```

### Comparing `slap_cli-1.9.7/LICENSE` & `slap_cli-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/pyproject.toml` & `slap_cli-1.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "slap-cli"
-version = "1.9.7"
+version = "1.9.8"
 description = "Slap is a command-line utility for developing Python applications."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "slap", from = "src" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
@@ -20,15 +20,15 @@
 Homepage = "https://github.com/NiklasRosenstein/slap"
 Repository = "https://github.com/NiklasRosenstein/slap.git"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = "^4.10.0"
 cleo = ">=1.0.0a4"
-"databind" = "^2.0.0"
+"databind" = "^4.4.0"
 flit = "^3.6.0"
 "nr.util" = ">=0.8.12,<1.0.0"
 poetry-core = "^1.1.0a6"
 ptyprocess = "^0.7.0"
 pygments = "^2.11.2"
 PyYAML = ">=4.0"
 requests = "^2.27.1"
```

### Comparing `slap_cli-1.9.7/src/slap/application.py` & `slap_cli-1.9.8/src/slap/application.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/changelog.py` & `slap_cli-1.9.8/src/slap/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/check.py` & `slap_cli-1.9.8/src/slap/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/configuration.py` & `slap_cli-1.9.8/src/slap/configuration.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/add.py` & `slap_cli-1.9.8/src/slap/ext/application/add.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/changelog.py` & `slap_cli-1.9.8/src/slap/ext/application/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/check.py` & `slap_cli-1.9.8/src/slap/ext/application/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/info.py` & `slap_cli-1.9.8/src/slap/ext/application/info.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/init.py` & `slap_cli-1.9.8/src/slap/ext/application/init.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/install.py` & `slap_cli-1.9.8/src/slap/ext/application/install.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/link.py` & `slap_cli-1.9.8/src/slap/ext/application/link.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/publish.py` & `slap_cli-1.9.8/src/slap/ext/application/publish.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/release.py` & `slap_cli-1.9.8/src/slap/ext/application/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import dataclasses
+import subprocess
 import sys
 import typing as t
 from pathlib import Path
 
 from databind.core.settings import Alias, ExtraKeys
 
 from slap.application import Application, Command, argument, option
 from slap.configuration import Configuration
 from slap.plugins import ApplicationPlugin, ReleasePlugin, VersionIncrementingRulePlugin
+from slap.project import Project
 
 if t.TYPE_CHECKING:
     from poetry.core.semver.version import Version  # type: ignore[import]
 
-    from slap.project import Project
     from slap.release import VersionRef
 
 
 @dataclasses.dataclass
 class VersionRefConfig:
     """Version reference."""
 
@@ -49,14 +50,17 @@
     #: version number in the source code).
     references: list[VersionRefConfig] = dataclasses.field(default_factory=list)
 
     #: A list of #ReleasePlugins to use. Defaults to contain the #SourceCodeVersionReferencesPlugin
     #: and #ChangelogReleasePlugin.
     plugins: list[str] = dataclasses.field(default_factory=lambda: ["changelog_release", "source_code_version"])
 
+    #: A shell command to execute after updating files but before committing them.
+    pre_commit: t.Annotated[str | None, Alias("pre-commit")] = None
+
 
 class ReleaseCommandPlugin(Command, ApplicationPlugin):
     """Create a new release of your Python package.
 
     This command can perform the following operations in sequence (most of them need
     to be enabled explicitly with flags):
 
@@ -475,14 +479,27 @@
                 return 1
             if self.option("tag") and not self._check_clean_worktree([x.file for x in version_refs]):
                 return 1
             if self.option("dry"):
                 self.line_error("dry mode enabled, no changes will be committed to disk", "comment")
             target_version = self._get_new_version(version_refs, version)
             changed_files = self._bump_version(version_refs, target_version, self.option("dry"))
+
+            run_once = False
+            for obj, config in self.config.items():
+                if isinstance(obj, Project) and obj.directory == self.app.repository.directory:
+                    continue
+                if config.pre_commit:
+                    if not run_once:
+                        self.line("")
+                        run_once = True
+                    self.line(f"running <fg=cyan>$ {config.pre_commit}</fg> hook in <info>{obj.directory}</info>")
+                    if not self.option("dry"):
+                        subprocess.run(config.pre_commit, shell=True, check=True, cwd=obj.directory)
+
             if self.option("tag"):
                 tag_name = self._create_tag(
                     str(target_version), changed_files, self.option("dry"), self.option("force")
                 )
                 if self.option("push"):
                     self._push_to_remote(tag_name, self.option("remote"), self.option("dry"), self.option("force"))
```

### Comparing `slap_cli-1.9.7/src/slap/ext/application/report.py` & `slap_cli-1.9.8/src/slap/ext/application/report.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/run.py` & `slap_cli-1.9.8/src/slap/ext/application/run.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/test.py` & `slap_cli-1.9.8/src/slap/ext/application/test.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/application/venv.py` & `slap_cli-1.9.8/src/slap/ext/application/venv.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/checks/changelog.py` & `slap_cli-1.9.8/src/slap/ext/checks/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/checks/general.py` & `slap_cli-1.9.8/src/slap/ext/checks/general.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/checks/poetry.py` & `slap_cli-1.9.8/src/slap/ext/checks/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/checks/release.py` & `slap_cli-1.9.8/src/slap/ext/checks/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/project_handlers/base.py` & `slap_cli-1.9.8/src/slap/ext/project_handlers/base.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/project_handlers/flit.py` & `slap_cli-1.9.8/src/slap/ext/project_handlers/flit.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/project_handlers/poetry.py` & `slap_cli-1.9.8/src/slap/ext/project_handlers/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/project_handlers/setuptools.py` & `slap_cli-1.9.8/src/slap/ext/project_handlers/setuptools.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/release/changelog.py` & `slap_cli-1.9.8/src/slap/ext/release/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/release/source_code_version.py` & `slap_cli-1.9.8/src/slap/ext/release/source_code_version.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/repository_ci/github_actions.py` & `slap_cli-1.9.8/src/slap/ext/repository_ci/github_actions.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/repository_handlers/default.py` & `slap_cli-1.9.8/src/slap/ext/repository_handlers/default.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/repository_hosts/github.py` & `slap_cli-1.9.8/src/slap/ext/repository_hosts/github.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/ext/version_incrementing_rule.py` & `slap_cli-1.9.8/src/slap/ext/version_incrementing_rule.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/install/installer.py` & `slap_cli-1.9.8/src/slap/install/installer.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/plugins.py` & `slap_cli-1.9.8/src/slap/plugins.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/project.py` & `slap_cli-1.9.8/src/slap/project.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/python/dependency.py` & `slap_cli-1.9.8/src/slap/python/dependency.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/python/environment.py` & `slap_cli-1.9.8/src/slap/python/environment.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/python/pep508.py` & `slap_cli-1.9.8/src/slap/python/pep508.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/release.py` & `slap_cli-1.9.8/src/slap/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/repository.py` & `slap_cli-1.9.8/src/slap/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """Represents a pull request."""
 
     id: str
     url: str
     shortform: str
 
 
-@Union("!slap.plugins.repository_host")
+@Union("!slap.plugins.repository_host")  # type: ignore[misc]
 class RepositoryHost(abc.ABC):
     """Interface for repository hosting services to resolve issue and pull request references, comment on issues
     and create releases."""
 
     ENTRYPOINT = "slap.plugins.repository_host"
 
     @abc.abstractmethod
```

### Comparing `slap_cli-1.9.7/src/slap/templates/github/.github/workflows/changelog.yaml` & `slap_cli-1.9.8/src/slap/templates/github/.github/workflows/changelog.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/templates/github/.github/workflows/python.yaml` & `slap_cli-1.9.8/src/slap/templates/github/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/templates/poetry/pyproject.toml` & `slap_cli-1.9.8/src/slap/templates/poetry/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/util/cleo.py` & `slap_cli-1.9.8/src/slap/util/cleo.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/util/external/licenses.py` & `slap_cli-1.9.8/src/slap/util/external/licenses.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/util/external/pypi_classifiers.py` & `slap_cli-1.9.8/src/slap/util/external/pypi_classifiers.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/util/toml_file.py` & `slap_cli-1.9.8/src/slap/util/toml_file.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/src/slap/util/vcs.py` & `slap_cli-1.9.8/src/slap/util/vcs.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.7/PKG-INFO` & `slap_cli-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slap-cli
-Version: 1.9.7
+Version: 1.9.8
 Summary: Slap is a command-line utility for developing Python applications.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=4.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: build (>=0.8.0,<0.9.0)
 Requires-Dist: cleo (>=1.0.0a4)
-Requires-Dist: databind (>=2.0.0,<3.0.0)
+Requires-Dist: databind (>=4.4.0,<5.0.0)
 Requires-Dist: flit (>=3.6.0,<4.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: nr.python.environment (>=0.1.4,<0.2.0)
 Requires-Dist: nr.util (>=0.8.12,<1.0.0)
 Requires-Dist: poetry-core (>=1.1.0a6,<2.0.0)
 Requires-Dist: ptyprocess (>=0.7.0,<0.8.0)
 Requires-Dist: pygments (>=2.11.2,<3.0.0)
```

