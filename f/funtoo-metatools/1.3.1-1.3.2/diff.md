# Comparing `tmp/funtoo-metatools-1.3.1.tar.gz` & `tmp/funtoo-metatools-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo-metatools-1.3.1.tar", last modified: Sat Jun  3 19:14:46 2023, max compression
+gzip compressed data, was "funtoo-metatools-1.3.2.tar", last modified: Thu Jun 29 16:44:11 2023, max compression
```

## Comparing `funtoo-metatools-1.3.1.tar` & `funtoo-metatools-1.3.2.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7697 2023-06-03 19:14:17.000000 funtoo-metatools-1.3.1/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.1/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-06-03 19:09:39.000000 funtoo-metatools-1.3.1/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.263907 funtoo-metatools-1.3.1/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.1/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-09-27 00:51:20.000000 funtoo-metatools-1.3.1/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.1/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.1/bin/fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.1/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.263907 funtoo-metatools-1.3.1/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.1/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25532 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23260 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-05-10 22:44:54.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8494 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2033 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-03 19:14:35.000000 funtoo-metatools-1.3.1/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/blos.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5547 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.1/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8854 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27038 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34989 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21741 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11722 2023-06-03 19:10:01.000000 funtoo-metatools-1.3.1/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18866 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-06-03 19:14:42.000000 funtoo-metatools-1.3.1/metatools/version.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/yaml_util.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/zmq/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:08:14.000000 funtoo-metatools-1.3.1/metatools/zmq/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/app_core.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/key_monkey.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_breezyops.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-06-03 19:14:42.000000 funtoo-metatools-1.3.1/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.1/setup.py.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10223 2023-06-29 16:44:05.000000 funtoo-metatools-1.3.2/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-28 13:33:54.000000 funtoo-metatools-1.3.2/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-06-29 16:44:05.000000 funtoo-metatools-1.3.2/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-07-01 21:12:13.000000 funtoo-metatools-1.3.2/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-06-21 18:32:19.000000 funtoo-metatools-1.3.2/bin/blos-check
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-07-05 16:37:27.000000 funtoo-metatools-1.3.2/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5765 2023-06-21 18:57:03.000000 funtoo-metatools-1.3.2/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-07-02 21:37:50.000000 funtoo-metatools-1.3.2/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-11 18:07:53.000000 funtoo-metatools-1.3.2/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-24 17:38:15.000000 funtoo-metatools-1.3.2/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2023-03-12 20:53:30.000000 funtoo-metatools-1.3.2/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-05-27 22:00:31.000000 funtoo-metatools-1.3.2/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-05-07 21:05:04.000000 funtoo-metatools-1.3.2/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-30 18:57:30.000000 funtoo-metatools-1.3.2/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25532 2023-05-11 18:07:53.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23252 2023-06-06 20:23:35.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-04-24 17:38:15.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8494 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.938894 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-06 20:18:23.000000 funtoo-metatools-1.3.2/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.942894 funtoo-metatools-1.3.2/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-07-01 21:12:17.000000 funtoo-metatools-1.3.2/metatools/blos.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.942894 funtoo-metatools-1.3.2/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5554 2023-06-21 18:28:47.000000 funtoo-metatools-1.3.2/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-24 17:38:15.000000 funtoo-metatools-1.3.2/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.942894 funtoo-metatools-1.3.2/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8955 2023-06-21 18:34:52.000000 funtoo-metatools-1.3.2/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27292 2023-06-15 16:13:13.000000 funtoo-metatools-1.3.2/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/fetch_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-07-01 21:12:17.000000 funtoo-metatools-1.3.2/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34989 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2023-05-31 18:48:13.000000 funtoo-metatools-1.3.2/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21776 2023-06-21 18:32:19.000000 funtoo-metatools-1.3.2/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-06-21 18:32:19.000000 funtoo-metatools-1.3.2/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18866 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/tree.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-06-29 16:44:08.000000 funtoo-metatools-1.3.2/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/yaml_util.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/metatools/zmq/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-06 20:18:23.000000 funtoo-metatools-1.3.2/metatools/zmq/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/app_core.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/key_monkey.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_breezyops.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-06-29 16:44:08.000000 funtoo-metatools-1.3.2/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/subpop.yaml
```

### Comparing `funtoo-metatools-1.3.1/.pre-commit-config.yaml` & `funtoo-metatools-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/ChangeLog.rst` & `funtoo-metatools-1.3.2/ChangeLog.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,55 @@
+metatools 1.3.2
+===============
+
+Released on June 29, 2023.
+
+This is a maintenance/general update release.
+
+* FL-11382: For ``Artifact``, throw exceptions when ``fetch()``,
+  ``ensure_fetched()``, ``ensure_completed()`` fail. If ``throw=False``
+  specified for ``ensure_fetched()`` then this behavior is disabled and
+  ``None`` is returned on fetch failure.
+* Add additional debugging for ``http_fetch`` if we get a 304 response
+  and are not expecting it. In this case, log detailed header information
+  so we can troubleshoot it. This may be an infrequently-occurring bug
+  that still needs to be fixed. We should only get a 304 if we specify
+  ``If-None-Match`` or ``If-Modified-Since``.
+* Small fix to allow Funtoo to only have one Python implementation as
+  up until now it has had two (2.7 and 3.7 in 1.4-release, and 3.7
+  and 3.9 in next-release. We are now moving to just 3.9 in next.
+* Add a ``blos-check`` tool to scan the Integrity Database (this is the
+  thing that maps a distfile name to a specific binary object in the
+  Base Layer Object Store, or BLOS) to look for any missing binary
+  objects. This is not really needed but sometimes when I am debugging
+  our stores, I need to run this for due diligence. It hasn't found
+  any issues yet.
+* Add ``distfile-kit-fetch`` tool which you would run on the system
+  you ran ``merge-kits`` on. It will try to grab all the non-autogenned
+  distfiles and download all it can, ultra-fast-spider style, and store
+  them locally in the BLOS. It is used like this:
+  ``distfile-kit-fetch <release> <kit> <branch-of-kit>``
+  It will use the kit-cache data from a previous ``merge-kits`` run.
+  This kit-cache data is stored in ``~/repo_tmp/tmp/kit_cache``.
+  This tool also will make sure it has a locally-checked out
+  ``kit-fixups`` repo in ``~/repo_tmp/source-trees/kit-fixups`` and
+  will utilize the ``thirdpartymirrors`` file located at
+  ``core-kit/curated/profiles/thirdpartymirrors`` to expand any
+  ``mirror://`` prefixes in ebuild ``SRC_URI`` strings. Additional
+  work has been done on this tool to make it production-quality. For
+  example, it won't stop running when it encounters a file download
+  that errors out -- instead it will be greedy and try to keep
+  downloading as many distfiles as it can.
+* Support for archive verification of ``.tar`` files (no compression,
+  and we do see these sometimes.)
+* Add missing ``await`` for initializing ``kit-fixups`` repo in
+  ``AutogenConfig`` initialization which should fix a potential
+  race condition.
+
+
 metatools 1.3.1
 ===============
 
 Released on June 3, 2023.
 
 This is a bugfix release.
 
@@ -14,15 +62,16 @@
   will be corrupt and the retrieved data will be invalid, and
   there was no obvious way to clear out this corrupt data.
   This would result in cached JSON data from ``get_page()``
   being invalid and re-running ``doit`` would not fix this.
   So a fix was added so that any corrupt entries in
   ``FileStorageBackend`` will be treated as if they don't exist
   (returning a ``CacheMiss()``) which will allow ``doit`` to
-  overwite these corrupt entries with new, corrected entries.
+  overwrite these corrupt entries with new, corrected entries.
+
 
 metatools 1.3.0
 ===============
 
 Released on May 29, 2023.
 
 This is a feature release containing a number of new capabilities
```

### Comparing `funtoo-metatools-1.3.1/PKG-INFO` & `funtoo-metatools-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.1/README.rst` & `funtoo-metatools-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/blos` & `funtoo-metatools-1.3.2/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/deepdive` & `funtoo-metatools-1.3.2/bin/deepdive`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/deepquery` & `funtoo-metatools-1.3.2/bin/deepquery`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/distfile-kit-fetch` & `funtoo-metatools-1.3.2/bin/distfile-kit-fetch`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 #!/usr/bin/env python3
 
 import argparse
+import asyncio
+import os
 import ssl
 import sys
 
-from metatools.fastpull.spider import FetchRequest, FetchError, Download
-from metatools.kit_cache import KitCache
-from metatools.store import StoreObject
 from subpop.hub import Hub
 
 from metatools.config.autogen import StoreSpiderConfig
+from metatools.fastpull.core import verify_callback
+from metatools.fastpull.spider import FetchRequest, FetchError, Download
+from metatools.kit_cache import KitCache
+from metatools.store import StoreObject
+from metatools.tree import GitTree
 
 hub = Hub()
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 
 CLI_CONFIG = {
+	"release": {"default": None, "action": "store", "positional": True, "help": "Release to process"},
 	"kit": {"default": None, "action": "store", "positional": True, "help": "Kit to process"},
 	"branch": {"default": None, "action": "store", "positional": True, "help": "Kit branch to process"},
 	"debug": {"default": False, "action": "store_true"},
 }
 
 
-def fetch_completion_callback(download: Download) -> StoreObject:
+async def fetch_completion_callback(download: Download) -> StoreObject:
 	"""
 	This method is intended to be called *once* when an actual in-progress download of a tarball (by
 	the Spider) has completed. It performs several important finalization actions upon successful
 	download:
 
 	1. The downloaded file will be stored in the BLOS, and the resultant BLOSObject will be assigned to
 	``response.blos_object``.
@@ -36,15 +41,16 @@
 	   ``response.blos_object``.
 
 	We pass this to any Download() object we instantiate so that it has proper post-actions defined
 	for it.
 	"""
 
 	store_obj: StoreObject = pkgtools.model.blos.insert_download(download)
-	pkgtools.model.spider.cleanup(download)
+	if pkgtools.model.spider:
+		pkgtools.model.spider.cleanup(download)
 	return store_obj
 
 
 def parse_args():
 	ap = argparse.ArgumentParser()
 	for arg, kwargs in CLI_CONFIG.items():
 		if "positional" in kwargs and kwargs["positional"]:
@@ -65,29 +71,64 @@
 	"sourceforge": "http://download.sourceforge.net",
 	"gentoo": "https://gentoo.osuosl.org/distfiles",
 	"apache": "http://apache.osuosl.org",
 	"kde": "https://download.kde.org"
 }
 
 
-def mini_mirror_expander(url):
+def mini_mirror_expander(mirr_dict, url):
 	url = url[len("mirror://"):]
 	mirr_name = url.split("/")[0]
 	path = "/".join(url.split("/")[1:])
-	if mirr_name in mirr_map:
-		return mirr_map[mirr_name] + "/" + path
+	if mirr_name in mirr_dict:
+		return mirr_dict[mirr_name] + "/" + path
 	else:
 		return None
 
 
+async def fetch_task(file, url):
+	pkgtools.model.log.info(f"Fetching {url}")
+	freq = FetchRequest(url=url, expected_hashes={'sha512': file['hashes']['sha512']})
+	try:
+		fresp = await pkgtools.model.spider.download(freq, completion_pipeline=[verify_callback, fetch_completion_callback])
+	except ssl.SSLError as ssle:
+		pkgtools.model.log.warning(f"SSL error for {url}: {ssle}")
+		return
+	except FetchError as fe:
+		pkgtools.model.log.warning(f"Fetch error for {url}: {fe}")
+		return
+	if fresp is not None:
+		pkgtools.model.log.info(f"Fetch OK: {url}")
+	else:
+		pkgtools.model.log.error(f"Fetch FAIL: {url}")
+
+
 async def main_thread():
 	hub.OPT = parse_args()
 	await pkgtools.launch(StoreSpiderConfig)
-	kit_cache = KitCache(name=hub.OPT.kit, branch=hub.OPT.branch)
+
+	kit_fixups_root = os.path.join(pkgtools.model.source_trees, "kit-fixups")
+	pkgtools.model.log.info("Cloning/updating kit-fixups to access thirdpartymirrors (--fast to use as-is)")
+	kit_fixups = GitTree(
+		name='kit-fixups',
+		root=kit_fixups_root,
+		model=pkgtools.model,
+		keep_branch=True
+	)
+	await kit_fixups.initialize()
+
+	mirr_dict = {}
+	with open(os.path.join(kit_fixups_root, "core-kit/curated/profiles/thirdpartymirrors"), "r") as f:
+		for line in f.readlines():
+			ls = line.split()
+			mirr_dict[ls[0]] = ls[1]
+
+	kit_cache = KitCache(name=hub.OPT.kit, branch=hub.OPT.branch, release=hub.OPT.release)
 	kit_cache.load()
+	tasks = []
 	for atom, pkg_dict in kit_cache.items():
 
 		# Filter out duplicate SHAs. Yes, this can and does happen with golang having multiple different filenames that are the same file.
 		shas = set()
 		if "files" in pkg_dict:
 			for file in pkg_dict["files"]:
 				if "hashes" not in file:
@@ -100,41 +141,35 @@
 				if obj is None:
 					pkgtools.model.log.debug(f"DICT {pkg_dict}")
 					if "src_uri" not in file:
 						pkgtools.model.log.warning(f"No src_uri for file: {file}")
 						continue
 					url = file['src_uri'][0]
 					if url.startswith("mirror://"):
-						new_url = mini_mirror_expander(url)
+						new_url = mini_mirror_expander(mirr_dict, url)
 						if new_url is None:
 							pkgtools.model.log.warning(f"Skipping mirror: {url}")
 							continue
 						else:
 							url = new_url
 					elif not url.startswith("http://") or not url.startswith("https://") or not url.startswith("ftp://"):
 						# likely a fetch-restricted file with just the filename
 						continue
-					pkgtools.model.log.info(f"Fetching {url}")
-					freq = FetchRequest(url=url, expected_hashes={'sha512': file['hashes']['sha512']})
-					try:
-						fresp = await pkgtools.model.spider.download(freq, completion_pipeline=[fetch_completion_callback])
-					except ssl.SSLError as ssle:
-						pkgtools.model.log.warning(f"SSL error for {url}: {ssle}")
-						continue
-					except FetchError as fe:
-						pkgtools.model.log.warning(f"Fetch error for {url}: {fe}")
-						continue
-					if fresp is not None:
-						pkgtools.model.log.info(f"Fetch OK: {url}")
-					else:
-						pkgtools.model.log.error(f"Fetch FAIL: {url}")
-
-					shas.add(file['hashes']['sha512'])
+					tasks.append(asyncio.create_task(fetch_task(file, url)))
+					await asyncio.sleep(0)
 
 
+					#shas.add(file['hashes']['sha512'])
+	baddies = False
+	results = await asyncio.gather(*tasks, return_exceptions=True)
+	for result in results:
+		if isinstance(result, Exception):
+			pkgtools.model.log.error("Exception encountered: ", exc_info=result)
+			baddies = True
+	return not baddies
 # if shas:
 #	print(atom)
 #	for sha in shas:
 #		print(">>>", sha)
 #	print()
```

### Comparing `funtoo-metatools-1.3.1/bin/distfile-stats` & `funtoo-metatools-1.3.2/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/doit` & `funtoo-metatools-1.3.2/bin/doit`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/fastpull-daemon` & `funtoo-metatools-1.3.2/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/fastpull-daemon-ng` & `funtoo-metatools-1.3.2/bin/fastpull-daemon-ng`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/fastpull-fixer` & `funtoo-metatools-1.3.2/bin/fastpull-fixer`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/fetch` & `funtoo-metatools-1.3.2/bin/fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/interkit-links` & `funtoo-metatools-1.3.2/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/list-kits` & `funtoo-metatools-1.3.2/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/mcafee-tool` & `funtoo-metatools-1.3.2/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/merge-gentoo-staging` & `funtoo-metatools-1.3.2/bin/merge-gentoo-staging`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/merge-kits` & `funtoo-metatools-1.3.2/bin/merge-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/missing-links` & `funtoo-metatools-1.3.2/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/release-yaml-test` & `funtoo-metatools-1.3.2/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/reposcan` & `funtoo-metatools-1.3.2/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/storage-test` & `funtoo-metatools-1.3.2/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/bin/test-metadata-extract` & `funtoo-metatools-1.3.2/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/deprecated/mongo_backends.py` & `funtoo-metatools-1.3.2/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/Makefile` & `funtoo-metatools-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/_ext/_static/consoleoutput.css` & `funtoo-metatools-1.3.2/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/_ext/consoleoutput.py` & `funtoo-metatools-1.3.2/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/autogen-dev.rst` & `funtoo-metatools-1.3.2/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/autogen.rst` & `funtoo-metatools-1.3.2/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/conf.py` & `funtoo-metatools-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/drafts/fastpull_object_store.rst` & `funtoo-metatools-1.3.2/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/drafts/repo_defs.rst` & `funtoo-metatools-1.3.2/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/features/dynamic-archives.rst` & `funtoo-metatools-1.3.2/docs/features/dynamic-archives.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/index.rst` & `funtoo-metatools-1.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/install.rst` & `funtoo-metatools-1.3.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/intro.rst` & `funtoo-metatools-1.3.2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/docs/meta-repo.rst` & `funtoo-metatools-1.3.2/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/autogen.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/ebuild.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/ebuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,21 +319,21 @@
 		if not self.exists:
 			self.fetch()
 		super().extract()
 
 	def exists(self):
 		return self.is_fetched()
 
-	async def ensure_fetched(self, throw=False) -> bool:
+	async def ensure_fetched(self, throw=True) -> bool:
 		"""
 		This function ensures that the artifact is 'fetched' -- in other words, it exists locally. This means we can
 		calculate its hashes or extract it.
 
-		Returns a boolean with True indicating success and False failure in the default behavior with ``throw=False``,
-		otherwise the original exception will be raised.
+		Returns a boolean with True indicating success and False failure when ``throw=False``. By default, the
+		original fetch exception will be raised on error.
 		"""
 
 		if self.blos_object is not None:
 			return True
 		try:
 			# TODO: add extra headers, retry,
 			req = FetchRequest(self.url,
```

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/fetch.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/fetch.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/github.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/github.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/golang.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/golang.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/http.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/http.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/meson.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/pages.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/pyhelper.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/pyhelper.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo/pkgtools/rust.py` & `funtoo-metatools-1.3.2/funtoo/pkgtools/rust.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/funtoo_metatools.egg-info/PKG-INFO` & `funtoo-metatools-1.3.2/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.1/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo-metatools-1.3.2/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 VERSION
 make.sh
 setup.py
 setup.py.in
 subpop.yaml
 bin/blos
+bin/blos-check
 bin/deepdive
 bin/deepquery
 bin/direct-sync
 bin/distfile-kit-fetch
 bin/distfile-stats
 bin/doit
 bin/fastpull-daemon
```

### Comparing `funtoo-metatools-1.3.1/make.sh` & `funtoo-metatools-1.3.2/make.sh`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/blos.py` & `funtoo-metatools-1.3.2/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/config/autogen.py` & `funtoo-metatools-1.3.2/metatools/config/autogen.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 			spider=self.spider,
 			hashes=self.hashes
 		)
 		self.fastpull_session = self.fpos.get_scope(self.fastpull_scope)
 
 
 class StoreSpiderConfig(StoreConfig):
-	logger_name = 'metatools.spider'
+	logger_name = 'metatools.autogen'
 
 	async def initialize(self, fastpull_scope=None, debug=False):
 		self.spider = WebSpider(os.path.join(self.temp_path, "spider"), hashes=self.hashes)
 		await super().initialize(fastpull_scope=fastpull_scope, debug=debug)
 
 
 class AutogenConfig(StoreSpiderConfig):
@@ -150,15 +150,15 @@
 					name='kit-fixups',
 					root=kit_fixups_root,
 					model=self,
 					url=fixups_url,
 					branch=fixups_branch,
 					keep_branch=True
 				)
