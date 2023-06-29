# Comparing `tmp/nbdev-mkdocs-0.6.0rc0.tar.gz` & `tmp/nbdev-mkdocs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-mkdocs-0.6.0rc0.tar", last modified: Thu Jun 29 09:12:09 2023, max compression
+gzip compressed data, was "nbdev-mkdocs-1.0.0.tar", last modified: Mon Jan 30 10:41:28 2023, max compression
```

## Comparing `nbdev-mkdocs-0.6.0rc0.tar` & `nbdev-mkdocs-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,50 @@
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.665451 nbdev-mkdocs-0.6.0rc0/
--rw-r--r--   0 harishm    (501) staff       (20)    11337 2022-11-21 23:54:00.000000 nbdev-mkdocs-0.6.0rc0/LICENSE
--rw-r--r--   0 harishm    (501) staff       (20)      143 2022-11-21 23:54:00.000000 nbdev-mkdocs-0.6.0rc0/MANIFEST.in
--rw-r--r--   0 harishm    (501) staff       (20)    10468 2023-06-29 09:12:09.665229 nbdev-mkdocs-0.6.0rc0/PKG-INFO
--rw-r--r--   0 harishm    (501) staff       (20)     9658 2023-03-15 13:12:41.000000 nbdev-mkdocs-0.6.0rc0/README.md
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.660298 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/
--rw-r--r--   0 harishm    (501) staff       (20)       25 2023-06-27 00:59:34.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/__init__.py
--rw-r--r--   0 harishm    (501) staff       (20)    13112 2023-06-29 09:10:47.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_cli.py
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.662349 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/
--rw-r--r--   0 harishm    (501) staff       (20)        0 2023-06-27 00:59:34.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/__init__.py
--rw-r--r--   0 harishm    (501) staff       (20)     7347 2023-06-27 00:59:33.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/api_docs_helper.py
--rw-r--r--   0 harishm    (501) staff       (20)     8620 2023-06-27 00:59:33.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/cli_doc.py
--rw-r--r--   0 harishm    (501) staff       (20)     7498 2023-06-27 00:59:33.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/doc_links_utils.py
--rw-r--r--   0 harishm    (501) staff       (20)     7348 2023-06-27 00:59:34.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/quarto_to_mkdocs.py
--rw-r--r--   0 harishm    (501) staff       (20)     3666 2023-06-27 00:59:34.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/utils.py
--rw-r--r--   0 harishm    (501) staff       (20)    26061 2023-06-29 09:10:47.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_modidx.py
--rw-r--r--   0 harishm    (501) staff       (20)      784 2023-06-27 00:59:34.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_package_data.py
--rw-r--r--   0 harishm    (501) staff       (20)      965 2023-06-27 00:59:34.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_testing.py
--rw-r--r--   0 harishm    (501) staff       (20)     8842 2023-06-27 00:59:33.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/docstring.py
--rw-r--r--   0 harishm    (501) staff       (20)    45766 2023-06-29 09:10:47.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/mkdocs.py
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.663553 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/
--rw-r--r--   0 harishm    (501) staff       (20)      375 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/changelog_not_found.md
--rw-r--r--   0 harishm    (501) staff       (20)      383 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/cli_commands_not_found.md
--rw-r--r--   0 harishm    (501) staff       (20)     1761 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/custom-social-image-template.html
--rw-r--r--   0 harishm    (501) staff       (20)      242 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/ghp_deploy_action_template.yml
--rw-r--r--   0 harishm    (501) staff       (20)       40 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/gitignore.txt
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.657186 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.657130 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.663686 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/css/
--rw-r--r--   0 harishm    (501) staff       (20)      883 2023-06-01 07:27:35.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/css/extra.css
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.664064 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/
--rw-r--r--   0 harishm    (501) staff       (20)     1085 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/compass-outline.png
--rw-r--r--   0 harishm    (501) staff       (20)   108442 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/default_social_logo.png
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.664700 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/js/
--rw-r--r--   0 harishm    (501) staff       (20)        0 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/js/extra.js
--rw-r--r--   0 harishm    (501) staff       (20)      302 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/js/mathjax.js
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.664845 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/
--rw-r--r--   0 harishm    (501) staff       (20)     1272 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/main.html
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.664993 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/partials/
--rw-r--r--   0 harishm    (501) staff       (20)      478 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/partials/copyright.html
--rw-r--r--   0 harishm    (501) staff       (20)     2442 2023-05-31 09:25:16.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template.yml
--rw-r--r--   0 harishm    (501) staff       (20)    10993 2023-06-29 09:10:47.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/social_image_generator.py
-drwxr-xr-x   0 harishm    (501) staff       (20)        0 2023-06-29 09:12:09.661269 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/
--rw-r--r--   0 harishm    (501) staff       (20)    10468 2023-06-29 09:12:09.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/PKG-INFO
--rw-r--r--   0 harishm    (501) staff       (20)     1574 2023-06-29 09:12:09.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/SOURCES.txt
--rw-r--r--   0 harishm    (501) staff       (20)        1 2023-06-29 09:12:09.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/dependency_links.txt
--rw-r--r--   0 harishm    (501) staff       (20)      104 2023-06-29 09:12:09.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/entry_points.txt
--rw-r--r--   0 harishm    (501) staff       (20)        1 2023-03-14 05:40:07.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/not-zip-safe
--rw-r--r--   0 harishm    (501) staff       (20)      495 2023-06-29 09:12:09.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/requires.txt
--rw-r--r--   0 harishm    (501) staff       (20)       13 2023-06-29 09:12:09.000000 nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/top_level.txt
--rw-r--r--   0 harishm    (501) staff       (20)     1801 2023-06-26 11:52:11.000000 nbdev-mkdocs-0.6.0rc0/settings.ini
--rw-r--r--   0 harishm    (501) staff       (20)       38 2023-06-29 09:12:09.665501 nbdev-mkdocs-0.6.0rc0/setup.cfg
--rw-r--r--   0 harishm    (501) staff       (20)     2828 2023-06-09 07:57:01.000000 nbdev-mkdocs-0.6.0rc0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/
+-rw-r--r--   0 davor     (1000) davor     (1000)    11337 2022-11-09 14:02:03.000000 nbdev-mkdocs-1.0.0/LICENSE
+-rw-r--r--   0 davor     (1000) davor     (1000)      143 2022-11-09 14:02:03.000000 nbdev-mkdocs-1.0.0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10228 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9391 2023-01-27 09:12:44.000000 nbdev-mkdocs-1.0.0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/
+-rw-rw-r--   0 davor     (1000) davor     (1000)       22 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9839 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_cli.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_helpers/
+-rw-r--r--   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_helpers/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     8621 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_helpers/cli_doc.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3124 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_helpers/utils.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    16252 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_modidx.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      784 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_package_data.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      965 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/_testing.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     8856 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/docstring.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    39285 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/mkdocs.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      375 2022-12-23 10:19:05.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/changelog_not_found.md
+-rw-rw-r--   0 davor     (1000) davor     (1000)      383 2022-12-23 10:19:05.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/cli_commands_not_found.md
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1761 2022-12-23 10:19:05.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/custom-social-image-template.html
+-rw-r--r--   0 davor     (1000) davor     (1000)      242 2022-12-02 14:11:59.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/ghp_deploy_action_template.yml
+-rw-r--r--   0 davor     (1000) davor     (1000)       40 2022-12-02 14:11:59.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/gitignore.txt
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.430825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.430825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/css/
+-rw-r--r--   0 davor     (1000) davor     (1000)        0 2022-12-02 14:11:59.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/css/extra.css
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/
+-rw-r--r--   0 davor     (1000) davor     (1000)     1085 2022-12-02 14:11:59.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/compass-outline.png
+-rw-rw-r--   0 davor     (1000) davor     (1000)   108442 2022-12-12 08:01:53.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/default_social_logo.png
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/js/
+-rw-r--r--   0 davor     (1000) davor     (1000)        0 2022-12-02 14:11:59.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/js/extra.js
+-rw-rw-r--   0 davor     (1000) davor     (1000)      302 2022-12-23 10:19:05.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/js/mathjax.js
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/
+-rw-r--r--   0 davor     (1000) davor     (1000)     1100 2022-12-13 11:47:19.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/main.html
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/partials/
+-rw-r--r--   0 davor     (1000) davor     (1000)      478 2022-12-13 11:47:19.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/site_overrides/partials/copyright.html
+-rw-r--r--   0 davor     (1000) davor     (1000)     2412 2023-01-04 15:10:06.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template.yml
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10924 2023-01-30 10:41:04.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs/social_image_generator.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/
+-rw-r--r--   0 davor     (1000) davor     (1000)    10228 2023-01-30 10:41:28.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/PKG-INFO
+-rw-r--r--   0 davor     (1000) davor     (1000)     1450 2023-01-30 10:41:28.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-01-30 10:41:28.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)      103 2023-01-30 10:41:28.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/entry_points.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-01 06:53:34.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/not-zip-safe
+-rw-r--r--   0 davor     (1000) davor     (1000)      414 2023-01-30 10:41:28.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/requires.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       13 2023-01-30 10:41:28.000000 nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1588 2023-01-30 10:40:56.000000 nbdev-mkdocs-1.0.0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-01-30 10:41:28.434825 nbdev-mkdocs-1.0.0/setup.cfg
+-rw-r--r--   0 davor     (1000) davor     (1000)     2805 2023-01-23 12:03:13.000000 nbdev-mkdocs-1.0.0/setup.py
```

### Comparing `nbdev-mkdocs-0.6.0rc0/LICENSE` & `nbdev-mkdocs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-mkdocs-0.6.0rc0/PKG-INFO` & `nbdev-mkdocs-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nbdev-mkdocs
-Version: 0.6.0rc0
+Version: 1.0.0
 Summary: Extension of nbdev for generating documentation using Material for Mkdocs instead of Quarto
 Home-page: https://github.com/airtai/nbdev-mkdocs
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python mkdocs material
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Material for nbdev
 ================
 
@@ -237,28 +237,25 @@
     ╭─ Options ────────────────────────────────────────────────────────────────────╮
     │ --install-completion          Install completion for the current shell.      │
     │ --show-completion             Show completion for the current shell, to copy │
     │                               it or customize the installation.              │
     │ --help                        Show this message and exit.                    │
     ╰──────────────────────────────────────────────────────────────────────────────╯
     ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-    │ delete-pre-release-docs  Deletes deployed pre-release documentation          │
-    │                          versions.                                           │
-    │ docs                     Prepares files in **mkdocs/docs** and then runs     │
-    │                          **mkdocs build** command on them                    │
-    │ docstring                Command for adding docstrings to classes and        │
-    │                          methods that don't have one using docstring-gen     │
-    │                          library.                                            │
-    │ new                      Creates files in **mkdocs** subdirectory needed for │
-    │                          other **nbdev_mkdocs** subcommands                  │
-    │ prepare                  Runs tests and prepares files in **mkdocs/docs**    │
-    │                          and then runs **mkdocs build** command on them      │
-    │ preview                  Prepares files in **mkdocs/docs** and then runs     │
-    │                          **mkdocs serve** command on them                    │
-    │ social-image             Command for generating a custom social share image. │
+    │ docs          Prepares files in **mkdocs/docs** and then runs **mkdocs       │
+    │               build** command on them                                        │
+    │ docstring     Command for adding docstrings to classes and methods that      │
+    │               don't have one using docstring-gen library.                    │
+    │ new           Creates files in **mkdocs** subdirectory needed for other      │
+    │               **nbdev_mkdocs** subcommands                                   │
+    │ prepare       Runs tests and prepares files in **mkdocs/docs** and then runs │
+    │               **mkdocs build** command on them                               │
+    │ preview       Prepares files in **mkdocs/docs** and then runs **mkdocs       │
+    │               serve** command on them                                        │
+    │ social-image  Command for generating a custom social share image.            │
     ╰──────────────────────────────────────────────────────────────────────────────╯
 
 #### Setup
 
 After installing nbdev-mkdocs, bootstrap your project documentation by
 executing the following command from the project’s root directory:
 
@@ -311,9 +308,7 @@
 
 Copyright © 2022 onwards airt technologies ltd, Inc.
 
 ## License
 
 This project is licensed under the terms of the [Apache License
 2.0](https://github.com/airtai/nbdev-mkdocs/blob/main/LICENSE)
-
-
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: nbdev-mkdocs Version: 0.6.0rc0 Summary: Extension
-of nbdev for generating documentation using Material for Mkdocs instead of
-Quarto Home-page: https://github.com/airtai/nbdev-mkdocs Author: airt Author-
-email: info@airt.ai License: Apache Software License 2.0 Keywords: nbdev
-jupyter notebook python mkdocs material Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
-Apache Software License Requires-Python: >=3.8 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE Material for nbdev
-================  ![](https://raw.githubusercontent.com/airtai/nbdev-mkdocs/
-main/nbs/images/nbdev_mkdocs_banner_img.png) ----------------------------------
--------------------------------------- **Documentation**: https://nbdev-
-mkdocs.airt.ai **Source Code**: https://github.com/airtai/nbdev-mkdocs --------
----------------------------------------------------------------- ## Getting
-Started ![PyPI](https://img.shields.io/pypi/v/nbdev-mkdocs.png) ![PyPI -
-Downloads](https://img.shields.io/pypi/dm/nbdev-mkdocs.png) ![PyPI - Python
-Version](https://img.shields.io/pypi/pyversions/nbdev-mkdocs.png) ![GitHub
-Workflow Status](https://img.shields.io/github/actions/workflow/status/airtai/
-nbdev-mkdocs/test.yaml) ![CodeQL](https://github.com/airtai/nbdev-mkdocs/
-actions/workflows/codeql.yml/badge.svg) ![Dependency Review](https://
-github.com/airtai/nbdev-mkdocs/actions/workflows/dependency-review.yml/
-badge.svg) ![GitHub](https://img.shields.io/github/license/airtai/nbdev-
-mkdocs.png) -------------------------------------------------------------------
------ **Material for nbdev** is a nbdev extension that allows you to use
-Material_for_MkDocs to generate documentation for nbdev projects. The key
-features are: - **Material style documentation**: Effortlessly create material
-style documentation for your nbdev projects with Material for MkDocs, a theme
-that provides a sleek and modern design for your documentation. - **Auto
-generate docstrings**: Instantly generate docstrings for your Python code using
-docstring-gen library, a tool that automatically generates docstrings for your
-functions and classes using Codex. - **Create stunning social media share
-images**: Boost your projectâs visibility by creating striking social share
-images using DALL-E. - **Customizability**: Add guides, release notes,
-customise the navigation menu and configure the Material for MkDocs easily to
-suit your project needs. With this documentation tool, you have more control
-over the look and feel of your documentation, allowing you to create a unique
-and personalized experience for your users. ### Workflow Hereâs a quick
-comparison of Quarto and Material for nbdev development workflows:
+Metadata-Version: 2.1 Name: nbdev-mkdocs Version: 1.0.0 Summary: Extension of
+nbdev for generating documentation using Material for Mkdocs instead of Quarto
+Home-page: https://github.com/airtai/nbdev-mkdocs Author: airt Author-email:
+info@airt.ai License: Apache Software License 2.0 Keywords: nbdev jupyter
+notebook python mkdocs material Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+License :: OSI Approved :: Apache Software License Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE Material for nbdev ================  ![](https://
+raw.githubusercontent.com/airtai/nbdev-mkdocs/main/nbs/images/
+nbdev_mkdocs_banner_img.png) --------------------------------------------------
+---------------------- **Documentation**: https://nbdev-mkdocs.airt.ai **Source
+Code**: https://github.com/airtai/nbdev-mkdocs --------------------------------
+---------------------------------------- ## Getting Started ![PyPI](https://
+img.shields.io/pypi/v/nbdev-mkdocs.png) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/nbdev-mkdocs.png) ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/nbdev-mkdocs.png) ![GitHub Workflow Status]
+(https://img.shields.io/github/actions/workflow/status/airtai/nbdev-mkdocs/
+test.yaml) ![CodeQL](https://github.com/airtai/nbdev-mkdocs/actions/workflows/
+codeql.yml/badge.svg) ![Dependency Review](https://github.com/airtai/nbdev-
+mkdocs/actions/workflows/dependency-review.yml/badge.svg) ![GitHub](https://
+img.shields.io/github/license/airtai/nbdev-mkdocs.png) ------------------------
+------------------------------------------------ **Material for nbdev** is a
+nbdev extension that allows you to use Material_for_MkDocs to generate
+documentation for nbdev projects. The key features are: - **Material style
+documentation**: Effortlessly create material style documentation for your
+nbdev projects with Material for MkDocs, a theme that provides a sleek and
+modern design for your documentation. - **Auto generate docstrings**: Instantly
+generate docstrings for your Python code using docstring-gen library, a tool
+that automatically generates docstrings for your functions and classes using
+Codex. - **Create stunning social media share images**: Boost your projectâs
+visibility by creating striking social share images using DALL-E. -
+**Customizability**: Add guides, release notes, customise the navigation menu
+and configure the Material for MkDocs easily to suit your project needs. With
+this documentation tool, you have more control over the look and feel of your
+documentation, allowing you to create a unique and personalized experience for
+your users. ### Workflow Hereâs a quick comparison of Quarto and Material for
+nbdev development workflows:
 Quarto workflow                                      Material for nbdev workflow
 Install: ``` shell $ pip install notebook nbdev $    Install: ``` shell $ pip install notebook nbdev $
 nbdev_install_quarto ```                             nbdev_install_quarto $ pip install nbdev-mkdocs ```
 Setup: ``` shell $ nbdev_new $ nbdev_install_hooks $ Setup: ``` shell $ nbdev_new $ nbdev_install_hooks $ vi
 vi settings.ini $ pip install -e '.[dev]' ```        settings.ini $ pip install -e '.[dev]' $ nbdev_mkdocs
                                                      new $ vi mkdocs/mkdocs.yml ```
 Development: ``` shell # Edit files $ nbdev_preview  Development: ``` shell # Edit files $ nbdev_mkdocs
