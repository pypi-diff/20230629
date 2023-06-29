# Comparing `tmp/AltTester-Driver-2.0.0.tar.gz` & `tmp/AltTester-Driver-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AltTester-Driver-2.0.0.tar", last modified: Wed May 24 14:53:54 2023, max compression
+gzip compressed data, was "AltTester-Driver-2.0.1.tar", last modified: Thu Jun 29 11:42:06 2023, max compression
```

## Comparing `AltTester-Driver-2.0.0.tar` & `AltTester-Driver-2.0.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.403305 AltTester-Driver-2.0.0/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.328344 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3406 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4513 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/SOURCES.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/dependency_links.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/not-zip-safe
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/requires.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/top_level.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.0/MANIFEST.in
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3406 2023-05-24 14:53:54.402649 AltTester-Driver-2.0.0/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1569 2023-05-24 13:53:56.000000 AltTester-Driver-2.0.0/README.md
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.337319 AltTester-Driver-2.0.0/alttester/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      340 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/alttester/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       18 2023-05-23 06:26:45.000000 AltTester-Driver-2.0.0/alttester/__version__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    10367 2023-05-23 11:50:16.000000 AltTester-Driver-2.0.0/alttester/_websocket.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    36372 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/altdriver.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    11419 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/altobject.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      277 2023-02-01 12:34:37.000000 AltTester-Driver-2.0.0/alttester/by.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.341904 AltTester-Driver-2.0.0/alttester/commands/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.345639 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      290 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1838 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/add_notification_listener.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1124 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/remove_notification_listener.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      292 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/reset_input.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1208 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/set_server_logging.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.354214 AltTester-Driver-2.0.0/alttester/commands/FindObjects/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      621 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1342 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      547 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object_at_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1363 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object_which_contains.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1343 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_objects.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1364 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_objects_which_contains.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1392 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1796 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1898 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1954 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object_which_contains.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.365358 AltTester-Driver-2.0.0/alttester/commands/InputActions/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      747 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      525 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/begin_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      914 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/click_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      519 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/end_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1251 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/keys_down.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1182 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/keys_up.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      834 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/move_mouse.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      647 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/move_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      815 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/multi_point_swipe.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1539 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/press_keys.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      923 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/scroll_mouse.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      874 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/swipe.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      910 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/tap_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      832 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/tilt.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.369977 AltTester-Driver-2.0.0/alttester/commands/Notifications/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      449 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      879 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/base_notification_callbacks.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      194 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/load_scene_mode.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      168 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/load_scene_notification_result.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      178 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/log_notification_result.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      138 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/notification_type.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.379863 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      748 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1887 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/call_method.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      799 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/click_element.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_all_components.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      905 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      475 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_text.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_down.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_enter.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      489 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_exit.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      489 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_up.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      910 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/set_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      621 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/set_text.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      795 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/tap_element.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.389230 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      878 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      240 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/delete_player_pref.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      479 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/delete_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      244 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_all_loaded_scenes.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      274 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_current_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      968 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      375 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_time_scale.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      709 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/load_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1337 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/set_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      710 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/set_time_scale.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      637 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/unload_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1010 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      556 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/alttester/commands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     7280 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/base_command.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      487 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/get_png_screenshot.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      240 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/get_server_version.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      874 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/get_static_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      854 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/alttester/commands/set_static_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3741 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/exceptions.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     7502 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/keycode.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      333 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/logging.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      260 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/playerpref.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      980 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/alttester/reverse_port_forwarding.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      112 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/requirements-dev.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       50 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/requirements.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2023-05-24 14:53:54.403512 AltTester-Driver-2.0.0/setup.cfg
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2560 2023-05-12 12:36:10.000000 AltTester-Driver-2.0.0/setup.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.321061 AltTester-Driver-2.0.0/tests/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.399345 AltTester-Driver-2.0.0/tests/integration/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        0 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.0/tests/integration/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      622 2023-05-12 12:36:10.000000 AltTester-Driver-2.0.0/tests/integration/conftest.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4408 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_driver.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3625 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_notifications.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      812 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/tests/integration/test_reverse_port_forwarding.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    34917 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_scene01.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4542 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene02.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5694 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene03.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4537 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene05.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3824 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_scene07.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1652 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene09.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3605 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene10.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      414 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/tests/integration/utils.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.401815 AltTester-Driver-2.0.0/tests/unit/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        0 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.0/tests/unit/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1668 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/tests/unit/test_altobject.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1529 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/tests/unit/test_commands.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5403 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/unit/test_websocket.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.345464 AltTester-Driver-2.0.1/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.251680 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3422 2023-06-29 11:42:06.000000 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4513 2023-06-29 11:42:06.000000 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-06-29 11:42:06.000000 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-06-29 11:42:06.000000 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/not-zip-safe
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2023-06-29 11:42:06.000000 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/requires.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2023-06-29 11:42:06.000000 AltTester-Driver-2.0.1/AltTester_Driver.egg-info/top_level.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.1/MANIFEST.in
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3422 2023-06-29 11:42:06.344829 AltTester-Driver-2.0.1/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1578 2023-06-28 13:24:09.000000 AltTester-Driver-2.0.1/README.md
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.263398 AltTester-Driver-2.0.1/alttester/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1045 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       18 2023-06-27 06:25:18.000000 AltTester-Driver-2.0.1/alttester/__version__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    11072 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/_websocket.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    37077 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/altdriver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    12124 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      982 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/by.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.269574 AltTester-Driver-2.0.1/alttester/commands/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.274377 AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      995 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2543 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/add_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1829 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/remove_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      997 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/reset_input.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1913 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/set_server_logging.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.285468 AltTester-Driver-2.0.1/alttester/commands/FindObjects/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1326 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2047 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/find_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1252 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/find_object_at_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2068 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/find_object_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2048 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/find_objects.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2069 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/find_objects_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2097 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/wait_for_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2501 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/wait_for_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2603 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2659 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/FindObjects/wait_for_object_which_contains.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.298961 AltTester-Driver-2.0.1/alttester/commands/InputActions/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1452 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1230 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/begin_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1619 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/click_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1224 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/end_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1956 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/keys_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1887 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/keys_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1539 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/move_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1352 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/move_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1520 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/multi_point_swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2244 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/press_keys.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1628 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/scroll_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1579 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1615 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/tap_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1537 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/InputActions/tilt.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.304822 AltTester-Driver-2.0.1/alttester/commands/Notifications/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1154 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/Notifications/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1584 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/Notifications/base_notification_callbacks.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      899 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/Notifications/load_scene_mode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      875 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/Notifications/load_scene_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      884 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/Notifications/log_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      843 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/Notifications/notification_type.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.316855 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1453 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2592 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/call_method.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1504 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/click_element.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1214 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/get_all_components.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/get_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1180 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/get_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1214 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/pointer_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1214 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/pointer_enter.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1194 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/pointer_exit.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1194 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/pointer_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1615 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/set_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1326 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/set_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1500 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/tap_element.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.326701 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1583 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      945 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/delete_player_pref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1184 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/delete_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      949 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/get_all_loaded_scenes.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      979 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/get_current_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1673 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/get_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1080 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/get_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1414 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/load_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2042 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/set_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1415 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/set_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1342 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/unload_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1715 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1261 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7985 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/base_command.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1192 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/get_png_screenshot.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      945 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/get_server_version.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1579 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/get_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1559 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/commands/set_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4446 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/exceptions.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     8207 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/keycode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1038 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/logging.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      965 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/playerpref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1685 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/alttester/reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      166 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/requirements-dev.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       50 2023-06-09 22:59:25.000000 AltTester-Driver-2.0.1/requirements.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2023-06-29 11:42:06.345634 AltTester-Driver-2.0.1/setup.cfg
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3272 2023-06-28 13:24:09.000000 AltTester-Driver-2.0.1/setup.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.244001 AltTester-Driver-2.0.1/tests/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.339776 AltTester-Driver-2.0.1/tests/integration/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      705 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4036 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/conftest.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5113 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_driver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4330 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_notifications.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1517 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    35622 2023-06-26 14:20:05.000000 AltTester-Driver-2.0.1/tests/integration/test_scene01.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5247 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_scene02.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     6578 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_scene03.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5242 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_scene05.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4529 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_scene07.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2357 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_scene09.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4310 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/test_scene10.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1119 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/integration/utils.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-06-29 11:42:06.343782 AltTester-Driver-2.0.1/tests/unit/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      705 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/unit/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2373 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/unit/test_altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2234 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/unit/test_commands.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     6108 2023-06-23 08:19:20.000000 AltTester-Driver-2.0.1/tests/unit/test_websocket.py
```

### Comparing `AltTester-Driver-2.0.0/AltTester_Driver.egg-info/PKG-INFO` & `AltTester-Driver-2.0.1/AltTester_Driver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: AltTester-Driver
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python bindings for the AltTester framework. AltTester is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
-Home-page: https://alttester.com/docs/pro/sdk
+Home-page: https://alttester.com/docs/sdk/latest/
 Author: Altom Consulting
 Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