-				self.kit_fixups.initialize()
+				await self.kit_fixups.initialize()
 			else:
 				self.log.info(f"Generators will be sourced from {kit_fixups_root}")
 			self.kit_fixups_repo = GitRepositoryLocator(start_path=kit_fixups_root)
 
 		if fetch_cache_interval is not None:
 			# use our default unless another timedelta specified:
 			self.fetch_cache_interval = fetch_cache_interval
```

### Comparing `funtoo-metatools-1.3.1/metatools/config/base.py` & `funtoo-metatools-1.3.2/metatools/config/base.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/config/merge.py` & `funtoo-metatools-1.3.2/metatools/config/merge.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/context.py` & `funtoo-metatools-1.3.2/metatools/context.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/fastpull/core.py` & `funtoo-metatools-1.3.2/metatools/fastpull/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 			obj = self.parent.blos.read({"hashes.sha512": existing_ref.data['sha512']})
 			if obj is not None:
 				log.debug(
 					f"IntegrityScope:{self.scope}._get_file_by_url_new: existing object found for ref {request.url}")
 				return obj
 		new_ref = await self.parent.spider.download(request,
 		                                            completion_pipeline=[
-														self.parent.verify_callback,
+														verify_callback,
 														self.parent.fetch_completion_callback])
 		assert isinstance(new_ref, StoreObject)
 		self.store.write(
 			{"url": request.url, "sha512": new_ref.data["hashes"]["sha512"], "updated_on": datetime.utcnow()})
 		return new_ref
 
 	def get_file_dynamic(self, key_dict: dict) -> Tuple[StoreObject, dict] | Tuple[None, None]:
