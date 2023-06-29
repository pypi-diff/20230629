# Comparing `tmp/embykeeper-2.2.6.tar.gz` & `tmp/embykeeper-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.6.tar", last modified: Wed Jun 28 08:03:19 2023, max compression
+gzip compressed data, was "embykeeper-2.2.7.tar", last modified: Thu Jun 29 12:10:41 2023, max compression
```

## Comparing `embykeeper-2.2.6.tar` & `embykeeper-2.2.7.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.138308 embykeeper-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-28 08:03:09.000000 embykeeper-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-28 08:03:09.000000 embykeeper-2.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-06-28 08:03:19.138308 embykeeper-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-06-28 08:03:09.000000 embykeeper-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.122308 embykeeper-2.2.6/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.126308 embykeeper-2.2.6/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.126308 embykeeper-2.2.6/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.130308 embykeeper-2.2.6/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.130308 embykeeper-2.2.6/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.126308 embykeeper-2.2.6/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-06-28 08:03:19.000000 embykeeper-2.2.6/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-28 08:03:19.000000 embykeeper-2.2.6/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 08:03:19.000000 embykeeper-2.2.6/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-28 08:03:19.000000 embykeeper-2.2.6/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 08:03:18.000000 embykeeper-2.2.6/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-28 08:03:19.000000 embykeeper-2.2.6/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-28 08:03:19.000000 embykeeper-2.2.6/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.122308 embykeeper-2.2.6/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.118308 embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.118308 embykeeper-2.2.6/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-28 08:03:09.000000 embykeeper-2.2.6/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-28 08:03:09.000000 embykeeper-2.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 08:03:19.138308 embykeeper-2.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:03:19.134308 embykeeper-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-28 08:03:09.000000 embykeeper-2.2.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 12:10:31.000000 embykeeper-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 12:10:31.000000 embykeeper-2.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23854 2023-06-29 12:10:41.581615 embykeeper-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22905 2023-06-29 12:10:31.000000 embykeeper-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/bots/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.577615 embykeeper-2.2.7/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23854 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 12:10:41.000000 embykeeper-2.2.7/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.573615 embykeeper-2.2.7/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-29 12:10:31.000000 embykeeper-2.2.7/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-29 12:10:31.000000 embykeeper-2.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:10:41.581615 embykeeper-2.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:10:41.581615 embykeeper-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-29 12:10:31.000000 embykeeper-2.2.7/tests/test_cli.py
```

### Comparing `embykeeper-2.2.6/LICENSE` & `embykeeper-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/PKG-INFO` & `embykeeper-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.6
+Version: 2.2.7
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -87,15 +87,15 @@
 
 ### 在线部署
 
 #### Railway
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
 #### Render.com
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.6 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.7 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -89,15 +89,15 @@
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
 å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
