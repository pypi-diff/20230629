# Comparing `tmp/blackboardsync-0.9.5a1.tar.gz` & `tmp/blackboardsync-0.9.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.5a1.tar", last modified: Tue Jun 27 16:01:39 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.6a1.tar", last modified: Thu Jun 29 14:28:20 2023, max compression
```

## Comparing `blackboardsync-0.9.5a1.tar` & `blackboardsync-0.9.6a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.742287 blackboardsync-0.9.5a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.742287 blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.742287 blackboardsync-0.9.5a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.746287 blackboardsync-0.9.5a1/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.746287 blackboardsync-0.9.5a1/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.746287 blackboardsync-0.9.5a1/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.562580 blackboardsync-0.9.6a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.562580 blackboardsync-0.9.6a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.562580 blackboardsync-0.9.6a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.566581 blackboardsync-0.9.6a1/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 14:28:20.000000 blackboardsync-0.9.6a1/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:28:20.570581 blackboardsync-0.9.6a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-29 14:27:30.000000 blackboardsync-0.9.6a1/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.6a1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/.github/workflows/build.yml` & `blackboardsync-0.9.6a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/.gitignore` & `blackboardsync-0.9.6a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/CHANGELOG.md` & `blackboardsync-0.9.6a1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.6] - 2023-06-29
+
+### Changed
+- Changing download since to an earlier year will cause a redownload
+- PyInstaller has been upgraded to 5.13, and other dependencies have also been upgraded
+
+### Fixed
+- Bug where resetting download since to 'all' would not take effect
+- Type hints were improved
+
 ## [0.9.5] - 2023-06-27
 
 ### Added
 - Option to go over setup wizard again after initial setup
 
 ### Fixed
 - Issue with session logging back in immediately after logout
```

### Comparing `blackboardsync-0.9.5a1/CONTRIBUTING.md` & `blackboardsync-0.9.6a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/LICENSE` & `blackboardsync-0.9.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/PKG-INFO` & `blackboardsync-0.9.6a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.5a1
+Version: 0.9.6a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -121,15 +121,14 @@
 ```
 
 
 
 To start the program
 
 ```bash
-cd blackboard_sync
 pipenv run python -m blackboard_sync
 ```
```

### Comparing `blackboardsync-0.9.5a1/Pipfile.lock` & `blackboardsync-0.9.6a1/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738464830376595%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'f1a1e9371ea7ae149569a27d835043205b2d3273a4423f1404259e275a536f33'}}",*

 * * "'default'": '{\'charset-normalizer\': {\'markers\': "python_full_version >= \'3.7.0\'"}, '*

 * *              "'typing-extensions': {'hashes': "*

 * *              "['sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771', "*

 * *              "'sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82'], "*

 * *              "'version': '==4.7.0'}}",*

 * * "'develop'": '{\'charset […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "98a952fb74aeef537f79e055303774178979d611ff7c00a5b0aeda9b768d4c13"
+            "sha256": "f1a1e9371ea7ae149569a27d835043205b2d3273a4423f1404259e275a536f33"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -114,15 +114,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
@@ -375,19 +375,19 @@
                 "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.4.1"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
-                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+                "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771",
+                "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.6.3"
+            "version": "==4.7.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
                 "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