@@ -112,14 +112,52 @@
 		return None, None
 
 	def store_file_dynamic(self, key_dict: dict, obj_path, metadata: dict = None):
 		store_obj = self.parent.blos.insert_blob(obj_path)
 		self.dynamic.write({"key": key_dict, "hashes": store_obj.data["hashes"], "metadata": metadata if metadata else {}})
 
 
+async def verify_callback(download: Download) -> Download:
+	fn = download.request.filename
+	run_cmd = None
+	arc_desc = None
+	if fn.endswith(".tar.gz"):
+		run_cmd = "tar tzf {archive}"
+		arc_desc = "tar.gz"
+	elif fn.endswith(".tar.bz2"):
+		run_cmd = "tar tjf {archive}"
+		arc_desc = "tar.bz2"
+	elif fn.endswith(".tar.xz"):
+		run_cmd = "tar tJf {archive}"
+		arc_desc = "tar.xz"
+	elif fn.endswith(".tar.zst"):
+		run_cmd = "tar -t --zstd -f {archive}"
+		arc_desc = "tar.xz"
+	elif fn.endswith(".tar"):
+		run_cmd = "tar -t -f {archive}"
+		arc_desc = "tar"
+	elif fn.endswith(".gz"):
+		run_cmd = "gzip -dc {archive} > /dev/null"
+		arc_desc = "gzip"
+	elif fn.endswith(".bz2"):
+		run_cmd = "bzip2 -dc {archive} > /dev/null"
+		arc_desc = "bzip2"
+	elif fn.endswith(".xz"):
+		run_cmd = "xz -dc {archive} > /dev/null"
+		arc_desc = "xz"
+	if run_cmd:
+		proc, out = await run_bg(run_cmd.format(archive=download.temp_path))
+		if proc.returncode != 0:
+			raise FileIntegrityError(f"File {download.temp_path} downloaded from {download.request.url} does not appear to be a valid {arc_desc} archive!")
+		log.info(f"Download from {download.request.url} verified as valid {arc_desc} archive.")
+	else:
+		log.debug(f"NO RUN CMD for verifying {download.temp_path}")
+	return download
+
+
 class IntegrityDatabase:
 
 	def __init__(self, db_base_path, blos: BaseLayerObjectStore = None, spider=None, hashes: set = None):
 		"""
 		``blos`` is an instance of a Base Layer Object Store (used to store distfiles, indexed by their hashes,
 		and also takes care of all integrity checking tasks for us.
 
@@ -147,46 +185,14 @@
 		associate URLs with entries in the BLOS, or Base Layer Object Store.
 		"""
 		if scope_id not in self.scopes:
 			self.scopes[scope_id] = IntegrityScope(self, scope_id)
 		log.debug(f"FastPull Integrity Scope: {scope_id}")
 		return self.scopes[scope_id]
 
