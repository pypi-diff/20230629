# Comparing `tmp/djangocms-audio-2.0.0.tar.gz` & `tmp/djangocms-audio-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangocms-audio-2.0.0.tar", last modified: Wed Sep  2 13:44:52 2020, max compression
+gzip compressed data, was "djangocms-audio-2.1.0.tar", last modified: Thu Jun 29 13:09:46 2023, max compression
```

## Comparing `djangocms-audio-2.0.0.tar` & `djangocms-audio-2.1.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.738243 djangocms-audio-2.0.0/
--rw-r--r--   0 finalangel   (501) staff       (20)     1475 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/LICENSE
--rw-r--r--   0 finalangel   (501) staff       (20)      196 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/MANIFEST.in
--rw-r--r--   0 finalangel   (501) staff       (20)     5919 2020-09-02 13:44:52.737687 djangocms-audio-2.0.0/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     3783 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/README.rst
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.545714 djangocms-audio-2.0.0/djangocms_audio/
--rw-r--r--   0 finalangel   (501) staff       (20)       22 2020-09-02 13:44:12.000000 djangocms-audio-2.0.0/djangocms_audio/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3228 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/djangocms_audio/cms_plugins.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.514571 djangocms-audio-2.0.0/djangocms_audio/locale/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.513682 djangocms-audio-2.0.0/djangocms_audio/locale/de/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.565965 djangocms-audio-2.0.0/djangocms_audio/locale/de/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     1856 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2716 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.513945 djangocms-audio-2.0.0/djangocms_audio/locale/en/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.567237 djangocms-audio-2.0.0/djangocms_audio/locale/en/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     1714 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2566 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.514187 djangocms-audio-2.0.0/djangocms_audio/locale/es/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.568623 djangocms-audio-2.0.0/djangocms_audio/locale/es/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2227 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.514423 djangocms-audio-2.0.0/djangocms_audio/locale/fr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.581005 djangocms-audio-2.0.0/djangocms_audio/locale/fr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     1885 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2744 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.514659 djangocms-audio-2.0.0/djangocms_audio/locale/it/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.601166 djangocms-audio-2.0.0/djangocms_audio/locale/it/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2227 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.629714 djangocms-audio-2.0.0/djangocms_audio/migrations/
--rw-r--r--   0 finalangel   (501) staff       (20)     4180 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/djangocms_audio/migrations/0001_initial.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1596 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/djangocms_audio/migrations/0002_auto_20160825_1821.py
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/djangocms_audio/migrations/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     5528 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/djangocms_audio/models.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.515061 djangocms-audio-2.0.0/djangocms_audio/templates/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.515241 djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.663307 djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/
--rw-r--r--   0 finalangel   (501) staff       (20)      325 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/audio_player.html
--rw-r--r--   0 finalangel   (501) staff       (20)      911 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/file.html
--rw-r--r--   0 finalangel   (501) staff       (20)      740 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/folder.html
--rw-r--r--   0 finalangel   (501) staff       (20)      630 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/track.html
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.559401 djangocms-audio-2.0.0/djangocms_audio.egg-info/
--rw-r--r--   0 finalangel   (501) staff       (20)     5919 2020-09-02 13:44:52.000000 djangocms-audio-2.0.0/djangocms_audio.egg-info/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     1344 2020-09-02 13:44:52.000000 djangocms-audio-2.0.0/djangocms_audio.egg-info/SOURCES.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:44:52.000000 djangocms-audio-2.0.0/djangocms_audio.egg-info/dependency_links.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:44:52.000000 djangocms-audio-2.0.0/djangocms_audio.egg-info/not-zip-safe
--rw-r--r--   0 finalangel   (501) staff       (20)       64 2020-09-02 13:44:52.000000 djangocms-audio-2.0.0/djangocms_audio.egg-info/requires.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       22 2020-09-02 13:44:52.000000 djangocms-audio-2.0.0/djangocms_audio.egg-info/top_level.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       38 2020-09-02 13:44:52.738393 djangocms-audio-2.0.0/setup.cfg
--rw-r--r--   0 finalangel   (501) staff       (20)     1610 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/setup.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:44:52.730311 djangocms-audio-2.0.0/tests/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/tests/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3235 2020-08-18 13:25:38.000000 djangocms-audio-2.0.0/tests/helpers.py
--rw-r--r--   0 finalangel   (501) staff       (20)      430 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/tests/settings.py
--rw-r--r--   0 finalangel   (501) staff       (20)      885 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/tests/test_migrations.py
--rw-r--r--   0 finalangel   (501) staff       (20)     6264 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/tests/test_models.py
--rw-r--r--   0 finalangel   (501) staff       (20)     4730 2020-09-02 08:29:39.000000 djangocms-audio-2.0.0/tests/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/djangocms_audio/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/0002_auto_20160825_1821.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/0003_alter_audiofile_cmsplugin_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/audio_player.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/folder.html
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/track.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/test_plugins.py
```

### Comparing `djangocms-audio-2.0.0/LICENSE` & `djangocms-audio-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/PKG-INFO` & `djangocms-audio-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,150 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangocms-audio
-Version: 2.0.0
+Version: 2.1.0
 Summary: Adds audio plugin to django CMS.
