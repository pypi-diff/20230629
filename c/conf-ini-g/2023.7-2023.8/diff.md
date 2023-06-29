# Comparing `tmp/conf-ini-g-2023.7.tar.gz` & `tmp/conf-ini-g-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf-ini-g-2023.7.tar", last modified: Wed Jun 28 11:01:47 2023, max compression
+gzip compressed data, was "conf-ini-g-2023.8.tar", last modified: Thu Jun 29 07:12:06 2023, max compression
```

## Comparing `conf-ini-g-2023.7.tar` & `conf-ini-g-2023.8.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.132863 conf-ini-g-2023.7/
--rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.7/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-06-28 11:01:47.132863 conf-ini-g-2023.7/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.7/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.7/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.7/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.119530 conf-ini-g-2023.7/conf_ini_g/
--rw-r--r--   0 eric      (1000) users      (984)     1779 2023-05-12 13:37:01.000000 conf-ini-g-2023.7/conf_ini_g/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/conf_ini_g/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/conf_ini_g/catalog/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.119530 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/
--rw-r--r--   0 eric      (1000) users      (984)     2529 2023-06-14 07:31:54.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2346 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.119530 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     1965 2023-06-02 15:09:21.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:29.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     2060 2023-05-31 13:36:33.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 14:56:56.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.122863 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/
--rw-r--r--   0 eric      (1000) users      (984)     2679 2023-06-14 07:32:27.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2344 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.122863 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     2010 2023-06-02 15:43:40.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:33.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     2059 2023-06-02 14:30:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 15:01:41.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.122863 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3631 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     3814 2023-06-14 08:11:16.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     3859 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/directory.py
--rw-r--r--   0 eric      (1000) users      (984)     3387 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/multitype.py
--rw-r--r--   0 eric      (1000) users      (984)     2222 2023-06-14 07:01:24.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/none.py
--rw-r--r--   0 eric      (1000) users      (984)     6047 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/path.py
--rw-r--r--   0 eric      (1000) users      (984)     7470 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)     2460 2023-06-14 08:11:16.000000 conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/conf_ini_g/catalog/specification/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.126196 conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     2267 2023-06-06 07:02:20.000000 conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     2472 2023-06-06 08:56:40.000000 conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     4619 2023-06-06 12:27:27.000000 conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/number.py
--rw-r--r--   0 eric      (1000) users      (984)     2929 2023-06-06 09:24:59.000000 conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/path.py
--rw-r--r--   0 eric      (1000) users      (984)     4289 2023-06-06 13:36:21.000000 conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.126196 conf-ini-g-2023.7/conf_ini_g/extension/
--rw-r--r--   0 eric      (1000) users      (984)     3078 2023-06-05 12:39:31.000000 conf-ini-g-2023.7/conf_ini_g/extension/path.py
--rw-r--r--   0 eric      (1000) users      (984)     3505 2023-06-28 10:57:28.000000 conf-ini-g-2023.7/conf_ini_g/extension/python.py
--rw-r--r--   0 eric      (1000) users      (984)     5501 2023-06-26 15:19:30.000000 conf-ini-g-2023.7/conf_ini_g/extension/string.py
--rw-r--r--   0 eric      (1000) users      (984)     7999 2023-06-28 10:58:44.000000 conf-ini-g-2023.7/conf_ini_g/extension/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.126196 conf-ini-g-2023.7/conf_ini_g/instance/
--rw-r--r--   0 eric      (1000) users      (984)    11085 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/instance/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.126196 conf-ini-g-2023.7/conf_ini_g/instance/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3335 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/instance/parameter/base.py
--rw-r--r--   0 eric      (1000) users      (984)     4385 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/instance/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     4108 2023-06-14 08:11:16.000000 conf-ini-g-2023.7/conf_ini_g/instance/parameter/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/conf_ini_g/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.126196 conf-ini-g-2023.7/conf_ini_g/interface/console/
--rw-r--r--   0 eric      (1000) users      (984)     1635 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/interface/console/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     6498 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/interface/console/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/interface/screen/
--rw-r--r--   0 eric      (1000) users      (984)     4500 2023-06-14 07:31:17.000000 conf-ini-g-2023.7/conf_ini_g/interface/screen/backend.py
--rw-r--r--   0 eric      (1000) users      (984)    16586 2023-06-14 14:16:41.000000 conf-ini-g-2023.7/conf_ini_g/interface/screen/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1945 2023-05-12 12:16:07.000000 conf-ini-g-2023.7/conf_ini_g/interface/screen/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/interface/screen/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     5655 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/interface/screen/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     7884 2023-06-14 13:10:38.000000 conf-ini-g-2023.7/conf_ini_g/interface/screen/parameter/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     8811 2023-06-14 14:12:59.000000 conf-ini-g-2023.7/conf_ini_g/interface/screen/section.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/interface/storage/
--rw-r--r--   0 eric      (1000) users      (984)     6515 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/interface/storage/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1577 2023-05-10 13:30:33.000000 conf-ini-g-2023.7/conf_ini_g/interface/storage/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/light/
--rw-r--r--   0 eric      (1000) users      (984)     4233 2023-06-06 15:18:55.000000 conf-ini-g-2023.7/conf_ini_g/light/config.py
--rw-r--r--   0 eric      (1000) users      (984)     3764 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/light/conversion.py
--rw-r--r--   0 eric      (1000) users      (984)     2595 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/light/ini.py
--rw-r--r--   0 eric      (1000) users      (984)     2071 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/light/xlsx.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/raw/
--rw-r--r--   0 eric      (1000) users      (984)     4519 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/raw/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/specification/
--rw-r--r--   0 eric      (1000) users      (984)     2820 2023-06-05 12:39:31.000000 conf-ini-g-2023.7/conf_ini_g/specification/base.py
--rw-r--r--   0 eric      (1000) users      (984)     7241 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/specification/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.129530 conf-ini-g-2023.7/conf_ini_g/specification/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     2500 2023-06-06 08:53:53.000000 conf-ini-g-2023.7/conf_ini_g/specification/parameter/annotation.py
--rw-r--r--   0 eric      (1000) users      (984)     4177 2023-06-14 14:12:58.000000 conf-ini-g-2023.7/conf_ini_g/specification/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     6127 2023-06-26 13:28:55.000000 conf-ini-g-2023.7/conf_ini_g/specification/parameter/type.py
--rw-r--r--   0 eric      (1000) users      (984)     3434 2023-06-05 14:27:55.000000 conf-ini-g-2023.7/conf_ini_g/specification/parameter/unit.py
--rw-r--r--   0 eric      (1000) users      (984)     2232 2023-05-31 14:26:58.000000 conf-ini-g-2023.7/conf_ini_g/specification/parameter/value.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.132863 conf-ini-g-2023.7/conf_ini_g/specification/section/
--rw-r--r--   0 eric      (1000) users      (984)     9488 2023-06-06 15:35:51.000000 conf-ini-g-2023.7/conf_ini_g/specification/section/main.py
--rw-r--r--   0 eric      (1000) users      (984)     1809 2023-05-12 12:45:21.000000 conf-ini-g-2023.7/conf_ini_g/specification/section/unit.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-06-28 10:58:57.000000 conf-ini-g-2023.7/conf_ini_g/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.119530 conf-ini-g-2023.7/conf_ini_g.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-06-28 11:01:47.000000 conf-ini-g-2023.7/conf_ini_g.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     3454 2023-06-28 11:01:47.000000 conf-ini-g-2023.7/conf_ini_g.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-06-28 11:01:47.000000 conf-ini-g-2023.7/conf_ini_g.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       14 2023-06-28 11:01:47.000000 conf-ini-g-2023.7/conf_ini_g.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       11 2023-06-28 11:01:47.000000 conf-ini-g-2023.7/conf_ini_g.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.116196 conf-ini-g-2023.7/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-28 11:01:47.132863 conf-ini-g-2023.7/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.7/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.7/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-06-28 11:01:47.132863 conf-ini-g-2023.7/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     6360 2023-06-26 12:16:56.000000 conf-ini-g-2023.7/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.191198 conf-ini-g-2023.8/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.8/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4428 2023-06-29 07:12:06.191198 conf-ini-g-2023.8/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.8/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.8/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.8/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/
+-rw-r--r--   0 eric      (1000) users      (984)     1779 2023-05-12 13:37:01.000000 conf-ini-g-2023.8/conf_ini_g/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/catalog/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.174532 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/
+-rw-r--r--   0 eric      (1000) users      (984)     2529 2023-06-14 07:31:54.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2346 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.174532 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
+-rw-r--r--   0 eric      (1000) users      (984)     1965 2023-06-02 15:09:21.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:29.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py
+-rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     2060 2023-05-31 13:36:33.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
+-rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 14:56:56.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.177865 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/
+-rw-r--r--   0 eric      (1000) users      (984)     2679 2023-06-14 07:32:27.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2344 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.177865 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py
+-rw-r--r--   0 eric      (1000) users      (984)     2010 2023-06-02 15:43:40.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:33.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py
+-rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     2059 2023-06-02 14:30:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py
+-rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 15:01:41.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.181198 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3631 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/boolean.py
+-rw-r--r--   0 eric      (1000) users      (984)     3814 2023-06-14 08:11:16.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     3859 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/directory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3387 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/multitype.py
+-rw-r--r--   0 eric      (1000) users      (984)     2222 2023-06-14 07:01:24.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/none.py
+-rw-r--r--   0 eric      (1000) users      (984)     6047 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     7923 2023-06-28 15:15:46.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)     2460 2023-06-14 08:11:16.000000 conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/catalog/specification/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.181198 conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     2267 2023-06-06 07:02:20.000000 conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/boolean.py
+-rw-r--r--   0 eric      (1000) users      (984)     2472 2023-06-06 08:56:40.000000 conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     4619 2023-06-06 12:27:27.000000 conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/number.py
+-rw-r--r--   0 eric      (1000) users      (984)     2929 2023-06-06 09:24:59.000000 conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     4289 2023-06-06 13:36:21.000000 conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.184532 conf-ini-g-2023.8/conf_ini_g/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     3078 2023-06-05 12:39:31.000000 conf-ini-g-2023.8/conf_ini_g/extension/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     3505 2023-06-28 10:57:28.000000 conf-ini-g-2023.8/conf_ini_g/extension/python.py
+-rw-r--r--   0 eric      (1000) users      (984)     5575 2023-06-29 06:37:51.000000 conf-ini-g-2023.8/conf_ini_g/extension/string.py
+-rw-r--r--   0 eric      (1000) users      (984)     8378 2023-06-28 13:43:01.000000 conf-ini-g-2023.8/conf_ini_g/extension/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.184532 conf-ini-g-2023.8/conf_ini_g/instance/
+-rw-r--r--   0 eric      (1000) users      (984)    11085 2023-06-28 14:04:38.000000 conf-ini-g-2023.8/conf_ini_g/instance/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.184532 conf-ini-g-2023.8/conf_ini_g/instance/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3353 2023-06-28 14:13:18.000000 conf-ini-g-2023.8/conf_ini_g/instance/parameter/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     4385 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/instance/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     4108 2023-06-14 08:11:16.000000 conf-ini-g-2023.8/conf_ini_g/instance/parameter/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/conf_ini_g/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.184532 conf-ini-g-2023.8/conf_ini_g/interface/console/
+-rw-r--r--   0 eric      (1000) users      (984)     1635 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/interface/console/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)     6498 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/interface/console/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.187865 conf-ini-g-2023.8/conf_ini_g/interface/screen/
+-rw-r--r--   0 eric      (1000) users      (984)     4500 2023-06-14 07:31:17.000000 conf-ini-g-2023.8/conf_ini_g/interface/screen/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)    16586 2023-06-28 14:07:17.000000 conf-ini-g-2023.8/conf_ini_g/interface/screen/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     1945 2023-05-12 12:16:07.000000 conf-ini-g-2023.8/conf_ini_g/interface/screen/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.187865 conf-ini-g-2023.8/conf_ini_g/interface/screen/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     5655 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/interface/screen/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     7884 2023-06-14 13:10:38.000000 conf-ini-g-2023.8/conf_ini_g/interface/screen/parameter/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     8811 2023-06-14 14:12:59.000000 conf-ini-g-2023.8/conf_ini_g/interface/screen/section.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.187865 conf-ini-g-2023.8/conf_ini_g/interface/storage/
+-rw-r--r--   0 eric      (1000) users      (984)     6515 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/interface/storage/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     1577 2023-05-10 13:30:33.000000 conf-ini-g-2023.8/conf_ini_g/interface/storage/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.187865 conf-ini-g-2023.8/conf_ini_g/light/
+-rw-r--r--   0 eric      (1000) users      (984)     4233 2023-06-06 15:18:55.000000 conf-ini-g-2023.8/conf_ini_g/light/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     3764 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/light/conversion.py
+-rw-r--r--   0 eric      (1000) users      (984)     2595 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/light/ini.py
+-rw-r--r--   0 eric      (1000) users      (984)     2071 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/light/xlsx.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.187865 conf-ini-g-2023.8/conf_ini_g/raw/
+-rw-r--r--   0 eric      (1000) users      (984)     4519 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/raw/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.187865 conf-ini-g-2023.8/conf_ini_g/specification/
+-rw-r--r--   0 eric      (1000) users      (984)     2820 2023-06-05 12:39:31.000000 conf-ini-g-2023.8/conf_ini_g/specification/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     7241 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/specification/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.191198 conf-ini-g-2023.8/conf_ini_g/specification/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     2500 2023-06-06 08:53:53.000000 conf-ini-g-2023.8/conf_ini_g/specification/parameter/annotation.py
+-rw-r--r--   0 eric      (1000) users      (984)     4177 2023-06-14 14:12:58.000000 conf-ini-g-2023.8/conf_ini_g/specification/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     6127 2023-06-26 13:28:55.000000 conf-ini-g-2023.8/conf_ini_g/specification/parameter/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     3437 2023-06-28 14:11:16.000000 conf-ini-g-2023.8/conf_ini_g/specification/parameter/unit.py
+-rw-r--r--   0 eric      (1000) users      (984)     2232 2023-05-31 14:26:58.000000 conf-ini-g-2023.8/conf_ini_g/specification/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.191198 conf-ini-g-2023.8/conf_ini_g/specification/section/
+-rw-r--r--   0 eric      (1000) users      (984)     9488 2023-06-06 15:35:51.000000 conf-ini-g-2023.8/conf_ini_g/specification/section/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     1809 2023-05-12 12:45:21.000000 conf-ini-g-2023.8/conf_ini_g/specification/section/unit.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-06-29 07:10:01.000000 conf-ini-g-2023.8/conf_ini_g/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.174532 conf-ini-g-2023.8/conf_ini_g.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4428 2023-06-29 07:12:06.000000 conf-ini-g-2023.8/conf_ini_g.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     3454 2023-06-29 07:12:06.000000 conf-ini-g-2023.8/conf_ini_g.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-06-29 07:12:06.000000 conf-ini-g-2023.8/conf_ini_g.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       14 2023-06-29 07:12:06.000000 conf-ini-g-2023.8/conf_ini_g.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       11 2023-06-29 07:12:06.000000 conf-ini-g-2023.8/conf_ini_g.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.171198 conf-ini-g-2023.8/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-29 07:12:06.191198 conf-ini-g-2023.8/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.8/documentation/wiki/description.asciidoc
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.8/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-06-29 07:12:06.191198 conf-ini-g-2023.8/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     6360 2023-06-26 12:16:56.000000 conf-ini-g-2023.8/setup.py
```

### Comparing `conf-ini-g-2023.7/PKG-INFO` & `conf-ini-g-2023.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.7
+Version: 2023.8
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf-ini-g-2023.7/README-COPYRIGHT-utf8.txt` & `conf-ini-g-2023.8/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/README-LICENCE-utf8.txt` & `conf-ini-g-2023.8/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/README.rst` & `conf-ini-g-2023.8/README.rst`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/__init__.py` & `conf-ini-g-2023.8/conf_ini_g/__init__.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/boolean.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/boolean.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/choices.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/choices.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/directory.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/directory.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/multitype.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/multitype.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/none.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/none.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/path.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/path.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/sequence.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/sequence.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     Cannot use slots (weak reference issue).
     """
 
     ENTRY_ANY: ClassVar[str] = "any"
     ENTRIES: ClassVar[tuple[str, ...]] = ("2", "3", "4", "5", "6", ENTRY_ANY)
 
     library_wgt: library_wgt_h
+    delimiters: str = None
     length_selector: choices_list_wgt_h = dtcl.field(init=False, default=None)
     components: tuple[text_wgt_h, ...] = dtcl.field(init=False, default=None)
 
     @classmethod
     def NewWithDetails(
         cls,
         value: tuple | None,
@@ -74,15 +75,23 @@
         If value_type does not contain the necessary details, a simple free-text input widget is used. If the value is not
         coherent with the details (which should not happen if value_type contains the necessary details and the value has
         been validated), a choice with the length of the value is added, with an exclamation point.
         """
         output = cls(library_wgt=backend.library_wgt_t())
 
         if value is None:
+            output.delimiters = "()"
             value = ()
+        elif isinstance(value, tuple):
+            output.delimiters = "()"
+        elif isinstance(value, list):
+            output.delimiters = "[]"
+        else:
+            raise TypeError(f"{type(value).__name__}: Unhandled sequence type.")
+
         length = value.__len__()
 
         default_parameters = (cls.ENTRIES, int(cls.ENTRIES[-2]))
         if value_type is None:
             entries, max_entry = default_parameters
         else:
             if isinstance(value_type, type_t):
@@ -164,19 +173,22 @@
                 break
             component_as_str = component.Text()
             if component_as_str.__len__() == 0:
                 break
             contents.append(component_as_str)
 
         if contents.__len__() == 0:
-            return "()"
+            return self.delimiters
         elif contents.__len__() == 1:
-            return "(" + contents[0] + ",)"
+            if self.delimiters[0] == "(":
+                return f"({contents[0]},)"
+            else:
+                return f"[{contents[0]}]"
         else:
-            return "(" + ", ".join(contents) + ")"
+            return self.delimiters[0] + ", ".join(contents) + self.delimiters[1]
 
 
 def _AdjustComponents(
     components: Sequence[text_wgt_h, ...],
     length: int,
 ) -> None:
     """"""
```

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/interface/screen/parameter/text.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/interface/screen/parameter/text.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/boolean.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/boolean.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/choices.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/choices.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/number.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/number.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/path.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/path.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/catalog/specification/parameter/sequence.py` & `conf-ini-g-2023.8/conf_ini_g/catalog/specification/parameter/sequence.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/extension/path.py` & `conf-ini-g-2023.8/conf_ini_g/extension/path.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/extension/python.py` & `conf-ini-g-2023.8/conf_ini_g/extension/python.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/extension/string.py` & `conf-ini-g-2023.8/conf_ini_g/extension/string.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,17 +117,14 @@
         value = string
 
     return value, True
 
 
 def _AsInterpretedObject(string: str, expected_type: type, /) -> tuple[Any, bool]:
     """"""