-	async def verify_callback(self, download: Download) -> Download:
-		fn = download.request.filename
-		run_cmd = None
-		arc_desc = None
-		if fn.endswith(".tar.gz"):
-			run_cmd = "tar tzf {archive}"
-			arc_desc = "tar.gz"
-		elif fn.endswith(".tar.bz2"):
-			run_cmd = "tar tjf {archive}"
-			arc_desc = "tar.bz2"
-		elif fn.endswith(".tar.xz"):
-			run_cmd = "tar tJf {archive}"
-			arc_desc = "tar.xz"
-		elif fn.endswith(".tar.zst"):
-			run_cmd = "tar -t --zstd -f {archive}"
-			arc_desc = "tar.xz"
-		elif fn.endswith(".gz"):
-			run_cmd = "gzip -dc {archive} > /dev/null"
-			arc_desc = "gzip"
-		elif fn.endswith(".bz2"):
-			run_cmd = "bzip2 -dc {archive} > /dev/null"
-			arc_desc = "bzip2"
-		elif fn.endswith(".xz"):
-			run_cmd = "xz -dc {archive} > /dev/null"
-			arc_desc = "xz"
-		if run_cmd:
-			proc, out = await run_bg(run_cmd.format(archive=download.temp_path))
-			if proc.returncode != 0:
-				raise FileIntegrityError(f"File {download.temp_path} downloaded from {download.request.url} does not appear to be a valid {arc_desc} archive!")
-			log.info(f"Download from {download.request.url} verified as valid {arc_desc} archive.")
-		return download
-
 	async def fetch_completion_callback(self, download: Download) -> StoreObject:
 		"""
 		This method is intended to be called *once* when an actual in-progress download of a tarball (by
 		the Spider) has completed. It performs several important finalization actions upon successful
 		download:
 
 		1. The downloaded file will be stored in the BLOS, and the resultant BLOSObject will be assigned to
```

### Comparing `funtoo-metatools-1.3.1/metatools/fastpull/spider.py` & `funtoo-metatools-1.3.2/metatools/fastpull/spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,14 +557,18 @@
 						retry = True
 					try:
 						err_response = response.json()
 					except JSONDecodeError:
 						err_response = response.text
 					log.error(
 						f"Fetch failure for {request.url}: {response.status_code} {response.reason_phrase} {err_response}")
+					if response.status_code == 304:
+						log.error("We should not get status 304 (not modified) but we did.")
+						log.error(f"Original request headers: {repr(http_client.headers)}")
+						log.error(f"Extra headers:            {repr(extra_headers)}")
 					raise FetchError(request,
 									 f"HTTP fetch Error: {request.url}: {response.status_code}: {response.reason_phrase} {err_response}",
 									 retry=retry)
 				if is_json:
 					return response.headers, response.json()
 				if encoding:
 					result = response.headers, response.content.decode(encoding)
```

### Comparing `funtoo-metatools-1.3.1/metatools/fetch_cache.py` & `funtoo-metatools-1.3.2/metatools/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/hashutils.py` & `funtoo-metatools-1.3.2/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/kit.py` & `funtoo-metatools-1.3.2/metatools/kit.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/kit_cache.py` & `funtoo-metatools-1.3.2/metatools/kit_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/metadata.py` & `funtoo-metatools-1.3.2/metatools/metadata.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/model.py` & `funtoo-metatools-1.3.2/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/pretty_logging.py` & `funtoo-metatools-1.3.2/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/steps.py` & `funtoo-metatools-1.3.2/metatools/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
 
 class GenPythonUse(MergeStep):
 	def __init__(self):
 		kit = model.release_yaml.kits["python-kit"][0]
 		pydata = kit.settings
 		out_subpath = f"funtoo/kits/python-kit/{kit.branch}"
 		self.def_python = pydata["primary"]
-		self.bk_python = pydata["alternate"]
+		self.bk_python = pydata["alternate"] if "alternate" in pydata else None
 		self.mask = pydata["mask"]
 		self.out_subpath = out_subpath
 
 	# TODO: not currently generating correct results
 	async def run(self, kit_gen):
 		all_lines = []
 		for catpkg, cpv_list in metadata.get_catpkg_from_cpvs(kit_gen.kit_cache.keys()).items():
```

### Comparing `funtoo-metatools-1.3.1/metatools/store.py` & `funtoo-metatools-1.3.2/metatools/store.py`

 * *Files 13% similar despite different names*

```diff
@@ -183,18 +183,20 @@
 class BLOBDiskReference(BLOBReference):
 	def __init__(self, path):
 		self.path = path
 
 
 class StoreObject:
 
-	def __init__(self, data, blob_path=None):
+	def __init__(self, data, blob_path=None, **kwargs):
 		self.data = data
 		if blob_path:
 			self.blob = BLOBDiskReference(path=blob_path)
+		for kw_key, kw_val in kwargs.items():
+			setattr(self, kw_key, kw_val)
 
 
 class StorageBackend:
 
 	"""
 	This is an abstract class for a storage backend. This class hierarchy allows for
 	the ``Store`` class to be re-targetable to different types of backends by choosing