-Home-page: https://github.com/divio/djangocms-audio
+Home-page: https://github.com/django-cms/djangocms-audio
 Author: Divio AG
 Author-email: info@divio.com
+Maintainer: Django CMS Association and contributors
+Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Description: ================
-        django CMS Audio
-        ================
-        
-        |pypi| |build| |coverage|
-        
-        **django CMS Audio** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allow you to publish audio files on your site (using an HTML5 player by default,
-        but you can override this in your own templates if required).
-        
-        It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
-        The plugins allow you to select a single file or an entire folder of files.
-        
-        This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-        `django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
-        for easy installation.
-        
-        .. image:: preview.gif
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. Before submitting your
-        pull request, please review our `contribution guidelines
-        <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        Contributors are listed at the `contributors <https://github.com/divio/djangocms-audio/graphs/contributors>`_
-        section.
-        
-        One of the easiest contributions you can make is helping to translate this addon on
-        `Transifex <https://www.transifex.com/projects/p/djangocms-audio/>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-audio/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        |python| |django| |djangocms|
-        
-        * Django Filer 1.7 or higher
-        
-        Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-audio``
-        * add ``djangocms_audio`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_audio``
-        
-        
-        Configuration
-        -------------
-        
-        Note that the provided templates are very minimal by design. You are encouraged
-        to adapt and override them to your project's requirements.
-        
-        This addon provides a ``default`` template for all instances. You can provide
-        additional template choices by adding a ``DJANGOCMS_AUDIO_TEMPLATES``
-        setting::
-        
-            DJANGOCMS_AUDIO_TEMPLATES = [
-                ('feature', _('Featured Version')),
-            ]
-        
-        You'll need to create the `feature` folder inside ``templates/djangocms_audio/``
-        otherwise you will get a *template does not exist* error. You can do this by
-        copying the ``default`` folder inside that directory and renaming it to
-        ``feature``.
-        
-        ``MP3`` and ``OGG`` files are allowed by default. We recommend using ``MP3``
-        as it's supported across all major browsers. You can change the default
-        setting by overriding::
-        
-            DJANGOCMS_AUDIO_ALLOWED_EXTENSIONS = ['mp3', 'ogg', 'wav']
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r tests/requirements.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-audio.svg
-            :target: http://badge.fury.io/py/djangocms-audio
-        .. |build| image:: https://travis-ci.org/divio/djangocms-audio.svg?branch=master
-            :target: https://travis-ci.org/divio/djangocms-audio
-        .. |coverage| image:: https://codecov.io/gh/divio/djangocms-audio/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/divio/djangocms-audio
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
-            :target: https://pypi.org/project/djangocms-audio/
-        .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
-            :target: https://www.djangoproject.com/
-        .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
-            :target: https://www.django-cms.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
+Classifier: Framework :: Django CMS :: 3.9
+Classifier: Framework :: Django CMS :: 3.10
+Classifier: Framework :: Django CMS :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+================
+django CMS Audio
+================
+
+|pypi| |build| |coverage|
+
+**django CMS Audio** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allow you to publish audio files on your site (using an HTML5 player by default,
+but you can override this in your own templates if required).
+
+It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
+The plugins allow you to select a single file or an entire folder of files.
+
+.. note:: 
+
+    This project is considered 3rd party (no supervision by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_). Join us on `Slack                 <https://www.django-cms.org/slack/>`_ for more information.
+
+.. image:: preview.gif
+
+
+*******************************************
+Contribute to this project and win rewards
+*******************************************
+
+Because this is a an open-source project, we welcome everyone to
+`get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution. 
+Become part of a fantastic community and help us make django CMS the best CMS in the world.   
+
+We'll be delighted to receive your
+feedback in the form of issues and pull requests. Before submitting your
+pull request, please review our `contribution guidelines
+<http://docs.django-cms.org/en/latest/contributing/index.html>`_.
+
+We're grateful to all contributors who have helped create and maintain this package.
+Contributors are listed at the `contributors <https://github.com/django-cms/djangocms-audio/graphs/contributors>`_
+section.
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-audio/blob/master/setup.py>`_
+file for additional dependencies:
+
+|python| |django| |djangocms|
+
+* Django Filer 1.7 or higher
+
+Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-audio``
+* add ``djangocms_audio`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_audio``
+
+
+Configuration
+-------------
+
+Note that the provided templates are very minimal by design. You are encouraged
+to adapt and override them to your project's requirements.
+
+This addon provides a ``default`` template for all instances. You can provide
+additional template choices by adding a ``DJANGOCMS_AUDIO_TEMPLATES``
+setting::
+
+    DJANGOCMS_AUDIO_TEMPLATES = [
+        ('feature', _('Featured Version')),
+    ]
+
+You'll need to create the `feature` folder inside ``templates/djangocms_audio/``
+otherwise you will get a *template does not exist* error. You can do this by
+copying the ``default`` folder inside that directory and renaming it to
+``feature``.
+
+``MP3`` and ``OGG`` files are allowed by default. We recommend using ``MP3``
+as it's supported across all major browsers. You can change the default
+setting by overriding::
+
+    DJANGOCMS_AUDIO_ALLOWED_EXTENSIONS = ['mp3', 'ogg', 'wav']
+
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r tests/requirements.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-audio.svg
+    :target: http://badge.fury.io/py/djangocms-audio
+.. |build| image:: https://travis-ci.org/divio/djangocms-audio.svg?branch=master
+    :target: https://travis-ci.org/divio/djangocms-audio
+.. |coverage| image:: https://codecov.io/gh/divio/djangocms-audio/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/divio/djangocms-audio
+
+.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+    :target: https://pypi.org/project/djangocms-audio/
+.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+    :target: https://www.djangoproject.com/
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+    :target: https://www.django-cms.org/
```

### Comparing `djangocms-audio-2.0.0/README.rst` & `djangocms-audio-2.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -7,37 +7,39 @@
 **django CMS Audio** is a set of plugins for `django CMS <http://django-cms.org>`_
 that allow you to publish audio files on your site (using an HTML5 player by default,
 but you can override this in your own templates if required).
 
 It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
 The plugins allow you to select a single file or an entire folder of files.
 