@@ -639,15 +639,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
@@ -789,19 +789,19 @@
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "version": "==6.0.0"
         },
         "hypothesis": {
             "hashes": [
-                "sha256:51fb2259489dc446d3edc04cbc8ebd5848d7d3f238121183bee5449b91f7a8d8",
-                "sha256:564d9860ed5e09b0434b7bafea392b0da8f67131190202c6002e58c2c96b7596"
+                "sha256:63dc6b094b52da6180ca50edd63bf08184bc96810f8624fdbe66578aaf377993",
+                "sha256:75d74da36fd3837b5b3fe15211dabc7389e78d882bf2c91bab2184ccf91fe64c"
             ],
             "index": "pypi",
-            "version": "==6.79.2"
+            "version": "==6.80.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -872,19 +872,19 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:ade5e1e7710a7579d7c01e64a712926270239aba48055b1cdc6c022dd6d789b5",
-                "sha256:bd48a36612ef55505bf70e563528e3e66ba93267e344b6780cf6151f9c1eda6d"
+                "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
+                "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==24.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.2.0"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
                 "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
                 "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
                 "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
@@ -1009,43 +1009,43 @@
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.1.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:0cf0ca95e4b8adeaf07815a78b4096b65adf64ea7871b39a2116c19497fcd0dd",
-                "sha256:0f98973e39e4a98709546a9afd82e1ffcc50c6ec9ce6f7870f33ebbf0bd4f26d",
-                "sha256:19d42b08c7532d736a7e0fb29525855e355fa51fd6aef4f9bbc80749ff64b1a2",
-                "sha256:210fe0f39ec5be45dd9d0de253cb79245f0a6f27631d62e0c9c7988be7152965",
-                "sha256:3b1b5c875fcf3e7217a3de7f708166f641ca154b589664c44a6fd6d9f17d9e7e",
-                "sha256:3f2b353eebef669529d9bd5ae3566905a685ae98b3af3aad7476d0d519714758",
-                "sha256:50f65f0e9985f1e50040e603baebab83efed9eb37e15a22a4246fa7cd660f981",
-                "sha256:53c2a1fed81e05ded10a4557fe12bae05b9ecf9153f162c662a71d924d504135",
-                "sha256:5a0ee54c2cb0f957f8a6f41794d68f1a7e32b9968675ade5846f538504856d42",
-                "sha256:62bf18d97c6b089f77f0067b4e321db089d8520cdeefc6ae3ec0f873621c22e5",
-                "sha256:653863c75f0dbb687d92eb0d4bd9fe7047d096987ecac93bb7b1bc336de48ebd",
-                "sha256:67242d5b28ed0fa88edd8f880aed24da481929467fdbca6487167cb5e3fd31ff",
-                "sha256:6ba9a69172abaa73910643744d3848877d6aac4a20c41742027dcfd8d78f05d9",
-                "sha256:6c34d43e3d54ad05024576aef28081d9d0580f6fa7f131255f54020eb12f5352",
-                "sha256:7461469e163f87a087a5e7aa224102a30f037c11a096a0ceeb721cb0dce274c8",
-                "sha256:94a81b9354545123feb1a99b960faeff9e1fa204fce47e0042335b473d71530d",
-                "sha256:a0b2e0da7ff9dd8d2066d093d35a169305fc4e38db378281fce096768a3dbdbf",
-                "sha256:a34eed094c16cad0f6b0d889811592c7a9b7acf10d10a7356349e325d8704b4f",
-                "sha256:a3af348e0925a59213244f28c7c0c3a2c2088b4ba2fe9d6c8d4fbb0aba0b7d05",
-                "sha256:b4c734d947e761c7ceb1f09a98359dd5666460acbc39f7d0a6b6beec373c5840",
-                "sha256:bba57b4d2328740749f676807fcf3036e9de723530781405cc5a5e41fc6e20de",
-                "sha256:ca33ab70a4aaa75bb01086a0b04f0ba8441e51e06fc57e28585176b08cad533b",
-                "sha256:de1e7e68148a213036276d1f5303b3836ad9a774188961eb2684eddff593b042",
-                "sha256:f051ca656be0c179c735a4c3193f307d34c92fdc4908d44fd4516fbe8b10567d",
-                "sha256:f5984a8d13d35624e3b235a793c814433d810acba9eeefe665cdfed3d08bc3af",
-                "sha256:f7a5971490fd4a5a436e143105a1f78fa8b3fe95b30fff2a77542b4f3227a01f"
+                "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
+                "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
+                "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
+                "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
+                "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7",
+                "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3",
+                "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816",
+                "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3",
+                "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc",
+                "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4",
+                "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b",
+                "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8",
+                "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c",
+                "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462",
+                "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7",
+                "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc",
+                "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258",
+                "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b",
+                "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9",
+                "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6",
+                "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f",
+                "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1",
+                "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828",
+                "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878",
+                "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f",
+                "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"
             ],
             "index": "pypi",
-            "version": "==1.4.0"
+            "version": "==1.4.1"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -1213,37 +1213,37 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyinstaller": {
             "hashes": [
-                "sha256:036a062a228af41f6bb6370a4e87cef34858cc839200a07ace7f8738ef64ad86",
-                "sha256:049cdc3524aefb5ca015a63d2c81b6bf1567cc818ac066859fbfde702c6165d3",
-                "sha256:0af9d11a09ce217d32f95c79c984054457b310671387ff32bae1496876308556",
-                "sha256:2a1fe6d0da22f207cfa4b3221fe365503cba071c77aac19f76a75503f67d9ff9",
-                "sha256:42fdea67e4c2217cedd54d17d1d402736df3ba718db2b497df65df5a68ae4f93",
-                "sha256:8454bac8f3cb2219a3ce2227fd039bdaf943dcba60e8c55732958ea3a6d81263",
-                "sha256:a445a91b85c9a1ea3985268643a674900dd86f244cc4be4ff4ec4c6367ff99a9",
-                "sha256:b3c6299fd7526c6ca87ea5f9017fb1928d47046df0b9f983d6bbd893801010dc",
-                "sha256:b4cac0e7b0d63c6a869843113008f59fd5b38b2959ffa6059e7fac4bb05de92b",
-                "sha256:b8a4f6834e5c85150948e22c74dd3ab8b98aa4ccdf964d880ac14d2f78d9c1a4",
-                "sha256:cb87cee0b3c81ccd74d4bf3f4faf03b5e1e39bb91f1a894b2ce4cd22363bf779",
-                "sha256:e359571327bbef434fc61324891399f9117efbb685b5065234eebb01713650a8"
+                "sha256:0df43697c4914285ecd333be968d2cd042ab9b2670124879ee87931d2344eaf5",
+                "sha256:1fde4381155f21d6354dc450dcaa338cd8a40aaacf6bd22b987b0f3e1f96f3ee",
+                "sha256:24009eba63cfdbcde6d2634e9c87f545eb67249ddf3b514e0cd3b2cdaa595828",
+                "sha256:28d9742c37e9fb518444b12f8c8ab3cb4ba212d752693c34475c08009aa21ccf",
+                "sha256:2d03419904d1c25c8968b0ad21da0e0f33d8d65716e29481b5bd83f7f342b0c5",
+                "sha256:3a331951f9744bc2379ea5d65d36f3c828eaefe2785f15039592cdc08560b262",
+                "sha256:5e446df41255e815017d96318e39f65a3eb807e74a796c7e7ff7f13b6366a2e9",
+                "sha256:78975043edeb628e23a73fb3ef0a273cda50e765f1716f75212ea3e91b09dede",
+                "sha256:7fdd319828de679f9c5e381eff998ee9b4164bf4457e7fca56946701cf002c3f",
+                "sha256:9fc27c5a853b14a90d39c252707673c7a0efec921cd817169aff3af0fca8c127",
+                "sha256:cd7d5c06f2847195a23d72ede17c60857d6f495d6f0727dc6c9bc1235f2eb79c",
+                "sha256:e5fb17de6c325d3b2b4ceaeb55130ad7100a79096490e4c5b890224406fa42f4"
             ],
             "index": "pypi",
