# Comparing `tmp/wagtail-transcription-0.0.8.tar.gz` & `tmp/wagtail-transcription-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-transcription-0.0.8.tar", last modified: Wed Nov  2 15:06:28 2022, max compression
+gzip compressed data, was "wagtail-transcription-0.0.9.tar", last modified: Wed Nov  2 16:51:39 2022, max compression
```

## Comparing `wagtail-transcription-0.0.8.tar` & `wagtail-transcription-0.0.9.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.553010 wagtail-transcription-0.0.8/
--rw-r--r--   0 kuba       (501) staff       (20)     1067 2022-09-13 08:54:53.000000 wagtail-transcription-0.0.8/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)      135 2022-09-13 08:59:43.000000 wagtail-transcription-0.0.8/MANIFEST.in
--rw-r--r--   0 kuba       (501) staff       (20)     7180 2022-11-02 15:06:28.553092 wagtail-transcription-0.0.8/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     6604 2022-10-24 10:48:43.000000 wagtail-transcription-0.0.8/README.md
--rw-r--r--   0 kuba       (501) staff       (20)      103 2022-09-13 11:30:49.000000 wagtail-transcription-0.0.8/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)      696 2022-11-02 15:06:28.553444 wagtail-transcription-0.0.8/setup.cfg
--rw-r--r--   0 kuba       (501) staff       (20)       37 2022-09-13 09:01:34.000000 wagtail-transcription-0.0.8/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.545209 wagtail-transcription-0.0.8/tests/
--rw-r--r--   0 kuba       (501) staff       (20)       39 2022-09-12 20:46:17.000000 wagtail-transcription-0.0.8/tests/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     1526 2022-09-12 12:15:22.000000 wagtail-transcription-0.0.8/tests/test_template_tags.py
--rw-r--r--   0 kuba       (501) staff       (20)     1647 2022-09-12 11:43:28.000000 wagtail-transcription-0.0.8/tests/test_transcription_model.py
--rw-r--r--   0 kuba       (501) staff       (20)     3884 2022-09-13 06:49:11.000000 wagtail-transcription-0.0.8/tests/test_views.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.547096 wagtail-transcription-0.0.8/wagtail_transcription/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-12 20:37:18.000000 wagtail-transcription-0.0.8/wagtail_transcription/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      173 2022-09-12 20:56:35.000000 wagtail-transcription-0.0.8/wagtail_transcription/apps.py
--rw-r--r--   0 kuba       (501) staff       (20)     3018 2022-09-15 16:28:45.000000 wagtail-transcription-0.0.8/wagtail_transcription/edit_handlers.py
--rw-r--r--   0 kuba       (501) staff       (20)       42 2022-11-02 14:24:17.000000 wagtail-transcription-0.0.8/wagtail_transcription/exceptions.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.548529 wagtail-transcription-0.0.8/wagtail_transcription/migrations/
--rw-r--r--   0 kuba       (501) staff       (20)     2375 2022-09-08 12:15:27.000000 wagtail-transcription-0.0.8/wagtail_transcription/migrations/0001_initial.py
--rw-r--r--   0 kuba       (501) staff       (20)      407 2022-09-12 10:41:00.000000 wagtail-transcription-0.0.8/wagtail_transcription/migrations/0002_alter_transcription_options.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-07 15:07:17.000000 wagtail-transcription-0.0.8/wagtail_transcription/migrations/__init__.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.548913 wagtail-transcription-0.0.8/wagtail_transcription/models/
--rw-r--r--   0 kuba       (501) staff       (20)       40 2022-09-07 15:44:23.000000 wagtail-transcription-0.0.8/wagtail_transcription/models/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     1641 2022-09-12 10:46:56.000000 wagtail-transcription-0.0.8/wagtail_transcription/models/transcription.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.542454 wagtail-transcription-0.0.8/wagtail_transcription/static/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.542614 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.542544 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.549916 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/
--rw-r--r--   0 kuba       (501) staff       (20)     2765 2022-09-12 08:24:52.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/change_transcription_field.js
--rw-r--r--   0 kuba       (501) staff       (20)      259 2022-09-08 12:10:56.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/fetch_message.js
--rw-r--r--   0 kuba       (501) staff       (20)     2221 2022-09-09 06:25:05.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/notify.js
--rw-r--r--   0 kuba       (501) staff       (20)     4582 2022-11-02 14:10:07.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/transcription.js
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.542661 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.550648 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/
--rw-r--r--   0 kuba       (501) staff       (20)      649 2022-09-05 10:11:04.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/fetch_message.css
--rw-r--r--   0 kuba       (501) staff       (20)     1524 2022-09-06 09:30:48.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/notify.css
--rw-r--r--   0 kuba       (501) staff       (20)      884 2022-09-06 10:54:41.000000 wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/transcription.css
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.542884 wagtail-transcription-0.0.8/wagtail_transcription/templates/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.542819 wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtail_transcription/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.550870 wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtail_transcription/widgets/
--rw-r--r--   0 kuba       (501) staff       (20)     1344 2022-10-24 09:57:09.000000 wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtail_transcription/widgets/transcription.html
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.551140 wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtailadmin/
--rw-r--r--   0 kuba       (501) staff       (20)     3266 2022-09-12 08:21:23.000000 wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtailadmin/base.html
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.551478 wagtail-transcription-0.0.8/wagtail_transcription/templatetags/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-07 15:21:03.000000 wagtail-transcription-0.0.8/wagtail_transcription/templatetags/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      467 2022-09-15 16:48:14.000000 wagtail-transcription-0.0.8/wagtail_transcription/templatetags/transcription_tags.py
--rw-r--r--   0 kuba       (501) staff       (20)     1683 2022-09-15 17:19:57.000000 wagtail-transcription-0.0.8/wagtail_transcription/urls.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.551794 wagtail-transcription-0.0.8/wagtail_transcription/utils/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-29 21:12:08.000000 wagtail-transcription-0.0.8/wagtail_transcription/utils/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     2302 2022-11-02 13:50:57.000000 wagtail-transcription-0.0.8/wagtail_transcription/utils/validation_errors.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.552751 wagtail-transcription-0.0.8/wagtail_transcription/views/
--rw-r--r--   0 kuba       (501) staff       (20)       57 2022-09-07 16:22:26.000000 wagtail-transcription-0.0.8/wagtail_transcription/views/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     9358 2022-11-02 14:53:55.000000 wagtail-transcription-0.0.8/wagtail_transcription/views/mixins.py
--rw-r--r--   0 kuba       (501) staff       (20)      632 2022-09-09 06:23:46.000000 wagtail-transcription-0.0.8/wagtail_transcription/views/notifications.py
--rw-r--r--   0 kuba       (501) staff       (20)    14723 2022-11-02 14:55:38.000000 wagtail-transcription-0.0.8/wagtail_transcription/views/transcription.py
--rw-r--r--   0 kuba       (501) staff       (20)     4290 2022-11-02 12:53:40.000000 wagtail-transcription-0.0.8/wagtail_transcription/wagtail_hooks.py
--rw-r--r--   0 kuba       (501) staff       (20)      498 2022-09-13 06:49:54.000000 wagtail-transcription-0.0.8/wagtail_transcription/widgets.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 15:06:28.547809 wagtail-transcription-0.0.8/wagtail_transcription.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     7180 2022-11-02 15:06:28.000000 wagtail-transcription-0.0.8/wagtail_transcription.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     1939 2022-11-02 15:06:28.000000 wagtail-transcription-0.0.8/wagtail_transcription.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2022-11-02 15:06:28.000000 wagtail-transcription-0.0.8/wagtail_transcription.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       59 2022-11-02 15:06:28.000000 wagtail-transcription-0.0.8/wagtail_transcription.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)       28 2022-11-02 15:06:28.000000 wagtail-transcription-0.0.8/wagtail_transcription.egg-info/top_level.txt
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.017612 wagtail-transcription-0.0.9/
+-rw-r--r--   0 kuba       (501) staff       (20)     1067 2022-09-13 08:54:53.000000 wagtail-transcription-0.0.9/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)      135 2022-09-13 08:59:43.000000 wagtail-transcription-0.0.9/MANIFEST.in
+-rw-r--r--   0 kuba       (501) staff       (20)     7180 2022-11-02 16:51:39.017704 wagtail-transcription-0.0.9/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     6604 2022-10-24 10:48:43.000000 wagtail-transcription-0.0.9/README.md
+-rw-r--r--   0 kuba       (501) staff       (20)      103 2022-09-13 11:30:49.000000 wagtail-transcription-0.0.9/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)      696 2022-11-02 16:51:39.018002 wagtail-transcription-0.0.9/setup.cfg
+-rw-r--r--   0 kuba       (501) staff       (20)       37 2022-09-13 09:01:34.000000 wagtail-transcription-0.0.9/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.009129 wagtail-transcription-0.0.9/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)       39 2022-09-12 20:46:17.000000 wagtail-transcription-0.0.9/tests/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1526 2022-09-12 12:15:22.000000 wagtail-transcription-0.0.9/tests/test_template_tags.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1647 2022-09-12 11:43:28.000000 wagtail-transcription-0.0.9/tests/test_transcription_model.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3884 2022-09-13 06:49:11.000000 wagtail-transcription-0.0.9/tests/test_views.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.011438 wagtail-transcription-0.0.9/wagtail_transcription/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-12 20:37:18.000000 wagtail-transcription-0.0.9/wagtail_transcription/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      173 2022-09-12 20:56:35.000000 wagtail-transcription-0.0.9/wagtail_transcription/apps.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1012 2022-11-02 16:48:26.000000 wagtail-transcription-0.0.9/wagtail_transcription/decorators.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3018 2022-09-15 16:28:45.000000 wagtail-transcription-0.0.9/wagtail_transcription/edit_handlers.py
+-rw-r--r--   0 kuba       (501) staff       (20)       42 2022-11-02 14:24:17.000000 wagtail-transcription-0.0.9/wagtail_transcription/exceptions.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.013114 wagtail-transcription-0.0.9/wagtail_transcription/migrations/
+-rw-r--r--   0 kuba       (501) staff       (20)     2375 2022-09-08 12:15:27.000000 wagtail-transcription-0.0.9/wagtail_transcription/migrations/0001_initial.py
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2022-09-12 10:41:00.000000 wagtail-transcription-0.0.9/wagtail_transcription/migrations/0002_alter_transcription_options.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-07 15:07:17.000000 wagtail-transcription-0.0.9/wagtail_transcription/migrations/__init__.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.013597 wagtail-transcription-0.0.9/wagtail_transcription/models/
+-rw-r--r--   0 kuba       (501) staff       (20)       40 2022-09-07 15:44:23.000000 wagtail-transcription-0.0.9/wagtail_transcription/models/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1641 2022-09-12 10:46:56.000000 wagtail-transcription-0.0.9/wagtail_transcription/models/transcription.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.005929 wagtail-transcription-0.0.9/wagtail_transcription/static/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.006094 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.006024 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.014683 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/
+-rw-r--r--   0 kuba       (501) staff       (20)     2765 2022-09-12 08:24:52.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/change_transcription_field.js
+-rw-r--r--   0 kuba       (501) staff       (20)      259 2022-09-08 12:10:56.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/fetch_message.js
+-rw-r--r--   0 kuba       (501) staff       (20)     2221 2022-09-09 06:25:05.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/notify.js
+-rw-r--r--   0 kuba       (501) staff       (20)     4582 2022-11-02 14:10:07.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/transcription.js
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.006141 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.015400 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/
+-rw-r--r--   0 kuba       (501) staff       (20)      649 2022-09-05 10:11:04.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/fetch_message.css
+-rw-r--r--   0 kuba       (501) staff       (20)     1524 2022-09-06 09:30:48.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/notify.css
+-rw-r--r--   0 kuba       (501) staff       (20)      884 2022-09-06 10:54:41.000000 wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/transcription.css
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.006361 wagtail-transcription-0.0.9/wagtail_transcription/templates/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.006299 wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtail_transcription/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.015634 wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtail_transcription/widgets/
+-rw-r--r--   0 kuba       (501) staff       (20)     1344 2022-10-24 09:57:09.000000 wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtail_transcription/widgets/transcription.html
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.015888 wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtailadmin/
+-rw-r--r--   0 kuba       (501) staff       (20)     3266 2022-09-12 08:21:23.000000 wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtailadmin/base.html
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.016220 wagtail-transcription-0.0.9/wagtail_transcription/templatetags/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-07 15:21:03.000000 wagtail-transcription-0.0.9/wagtail_transcription/templatetags/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      467 2022-09-15 16:48:14.000000 wagtail-transcription-0.0.9/wagtail_transcription/templatetags/transcription_tags.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2221 2022-11-02 16:50:18.000000 wagtail-transcription-0.0.9/wagtail_transcription/urls.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.016539 wagtail-transcription-0.0.9/wagtail_transcription/utils/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2022-09-29 21:12:08.000000 wagtail-transcription-0.0.9/wagtail_transcription/utils/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2302 2022-11-02 13:50:57.000000 wagtail-transcription-0.0.9/wagtail_transcription/utils/validation_errors.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.017502 wagtail-transcription-0.0.9/wagtail_transcription/views/
+-rw-r--r--   0 kuba       (501) staff       (20)       57 2022-09-07 16:22:26.000000 wagtail-transcription-0.0.9/wagtail_transcription/views/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9358 2022-11-02 14:53:55.000000 wagtail-transcription-0.0.9/wagtail_transcription/views/mixins.py
+-rw-r--r--   0 kuba       (501) staff       (20)      632 2022-09-09 06:23:46.000000 wagtail-transcription-0.0.9/wagtail_transcription/views/notifications.py
+-rw-r--r--   0 kuba       (501) staff       (20)    14723 2022-11-02 16:05:01.000000 wagtail-transcription-0.0.9/wagtail_transcription/views/transcription.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4290 2022-11-02 12:53:40.000000 wagtail-transcription-0.0.9/wagtail_transcription/wagtail_hooks.py
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2022-09-13 06:49:54.000000 wagtail-transcription-0.0.9/wagtail_transcription/widgets.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2022-11-02 16:51:39.012361 wagtail-transcription-0.0.9/wagtail_transcription.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     7180 2022-11-02 16:51:38.000000 wagtail-transcription-0.0.9/wagtail_transcription.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     1975 2022-11-02 16:51:38.000000 wagtail-transcription-0.0.9/wagtail_transcription.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2022-11-02 16:51:38.000000 wagtail-transcription-0.0.9/wagtail_transcription.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       59 2022-11-02 16:51:38.000000 wagtail-transcription-0.0.9/wagtail_transcription.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       28 2022-11-02 16:51:38.000000 wagtail-transcription-0.0.9/wagtail_transcription.egg-info/top_level.txt
```

### Comparing `wagtail-transcription-0.0.8/LICENSE` & `wagtail-transcription-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/PKG-INFO` & `wagtail-transcription-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-transcription
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/LilJack118/wagtail-transcription
 Author: LilJack118
 Author-email: jakub@kachange.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LilJack118/wagtail-transcription/issues
 Keywords: wagtail django
