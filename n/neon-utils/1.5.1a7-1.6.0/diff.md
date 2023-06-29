# Comparing `tmp/neon-utils-1.5.1a7.tar.gz` & `tmp/neon-utils-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-utils-1.5.1a7.tar", last modified: Tue Jun 27 00:50:47 2023, max compression
+gzip compressed data, was "neon-utils-1.6.0.tar", last modified: Thu Jun 29 17:07:13 2023, max compression
```

## Comparing `neon-utils-1.5.1a7.tar` & `neon-utils-1.6.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.458493 neon-utils-1.5.1a7/neon_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/authentication_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68558 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.462494 neon-utils-1.5.1a7/neon_utils/default_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/default_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/default_configurations/default_user_conf.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/location_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/messagebus_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/mq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/process_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.450493 neon-utils-1.5.1a7/neon_utils/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.462494 neon-utils-1.5.1a7/neon_utils/res/snd/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   428660 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/snd/loaded.wav
--rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/snd/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.450493 neon-utils-1.5.1a7/neon_utils/res/text/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.462494 neon-utils-1.5.1a7/neon_utils/res/text/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/text/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/text/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/text/en-us/stop.voc
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/text/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.466493 neon-utils-1.5.1a7/neon_utils/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/res/ui/neon_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.466493 neon-utils-1.5.1a7/neon_utils/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/common_message_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/common_play_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/common_query_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/instructor_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/kiosk_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/mycroft_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/neon_fallback_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/neon_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/skills/skill_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/socket_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/validator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/neon_utils/web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.462494 neon-utils-1.5.1a7/neon_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-27 00:50:47.000000 neon-utils-1.5.1a7/neon_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-27 00:50:47.000000 neon-utils-1.5.1a7/neon_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:50:47.000000 neon-utils-1.5.1a7/neon_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 00:50:47.000000 neon-utils-1.5.1a7/neon_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-27 00:50:47.000000 neon-utils-1.5.1a7/neon_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 00:50:47.000000 neon-utils-1.5.1a7/neon_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/authentication_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/cache_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/configuration_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/file_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/language_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/location_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/log_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/message_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/messagebus_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/metric_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/mq_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    55268 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/neon_skill_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/net_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/packaging_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/parse_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/search_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/signal_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/tests/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/tests/skills/test_skill/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/skills/test_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/skills/test_skill/settingsmeta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/socket_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/user_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:50:47.474493 neon-utils-1.5.1a7/tests/valid_skill/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/valid_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/validator_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-27 00:50:43.000000 neon-utils-1.5.1a7/tests/web_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.266245 neon-utils-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 17:07:09.000000 neon-utils-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 17:07:13.262245 neon-utils-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 17:07:09.000000 neon-utils-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/authentication_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68558 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/default_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/default_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/default_configurations/default_user_conf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/location_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/messagebus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/mq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/process_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.254244 neon-utils-1.6.0/neon_utils/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   428660 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/snd/loaded.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/snd/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.254244 neon-utils-1.6.0/neon_utils/res/text/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/res/text/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/text/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/res/ui/neon_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/neon_utils/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/common_message_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/common_play_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/common_query_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/instructor_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/kiosk_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/mycroft_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/neon_fallback_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/neon_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/skills/skill_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/socket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/validator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-29 17:07:09.000000 neon-utils-1.6.0/neon_utils/web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.258245 neon-utils-1.6.0/neon_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 17:07:13.000000 neon-utils-1.6.0/neon_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:07:13.266245 neon-utils-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-29 17:07:09.000000 neon-utils-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/authentication_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/cache_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/configuration_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/file_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/language_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/location_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/log_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/message_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/messagebus_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/metric_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/mq_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55268 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/neon_skill_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/net_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/packaging_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/parse_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/search_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/signal_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/skills/test_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/skills/test_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/skills/test_skill/settingsmeta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/socket_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/user_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:07:13.262245 neon-utils-1.6.0/tests/valid_skill/
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/valid_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/validator_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-29 17:07:09.000000 neon-utils-1.6.0/tests/web_util_tests.py
```

### Comparing `neon-utils-1.5.1a7/LICENSE.md` & `neon-utils-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/PKG-INFO` & `neon-utils-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.5.1a7
+Version: 1.6.0
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.5.1a7/neon_utils/__init__.py` & `neon-utils-1.6.0/neon_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/authentication_utils.py` & `neon-utils-1.6.0/neon_utils/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/cache_utils.py` & `neon-utils-1.6.0/neon_utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/configuration_utils.py` & `neon-utils-1.6.0/neon_utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/decorators.py` & `neon-utils-1.6.0/neon_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/default_configurations/__init__.py` & `neon-utils-1.6.0/neon_utils/default_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/default_configurations/default_user_conf.yml` & `neon-utils-1.6.0/neon_utils/default_configurations/default_user_conf.yml`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/file_utils.py` & `neon-utils-1.6.0/neon_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/language_utils.py` & `neon-utils-1.6.0/neon_utils/language_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/location_utils.py` & `neon-utils-1.6.0/neon_utils/location_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/log_utils.py` & `neon-utils-1.6.0/neon_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/logger.py` & `neon-utils-1.6.0/neon_utils/logger.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/message_utils.py` & `neon-utils-1.6.0/neon_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/messagebus_utils.py` & `neon-utils-1.6.0/neon_utils/messagebus_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/metrics_utils.py` & `neon-utils-1.6.0/neon_utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/mq_utils.py` & `neon-utils-1.6.0/neon_utils/mq_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/net_utils.py` & `neon-utils-1.6.0/neon_utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/packaging_utils.py` & `neon-utils-1.6.0/neon_utils/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/parse_utils.py` & `neon-utils-1.6.0/neon_utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/process_utils.py` & `neon-utils-1.6.0/neon_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/res/snd/acknowledge.mp3` & `neon-utils-1.6.0/neon_utils/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/res/snd/loaded.wav` & `neon-utils-1.6.0/neon_utils/res/snd/loaded.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/res/snd/start_listening.wav` & `neon-utils-1.6.0/neon_utils/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/res/ui/neon_logo.png` & `neon-utils-1.6.0/neon_utils/res/ui/neon_logo.png`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/search_utils.py` & `neon-utils-1.6.0/neon_utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/signal_utils.py` & `neon-utils-1.6.0/neon_utils/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/__init__.py` & `neon-utils-1.6.0/neon_utils/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/common_message_skill.py` & `neon-utils-1.6.0/neon_utils/skills/common_message_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/common_play_skill.py` & `neon-utils-1.6.0/neon_utils/skills/common_play_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/common_query_skill.py` & `neon-utils-1.6.0/neon_utils/skills/common_query_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/instructor_skill.py` & `neon-utils-1.6.0/neon_utils/skills/instructor_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/kiosk_skill.py` & `neon-utils-1.6.0/neon_utils/skills/kiosk_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/mycroft_skill.py` & `neon-utils-1.6.0/neon_utils/skills/mycroft_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/neon_fallback_skill.py` & `neon-utils-1.6.0/neon_utils/skills/neon_fallback_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/neon_skill.py` & `neon-utils-1.6.0/neon_utils/skills/neon_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/skills/skill_gui.py` & `neon-utils-1.6.0/neon_utils/skills/skill_gui.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/socket_utils.py` & `neon-utils-1.6.0/neon_utils/socket_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/user_utils.py` & `neon-utils-1.6.0/neon_utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/validator_utils.py` & `neon-utils-1.6.0/neon_utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils/web_utils.py` & `neon-utils-1.6.0/neon_utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils.egg-info/PKG-INFO` & `neon-utils-1.6.0/neon_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.5.1a7
+Version: 1.6.0
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.5.1a7/neon_utils.egg-info/SOURCES.txt` & `neon-utils-1.6.0/neon_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/neon_utils.egg-info/requires.txt` & `neon-utils-1.6.0/neon_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/setup.py` & `neon-utils-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/__init__.py` & `neon-utils-1.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/authentication_util_tests.py` & `neon-utils-1.6.0/tests/authentication_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/cache_util_tests.py` & `neon-utils-1.6.0/tests/cache_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/configuration_util_tests.py` & `neon-utils-1.6.0/tests/configuration_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/file_util_tests.py` & `neon-utils-1.6.0/tests/file_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/language_util_tests.py` & `neon-utils-1.6.0/tests/language_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/location_util_tests.py` & `neon-utils-1.6.0/tests/location_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/log_util_tests.py` & `neon-utils-1.6.0/tests/log_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/message_util_tests.py` & `neon-utils-1.6.0/tests/message_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/messagebus_util_tests.py` & `neon-utils-1.6.0/tests/messagebus_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/metric_util_tests.py` & `neon-utils-1.6.0/tests/metric_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/mq_util_tests.py` & `neon-utils-1.6.0/tests/mq_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/neon_skill_tests.py` & `neon-utils-1.6.0/tests/neon_skill_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/net_util_tests.py` & `neon-utils-1.6.0/tests/net_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/packaging_util_tests.py` & `neon-utils-1.6.0/tests/packaging_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/parse_util_tests.py` & `neon-utils-1.6.0/tests/parse_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/search_util_tests.py` & `neon-utils-1.6.0/tests/search_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/signal_util_tests.py` & `neon-utils-1.6.0/tests/signal_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/skills/__init__.py` & `neon-utils-1.6.0/tests/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/skills/test_skill/__init__.py` & `neon-utils-1.6.0/tests/skills/test_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/socket_utils_tests.py` & `neon-utils-1.6.0/tests/socket_utils_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/user_util_tests.py` & `neon-utils-1.6.0/tests/user_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/valid_skill/__init__.py` & `neon-utils-1.6.0/tests/valid_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/validator_util_tests.py` & `neon-utils-1.6.0/tests/validator_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.5.1a7/tests/web_util_tests.py` & `neon-utils-1.6.0/tests/web_util_tests.py`

 * *Files identical despite different names*

