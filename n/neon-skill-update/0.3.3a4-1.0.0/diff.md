# Comparing `tmp/neon-skill-update-0.3.3a4.tar.gz` & `tmp/neon-skill-update-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-0.3.3a4.tar", last modified: Mon Jun 26 17:02:59 2023, max compression
+gzip compressed data, was "neon-skill-update-1.0.0.tar", last modified: Thu Jun 29 16:58:45 2023, max compression
```

## Comparing `neon-skill-update-0.3.3a4.tar` & `neon-skill-update-1.0.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.609878 neon-skill-update-0.3.3a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-26 17:02:59.609878 neon-skill-update-0.3.3a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.601878 neon-skill-update-0.3.3a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.601878 neon-skill-update-0.3.3a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_update_failure.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_update_success.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:02:59.609878 neon-skill-update-0.3.3a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.091940 neon-skill-update-1.0.0/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.091940 neon-skill-update-1.0.0/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.095940 neon-skill-update-1.0.0/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.095940 neon-skill-update-1.0.0/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.095940 neon-skill-update-1.0.0/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 16:58:45.000000 neon-skill-update-1.0.0/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:58:45.099940 neon-skill-update-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 16:58:42.000000 neon-skill-update-1.0.0/version.py
```

### Comparing `neon-skill-update-0.3.3a4/LICENSE.md` & `neon-skill-update-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/PKG-INFO` & `neon-skill-update-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 0.3.3a4
+Version: 1.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-0.3.3a4/README.md` & `neon-skill-update-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/__init__.py` & `neon-skill-update-1.0.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-1.0.0/neon_skill_update.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 0.3.3a4
+Version: 1.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-0.3.3a4/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-1.0.0/neon_skill_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/setup.py` & `neon-skill-update-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/skill.json` & `neon-skill-update-1.0.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/test/test_skill.py` & `neon-skill-update-1.0.0/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a4/version.py` & `neon-skill-update-1.0.0/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.3a4"
+__version__ = "1.0.0"
```