-    # TODO: Somewhere, maybe here, a string representation of a path is compared with
-    #     the original string. If there is a trailing /, then there is a mismatch. E.g.,
-    #     str(path(/etc/)) is probably "/etc".
     failed_interpretation = None, False
     lowered = string.lower()
 
     if expected_type is EXPECTS_NONE:
         return None, (lowered == "none")
 
     if expected_type is bool:
@@ -146,15 +143,21 @@
     # The expected type might be instantiable from a string, e.g.: float("1.0").
     # However, a success does not mean that the interpretation is valid, e.g.:
     # tuple("(1, 2, 3)"). To confirm that a success is indeed a correct interpretation,
     # the string representation of the interpreted value is compared with the string.
     # This is not a perfect test, so "literal_eval" might still be called below.
     try:
         value = expected_type(string)
-        success = str(value).replace(" ", "") == string.replace(" ", "")
+        # If "expected_type" is a path and the consolidated value has a trailing folder
+        # separator, then the general-purpose test fails. Hence the specialized
+        # test below.
+        if issubclass(expected_type, path_t):
+            success = value.match(string)
+        else:
+            success = str(value).replace(" ", "") == string.replace(" ", "")
     except:
         value, success = failed_interpretation
     if success:
         return value, True
 
     try:
         value = bstr.literal_eval(string)