-This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-`django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
-for easy installation.
+.. note:: 
+
+    This project is considered 3rd party (no supervision by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_). Join us on `Slack                 <https://www.django-cms.org/slack/>`_ for more information.
 
 .. image:: preview.gif
 
 
-Contributing
-============
+*******************************************
+Contribute to this project and win rewards
+*******************************************
+
+Because this is a an open-source project, we welcome everyone to
+`get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution. 
+Become part of a fantastic community and help us make django CMS the best CMS in the world.   
 
-This is a an open-source project. We'll be delighted to receive your
+We'll be delighted to receive your
 feedback in the form of issues and pull requests. Before submitting your
 pull request, please review our `contribution guidelines
 <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
 
 We're grateful to all contributors who have helped create and maintain this package.
-Contributors are listed at the `contributors <https://github.com/divio/djangocms-audio/graphs/contributors>`_
+Contributors are listed at the `contributors <https://github.com/django-cms/djangocms-audio/graphs/contributors>`_
 section.
 
-One of the easiest contributions you can make is helping to translate this addon on
-`Transifex <https://www.transifex.com/projects/p/djangocms-audio/>`_.
-
-
 Documentation
 =============
 
 See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-audio/blob/master/setup.py>`_
 file for additional dependencies:
 
 |python| |django| |djangocms|
```

