# Comparing `tmp/ayugespidertools-3.3.0.tar.gz` & `tmp/ayugespidertools-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.3.0.tar", max compression
+gzip compressed data, was "ayugespidertools-3.3.1.tar", max compression
```

## Comparing `ayugespidertools-3.3.0.tar` & `ayugespidertools-3.3.1.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/LICENSE
--rw-r--r--   0        0        0    14144 2023-06-21 05:41:38.000000 ayugespidertools-3.3.0/README.md
--rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.0/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.0/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.3.0/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.0/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.3.0/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3696 2023-06-07 02:13:50.000000 ayugespidertools-3.3.0/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6610 2023-06-07 02:13:56.000000 ayugespidertools-3.3.0/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     5265 2023-06-09 09:17:13.000000 ayugespidertools-3.3.0/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    16918 2023-06-20 02:40:39.000000 ayugespidertools-3.3.0/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13306 2023-06-07 01:56:44.000000 ayugespidertools-3.3.0/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32649 2023-06-20 01:18:52.000000 ayugespidertools-3.3.0/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     6000 2023-06-06 07:14:58.000000 ayugespidertools-3.3.0/ayugespidertools/common/spiderconf.py
--rw-r--r--   0        0        0     3718 2023-06-07 02:14:02.000000 ayugespidertools-3.3.0/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     3158 2023-06-07 07:53:47.000000 ayugespidertools-3.3.0/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    10672 2023-06-20 02:00:17.000000 ayugespidertools-3.3.0/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3685 2023-06-07 02:14:19.000000 ayugespidertools-3.3.0/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      388 2023-06-07 02:14:26.000000 ayugespidertools-3.3.0/ayugespidertools/config.py
--rw-r--r--   0        0        0     9982 2023-06-07 02:14:34.000000 ayugespidertools-3.3.0/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7673 2023-06-07 02:14:39.000000 ayugespidertools-3.3.0/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     4714 2023-06-21 02:16:27.000000 ayugespidertools-3.3.0/ayugespidertools/items.py
--rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.0/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8542 2023-06-07 02:14:45.000000 ayugespidertools-3.3.0/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.0/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5448 2023-06-09 09:27:15.000000 ayugespidertools-3.3.0/ayugespidertools/oss.py
--rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.0/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.0/ayugespidertools/request.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-07 02:13:19.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10562 2023-06-19 03:16:03.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     3779 2023-06-07 02:15:17.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2429 2023-06-07 02:15:24.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/download/__init__.py
--rw-r--r--   0        0        0     2453 2023-06-21 06:16:08.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     1495 2023-06-19 09:43:52.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2046 2023-06-19 09:44:14.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1183 2023-06-19 09:44:52.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     3180 2023-06-07 09:54:44.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
--rw-r--r--   0        0        0     1779 2023-06-07 09:52:37.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0    11430 2023-06-20 02:32:25.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     3851 2023-06-19 09:45:42.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-06-16 03:09:25.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2734 2023-06-06 08:35:52.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3608 2023-06-19 09:45:59.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     7944 2023-06-21 08:29:00.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.0/ayugespidertools/spiders.py
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     5168 2023-06-21 08:26:39.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.0/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.3.0/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3074 2023-06-21 07:30:30.000000 ayugespidertools-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 ayugespidertools-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/LICENSE
+-rw-r--r--   0        0        0    14144 2023-06-21 05:41:38.000000 ayugespidertools-3.3.1/README.md
+-rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.1/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.1/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.3.1/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.1/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.3.1/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3696 2023-06-07 02:13:50.000000 ayugespidertools-3.3.1/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6610 2023-06-07 02:13:56.000000 ayugespidertools-3.3.1/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     5265 2023-06-09 09:17:13.000000 ayugespidertools-3.3.1/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    16918 2023-06-20 02:40:39.000000 ayugespidertools-3.3.1/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13306 2023-06-07 01:56:44.000000 ayugespidertools-3.3.1/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32649 2023-06-20 01:18:52.000000 ayugespidertools-3.3.1/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     6000 2023-06-06 07:14:58.000000 ayugespidertools-3.3.1/ayugespidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3718 2023-06-07 02:14:02.000000 ayugespidertools-3.3.1/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     3577 2023-06-26 09:54:18.000000 ayugespidertools-3.3.1/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    10672 2023-06-20 02:00:17.000000 ayugespidertools-3.3.1/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3685 2023-06-07 02:14:19.000000 ayugespidertools-3.3.1/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      388 2023-06-07 02:14:26.000000 ayugespidertools-3.3.1/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9982 2023-06-07 02:14:34.000000 ayugespidertools-3.3.1/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7673 2023-06-07 02:14:39.000000 ayugespidertools-3.3.1/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     6383 2023-06-29 08:59:35.000000 ayugespidertools-3.3.1/ayugespidertools/items.py
+-rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.1/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8542 2023-06-07 02:14:45.000000 ayugespidertools-3.3.1/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.1/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5448 2023-06-09 09:27:15.000000 ayugespidertools-3.3.1/ayugespidertools/oss.py
+-rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.1/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.1/ayugespidertools/request.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 06:57:30.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/headers/__init__.py
+-rw-r--r--   0        0        0     1644 2023-06-26 09:00:55.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10562 2023-06-19 03:16:03.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3779 2023-06-07 02:15:17.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2429 2023-06-07 02:15:24.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/download/__init__.py
+-rw-r--r--   0        0        0     2453 2023-06-25 08:49:18.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1495 2023-06-19 09:43:52.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2046 2023-06-19 09:44:14.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1183 2023-06-19 09:44:52.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3180 2023-06-07 09:54:44.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     1779 2023-06-07 09:52:37.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0    11430 2023-06-20 02:32:25.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     3851 2023-06-19 09:45:42.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-06-16 03:09:25.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2734 2023-06-06 08:35:52.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3608 2023-06-19 09:45:59.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7944 2023-06-21 08:29:00.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.1/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     5168 2023-06-21 08:26:39.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.1/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.3.1/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3074 2023-06-29 07:47:06.000000 ayugespidertools-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 ayugespidertools-3.3.1/PKG-INFO
```

### Comparing `ayugespidertools-3.3.0/LICENSE` & `ayugespidertools-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/README.md` & `ayugespidertools-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.3.1/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/commands/version.py` & `ayugespidertools-3.3.1/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/encryption.py` & `ayugespidertools-3.3.1/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/expend.py` & `ayugespidertools-3.3.1/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.3.1/ayugespidertools/common/mongodbpipe.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.3.1/ayugespidertools/common/multiplexing.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.3.1/ayugespidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/params.py` & `ayugespidertools-3.3.1/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/spiderconf.py` & `ayugespidertools-3.3.1/ayugespidertools/common/spiderconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.3.1/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/typevars.py` & `ayugespidertools-3.3.1/ayugespidertools/common/typevars.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     "MongoDBConf",
     "AiohttpConf",
     "AiohttpRequestArgs",
     "MQConf",
     "KafkaConf",
     "DynamicProxyConf",
     "ExclusiveProxyConf",