```

### Comparing `wagtail-transcription-0.0.8/README.md` & `wagtail-transcription-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/setup.cfg` & `wagtail-transcription-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-transcription
-version = 0.0.8
+version = 0.0.9
 author = LilJack118
 author_email = jakub@kachange.com
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/LilJack118/wagtail-transcription
 project_urls = 
 	Bug Tracker = https://github.com/LilJack118/wagtail-transcription/issues
```

### Comparing `wagtail-transcription-0.0.8/tests/test_template_tags.py` & `wagtail-transcription-0.0.9/tests/test_template_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/tests/test_transcription_model.py` & `wagtail-transcription-0.0.9/tests/test_transcription_model.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/tests/test_views.py` & `wagtail-transcription-0.0.9/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/edit_handlers.py` & `wagtail-transcription-0.0.9/wagtail_transcription/edit_handlers.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/migrations/0001_initial.py` & `wagtail-transcription-0.0.9/wagtail_transcription/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/models/transcription.py` & `wagtail-transcription-0.0.9/wagtail_transcription/models/transcription.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/change_transcription_field.js` & `wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/change_transcription_field.js`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/notify.js` & `wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/notify.js`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/js/widgets/transcription.js` & `wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/js/widgets/transcription.js`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/fetch_message.css` & `wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/fetch_message.css`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/notify.css` & `wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/notify.css`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/static/wagtail_transcription/style/widgets/transcription.css` & `wagtail-transcription-0.0.9/wagtail_transcription/static/wagtail_transcription/style/widgets/transcription.css`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtail_transcription/widgets/transcription.html` & `wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtail_transcription/widgets/transcription.html`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/templates/wagtailadmin/base.html` & `wagtail-transcription-0.0.9/wagtail_transcription/templates/wagtailadmin/base.html`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/urls.py` & `wagtail-transcription-0.0.9/wagtail_transcription/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,69 @@
 from django.urls import path, re_path
 from django.urls import path
 from .views import (
-    ValidateTranscriptionDataView, 
-    RequestTranscriptionView, 
-    ReceiveTranscriptionView, 
-    DeleteNotificationView, 
-    GetProcessingTranscriptionsView, 
-    GetTranscriptionData
+    ValidateTranscriptionDataView,
+    RequestTranscriptionView,
+    ReceiveTranscriptionView,
+    DeleteNotificationView,
+    GetProcessingTranscriptionsView,
+    GetTranscriptionData,
 )