### Comparing `djangocms-audio-2.0.0/djangocms_audio/cms_plugins.py` & `djangocms-audio-2.1.0/djangocms_audio/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from django.utils.translation import gettext_lazy as _
-
 from cms.plugin_base import CMSPluginBase
 from cms.plugin_pool import plugin_pool
+from django.utils.translation import gettext_lazy as _
 
 from . import models
 
 
 class AudioPlayerPlugin(CMSPluginBase):
     model = models.AudioPlayer
     name = _('Audio player')
@@ -29,15 +28,15 @@
 
     def render(self, context, instance, placeholder):
         context = super().render(context, instance, placeholder)
         context['audio_template'] = instance.template
         return context
 
     def get_render_template(self, context, instance, placeholder):
-        return 'djangocms_audio/{}/audio_player.html'.format(instance.template)
+        return f'djangocms_audio/{instance.template}/audio_player.html'
 
 
 class AudioFilePlugin(CMSPluginBase):
     model = models.AudioFile
     name = _('File')
     module = _('Audio player')
     allow_children = True
```

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/de/LC_MESSAGES/django.mo` & `djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/de/LC_MESSAGES/django.po` & `djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/en/LC_MESSAGES/django.mo` & `djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/en/LC_MESSAGES/django.po` & `djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/es/LC_MESSAGES/django.po` & `djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/fr/LC_MESSAGES/django.mo` & `djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/fr/LC_MESSAGES/django.po` & `djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/locale/it/LC_MESSAGES/django.po` & `djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/migrations/0001_initial.py` & `djangocms-audio-2.1.0/djangocms_audio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/migrations/0002_auto_20160825_1821.py` & `djangocms-audio-2.1.0/djangocms_audio/migrations/0002_auto_20160825_1821.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/models.py` & `djangocms-audio-2.1.0/djangocms_audio/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Enables the user to add an "Audio player" plugin that serves as
 a wrapper rendering the player and its options.
 
 The "Audio player" plugin allows to add either a single "File" or a reference
 to a "Folder" as children.
 """
+from cms.models import CMSPlugin
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
-
-from cms.models import CMSPlugin
-
 from djangocms_attributes_field.fields import AttributesField
 from filer.fields.file import FilerFileField
 from filer.fields.folder import FilerFolderField
 
 
 # mp3 is supported by all major browsers
 def get_extensions():
@@ -194,9 +192,9 @@
         verbose_name=_('Attributes'),
         blank=True,
     )
 
     def __str__(self):
         label = self.kind
         if self.srclang:
-            label += ' ({})'.format(self.srclang)
+            label += f' ({self.srclang})'
         return label
```

### Comparing `djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/file.html` & `djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/file.html`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/folder.html` & `djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/folder.html`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio/templates/djangocms_audio/default/track.html` & `djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/track.html`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/djangocms_audio.egg-info/PKG-INFO` & `djangocms-audio-2.1.0/djangocms_audio.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,150 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangocms-audio
-Version: 2.0.0
+Version: 2.1.0
 Summary: Adds audio plugin to django CMS.