-(https://railway.app/button.svg)](https://railway.app/template/
+(https://railway.app/button.svg)](https://railway.app/new/template/
 WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
 embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
 06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
 5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
 é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
```

### Comparing `embykeeper-2.2.6/README.md` & `embykeeper-2.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 ### 在线部署
 
 #### Railway
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
 #### Render.com
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
```

#### html2text {}

```diff
@@ -77,15 +77,15 @@
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
 å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
-(https://railway.app/button.svg)](https://railway.app/template/
+(https://railway.app/button.svg)](https://railway.app/new/template/
 WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
 embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
 06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
 5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
 é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
```

### Comparing `embykeeper-2.2.6/embykeeper/cli.py` & `embykeeper-2.2.7/embykeeper/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,16 +56,20 @@
     monitor: bool = typer.Option(False, "--monitor", "-m", rich_help_panel="模块开关", help="启用群聊监视"),
     send: bool = typer.Option(False, "--send", "-s", rich_help_panel="模块开关", help="启用自动水群"),
     instant: bool = typer.Option(
         True, "--instant/--no-instant", "-i/-I", rich_help_panel="调试参数", help="立刻执行一次任务"
     ),
     once: bool = typer.Option(False, "--once/--cron", "-o/-O", rich_help_panel="调试参数", help="仅执行一次任务而不计划执行"),
     public: bool = typer.Option(False, rich_help_panel="调试参数", help="启用公共仓库部署模式"),
-    debug: bool = typer.Option(False, "--debug", "-d", rich_help_panel="调试参数", help="开启调试模式"),
-    debug_cron: bool = typer.Option(False, hidden=True, help="开启任务调试模式, 在三秒后立刻开始执行计划任务"),
+    debug: bool = typer.Option(
+        False, "--debug", "-d", envvar="EK_DEBUG", show_envvar=False, rich_help_panel="调试参数", help="开启调试模式"
+    ),
+    debug_cron: bool = typer.Option(
+        False, hidden=True, envvar="EK_DEBUG_CRON", show_envvar=False, help="开启任务调试模式, 在三秒后立刻开始执行计划任务"
+    ),
     version: bool = typer.Option(
         None,
         "--version",
         "-v",
         rich_help_panel="调试参数",
         callback=version,
         is_eager=True,
```

### Comparing `embykeeper-2.2.6/embykeeper/data.py` & `embykeeper-2.2.7/embykeeper/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,60 +28,64 @@
     if not_existing:
         logger.info(f"这是您首次使用{caller or '该功能'}, 将下载所需文件: {', '.join(not_existing)}")
 
     for name in to_iterable(names):
         if name in existing:
             yield existing[name]
         else:
-            url = f"https://raw.githubusercontent.com/embykeeper/embykeeper-data/main/data/{name}"
-            for retries in range(3):
-                if proxy:
-                    connector = ProxyConnector(
-                        proxy_type=ProxyType[proxy["scheme"].upper()],
-                        host=proxy["hostname"],
-                        port=proxy["port"],
-                    )
+            try:
+                url = f"https://raw.githubusercontent.com/embykeeper/embykeeper-data/main/data/{name}"
+                for retries in range(3):
+                    if proxy:
+                        connector = ProxyConnector(
+                            proxy_type=ProxyType[proxy["scheme"].upper()],
+                            host=proxy["hostname"],
+                            port=proxy["port"],
+                        )
+                    else:
+                        connector = aiohttp.TCPConnector()
+                    async with aiohttp.ClientSession(connector=connector) as session:
+                        try:
+                            async with session.get(url) as resp:
+                                if resp.status == 200:
+                                    file_size = int(resp.headers.get("Content-Length", 0))
+                                    logger.info(f"开始下载: {name} ({humanbytes(file_size)})")
+                                    async with aiofiles.open(basedir / name, mode="wb+") as f:
+                                        timer = time.time()
+                                        length = 0
+                                        async for chunk in resp.content.iter_chunked(512):
+                                            if time.time() - timer > 3:
+                                                timer = time.time()
+                                                logger.info(
+                                                    f"正在下载: {name} ({humanbytes(length)} / {humanbytes(file_size)})"
+                                                )
+                                            await f.write(chunk)
+                                            length += len(chunk)
+                                    logger.info(f"下载完成: {name} ({humanbytes(file_size)})")
+                                    yield basedir / name
+                                    break
+                                else:
+                                    logger.warning(f"下载失败: {name} ({resp.status})")
+                                    yield None
+                                    break
+                        except aiohttp.ClientConnectorError as e:
+                            (basedir / name).unlink(missing_ok=True)
+                            logger.warning(f"下载失败: {name}, 将在 3 秒后重试.")
+                            await asyncio.sleep(3)
+                            continue
+                        except Exception as e:
+                            (basedir / name).unlink(missing_ok=True)
+                            logger.warning(f"下载失败: {name} ({e})")
+                            yield None
+                            break
                 else:
-                    connector = aiohttp.TCPConnector()
-                async with aiohttp.ClientSession(connector=connector) as session:
-                    try:
-                        async with session.get(url) as resp:
-                            if resp.status == 200:
-                                file_size = int(resp.headers.get("Content-Length", 0))
-                                logger.info(f"开始下载: {name} ({humanbytes(file_size)})")
-                                async with aiofiles.open(basedir / name, mode="wb+") as f:
-                                    timer = time.time()
-                                    length = 0
-                                    async for chunk in resp.content.iter_chunked(512):
-                                        if time.time() - timer > 3:
-                                            timer = time.time()
-                                            logger.info(
-                                                f"正在下载: {name} ({humanbytes(length)} / {humanbytes(file_size)})"
-                                            )
-                                        await f.write(chunk)
-                                        length += len(chunk)
-                                logger.info(f"下载完成: {name} ({humanbytes(file_size)})")
-                                yield basedir / name
-                                break
-                            else:
-                                logger.warning(f"下载失败: {name} ({resp.status})")
-                                yield None
-                                break
-                    except aiohttp.ClientConnectorError as e:
-                        (basedir / name).unlink(missing_ok=True)
-                        logger.warning(f"下载失败: {name}, 将在 3 秒后重试.")
-                        await asyncio.sleep(3)
-                        continue
-                    except Exception as e:
-                        (basedir / name).unlink(missing_ok=True)
-                        logger.warning(f"下载失败: {name} ({e})")
-                        yield None
-                        break
-            else:
-                logger.warning(f"下载失败: {name}.")
-                yield None
-                continue
+                    logger.warning(f"下载失败: {name}.")
+                    yield None
+                    continue
+            except KeyboardInterrupt:
+                (basedir / name).unlink(missing_ok=True)
+                raise
 
 
 async def get_data(basedir: Path, name: str, proxy: dict = None, caller: str = None):
     async for data in get_datas(basedir, name, proxy, caller):
         return data
```

### Comparing `embykeeper-2.2.6/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.7/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/embywatcher/main.py` & `embykeeper-2.2.7/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/log.py` & `embykeeper-2.2.7/embykeeper/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from logging import Formatter
+import asyncio
+
 from loguru import logger
 from rich.logging import Console, RichHandler
-import asyncio
 
 from .utils import to_iterable
 
 
 def formatter(record):
     extra = record["extra"]
     scheme = extra.get("scheme", None)
@@ -40,11 +41,14 @@
     else:
         return "{message}"
 
 
 def initialize(level="INFO"):
     logger.remove()
     handler = RichHandler(
-        console=Console(stderr=True), markup=True, rich_tracebacks=True, tracebacks_suppress=[asyncio]
+        console=Console(stderr=True),
+        markup=True,
+        rich_tracebacks=True,
+        tracebacks_suppress=[asyncio],
     )
     handler.setFormatter(Formatter(None, "[%m/%d %H:%M]"))
     logger.add(handler, format=formatter, level=level, colorize=False)
```

### Comparing `embykeeper-2.2.6/embykeeper/settings.py` & `embykeeper-2.2.7/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 from loguru import logger
 from PIL import Image
 from pyrogram import filters
 from pyrogram.errors import UsernameNotOccupied, FloodWait
 from pyrogram.handlers import EditedMessageHandler, MessageHandler
 from pyrogram.types import InlineKeyboardMarkup, Message, ReplyKeyboardMarkup
 from thefuzz import fuzz
+from aiocache import cached
 
 from ...data import get_datas
 from ...utils import to_iterable, AsyncCountPool
 from ..tele import Client
 
 __ignore__ = True
 
-default_ocr = DdddOcr(beta=True, show_ad=False)
-
 
 class MessageType(Flag):
     TEXT = auto()
     CAPTION = auto()
     CAPTCHA = auto()
     ANSWER = auto()
 
@@ -63,16 +62,15 @@
         pass
 
 
 class BotCheckin(BaseBotCheckin):
     """签到类, 用于回复模式签到."""
 
     group_pool = AsyncCountPool(base=2000)
-    ocr = default_ocr
-    lock = asyncio.Lock()
+    ocr = None
 
     name: str = None  # 签到器的名称
     bot_id: int = None  # Bot 的 UserID
     bot_username: str = None  # Bot 的 用户名
     bot_checkin_cmd: Union[str, List[str]] = ["/checkin"]  # Bot 依次执行的签到命令
     bot_send_interval: int = 1  # 签到命令间等待的秒数
     bot_checkin_caption_pat: str = None  # 当 Bot 返回图片时, 仅当符合该 regex 才识别为验证码
@@ -113,14 +111,29 @@
         yield
         for h in handlers:
             try:
                 self.client.remove_handler(h, group=group)
             except ValueError:
                 pass
 
+    @cached(ttl=60, noself=True)
+    async def get_ocr(self, ocr: str = None):
+        if not ocr:
+            return DdddOcr(beta=True, show_ad=False)
+        else:
+            data = []
+            files = (f"{ocr}.onnx", f"{ocr}.json")
+            async for p in get_datas(self.basedir, files, proxy=self.proxy, caller=self.name):
+                if p is None:
+                    self.log.warning(f"初始化错误: 无法下载所需文件.")
+                    return None
+                else:
+                    data.append(p)
+            return DdddOcr(show_ad=False, import_onnx_path=str(data[0]), charsets_path=str(data[1]))
+
     async def start(self):
         ident = self.chat_name or self.bot_id or self.bot_username
         while True:
             try:
                 chat = await self.client.get_chat(ident)
             except UsernameNotOccupied:
                 self.log.warning(f'初始化错误: 会话 "{ident}" 不存在.')
@@ -142,65 +155,56 @@
                 if d.chat.id == chat.id:
                     break
             else:
                 if not self.bot_allow_from_scratch:
                     self.log.info(f'跳过签到: 从未与 "{ident}" 交流.')
                     return None
 
-        async with self.lock:
-            if isinstance(self.ocr, str):
-                data = []
-                files = (f"{self.ocr}.onnx", f"{self.ocr}.json")
-                async for p in get_datas(self.basedir, files, proxy=self.proxy, caller=self.name):
-                    if p is None:
-                        self.log.warning(f"初始化错误: 无法下载所需文件.")
-                        return None
-                    else:
-                        data.append(p)
-                self.__class__.ocr = DdddOcr(
-                    show_ad=False, import_onnx_path=str(data[0]), charsets_path=str(data[1])
-                )
-
         bot = await self.client.get_users(self.bot_id or self.bot_username)
         msg = f"开始执行签到: [green]{bot.name}[/] [gray50](@{bot.username})[/]"
         if chat.title:
             msg += f" @ [green]{chat.title}[/] [gray50](@{chat.username})[/]"
         self.log.info(msg + ".")
 
         if not self.chat_name:
             self.log.debug(f"[gray50]禁用提醒 {self.timeout} 秒: {bot.username}[/]")
             await self.client.mute_chat(ident, time.time() + self.timeout + 10)
 
         try:
             async with self.listener():
-                if self.bot_use_history is None:
-                    await self.send_checkin()
-                elif not await self.walk_history(self.bot_use_history):
-                    await self.send_checkin()
+                cancelled = False
                 try:
+                    if self.bot_use_history is None:
+                        await self.send_checkin()
+                    elif not await self.walk_history(self.bot_use_history):
+                        await self.send_checkin()
                     await asyncio.wait_for(self.finished.wait(), self.timeout)
-                except asyncio.TimeoutError:
-                    pass
+                except asyncio.CancelledError:
+                    cancelled = True
+                    raise
                 finally:
-                    if self._is_archived:
-                        self.log.debug(f"[gray50]将会话重新归档: {ident}[/]")
-                        try:
-                            await asyncio.shield(asyncio.wait_for(chat.archive(), 3))
-                        except asyncio.TimeoutError:
-                            self.log.debug(f"[gray50]归档失败: {ident}[/]")
+                    if not cancelled:
+                        if self._is_archived:
+                            self.log.debug(f"[gray50]将会话重新归档: {ident}[/]")
+                            try:
+                                await chat.archive()
+                            except asyncio.TimeoutError:
+                                self.log.debug(f"[gray50]归档失败: {ident}[/]")
+                        if not self.chat_name:
+                            self.log.debug(f"[gray50]将会话设为已读: {ident}[/]")
+                            try:
+                                if await self.client.read_chat_history(ident):
+                                    self.log.debug(f"[gray50]设为已读成功: {ident}[/]")
+                            except asyncio.TimeoutError:
+                                self.log.debug(f"[gray50]设为已读失败: {ident}[/]")
         except OSError as e:
             self.log.warning(f'初始化错误: "{e}".')
             return False
-        finally:
-            if not self.chat_name:
-                self.log.debug(f"[gray50]将会话设为已读: {ident}[/]")
-                try:
-                    await asyncio.shield(asyncio.wait_for(self.client.read_chat_history(ident), 3))
-                except asyncio.TimeoutError:
-                    self.log.debug(f"[gray50]设为已读失败: {ident}[/]")
+        except asyncio.TimeoutError:
+            pass
         if not self.finished.is_set():
             self.log.warning("无法在时限内完成签到.")
             return False
         else:
             return self._retries <= self.retries
 
     async def walk_history(self, limit=0):
@@ -276,15 +280,16 @@
         elif message.text:
             return MessageType.TEXT
 
     async def on_photo(self, message: Message):
         data = await self.client.download_media(message, in_memory=True)
         image = Image.open(data)
         captcha = (
-            self.ocr.classification(image)
+            (await self.get_ocr(self.ocr))
+            .classification(image)
             .translate(str.maketrans("", "", string.punctuation))
             .replace(" ", "")
         )
         if captcha:
             self.log.debug(f"[gray50]接收验证码: {captcha}.[/]")
             if self.bot_captcha_len and len(captcha) not in to_iterable(self.bot_captcha_len):
                 self.log.info(f"签到失败: 验证码低于设定长度, 正在重试.")
```

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/jms.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ...data import get_data
 from .base import AnswerBotCheckin
 
 
 class JMSCheckin(AnswerBotCheckin):
     ocr = "idioms@v2"
     idioms = None
+    lock = asyncio.Lock()
 
     name = "卷毛鼠"
     bot_username = "jmsembybot"
 
     async def start(self):
         self.retries = 2
         async with self.lock:
```

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.7/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/link.py` & `embykeeper-2.2.7/embykeeper/telechecker/link.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,20 +46,21 @@
             self.log.debug(f"[gray50]禁用提醒 {timeout} 秒: {self.bot}[/]")
             await self.client.mute_chat(self.bot, time.time() + timeout + 5)
             future = asyncio.Future()
             handler = MessageHandler(
                 async_partial(self._handler, cmd=cmd, future=future, condition=condition),
                 filters.text & filters.bot & filters.user(self.bot),
             )
-            self.client.add_handler(handler, group=1)
+            await self.client.add_handler(handler, group=1)
             try:
                 messages = []
                 messages.append(await self.client.send_message(self.bot, f"/start quiet"))
                 await asyncio.sleep(0.5)
                 messages.append(await self.client.send_message(self.bot, cmd))
+                self.log.debug(f"[gray50]-> {cmd}[/]")
                 results = await asyncio.wait_for(future, timeout=timeout)
             except asyncio.CancelledError:
                 try:
                     await asyncio.wait_for(self.delete_messages(messages), 1.0)
                 except asyncio.TimeoutError:
                     pass
                 finally:
@@ -81,15 +82,15 @@
                     return False
                 elif status == "ok":
                     return results
                 else:
                     self.log.warning(f"{name}出现未知错误.")
                     return False
             finally:
-                self.client.remove_handler(handler, group=1)
+                await self.client.remove_handler(handler, group=1)
 
     async def _handler(
         self,
         client: Client,
         message: Message,
         cmd: str,
         future: asyncio.Future,
```

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/log.py` & `embykeeper-2.2.7/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/main.py` & `embykeeper-2.2.7/embykeeper/telechecker/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from datetime import datetime
+from functools import lru_cache
 import inspect
 import logging
 import operator
 import pkgutil
 import random
 from typing import List, Type
 from importlib import import_module
@@ -11,15 +12,14 @@
 from dateutil import parser
 from pyrogram.enums import ChatType
 from pyrogram.handlers import MessageHandler
 from pyrogram.types import Message
 from rich import box
 from rich.live import Live
 from rich.panel import Panel
-from rich.progress import MofNCompleteColumn, Progress, SpinnerColumn
 from rich.table import Column, Table
 from rich.text import Text
 
 from ..utils import batch, flatten, idle, time_in_range, async_partial, next_random_datetime
 from ..log import logger, formatter
 from . import __name__
 from .link import Link
@@ -41,14 +41,15 @@
         sub = "messager"
         suffix = "messager"
     else:
         raise ValueError(f"{type} is not a valid service.")
     return sub, suffix
 
 
+@lru_cache
 def get_names(type: str) -> List[str]:
     sub, _ = get_spec(type)
     results = []
     typemodule = import_module(f"{__name__}.{sub}")
     for _, mn, _ in pkgutil.iter_modules(typemodule.__path__):
         module = import_module(f"{__name__}.{sub}.{mn}")
         if not getattr(module, "__ignore__", False):
@@ -210,15 +211,15 @@
     while True:
         logger.bind(scheme="telechecker").info(f"下一次签到将在 {dt.strftime('%m-%d %H:%M %p')} 进行.")
         await asyncio.sleep((dt - datetime.now()).seconds)
         await checkiner(config, instant=instant)
 
 
 async def monitorer(config: dict):
-    logger.debug("正在启动消息监控模块, 请等待登录.")
+    logger.debug("正在启动消息监控模块.")
     jobs = []
     async with ClientsSession.from_config(config, monitor=True) as clients:
         async for tg in clients:
             log = logger.bind(scheme="telemonitor", username=tg.me.name)
             if not await Link(tg).auth("monitorer"):
                 log.error(f"功能初始化失败: 权限校验不通过.")
                 continue
@@ -285,14 +286,16 @@
         async for tg in clients:
             tg.add_handler(MessageHandler(async_partial(dump_message, table=table)))
         with Live(table, refresh_per_second=4, vertical_overflow="visible"):
             await idle()
 
 
 async def analyzer(config: dict, chats, keywords, timerange, limit=2000):
+    from rich.progress import MofNCompleteColumn, Progress, SpinnerColumn
+
     def render_page(progress, texts):
         page = Table.grid()
         page.add_row(Panel(progress))
         if texts:
             msgs = sorted(texts.items(), key=operator.itemgetter(1), reverse=True)
             columns = flatten([[Column(max_width=15, no_wrap=True), Column(min_width=2)] for _ in range(4)])
             table = Table(*columns, show_header=False, box=box.SIMPLE)
```

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.7/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.7/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.7/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper/telechecker/tele.py` & `embykeeper-2.2.7/embykeeper/telechecker/tele.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from collections import OrderedDict
 
 from datetime import datetime
 import asyncio
 import inspect
-from typing import AsyncGenerator, List, Optional, Union
+from typing import AsyncGenerator, Optional, Union
 
 from rich.prompt import Prompt
 from appdirs import user_data_dir
 from loguru import logger
 import pyrogram
 from pyrogram import raw, types, utils, filters, dispatcher
 from pyrogram.enums import SentCodeType
@@ -16,15 +16,16 @@
     BadRequest,
     RPCError,
     Unauthorized,
     SessionPasswordNeeded,
     CodeInvalid,
     PhoneCodeInvalid,
 )
-from pyrogram.handlers import MessageHandler, RawUpdateHandler
+from pyrogram.handlers import MessageHandler, RawUpdateHandler, DisconnectHandler
+from pyrogram.handlers.handler import Handler
 from aiocache import Cache
 
 from .. import __name__, __version__
 from ..utils import async_partial, to_iterable
 
 logger = logger.bind(scheme="telegram")
 
@@ -59,27 +60,27 @@
     def add_handler(self, handler, group: int):
         async def fn():
             async with self.mutex:
                 if group not in self.groups:
                     self.groups[group] = []
                     self.groups = OrderedDict(sorted(self.groups.items()))
                 self.groups[group].append(handler)
-                logger.debug(f"增加了 Telegram 更新处理器: {handler.__class__.__name__}.")
+                # logger.debug(f"增加了 Telegram 更新处理器: {handler.__class__.__name__}.")
 
-        self.loop.create_task(fn())
+        return self.loop.create_task(fn())
 
     def remove_handler(self, handler, group: int):
         async def fn():
             async with self.mutex:
                 if group not in self.groups:
                     raise ValueError(f"Group {group} does not exist. Handler was not removed.")
                 self.groups[group].remove(handler)
-                logger.debug(f"移除了 Telegram 更新处理器: {handler.__class__.__name__}.")
+                # logger.debug(f"移除了 Telegram 更新处理器: {handler.__class__.__name__}.")
 
-        self.loop.create_task(fn())
+        return self.loop.create_task(fn())
 
     async def handler_worker(self):
         while True:
             packet = await self.updates_queue.get()
 
             if packet is None:
                 break
@@ -181,14 +182,36 @@
             else:
                 break
         if isinstance(signed_in, types.User):
             return signed_in
         else:
             raise BadRequest("该账户尚未注册")
 
+    def add_handler(self, handler: Handler, group: int = 0):
+        if isinstance(handler, DisconnectHandler):
+            self.disconnect_handler = handler.callback
+
+            async def dummy():
+                pass
+
+            return asyncio.ensure_future(dummy())
+        else:
+            return self.dispatcher.add_handler(handler, group)
+
+    def remove_handler(self, handler: Handler, group: int = 0):
+        if isinstance(handler, DisconnectHandler):
+            self.disconnect_handler = None
+
+            async def dummy():
+                pass
+
+            return asyncio.ensure_future(dummy())
+        else:
+            return self.dispatcher.remove_handler(handler, group)
+
     async def get_dialogs(
         self, limit: int = 0, exclude_pinned=None, folder_id=None
     ) -> Optional[AsyncGenerator["types.Dialog", None]]:
         cache_id = f"dialogs_{self.phone_number}_{folder_id}_{1 if exclude_pinned else 0}"
         (offset_id, offset_date, offset_peer), cache = await self.cache.get(
             cache_id, ((0, 0, raw.types.InputPeerEmpty()), [])
         )
@@ -263,15 +286,15 @@
             future.set_result(message)
 
         future = asyncio.Future()
         filter = filters.chat(chat_id)
         if not outgoing:
             filter = filter & (~filters.outgoing)
         handler = MessageHandler(async_partial(handler_func, future=future), filter)
-        self.add_handler(handler, group=0)
+        await self.add_handler(handler, group=0)
         try:
             if text:
                 await self.send_message(chat_id, text)
             msg: types.Message = await asyncio.wait_for(future, timeout)
             return msg
         finally:
             self.remove_handler(handler, group=0)
```

### Comparing `embykeeper-2.2.6/embykeeper/utils.py` & `embykeeper-2.2.7/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.7/embykeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.6
+Version: 2.2.7
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -87,15 +87,15 @@
 
 ### 在线部署
 
 #### Railway
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
 #### Render.com
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.6 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.7 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -89,15 +89,15 @@
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
 (https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
 å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
-(https://railway.app/button.svg)](https://railway.app/template/
+(https://railway.app/button.svg)](https://railway.app/new/template/
 WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
 embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
 06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
 5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
 é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://render.com/images/deploy-to-render-button.svg)](https://render.com/
```

### Comparing `embykeeper-2.2.6/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.2.7/embykeeper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 embykeeper/telechecker/bots/ljyy.py
 embykeeper/telechecker/bots/nebula.py
 embykeeper/telechecker/bots/peach.py
 embykeeper/telechecker/bots/pornemby.py
 embykeeper/telechecker/bots/singularity.py
 embykeeper/telechecker/bots/sssq.py
 embykeeper/telechecker/bots/terminus.py
+embykeeper/telechecker/bots/test.py
 embykeeper/telechecker/messager/__init__.py
 embykeeper/telechecker/messager/base.py
 embykeeper/telechecker/messager/common.py
 embykeeper/telechecker/messager/nakonako.py
 embykeeper/telechecker/messager/test.py
 embykeeper/telechecker/monitor/__init__.py
 embykeeper/telechecker/monitor/base.py
```

### Comparing `embykeeper-2.2.6/embykeeperweb/app.py` & `embykeeper-2.2.7/embykeeperweb/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pty
 import select
 import fcntl
 import struct
 import subprocess
 import termios
+import threading
 import time
 import signal
 
 import typer
 from loguru import logger
 from flask import Flask, render_template, request, redirect, url_for, jsonify, abort
 from flask_socketio import SocketIO
@@ -24,14 +25,16 @@
 
 app.config["args"] = None
 app.config["fd"] = None
 app.config["pid"] = None
 app.config["hist"] = ""
 app.config["faillog"] = []
 
+lock = threading.Lock()
+
 
 class DummyUser:
     def is_authenticated(self):
         return True
 
     def is_active(self):
         return True
@@ -91,22 +94,16 @@
 def heartbeat():
     webpass = os.environ.get("EK_WEBPASS", "")
     password = request.args.get("pass", None)
     if (not password) or (not webpass):
         return abort(403)
     if password == webpass:
         if app.config["pid"] is None:
-            (pid, fd) = pty.fork()
-            if pid == 0:
-                subprocess.run(["embykeeper", *app.config["args"]])
-            else:
-                app.config["fd"] = fd
-                app.config["pid"] = pid
-                logger.debug(f"Embykeeper started at: {pid}.")
-            return jsonify({"status": "restarted", "pid": pid}), 201
+            start({"rows": 32, "cols": 106}, auth=False)
+            return jsonify({"status": "restarted", "pid": app.config["pid"]}), 201
         else:
             return jsonify({"status": "running", "pid": app.config["pid"]}), 200
     else:
         return abort(403)
 
 
 @app.errorhandler(404)
@@ -144,52 +141,77 @@
             (data, _, _) = select.select([app.config["fd"]], [], [], 0)
             if data:
                 output = os.read(app.config["fd"], max_read_bytes).decode(errors="ignore")
                 app.config["hist"] += output
                 socketio.emit("pty-output", {"output": output}, namespace="/pty")
 
 
+@socketio.on("connect", namespace="/pty")
+def connected():
+    logger.debug(f"Console connected.")
+
+
+@socketio.on("disconnect", namespace="/pty")
+def connected():
+    logger.debug(f"Console disconnected.")
+
+
 @socketio.on("embykeeper_start", namespace="/pty")
-def start(data):
-    if not current_user.is_authenticated():
+def start(data, auth=True):
+    if auth and (not current_user.is_authenticated()):
         return
-    if app.config["fd"]:
-        set_size(app.config["fd"], data["rows"], data["cols"])
-        socketio.emit("pty-output", {"output": app.config["hist"]}, namespace="/pty")
-    else:
-        (pid, fd) = pty.fork()
-        if pid == 0:
-            subprocess.run(["embykeeper", *app.config["args"]])
-        else:
-            app.config["fd"] = fd
-            app.config["pid"] = pid
-            logger.debug(f"Embykeeper started at: {pid}.")
+    with lock:
+        if app.config["fd"]:
             set_size(app.config["fd"], data["rows"], data["cols"])
-            socketio.start_background_task(target=read_and_forward_pty_output)
+            socketio.emit("pty-output", {"output": app.config["hist"]}, namespace="/pty")
+        else:
+            (pid, fd) = pty.fork()
+            if pid == 0:
+                while True:
+                    try:
+                        p = subprocess.run(["embykeeper", *app.config["args"]])
+                        if p.returncode:
+                            raise RuntimeError()
+                    except (KeyboardInterrupt, RuntimeError):
+                        print()
+                        while True:
+                            try:
+                                input("Embykeeper 已退出, 请按 Enter 以重新开始 ...")
+                                print()
+                                break
+                            except KeyboardInterrupt:
+                                print()
+            else:
+                app.config["fd"] = fd
+                app.config["pid"] = pid
+                logger.debug(f"Embykeeper started at: {pid}.")
+                set_size(app.config["fd"], data["rows"], data["cols"])
+                socketio.start_background_task(target=read_and_forward_pty_output)
 
 
 @socketio.on("embykeeper_kill", namespace="/pty")
 def stop():
     if not current_user.is_authenticated():
         return
-    if app.config["pid"] is not None:
-        os.kill(app.config["pid"], signal.SIGINT)
-        for _ in range(50):
-            try:
-                os.kill(app.config["pid"], 0)
-            except OSError:
-                break
+    with lock:
+        if app.config["pid"] is not None:
+            os.kill(app.config["pid"], signal.SIGINT)
+            for _ in range(50):
+                try:
+                    os.kill(app.config["pid"], 0)
+                except OSError:
+                    break
+                else:
+                    time.sleep(0.1)
             else:
-                time.sleep(0.1)
-        else:
-            os.kill(app.config["pid"], signal.SIGKILL)
-        app.config["fd"] = None
-        app.config["pid"] = None
-        app.config["hist"] = ""
-        logger.debug(f"Embykeeper stopped.")
+                os.kill(app.config["pid"], signal.SIGKILL)
+            app.config["fd"] = None
+            app.config["pid"] = None
+            app.config["hist"] = ""
+            logger.debug(f"Embykeeper stopped.")
 
 
 @cli.command(context_settings={"ignore_unknown_options": True, "allow_extra_args": True})
 def run(ctx: typer.Context, port: int = 1818, host: str = "0.0.0.0", debug: bool = False):
     app.config["args"] = ctx.args
     logger.info(f"Embykeeper webserver started at {host}:{port}.")
     socketio.run(app, port=port, host=host, debug=debug)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/404.html` & `embykeeper-2.2.7/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.2.7/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.2.7/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.2.7/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.2.7/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.2.7/embykeeperweb/templates/assets/js/console.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -46,22 +46,22 @@
         const dims = {
             cols: term.cols,
             rows: term.rows
         };
         socket.emit("embykeeper_start", dims);
     });
 
-    socket.on("disconnect", () => {
+    socket.on("disconnect", (reason) => {
         var statusIcon = document.getElementById("status-icon");
         statusIcon.style.backgroundColor = "red";
         var statusMsg = document.getElementById("status-msg");
         statusMsg.textContent = "Program Disconnected";
         var restartIcon = document.getElementById("restart-icon");
         restartIcon.style.animationPlayState = "running";
-        console.info("Web console disconnected.");
+        console.info("Web console disconnected: ", reason);
     });
 
     var restartBtn = document.getElementById("restart-btn");
     restartBtn.addEventListener('click', () => {
         socket.emit("embykeeper_kill");
         socket.disconnect();
         var statusMsg = document.getElementById("status-msg");
@@ -88,14 +88,15 @@
             timeout = setTimeout(() => func.apply(context, args), wait_ms);
         };
     }
 
     window.onresize = debounce(resize, 50);
 
     term.onData((data) => {
+        console.debug(data)
         socket.emit("pty-input", {
             input: data
         });
     });
 
     socket.on("pty-output", (data) => {
         term.write(data.output);
```

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.2.7/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/console.html` & `embykeeper-2.2.7/embykeeperweb/templates/console.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="stylesheet" href="assets/bootstrap/css/bootstrap.min.css">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800&amp;display=swap">
-    <link rel="stylesheet" href="assets/css/cascadia-code.css">
     <link rel="stylesheet" href="assets/css/icons.css">
     <link rel="stylesheet" href="assets/css/styles.css">
     <link rel="stylesheet" href="https://unpkg.com/xterm@5.2.1/css/xterm.css">
 </head>
 
 <body>
     <nav class="navbar navbar-light navbar-expand-md fixed-top navbar-shrink py-3" id="mainNav">
```

#### html2text {}

```diff
@@ -8,15 +8,14 @@
 
 
 
 
 
 
 
-
 EmbykeeperToggle navigation
 Web_Console
 
 Program Connecting
 
 
 Copyright Â© 2023 Embykeeper
```

### Comparing `embykeeper-2.2.6/embykeeperweb/templates/login.html` & `embykeeper-2.2.7/embykeeperweb/templates/login.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="icon" type="image/svg+xml" sizes="160x160" href="assets/img/illustrations/logo-only.svg">
     <link rel="stylesheet" href="assets/bootstrap/css/bootstrap.min.css">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800&amp;display=swap">
-    <link rel="stylesheet" href="assets/css/cascadia-code.css">
     <link rel="stylesheet" href="assets/css/icons.css">
     <link rel="stylesheet" href="assets/css/styles.css">
 </head>
 
 <body>
     <nav class="navbar navbar-light navbar-expand-md fixed-top navbar-shrink py-3" id="mainNav">
         <div class="container"><a class="navbar-brand d-flex align-items-center" href="/"><span>Embykeeper</span></a><button data-bs-toggle="collapse" class="navbar-toggler" data-bs-target="#navcol-1"><span class="visually-hidden">Toggle navigation</span><span class="navbar-toggler-icon"></span></button>
```

#### html2text {}

```diff
@@ -7,15 +7,14 @@
 
 
 
 
 
 
 
-
 EmbykeeperToggle navigation
 Web_Console
 
 [assets/img/illustrations/login.svg]
 ***** Login
  *****
 {% if emsg %}
```

### Comparing `embykeeper-2.2.6/pyproject.toml` & `embykeeper-2.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.6"
+version = "2.2.7"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-2.2.6/tests/test_cli.py` & `embykeeper-2.2.7/tests/test_cli.py`

 * *Files identical despite different names*