-from django.contrib.admin.views.decorators import staff_member_required
 from django.utils.module_loading import import_string
 from django.conf import settings
+from .decorators import staff_or_group_required
 
-if hasattr(settings, 'RECEIVE_TRANSCRIPTION_VIEW'):
+if hasattr(settings, "RECEIVE_TRANSCRIPTION_VIEW"):
     ReceiveTranscriptionView = import_string(settings.RECEIVE_TRANSCRIPTION)
-if hasattr(settings, 'REQUEST_TRANSCRIPTION_VIEW'):
+if hasattr(settings, "REQUEST_TRANSCRIPTION_VIEW"):
     RequestTranscriptionView = import_string(settings.REQUEST_TRANSCRIPTION_VIEW)
 
-app_name = 'wagtail_transcription'
+app_name = "wagtail_transcription"
 urlpatterns = [
     # Transcription Urls
-    path('validate_transcription_data/', staff_member_required(ValidateTranscriptionDataView.as_view()), name='validate_transcription_data'),
-    path('request_transcription/', staff_member_required(RequestTranscriptionView.as_view()), name='request_transcription'),
-    path('processing_transcriptions/', staff_member_required(GetProcessingTranscriptionsView.as_view()), name='processing_transcriptions'),
-    path('transcription_data/', staff_member_required(GetTranscriptionData.as_view()), name='transcription_data'),
-    re_path(r'^receive_transcription/(?P<m>[0-9A-Za-z_/-]+)/(?P<t>[0-9A-Za-z_/-]+)/(?P<f>[0-9A-Za-z_/-]+)/(?P<e>[0-9A-Za-z_/-]+)/(?P<v>[0-9A-Za-z_-]+)/(?P<u>[0-9]+)?$', ReceiveTranscriptionView.as_view(), name='receive_transcription'),
+    path(
+        "validate_transcription_data/",
+        staff_or_group_required(
+            ValidateTranscriptionDataView.as_view(),
+            group_names=["moderators", "editors"],
+        ),
+        name="validate_transcription_data",
+    ),
+    path(
+        "request_transcription/",
+        staff_or_group_required(
+            RequestTranscriptionView.as_view(),
+            group_names=["moderators", "editors"],
+        ),
+        name="request_transcription",
+    ),
+    path(
+        "processing_transcriptions/",
+        staff_or_group_required(
+            GetProcessingTranscriptionsView.as_view(),
+            group_names=["moderators", "editors"],
+        ),
+        name="processing_transcriptions",
+    ),
+    path(
+        "transcription_data/",
+        staff_or_group_required(
+            GetTranscriptionData.as_view(),
+            group_names=["moderators", "editors"],
+        ),
+        name="transcription_data",
+    ),
+    re_path(
+        r"^receive_transcription/(?P<m>[0-9A-Za-z_/-]+)/(?P<t>[0-9A-Za-z_/-]+)/(?P<f>[0-9A-Za-z_/-]+)/(?P<e>[0-9A-Za-z_/-]+)/(?P<v>[0-9A-Za-z_-]+)/(?P<u>[0-9]+)?$",
+        ReceiveTranscriptionView.as_view(),
+        name="receive_transcription",
+    ),
     # Notification Urls
-    path('delete_notification/', staff_member_required(DeleteNotificationView.as_view()), name='delete_notification'),
+    path(
+        "delete_notification/",
+        staff_or_group_required(
+            DeleteNotificationView.as_view(),
+            group_names=["moderators", "editors"],
+        ),
+        name="delete_notification",
+    ),
 ]