@@ -281,28 +283,28 @@
 			# The try/except clause below prevents this collision from causing problems.
 			try:
 				os.link(blob_path, blob_outpath)
 			except FileExistsError:
 				pass
 		else:
 			blob_outpath = None
-		return StoreObject(data=data, blob_path=blob_outpath)
+		return StoreObject(data=data, blob_path=blob_outpath, json_path=out_path)
 
 	def read(self, spec_dict) -> Optional[StoreObject]:
 		sha = self.store.key_spec.specdict_as_hash(spec_dict)
 		dir_index = f"{sha[0:2]}/{sha[2:4]}/{sha[4:6]}"
 		in_path = f"{self.root}/{dir_index}/{sha}"
 		if not os.path.exists(in_path):
 			return None
 		blob_path = in_path + ".blob"
 		try:
 			data = self.decode_data(in_path)
 		except json.decoder.JSONDecodeError as je:
 			return None
-		return StoreObject(data=data, blob_path=blob_path if os.path.exists(blob_path) else None)
+		return StoreObject(data=data, blob_path=blob_path if os.path.exists(blob_path) else None, json_path=in_path)
 
 	def delete(self, spec_dict) -> None:
 		sha = self.store.key_spec.specdict_as_hash(spec_dict)
 		dir_index = f"{sha[0:2]}/{sha[2:4]}/{sha[4:6]}"
 		in_path = f"{self.root}/{dir_index}/{sha}"
 		if os.path.exists(in_path):
 			os.unlink(in_path)
