# Comparing `tmp/pmxbot-1122.9.2.tar.gz` & `tmp/pmxbot-1122.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpi_v8om34/tmpnrt5bykx/pmxbot-1122.9.2.tar", last modified: Sun Feb  9 14:38:47 2020, max compression
+gzip compressed data, was "/tmp/tmpprc0l3i9/tmp7_r3uyqi/pmxbot-1122.9.3.tar", last modified: Wed Sep 23 08:33:56 2020, max compression
```

## Comparing `pmxbot-1122.9.2.tar` & `pmxbot-1122.9.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.832824 pmxbot-1122.9.2/
--rw-r--r--   0 vsts      (1001) docker     (115)       50 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/.coveragerc
--rw-r--r--   0 vsts      (1001) docker     (115)      246 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/.flake8
--rw-r--r--   0 vsts      (1001) docker     (115)       95 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (115)      176 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/.pre-commit-config.yaml
--rw-r--r--   0 vsts      (1001) docker     (115)       74 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (115)      312 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/.travis.yml
--rw-r--r--   0 vsts      (1001) docker     (115)    17447 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/CHANGES.rst
--rw-r--r--   0 vsts      (1001) docker     (115)     1047 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (115)    10048 2020-02-09 14:38:47.832824 pmxbot-1122.9.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (115)     7530 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/README.rst
--rw-r--r--   0 vsts      (1001) docker     (115)      468 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/appveyor.yml
--rw-r--r--   0 vsts      (1001) docker     (115)     1441 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/azure-pipelines.yml
--rw-r--r--   0 vsts      (1001) docker     (115)     1145 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/config.yaml
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.820824 pmxbot-1122.9.2/docs/
--rw-r--r--   0 vsts      (1001) docker     (115)      755 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (115)       81 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/docs/history.rst
--rw-r--r--   0 vsts      (1001) docker     (115)      296 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (115)    27714 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/horrible-logos-pmxbot.gif
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.824823 pmxbot-1122.9.2/pmxbot/
--rw-r--r--   0 vsts      (1001) docker     (115)       56 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)       69 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3564 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/asciilogo.txt
--rw-r--r--   0 vsts      (1001) docker     (115)    26924 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/commands.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1035 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/config_.py
--rw-r--r--   0 vsts      (1001) docker     (115)    17873 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/core.py
--rw-r--r--   0 vsts      (1001) docker     (115)      348 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/dictlib.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2307 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/example usage.txt
--rw-r--r--   0 vsts      (1001) docker     (115)     7128 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/irc.py
--rw-r--r--   0 vsts      (1001) docker     (115)      704 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/itertools.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10929 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/karma.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3264 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/klingonisms.txt
--rw-r--r--   0 vsts      (1001) docker     (115)    17407 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/logging.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1876 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/murphy's laws.txt
--rw-r--r--   0 vsts      (1001) docker     (115)     2890 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/notify.py
--rw-r--r--   0 vsts      (1001) docker     (115)    14289 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/phrases.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7008 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/quotes.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2825 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/rolls.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3671 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/slack.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1609 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/social strategies.txt
--rw-r--r--   0 vsts      (1001) docker     (115)    13226 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/stack.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3067 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/storage.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1701 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/system.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/pmxbot/testing/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)      311 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/testing/fixtures.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4685 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/pmxbot/web/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)       81 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/pmxbot/web/templates/
--rw-r--r--   0 vsts      (1001) docker     (115)    27170 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/Autolinker.js
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2673 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (115)      425 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/channel.html
--rw-r--r--   0 vsts      (1001) docker     (115)      611 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/day.html
--rw-r--r--   0 vsts      (1001) docker     (115)      602 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/help.html
--rw-r--r--   0 vsts      (1001) docker     (115)      409 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/index.html
--rw-r--r--   0 vsts      (1001) docker     (115)      921 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/karma.html
--rw-r--r--   0 vsts      (1001) docker     (115)    76606 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/pmxbot.png
--rw-r--r--   0 vsts      (1001) docker     (115)      526 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/templates/search.html
--rw-r--r--   0 vsts      (1001) docker     (115)    11243 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pmxbot/web/viewer.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/pmxbot.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (115)    10048 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (115)     2134 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (115)        1 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (115)      539 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (115)        7 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/namespace_packages.txt
--rw-r--r--   0 vsts      (1001) docker     (115)      648 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (115)       13 2020-02-09 14:38:47.000000 pmxbot-1122.9.2/pmxbot.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (115)      195 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (115)      526 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (115)        2 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/routines/
--rw-r--r--   0 vsts      (1001) docker     (115)      335 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/routines/dedup-karma.py
--rw-r--r--   0 vsts      (1001) docker     (115)      361 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/routines/migrate-all.py
--rw-r--r--   0 vsts      (1001) docker     (115)      391 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/routines/rebuild-recent.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2182 2020-02-09 14:38:47.832824 pmxbot-1122.9.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (115)       92 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/setup.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8960 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/skeleton.md
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/tests/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)      617 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/tests/functional/
--rw-r--r--   0 vsts      (1001) docker     (115)     4911 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.828824 pmxbot-1122.9.2/tests/functional/plugins/
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.832824 pmxbot-1122.9.2/tests/functional/plugins/pmxbot_test_commands.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (115)       73 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/plugins/pmxbot_test_commands.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (115)      572 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/plugins/pmxbot_test_commands.py
--rw-r--r--   0 vsts      (1001) docker     (115)      755 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4130 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/test_logging.py
--rw-r--r--   0 vsts      (1001) docker     (115)      487 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/test_messages.py
--rw-r--r--   0 vsts      (1001) docker     (115)      455 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/functional/test_regexps.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:47.832824 pmxbot-1122.9.2/tests/unit/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)    18397 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_commands.py
--rw-r--r--   0 vsts      (1001) docker     (115)      349 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_config_mod.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2602 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_core.py
--rw-r--r--   0 vsts      (1001) docker     (115)      592 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_handlers.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3034 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_karma.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2248 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_logging.py
--rw-r--r--   0 vsts      (1001) docker     (115)      680 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_quotes.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13632 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_stack.py
--rw-r--r--   0 vsts      (1001) docker     (115)      348 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (115)      225 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/test_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (115)      611 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tests/unit/testconf.yaml
--rw-r--r--   0 vsts      (1001) docker     (115)      812 2020-02-09 14:38:23.000000 pmxbot-1122.9.2/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.165295 pmxbot-1122.9.3/
+-rw-r--r--   0 vsts      (1001) docker     (116)       50 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/.coveragerc
+-rw-r--r--   0 vsts      (1001) docker     (116)      246 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/.flake8
+-rw-r--r--   0 vsts      (1001) docker     (116)       95 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (116)      176 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 vsts      (1001) docker     (116)       74 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (116)      312 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/.travis.yml
+-rw-r--r--   0 vsts      (1001) docker     (116)    17447 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/CHANGES.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)     1047 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (116)    10048 2020-09-23 08:33:56.165295 pmxbot-1122.9.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)     7530 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)      468 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/appveyor.yml
+-rw-r--r--   0 vsts      (1001) docker     (116)     1441 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/azure-pipelines.yml
+-rw-r--r--   0 vsts      (1001) docker     (116)     1145 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/config.yaml
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.157294 pmxbot-1122.9.3/docs/
+-rw-r--r--   0 vsts      (1001) docker     (116)      755 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (116)       81 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/docs/history.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)      296 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (116)    27714 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/horrible-logos-pmxbot.gif
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/pmxbot/
+-rw-r--r--   0 vsts      (1001) docker     (116)       56 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)       69 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3564 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/asciilogo.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)    26924 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1035 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/config_.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    17873 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/core.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      348 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/dictlib.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2307 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/example usage.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)     7128 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/irc.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      704 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/itertools.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    10929 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/karma.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3264 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/klingonisms.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)    17407 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1876 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/murphy's laws.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)     2890 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/notify.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    14289 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/phrases.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7008 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/quotes.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2825 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/rolls.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5081 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/slack.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1609 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/social strategies.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)    13226 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/stack.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3067 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/storage.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1701 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/system.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/pmxbot/testing/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      311 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/testing/fixtures.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4685 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/pmxbot/web/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)       81 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/pmxbot/web/templates/
+-rw-r--r--   0 vsts      (1001) docker     (116)    27170 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/Autolinker.js
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2673 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (116)      425 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/channel.html
+-rw-r--r--   0 vsts      (1001) docker     (116)      611 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/day.html
+-rw-r--r--   0 vsts      (1001) docker     (116)      602 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/help.html
+-rw-r--r--   0 vsts      (1001) docker     (116)      409 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/index.html
+-rw-r--r--   0 vsts      (1001) docker     (116)      921 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/karma.html
+-rw-r--r--   0 vsts      (1001) docker     (116)    76606 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/pmxbot.png
+-rw-r--r--   0 vsts      (1001) docker     (116)      526 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/templates/search.html
+-rw-r--r--   0 vsts      (1001) docker     (116)    11243 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pmxbot/web/viewer.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/pmxbot.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)    10048 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)     2134 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      539 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        7 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/namespace_packages.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      648 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       13 2020-09-23 08:33:55.000000 pmxbot-1122.9.3/pmxbot.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      195 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (116)      526 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (116)        2 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/routines/
+-rw-r--r--   0 vsts      (1001) docker     (116)      335 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/routines/dedup-karma.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      361 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/routines/migrate-all.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      391 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/routines/rebuild-recent.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2182 2020-09-23 08:33:56.165295 pmxbot-1122.9.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)       92 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8960 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/skeleton.md
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/tests/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      617 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/tests/functional/
+-rw-r--r--   0 vsts      (1001) docker     (116)     4911 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/tests/functional/plugins/
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.161294 pmxbot-1122.9.3/tests/functional/plugins/pmxbot_test_commands.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)       73 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/plugins/pmxbot_test_commands.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      572 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/plugins/pmxbot_test_commands.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      755 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4130 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/test_logging.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      487 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/test_messages.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      455 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/functional/test_regexps.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:56.165295 pmxbot-1122.9.3/tests/unit/
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    18418 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_commands.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      349 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_config_mod.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2602 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_core.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      592 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_handlers.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3034 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_karma.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2248 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_logging.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      680 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_quotes.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13632 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      348 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      225 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/test_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      611 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tests/unit/testconf.yaml
+-rw-r--r--   0 vsts      (1001) docker     (116)      812 2020-09-23 08:33:30.000000 pmxbot-1122.9.3/tox.ini
```

### Comparing `pmxbot-1122.9.2/CHANGES.rst` & `pmxbot-1122.9.3/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/LICENSE` & `pmxbot-1122.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/PKG-INFO` & `pmxbot-1122.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmxbot
-Version: 1122.9.2
+Version: 1122.9.3
 Summary: IRC bot - full featured, yet extensible and customizable
 Home-page: https://github.com/pmxbot/pmxbot
 Author: YouGov, Plc.
 Author-email: dev@yougov.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 License: UNKNOWN