@@ -62,24 +63,23 @@
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --install-completion Install completion for the current shell. â â --
 show-completion Show completion for the current shell, to copy â â it or
 customize the installation. â â --help Show this message and exit. â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 â­â Commands
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
-â delete-pre-release-docs Deletes deployed pre-release documentation â â
-versions. â â docs Prepares files in **mkdocs/docs** and then runs â â
-**mkdocs build** command on them â â docstring Command for adding
-docstrings to classes and â â methods that don't have one using docstring-
-gen â â library. â â new Creates files in **mkdocs** subdirectory
-needed for â â other **nbdev_mkdocs** subcommands â â prepare Runs
-tests and prepares files in **mkdocs/docs** â â and then runs **mkdocs
-build** command on them â â preview Prepares files in **mkdocs/docs** and
-then runs â â **mkdocs serve** command on them â â social-image Command
-for generating a custom social share image. â
+â docs Prepares files in **mkdocs/docs** and then runs **mkdocs â â
+build** command on them â â docstring Command for adding docstrings to
+classes and methods that â â don't have one using docstring-gen library.
+â â new Creates files in **mkdocs** subdirectory needed for other â â
+**nbdev_mkdocs** subcommands â â prepare Runs tests and prepares files in
+**mkdocs/docs** and then runs â â **mkdocs build** command on them â â
+preview Prepares files in **mkdocs/docs** and then runs **mkdocs â â
+serve** command on them â â social-image Command for generating a custom
+social share image. â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 #### Setup After installing nbdev-mkdocs, bootstrap your project documentation
 by executing the following command from the projectâs root directory: ```
 shell nbdev_mkdocs new ``` Using information from the projectâs settings.ini
 file, the above command creates files and directories required to build the
 documentation and saves it in the **mkdocs** subdirectory. Note: You should
 only run the **nbdev_mkdocs new** command once for the project to initialise
```

### Comparing `nbdev-mkdocs-0.6.0rc0/README.md` & `nbdev-mkdocs-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -215,28 +215,25 @@
     ╭─ Options ────────────────────────────────────────────────────────────────────╮
     │ --install-completion          Install completion for the current shell.      │
     │ --show-completion             Show completion for the current shell, to copy │
     │                               it or customize the installation.              │
     │ --help                        Show this message and exit.                    │
     ╰──────────────────────────────────────────────────────────────────────────────╯
     ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-    │ delete-pre-release-docs  Deletes deployed pre-release documentation          │
-    │                          versions.                                           │
-    │ docs                     Prepares files in **mkdocs/docs** and then runs     │
-    │                          **mkdocs build** command on them                    │
-    │ docstring                Command for adding docstrings to classes and        │
-    │                          methods that don't have one using docstring-gen     │
-    │                          library.                                            │
-    │ new                      Creates files in **mkdocs** subdirectory needed for │
-    │                          other **nbdev_mkdocs** subcommands                  │
-    │ prepare                  Runs tests and prepares files in **mkdocs/docs**    │
-    │                          and then runs **mkdocs build** command on them      │
-    │ preview                  Prepares files in **mkdocs/docs** and then runs     │
-    │                          **mkdocs serve** command on them                    │
-    │ social-image             Command for generating a custom social share image. │
+    │ docs          Prepares files in **mkdocs/docs** and then runs **mkdocs       │
+    │               build** command on them                                        │
+    │ docstring     Command for adding docstrings to classes and methods that      │
+    │               don't have one using docstring-gen library.                    │
+    │ new           Creates files in **mkdocs** subdirectory needed for other      │
+    │               **nbdev_mkdocs** subcommands                                   │
+    │ prepare       Runs tests and prepares files in **mkdocs/docs** and then runs │
+    │               **mkdocs build** command on them                               │
+    │ preview       Prepares files in **mkdocs/docs** and then runs **mkdocs       │
+    │               serve** command on them                                        │
+    │ social-image  Command for generating a custom social share image.            │
     ╰──────────────────────────────────────────────────────────────────────────────╯
 
 #### Setup
 
 After installing nbdev-mkdocs, bootstrap your project documentation by
 executing the following command from the project’s root directory:
```

#### html2text {}

```diff
@@ -51,24 +51,23 @@
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --install-completion Install completion for the current shell. â â --
 show-completion Show completion for the current shell, to copy â â it or
 customize the installation. â â --help Show this message and exit. â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 â­â Commands
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
-â delete-pre-release-docs Deletes deployed pre-release documentation â â
-versions. â â docs Prepares files in **mkdocs/docs** and then runs â â
-**mkdocs build** command on them â â docstring Command for adding
-docstrings to classes and â â methods that don't have one using docstring-
-gen â â library. â â new Creates files in **mkdocs** subdirectory
-needed for â â other **nbdev_mkdocs** subcommands â â prepare Runs
-tests and prepares files in **mkdocs/docs** â â and then runs **mkdocs
-build** command on them â â preview Prepares files in **mkdocs/docs** and
-then runs â â **mkdocs serve** command on them â â social-image Command
-for generating a custom social share image. â
+â docs Prepares files in **mkdocs/docs** and then runs **mkdocs â â
+build** command on them â â docstring Command for adding docstrings to
+classes and methods that â â don't have one using docstring-gen library.
+â â new Creates files in **mkdocs** subdirectory needed for other â â
+**nbdev_mkdocs** subcommands â â prepare Runs tests and prepares files in
+**mkdocs/docs** and then runs â â **mkdocs build** command on them â â
+preview Prepares files in **mkdocs/docs** and then runs **mkdocs â â
+serve** command on them â â social-image Command for generating a custom
+social share image. â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 #### Setup After installing nbdev-mkdocs, bootstrap your project documentation
 by executing the following command from the projectâs root directory: ```
 shell nbdev_mkdocs new ``` Using information from the projectâs settings.ini
 file, the above command creates files and directories required to build the
 documentation and saves it in the **mkdocs** subdirectory. Note: You should
 only run the **nbdev_mkdocs new** command once for the project to initialise
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_cli.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/CLI.ipynb.
 
 # %% auto 0
-__all__ = ['new', 'prepare', 'preview', 'docs', 'delete_pre_release_docs']
+__all__ = ['new', 'prepare', 'preview', 'docs']
 
 # %% ../nbs/CLI.ipynb 1
-import subprocess  # nosec: B404
 from asyncio import run as aiorun
 from pathlib import Path
 from typing import *
 
 import typer
 from docstring_gen.docstring_generator import add_docstring_to_source
 from nbdev.config import get_config
@@ -47,29 +46,19 @@
 @_app.command(
     help="Prepares files in **mkdocs/docs** and then runs **mkdocs serve** command on them ",
 )
 def preview(
     root_path: str = typer.Option(
         ".", help="path under which mkdocs directory will be created"
     ),
-    use_relative_doc_links: bool = typer.Option(
-        True,
-        "--use-relative-doc-links/--use-host-doc-links",
-        help="If set to --use-relative-doc-links, relative links are added to symbol references in "
-        "generated documentation. If set to --use-host-doc-links, the value set in doc_host in settings.ini is added to symbol references in generated documentation.",
-    ),
     port: int = typer.Option(4000, help="port to use"),
 ) -> None:
     """CLI command for creating files for nbdev_mkdocs command"""
     try:
-        nbdev_mkdocs.mkdocs.preview(
-            root_path=root_path,
-            use_relative_doc_links=use_relative_doc_links,
-            port=port,
-        )
+        nbdev_mkdocs.mkdocs.preview(root_path=root_path, port=port)
     except Exception as e:
         typer.secho(f"Unexpected internal error: {e}", err=True, fg=typer.colors.RED)
         raise typer.Exit(1)
 
 
 @_app.command(
     help="Prepares files in **mkdocs/docs** and then runs **mkdocs build** command on them ",
@@ -96,19 +85,19 @@
         root_path: str = typer.Option(".", help="Project's root path."),
         generator: nbdev_mkdocs.social_image_generator._IMG_Generator = typer.Option(
             "file",
             help="Generator to use to create the social image. Valid options are: 'file' and 'dall_e'. Choose 'file' if you want to use an existing image from your local machine in the social share image.",
         ),
         prompt: str = typer.Option(
             "Cute animal wearing hoodie sitting in high chair in purple room, browsing computer, 3d render",
-            help="The prompt to use for generating the image. Please pass this option only when using 'dall_e' as the generator.",
+            help="The prompt to use for generating the image.",
         ),
         image_path: Optional[str] = typer.Option(
             None,
-            help="Image file path to use in the social share image. Use images with a 1:1 aspect ratio and at least 512x512 pixels for the best results. If None, then the default image will be used. Please pass this option only when using 'file' as the generator.",
+            help="Image file path to use in the social share image. Use images with a 1:1 aspect ratio and at least 512x512 pixels for the best results. If None, then the default image will be used.",
         ),
     ) -> None:
         """CLI command for generating a custom social share image"""
 
         async def _generate_social_image(
             root_path: str, generator: str, prompt: str, image_path: Optional[str]
         ) -> None:
@@ -159,22 +148,22 @@
         recreate_auto_gen_docs: bool = typer.Option(
             False,
             "--force-recreate-auto-generated",
             "-f",
             help="If set to True, the autogenerated docstrings from the previous runs will be replaced with the new one.",
         ),
         model: str = typer.Option(
-            "gpt-3.5-turbo",
-            help="The name of the OpenAI model that will be used to generate docstrings.",
+            "code-davinci-002",
+            help="The name of the Codex model that will be used to generate docstrings.",
         ),
         temperature: float = typer.Option(
             0.2,
             help="Setting the temperature close to zero produces better results, whereas higher temperatures produce more complex, and sometimes irrelevant docstrings.",
             min=0.0,
-            max=2.0,
+            max=1.0,
         ),
         max_tokens: int = typer.Option(
             250,
             help="The maximum number of tokens to be used when generating a docstring for a function or class. Please note that a higher number will deplete your token quota faster.",
         ),
         top_p: float = typer.Option(
             1.0,
@@ -183,14 +172,15 @@
             max=1.0,
         ),
         n: int = typer.Option(
             3,
             help="The number of docstrings to be generated for each function or class, with the best one being added to the source code. Please note that a higher number will deplete your token quota faster.",
         ),
     ) -> None:
+
         """Add docstring to classes and methods that don't have one by using the 'docstring-gen' library
 
         Args:
             path: The path to the directory containing Jupyter notebooks. If None, then the "nbs_path" from the settings.ini will be used.
             include_auto_gen_txt: If set to True, a note indicating that the docstring was autogenerated by 'docstring-gen' library will be added to the end.
             recreate_auto_gen_docs: If set to True, the autogenerated docstrings from the previous runs will be replaced with the new one.
             model: The name of the Codex model that will be used to generate docstrings.
@@ -236,71 +226,7 @@
     _app.add_typer(
         _docstring_gen_app,
         name="docstring",
     )
 
 
 _create_docstring_gen_sub_cmd()
-
-# %% ../nbs/CLI.ipynb 8
-def _filter_rc_branches(all_branches: str) -> str:
-    return "\n".join(
-        [
-            i.split(" ")[0]
-            for i in all_branches.split("\n")
-            if i != "" and not i.split(".")[-1].split(" ")[0].isdigit()
-        ]
-    )
-
-# %% ../nbs/CLI.ipynb 11
-def _get_version_numbers(all_versions: str) -> List[str]:
-    return [v.split(" ")[0] for v in all_versions.split("\n")]
-
-# %% ../nbs/CLI.ipynb 13
-@_app.command(
-    help="Deletes deployed pre-release documentation versions.",
-)
-def delete_pre_release_docs() -> None:
-    """Deletes deployed pre-release documentation versions."""
-    try:
-        typer.echo(f"Fetching origin/gh-pages for changes.")
-        nbdev_mkdocs.mkdocs._sprun(f"git fetch origin gh-pages --depth=1")
-        cmd = ["--config-file", "mkdocs/mkdocs.yml", "--rebase"]
-        # nosemgrep: python.lang.security.audit.subprocess-shell-true.subprocess-shell-true
-        result = subprocess.run(  # nosec: B603:subprocess_without_shell_equals_true
-            ["mike", "list"] + cmd,
-            stdout=subprocess.PIPE,
-        )
-        deployed_docs_list = result.stdout.decode("utf-8")
-        deployed_docs_list = _filter_rc_branches(deployed_docs_list)
-
-        if deployed_docs_list == "":
-            typer.echo("\nNo pre-release documentation version has been deployed.")
-            return
-
-        typer.echo(
-            f"\nList of deployed pre-release documentation version(s): \n{deployed_docs_list}\n"
-        )
-
-        delete = typer.confirm("Delete the pre-release version(s) listed above?")
-        if not delete:
-            typer.echo(
-                "\nNo changes made. Pre-release documentation versions remain untouched."
-            )
-            return
-
-        versions_to_delete = _get_version_numbers(deployed_docs_list)
-        cmd = versions_to_delete + ["--config-file", "mkdocs/mkdocs.yml", "--push"]
-        # nosemgrep: python.lang.security.audit.subprocess-shell-true.subprocess-shell-true
-        result = subprocess.run(  # nosec: B603:subprocess_without_shell_equals_true
-            ["mike", "delete"] + cmd,
-            stdout=subprocess.PIPE,
-        )
-        if result.returncode == 0:
-            typer.echo(f"\nSuccessfully deleted the version(s) listed above.")
-            typer.echo(
-                "\nOnce the 'pages build and deployment' Github action completes, view the project documentation URL to see the changes."
-            )
-
-    except Exception as e:
-        typer.secho(f"Unexpected internal error: {e}", err=True, fg=typer.colors.RED)
-        raise typer.Exit(1)
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/cli_doc.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/_helpers/cli_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,15 @@
             docs += _get_docs_for_click(
                 obj=command_obj, ctx=ctx, indent=indent + 1, call_prefix=use_prefix  # type: ignore
             )
     return docs
 
 # %% ../../nbs/CLI_Doc_Helper.ipynb 4
 def generate_cli_doc(module_name: str, app_name: str) -> str:
+
     """Generate CLI documentation for a Typer app.
 
     Args:
         module_name: The name of the module containing the Typer app.
         app_name: The name of the Typer app.
 
     Returns:
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/doc_links_utils.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/docstring.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,227 +1,290 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/Doc_Links_Utils.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Docstring.ipynb.
 
 # %% auto 0
-__all__ = ['fix_sym_links']
+__all__ = ['logger', 'run_examples_from_docstring']
 
-# %% ../../nbs/Doc_Links_Utils.ipynb 1
-import importlib
+# %% ../nbs/Docstring.ipynb 2
+import logging
+import os
 import re
+import sys
+import textwrap
+from pathlib import Path
+from subprocess import CalledProcessError, run  # nosec: B404
+from tempfile import TemporaryDirectory
 from typing import *
 