@@ -312,14 +314,31 @@
 
 	def get_relative_path_to_root(self, disk_path):
 		common = os.path.commonpath([self.root, disk_path])
 		if common != self.root:
 			return None
 		return disk_path[len(common):].lstrip("/")
 
+	def scan(self):
+		"""
+		Scan all entries in the FileStorageBackend. This assumes that all files not ending in .blob are database
+		entries. Yields ``StoreObject``s.
+		"""
+		for w_path, w_dirs, w_files in os.walk(self.root):
+			for file in w_files:
+				if file.endswith(".blob"):
+					continue
+				in_path = os.path.join(w_path, file)
+				blob_path = in_path + ".blob"
+				try:
+					data = self.decode_data(in_path)
+				except json.decoder.JSONDecodeError as je:
+					continue
+				yield StoreObject(data=data, blob_path=blob_path if os.path.exists(blob_path) else None, json_path=in_path)
+
 
 class Store:
 
 	"""
 	This is the ``Store`` class which is the class intended to be instantiated and used by
 	other code. You will typically also pass it a ``FileStorageBackend()`` for it to
 	initialize, which will actually store your data on disk. However, in the future it
@@ -351,7 +370,8 @@
 		return self.backend.write(data, blob_path=blob_path)
 
 	def read(self, spec_dict: dict) -> Optional[StoreObject]:
 		return self.backend.read(spec_dict)
 
 	def delete(self, key_spec: dict) -> None:
 		return self.backend.delete(key_spec)
+
```

### Comparing `funtoo-metatools-1.3.1/metatools/tree.py` & `funtoo-metatools-1.3.2/metatools/tree.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/yaml_util.py` & `funtoo-metatools-1.3.2/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/zmq/app_core.py` & `funtoo-metatools-1.3.2/metatools/zmq/app_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/zmq/key_monkey.py` & `funtoo-metatools-1.3.2/metatools/zmq/key_monkey.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_breezyops.py` & `funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_breezyops.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_core.py` & `funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.1/setup.py` & `funtoo-metatools-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.3.1",
+	version="1.3.2",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
```

### Comparing `funtoo-metatools-1.3.1/setup.py.in` & `funtoo-metatools-1.3.2/setup.py.in`

 * *Files identical despite different names*