```

### Comparing `pmxbot-1122.9.2/README.rst` & `pmxbot-1122.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/azure-pipelines.yml` & `pmxbot-1122.9.3/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/config.yaml` & `pmxbot-1122.9.3/config.yaml`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/docs/conf.py` & `pmxbot-1122.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/horrible-logos-pmxbot.gif` & `pmxbot-1122.9.3/horrible-logos-pmxbot.gif`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/asciilogo.txt` & `pmxbot-1122.9.3/pmxbot/asciilogo.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/commands.py` & `pmxbot-1122.9.3/pmxbot/commands.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/config_.py` & `pmxbot-1122.9.3/pmxbot/config_.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/core.py` & `pmxbot-1122.9.3/pmxbot/core.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/example usage.txt` & `pmxbot-1122.9.3/pmxbot/example usage.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/irc.py` & `pmxbot-1122.9.3/pmxbot/irc.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/itertools.py` & `pmxbot-1122.9.3/pmxbot/itertools.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/karma.py` & `pmxbot-1122.9.3/pmxbot/karma.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/klingonisms.txt` & `pmxbot-1122.9.3/pmxbot/klingonisms.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/logging.py` & `pmxbot-1122.9.3/pmxbot/logging.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/murphy's laws.txt` & `pmxbot-1122.9.3/pmxbot/murphy's laws.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/notify.py` & `pmxbot-1122.9.3/pmxbot/notify.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/phrases.py` & `pmxbot-1122.9.3/pmxbot/phrases.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/quotes.py` & `pmxbot-1122.9.3/pmxbot/quotes.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/rolls.py` & `pmxbot-1122.9.3/pmxbot/rolls.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/social strategies.txt` & `pmxbot-1122.9.3/pmxbot/social strategies.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/stack.py` & `pmxbot-1122.9.3/pmxbot/stack.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/storage.py` & `pmxbot-1122.9.3/pmxbot/storage.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/system.py` & `pmxbot-1122.9.3/pmxbot/system.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/util.py` & `pmxbot-1122.9.3/pmxbot/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,17 +101,17 @@
     """
     https://github.com/wordnik/wordnik-python3/issues/1
     """
     wordnik.swagger.MethodRequest = backports.method_request.Request
 
 
 def lookup(word):