-Project-URL: Documentation, https://alttester.com/docs/pro/sdk
+Project-URL: Documentation, https://alttester.com/docs/sdk/latest
 Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
 Keywords: unity testing tests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: C#
@@ -39,19 +39,19 @@
 
 This package contains an library for adding Python language binding to the AltTester framework.
 
 AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
 
 You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
 
-Read the documentation on https://alttester.com/docs/pro/sdk/
+Read the documentation on https://alttester.com/docs/sdk/latest/
 
 ## Get Started
 
-Check out the [Get Started](https://alttester.com/docs/pro/sdk/pages/get-started.html) guide from the documentation.
+Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
 
 ## Development
 
 -   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
 -   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 
 ### Running Tests
@@ -72,15 +72,15 @@
 
 ```
 $ pytest tests/integration/
 ```
 
 ## Contributing
 
-Check out the full contributing guide [contributing](https://alttester.com/docs/pro/sdk/pages/contributing.html).
+Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
 
 ## Support
 
 Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
 
 Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
```

### Comparing `AltTester-Driver-2.0.0/AltTester_Driver.egg-info/SOURCES.txt` & `AltTester-Driver-2.0.1/AltTester_Driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-2.0.0/PKG-INFO` & `AltTester-Driver-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: AltTester-Driver
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python bindings for the AltTester framework. AltTester is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
-Home-page: https://alttester.com/docs/pro/sdk
+Home-page: https://alttester.com/docs/sdk/latest/
 Author: Altom Consulting
 Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
-Project-URL: Documentation, https://alttester.com/docs/pro/sdk
+Project-URL: Documentation, https://alttester.com/docs/sdk/latest
 Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
 Keywords: unity testing tests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: C#
@@ -39,19 +39,19 @@
 
 This package contains an library for adding Python language binding to the AltTester framework.
 
 AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
 
 You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
 
-Read the documentation on https://alttester.com/docs/pro/sdk/
+Read the documentation on https://alttester.com/docs/sdk/latest/
 
 ## Get Started
 
-Check out the [Get Started](https://alttester.com/docs/pro/sdk/pages/get-started.html) guide from the documentation.
+Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
 
 ## Development
 
 -   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
 -   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 
 ### Running Tests
@@ -72,15 +72,15 @@
 
 ```
 $ pytest tests/integration/
 ```
 
 ## Contributing
 
-Check out the full contributing guide [contributing](https://alttester.com/docs/pro/sdk/pages/contributing.html).
+Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
 
 ## Support
 
 Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
 
 Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
```

### Comparing `AltTester-Driver-2.0.0/README.md` & `AltTester-Driver-2.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 This package contains an library for adding Python language binding to the AltTester framework.
 
 AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
 
 You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
 
-Read the documentation on https://alttester.com/docs/pro/sdk/
+Read the documentation on https://alttester.com/docs/sdk/latest/
 
 ## Get Started
 
-Check out the [Get Started](https://alttester.com/docs/pro/sdk/pages/get-started.html) guide from the documentation.
+Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
 
 ## Development
 
 -   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
 -   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 
 ### Running Tests
@@ -35,15 +35,15 @@
 
 ```
 $ pytest tests/integration/
 ```
 
 ## Contributing
 
-Check out the full contributing guide [contributing](https://alttester.com/docs/pro/sdk/pages/contributing.html).
+Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
 
 ## Support
 
 Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
 
 Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
```

### Comparing `AltTester-Driver-2.0.0/alttester/_websocket.py` & `AltTester-Driver-2.0.1/alttester/_websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import time
 import json
 from collections import defaultdict, deque
 from urllib.parse import urlencode, urlunparse
 from threading import Thread
 
 from loguru import logger
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/altdriver.py` & `AltTester-Driver-2.0.1/alttester/altdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import warnings
 import sys
 
 from loguru import logger
 
 import alttester.commands as commands
 from alttester.commands.base_command import Command
```

### Comparing `AltTester-Driver-2.0.0/alttester/altobject.py` & `AltTester-Driver-2.0.1/alttester/altobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import json
 
 import alttester.commands as commands
 from alttester.by import By
 
 
 class AltObject:
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/add_notification_listener.py` & `AltTester-Driver-2.0.1/alttester/commands/AltTesterCommands/add_notification_listener.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from alttester.commands.Notifications.notification_type import NotificationType
 from alttester.commands.base_command import BaseCommand
 from alttester.exceptions import InvalidParameterTypeException
 
 
 class AddNotificationListener(BaseCommand):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object.py` & `AltTester-Driver-2.0.1/alttester/commands/FindObjects/wait_for_object_which_contains.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,37 @@
-from alttester.commands.base_command import BaseCommand
-from alttester.exceptions import InvalidParameterTypeException
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+import time
+
+from loguru import logger
+
 from alttester.by import By
+from alttester.commands.base_command import Command
+from alttester.commands.FindObjects.find_object_which_contains import FindObjectWhichContains
+from alttester.exceptions import NotFoundException, WaitTimeOutException, InvalidParameterTypeException
 
 
-class FindObject(BaseCommand):
+class WaitForObjectWhichContains(Command):
 
-    def __init__(self, connection, by, value, camera_by, camera_value, enabled):
-        super().__init__(connection, "findObject")
+    def __init__(self, connection, by, value, camera_by, camera_value, timeout, interval, enabled):
+        self.connection = connection
 
         if by not in By:
             raise InvalidParameterTypeException(
                 parameter_name="by",
                 expected_types=[By],
                 received_type=type(by)
             )
@@ -22,24 +43,35 @@
                 received_type=type(camera_by)
             )
 
         self.by = by
         self.value = value
         self.camera_by = camera_by
         self.camera_value = camera_value
+        self.timeout = timeout
+        self.interval = interval
         self.enabled = enabled
 
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "by": str(self.by),
-            "path": self.get_path(self.by, self.value),
-            "cameraBy": str(self.camera_by),
-            "cameraPath": self.get_path(self.camera_by, self.camera_value),
-            "enabled": self.enabled,
-        })
+    def execute(self):
+        t = 0
+        alt_unity_object = None
 
-        return parameters
+        while (t <= self.timeout):
+            try:
+                alt_unity_object = FindObjectWhichContains(
+                    self.connection,
+                    self.by, self.value, self.camera_by, self.camera_value, self.enabled
+                ).execute()
+
+                break
+            except NotFoundException:
+                logger.debug("Waiting for element where name contains {}...", self.value)
+                time.sleep(self.interval)
+                t += self.interval
+
+        if t >= self.timeout:
+            raise WaitTimeOutException("Element where name contains {} not found after {} seconds".format(
+                self.value,
+                self.timeout
+            ))
 
-    def execute(self):
-        return self.send()
+        return alt_unity_object
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/InputActions/click_coordinates.py` & `AltTester-Driver-2.0.1/alttester/commands/InputActions/click_coordinates.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from alttester.commands.base_command import validate_coordinates, BaseCommand
 
 
 class ClickCoordinates(BaseCommand):
 
     def __init__(self, connection, coordinates, count, interval, wait):
         super().__init__(connection, "clickCoordinates")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/InputActions/move_mouse.py` & `AltTester-Driver-2.0.1/alttester/commands/InputActions/move_mouse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from alttester.commands.base_command import validate_coordinates, BaseCommand
 
 
 class MoveMouse(BaseCommand):
 
     def __init__(self, connection, coordinates, duration, wait):
         super().__init__(connection, "moveMouse")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/InputActions/tap_coordinates.py` & `AltTester-Driver-2.0.1/alttester/commands/InputActions/move_touch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from alttester.commands.base_command import validate_coordinates, BaseCommand
 
 
-class TapCoordinates(BaseCommand):
+class MoveTouch(BaseCommand):
 
-    def __init__(self, connection, coordinates, count, interval, wait):
-        super().__init__(connection, "tapCoordinates")
+    def __init__(self, connection, finger_id, coordinates):
+        super().__init__(connection, "moveTouch")
 
         self.coordinates = validate_coordinates(coordinates)
-        self.count = count
-        self.interval = interval
-        self.wait = wait
+        self.finger_id = finger_id
 
     @property
     def _parameters(self):
         parameters = super()._parameters
         parameters.update(**{
-            "coordinates": self.coordinates,
-            "count": self.count,
-            "interval": self.interval,
-            "wait": self.wait
+            "fingerId": self.finger_id,
+            "coordinates": self.coordinates
         })
 
         return parameters
 
     def execute(self):
         data = self.send()
         self.validate_response("Ok", data)
-
-        if self.wait:
-            data = self.recv()
-            self.validate_response("Finished", data)
-
-        return data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_component_property.py` & `AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/get_all_components.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from alttester.commands.base_command import BaseCommand
 
 
-class GetComponentProperty(BaseCommand):
+class GetAllComponents(BaseCommand):
 
-    def __init__(self, connection, component_name, property_name, assembly_name, max_depth, alt_object):
-        super().__init__(connection, "getObjectComponentProperty")
+    def __init__(self, connection, alt_object):
+        super(GetAllComponents, self).__init__(connection, "getAllComponents")
 
         self.alt_object = alt_object
 
-        self.component_name = component_name
-        self.property_name = property_name
-        self.assembly_name = assembly_name
-        self.max_depth = max_depth
-
     @property
     def _parameters(self):
         parameters = super()._parameters
         parameters.update(**{
-            "altObject": self.alt_object.to_json(),
-            "component": self.component_name,
-            "property": self.property_name,
-            "assembly": self.assembly_name,
-            "maxDepth": self.max_depth,
+            "altObjectId": self.alt_object.id
         })
 
         return parameters
 
     def execute(self):
         return self.send()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/base_command.py` & `AltTester-Driver-2.0.1/alttester/commands/base_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import abc
 import json
 import time
 from datetime import datetime
 
 from loguru import logger
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/commands/set_static_property.py` & `AltTester-Driver-2.0.1/alttester/commands/ObjectCommands/set_component_property.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,47 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+import json
 from alttester.commands.base_command import BaseCommand
 
 
-class SetStaticProperty(BaseCommand):
+class SetComponentProperty(BaseCommand):
 
-    def __init__(self, connection, component_name, property_name, assembly_name, value):
+    def __init__(self, connection, component_name, property_name, value, assembly_name, alt_object):
         super().__init__(connection, "setObjectComponentProperty")
 
-        self.alt_object = None
+        self.alt_object = alt_object
 
         self.component_name = component_name
         self.property_name = property_name
+        self.value = json.dumps(value)
         self.assembly_name = assembly_name
-        self.value = value
 
     @property
     def _parameters(self):
         parameters = super()._parameters
         parameters.update(**{
-            "altObject": self.alt_object,
+            "altObject": self.alt_object.to_json(),
             "component": self.component_name,
             "property": self.property_name,
             "assembly": self.assembly_name,
-            "value": self.value
+            "value": self.value,
         })
 
         return parameters
 
     def execute(self):
         return self.send()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/alttester/keycode.py` & `AltTester-Driver-2.0.1/alttester/keycode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from enum import Enum
 
 
 class AltKeyCode(Enum):
     NoKey = 0
     Backspace = 8
     Tab = 9
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/setup.py` & `AltTester-Driver-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,30 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 from setuptools import setup, find_packages
 
 
 NAME = 'AltTester-Driver'
 DESCRIPTION = "Python bindings for the AltTester framework. AltTester is an open-source UI driven test " \
     "automation tool that helps you find objects in your game and interacts with them."
-URL = 'https://alttester.com/docs/pro/sdk'
+URL = 'https://alttester.com/docs/sdk/latest/'
 EMAIL = 'contact@alttester.com'
 AUTHOR = 'Altom Consulting'
 REQUIRES_PYTHON = '>=3.4.0'
 LICENSE = 'GNU GPLv3'
 
 
 with open("alttester/__version__.py") as f:
@@ -29,15 +45,15 @@
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type='text/markdown',
     license=LICENSE,
     url=URL,
     project_urls={
         "Bug Tracker": "https://github.com/alttester/AltTester-Unity-SDK/issues",
-        "Documentation": "https://alttester.com/docs/pro/sdk",
+        "Documentation": "https://alttester.com/docs/sdk/latest",
         "Source": "https://github.com/alttester/AltTester-Unity-SDK",
     },
 
     author=AUTHOR,
     author_email=EMAIL,
 
     zip_safe=False,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/tests/integration/test_notifications.py` & `AltTester-Driver-2.0.1/tests/integration/test_notifications.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import pytest
 
 from .utils import Scenes
 from alttester import By
 from alttester.commands.Notifications.notification_type import NotificationType
 from alttester.commands.Notifications.base_notification_callbacks import BaseNotificationCallbacks
 from alttester.logging import AltLogLevel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/tests/integration/test_scene01.py` & `AltTester-Driver-2.0.1/tests/integration/test_scene01.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import time
 
 import pytest
 
 from .utils import Scenes
 from alttester import By, PlayerPrefKeyType, AltKeyCode
 import alttester.exceptions as exceptions
```

### Comparing `AltTester-Driver-2.0.0/tests/integration/test_scene03.py` & `AltTester-Driver-2.0.1/tests/integration/test_scene03.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
 import pytest
 
 from .utils import Scenes
 from alttester import By
 
 
 class TestScene03:
@@ -32,15 +49,16 @@
 
         self.altdriver.multipoint_swipe(positions, duration, wait)
 
     def drop_image(self, drag_location_name, drop_location_name, duration, wait):
         drag_location = self.altdriver.find_object(By.NAME, drag_location_name)
         drop_location = self.altdriver.find_object(By.NAME, drop_location_name)
 
-        self.altdriver.swipe(drag_location.get_screen_position(), drop_location.get_screen_position(), duration, wait)
+        self.altdriver.swipe(drag_location.get_screen_position(
+        ), drop_location.get_screen_position(), duration, wait)
 
     def test_pointer_enter_and_exit(self):
         alt_object = self.altdriver.find_object(By.NAME, "Drop Image")
         color1 = alt_object.get_component_property(
             "AltExampleScriptDropMe",
             "highlightColor",
             "Assembly-CSharp"
@@ -75,58 +93,71 @@
             color3["a"] == color1["a"]
 
     def test_multiple_swipes(self):
         self.drop_image("Drag Image2", "Drop Box2", 1, False)
         self.drop_image("Drag Image2", "Drop Box1", 1, False)
         self.drop_image("Drag Image1", "Drop Box1", 2, False)
         self.wait_for_swipe_to_finish()
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image1", "Drop Image")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
         assert image_source == image_source_drop_zone
 
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image2", "Drop")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
         assert image_source == image_source_drop_zone
 
     def test_multiple_swipe_and_waits(self):
         self.drop_image("Drag Image2", "Drop Box2", 1, True)
         self.drop_image("Drag Image2", "Drop Box1", 1, True)
         self.drop_image("Drag Image1", "Drop Box1", 1, True)
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image1", "Drop Image")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
         assert image_source == image_source_drop_zone
 
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image2", "Drop")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
         assert image_source == image_source_drop_zone
 
     def test_multiple_swipe_with_multipoint_swipe(self):
 
-        self.drop_image_with_multipoint_swipe(["Drag Image1", "Drop Box1"],  1, False)
-        self.drop_image_with_multipoint_swipe(["Drag Image2", "Drop Box1", "Drop Box2"],  1, False)
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image1", "Drop Box1"],  1, False)
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image2", "Drop Box1", "Drop Box2"],  1, False)
 
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image1", "Drop Image")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
         assert image_source == image_source_drop_zone
 
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image2", "Drop")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
         assert image_source == image_source_drop_zone
 
     def test_multiple_swipe_and_waits_with_multipoint_swipe(self):
 
-        self.drop_image_with_multipoint_swipe(["Drag Image1", "Drop Box1"],  1, True)
-        self.drop_image_with_multipoint_swipe(["Drag Image2", "Drop Box1", "Drop Box2"],  1, True)
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image1", "Drop Box1"],  1, True)
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image2", "Drop Box1", "Drop Box2"],  1, True)
 
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image1", "Drop Image")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
         assert image_source == image_source_drop_zone
 
-        image_source, image_source_drop_zone = self.get_sprite_name("Drag Image2", "Drop")
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
         assert image_source == image_source_drop_zone
 
     def test_begin_move_end_touch(self):
         alt_object1 = self.altdriver.find_object(By.NAME, "Drag Image1")
         alt_object2 = self.altdriver.find_object(By.NAME, "Drop Box1")
 
         id = self.altdriver.begin_touch(alt_object1.get_screen_position())
         self.altdriver.move_touch(id, alt_object2.get_screen_position())
         self.altdriver.end_touch(id)
 
-        imageSource = alt_object1.get_component_property("UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
+        imageSource = alt_object1.get_component_property(
+            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
         imageSourceDropZone = self.altdriver.find_object(By.NAME, "Drop Image").get_component_property(
             "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
 
         assert imageSource == imageSourceDropZone
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/tests/integration/test_scene07.py` & `AltTester-Driver-2.0.1/tests/integration/test_scene07.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import pytest
 from alttester import By
 
 from .utils import Scenes
 
 
 class TestScene07A:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.0/tests/integration/test_scene10.py` & `AltTester-Driver-2.0.1/tests/integration/test_scene10.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+﻿"""
+    Copyright(C) 2023  Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
 import pytest
 
 from .utils import Scenes
 from alttester import By, AltKeyCode
 
 
 class TestScene10:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