-            "version": "==5.11.0"
+            "version": "==5.13.0"
         },
         "pyinstaller-hooks-contrib": {
             "hashes": [
-                "sha256:062ad7a1746e1cfc24d3a8c4be4e606fced3b123bda7d419f14fcf7507804b07",
-                "sha256:bb39e1038e3e0972420455e0b39cd9dce73f3d80acaf4bf2b3615fea766ff370"
+                "sha256:9c11197653de9605a81975325a60b9369e9cdc37c009b6aeb0221a57211f9388",
+                "sha256:fc9892e46fa19d05725205413fb21a764f2f6ff1e70ba95322fb02420a665a45"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2023.3"
+            "version": "==2023.4"
         },
         "pylint": {
             "hashes": [
                 "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
                 "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "version": "==2.17.4"
@@ -1252,14 +1252,22 @@
             "hashes": [
                 "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
+        "pyqt5-stubs": {
+            "hashes": [
+                "sha256:7fb8177c72489a8911f021b7bd7c33f12c87f6dba92dcef3fdcdb5d9400f0f3f",
+                "sha256:91270ac23ebf38a1dc04cd97aa852cd08af82dc839100e5395af1447e3e99707"
+            ],
+            "index": "pypi",
+            "version": "==5.15.6.0"
+        },
         "pytest": {
             "hashes": [
                 "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
             "version": "==7.4.0"
@@ -1307,19 +1315,19 @@
                 "sha256:a50f9dfe23b03a9d40414c1fdf902fefbeae12f2ac75a3c8f915944d6ffac279"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.2.5"
         },
         "pywin32-ctypes": {
             "hashes": [
-                "sha256:934a2def1e5cbc472b2b6bf80680c0f03cd87df65dfd58bfd1846969de095b03",
-                "sha256:b9a53ef754c894a525469933ab2a447c74ec1ea6b9d2ef446f40ec50d3dcec9f"
+                "sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60",
+                "sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7"
             ],
             "index": "pypi",
-            "version": "==0.2.1"
+            "version": "==0.2.2"
         },
         "readme-renderer": {
             "hashes": [
                 "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
                 "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
             "markers": "python_version >= '3.8'",
@@ -1358,15 +1366,15 @@
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
         "rope": {
             "hashes": [
                 "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd",
                 "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"
             ],
@@ -1497,21 +1505,67 @@
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
+        "types-appdirs": {
+            "hashes": [
+                "sha256:337c750e423c40911d389359b4edabe5bbc2cdd5cd0bd0518b71d2839646273b",
+                "sha256:83268da64585361bfa291f8f506a209276212a0497bd37f0512a939b3d69ff14"
+            ],
+            "index": "pypi",
+            "version": "==1.4.3.5"
+        },
+        "types-beautifulsoup4": {
+            "hashes": [
+                "sha256:718364c8e6787884501c700b1d22b6c0a8711bf9d6c9bf96e1fba81495bc46a8",
+                "sha256:d9be456416a62a5b9740559592e1063a69d4b0a1b83911d878558c8ae8e07074"
+            ],
+            "index": "pypi",
+            "version": "==4.12.0.5"
+        },
+        "types-html5lib": {
+            "hashes": [
+                "sha256:091e9e74e0ee37c93fd789a164e99b2af80ecf5a314280450c6a763d027ea209",
+                "sha256:758c1a27f3b63363a346f3646be9f8b1f25df4fc1f96f88af6d1d831f24ad675"
+            ],
+            "version": "==1.1.11.14"
+        },
+        "types-python-dateutil": {
+            "hashes": [
+                "sha256:09a0275f95ee31ce68196710ed2c3d1b9dc42e0b61cc43acc369a42cb939134f",
+                "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
+            ],
+            "index": "pypi",
+            "version": "==2.8.19.13"
+        },
+        "types-requests": {
+            "hashes": [
+                "sha256:3de667cffa123ce698591de0ad7db034a5317457a596eb0b4944e5a9d9e8d1ac",
+                "sha256:afb06ef8f25ba83d59a1d424bd7a5a939082f94b94e90ab5e6116bd2559deaa3"
+            ],
+            "index": "pypi",
+            "version": "==2.31.0.1"
+        },
+        "types-urllib3": {
+            "hashes": [
+                "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
+                "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
+            ],
+            "version": "==1.26.25.13"
+        },
         "typing-extensions": {
             "hashes": [
-                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
-                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+                "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771",
+                "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.6.3"
+            "version": "==4.7.0"
         },
         "ujson": {
             "hashes": [
                 "sha256:07d459aca895eb17eb463b00441986b021b9312c6c8cc1d06880925c7f51009c",
                 "sha256:0be81bae295f65a6896b0c9030b55a106fb2dec69ef877253a87bc7c9c5308f7",
                 "sha256:0fe1b7edaf560ca6ab023f81cbeaf9946a240876a993b8c5a21a1c539171d903",
                 "sha256:102bf31c56f59538cccdfec45649780ae00657e86247c07edac434cb14d5388c",
```

### Comparing `blackboardsync-0.9.5a1/README.md` & `blackboardsync-0.9.6a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 ```
 
 
 
 To start the program
 
 ```bash
-cd blackboard_sync
 pipenv run python -m blackboard_sync
 ```
```

### Comparing `blackboardsync-0.9.5a1/UNIVERSITIES.md` & `blackboardsync-0.9.6a1/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/__about__.py` & `blackboardsync-0.9.6a1/blackboard_sync/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.5-alpha.1"
+__version__ = "0.9.6-alpha.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/__init__.py` & `blackboardsync-0.9.6a1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/__main__.py` & `blackboardsync-0.9.6a1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.6a1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.6a1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.6a1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.6a1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.6a1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.6a1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.6a1/blackboard_sync/blackboard/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # You should have received a copy of the GNU General Public License v2
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor,
 # Boston, MA  02110-1301, USA.
 
 import logging
-from typing import Union
+from typing import Union, Optional
 from functools import wraps
 from collections.abc import Callable
 
 import requests
 from requests.cookies import RequestsCookieJar
 
 from .blackboard import (BBCourse, BBAttachment, BBMembership, BBContentChild,
@@ -54,15 +54,15 @@
     def __init__(self, base_url: str, cookies: RequestsCookieJar):
         # Root API URL
         self._base_url = base_url
         # Use cookies for requests
         self._bb_session = requests.Session()
         self._bb_session.cookies = cookies
         # Obtain username by calling self
-        self._username = None
+        self._username : Optional[str] = None
         self._timeout = 12
 
     def get(endpoint: str, version: int = 1, use_api: bool = True, json: bool = True, **g_kwargs):
         """Return a decorator (needed to use fancy notation).
 
         :param string endpoint: Endpoint to make API call to, including placeholders
         :param int version: Version of the BB API used at endpoint (used as part of url)
@@ -256,15 +256,15 @@
         """
         return [BBContentChild(**child) for child in response]
 
     # content file attachments #
 
     # Get File Attachment(s)
     @get("/courses/{course_id}/contents/{content_id}/attachments/{attachment_id}")
-    def fetch_file_attachments(self, response) -> list[BBAttachment]:
+    def fetch_file_attachments(self, response) -> list[BBAttachment] | BBAttachment:
         """Get the file attachment meta data associated to the Content Item.
 
         or Get the file attachment meta data by an attachment ID.
 
         :param course_id: The course or organization ID.
         :param content_id: The Content ID.
         :param attachment_id:
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/config.py` & `blackboardsync-0.9.6a1/blackboard_sync/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,9 +111,9 @@
 
     @property
     def min_year(self) -> Optional[int]:
         return self._sync.getint('min_year')
 
     @min_year.setter
     @Config.persist
-    def min_year(self, year: int) -> None:
-        self._sync['min_year'] = str(year)
+    def min_year(self, year: Optional[int])-> None:
+        self._sync['min_year'] = str(year or 0)
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/download.py` & `blackboardsync-0.9.6a1/blackboard_sync/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,19 @@
 
     _last_downloaded = datetime.fromtimestamp(0, tz=timezone.utc)
 
     _logger = logging.getLogger(__name__)
     _logger.setLevel(logging.DEBUG)
     _logger.addHandler(logging.StreamHandler())
 
-    def __init__(self, sess: BlackboardSession, download_location: Path,
-                 last_downloaded: datetime = None, data_sources: list[str] = [], min_year: int = None):
+    def __init__(self, sess: BlackboardSession,
+                 download_location: Path,
+                 last_downloaded: Optional[datetime] = None,
+                 data_sources: list[str] = [],
+                 min_year: Optional[int] = None):
         """BlackboardDownload constructor
 
         Download all files in blackboard recursively to download_location,
         only if they have been altered since specified datetime
 
         Keyword arguments:
 
@@ -93,15 +96,15 @@
         """Get stream for blackboard file and download."""
         try:
             d_stream = self._sess.download(course_id=course_id,
                                        content_id=content_id,
                                        attachment_id=attachment_id)
             self._download_stream(d_stream, file_path)
         except RequestException as e:
-            self.logger.warn(f"Error while downloading file {link}")
+            self.logger.warn(f"Error while downloading file {content_id}")
 
     def _download_webdav_file(self, link: str, file_path: Path) -> None:
         try:
             response = self._sess.download_webdav(webdav_url=link)
             if validate_webdav_response(response, link, self._sess.base_url):
                 self._download_stream(response, file_path)
             else:
@@ -116,25 +119,33 @@
             self.logger.info(f"Writing to {file_path}")
             for chunk in stream.iter_content(chunk_size=1024):
                 f.write(chunk)
 
     def _handle_file(self, content: BBCourseContent, parent_path: Path,
                      course_id: str, depth: int = 0) -> None:
         """Download BBContent recursively, depending on filetype"""
-        self.logger.info(f"{'    ' * depth}{content.title}[{content.contentHandler.id}]")
-
         if self.cancelled:
             return
 
         res = content.contentHandler
+
+        handler_id = res.id if res is not None else '?'
+        self.logger.info(f"{'    ' * depth}{content.title}[{handler_id}]")
+
         body_path = parent_path
         file_path = Path(parent_path, content.title_path_safe)
-        has_changed = (content.modified >= self._last_downloaded)
+        has_changed = True
+
+        if content.modified is not None:
+            has_changed = (content.modified >= self._last_downloaded)
+
+        if res is None:
+            pass
 
-        if res == BBResourceType.folder:
+        elif res == BBResourceType.folder:
             try:
                 body_path = file_path
                 children = self._sess.fetch_content_children(course_id=course_id,
                                                              content_id=content.id)
 
                 if children or content.body:
                     file_path.mkdir(exist_ok=True, parents=True)
@@ -155,22 +166,25 @@
                 body_path = file_path
 
             for attachment in attachments:
                 download_path = Path(body_path / attachment.fileName)
                 if attachment.mimeType.startswith('video/'):
                     self.logger.info(f'Not downloading {attachment.fileName}')
                 else:
-                    if not self.cancelled:
-                        self.executor.submit(self._download_file, course_id, content.id, attachment.id, download_path)
+                    if not self.cancelled and content.id is not None:
+                        self.executor.submit(self._download_file,
+                                             course_id, content.id,
+                                             attachment.id, download_path)
 
         elif res == BBResourceType.externallink and has_changed:
             # Place link under folder of its own, in case it has a body
             file_path.mkdir(exist_ok=True, parents=True)
             link_path = file_path / content.title_path_safe
-            self._create_desktop_link(link_path, res.url)
+            if res.url is not None:
+                self._create_desktop_link(link_path, res.url)
 
         elif not res.is_not_handled and has_changed:
             self.logger.warning(f"Not handled, {content.title}")
 
         # If item has body, write in markdown file
         if content.body and has_changed:
             file_path.mkdir(exist_ok=True, parents=True)
@@ -241,15 +255,15 @@
         return start_time
 
     def cancel(self) -> None:
         """Cancel the download job."""
         self.cancelled = True
 
     @property
-    def download_location(self) -> str:
+    def download_location(self) -> Path:
         """The location where files will be downloaded to."""
         return self._download_location
 
     @property
     def data_sources(self) -> list[str]:
         """Filter for courses."""
         return self._data_sources
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/institutions.py` & `blackboardsync-0.9.6a1/blackboard_sync/institutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,7 +133,8 @@
                     found = True
         if ip_isp:
             for isp in uni.network.isp:
                 if ip_isp == isp:
                     found = True
         if found:
             return i
+    return None
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.6a1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.6a1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.6a1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.6a1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.6a1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.6a1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.6a1/blackboard_sync/qt/qt_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import os
+import sys
 import json
 import platform
 import subprocess
 import webbrowser
 from enum import IntEnum
 from typing import Optional
 from pathlib import Path
 
 from PyQt5 import uic
 from PyQt5.QtGui import QIcon, QPixmap
 from PyQt5.QtCore import Qt, QSettings, QUrl, pyqtSlot, pyqtSignal
 from PyQt5.QtNetwork import QNetworkCookie
 from PyQt5.QtWidgets import (QMenu, QStyle, QAction, QDialog, QWidget, QWizard,
-                             QCompleter, QFileDialog, QMessageBox,
-                             QApplication, QSystemTrayIcon)
+                             QCompleter, QFileDialog, QMessageBox, QApplication,
+                             QSystemTrayIcon, QComboBox, QLabel, QCheckBox, QSpinBox)
 from requests.cookies import RequestsCookieJar
 from PyQt5.QtWebEngineCore import QWebEngineCookieStore
-from PyQt5.QtWebEngineWidgets import QWebEnginePage, QWebEngineProfile
+from PyQt5.QtWebEngineWidgets import QWebEngineView, QWebEnginePage, QWebEngineProfile
 
 
 class SyncPeriod(IntEnum):
     """Enum containing all valid Sync intervals for this UI."""
 
     HALF_HOUR = 60 * 30
     ONE_HOUR = 60 * 60
@@ -63,33 +64,31 @@
 
     @staticmethod
     def _get_asset_path(icon) -> Path:
         """Get the `Path` of a media asset."""
         return (Path(__file__).parent.parent / 'assets' / icon).resolve()
 
     @classmethod
-    @property
     def icon(cls) -> QIcon:
         """`QIcon` of application logo."""
         return QIcon(str(cls._get_asset_path(cls._icon_filename)))
 
     @classmethod
-    @property
     def watermark(cls) -> QPixmap:
         """`QPixmap` of application watermark."""
         wm = QPixmap(str(cls._get_asset_path(cls._watermark_filename)))
         wm = wm.scaledToWidth(100)
         return wm
 
 
 class OSUtils:
     @staticmethod
     def open_dir_in_file_browser(dir_to_open: Path) -> None:
         """Start a subprocess to open the default file explorer at the given location."""
-        if platform.system() == "Windows":
+        if sys.platform == "win32":
             os.startfile(dir_to_open)
         elif platform.system() == "Darwin":
             subprocess.Popen(["open", dir_to_open])
         else:
             subprocess.Popen(["xdg-open", dir_to_open])
 
     @staticmethod
@@ -212,15 +211,15 @@
     def __init__(self):
         """Create a `QSystemTrayIcon`."""
         super().__init__()
         self._init_ui()
 
     def _init_ui(self) -> None:
         # Create the icon
-        icon = Assets.icon
+        icon = Assets.icon()
 
         # Create the tray
         self.setIcon(icon)
         self.setVisible(True)
 
         # Create the menu
         self._menu = SyncTrayMenu()
@@ -314,15 +313,15 @@
     def _init_ui(self) -> None:
         self.setText(self._dialog_text)
         self.setInformativeText(self._info_text)
         self.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
         self.setDefaultButton(QMessageBox.No)
         self.setWindowTitle(self._window_title)
         self.setIcon(QMessageBox.Question)
-        self.setWindowIcon(Assets.icon)
+        self.setWindowIcon(Assets.icon())
 
     @property
     def redownload(self) -> bool:
         """Indicate if files have to be redownloaded."""
         return self.exec() == QMessageBox.Yes
 
 
@@ -341,18 +340,18 @@
     def _init_ui(self) -> None:
         self.setText(self._dialog_text)
         self.setInformativeText(self._info_text)
         self.setStandardButtons(QMessageBox.Open | QMessageBox.Cancel)
         self.setDefaultButton(QMessageBox.Open)
         self.setWindowTitle(self._window_title)
         self.setIcon(QMessageBox.Information)
-        self.setWindowIcon(Assets.icon)
+        self.setWindowIcon(Assets.icon())
 
     @property
-    def update(self) -> bool:
+    def should_update(self) -> bool:
         """Indicate if BBSync should be updated."""
         return self.exec() == QMessageBox.Open
 
 
 class PersistenceWarning(QDialog):
     """QDialog shown if user chooses to store their login details on their device."""
 
@@ -376,14 +375,17 @@
     _log_out_signal = pyqtSignal()
     _setup_wiz_signal = pyqtSignal()
     _save_signal = pyqtSignal()
 
     def __init__(self):
         """Create instance of SettingsWindow."""
         super().__init__()
+        self.frequency_combo: QComboBox
+        self.current_session_label: QLabel
+        self.download_location_hint: QLabel
         self._init_ui()
 
     def _init_ui(self):
         Assets.load_ui(self)
 
         self.move(*self._initial_position)
         self.setWindowTitle(self._window_title)
@@ -465,14 +467,15 @@
 
     def __init__(self, start_url: str, target_url: str):
         """Create instance of LoginWebView."""
         super().__init__()
         self.start_url = start_url
         self.target_url = target_url
 
+        self.web_view : QWebEngineView
         self._init_ui()
         self._cookie_jar = RequestsCookieJar()
 
     def _init_ui(self) -> None:
         Assets.load_ui(self)
         self.web_view.load(QUrl.fromUserInput(self.start_url))
         self.web_view.loadFinished.connect(self._page_load_handler)
@@ -546,14 +549,17 @@
     def __init__(self, institutions: list[str]):
         """Create a `SetupWizard`.
 
         :param list[str] institutions: List of institution names
         """
         super().__init__()
 
+        self.uni_selection_box: QComboBox
+        self.since_all_checkbox: QCheckBox
+        self.date_spinbox: QSpinBox
         self.institutions = institutions
         self._init_ui()
         self._has_chosen_location = False
 
     def _init_ui(self):
         Assets.load_ui(self)
         self.uni_selection_box.addItems(self.institutions)
@@ -581,15 +587,16 @@
         self.sync_location_page.registerField(
             "syncLocation*",
             self.sync_location_button,
             property="text",
             changedSignal=self.sync_location_button.clicked
         )
 
-        self.intro_page.setPixmap(QWizard.WatermarkPixmap, Assets.watermark)
+        self.intro_page.setPixmap(QWizard.WatermarkPixmap,
+                                  Assets.watermark())
 
     def initializePage(self, id) -> None:
         if id == self.Pages.DOWNLOAD_LOCATION:
             if self._has_chosen_location:
                 self._set_location()
 
     def validateCurrentPage(self) -> bool:
@@ -637,14 +644,15 @@
         return Path(self.file_chooser.directory().path())
 
     @property
     def min_year(self) -> Optional[int]:
         """Courses from this year onward will be downloaded."""
         if not self.since_all_checkbox.isChecked():
             return self.date_spinbox.value()
+        return None
 
 
 class UniNotSupportedDialog(QDialog):
     """`QDialog` about unsupported Blackboard partners."""
 
     def __init__(self, help_url: str):
         """Create instance of dialog.
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/sync.py` & `blackboardsync-0.9.6a1/blackboard_sync/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import time
 import logging
 import threading
 from pathlib import Path
+from typing import Optional
 from datetime import datetime, timezone, timedelta
 
 from requests.cookies import RequestsCookieJar
 from requests.exceptions import ConnectionError
 
 from .config import SyncConfig
 from .download import BlackboardDownload
@@ -81,41 +82,48 @@
         download_logger = logging.getLogger("BlackboardDownload")
         download_logger.setLevel(logging.DEBUG)
         download_logger.addHandler(logging.StreamHandler())
 
         self.sess_logger = sess_logger
         self.download_logger = download_logger
 
-        self.university = None
+        self.university : Optional[Institution] = None
+        self.sess : Optional[BlackboardSession] = None
 
         # Attempt to load existing configuration
         self._config = SyncConfig()
         self.logger.info("Loading preexisting configuration")
 
         if self._config.university_index is not None:
             self.university = get_by_index(self._config.university_index)
 
         if self._config.last_sync_time is not None:
             self._update_next_sync()
 
     def setup(self, university_index: int, download_location: Path,
-              min_year: int = None):
+              min_year: Optional[int] = None) -> None:
         """Setup the university information."""
         self.university_index = university_index
         self._config.download_location = download_location
-        if min_year is not None:
-            self._config.min_year = min_year
+        self._config.min_year = min_year
+
+        # If min_year has decreased, redownload
+        if (self._config.min_year or 0) > (min_year or 0):
+            self.last_sync_time = None
 
     def auth(self, cookie_jar: RequestsCookieJar) -> bool:
         """Create a new Blackboard session with the given credentials.
 
         Will start syncing automatically if login successful.
 
         :param bool persistence: If true, login will be saved in the OS designated keyring.
         """
+        if self.university is None:
+            return False
+
         self._cookies = cookie_jar
 
         try:
             u_sess = BlackboardSession(self.university.api_url, cookie_jar)
         except ValueError:
             self.logger.warning("Credentials are incorrect")
         else:
@@ -142,19 +150,22 @@
 
         while self._is_active:
             if self.outdated or self._force_sync:
                 self.logger.debug("Syncing now")
                 self._is_syncing = True
 
                 # Download from last datetime
-                self._download = BlackboardDownload(self.sess,
-                                                    self.download_location / '',
-                                                    self.last_sync_time,
-                                                    self.university.data_sources,
-                                                    self.min_year)
+                user_session = self.sess
+
+                if user_session is not None and self.university is not None:
+                    self._download = BlackboardDownload(user_session,
+                                                        self.download_location / '',
+                                                        self.last_sync_time,
+                                                        self.university.data_sources,
+                                                        self.min_year)
 
                 try:
                     if not self._is_active:
                         self._download.cancel()
                     job_start_time = self._download.download()
                     if job_start_time is not None:
                         self.last_sync_time = job_start_time
@@ -207,33 +218,33 @@
 
     def force_sync(self) -> None:
         """Force Sync thread to start download job ASAP."""
         self.logger.debug("Forced syncing")
         self._force_sync = True
 
     @property
-    def username(self) -> str:
-        return self.sess.username
+    def username(self) -> Optional[str]:
+        return self.sess.username if self.sess is not None else None
 
     @property
     def _log_path(self) -> Path:
         filename = f"sync_error_{datetime.now():%Y-%m-%dT%H_%M_%S_%f}.log"
         return Path(self._log_dir / filename)
 
     @property
     def _log_dir(self) -> Path:
         return Path(self.download_location / self._log_directory)
 
     @property
-    def last_sync_time(self) -> datetime:
+    def last_sync_time(self) -> Optional[datetime]:
         """Datetime right before last download job started."""
         return self._config.last_sync_time
 
     @last_sync_time.setter
-    def last_sync_time(self, last_time: datetime):
+    def last_sync_time(self, last_time: Optional[datetime]):
         """Updates the last sync time recorded."""
         self._config.last_sync_time = last_time
         self._update_next_sync()
 
     def _update_next_sync(self) -> None:
         """Store a calculated datetime when next sync should take place."""
         self._next_sync = (self._config.last_sync_time +
@@ -248,15 +259,15 @@
     def outdated(self) -> bool:
         """Return true if last download job is outdated."""
         if self._config.last_sync_time is None:
             return True
         return datetime.now(timezone.utc) >= self.next_sync
 
     @property
-    def min_year(self):
+    def min_year(self) -> int:
         return self._config.min_year
 
     @property
     def university_index(self):
         return self._config.university_index
 
     @university_index.setter
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.6a1/blackboard_sync/sync_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import sys
 import webbrowser
+from typing import Optional
 
 from PyQt5.QtGui import QWindow
 from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QApplication, QStyleFactory, QSystemTrayIcon
+from PyQt5.QtWidgets import QApplication, QStyleFactory, QSystemTrayIcon, QWidget
 
 from .sync import BlackboardSync
 from .institutions import Institution, get_names, InstitutionLogin
 from .__about__ import __title__, __version__
 from .updates import check_for_updates
 from .qt.qt_elements import (LoginWebView, SyncTrayIcon, SettingsWindow,
                              RedownloadDialog, OSUtils, SetupWizard, UpdateFoundDialog)
@@ -58,15 +59,15 @@
             self._show_login_window()
         self.app.exec()
 
     def _init_ui(self) -> None:
         self.setup_window = SetupWizard(get_names())
         self.setup_window.accepted.connect(self._setup_complete)
 
-        self.login_window = None
+        self.login_window : Optional[LoginWebView] = None
 
         self.config_window = SettingsWindow()
 
         self.config_window.log_out_signal.connect(self._log_out)
         self.config_window.setup_wiz_signal.connect(self._reset_setup)
         self.config_window.save_signal.connect(self._save_setting_changes)
 
@@ -93,14 +94,17 @@
     def _build_login_window(self, uni_login_info: InstitutionLogin) -> None:
         # Get login url from uni DB
         self.login_window = LoginWebView(start_url=uni_login_info.start_url,
                                          target_url=uni_login_info.target_url)
         self.login_window.login_complete_signal.connect(self._login_complete)
 
     def _login_complete(self) -> None:
+        if self.login_window is None:
+            return
+
         self.app.setOverrideCursor(Qt.WaitCursor)
         # Call login function on sync
         auth = self.model.auth(self.login_window.cookie_jar)
         self.tray.set_logged_in(auth)
         self.login_window.setVisible(False)
         self.app.restoreOverrideCursor()
         self._check_for_updates()
@@ -111,15 +115,15 @@
         if self.login_window is not None:
             self._log_out()
             self.login_window.setVisible(False)
         self._show_setup_window()
 
     def _check_for_updates(self) -> None:
         if (html_url := check_for_updates()) is not None:
-            if UpdateFoundDialog().update:
+            if UpdateFoundDialog().should_update:
                 webbrowser.open(html_url)
 
     def _show_login_window(self) -> None:
         if self.login_window is not None:
             self._show_window(self.login_window)
 
     def _show_setup_window(self) -> None:
@@ -128,15 +132,15 @@
     def _show_config_window(self) -> None:
         # Update displayed settings
         self.config_window.download_location = self.model.download_location
         self.config_window.username = self.model.username.split(':')[1]
         self.config_window.sync_frequency = self.model.sync_interval
         self._show_window(self.config_window)
 
-    def _show_window(self, window: QWindow) -> None:
+    def _show_window(self, window: QWidget) -> None:
         window.setWindowState(Qt.WindowNoState)
         window.show()
         window.setFocus()
 
     def _open_download_dir(self) -> None:
         # Open folder in browser
         OSUtils.open_dir_in_file_browser(self.model.download_location)
@@ -151,16 +155,19 @@
 
     def _log_out(self) -> None:
         if self.model.is_active:
             self.model.stop_sync()
 
         self.model.log_out()
         self.tray.set_logged_in(False)
-        self.login_window.restore()
-        self.login_window.setVisible(True)
+        
+        if self.login_window is not None:
+            self.login_window.restore()
+            self.login_window.setVisible(True)
+
         self.config_window.setVisible(False)
 
     def _save_setting_changes(self) -> None:
         self.config_window.setVisible(False)
 
         if self.model.download_location != self.config_window.download_location:
             redownload = RedownloadDialog().redownload
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/universities.json` & `blackboardsync-0.9.6a1/blackboard_sync/universities.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666666%*

 * *Differences: {'0': "{'data_sources': []}"}*

```diff
@@ -1,13 +1,11 @@
 [
     {
         "api_url": "https://portal.uclan.ac.uk/",
-        "data_sources": [
-            "_21_1"
-        ],
+        "data_sources": [],
         "login": {
             "start_url": "https://portal.uclan.ac.uk",
             "target_url": "https://portal.uclan.ac.uk/ultra/"
         },
         "name": "University of Central Lancashire",
         "network": {
             "isp": [],
```

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/updates.py` & `blackboardsync-0.9.6a1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/blackboard_sync/webdav.py` & `blackboardsync-0.9.6a1/blackboard_sync/webdav.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     def links(self) -> List[Link]:
         return self._links
 
     @property
     def body(self) -> str:
         return str(self.soup)
 
-def validate_webdav_response(response, link: Link, base_url: str):
+def validate_webdav_response(response, link: str, base_url: str):
     if response.status_code == 200:
         h = response.headers
-        content_type = h.get('Content-Type')
+        content_type = h.get('Content-Type', '')
         content_len = int(h.get('Content-Length', 0))
 
         # TODO: feature: select mime types
         len_limit = 1024 * 1024 * 20 # 20 MB
         return link.startswith(base_url) and 'video' not in content_type and content_len < len_limit
     return False
```

### Comparing `blackboardsync-0.9.5a1/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.6a1/blackboardsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.5a1
+Version: 0.9.6a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -121,15 +121,14 @@
 ```
 
 
 
 To start the program
 
 ```bash
-cd blackboard_sync
 pipenv run python -m blackboard_sync
 ```
```

### Comparing `blackboardsync-0.9.5a1/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.6a1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/docs/Makefile` & `blackboardsync-0.9.6a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/docs/conf.py` & `blackboardsync-0.9.6a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/docs/index.rst` & `blackboardsync-0.9.6a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/docs/make.bat` & `blackboardsync-0.9.6a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/main.py` & `blackboardsync-0.9.6a1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/packaging/pkg_macos.sh` & `blackboardsync-0.9.6a1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/packaging/pkg_win.nsi` & `blackboardsync-0.9.6a1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/packaging/pyinst.py` & `blackboardsync-0.9.6a1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/pyproject.toml` & `blackboardsync-0.9.6a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/tests/strategies.py` & `blackboardsync-0.9.6a1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/tests/test_api.py` & `blackboardsync-0.9.6a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/tests/test_blackboard.py` & `blackboardsync-0.9.6a1/tests/test_blackboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     )
     def test_content_sanitise_title(self, title, sanitised):
         obj = BBCourseContent(title=title)
         assert obj.title_path_safe == sanitised
 
     @given(st.text())
     def test_content_sanitise_title_hypothesis(self, filename):
-        safe_path = sanitize_filename(filename, replacement_text='_')
+        safe_path = sanitize_filename(filename or 'Title missing', replacement_text='_')
         obj = BBCourseContent(title=filename)
-        assert safe_path == obj.title_path_safe
+        assert safe_path or '' == obj.title_path_safe
```

### Comparing `blackboardsync-0.9.5a1/tests/test_download.py` & `blackboardsync-0.9.6a1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/tests/test_qt.py` & `blackboardsync-0.9.6a1/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5a1/tests/test_sync_config.py` & `blackboardsync-0.9.6a1/tests/test_sync_config.py`

 * *Files identical despite different names*