+    "FieldAlreadyExistsError",
+    "EmptyKeyError",
 ]
 
 AiohttpRequestMethodStr = Literal["GET", "POST"]
 TableEnumTypeVar = TypeVar("TableEnumTypeVar", bound="TableEnum")
 
 sentinel: Any = object()
 
@@ -129,7 +131,20 @@
     index: int
 
 
 class KafkaConf(NamedTuple):
     bootstrap_servers: list
     topic: str
     key: str
+
+
+class FieldAlreadyExistsError(Exception):
+    def __init__(self, field_name: str):
+        self.field_name = field_name
+        self.message = f"字段 {field_name} 已存在！"
+        super().__init__(self.message)
+
+
+class EmptyKeyError(Exception):
+    def __init__(self):
+        self.message = "字段名不能为空！"
+        super().__init__(self.message)
```

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/utils.py` & `ayugespidertools-3.3.1/ayugespidertools/common/utils.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.3.1/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/formatdata.py` & `ayugespidertools-3.3.1/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/imgoperation.py` & `ayugespidertools-3.3.1/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/middlewares.py` & `ayugespidertools-3.3.1/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/mongoclient.py` & `ayugespidertools-3.3.1/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.3.1/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/oss.py` & `ayugespidertools-3.3.1/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/pipelines.py` & `ayugespidertools-3.3.1/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,23 +28,22 @@
     @classmethod
     def from_crawler(cls, crawler):
         s = cls()
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
     def spider_opened(self, spider):
-        # 带权重的 ua 列表，将比较常用的 ua 标识的权重设置高一点。这里是根据 fake_useragent 库中的打印信息来规划权重的。
+        # 带权重的 ua 列表，这里是根据 fake_useragent 库中的打印信息来规划权重的。
         ua_arr = [
             {"explorer": "opera", "weight": 16},
             {"explorer": "safari", "weight": 32},
             {"explorer": "internetexplorer", "weight": 41},
             {"explorer": "firefox", "weight": 124},
             {"explorer": "chrome", "weight": 772},
         ]
         self.explorer_types = [x["explorer"] for x in ua_arr]
         self.explorer_weights = [x["weight"] for x in ua_arr]
         spider.slog.info(f"随机请求头中间件 RandomRequestUaMiddleware 已开启，生效脚本为: {spider.name}")
 
     def process_request(self, request, spider):
         # 根据权重来获取随机请求头 ua 信息
-        if curr_ua := self.get_random_ua_by_weight():
-            request.headers.setdefault(b"User-Agent", curr_ua)
+        request.headers.setdefault(b"User-Agent", self.get_random_ua_by_weight())
```

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __all__ = [
     "FilesDownloadPipeline",
 ]
 
 
 class FilesDownloadPipeline:
     """
-    截图场景的 scrapy pipeline 扩展
+    文件下载的 scrapy pipeline 扩展
     """
 
     _type = "normal"
 
     def __init__(self, file_path=None, doc_path=None):
         self.file_path = file_path or doc_path
```

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.3.1/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.3.1/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/ayugespidertools/verificationcode.py` & `ayugespidertools-3.3.1/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.0/pyproject.toml` & `ayugespidertools-3.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "3.3.0"
+version = "3.3.1"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
```

### Comparing `ayugespidertools-3.3.0/PKG-INFO` & `ayugespidertools-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 3.3.0
+Version: 3.3.1
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
```