-from fastcore.basics import merge
-from fastcore.foundation import L
-from nbdev.doclinks import NbdevLookup
-
-# %% ../../nbs/Doc_Links_Utils.ipynb 3
-def _get_backtick_enclosed_string(s: str) -> str:
-    """Get the string enclosed in backticks.
+import rich
+from rich import print
+from rich.console import Console, Group
+from rich.panel import Panel
+from rich.rule import Rule
 
-    Args:
-        s: The string to extract from
+# %% ../nbs/Docstring.ipynb 3
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
 
-    Returns:
-        The extracted string enclosed in backticks.
+# %% ../nbs/Docstring.ipynb 4
+try:
+    import griffe
 
-    !!! note
+    griffe_logger = logging.getLogger("griffe.docstrings.google")
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-    """
-    pattern = r"`(.*?)`"
-    match = re.search(pattern, s)
-    return match.group(1)  # type: ignore
-
-# %% ../../nbs/Doc_Links_Utils.ipynb 5
-def _get_sym_path_from_nbdev_lookup(nbdev_lookup: NbdevLookup, symbol_details: Tuple[str, str, str]) -> str:  # type: ignore
-    """Get the symbol path from the NbdevLookup instance
+    griffe_logger.setLevel(logging.ERROR)
 
-    Args:
-        nbdev_lookup: Instance of NbdevLookup
-        symbol_details: The details of the symbol returned by the NbdevLookup instance
+    griffe_logger.warning("you should not see this")
+except:  # nosec: B110:try_except_pass] Try, Except, Pass detected.
+    pass
 
-    Returns:
-        The matched symbol path
+# %% ../nbs/Docstring.ipynb 6
+import rich.jupyter
 
-    !!! note
+rich.jupyter.JUPYTER_HTML_FORMAT = """\
+<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace;font-size:.68rem">{code}</pre>
+"""
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-    """
-    py_syms = merge(
-        *L(o["syms"].values() for o in nbdev_lookup.entries.values()).concat()
-    )
-    ret_val: List[str] = [
-        key for key, value in py_syms.items() if value == symbol_details
-    ]
-    return ret_val[0]
+# logger.info(f"{rich.jupyter.JUPYTER_HTML_FORMAT=}")
 
-# %% ../../nbs/Doc_Links_Utils.ipynb 8
-def _import_symbol(symbol: str) -> Any:
-    """Import the given symbol.
+# %% ../nbs/Docstring.ipynb 10
+def _extract_examples_from_docstring(o: Any) -> List[str]:
+    """Extract examples from docstring
 
     Args:
-        symbol: The symbol to import.
+        o: Any object with a docstring
 
     Returns:
-        The imported symbol.
+        List of examples
 
     Raises:
-        ModuleNotFoundError: If the module is not found.
+        ValueError: If the object has no docstring
 
     !!! note
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    names = symbol.split(".")
-    for i in range(len(names), 0, -1):
-        try:
-            module_name = ".".join(names[:i])
-            # nosemgrep: python.lang.security.audit.non-literal-import.non-literal-import
-            module = importlib.import_module(module_name)
-            o = module
-            for name in names[i:]:
-                o = getattr(o, name)
-            return o
-        except ModuleNotFoundError:
-            continue
-    raise ModuleNotFoundError(f"ModuleNotFound: {symbol}")
-
-# %% ../../nbs/Doc_Links_Utils.ipynb 18
-def _get_current_docs_version(docs_versioning: str, lib_version: str) -> str:
-    """Get the current docs version.
+    try:
+        import griffe
+    except:
+        raise Exception(
+            "This function should only be used for testing where griffe package is installed."
+        )
+
+    if o.__doc__ is None:
+        raise ValueError(f"{o.__name__}.__doc__ = {o.__doc__}")
+    sections = griffe.docstrings.parse(
+        griffe.dataclasses.Docstring(o.__doc__), griffe.docstrings.Parser.google
+    )
 
-    Args:
-        docs_versioning: The value set for docs_versioning flag in settings.ini file.
-        lib_version: The current version of the library.
+    def find_python_code(s: str) -> str:
+        """Finds the python code in a string
 
-    Returns:
-        The current docs version.
+        Args:
+            s: The string to search
 
-    !!! note
+        Returns:
+            The python code
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-    """
-    return (
-        ".".join(lib_version.split(".")[:-1])
-        if docs_versioning == "minor" and lib_version.replace(".", "").isdigit()
-        else lib_version
-    )
+        Raises:
+            ValueError: If no python code is found
+
+        !!! note
+
+            The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
+        """
+        code = [x[0] for x in re.findall("```\s*python((\n|.|\\n])+)```", s)]
+        #         print(f"{code=}")
+        if len(code) == 0:
+            raise ValueError(f"No python code found in {s}")
+        return "\n\n".join(code)
+
+    examples = [
+        find_python_code(section.value.description)  # type: ignore
+        for section in sections
+        if section.kind.value == "admonition" and section.value.annotation == "example"  # type: ignore
+    ]
 
-# %% ../../nbs/Doc_Links_Utils.ipynb 23
-def _append_doc_version(fixed_part: str, docs_versioning: str, lib_version: str) -> str:
-    """Append the current version of the documentation to a URL.
+    return examples
+
+# %% ../nbs/Docstring.ipynb 15
+def _get_keywords(examples: List[str]) -> List[str]:
+    """Get keywords from examples.
 
     Args:
-        fixed_part: The fixed part of the URL.
-        docs_versioning: The value set for docs_versioning flag in settings.ini file.
-        lib_version: The version of the library.
+        examples (List[str]): List of examples.
 
     Returns:
-        The URL with the documentation version appended.
+        List[str]: List of keywords.
 
     !!! note
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    return (
-        f"{fixed_part}/{_get_current_docs_version(docs_versioning, lib_version)}"
-        if docs_versioning != "" and docs_versioning != "None"
-        else fixed_part
+    keywords: List[str] = sum(
+        [
+            [x[9:-1] for x in re.findall("{fill in \w+}", example)]
+            for example in examples
+        ],
+        [],
     )
 
-# %% ../../nbs/Doc_Links_Utils.ipynb 28
-def _get_relative_sym_path(o: Any) -> str:
-    """Get the relative path of a symbol
+    return keywords
+
+# %% ../nbs/Docstring.ipynb 17
+def _replace_keywords(examples: List[str], **kwargs: str) -> List[str]:
+    """Replace keywords in a list of strings with the corresponding values in kwargs.
 
     Args:
-        o: The symbol to get the relative path of
+        examples: A list of strings
+        **kwargs: Keyword arguments
 
     Returns:
-        The relative path of the symbol
+        A list of strings with keywords replaced by values
+
+    Raises:
+        ValueError: If the set of keywords is not a subset of the set of keys in kwargs
 
     !!! note
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    qualname = o.__qualname__.split(".")
-    _o = (
-        o
-        if len(qualname) == 1
-        else _import_symbol(o.__module__ + "." + o.__qualname__.split(".")[0])
-    )
-    return "/".join((_o.__module__ + "." + _o.__qualname__).split("."))
+    keywords = _get_keywords(examples)
 
-# %% ../../nbs/Doc_Links_Utils.ipynb 36
-def _update_link(  # type: ignore
-    symbol: str,
-    symbol_details: Tuple[str, str, str],
-    nbdev_lookup: NbdevLookup,
-    docs_versioning: str,
-    lib_version: str,
-    use_relative_doc_links: bool,
-) -> str:
-    """Update the link of a symbol
+    if set(keywords) > set(kwargs.keys()):
+        raise ValueError(f"{set(keywords)} > {set(kwargs.keys())}")
+
+    for keyword in keywords:
+        examples = [
+            example.replace("{fill in " + keyword + "}", kwargs[keyword])
+            for example in examples
+        ]
+
+    return examples
+
+# %% ../nbs/Docstring.ipynb 19
+def _format_output(
+    s: str,
+    *,
+    title: str,
+    supress: bool = False,
+    sub_dict: Optional[Dict[str, str]] = None,
+    width: Optional[int] = None,
+) -> Group:
+    """Format the output of a string.
 
     Args:
-        symbol: The symbol to update
-        symbol_details: The details of the symbol returned by the NbdevLookup instance
-        nbdev_lookup: Instance of the NbdevLookup class
-        docs_versioning: The value set for docs_versioning flag in settings.ini file
-        lib_version: The current version of the library
-        use_relative_doc_links: If set to True, relative link to symbols will be add in the generated
-            documentation for easier local navigation
+        s: The string to format.
+        title: The title of the output.
+        supress: Whether to supress the output.
+        sub_dict: A dictionary of patterns to replace in the string.
+        width: The width of the output.
 
     Returns:
-        The updated link
+        The formatted string.
 
     !!! note
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    fixed_part = "/".join(symbol_details[0].split("/")[:4])
-    fixed_part_with_docs_version = _append_doc_version(
-        fixed_part, docs_versioning, lib_version
-    )
-
-    full_symbol_path = _get_sym_path_from_nbdev_lookup(nbdev_lookup, symbol_details)
-    o = _import_symbol(full_symbol_path)
-    relative_sym_path = _get_relative_sym_path(o)
-    if use_relative_doc_links:
-        updated_link = f"[`{symbol}`](api/{relative_sym_path}/#{o.__module__ + '.' + o.__qualname__})"
+    if sub_dict:
+        for pattern, replacement in sub_dict.items():
+            s = re.sub(pattern, replacement, s)
+    if supress:
+        return Group(Rule(f"{title} supressed"), "N/A")
+    #         return Panel("", title=f"{title} supressed", width=width)
     else:
-        updated_link = f"[`{symbol}`]({fixed_part_with_docs_version}/api/{relative_sym_path}/#{o.__module__ + '.' + o.__qualname__})"
+        return Group(Rule(title), s)
+
 
-    return updated_link
+#         return Panel(s, title=title, width=width)
 
-# %% ../../nbs/Doc_Links_Utils.ipynb 42
-def fix_sym_links(s: str, nbdev_lookup: NbdevLookup, docs_versioning: str, lib_version: str, use_relative_doc_links: bool) -> str:  # type: ignore
-    """Fix the default sym links generated by nbdev in the given string.
+# %% ../nbs/Docstring.ipynb 21
+def run_examples_from_docstring(
+    o: Any,
+    *,
+    supress_stdout: bool = False,
+    supress_stderr: bool = False,
+    sub_dict: Optional[Dict[str, str]] = None,
+    width: Optional[int] = 80,
+    **kwargs: str,
+) -> None:
+    """Runs example from a docstring
+
+    Parses docstring of an objects looking for examples. The examples are then saved into files and executed
+    in a separate process.
+
+    Note:
+        Execution context is not the same as the one in the notebook because we want examples to work from
+        user code. Make sure you compiled the library prior to executing the examples, otherwise you might
+        be running them agains an old version of the library.
 
     Args:
-        s: The string to fix
-        nbdev_lookup: Instance of the NbdevLookup class.
-        docs_versioning: The value set for docs_versioning flag in settings.ini file.
-        lib_version: The current version of the library.
-        use_relative_doc_links: If set to True, relative link to symbols will be add in the generated
-            documentation for easier local navigation.
+        o: an object, typically a function or a class, for which docstring is being parsed for examples
+        supress_stdout: omit stdout from output, typically due to security considerations
+        supress_stderr: omit stderr from output, typically due to security considerations
+        sub_dict: a dictionary mapping regexp patterns into replacement strings used to mask stdout and
+            stderr, typically used to mask sensitive information such as passwords
 
-    Returns:
-        The string with correct links added to the symbol references.
+        **kwargs: arguments use to replace "{fill in **param**}" in docstring with the actual values when running examples
+
+    Raises:
+        ValueError: if some params are missing from the **kwargs**
+        RuntimeException: if example fails
+
+    Example:
+        ```python
+        from  nbdev_mkdocs.docstring import run_examples_from_docstring
+
+        def f():
+            ```python
+            Example:
+                print("Hello {fill in name}!")
+                print("Goodbye {fill in other_name}!")
+            ```
+            pass
+
+
+        run_examples_from_docstring(f, name="John", other_name="Jane")
+        ```
 
     !!! note
 
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    pattern = r"\[`.+?`\]\(https?://[^)]+\)"
-    for match in re.findall(pattern, s):
-        symbol = _get_backtick_enclosed_string(match)
-        symbol_details = nbdev_lookup[symbol]
-        if symbol_details is not None:
-            updated_link = _update_link(
-                symbol,
-                symbol_details,
-                nbdev_lookup,
-                docs_versioning,
-                lib_version,
-                use_relative_doc_links,
+    console = Console(width=width)
+
+    examples = _extract_examples_from_docstring(o)
+    if len(examples) == 0:
+        raise ValueError(f"No examples found in:\n{o.__doc__}")
+
+    executable_examples = _replace_keywords(examples, **kwargs)
+    for example, executable_example in zip(examples, executable_examples):
+        with TemporaryDirectory() as d:
+            cmd_path = (Path(d) / "example.py").absolute()
+            with open(cmd_path, "w") as f:
+                f.write(executable_example)
+            process = run(  # nosec: B603
+                [sys.executable, str(cmd_path)], capture_output=True, text=True
+            )
+            group = Group(
+                "Example:",
+                Rule("code"),
+                textwrap.indent(example, " " * 4),
+                _format_output(
+                    process.stdout,
+                    title="stdout",
+                    supress=supress_stdout,
+                    sub_dict=sub_dict,
+                    width=width,
+                ),
+                _format_output(
+                    process.stderr,
+                    title="stderr",
+                    supress=supress_stderr,
+                    sub_dict=sub_dict,
+                    width=width,
+                ),
             )
-            s = s.replace(match, updated_link)
-    return s
+            #             print(Panel(panel_group, width=width))
+            console.print(group)
+            if process.returncode != 0:
+                raise RuntimeError(process.stderr)
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_helpers/utils.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/_helpers/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/Utils.ipynb.
 
 # %% auto 0
-__all__ = ['set_cwd', 'get_value_from_config', 'is_local_path', 'add_counter_suffix_to_filename', 'raise_error_and_exit']
+__all__ = ['set_cwd', 'get_value_from_config', 'is_local_path', 'add_counter_suffix_to_filename']
 
 # %% ../../nbs/Utils.ipynb 1
 import os
 from configparser import ConfigParser
 from contextlib import contextmanager
 from pathlib import Path
 from typing import *
 from urllib.parse import urlparse
 
 import nbdev
-import typer
 
 # %% ../../nbs/Utils.ipynb 3
 @contextmanager
 def set_cwd(cwd_path: Union[Path, str]) -> Generator:
     """Set the current working directory for the duration of the context manager.
 
     Args:
@@ -108,31 +107,7 @@
             ],
             default=0,
         )
         + 1
     )
     dst_path = parent_dir / f"{src_path.stem}.{counter_suffix}{src_path.suffix}"
     os.rename(src_path, dst_path)
-
-# %% ../../nbs/Utils.ipynb 12
-def raise_error_and_exit(message: str) -> None:
-    """Raise an error and exit
-
-    Args:
-        message: The error message to display
-
-    Returns:
-        None
-
-    Raises:
-        typer.Exit: If the error message is not provided
-
-    !!! note
-
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-    """
-    typer.secho(
-        message,
-        err=True,
-        fg=typer.colors.RED,
-    )
-    raise typer.Exit(code=1)
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_modidx.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/_modidx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,46 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/nbdev-mkdocs',
                 'doc_host': 'https://airtai.github.io',
                 'git_url': 'https://github.com/airtai/nbdev-mkdocs',
                 'lib_path': 'nbdev_mkdocs'},
-  'syms': { 'nbdev_mkdocs._helpers.api_docs_helper': { 'nbdev_mkdocs._helpers.api_docs_helper._add_mkdocstring_header_config': ( 'api_docs_helper.html#_add_mkdocstring_header_config',
-                                                                                                                                 'nbdev_mkdocs/_helpers/api_docs_helper.py'),
-                                                       'nbdev_mkdocs._helpers.api_docs_helper._filter_attributes_in_autodoc': ( 'api_docs_helper.html#_filter_attributes_in_autodoc',
-                                                                                                                                'nbdev_mkdocs/_helpers/api_docs_helper.py'),
-                                                       'nbdev_mkdocs._helpers.api_docs_helper._generate_autodoc': ( 'api_docs_helper.html#_generate_autodoc',
-                                                                                                                    'nbdev_mkdocs/_helpers/api_docs_helper.py'),
-                                                       'nbdev_mkdocs._helpers.api_docs_helper._generate_autodoc_string': ( 'api_docs_helper.html#_generate_autodoc_string',
-                                                                                                                           'nbdev_mkdocs/_helpers/api_docs_helper.py'),
-                                                       'nbdev_mkdocs._helpers.api_docs_helper._get_mkdocstring_config': ( 'api_docs_helper.html#_get_mkdocstring_config',
-                                                                                                                          'nbdev_mkdocs/_helpers/api_docs_helper.py'),
-                                                       'nbdev_mkdocs._helpers.api_docs_helper._get_symbol_filepath': ( 'api_docs_helper.html#_get_symbol_filepath',
-                                                                                                                       'nbdev_mkdocs/_helpers/api_docs_helper.py'),
-                                                       'nbdev_mkdocs._helpers.api_docs_helper.get_formatted_docstring_for_symbol': ( 'api_docs_helper.html#get_formatted_docstring_for_symbol',
-                                                                                                                                     'nbdev_mkdocs/_helpers/api_docs_helper.py')},
-            'nbdev_mkdocs._helpers.cli_doc': { 'nbdev_mkdocs._helpers.cli_doc._State': ( 'cli_doc_helper.html#_state',
+  'syms': { 'nbdev_mkdocs._helpers.cli_doc': { 'nbdev_mkdocs._helpers.cli_doc._State': ( 'cli_doc_helper.html#_state',
                                                                                          'nbdev_mkdocs/_helpers/cli_doc.py'),
                                                'nbdev_mkdocs._helpers.cli_doc._State.__init__': ( 'cli_doc_helper.html#_state.__init__',
                                                                                                   'nbdev_mkdocs/_helpers/cli_doc.py'),
                                                'nbdev_mkdocs._helpers.cli_doc._get_docs_for_click': ( 'cli_doc_helper.html#_get_docs_for_click',
                                                                                                       'nbdev_mkdocs/_helpers/cli_doc.py'),
                                                'nbdev_mkdocs._helpers.cli_doc._get_typer_from_module': ( 'cli_doc_helper.html#_get_typer_from_module',
                                                                                                          'nbdev_mkdocs/_helpers/cli_doc.py'),
                                                'nbdev_mkdocs._helpers.cli_doc._get_typer_from_state': ( 'cli_doc_helper.html#_get_typer_from_state',
                                                                                                         'nbdev_mkdocs/_helpers/cli_doc.py'),
                                                'nbdev_mkdocs._helpers.cli_doc.generate_cli_doc': ( 'cli_doc_helper.html#generate_cli_doc',
                                                                                                    'nbdev_mkdocs/_helpers/cli_doc.py')},
-            'nbdev_mkdocs._helpers.doc_links_utils': { 'nbdev_mkdocs._helpers.doc_links_utils._append_doc_version': ( 'doc_links_utils.html#_append_doc_version',
-                                                                                                                      'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils._get_backtick_enclosed_string': ( 'doc_links_utils.html#_get_backtick_enclosed_string',
-                                                                                                                                'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils._get_current_docs_version': ( 'doc_links_utils.html#_get_current_docs_version',
-                                                                                                                            'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils._get_relative_sym_path': ( 'doc_links_utils.html#_get_relative_sym_path',
-                                                                                                                         'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils._get_sym_path_from_nbdev_lookup': ( 'doc_links_utils.html#_get_sym_path_from_nbdev_lookup',
-                                                                                                                                  'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils._import_symbol': ( 'doc_links_utils.html#_import_symbol',
-                                                                                                                 'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils._update_link': ( 'doc_links_utils.html#_update_link',
-                                                                                                               'nbdev_mkdocs/_helpers/doc_links_utils.py'),
-                                                       'nbdev_mkdocs._helpers.doc_links_utils.fix_sym_links': ( 'doc_links_utils.html#fix_sym_links',
-                                                                                                                'nbdev_mkdocs/_helpers/doc_links_utils.py')},
-            'nbdev_mkdocs._helpers.quarto_to_mkdocs': { 'nbdev_mkdocs._helpers.quarto_to_mkdocs._add_markdown_attribute_to_enable_md_in_html': ( 'quarto_to_mkdocs_syntax_convertor.html#_add_markdown_attribute_to_enable_md_in_html',
-                                                                                                                                                 'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._fix_callout_syntax': ( 'quarto_to_mkdocs_syntax_convertor.html#_fix_callout_syntax',
-                                                                                                                        'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._fix_callout_syntax_in_file': ( 'quarto_to_mkdocs_syntax_convertor.html#_fix_callout_syntax_in_file',
-                                                                                                                                'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._get_callout_identifier': ( 'quarto_to_mkdocs_syntax_convertor.html#_get_callout_identifier',
-                                                                                                                            'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._get_callout_title_and_content': ( 'quarto_to_mkdocs_syntax_convertor.html#_get_callout_title_and_content',
-                                                                                                                                   'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._update_conditional_content_tags': ( 'quarto_to_mkdocs_syntax_convertor.html#_update_conditional_content_tags',
-                                                                                                                                     'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._update_mermaid_chart_tags': ( 'quarto_to_mkdocs_syntax_convertor.html#_update_mermaid_chart_tags',
-                                                                                                                               'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py'),
-                                                        'nbdev_mkdocs._helpers.quarto_to_mkdocs._update_quarto_tags_to_markdown_format': ( 'quarto_to_mkdocs_syntax_convertor.html#_update_quarto_tags_to_markdown_format',
-                                                                                                                                           'nbdev_mkdocs/_helpers/quarto_to_mkdocs.py')},
             'nbdev_mkdocs._helpers.utils': { 'nbdev_mkdocs._helpers.utils.add_counter_suffix_to_filename': ( 'utils.html#add_counter_suffix_to_filename',
                                                                                                              'nbdev_mkdocs/_helpers/utils.py'),
                                              'nbdev_mkdocs._helpers.utils.get_value_from_config': ( 'utils.html#get_value_from_config',
                                                                                                     'nbdev_mkdocs/_helpers/utils.py'),
                                              'nbdev_mkdocs._helpers.utils.is_local_path': ( 'utils.html#is_local_path',
                                                                                             'nbdev_mkdocs/_helpers/utils.py'),
-                                             'nbdev_mkdocs._helpers.utils.raise_error_and_exit': ( 'utils.html#raise_error_and_exit',
-                                                                                                   'nbdev_mkdocs/_helpers/utils.py'),
                                              'nbdev_mkdocs._helpers.utils.set_cwd': ( 'utils.html#set_cwd',
                                                                                       'nbdev_mkdocs/_helpers/utils.py')},
             'nbdev_mkdocs.docstring': { 'nbdev_mkdocs.docstring._extract_examples_from_docstring': ( 'docstring.html#_extract_examples_from_docstring',
                                                                                                      'nbdev_mkdocs/docstring.py'),
                                         'nbdev_mkdocs.docstring._format_output': ( 'docstring.html#_format_output',
                                                                                    'nbdev_mkdocs/docstring.py'),
                                         'nbdev_mkdocs.docstring._get_keywords': ( 'docstring.html#_get_keywords',
                                                                                   'nbdev_mkdocs/docstring.py'),
                                         'nbdev_mkdocs.docstring._replace_keywords': ( 'docstring.html#_replace_keywords',
                                                                                       'nbdev_mkdocs/docstring.py'),
                                         'nbdev_mkdocs.docstring.run_examples_from_docstring': ( 'docstring.html#run_examples_from_docstring',
                                                                                                 'nbdev_mkdocs/docstring.py')},
-            'nbdev_mkdocs.mkdocs': { 'nbdev_mkdocs.mkdocs._add_all_submodules': ( 'mkdocs.html#_add_all_submodules',
-                                                                                  'nbdev_mkdocs/mkdocs.py'),
+            'nbdev_mkdocs.mkdocs': { 'nbdev_mkdocs.mkdocs._add_markdown_attribute_to_enable_md_in_html': ( 'mkdocs.html#_add_markdown_attribute_to_enable_md_in_html',
+                                                                                                           'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._build_summary': ('mkdocs.html#_build_summary', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._copy_change_log_if_exists': ( 'mkdocs.html#_copy_change_log_if_exists',
                                                                                          'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._copy_cname_if_needed': ( 'mkdocs.html#_copy_cname_if_needed',
                                                                                     'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._copy_docs_overrides': ( 'mkdocs.html#_copy_docs_overrides',
                                                                                    'nbdev_mkdocs/mkdocs.py'),
@@ -99,69 +51,59 @@
                                      'nbdev_mkdocs.mkdocs._create_mkdocs_dir': ('mkdocs.html#_create_mkdocs_dir', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._create_mkdocs_yaml': ( 'mkdocs.html#_create_mkdocs_yaml',
                                                                                   'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._create_summary_template': ( 'mkdocs.html#_create_summary_template',
                                                                                        'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._expand_sidebar_if_needed': ( 'mkdocs.html#_expand_sidebar_if_needed',
                                                                                         'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._fix_sym_links_in_nbs': ( 'mkdocs.html#_fix_sym_links_in_nbs',
-                                                                                    'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._flattern_sidebar_items': ( 'mkdocs.html#_flattern_sidebar_items',
                                                                                       'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._generate_api_doc': ('mkdocs.html#_generate_api_doc', 'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._generate_api_docs': ('mkdocs.html#_generate_api_docs', 'nbdev_mkdocs/mkdocs.py'),
+                                     'nbdev_mkdocs.mkdocs._generate_api_doc_for_submodule': ( 'mkdocs.html#_generate_api_doc_for_submodule',
+                                                                                              'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_api_docs_for_module': ( 'mkdocs.html#_generate_api_docs_for_module',
                                                                                             'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_cli_doc_for_submodule': ( 'mkdocs.html#_generate_cli_doc_for_submodule',
                                                                                               'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_cli_docs_for_module': ( 'mkdocs.html#_generate_cli_docs_for_module',
                                                                                             'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_default_social_image_link': ( 'mkdocs.html#_generate_default_social_image_link',
                                                                                                   'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_markdown_from_files': ( 'mkdocs.html#_generate_markdown_from_files',
                                                                                             'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_nav_from_sidebar': ( 'mkdocs.html#_generate_nav_from_sidebar',
                                                                                          'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._generate_summary_for_sidebar': ( 'mkdocs.html#_generate_summary_for_sidebar',
                                                                                             'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._get_api_summary': ('mkdocs.html#_get_api_summary', 'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._get_api_summary_item': ( 'mkdocs.html#_get_api_summary_item',
-                                                                                    'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._get_files_to_convert_to_markdown': ( 'mkdocs.html#_get_files_to_convert_to_markdown',
                                                                                                 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._get_kwargs_from_settings': ( 'mkdocs.html#_get_kwargs_from_settings',
                                                                                         'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._get_sidebar_from_config': ( 'mkdocs.html#_get_sidebar_from_config',
                                                                                        'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._get_submodule_members': ( 'mkdocs.html#_get_submodule_members',
-                                                                                     'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._get_submodules': ('mkdocs.html#_get_submodules', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._get_title_from_notebook': ( 'mkdocs.html#_get_title_from_notebook',
                                                                                        'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._import_all_members': ( 'mkdocs.html#_import_all_members',
-                                                                                  'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._import_functions_and_classes': ( 'mkdocs.html#_import_functions_and_classes',
-                                                                                            'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._import_submodules': ('mkdocs.html#_import_submodules', 'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._is_private': ('mkdocs.html#_is_private', 'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._load_submodules': ('mkdocs.html#_load_submodules', 'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._merge_lists': ('mkdocs.html#_merge_lists', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._read_sidebar_from_yml': ( 'mkdocs.html#_read_sidebar_from_yml',
                                                                                      'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._replace_all': ('mkdocs.html#_replace_all', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._replace_ghp_deploy_action': ( 'mkdocs.html#_replace_ghp_deploy_action',
                                                                                          'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._restrict_line_length': ( 'mkdocs.html#_restrict_line_length',
                                                                                     'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._sprun': ('mkdocs.html#_sprun', 'nbdev_mkdocs/mkdocs.py'),
-                                     'nbdev_mkdocs.mkdocs._update_api_docs': ('mkdocs.html#_update_api_docs', 'nbdev_mkdocs/mkdocs.py'),
+                                     'nbdev_mkdocs.mkdocs._update_conditional_content_tags': ( 'mkdocs.html#_update_conditional_content_tags',
+                                                                                               'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._update_gitignore_file': ( 'mkdocs.html#_update_gitignore_file',
                                                                                      'nbdev_mkdocs/mkdocs.py'),
+                                     'nbdev_mkdocs.mkdocs._update_mermaid_chart_tags': ( 'mkdocs.html#_update_mermaid_chart_tags',
+                                                                                         'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs._update_path_in_markdown': ( 'mkdocs.html#_update_path_in_markdown',
                                                                                        'nbdev_mkdocs/mkdocs.py'),
+                                     'nbdev_mkdocs.mkdocs._update_quarto_tags_to_markdown_format': ( 'mkdocs.html#_update_quarto_tags_to_markdown_format',
+                                                                                                     'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs.nbdev_mkdocs_docs': ('mkdocs.html#nbdev_mkdocs_docs', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs.new': ('mkdocs.html#new', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs.prepare': ('mkdocs.html#prepare', 'nbdev_mkdocs/mkdocs.py'),
                                      'nbdev_mkdocs.mkdocs.preview': ('mkdocs.html#preview', 'nbdev_mkdocs/mkdocs.py')},
             'nbdev_mkdocs.social_image_generator': { 'nbdev_mkdocs.social_image_generator._IMG_Generator': ( 'social_image_generator.html#_img_generator',
                                                                                                              'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._capture_and_save_screenshot': ( 'social_image_generator.html#_capture_and_save_screenshot',
@@ -170,16 +112,14 @@
                                                                                                                    'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._generate_ai_image': ( 'social_image_generator.html#_generate_ai_image',
                                                                                                                  'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._generate_html_str': ( 'social_image_generator.html#_generate_html_str',
                                                                                                                  'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._generate_image_url': ( 'social_image_generator.html#_generate_image_url',
                                                                                                                   'nbdev_mkdocs/social_image_generator.py'),
-                                                     'nbdev_mkdocs.social_image_generator._read_yaml_file': ( 'social_image_generator.html#_read_yaml_file',
-                                                                                                              'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._unescape_exclamation_mark': ( 'social_image_generator.html#_unescape_exclamation_mark',
                                                                                                                          'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._update_social_image_in_mkdocs_yml': ( 'social_image_generator.html#_update_social_image_in_mkdocs_yml',
                                                                                                                                  'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator._update_social_image_in_site_overrides': ( 'social_image_generator.html#_update_social_image_in_site_overrides',
                                                                                                                                      'nbdev_mkdocs/social_image_generator.py'),
                                                      'nbdev_mkdocs.social_image_generator.generate_social_image': ( 'social_image_generator.html#generate_social_image',
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_package_data.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/_package_data.py`

 * *Files identical despite different names*

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/_testing.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/_testing.py`

 * *Files identical despite different names*

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/mkdocs.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/mkdocs.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,84 +3,72 @@
 # %% auto 0
 __all__ = ['new', 'nbdev_mkdocs_docs', 'prepare', 'preview']
 
 # %% ../nbs/Mkdocs.ipynb 1
 import collections
 import datetime
 import importlib
-import itertools
 import multiprocessing
 import os
 import pkgutil
 import re
 import shlex
 import shutil
 import subprocess  # nosec: B404
 import sys
 import textwrap
 import types
 from configparser import ConfigParser
-from inspect import getmembers, getmodule, isclass, iscoroutine, isfunction, ismethod
 from pathlib import Path
 from typing import *
 
 import nbdev
-import nbformat
 import typer
 import yaml
 from configupdater import ConfigUpdater, Section
 from configupdater.option import Option
-from fastcore.basics import merge
-from fastcore.foundation import L
 from fastcore.shutil import move
-from nbdev.clean import nbdev_clean
-from nbdev.doclinks import NbdevLookup, nbdev_export
+from nbdev.doclinks import nbdev_export
 from nbdev.frontmatter import FrontmatterProc, _fm2dict
 from nbdev.process import NBProcessor
+from nbdev.quarto import nbdev_readme
 from nbdev.quarto import prepare as nbdev_prepare
 from nbdev.quarto import refresh_quarto_yml
 from nbdev.serve import proc_nbs
-from nbdev.test import nbdev_test
 
 from ._helpers.cli_doc import generate_cli_doc
-from ._helpers.doc_links_utils import fix_sym_links
-from nbdev_mkdocs._helpers.utils import (
-    get_value_from_config,
-    raise_error_and_exit,
-    set_cwd,
-)
+from ._helpers.utils import get_value_from_config, set_cwd
 from ._package_data import get_root_data_path
 from .social_image_generator import _update_social_image_in_mkdocs_yml
-from nbdev_mkdocs._helpers.quarto_to_mkdocs import (
-    _update_quarto_tags_to_markdown_format,
-)
-from ._helpers.api_docs_helper import get_formatted_docstring_for_symbol
 
 # %% ../nbs/Mkdocs.ipynb 5
 def _create_mkdocs_dir(root_path: str) -> None:
     """Create a mkdocs directory in the root path.
 
     Args:
-        root_path: The root path of the project.
+        root_path: The root path.
 
     Returns:
         None
 
     Raises:
         typer.Exit: If the mkdocs_template path does not exist.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     mkdocs_template_path = get_root_data_path() / "mkdocs_template"
     if not mkdocs_template_path.exists():
-        raise_error_and_exit(
-            f"Unexpected error: path {mkdocs_template_path.resolve()} does not exists!"
+        typer.secho(
+            f"Unexpected error: path {mkdocs_template_path.resolve()} does not exists!",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=4)
     dst_path = Path(root_path) / "mkdocs"
     if dst_path.exists():
         typer.secho(
             f"Directory {dst_path.resolve()} already exist, skipping its creation.",
         )
     else:
         shutil.copytree(mkdocs_template_path, dst_path)
@@ -89,15 +77,15 @@
             f"Directory {dst_path.resolve()} created.",
         )
 
 # %% ../nbs/Mkdocs.ipynb 8
 _mkdocs_template_path = get_root_data_path() / "mkdocs_template.yml"
 
 # %% ../nbs/Mkdocs.ipynb 10
-with open(_mkdocs_template_path, "r", encoding="utf-8") as f:
+with open(_mkdocs_template_path, "r") as f:
     _mkdocs_template = f.read()
 
 # %% ../nbs/Mkdocs.ipynb 12
 def _get_kwargs_from_settings(
     settings_path: Path, mkdocs_template: Optional[str] = None
 ) -> Dict[str, str]:
     """Get the values from the settings file
@@ -146,22 +134,25 @@
             )
             return
 
         # get default values from settings.ini
         settings_path = Path(root_path) / "settings.ini"
         kwargs = _get_kwargs_from_settings(settings_path)
         mkdocs_yaml_str = _mkdocs_template.format(**kwargs)
-        with open(mkdocs_path, "w", encoding="utf-8") as f:
+        with open(mkdocs_path, "w") as f:
             f.write(mkdocs_yaml_str)
             typer.secho(f"File '{mkdocs_path.resolve()}' generated.")
             return
     except Exception as e:
-        raise_error_and_exit(
-            f"Unexpected Error while creating '{mkdocs_path.resolve()}': {e}"
+        typer.secho(
+            f"Unexpected Error while creating '{mkdocs_path.resolve()}': {e}",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=3)
 
 # %% ../nbs/Mkdocs.ipynb 17
 _summary_template = """{sidebar}
 - API
 {api}
 - CLI
 {cli}
@@ -187,39 +178,45 @@
         if summary_template_path.exists():
             typer.secho(
                 f"Path '{summary_template_path.resolve()}' exists, skipping generation of it."
             )
             return
 
         # generated a new summary_template_path.yml file
-        with open(summary_template_path, "w", encoding="utf-8") as f:
+        with open(summary_template_path, "w") as f:
             f.write(_summary_template)
             typer.secho(f"File '{summary_template_path.resolve()}' generated.")
             return
     except Exception as e:
-        raise_error_and_exit(
-            f"Unexpected Error while creating '{summary_template_path.resolve()}': {e}"
+        typer.secho(
+            f"Unexpected Error while creating '{summary_template_path.resolve()}': {e}",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=3)
 
 # %% ../nbs/Mkdocs.ipynb 19
 def _replace_ghp_deploy_action(root_path: str) -> None:
     """Replace the default deploy action file in the .github/workflows directory with a custom one.
 
     Args:
         root_path: The root path of the project.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     src_path = get_root_data_path() / "ghp_deploy_action_template.yml"
     if not src_path.exists():
-        raise_error_and_exit(
+        typer.secho(
             f"Unexpected error: path {src_path.resolve()} does not exists!",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=4)
 
     workflows_path = Path(root_path) / ".github" / "workflows"
     workflows_path.mkdir(exist_ok=True, parents=True)
 
     dst_path = Path(workflows_path) / "deploy.yaml"
     shutil.copyfile(src_path, dst_path)
 
@@ -231,25 +228,28 @@
         root_path: The root path of the project
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     _mkdocs_gitignore_path = get_root_data_path() / "gitignore.txt"
-    with open(_mkdocs_gitignore_path, "r", encoding="utf-8") as f:
+    with open(_mkdocs_gitignore_path, "r") as f:
         _new_paths_to_ignore = f.read()
         _new_paths_to_ignore = "\n\n" + _new_paths_to_ignore
 
     gitignore_path = Path(root_path) / ".gitignore"
     if not gitignore_path.exists():
-        raise_error_and_exit(
-            f"Unexpected error: path {gitignore_path.resolve()} does not exists!"
+        typer.secho(
+            f"Unexpected error: path {gitignore_path.resolve()} does not exists!",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=1)
 
-    with open(gitignore_path, "a", encoding="utf-8") as f:
+    with open(gitignore_path, "a") as f:
         f.write(_new_paths_to_ignore)
 
 # %% ../nbs/Mkdocs.ipynb 24
 def _generate_default_social_image_link(root_path: str) -> None:
     """Add default social sharing image link to the mkdocs yaml file
 
     Args:
@@ -310,14 +310,95 @@
         for f in cache.rglob("*")
         if f.suffix in exts and not any(p.startswith(".") for p in f.parts)
     ]
 
     return files
 
 # %% ../nbs/Mkdocs.ipynb 33
+def _update_conditional_content_tags(text: str) -> str:
+    """Update conditional content tags.
+
+    Args:
+        text: The text to update the conditional content tags in.
+
+    Returns:
+        The updated text with the conditional content tags modified.
+
+    !!! note
+
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
+    """
+    pattern = r":::\s*{(?:\s*.*\.content-visible|\s*\.content-hidden)\s*(when|unless)-format\s*=\\\s*(\"|\')\s*(html|markdown)\s*\\(\"|\')\s*.*}"
+    text = re.sub(
+        pattern,
+        lambda m: m.group(0).replace(
+            m.group(1), "when" if m.group(1) == "unless" else "unless"
+        ),
+        text,
+    )
+    return text
+
+# %% ../nbs/Mkdocs.ipynb 36
+def _update_mermaid_chart_tags(text: str) -> str:
+    """Convert the mermaid chart tags from quarto format to markdown format.
+
+    Args:
+        text: The text to update the mermaid chart tags in.
+
+    Returns:
+        The updated text with the mermaid chart tags modified.
+
+    !!! note
+
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
+    """
+    pattern = r"```\s*{mermaid\s*}"
+    text = re.sub(pattern, "``` mermaid", text)
+    return text
+
+# %% ../nbs/Mkdocs.ipynb 38
+def _add_markdown_attribute_to_enable_md_in_html(text: str) -> str:
+    """Add markdown attribute to enable markdown in html.
+
+    Args:
+        text: The text to add the markdown attribute to
+
+    Returns:
+        The text with the markdown attribute added
+
+    !!! note
+
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
+    """
+    pattern = r":::\s*{\s*(markdown=1)?\s*"
+    text = re.sub(pattern, r"::: {markdown=1 ", text)
+    return text
+
+# %% ../nbs/Mkdocs.ipynb 40
+def _update_quarto_tags_to_markdown_format(nb_path: Path) -> None:
+    """Update Quarto tags to Markdown format
+
+    Args:
+        nb_path: Path to the notebook
+
+    !!! note
+
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
+    """
+    with open(nb_path, "r") as f:
+        contents = f.read()
+
+    contents = _update_conditional_content_tags(contents)
+    contents = _update_mermaid_chart_tags(contents)
+    contents = _add_markdown_attribute_to_enable_md_in_html(contents)
+
+    with open(nb_path, "w") as f:
+        f.write(contents)
+
+# %% ../nbs/Mkdocs.ipynb 43
 def _sprun(cmd: str) -> None:
     """Run a command via subprocess.check_output
 
     Args:
         cmd: The command to run
 
     Raises:
@@ -334,46 +415,47 @@
         )
 
     except subprocess.CalledProcessError as e:
         sys.exit(
             f"CMD Failed: e={e}\n e.returncode={e.returncode}\n e.output={e.output}\n e.stderr={e.stderr}\n cmd={cmd}"
         )
 
-# %% ../nbs/Mkdocs.ipynb 34
-def _generate_markdown_from_files(root_path: str, cache_path: Path) -> None:
+# %% ../nbs/Mkdocs.ipynb 44
+def _generate_markdown_from_files(root_path: str) -> None:
     """Generate markdown files from notebook files.
 
     Args:
         root_path: The root path of the project.
-        cache_path: The path to the _proc directory.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     doc_path = Path(root_path) / "mkdocs" / "docs"
     doc_path.mkdir(exist_ok=True, parents=True)
 
     with set_cwd(root_path):
-        files = _get_files_to_convert_to_markdown(cache_path)
+
+        cache = proc_nbs()
+        files = _get_files_to_convert_to_markdown(cache)
 
         for f in files:
-            dir_prefix = str(f.parent)[len(str(cache_path)) + 1 :]
+            dir_prefix = str(f.parent)[len(str(cache)) + 1 :]
             dst_md = doc_path / f"{dir_prefix}" / f"{f.stem}.md"
             dst_md.parent.mkdir(parents=True, exist_ok=True)
 
             _update_quarto_tags_to_markdown_format(f)
 
-            cmd = f'cd "{cache_path}" && quarto render "{f}" -o "{f.stem}.md" -t gfm --no-execute'
+            cmd = f'cd "{cache}" && quarto render "{f}" -o "{f.stem}.md" -t gfm --no-execute'
             _sprun(cmd)
 
-            src_md = cache_path / "_docs" / f"{f.stem}.md"
-            shutil.move(str(src_md), dst_md)
+            src_md = cache / "_docs" / f"{f.stem}.md"
+            shutil.move(src_md, dst_md)
 
-# %% ../nbs/Mkdocs.ipynb 36
+# %% ../nbs/Mkdocs.ipynb 46
 def _replace_all(text: str, dir_prefix: str) -> str:
     """Replace the images relative path in the markdown string
 
     Args:
         text: The markdown string
         dir_prefix: Sub directory prefix to append to the image's relative path
 
@@ -408,46 +490,45 @@
                 )
 
     for k, v in _replace.items():
         text = text.replace(k, v)
 
     return text
 
-# %% ../nbs/Mkdocs.ipynb 38
-def _update_path_in_markdown(cache_path: Path, doc_path: Path) -> None:
+# %% ../nbs/Mkdocs.ipynb 48
+def _update_path_in_markdown(cache: Path, doc_path: Path) -> None:
     """Update guide images relative path in the markdown files
 
     Args:
-        cache_path: The path to the _proc directory.
-        doc_path: Path to the mkdocs/docs directory.
+        cache: Path to the nbs cache directory
+        doc_path: Path to the mkdocs/docs directory
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    files = _get_files_to_convert_to_markdown(cache_path)
+    files = _get_files_to_convert_to_markdown(cache)
 
     for file in files:
-        dir_prefix = str(file.parent)[len(str(cache_path)) + 1 :]
+        dir_prefix = str(file.parent)[len(str(cache)) + 1 :]
         md = doc_path / f"{dir_prefix}" / f"{file.stem}.md"
 
-        with open(Path(md), "r", encoding="utf-8") as f:
+        with open(Path(md), "r") as f:
             _new_text = f.read()
             _new_text = _replace_all(_new_text, dir_prefix)
-        with open(Path(md), "w", encoding="utf-8") as f:
+        with open(Path(md), "w") as f:
             f.write(_new_text)
 
 
-def _copy_images_to_docs_dir(root_path: str, cache_path: Path) -> None:
+def _copy_images_to_docs_dir(root_path: str) -> None:
     # Reference: https://github.com/quarto-dev/quarto-cli/blob/main/src/core/image.ts#L38
     """Copy images from nbs to docs directory.
 
     Args:
         root_path: The root path of the project.
-        cache_path: The path to the _proc directory.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     image_extensions = [
         ".apng",
@@ -459,54 +540,58 @@
         ".pjpeg",
         ".pjp",
         ".png",
         ".svg",
         ".webp",
     ]
 
+    cache = proc_nbs()
     nbs_images_path = [
-        p for p in Path(cache_path).glob(r"**/*") if p.suffix in image_extensions
+        p for p in Path(cache).glob(r"**/*") if p.suffix in image_extensions
     ]
 
     if len(nbs_images_path) > 0:
         doc_path = Path(root_path) / "mkdocs" / "docs"
         img_path = Path(doc_path) / "images" / "nbs"
         for src_path in nbs_images_path:
-            dir_prefix = str(src_path.parent)[len(str(cache_path)) + 1 :]
+            dir_prefix = str(src_path.parent)[len(str(cache)) + 1 :]
             dst_path = Path(img_path) / f"{dir_prefix}"
             dst_path.mkdir(exist_ok=True, parents=True)
             shutil.copy(src_path, dst_path)
 
-        _update_path_in_markdown(cache_path, doc_path)
+        _update_path_in_markdown(cache, doc_path)
 
-# %% ../nbs/Mkdocs.ipynb 42
-def _get_title_from_notebook(cache_path: Path, file_path: Path) -> str:
+# %% ../nbs/Mkdocs.ipynb 52
+def _get_title_from_notebook(file_path: Path) -> str:
     """Get the title of a notebook or markdown file.
 
     Args:
-        cache_path: The path to the _proc directory.
-        file_path: The path to the notebook file.
+        file_path: The path to the file.
 
     Returns:
         The title of the file.
 
     Raises:
         ValueError: If the file does not exist.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     title: str
-    _file_path = cache_path / file_path
+    cache = proc_nbs()
+    _file_path = Path(cache) / file_path
 
     if not _file_path.exists():
-        raise_error_and_exit(
-            f"Unexpected error: path {_file_path.resolve()} does not exists!"
+        typer.secho(
+            f"Unexpected error: path {_file_path.resolve()} does not exists!",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=1)
 
     if _file_path.suffix == ".ipynb":
         nbp = NBProcessor(_file_path, procs=FrontmatterProc)
         nbp.process()
 
         if "title" in nbp.nb.frontmatter_:
             title = nbp.nb.frontmatter_["title"]
@@ -518,23 +603,23 @@
             ]
             title = (
                 f"{_file_path.stem}.html"
                 if len(headers) == 0
                 else headers[0].replace("#", "").strip()
             )
     else:
-        with open(_file_path, "r", encoding="utf-8") as f:
+        with open(_file_path) as f:
             contents = f.read()
         metadata = _fm2dict(contents, nb=False)
         metadata = {k.lower(): v for k, v in metadata.items()}
         title = metadata["title"]
 
     return title
 
-# %% ../nbs/Mkdocs.ipynb 44
+# %% ../nbs/Mkdocs.ipynb 54
 def _get_sidebar_from_config(file_path: Path) -> List[Any]:
     """Get the sidebar contents from the sidebar.yml or _quarto.yml file.
 
     Args:
         file_path: Path to the sidebar.yml or _quarto.yml file.
 
     Returns:
@@ -544,24 +629,32 @@
         KeyError: If the sidebar is not defined in the config file.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     if not file_path.exists():
-        raise_error_and_exit(f"Path '{file_path.resolve()}' does not exists!")
+        typer.secho(
+            f"Path '{file_path.resolve()}' does not exists!",
+            err=True,
+            fg=typer.colors.RED,
+        )
+        raise typer.Exit(code=1)
 
     try:
-        with open(file_path, "r", encoding="utf-8") as f:
+        with open(file_path) as f:
             config = yaml.safe_load(f)
         sidebar: List[Any] = config["website"]["sidebar"]["contents"]
     except KeyError as e:
-        raise_error_and_exit(
-            f"Key Error: Contents of the sidebar are not defined in the files sidebar.yml or _quarto.yml."
+        typer.secho(
+            f"Key Error: Contents of the sidebar are not defined in the files sidebar.yml or _quarto.yml.",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=1)
 
     return sidebar
 
 
 def _read_sidebar_from_yml(root_path: str) -> List[Union[str, Any]]:
     """Get the sidebar contents from the sidebar.yml or _quarto.yml file.
 
@@ -586,15 +679,15 @@
 
     return (
         _get_sidebar_from_config(sidebar_yml_path)
         if sidebar_yml_path.exists()
         else _get_sidebar_from_config(_quarto_yml_path)
     )
 
-# %% ../nbs/Mkdocs.ipynb 47
+# %% ../nbs/Mkdocs.ipynb 57
 def _flattern_sidebar_items(items: List[Union[str, Any]]) -> List[Union[str, Any]]:
     """Flatten a list of items.
 
     Args:
         items: A list of items.
 
     Returns:
@@ -640,70 +733,97 @@
                 files = list(_proc_dir.glob(item["contents"]))
                 files = sorted([str(f.relative_to(_proc_dir)) for f in files if f.suffix in exts])  # type: ignore
                 item["contents"] = files
 
     flat_sidebar = _flattern_sidebar_items(sidebar)
     return flat_sidebar
 
-# %% ../nbs/Mkdocs.ipynb 49
+# %% ../nbs/Mkdocs.ipynb 59
 def _generate_nav_from_sidebar(
-    sidebar_items: List[Union[str, Dict[str, Any]]], cache_path: Path, level: int = 0
+    sidebar_items: List[Union[str, Dict[str, Any]]], level: int = 0
 ) -> str:
     """Generate a navigation string for mkdocs from a sidebar list.
 
     Args:
         sidebar_items: A list of strings or dictionaries.
-        cache_path: The path to the _proc directory.
         level: The level of indentation to use.
 
     Returns:
         str: The navigation string.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     output = ""
     links = [
         "{}- [{}]({}.md)\n".format(
             "    " * level,
-            _get_title_from_notebook(cache_path, Path(item)),
+            _get_title_from_notebook(Path(item)),
             Path(item).with_suffix(""),
         )
         if isinstance(item, str)
         else "{}- {}\n".format("    " * level, item["section"])
-        + _generate_nav_from_sidebar(item["contents"], cache_path, level + 1)
+        + _generate_nav_from_sidebar(item["contents"], level + 1)
         for item in sidebar_items
     ]
     output += "".join(links)
     return output
 
-# %% ../nbs/Mkdocs.ipynb 51
-def _generate_summary_for_sidebar(root_path: str, cache_path: Path) -> str:
+# %% ../nbs/Mkdocs.ipynb 61
+def _generate_summary_for_sidebar(
+    root_path: str,
+) -> str:
     """Generate a summary for the sidebar
 
     Args:
-        root_path: The root path of the project.
-        cache_path: The path to the _proc directory.
+        root_path: The root path
 
     Returns:
         The summary for the sidebar
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     with set_cwd(root_path):
         sidebar = _read_sidebar_from_yml(root_path)
         expanded_sidebar = _expand_sidebar_if_needed(root_path, sidebar)
-        sidebar_nav = _generate_nav_from_sidebar(expanded_sidebar, cache_path)
+        sidebar_nav = _generate_nav_from_sidebar(expanded_sidebar)
 
         return sidebar_nav
 
-# %% ../nbs/Mkdocs.ipynb 53
+# %% ../nbs/Mkdocs.ipynb 64
+def _get_submodules(package_name: str) -> List[str]:
+    """Get all submodules of a package.
+
+    Args:
+        package_name: The name of the package.
+
+    Returns:
+        A list of submodules.
+
+    !!! note
+
+        The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
+    """
+    # nosemgrep: python.lang.security.audit.non-literal-import.non-literal-import
+    m = importlib.import_module(package_name)
+    submodules = [
+        info.name
+        for info in pkgutil.walk_packages(m.__path__, prefix=f"{package_name}.")
+    ]
+    submodules = [
+        x
+        for x in submodules
+        if not any([name.startswith("_") for name in x.split(".")])
+    ]
+    return submodules
+
+# %% ../nbs/Mkdocs.ipynb 66
 def _copy_not_found_file_and_get_path(root_path: str, file_prefix: str) -> str:
     """Copy the CLI command found file to the docs directory and return the path to the file.
 
     Args:
         root_path: The root path of the project
         file_prefix: The prefix of the file to be copied
 
@@ -712,247 +832,97 @@
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     src_path = get_root_data_path() / f"{file_prefix}_not_found.md"
     if not src_path.exists():
-        raise_error_and_exit(
-            f"Unexpected error: path {src_path.resolve()} does not exists!"
+        typer.secho(
+            f"Unexpected error: path {src_path.resolve()} does not exists!",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=1)
 
     docs_path = Path(root_path) / "mkdocs" / "docs"
     docs_path.mkdir(exist_ok=True, parents=True)
     dst_path = docs_path / f"{file_prefix}_not_found.md"
     shutil.copyfile(src_path, dst_path)
 
     return (
         f"({dst_path.name})"
         if file_prefix == "changelog"
         else " " * 4 + f"- [Not found]({dst_path.name})"
     )
 
-# %% ../nbs/Mkdocs.ipynb 56
-def _get_submodules(package_name: str) -> List[str]:
-    """Get all submodules of a package.
+# %% ../nbs/Mkdocs.ipynb 68
+def _generate_api_doc_for_submodule(
+    root_path: str, docs_dir_name: str, submodule: str
+) -> str:
+    """Generate API documentation for a submodule.
 
     Args:
-        package_name: The name of the package.
+        root_path: The root path of the project
+        docs_dir_name: The name of the docs directory
+        submodule: The submodule for which to generate the API documentation
 
     Returns:
-        A list of submodules.
+        The path to the generated API documentation
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    try:
-        # nosemgrep: python.lang.security.audit.non-literal-import.non-literal-import
-        m = importlib.import_module(package_name)
-    except ModuleNotFoundError as e:
-        #         if (
-        #             "NBDEV_MKDOCS_PATCH_IMPORTLIB" in os.environ
-        #             and os.environ["NBDEV_MKDOCS_PATCH_IMPORTLIB"] != "false"
-        #         ):
-        #             # nosemgrep: python.lang.security.audit.non-literal-import.non-literal-import
-        #             m = importlib.import_module("nbdev_mkdocs")
-        #         else:
-        raise e
-    submodules = [
-        info.name
-        for info in pkgutil.walk_packages(m.__path__, prefix=f"{package_name}.")
-    ]
-    submodules = [
-        x
-        for x in submodules
-        if not any([name.startswith("_") for name in x.split(".")])
-    ]
-    return [package_name] + submodules
-
-# %% ../nbs/Mkdocs.ipynb 59
-def _import_submodules(module_name: str) -> List[types.ModuleType]:
-    def import_module(name: str) -> Optional[types.ModuleType]:
-        try:
-            # nosemgrep: python.lang.security.audit.non-literal-import.non-literal-import
-            return importlib.import_module(name)
-        except Exception:
-            return None
-
-    package_names = _get_submodules(module_name)
-    modules = [import_module(n) for n in package_names]
-    return [m for m in modules if m is not None]
-
-# %% ../nbs/Mkdocs.ipynb 62
-def _import_functions_and_classes(
-    m: types.ModuleType,
-) -> List[Tuple[str, Union[types.FunctionType, Type[Any]]]]:
-    return [(x, y) for x, y in getmembers(m) if isfunction(y) or isclass(y)]
-
-# %% ../nbs/Mkdocs.ipynb 64
-def _is_private(name: str) -> bool:
-    parts = name.split(".")
-    return any([part.startswith("_") for part in parts])
-
-# %% ../nbs/Mkdocs.ipynb 66
-def _import_all_members(module_name: str) -> List[str]:
-    submodules = _import_submodules(module_name)
-    members: List[Tuple[str, Union[types.FunctionType, Type[Any]]]] = list(
-        itertools.chain(*[_import_functions_and_classes(m) for m in submodules])
-    )
-
-    names = [f"{y.__module__}.{y.__name__}" for x, y in members]
-    names = [
-        name for name in names if not _is_private(name) and name.startswith(module_name)
-    ]
-    return names
-
-# %% ../nbs/Mkdocs.ipynb 68
-def _merge_lists(members: List[str], submodules: List[str]) -> List[str]:
-    members_copy = members[:]
-    for sm in submodules:
-        for i, el in enumerate(members_copy):
-            if el.startswith(sm):
-                members_copy.insert(i, sm)
-                break
-    return members_copy
-
-
-def _add_all_submodules(members: List[str]) -> List[str]:
-    def _f(x: str) -> List[str]:
-        xs = x.split(".")
-        return [".".join(xs[:i]) + "." for i in range(1, len(xs))]
-
-    submodules = list(set(itertools.chain(*[_f(x) for x in members])))
-    members = _merge_lists(members, submodules)
-    members = list(dict.fromkeys(members))
-    return members
-
-# %% ../nbs/Mkdocs.ipynb 72
-def _get_api_summary_item(x: str) -> str:
-    xs = x.split(".")
-    if x.endswith("."):
-        indent = " " * (4 * (len(xs) - 1))
-        return f"{indent}- {xs[-2]}"
-    else:
-        indent = " " * (4 * (len(xs)))
-        return f"{indent}- [{xs[-1]}](api/{'/'.join(xs)}.md)"
-
-# %% ../nbs/Mkdocs.ipynb 74
-def _get_api_summary(members: List[str]) -> str:
-    return "\n".join([_get_api_summary_item(x) for x in members]) + "\n"
-
-# %% ../nbs/Mkdocs.ipynb 76
-def _get_submodule_members(module_name: str) -> List[str]:
-    """Get a list of all submodules contained within the module.
-
-    Args:
-        module_name: The name of the module to retrieve submodules from
-
-    Returns:
-        A list of submodule names within the module
-    """
-    members = _import_all_members(module_name)
-    members_with_submodules = _add_all_submodules(members)
-    members_with_submodules_str: List[str] = [
-        x[:-1] if x.endswith(".") else x for x in members_with_submodules
-    ]
-    return members_with_submodules_str
-
-# %% ../nbs/Mkdocs.ipynb 78
-def _load_submodules(
-    module_name: str, members_with_submodules: List[str]
-) -> List[Union[types.FunctionType, Type[Any]]]:
-    """Load the given submodules from the module.
-
-    Args:
-        module_name: The name of the module whose submodules to load
-        members_with_submodules: A list of submodule names to load
-
-    Returns:
-        A list of imported submodule objects.
-    """
-    submodules = _import_submodules(module_name)
-    members: List[Tuple[str, Union[types.FunctionType, Type[Any]]]] = list(
-        itertools.chain(*[_import_functions_and_classes(m) for m in submodules])
-    )
-    names = [
-        y
-        for x, y in members
-        if f"{y.__module__}.{y.__name__}" in members_with_submodules
-    ]
-    return names
-
-# %% ../nbs/Mkdocs.ipynb 80
-def _generate_api_doc(name: str, docs_path: Path) -> Path:
-    xs = name.split(".")
-    module_name = ".".join(xs[:-1])
-    member_name = xs[-1]
-    path = docs_path / f"{('/').join(xs)}.md"
-    content = f"::: {module_name}.{member_name}\n"
-
+    subpath = f"{docs_dir_name}/" + submodule.replace(".", "/") + ".md"
+    path = Path(root_path) / "mkdocs" / "docs" / subpath
     path.parent.mkdir(exist_ok=True, parents=True)
-    with open(path, "w", encoding="utf-8") as f:
-        f.write(content)
-
-    return path
-
-# %% ../nbs/Mkdocs.ipynb 82
-def _generate_api_docs(members: List[str], docs_path: Path) -> List[Path]:
-    return [_generate_api_doc(x, docs_path) for x in members if not x.endswith(".")]
-
-# %% ../nbs/Mkdocs.ipynb 84
-def _update_api_docs(
-    symbols: List[Union[types.FunctionType, Type[Any]]], docs_path: Path
-) -> None:
-    for symbol in symbols:
-        content = ""
-        content += get_formatted_docstring_for_symbol(symbol, docs_path.parent)
-        target_file_path = (
-            "/".join(f"{symbol.__module__}.{symbol.__name__}".split(".")) + ".md"
-        )
+    with open(path, "w") as f:
+        f.write(f"::: {submodule}")
+    subnames = submodule.split(".")
+    if len(subnames) > 2:
+        return " " * 4 * (len(subnames) - 2) + f"- [{subnames[-1]}]({subpath})"
+    else:
+        return f"- [{submodule}]({subpath})"
 
-        with open(
-            (Path(docs_path) / "api" / target_file_path), "w", encoding="utf-8"
-        ) as f:
-            f.write(content)
 
-# %% ../nbs/Mkdocs.ipynb 87
 def _generate_api_docs_for_module(root_path: str, module_name: str) -> str:
     """Generate API documentation for a module.
 
     Args:
         root_path: The root path of the project.
         module_name: The name of the module.
 
     Returns:
         A string containing the API documentation for the module.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    members = _import_all_members(module_name)
-    members_with_submodules = _add_all_submodules(members)
-    api_summary = _get_api_summary(members_with_submodules)
-
-    _generate_api_docs(
-        members_with_submodules, Path(root_path) / "mkdocs" / "docs" / "api"
+    submodules = _get_submodules(module_name)
+    docs_dir_name = f"{module_name}_api_docs"
+    shutil.rmtree(
+        Path(root_path) / "mkdocs" / "docs" / f"{docs_dir_name}", ignore_errors=True
     )
 
-    members_with_submodules = _get_submodule_members(module_name)
-    symbols = _load_submodules(module_name, members_with_submodules)
-
-    _update_api_docs(symbols, Path(root_path) / "mkdocs" / "docs")
-
-    return api_summary
+    if len(submodules) == 0:
+        submodules = [f"{module_name}"]
 
+    submodule_summary = "\n".join(
+        [
+            _generate_api_doc_for_submodule(
+                root_path=root_path, docs_dir_name=docs_dir_name, submodule=x
+            )
+            for x in submodules
+        ]
+    )
 
-#     return textwrap.indent(submodule_summary, prefix=" " * 4)
+    return textwrap.indent(submodule_summary, prefix=" " * 4)
 
-# %% ../nbs/Mkdocs.ipynb 89
+# %% ../nbs/Mkdocs.ipynb 70
 def _restrict_line_length(s: str, width: int = 80) -> str:
     """Restrict the line length of a string.
 
     Args:
         s: The string to be processed.
         width: The maximum line length.
 
@@ -972,15 +942,15 @@
             line = "\n".join(textwrap.wrap(line, width=width, replace_whitespace=False))
             if len(sub_block) == 1:
                 _s += line + "\n\n"
             else:
                 _s += "\n" + line + "\n" if line.endswith(":") else " " + line + "\n"
     return _s
 
-# %% ../nbs/Mkdocs.ipynb 91
+# %% ../nbs/Mkdocs.ipynb 72
 def _generate_cli_doc_for_submodule(
     root_path: str, docs_dir_name: str, cmd: str
 ) -> str:
     """Generate CLI documentation for a submodule.
 
     Args:
         root_path: The root path of the project.
@@ -1021,15 +991,15 @@
 
             cli_doc = _restrict_line_length(cli_doc)
             cli_doc = "\n```\n" + cli_doc + "\n```\n"
 
     except AttributeError as e:
         cli_doc = f"Unable to generate documentation for command. Execution of `{cli_app_name} --help` command failed."
 
-    with open(path, "w", encoding="utf-8") as f:
+    with open(path, "w") as f:
         f.write(cli_doc)
 
     return f"- [{cli_app_name}]({subpath})"
 
 
 def _generate_cli_docs_for_module(root_path: str, module_name: str) -> str:
     """Generate CLI docs for a module.
@@ -1041,15 +1011,15 @@
     Returns:
         The generated CLI docs
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    docs_dir_name = "cli"
+    docs_dir_name = f"{module_name}_cli_docs"
     shutil.rmtree(
         Path(root_path) / "mkdocs" / "docs" / f"{docs_dir_name}", ignore_errors=True
     )
     console_scripts = get_value_from_config(root_path, "console_scripts")
 
     if not console_scripts:
         ret_val = _copy_not_found_file_and_get_path(
@@ -1065,15 +1035,15 @@
             for cmd in console_scripts.split("\n")
             if cmd != ""
         ]
     )
 
     return textwrap.indent(submodule_summary, prefix=" " * 4)
 
-# %% ../nbs/Mkdocs.ipynb 95
+# %% ../nbs/Mkdocs.ipynb 76
 def _copy_change_log_if_exists(root_path: str, docs_path: Union[Path, str]) -> str:
     """Copy the CHANGELOG.md file to the docs folder if it's not already present.
 
     Args:
         root_path: The root path of the project.
         docs_path: The path to the docs folder.
 
@@ -1093,73 +1063,69 @@
     else:
         changelog = _copy_not_found_file_and_get_path(
             root_path=root_path, file_prefix="changelog"
         )
 
     return changelog
 
-# %% ../nbs/Mkdocs.ipynb 98
+# %% ../nbs/Mkdocs.ipynb 79
 def _build_summary(
     root_path: str,
     module: str,
-    cache_path: Path,
 ) -> None:
     # create docs_path if needed
     """Create a summary navigation file for generating navigation that is compatible with mkdocs.
 
     Args:
         root_path: The root path of the project.
         module: The module to generate the API documentation for.
-        cache_path: The path to the _proc directory.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     docs_path = Path(root_path) / "mkdocs" / "docs"
     docs_path.mkdir(exist_ok=True)
 
     # copy README.md as index.md
     shutil.copy(Path(root_path) / "README.md", docs_path / "index.md")
 
     # generate markdown files
-    _generate_markdown_from_files(root_path, cache_path)
+    _generate_markdown_from_files(root_path)
 
     # copy images to docs dir and update path in generated markdown files
-    _copy_images_to_docs_dir(root_path, cache_path)
+    _copy_images_to_docs_dir(root_path)
 
     # generates sidebar navigation
-    sidebar = _generate_summary_for_sidebar(root_path, cache_path)
+    sidebar = _generate_summary_for_sidebar(root_path)
 
     # generate API
     api = _generate_api_docs_for_module(root_path, module)
 
     # generate CLI
     cli = _generate_cli_docs_for_module(root_path, module)
 
     # copy CHANGELOG.md as CHANGELOG.md is exists
     changelog = _copy_change_log_if_exists(root_path, docs_path)
 
     # read summary template from file
-    with open(
-        Path(root_path) / "mkdocs" / "summary_template.txt", "r", encoding="utf-8"
-    ) as f:
+    with open(Path(root_path) / "mkdocs" / "summary_template.txt") as f:
         summary_template = f.read()
 
     summary = summary_template.format(
         sidebar=sidebar, api=api, cli=cli, changelog=changelog
     )
     summary = "\n".join(
         [l for l in [l.rstrip() for l in summary.split("\n")] if l != ""]
     )
 
-    with open(docs_path / "SUMMARY.md", mode="w", encoding="utf-8") as f:
+    with open(docs_path / "SUMMARY.md", mode="w") as f:
         f.write(summary)
 
-# %% ../nbs/Mkdocs.ipynb 101
+# %% ../nbs/Mkdocs.ipynb 82
 def _copy_cname_if_needed(root_path: str) -> None:
     """Copy the CNAME file to mkdocs/docs/CNAME if it's not already present.
 
     Args:
         root_path: The root path of the project
 
     !!! note
@@ -1175,194 +1141,107 @@
             f"File '{cname_path.resolve()}' copied to '{dst_path.resolve()}'.",
         )
     else:
         typer.secho(
             f"File '{cname_path.resolve()}' not found, skipping copying..",
         )
 
-# %% ../nbs/Mkdocs.ipynb 103
+# %% ../nbs/Mkdocs.ipynb 84
 def _copy_docs_overrides(root_path: str) -> None:
     """Copy the docs_overrides directory to the mkdocs/docs/overrides directory.
 
     Args:
         root_path: The root path of the project.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     src_path = Path(root_path) / "mkdocs" / "docs_overrides"
     dst_path = Path(root_path) / "mkdocs" / "docs" / "overrides"
 
     if not src_path.exists():
-        raise_error_and_exit(
-            f"Unexpected error: path {src_path.resolve()} does not exists!"
+        typer.secho(
+            f"Unexpected error: path {src_path.resolve()} does not exists!",
+            err=True,
+            fg=typer.colors.RED,
         )
+        raise typer.Exit(code=1)
 
     shutil.rmtree(dst_path, ignore_errors=True)
     shutil.copytree(src_path, dst_path)
 
-# %% ../nbs/Mkdocs.ipynb 105
-def _fix_sym_links_in_nbs(root_path: str, cache_path: Path, nbdev_lookup: NbdevLookup, docs_versioning: str, lib_version: str, use_relative_doc_links: bool) -> None:  # type: ignore
-    """Fix the default sym links generated by nbdev in the notebooks
-
-    Args:
-        root_path: The root path of the project.
-        cache_path: The path to the _proc directory.
-        nbdev_lookup: Instance of NbdevLookup.
-        docs_versioning: The value set for docs_versioning flag in settings.ini file.
-        lib_version: The current version of the library.
-        use_relative_doc_links: If set to True, relative links are added to symbol references in generated
-            documentation. Else, the value set in doc_host in settings.ini is added to symbol references in generated documentation.
-
-
-    !!! note
-
-        The above docstring is autogenerated by docstring-gen library (https://docstring-gen.airt.ai)
-    """
-    files = [
-        f
-        for f in cache_path.rglob("*")
-        if f.suffix == ".ipynb"
-        and not any(cache_path.startswith(".") for cache_path in f.parts)
-        and not f.name.startswith("_")
-    ]
-
-    for file in files:
-        _f = nbformat.read(file, as_version=4)
-        for cell in _f.cells:
-            if cell.cell_type == "markdown":
-                updated_src = fix_sym_links(
-                    cell["source"],
-                    nbdev_lookup,
-                    docs_versioning,
-                    lib_version,
-                    use_relative_doc_links,
-                )
-                cell["source"] = updated_src
-
-        nbformat.write(_f, file)
-
-# %% ../nbs/Mkdocs.ipynb 108
-def nbdev_mkdocs_docs(
-    root_path: str,
-    refresh_quarto_settings: bool = False,
-    use_relative_doc_links: bool = False,
-    no_mkdocs_build: bool = False,
-) -> None:
+# %% ../nbs/Mkdocs.ipynb 86
+def nbdev_mkdocs_docs(root_path: str, refresh_quarto_settings: bool = False) -> None:
     """Prepare mkdocs documentation
 
     Args:
         root_path: The root path of the project
         refresh_quarto_settings: Flag to refresh quarto yml file. This flag should be set to `True`
             if this function is called directly without calling prepare.
-        use_relative_doc_links: If set to True, relative links are added to symbol references in generated
-            documentation. Else, the value set in doc_host in settings.ini is added to symbol references in
-            generated documentation. This flag should be set to `False` if this function is called directly
-            without calling preview.
-        no_mkdocs_build: If set to True, then the mkdocs build will be skipped. This flag should be set to
-            `False` if this function is called directly without calling preview.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     with set_cwd(root_path):
+
         if refresh_quarto_settings:
             refresh_quarto_yml()
 
         _copy_cname_if_needed(root_path)
 
         _copy_docs_overrides(root_path)
 
         lib_name = get_value_from_config(root_path, "lib_name")
         lib_path = get_value_from_config(root_path, "lib_path")
 
-        cache_path = proc_nbs(force=True)
-        nbdev_lookup = NbdevLookup(incl_libs=lib_name.replace("_", "-"))
-        docs_versioning = get_value_from_config(root_path, "docs_versioning")
-        lib_version = get_value_from_config(root_path, "version")
-        _fix_sym_links_in_nbs(
-            root_path,
-            cache_path,
-            nbdev_lookup,
-            docs_versioning,
-            lib_version,
-            use_relative_doc_links,
-        )
-
-        _build_summary(root_path, lib_path, cache_path)
+        _build_summary(root_path, lib_path)
 
-        if not no_mkdocs_build:
-            cmd = f"mkdocs build -f \"{(Path(root_path) / 'mkdocs' / 'mkdocs.yml').resolve()}\""
-            _sprun(cmd)
+        cmd = f"mkdocs build -f \"{(Path(root_path) / 'mkdocs' / 'mkdocs.yml').resolve()}\""
+        _sprun(cmd)
 
 
-def prepare(
-    root_path: str,
-    use_relative_doc_links: bool = False,
-    no_test: bool = False,
-    no_mkdocs_build: bool = False,
-) -> None:
+def prepare(root_path: str, no_test: bool = False) -> None:
     """Prepare mkdocs for serving
 
     Args:
         root_path: The root path of the project
-        use_relative_doc_links: If set to True, relative links are added to symbol references in generated
-            documentation. Else, the value set in doc_host in settings.ini is added to symbol references in
-            generated documentation. This flag should be set to `False` if this function is called directly
-            without calling preview.
         no_test: If set to False, the unit tests will be run, else they will be skipped
-        no_mkdocs_build: If set to True, then the mkdocs build will be skipped. This flag
-            should be set to `False` if this function is called directly without calling preview
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     with set_cwd(root_path):
+
         if no_test:
             nbdev_export.__wrapped__()
             refresh_quarto_yml()
+            nbdev_readme.__wrapped__(chk_time=True)
         else:
-            nbdev_export.__wrapped__()
-            nbdev_test.__wrapped__()
-            nbdev_clean.__wrapped__()
-            refresh_quarto_yml()
+            cmd = "nbdev_prepare"
+            _sprun(cmd)
 
-    nbdev_mkdocs_docs(
-        root_path=root_path,
-        use_relative_doc_links=use_relative_doc_links,
-        no_mkdocs_build=no_mkdocs_build,
-    )
+    nbdev_mkdocs_docs(root_path)
 
-# %% ../nbs/Mkdocs.ipynb 111
-def preview(
-    root_path: str, use_relative_doc_links: bool, port: Optional[int] = None
-) -> None:
+# %% ../nbs/Mkdocs.ipynb 89
+def preview(root_path: str, port: Optional[int] = None) -> None:
     """Preview the mkdocs documentation.
 
     Args:
         root_path: The root path of the documentation.
-        use_relative_doc_links: If set to True, relative links are added to symbol references in generated
-            documentation. Else, the value set in doc_host in settings.ini is added to symbol references in
-            generated documentation.
         port: The port to serve the documentation on.
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     with set_cwd(root_path):
-        prepare(
-            root_path=root_path,
-            use_relative_doc_links=use_relative_doc_links,
-            no_test=True,
-            no_mkdocs_build=True,
-        )
+        prepare(root_path=root_path, no_test=True)
 
         cmd = f"mkdocs serve -f {root_path}/mkdocs/mkdocs.yml -a 0.0.0.0"
         if port:
             cmd = cmd + f":{port}"
 
         with subprocess.Popen(  # nosec B603:subprocess_without_shell_equals_true
             shlex.split(cmd),
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/custom-social-image-template.html` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/custom-social-image-template.html`

 * *Files identical despite different names*

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/compass-outline.png` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/compass-outline.png`

 * *Files identical despite different names*

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/default_social_logo.png` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template/docs_overrides/images/default_social_logo.png`

 * *Files identical despite different names*

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/package_data/mkdocs_template.yml` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/package_data/mkdocs_template.yml`

 * *Files 2% similar despite different names*

```diff
@@ -97,10 +97,8 @@
 
 extra_javascript:
   - overrides/js/extra.js
   - overrides/js/mathjax.js
   - https://polyfill.io/v3/polyfill.min.js?features=es6
   - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js  
 extra:
-  version:
-    provider: mike
   social_image: ""
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs/social_image_generator.py` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs/social_image_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from playwright.async_api import async_playwright
 from ruamel.yaml import YAML
 
 from nbdev_mkdocs._helpers.utils import (
     add_counter_suffix_to_filename,
     get_value_from_config,
     is_local_path,
-    raise_error_and_exit,
     set_cwd,
 )
 from ._package_data import get_root_data_path
 
 # %% ../nbs/Social_Image_Generator.ipynb 3
 def _generate_ai_image(prompt: str) -> str:
     """Generate an image from a prompt using OpenAI's API.
@@ -61,19 +60,20 @@
         ValueError: If root_path or image_url is None
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     with set_cwd(root_path):
+
         _custom_social_image_template_path = (
             get_root_data_path() / "custom-social-image-template.html"
         )
 
-        with open(_custom_social_image_template_path, "r", encoding="utf-8") as f:
+        with open(_custom_social_image_template_path, "r") as f:
             _html_template = f.read()
 
         user_name = get_value_from_config(root_path, "user")
         project_name = get_value_from_config(root_path, "repo")
         project_description = get_value_from_config(root_path, "description")
 
         image_url = Path(image_url).name if is_local_path(image_url) else image_url
@@ -143,16 +143,17 @@
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     html_str = _generate_html_str(root_path, image_url)
 
     with TemporaryDirectory() as d:
+
         html_path = Path(d) / "social_image.html"
-        with open(html_path, "w", encoding="utf-8") as f:
+        with open(html_path, "w") as f:
             f.write(html_str)
 
         if is_local_path(image_url):
             shutil.copyfile(Path(image_url), Path(d) / Path(image_url).name)
 
         await _capture_and_save_screenshot(d, root_path)
 
@@ -171,76 +172,75 @@
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     pattern = r":\s*!%21"
     text = re.sub(pattern, r": !!", text)
     return text
 
 # %% ../nbs/Social_Image_Generator.ipynb 15
-@contextmanager
-def _read_yaml_file(file_path: Path) -> Generator[Tuple[YAML, Any], None, None]:
-    yaml = YAML()
-    yaml.preserve_quotes = True
-
-    config = yaml.load(file_path)
-    yield yaml, config
-
-# %% ../nbs/Social_Image_Generator.ipynb 17
 def _update_social_image_in_mkdocs_yml(root_path: str, image_url: str) -> None:
     """Update social image link in mkdocs yml file
 
     Args:
         root_path: The root path
         image_url: The image url
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
     image_url = (
-        image_url
-        if "https://opengraph.githubassets.com" in image_url
-        else "overrides/images/social_image.png"
+        "overrides/images/social_image.png" if is_local_path(image_url) else image_url
     )
 
+    yaml = YAML()
     mkdocs_yml_path = Path(root_path) / "mkdocs" / "mkdocs.yml"
-    with _read_yaml_file(mkdocs_yml_path) as (yaml, config):
-        config["extra"]["social_image"] = image_url
-        yaml.dump(config, mkdocs_yml_path, transform=_unescape_exclamation_mark)
+    config = yaml.load(mkdocs_yml_path)
+    config["extra"]["social_image"] = image_url
+    yaml.dump(config, mkdocs_yml_path, transform=_unescape_exclamation_mark)
 
-# %% ../nbs/Social_Image_Generator.ipynb 19
-def _update_social_image_in_site_overrides(root_path: str) -> None:
+# %% ../nbs/Social_Image_Generator.ipynb 17
+def _update_social_image_in_site_overrides(root_path: str, image_url: str) -> None:
     """Update social image link in site_overrides HTML template
 
     Args:
         root_path: The root path of the project
+        image_url: The social image url
 
     !!! note
 
         The above docstring is autogenerated by docstring-gen library (https://github.com/airtai/docstring-gen)
     """
-    _replace_str = 'config.site_url ~ ("" if config.site_url.endswith("/") else "/") ~ config.extra.social_image '
+    _replace_str = (
+        'page.canonical_url ~ "" ~ config.extra.social_image '
+        if is_local_path(image_url)
+        else "config.extra.social_image "
+    )
+
     with set_cwd(root_path):
         site_overrides_path = (
             Path(root_path) / "mkdocs" / "site_overrides" / "main.html"
         )
         if not site_overrides_path.exists():
-            raise_error_and_exit(
-                f"Unexpected error: path {site_overrides_path.resolve()} does not exists!"
+            typer.secho(
+                f"Unexpected error: path {site_overrides_path.resolve()} does not exists!",
+                err=True,
+                fg=typer.colors.RED,
             )
+            raise typer.Exit(code=1)
 
-        with open(site_overrides_path, "r", encoding="utf-8") as f:
+        with open(site_overrides_path, "r") as f:
             _new_text = f.read()
             _pattern = re.compile(r".*?{%.*?image_url = (.*)%}")
             _match = re.search(_pattern, _new_text)
             _new_text = _new_text.replace(_match.group(1), _replace_str)  # type: ignore
 
-        with open(site_overrides_path, "w", encoding="utf-8") as f:
+        with open(site_overrides_path, "w") as f:
             f.write(_new_text)
 
-# %% ../nbs/Social_Image_Generator.ipynb 21
+# %% ../nbs/Social_Image_Generator.ipynb 20
 class _IMG_Generator(str, Enum):
     """An enumeration class for the different types of image generators.
 
     Attributes:
         file : file
         dall_e : dall_e
 
@@ -286,17 +286,20 @@
         with set_cwd(root_path):
             if image_path is not None:
                 _image_path = Path(
                     os.path.normpath(Path(root_path).joinpath(image_path))
                 ).resolve()
 
                 if not _image_path.exists():
-                    raise_error_and_exit(
-                        f"Unexpected error: path {_image_path.resolve()} does not exists!"
+                    typer.secho(
+                        f"Unexpected error: path {_image_path.resolve()} does not exists!",
+                        err=True,
+                        fg=typer.colors.RED,
                     )
+                    raise typer.Exit(code=1)
 
                 image_url = str(_image_path)
 
             else:
                 image_url = str(
                     (
                         Path(root_path)
@@ -305,15 +308,15 @@
                         / "images"
                         / "default_social_logo.png"
                     ).resolve()
                 )
 
     return image_url
 
-# %% ../nbs/Social_Image_Generator.ipynb 28
+# %% ../nbs/Social_Image_Generator.ipynb 27
 async def generate_social_image(
     root_path: str,
     generator: str = "file",
     prompt: str = "Cute animal wearing hoodie sitting in high chair in purple room, browsing computer, 3d render",
     image_path: Optional[str] = None,
 ) -> None:
     """Generate a custom image for social card using the OpenAI Image API.
@@ -330,8 +333,8 @@
     """
     image_url = _generate_image_url(root_path, generator, prompt, image_path)
 
     await _create_social_image(root_path, image_url)
 
     _update_social_image_in_mkdocs_yml(root_path, image_url)
 
-    _update_social_image_in_site_overrides(root_path)
+    _update_social_image_in_site_overrides(root_path, image_url)
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/PKG-INFO` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nbdev-mkdocs
-Version: 0.6.0rc0
+Version: 1.0.0
 Summary: Extension of nbdev for generating documentation using Material for Mkdocs instead of Quarto
 Home-page: https://github.com/airtai/nbdev-mkdocs
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python mkdocs material
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Material for nbdev
 ================
 
@@ -237,28 +237,25 @@
     ╭─ Options ────────────────────────────────────────────────────────────────────╮
     │ --install-completion          Install completion for the current shell.      │
     │ --show-completion             Show completion for the current shell, to copy │
     │                               it or customize the installation.              │
     │ --help                        Show this message and exit.                    │
     ╰──────────────────────────────────────────────────────────────────────────────╯
     ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-    │ delete-pre-release-docs  Deletes deployed pre-release documentation          │
-    │                          versions.                                           │
-    │ docs                     Prepares files in **mkdocs/docs** and then runs     │
-    │                          **mkdocs build** command on them                    │
-    │ docstring                Command for adding docstrings to classes and        │
-    │                          methods that don't have one using docstring-gen     │
-    │                          library.                                            │
-    │ new                      Creates files in **mkdocs** subdirectory needed for │
-    │                          other **nbdev_mkdocs** subcommands                  │
-    │ prepare                  Runs tests and prepares files in **mkdocs/docs**    │
-    │                          and then runs **mkdocs build** command on them      │
-    │ preview                  Prepares files in **mkdocs/docs** and then runs     │
-    │                          **mkdocs serve** command on them                    │
-    │ social-image             Command for generating a custom social share image. │
+    │ docs          Prepares files in **mkdocs/docs** and then runs **mkdocs       │
+    │               build** command on them                                        │
+    │ docstring     Command for adding docstrings to classes and methods that      │
+    │               don't have one using docstring-gen library.                    │
+    │ new           Creates files in **mkdocs** subdirectory needed for other      │
+    │               **nbdev_mkdocs** subcommands                                   │
+    │ prepare       Runs tests and prepares files in **mkdocs/docs** and then runs │
+    │               **mkdocs build** command on them                               │
+    │ preview       Prepares files in **mkdocs/docs** and then runs **mkdocs       │
+    │               serve** command on them                                        │
+    │ social-image  Command for generating a custom social share image.            │
     ╰──────────────────────────────────────────────────────────────────────────────╯
 
 #### Setup
 
 After installing nbdev-mkdocs, bootstrap your project documentation by
 executing the following command from the project’s root directory:
 
@@ -311,9 +308,7 @@
 
 Copyright © 2022 onwards airt technologies ltd, Inc.
 
 ## License
 
 This project is licensed under the terms of the [Apache License
 2.0](https://github.com/airtai/nbdev-mkdocs/blob/main/LICENSE)
-
-
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: nbdev-mkdocs Version: 0.6.0rc0 Summary: Extension
-of nbdev for generating documentation using Material for Mkdocs instead of
-Quarto Home-page: https://github.com/airtai/nbdev-mkdocs Author: airt Author-
-email: info@airt.ai License: Apache Software License 2.0 Keywords: nbdev
-jupyter notebook python mkdocs material Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
-Apache Software License Requires-Python: >=3.8 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE Material for nbdev
-================  ![](https://raw.githubusercontent.com/airtai/nbdev-mkdocs/
-main/nbs/images/nbdev_mkdocs_banner_img.png) ----------------------------------
--------------------------------------- **Documentation**: https://nbdev-
-mkdocs.airt.ai **Source Code**: https://github.com/airtai/nbdev-mkdocs --------
----------------------------------------------------------------- ## Getting
-Started ![PyPI](https://img.shields.io/pypi/v/nbdev-mkdocs.png) ![PyPI -
-Downloads](https://img.shields.io/pypi/dm/nbdev-mkdocs.png) ![PyPI - Python
-Version](https://img.shields.io/pypi/pyversions/nbdev-mkdocs.png) ![GitHub
-Workflow Status](https://img.shields.io/github/actions/workflow/status/airtai/
-nbdev-mkdocs/test.yaml) ![CodeQL](https://github.com/airtai/nbdev-mkdocs/
-actions/workflows/codeql.yml/badge.svg) ![Dependency Review](https://
-github.com/airtai/nbdev-mkdocs/actions/workflows/dependency-review.yml/
-badge.svg) ![GitHub](https://img.shields.io/github/license/airtai/nbdev-
-mkdocs.png) -------------------------------------------------------------------
------ **Material for nbdev** is a nbdev extension that allows you to use
-Material_for_MkDocs to generate documentation for nbdev projects. The key
-features are: - **Material style documentation**: Effortlessly create material
-style documentation for your nbdev projects with Material for MkDocs, a theme
-that provides a sleek and modern design for your documentation. - **Auto
-generate docstrings**: Instantly generate docstrings for your Python code using
-docstring-gen library, a tool that automatically generates docstrings for your
-functions and classes using Codex. - **Create stunning social media share
-images**: Boost your projectâs visibility by creating striking social share
-images using DALL-E. - **Customizability**: Add guides, release notes,
-customise the navigation menu and configure the Material for MkDocs easily to
-suit your project needs. With this documentation tool, you have more control
-over the look and feel of your documentation, allowing you to create a unique
-and personalized experience for your users. ### Workflow Hereâs a quick
-comparison of Quarto and Material for nbdev development workflows:
+Metadata-Version: 2.1 Name: nbdev-mkdocs Version: 1.0.0 Summary: Extension of
+nbdev for generating documentation using Material for Mkdocs instead of Quarto
+Home-page: https://github.com/airtai/nbdev-mkdocs Author: airt Author-email:
+info@airt.ai License: Apache Software License 2.0 Keywords: nbdev jupyter
+notebook python mkdocs material Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+License :: OSI Approved :: Apache Software License Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE Material for nbdev ================  ![](https://
+raw.githubusercontent.com/airtai/nbdev-mkdocs/main/nbs/images/
+nbdev_mkdocs_banner_img.png) --------------------------------------------------
+---------------------- **Documentation**: https://nbdev-mkdocs.airt.ai **Source
+Code**: https://github.com/airtai/nbdev-mkdocs --------------------------------
+---------------------------------------- ## Getting Started ![PyPI](https://
+img.shields.io/pypi/v/nbdev-mkdocs.png) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/nbdev-mkdocs.png) ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/nbdev-mkdocs.png) ![GitHub Workflow Status]
+(https://img.shields.io/github/actions/workflow/status/airtai/nbdev-mkdocs/
+test.yaml) ![CodeQL](https://github.com/airtai/nbdev-mkdocs/actions/workflows/
+codeql.yml/badge.svg) ![Dependency Review](https://github.com/airtai/nbdev-
+mkdocs/actions/workflows/dependency-review.yml/badge.svg) ![GitHub](https://
+img.shields.io/github/license/airtai/nbdev-mkdocs.png) ------------------------
+------------------------------------------------ **Material for nbdev** is a
+nbdev extension that allows you to use Material_for_MkDocs to generate
+documentation for nbdev projects. The key features are: - **Material style
+documentation**: Effortlessly create material style documentation for your
+nbdev projects with Material for MkDocs, a theme that provides a sleek and
+modern design for your documentation. - **Auto generate docstrings**: Instantly
+generate docstrings for your Python code using docstring-gen library, a tool
+that automatically generates docstrings for your functions and classes using
+Codex. - **Create stunning social media share images**: Boost your projectâs
+visibility by creating striking social share images using DALL-E. -
+**Customizability**: Add guides, release notes, customise the navigation menu
+and configure the Material for MkDocs easily to suit your project needs. With
+this documentation tool, you have more control over the look and feel of your
+documentation, allowing you to create a unique and personalized experience for
+your users. ### Workflow Hereâs a quick comparison of Quarto and Material for
+nbdev development workflows:
 Quarto workflow                                      Material for nbdev workflow
 Install: ``` shell $ pip install notebook nbdev $    Install: ``` shell $ pip install notebook nbdev $
 nbdev_install_quarto ```                             nbdev_install_quarto $ pip install nbdev-mkdocs ```
 Setup: ``` shell $ nbdev_new $ nbdev_install_hooks $ Setup: ``` shell $ nbdev_new $ nbdev_install_hooks $ vi
 vi settings.ini $ pip install -e '.[dev]' ```        settings.ini $ pip install -e '.[dev]' $ nbdev_mkdocs
                                                      new $ vi mkdocs/mkdocs.yml ```
 Development: ``` shell # Edit files $ nbdev_preview  Development: ``` shell # Edit files $ nbdev_mkdocs
@@ -62,24 +63,23 @@
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --install-completion Install completion for the current shell. â â --
 show-completion Show completion for the current shell, to copy â â it or
 customize the installation. â â --help Show this message and exit. â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 â­â Commands
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
-â delete-pre-release-docs Deletes deployed pre-release documentation â â
-versions. â â docs Prepares files in **mkdocs/docs** and then runs â â
-**mkdocs build** command on them â â docstring Command for adding
-docstrings to classes and â â methods that don't have one using docstring-
-gen â â library. â â new Creates files in **mkdocs** subdirectory
-needed for â â other **nbdev_mkdocs** subcommands â â prepare Runs
-tests and prepares files in **mkdocs/docs** â â and then runs **mkdocs
-build** command on them â â preview Prepares files in **mkdocs/docs** and
-then runs â â **mkdocs serve** command on them â â social-image Command
-for generating a custom social share image. â
+â docs Prepares files in **mkdocs/docs** and then runs **mkdocs â â
+build** command on them â â docstring Command for adding docstrings to
+classes and methods that â â don't have one using docstring-gen library.
+â â new Creates files in **mkdocs** subdirectory needed for other â â
+**nbdev_mkdocs** subcommands â â prepare Runs tests and prepares files in
+**mkdocs/docs** and then runs â â **mkdocs build** command on them â â
+preview Prepares files in **mkdocs/docs** and then runs **mkdocs â â
+serve** command on them â â social-image Command for generating a custom
+social share image. â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 #### Setup After installing nbdev-mkdocs, bootstrap your project documentation
 by executing the following command from the projectâs root directory: ```
 shell nbdev_mkdocs new ``` Using information from the projectâs settings.ini
 file, the above command creates files and directories required to build the
 documentation and saves it in the **mkdocs** subdirectory. Note: You should
 only run the **nbdev_mkdocs new** command once for the project to initialise
```

### Comparing `nbdev-mkdocs-0.6.0rc0/nbdev_mkdocs.egg-info/SOURCES.txt` & `nbdev-mkdocs-1.0.0/nbdev_mkdocs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 nbdev_mkdocs.egg-info/SOURCES.txt
 nbdev_mkdocs.egg-info/dependency_links.txt
 nbdev_mkdocs.egg-info/entry_points.txt
 nbdev_mkdocs.egg-info/not-zip-safe
 nbdev_mkdocs.egg-info/requires.txt
 nbdev_mkdocs.egg-info/top_level.txt
 nbdev_mkdocs/_helpers/__init__.py
-nbdev_mkdocs/_helpers/api_docs_helper.py
 nbdev_mkdocs/_helpers/cli_doc.py
-nbdev_mkdocs/_helpers/doc_links_utils.py
-nbdev_mkdocs/_helpers/quarto_to_mkdocs.py
 nbdev_mkdocs/_helpers/utils.py
 nbdev_mkdocs/package_data/changelog_not_found.md
 nbdev_mkdocs/package_data/cli_commands_not_found.md
 nbdev_mkdocs/package_data/custom-social-image-template.html
 nbdev_mkdocs/package_data/ghp_deploy_action_template.yml
 nbdev_mkdocs/package_data/gitignore.txt
 nbdev_mkdocs/package_data/mkdocs_template.yml
```

### Comparing `nbdev-mkdocs-0.6.0rc0/settings.ini` & `nbdev-mkdocs-1.0.0/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = nbdev-mkdocs
 lib_name = %(repo)s
-version = 0.6.0rc0
-min_python = 3.8
+version = 1.0.0
+min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = nbdev_mkdocs
 nbs_path = nbs
 recursive = True
@@ -21,56 +21,49 @@
 ### Docs ###
 branch = main
 custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
-# Documentation versioning level ("None", "minor", "patch"). Recommended: "minor"
-docs_versioning = minor
 
 ### PyPI ###
 audience = Developers
 author = airt
 author_email = info@airt.ai
 copyright = 2022 onwards, %(author)s
 description = Extension of nbdev for generating documentation using Material for Mkdocs instead of Quarto
 keywords = nbdev jupyter notebook python mkdocs material
 language = English
 status = 3
 user = airtai
 
-
 ### Optional ###
 requirements =     \
-    nbdev==2.3.12 \
+    nbdev>=2.3.9 \
     typer[all]>=0.7.0 \
     mkdocs>=1.4.2 \
-    mkdocstrings[python]>=0.20.0 \
-    mkdocs-material>=9.1.1 \
-    mkdocs-literate-nav>=0.6.0 \
+    mkdocstrings==0.18.1 \
+    mkdocs-material>=8.5.11 \
+    mkdocs-literate-nav>=0.5.0 \
     mkdocs-section-index>=0.3.4 \
     configupdater>=3.1.1 \
     griffe>=0.24.1 \
     ruamel.yaml>=0.17.21 \
-    openai>=0.27.2 \
+    openai>=0.25.0 \
     playwright>=1.28.0 \
-    docstring-gen>=0.3.0 \
-    mypy-extensions>=0.4.3 \
-    mike>=1.1.2 \
-    nbformat>=5.8.0
+    docstring-gen>=0.2.0 \
+    mypy-extensions>=0.4.3
 
 dev_requirements = \
-    bandit==1.7.4 \
-    semgrep==1.14.0 \
-    pytest==7.2.1 \
-    nbqa==1.5.3 \
-    black==23.1.0 \
-    mypy==1.0.1 \
-    isort==5.11.5 \
-    pre-commit==2.21.0 \
-    detect-secrets==1.4.0 \
-    pandas>=1.3.5,<2.0.0 \
-    numpy>=1.21.6
+    bandit>=1.7.4 \
+    semgrep>=0.115.0 \
+    pytest>=7.1.3 \
+    numpy>=1.0 \
+    black>=22.8.0 \
+    mypy>=0.960 \
+    nbqa>=1.5.3 \
+    isort>=5.11.4 \
+    pre-commit>=2.21.0 \
     
 
 console_scripts = nbdev_mkdocs=nbdev_mkdocs._cli:_app
```

### Comparing `nbdev-mkdocs-0.6.0rc0/setup.py` & `nbdev-mkdocs-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md', 'r', encoding='utf-8').read(),
+    long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
         'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
     },
     **setup_cfg)
```