-    '''
+    """
     Get a definition for a word (uses Wordnik)
-    '''
+    """
     _patch_wordnik()
     # Jason's key - do not abuse
     key = 'edc4b9b94b341eeae350e087c2e05d2f5a2a9e0478cefc6dc'
     client = wordnik.swagger.ApiClient(key, 'http://api.wordnik.com/v4')
     words = wordnik.WordApi.WordApi(client)
     try:
         definitions = words.getDefinitions(word, limit=1)
@@ -121,18 +121,18 @@
     return str(definition.text)
 
 
 lookup.provider = 'Wordnik'
 
 
 def urban_lookup(word):
-    '''
+    """
     Return a Urban Dictionary definition for a word or None if no result was
     found.
-    '''
+    """
     url = "http://api.urbandictionary.com/v0/define"
     params = dict(term=word)
     resp = requests.get(url, params=params)
     resp.raise_for_status()
     res = resp.json()
     if not res['list']:
         return
```

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/Autolinker.js` & `pmxbot-1122.9.3/pmxbot/web/templates/Autolinker.js`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/base.html` & `pmxbot-1122.9.3/pmxbot/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/day.html` & `pmxbot-1122.9.3/pmxbot/web/templates/day.html`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/help.html` & `pmxbot-1122.9.3/pmxbot/web/templates/help.html`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/karma.html` & `pmxbot-1122.9.3/pmxbot/web/templates/karma.html`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/pmxbot.png` & `pmxbot-1122.9.3/pmxbot/web/templates/pmxbot.png`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/templates/search.html` & `pmxbot-1122.9.3/pmxbot/web/templates/search.html`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot/web/viewer.py` & `pmxbot-1122.9.3/pmxbot/web/viewer.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot.egg-info/PKG-INFO` & `pmxbot-1122.9.3/pmxbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmxbot
-Version: 1122.9.2
+Version: 1122.9.3
 Summary: IRC bot - full featured, yet extensible and customizable
 Home-page: https://github.com/pmxbot/pmxbot
 Author: YouGov, Plc.
 Author-email: dev@yougov.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 License: UNKNOWN
```

### Comparing `pmxbot-1122.9.2/pmxbot.egg-info/SOURCES.txt` & `pmxbot-1122.9.3/pmxbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot.egg-info/entry_points.txt` & `pmxbot-1122.9.3/pmxbot.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pmxbot.egg-info/requires.txt` & `pmxbot-1122.9.3/pmxbot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/pytest.ini` & `pmxbot-1122.9.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/setup.cfg` & `pmxbot-1122.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/skeleton.md` & `pmxbot-1122.9.3/skeleton.md`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/conftest.py` & `pmxbot-1122.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/functional/__init__.py` & `pmxbot-1122.9.3/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/functional/plugins/pmxbot_test_commands.py` & `pmxbot-1122.9.3/tests/functional/plugins/pmxbot_test_commands.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/functional/test_exceptions.py` & `pmxbot-1122.9.3/tests/functional/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/functional/test_logging.py` & `pmxbot-1122.9.3/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/test_commands.py` & `pmxbot-1122.9.3/tests/unit/test_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         assert res == "Wordnik does not have a definition for that."
 
     def test_urb_irc(self, needs_internet):
         """
         Test the urban dictionary with the word IRC.
         """
         res = commands.urbandict("irc")
-        assert "Internet Relay Chat" in res
+        assert "It's a place where broken and odd people" in res
 
     def test_acronym_irc(self, needs_internet):
         """
         Test acronym finder with the word IRC.
         """
         res = commands.acit("irc")
         assert "|" in res
```

### Comparing `pmxbot-1122.9.2/tests/unit/test_core.py` & `pmxbot-1122.9.3/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/test_handlers.py` & `pmxbot-1122.9.3/tests/unit/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/test_karma.py` & `pmxbot-1122.9.3/tests/unit/test_karma.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/test_logging.py` & `pmxbot-1122.9.3/tests/unit/test_logging.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/test_quotes.py` & `pmxbot-1122.9.3/tests/unit/test_quotes.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/test_stack.py` & `pmxbot-1122.9.3/tests/unit/test_stack.py`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tests/unit/testconf.yaml` & `pmxbot-1122.9.3/tests/unit/testconf.yaml`

 * *Files identical despite different names*

### Comparing `pmxbot-1122.9.2/tox.ini` & `pmxbot-1122.9.3/tox.ini`

 * *Files identical despite different names*