```

### Comparing `conf-ini-g-2023.7/conf_ini_g/extension/type.py` & `conf-ini-g-2023.8/conf_ini_g/extension/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
+from pathlib import Path as path_t
 from types import EllipsisType, GenericAlias, NoneType, UnionType
 from typing import Annotated, Any, Iterable, Sequence, get_args, get_origin
 
-from conf_ini_g.extension.python import SpecificationPath
+# from conf_ini_g.extension.python import SpecificationPath
 
 complex_hint_h = GenericAlias | UnionType
 raw_hint_h = type | Any | complex_hint_h
 annotated_hint_t = type(Annotated[object, None])
 any_hint_h = raw_hint_h | annotated_hint_t
 
 
@@ -195,17 +196,23 @@
             return True
         else:
             return False
 
     if not isinstance(value_node.consolidated, hn_type):
         try:
             converted = hn_type(value_node.consolidated)
-            success = str(converted).replace(" ", "") == str(
-                value_node.consolidated
-            ).replace(" ", "")
+            # If "hn_type" is a path and the consolidated value has a trailing folder
+            # separator, then the general-purpose test fails. Hence the specialized
+            # test below.
+            if issubclass(hn_type, path_t):
+                success = converted.match(str(value_node.consolidated))
+            else:
+                success = str(converted).replace(" ", "") == str(
+                    value_node.consolidated
+                ).replace(" ", "")
         except:
             success = False
         if not success:
             return False
     if (value_node.elements is None) and (hn_elements is None):
         value_node.type = hn_type
         return True