```

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/utils/validation_errors.py` & `wagtail-transcription-0.0.9/wagtail_transcription/utils/validation_errors.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/views/mixins.py` & `wagtail-transcription-0.0.9/wagtail_transcription/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/views/notifications.py` & `wagtail-transcription-0.0.9/wagtail_transcription/views/notifications.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/views/transcription.py` & `wagtail-transcription-0.0.9/wagtail_transcription/views/transcription.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                 with transaction.atomic():
                     # create transcription with completed=False
                     Transcription.objects.create(
                         title=f"auto_transcription-{video_id}",
                         video_id=video_id,
                     )
                     response = self.request_audio_transcription(
-                        "https://invalid_url", webhook_url
+                        data.get("audio_url"), webhook_url
                     )
                     # if response do not have header raise error
                     if response.get("id") is None:
                         error_msg = response.get("error")
                         raise ValueError()
             except Exception as e:
                 print(e)
```

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription/wagtail_hooks.py` & `wagtail-transcription-0.0.9/wagtail_transcription/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription.egg-info/PKG-INFO` & `wagtail-transcription-0.0.9/wagtail_transcription.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-transcription
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/LilJack118/wagtail-transcription
 Author: LilJack118
 Author-email: jakub@kachange.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LilJack118/wagtail-transcription/issues
 Keywords: wagtail django
```

### Comparing `wagtail-transcription-0.0.8/wagtail_transcription.egg-info/SOURCES.txt` & `wagtail-transcription-0.0.9/wagtail_transcription.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 tests/__init__.py
 tests/test_template_tags.py
 tests/test_transcription_model.py
 tests/test_views.py
 wagtail_transcription/__init__.py
 wagtail_transcription/apps.py
+wagtail_transcription/decorators.py
 wagtail_transcription/edit_handlers.py
 wagtail_transcription/exceptions.py
 wagtail_transcription/urls.py
 wagtail_transcription/wagtail_hooks.py
 wagtail_transcription/widgets.py
 wagtail_transcription.egg-info/PKG-INFO
 wagtail_transcription.egg-info/SOURCES.txt
```