-Home-page: https://github.com/divio/djangocms-audio
+Home-page: https://github.com/django-cms/djangocms-audio
 Author: Divio AG
 Author-email: info@divio.com
+Maintainer: Django CMS Association and contributors
+Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Description: ================
-        django CMS Audio
-        ================
-        
-        |pypi| |build| |coverage|
-        
-        **django CMS Audio** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allow you to publish audio files on your site (using an HTML5 player by default,
-        but you can override this in your own templates if required).
-        
-        It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
-        The plugins allow you to select a single file or an entire folder of files.
-        
-        This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-        `django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-googlemap/>`_
-        for easy installation.
-        
-        .. image:: preview.gif
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. Before submitting your
-        pull request, please review our `contribution guidelines
-        <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        Contributors are listed at the `contributors <https://github.com/divio/djangocms-audio/graphs/contributors>`_
-        section.
-        
-        One of the easiest contributions you can make is helping to translate this addon on
-        `Transifex <https://www.transifex.com/projects/p/djangocms-audio/>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-audio/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        |python| |django| |djangocms|
-        
-        * Django Filer 1.7 or higher
-        
-        Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-audio``
-        * add ``djangocms_audio`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_audio``
-        
-        
-        Configuration
-        -------------
-        
-        Note that the provided templates are very minimal by design. You are encouraged
-        to adapt and override them to your project's requirements.
-        
-        This addon provides a ``default`` template for all instances. You can provide
-        additional template choices by adding a ``DJANGOCMS_AUDIO_TEMPLATES``
-        setting::
-        
-            DJANGOCMS_AUDIO_TEMPLATES = [
-                ('feature', _('Featured Version')),
-            ]
-        
-        You'll need to create the `feature` folder inside ``templates/djangocms_audio/``
-        otherwise you will get a *template does not exist* error. You can do this by
-        copying the ``default`` folder inside that directory and renaming it to
-        ``feature``.
-        
-        ``MP3`` and ``OGG`` files are allowed by default. We recommend using ``MP3``
-        as it's supported across all major browsers. You can change the default
-        setting by overriding::
-        
-            DJANGOCMS_AUDIO_ALLOWED_EXTENSIONS = ['mp3', 'ogg', 'wav']
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r tests/requirements.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-audio.svg
-            :target: http://badge.fury.io/py/djangocms-audio
-        .. |build| image:: https://travis-ci.org/divio/djangocms-audio.svg?branch=master
-            :target: https://travis-ci.org/divio/djangocms-audio
-        .. |coverage| image:: https://codecov.io/gh/divio/djangocms-audio/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/divio/djangocms-audio
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
-            :target: https://pypi.org/project/djangocms-audio/
-        .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
-            :target: https://www.djangoproject.com/
-        .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
-            :target: https://www.django-cms.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
+Classifier: Framework :: Django CMS :: 3.9
+Classifier: Framework :: Django CMS :: 3.10
+Classifier: Framework :: Django CMS :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+================
+django CMS Audio
+================
+
+|pypi| |build| |coverage|
+
+**django CMS Audio** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allow you to publish audio files on your site (using an HTML5 player by default,
+but you can override this in your own templates if required).
+
+It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
+The plugins allow you to select a single file or an entire folder of files.
+
+.. note:: 
+
+    This project is considered 3rd party (no supervision by the `django CMS Association <https://www.django-cms.org/en/about-us/>`_). Join us on `Slack                 <https://www.django-cms.org/slack/>`_ for more information.
+
+.. image:: preview.gif
+
+
+*******************************************
+Contribute to this project and win rewards
+*******************************************
+
+Because this is a an open-source project, we welcome everyone to
+`get involved in the project <https://www.django-cms.org/en/contribute/>`_ and
+`receive a reward <https://www.django-cms.org/en/bounty-program/>`_ for their contribution. 
+Become part of a fantastic community and help us make django CMS the best CMS in the world.   
+
+We'll be delighted to receive your
+feedback in the form of issues and pull requests. Before submitting your
+pull request, please review our `contribution guidelines
+<http://docs.django-cms.org/en/latest/contributing/index.html>`_.
+
+We're grateful to all contributors who have helped create and maintain this package.
+Contributors are listed at the `contributors <https://github.com/django-cms/djangocms-audio/graphs/contributors>`_
+section.
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-audio/blob/master/setup.py>`_
+file for additional dependencies:
+
+|python| |django| |djangocms|
+
+* Django Filer 1.7 or higher
+
+Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-audio``
+* add ``djangocms_audio`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_audio``
+
+
+Configuration
+-------------
+
+Note that the provided templates are very minimal by design. You are encouraged
+to adapt and override them to your project's requirements.
+
+This addon provides a ``default`` template for all instances. You can provide
+additional template choices by adding a ``DJANGOCMS_AUDIO_TEMPLATES``
+setting::
+
+    DJANGOCMS_AUDIO_TEMPLATES = [
+        ('feature', _('Featured Version')),
+    ]
+
+You'll need to create the `feature` folder inside ``templates/djangocms_audio/``
+otherwise you will get a *template does not exist* error. You can do this by
+copying the ``default`` folder inside that directory and renaming it to
+``feature``.
+
+``MP3`` and ``OGG`` files are allowed by default. We recommend using ``MP3``
+as it's supported across all major browsers. You can change the default
+setting by overriding::
+
+    DJANGOCMS_AUDIO_ALLOWED_EXTENSIONS = ['mp3', 'ogg', 'wav']
+
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r tests/requirements.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-audio.svg
+    :target: http://badge.fury.io/py/djangocms-audio
+.. |build| image:: https://travis-ci.org/divio/djangocms-audio.svg?branch=master
+    :target: https://travis-ci.org/divio/djangocms-audio
+.. |coverage| image:: https://codecov.io/gh/divio/djangocms-audio/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/divio/djangocms-audio
+
+.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+    :target: https://pypi.org/project/djangocms-audio/
+.. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
+    :target: https://www.djangoproject.com/
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+    :target: https://www.django-cms.org/
```

### Comparing `djangocms-audio-2.0.0/djangocms_audio.egg-info/SOURCES.txt` & `djangocms-audio-2.1.0/djangocms_audio.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 djangocms_audio/__init__.py
 djangocms_audio/cms_plugins.py
 djangocms_audio/models.py
 djangocms_audio.egg-info/PKG-INFO
 djangocms_audio.egg-info/SOURCES.txt
 djangocms_audio.egg-info/dependency_links.txt