```

### Comparing `conf-ini-g-2023.7/conf_ini_g/instance/config.py` & `conf-ini-g-2023.8/conf_ini_g/instance/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/instance/parameter/base.py` & `conf-ini-g-2023.8/conf_ini_g/instance/parameter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,13 +96,13 @@
     if from_left:
         where_separator = combined.find(separator)
     else:
         where_separator = combined.rfind(separator)
 
     if where_separator != -1:
         left = combined[:where_separator].strip()
-        right = combined[(where_separator + 1) :].strip()
+        right = combined[(where_separator + separator.__len__()) :].strip()
     else:
         left = combined
         right = None
 
     return left, right
```

### Comparing `conf-ini-g-2023.7/conf_ini_g/instance/parameter/main.py` & `conf-ini-g-2023.8/conf_ini_g/instance/parameter/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/instance/parameter/unit.py` & `conf-ini-g-2023.8/conf_ini_g/instance/parameter/unit.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/console/__init__.py` & `conf-ini-g-2023.8/conf_ini_g/interface/console/__init__.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/console/config.py` & `conf-ini-g-2023.8/conf_ini_g/interface/console/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/screen/backend.py` & `conf-ini-g-2023.8/conf_ini_g/interface/screen/backend.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/screen/config.py` & `conf-ini-g-2023.8/conf_ini_g/interface/screen/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/screen/generic.py` & `conf-ini-g-2023.8/conf_ini_g/interface/screen/generic.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/screen/parameter/main.py` & `conf-ini-g-2023.8/conf_ini_g/interface/screen/parameter/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/screen/parameter/path_chooser.py` & `conf-ini-g-2023.8/conf_ini_g/interface/screen/parameter/path_chooser.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/screen/section.py` & `conf-ini-g-2023.8/conf_ini_g/interface/screen/section.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/storage/config.py` & `conf-ini-g-2023.8/conf_ini_g/interface/storage/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/interface/storage/constant.py` & `conf-ini-g-2023.8/conf_ini_g/interface/storage/constant.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/light/config.py` & `conf-ini-g-2023.8/conf_ini_g/light/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/light/conversion.py` & `conf-ini-g-2023.8/conf_ini_g/light/conversion.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/light/ini.py` & `conf-ini-g-2023.8/conf_ini_g/light/ini.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/light/xlsx.py` & `conf-ini-g-2023.8/conf_ini_g/light/xlsx.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/raw/config.py` & `conf-ini-g-2023.8/conf_ini_g/raw/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/base.py` & `conf-ini-g-2023.8/conf_ini_g/specification/base.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/config.py` & `conf-ini-g-2023.8/conf_ini_g/specification/config.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/parameter/annotation.py` & `conf-ini-g-2023.8/conf_ini_g/specification/parameter/annotation.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/parameter/main.py` & `conf-ini-g-2023.8/conf_ini_g/specification/parameter/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/parameter/type.py` & `conf-ini-g-2023.8/conf_ini_g/specification/parameter/type.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/parameter/unit.py` & `conf-ini-g-2023.8/conf_ini_g/specification/parameter/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 import dataclasses as dtcl
 from math import pi as PI
 
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.type import type_t
 
