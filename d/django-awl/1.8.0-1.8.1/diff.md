# Comparing `tmp/django-awl-1.8.0.tar.gz` & `tmp/django-awl-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-awl-1.8.0.tar", last modified: Thu Mar 16 15:40:05 2023, max compression
+gzip compressed data, was "django-awl-1.8.1.tar", last modified: Thu Jun 29 20:46:24 2023, max compression
```

## Comparing `django-awl-1.8.0.tar` & `django-awl-1.8.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.425900 django-awl-1.8.0/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2018-09-23 18:34:37.000000 django-awl-1.8.0/LICENSE
--rw-r--r--   0 ctrudeau   (501) staff       (20)       35 2018-09-23 18:34:37.000000 django-awl-1.8.0/MANIFEST.in
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1493 2023-03-16 15:40:05.425389 django-awl-1.8.0/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      583 2023-03-16 15:39:19.000000 django-awl-1.8.0/README.rst
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.410357 django-awl-1.8.0/awl/
--rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2023-03-16 13:43:29.000000 django-awl-1.8.0/awl/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      906 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/absmodels.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    27475 2022-06-29 00:03:28.000000 django-awl-1.8.0/awl/admintools.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      506 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/context_processors.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     8468 2020-11-05 15:10:46.000000 django-awl-1.8.0/awl/css_colours.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     4036 2018-11-22 15:36:22.000000 django-awl-1.8.0/awl/decorators.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      930 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/logtools.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.410673 django-awl-1.8.0/awl/management/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/management/__init__.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.412782 django-awl-1.8.0/awl/management/commands/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/management/commands/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2816 2019-07-26 20:05:33.000000 django-awl-1.8.0/awl/management/commands/create_cmd.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      514 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/management/commands/create_test_admin.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      924 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/management/commands/print_setting.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      685 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/management/commands/run_script.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1228 2019-07-26 17:26:45.000000 django-awl-1.8.0/awl/management/commands/wipe_migrations.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.413489 django-awl-1.8.0/awl/migrations/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1238 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/migrations/0001_initial.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/migrations/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6906 2020-04-18 17:18:50.000000 django-awl-1.8.0/awl/models.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.415552 django-awl-1.8.0/awl/rankedmodel/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/rankedmodel/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2944 2020-06-12 15:49:39.000000 django-awl-1.8.0/awl/rankedmodel/admintools.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5580 2022-07-17 16:25:59.000000 django-awl-1.8.0/awl/rankedmodel/models.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      197 2021-12-20 20:40:36.000000 django-awl-1.8.0/awl/rankedmodel/urls.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1133 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/rankedmodel/views.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.416735 django-awl-1.8.0/awl/templatetags/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/templatetags/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     7229 2023-03-16 15:27:52.000000 django-awl-1.8.0/awl/templatetags/awltags.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.422751 django-awl-1.8.0/awl/tests/
--rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/tests/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3643 2022-06-28 23:47:42.000000 django-awl-1.8.0/awl/tests/admin.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3718 2022-06-28 23:20:34.000000 django-awl-1.8.0/awl/tests/models.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      573 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/tests/test_absmodels.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     9193 2022-06-28 23:48:59.000000 django-awl-1.8.0/awl/tests/test_admintools.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2633 2020-11-05 15:11:33.000000 django-awl-1.8.0/awl/tests/test_colours.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3152 2020-04-02 18:23:25.000000 django-awl-1.8.0/awl/tests/test_commands.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      536 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/tests/test_contextproc.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2140 2018-11-22 15:35:02.000000 django-awl-1.8.0/awl/tests/test_decorators.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      330 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/tests/test_logtools.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2311 2020-04-02 18:32:38.000000 django-awl-1.8.0/awl/tests/test_models.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     7938 2020-06-12 20:44:18.000000 django-awl-1.8.0/awl/tests/test_ranked.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5054 2023-03-16 15:25:33.000000 django-awl-1.8.0/awl/tests/test_tags.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     3111 2020-08-21 14:23:27.000000 django-awl-1.8.0/awl/tests/test_utils.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6141 2023-03-16 15:36:49.000000 django-awl-1.8.0/awl/tests/test_waelsteng.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      348 2021-12-20 20:41:19.000000 django-awl-1.8.0/awl/tests/urls.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)      363 2018-09-23 18:34:37.000000 django-awl-1.8.0/awl/tests/views.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6331 2020-08-21 14:23:28.000000 django-awl-1.8.0/awl/utils.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11508 2021-12-20 20:34:56.000000 django-awl-1.8.0/awl/waelsteng.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-16 15:40:05.424871 django-awl-1.8.0/django_awl.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1493 2023-03-16 15:40:05.000000 django-awl-1.8.0/django_awl.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1317 2023-03-16 15:40:05.000000 django-awl-1.8.0/django_awl.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-03-16 15:40:05.000000 django-awl-1.8.0/django_awl.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       65 2023-03-16 15:40:05.000000 django-awl-1.8.0/django_awl.egg-info/requires.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        4 2023-03-16 15:40:05.000000 django-awl-1.8.0/django_awl.egg-info/top_level.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-03-16 15:40:05.426036 django-awl-1.8.0/setup.cfg
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1545 2023-03-16 13:46:53.000000 django-awl-1.8.0/setup.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.254359 django-awl-1.8.1/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1087 2018-09-23 18:34:37.000000 django-awl-1.8.1/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       35 2018-09-23 18:34:37.000000 django-awl-1.8.1/MANIFEST.in
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1499 2023-06-29 20:46:24.254091 django-awl-1.8.1/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      589 2023-06-29 20:45:05.000000 django-awl-1.8.1/README.rst
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.241017 django-awl-1.8.1/awl/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2023-06-29 20:44:48.000000 django-awl-1.8.1/awl/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      906 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/absmodels.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    27475 2022-06-29 00:03:28.000000 django-awl-1.8.1/awl/admintools.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      506 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/context_processors.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     8468 2020-11-05 15:10:46.000000 django-awl-1.8.1/awl/css_colours.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     4036 2018-11-22 15:36:22.000000 django-awl-1.8.1/awl/decorators.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      930 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/logtools.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.241330 django-awl-1.8.1/awl/management/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/management/__init__.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.243060 django-awl-1.8.1/awl/management/commands/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/management/commands/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2816 2019-07-26 20:05:33.000000 django-awl-1.8.1/awl/management/commands/create_cmd.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      514 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/management/commands/create_test_admin.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      924 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/management/commands/print_setting.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      685 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/management/commands/run_script.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1228 2019-07-26 17:26:45.000000 django-awl-1.8.1/awl/management/commands/wipe_migrations.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.243632 django-awl-1.8.1/awl/migrations/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1238 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/migrations/0001_initial.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/migrations/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6906 2020-04-18 17:18:50.000000 django-awl-1.8.1/awl/models.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.245052 django-awl-1.8.1/awl/rankedmodel/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/rankedmodel/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2944 2020-06-12 15:49:39.000000 django-awl-1.8.1/awl/rankedmodel/admintools.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5580 2022-07-17 16:25:59.000000 django-awl-1.8.1/awl/rankedmodel/models.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      197 2021-12-20 20:40:36.000000 django-awl-1.8.1/awl/rankedmodel/urls.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1133 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/rankedmodel/views.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.245605 django-awl-1.8.1/awl/templatetags/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/templatetags/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     7229 2023-03-16 15:27:52.000000 django-awl-1.8.1/awl/templatetags/awltags.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.251662 django-awl-1.8.1/awl/tests/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        0 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/tests/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3643 2022-06-28 23:47:42.000000 django-awl-1.8.1/awl/tests/admin.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3718 2022-06-28 23:20:34.000000 django-awl-1.8.1/awl/tests/models.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      573 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/tests/test_absmodels.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     9193 2022-06-28 23:48:59.000000 django-awl-1.8.1/awl/tests/test_admintools.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2633 2020-11-05 15:11:33.000000 django-awl-1.8.1/awl/tests/test_colours.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3152 2020-04-02 18:23:25.000000 django-awl-1.8.1/awl/tests/test_commands.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      536 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/tests/test_contextproc.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2140 2018-11-22 15:35:02.000000 django-awl-1.8.1/awl/tests/test_decorators.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      330 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/tests/test_logtools.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2311 2020-04-02 18:32:38.000000 django-awl-1.8.1/awl/tests/test_models.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     7938 2020-06-12 20:44:18.000000 django-awl-1.8.1/awl/tests/test_ranked.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5054 2023-03-16 15:25:33.000000 django-awl-1.8.1/awl/tests/test_tags.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     3111 2020-08-21 14:23:27.000000 django-awl-1.8.1/awl/tests/test_utils.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6141 2023-03-16 15:36:49.000000 django-awl-1.8.1/awl/tests/test_waelsteng.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      348 2021-12-20 20:41:19.000000 django-awl-1.8.1/awl/tests/urls.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      363 2018-09-23 18:34:37.000000 django-awl-1.8.1/awl/tests/views.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6331 2020-08-21 14:23:28.000000 django-awl-1.8.1/awl/utils.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11508 2021-12-20 20:34:56.000000 django-awl-1.8.1/awl/waelsteng.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-29 20:46:24.253595 django-awl-1.8.1/django_awl.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1499 2023-06-29 20:46:23.000000 django-awl-1.8.1/django_awl.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1317 2023-06-29 20:46:23.000000 django-awl-1.8.1/django_awl.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-06-29 20:46:23.000000 django-awl-1.8.1/django_awl.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       65 2023-06-29 20:46:23.000000 django-awl-1.8.1/django_awl.egg-info/requires.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        4 2023-06-29 20:46:23.000000 django-awl-1.8.1/django_awl.egg-info/top_level.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-06-29 20:46:24.254445 django-awl-1.8.1/setup.cfg
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1545 2023-03-16 13:46:53.000000 django-awl-1.8.1/setup.py
```

### Comparing `django-awl-1.8.0/LICENSE` & `django-awl-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/PKG-INFO` & `django-awl-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-awl
-Version: 1.8.0
+Version: 1.8.1
 Summary: Miscellaneous django tools
 Home-page: https://github.com/cltrudeau/django-awl
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
 Keywords: django,state machine
 Classifier: Development Status :: 4 - Beta