@@ -19,14 +20,15 @@
 djangocms_audio/locale/es/LC_MESSAGES/django.po
 djangocms_audio/locale/fr/LC_MESSAGES/django.mo
 djangocms_audio/locale/fr/LC_MESSAGES/django.po
 djangocms_audio/locale/it/LC_MESSAGES/django.mo
 djangocms_audio/locale/it/LC_MESSAGES/django.po
 djangocms_audio/migrations/0001_initial.py
 djangocms_audio/migrations/0002_auto_20160825_1821.py
+djangocms_audio/migrations/0003_alter_audiofile_cmsplugin_ptr_and_more.py
 djangocms_audio/migrations/__init__.py
 djangocms_audio/templates/djangocms_audio/default/audio_player.html
 djangocms_audio/templates/djangocms_audio/default/file.html
 djangocms_audio/templates/djangocms_audio/default/folder.html
 djangocms_audio/templates/djangocms_audio/default/track.html
 tests/__init__.py
 tests/helpers.py
```

### Comparing `djangocms-audio-2.0.0/tests/helpers.py` & `djangocms-audio-2.1.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/tests/test_migrations.py` & `djangocms-audio-2.1.0/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/tests/test_models.py` & `djangocms-audio-2.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.0.0/tests/test_plugins.py` & `djangocms-audio-2.1.0/tests/test_plugins.py`

 * *Files identical despite different names*