-UNIT_SEPARATOR = "'"
+UNIT_SEPARATOR = ":IN:"
 
 _STD_UNIT_CONVERSIONS = (
     # unit, unit name, parent unit (None if none), conversion factor (1.0 if None)
     ("si", "site", None, 1.0),  # Synonym for sample, pixel, voxel...
     #
     ("km", "kilometer", "m", 1000.0),
     ("m", "meter", "si", 1.0),
```

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/parameter/value.py` & `conf-ini-g-2023.8/conf_ini_g/specification/parameter/value.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/section/main.py` & `conf-ini-g-2023.8/conf_ini_g/specification/section/main.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/specification/section/unit.py` & `conf-ini-g-2023.8/conf_ini_g/specification/section/unit.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/conf_ini_g/version.py` & `conf-ini-g-2023.8/conf_ini_g/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.7"
+__version__ = "2023.8"
```

### Comparing `conf-ini-g-2023.7/conf_ini_g.egg-info/PKG-INFO` & `conf-ini-g-2023.8/conf_ini_g.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.7
+Version: 2023.8
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf-ini-g-2023.7/conf_ini_g.egg-info/SOURCES.txt` & `conf-ini-g-2023.8/conf_ini_g.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/documentation/wiki/description.asciidoc` & `conf-ini-g-2023.8/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.7/setup.py` & `conf-ini-g-2023.8/setup.py`

 * *Files identical despite different names*