@@ -38,16 +38,16 @@
 
 Supports
 ========
 
 django-awl has been tested with:
 
 * Django 3.2 using Python 3.7, 3.8, 3.9, 3.10
-* Django 4.0 using Python 3.8, 3.9, 3.10
 * Django 4.1 using Python 3.8, 3.9, 3.10, 3.11
+* Django 4.2 using Python 3.8, 3.9, 3.10, 3.11
 
 
 Docs & Source
 =============
 
 Docs: http://django-awl.readthedocs.io/en/latest/
```

### Comparing `django-awl-1.8.0/README.rst` & `django-awl-1.8.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 Supports
 ========
 
 django-awl has been tested with:
 
 * Django 3.2 using Python 3.7, 3.8, 3.9, 3.10
-* Django 4.0 using Python 3.8, 3.9, 3.10
 * Django 4.1 using Python 3.8, 3.9, 3.10, 3.11
+* Django 4.2 using Python 3.8, 3.9, 3.10, 3.11
 
 
 Docs & Source
 =============
 
 Docs: http://django-awl.readthedocs.io/en/latest/
```

### Comparing `django-awl-1.8.0/awl/absmodels.py` & `django-awl-1.8.1/awl/absmodels.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/admintools.py` & `django-awl-1.8.1/awl/admintools.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/css_colours.py` & `django-awl-1.8.1/awl/css_colours.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/decorators.py` & `django-awl-1.8.1/awl/decorators.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/logtools.py` & `django-awl-1.8.1/awl/logtools.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/management/commands/create_cmd.py` & `django-awl-1.8.1/awl/management/commands/create_cmd.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/management/commands/create_test_admin.py` & `django-awl-1.8.1/awl/management/commands/create_test_admin.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/management/commands/print_setting.py` & `django-awl-1.8.1/awl/management/commands/print_setting.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/management/commands/run_script.py` & `django-awl-1.8.1/awl/management/commands/run_script.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/management/commands/wipe_migrations.py` & `django-awl-1.8.1/awl/management/commands/wipe_migrations.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/migrations/0001_initial.py` & `django-awl-1.8.1/awl/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/models.py` & `django-awl-1.8.1/awl/models.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/rankedmodel/admintools.py` & `django-awl-1.8.1/awl/rankedmodel/admintools.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/rankedmodel/models.py` & `django-awl-1.8.1/awl/rankedmodel/models.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/rankedmodel/views.py` & `django-awl-1.8.1/awl/rankedmodel/views.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/templatetags/awltags.py` & `django-awl-1.8.1/awl/templatetags/awltags.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/admin.py` & `django-awl-1.8.1/awl/tests/admin.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/models.py` & `django-awl-1.8.1/awl/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_absmodels.py` & `django-awl-1.8.1/awl/tests/test_absmodels.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_admintools.py` & `django-awl-1.8.1/awl/tests/test_admintools.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_colours.py` & `django-awl-1.8.1/awl/tests/test_colours.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_commands.py` & `django-awl-1.8.1/awl/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_contextproc.py` & `django-awl-1.8.1/awl/tests/test_contextproc.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_decorators.py` & `django-awl-1.8.1/awl/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_models.py` & `django-awl-1.8.1/awl/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_ranked.py` & `django-awl-1.8.1/awl/tests/test_ranked.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_tags.py` & `django-awl-1.8.1/awl/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_utils.py` & `django-awl-1.8.1/awl/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/tests/test_waelsteng.py` & `django-awl-1.8.1/awl/tests/test_waelsteng.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/utils.py` & `django-awl-1.8.1/awl/utils.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/awl/waelsteng.py` & `django-awl-1.8.1/awl/waelsteng.py`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/django_awl.egg-info/PKG-INFO` & `django-awl-1.8.1/django_awl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-awl
-Version: 1.8.0
+Version: 1.8.1
 Summary: Miscellaneous django tools
 Home-page: https://github.com/cltrudeau/django-awl
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
 Keywords: django,state machine
 Classifier: Development Status :: 4 - Beta
@@ -38,16 +38,16 @@
 
 Supports
 ========
 
 django-awl has been tested with:
 
 * Django 3.2 using Python 3.7, 3.8, 3.9, 3.10
-* Django 4.0 using Python 3.8, 3.9, 3.10
 * Django 4.1 using Python 3.8, 3.9, 3.10, 3.11
+* Django 4.2 using Python 3.8, 3.9, 3.10, 3.11
 
 
 Docs & Source
 =============
 
 Docs: http://django-awl.readthedocs.io/en/latest/
```

### Comparing `django-awl-1.8.0/django_awl.egg-info/SOURCES.txt` & `django-awl-1.8.1/django_awl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-awl-1.8.0/setup.py` & `django-awl-1.8.1/setup.py`

 * *Files identical despite different names*

