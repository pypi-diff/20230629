# Comparing `tmp/badger-opt-0.9.1.tar.gz` & `tmp/badger-opt-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zhezhang/Projects/Badger/dist/tmp6z2upcw8/badger-opt-0.9.1.tar", last modified: Tue Aug 30 16:50:31 2022, max compression
+gzip compressed data, was "/Users/zhezhang/Projects/Badger/dist/.tmp-lh8z9vju/badger-opt-0.9.2.tar", last modified: Thu Feb  2 09:05:07 2023, max compression
```

## Comparing `badger-opt-0.9.1.tar` & `badger-opt-0.9.2.tar`

### file list

```diff
@@ -1,144 +1,118 @@
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/
--rw-r--r--   0 zhezhang (1762935258) 1704612529    35149 2021-11-13 19:54:28.000000 badger-opt-0.9.1/LICENSE
--rw-r--r--   0 zhezhang (1762935258) 1704612529      238 2022-08-18 17:52:13.000000 badger-opt-0.9.1/MANIFEST.in
--rw-r--r--   0 zhezhang (1762935258) 1704612529      274 2022-08-30 16:50:31.000000 badger-opt-0.9.1/PKG-INFO
--rw-r--r--   0 zhezhang (1762935258) 1704612529    12158 2021-11-18 00:49:41.000000 badger-opt-0.9.1/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      174 2022-08-30 16:50:31.000000 badger-opt-0.9.1/setup.cfg
--rw-r--r--   0 zhezhang (1762935258) 1704612529      895 2022-08-26 22:04:03.000000 badger-opt-0.9.1/setup.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       72 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5168 2022-08-25 19:31:51.000000 badger-opt-0.9.1/src/badger/__main__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      497 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/_version.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/actions/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1770 2022-08-30 16:47:45.000000 badger-opt-0.9.1/src/badger/actions/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      603 2022-05-27 18:36:03.000000 badger-opt-0.9.1/src/badger/actions/algo.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3559 2022-07-21 18:16:19.000000 badger-opt-0.9.1/src/badger/actions/config.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      596 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/actions/doctor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      685 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/actions/env.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4749 2022-08-27 04:55:04.000000 badger-opt-0.9.1/src/badger/actions/install.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      603 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/actions/intf.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      966 2022-05-27 19:32:46.000000 badger-opt-0.9.1/src/badger/actions/routine.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4953 2022-07-29 04:58:39.000000 badger-opt-0.9.1/src/badger/actions/run.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1096 2022-08-26 22:01:06.000000 badger-opt-0.9.1/src/badger/actions/uninstall.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3290 2022-07-29 04:11:42.000000 badger-opt-0.9.1/src/badger/archive.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    13695 2022-07-29 04:06:51.000000 badger-opt-0.9.1/src/badger/core.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5961 2022-08-25 19:14:13.000000 badger-opt-0.9.1/src/badger/db.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     6199 2022-06-15 18:45:28.000000 badger-opt-0.9.1/src/badger/environment.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      606 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/extension.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5918 2022-07-05 17:45:00.000000 badger-opt-0.9.1/src/badger/factory.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2429 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/__init__.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui/components/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/components/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1762 2021-12-14 08:08:46.000000 badger-opt-0.9.1/src/badger/gui/components/constraint_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      589 2021-12-15 07:56:40.000000 badger-opt-0.9.1/src/badger/gui/components/labeled_lineedit.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      678 2021-11-17 20:51:04.000000 badger-opt-0.9.1/src/badger/gui/components/labeled_spinbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1033 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/components/objective_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3172 2022-05-27 19:36:45.000000 badger-opt-0.9.1/src/badger/gui/components/routine_runner.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      249 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/components/search_bar.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     7164 2022-02-10 06:24:38.000000 badger-opt-0.9.1/src/badger/gui/components/syntax.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      980 2021-11-17 17:35:24.000000 badger-opt-0.9.1/src/badger/gui/components/variable_item.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui/images/
--rw-r--r--   0 zhezhang (1762935258) 1704612529    46055 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/images/icon.png
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui/pages/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/pages/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     7290 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/pages/home_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    27601 2022-05-27 19:38:52.000000 badger-opt-0.9.1/src/badger/gui/pages/routine_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    10257 2021-12-09 09:08:16.000000 badger-opt-0.9.1/src/badger/gui/pages/run_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      284 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/utils.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui/windows/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/windows/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1941 2022-02-10 06:16:38.000000 badger-opt-0.9.1/src/badger/gui/windows/edit_script_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2230 2021-12-15 19:17:21.000000 badger-opt-0.9.1/src/badger/gui/windows/main_window.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    19414 2022-03-29 22:39:08.000000 badger-opt-0.9.1/src/badger/gui/windows/opt_monitor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      777 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/windows/review_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2853 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/gui/windows/settings_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3470 2022-05-27 19:41:39.000000 badger-opt-0.9.1/src/badger/gui/windows/var_dialog.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui_acr/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2442 2022-08-18 19:46:59.000000 badger-opt-0.9.1/src/badger/gui_acr/__init__.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui_acr/components/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2022-03-11 21:02:36.000000 badger-opt-0.9.1/src/badger/gui_acr/components/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3533 2022-07-03 21:09:50.000000 badger-opt-0.9.1/src/badger/gui_acr/components/algo_cbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3640 2022-07-03 20:54:23.000000 badger-opt-0.9.1/src/badger/gui_acr/components/collapsible_box.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1917 2022-07-03 21:29:59.000000 badger-opt-0.9.1/src/badger/gui_acr/components/constraint_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2768 2022-07-12 23:15:31.000000 badger-opt-0.9.1/src/badger/gui_acr/components/data_table.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     9113 2022-07-04 00:12:31.000000 badger-opt-0.9.1/src/badger/gui_acr/components/env_cbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2180 2022-08-25 17:29:43.000000 badger-opt-0.9.1/src/badger/gui_acr/components/filter_cbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5249 2022-04-12 06:51:58.000000 badger-opt-0.9.1/src/badger/gui_acr/components/history_navigator.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      589 2022-04-13 21:05:00.000000 badger-opt-0.9.1/src/badger/gui_acr/components/labeled_lineedit.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      859 2022-07-03 21:29:25.000000 badger-opt-0.9.1/src/badger/gui_acr/components/labeled_spinbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1091 2022-07-28 22:02:15.000000 badger-opt-0.9.1/src/badger/gui_acr/components/objective_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3059 2022-07-03 06:51:34.000000 badger-opt-0.9.1/src/badger/gui_acr/components/routine_editor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3249 2022-04-15 08:02:59.000000 badger-opt-0.9.1/src/badger/gui_acr/components/routine_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    29452 2022-08-25 18:43:10.000000 badger-opt-0.9.1/src/badger/gui_acr/components/routine_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3823 2022-07-04 01:01:06.000000 badger-opt-0.9.1/src/badger/gui_acr/components/routine_runner.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    31501 2022-07-29 04:07:04.000000 badger-opt-0.9.1/src/badger/gui_acr/components/run_monitor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      232 2022-03-11 21:08:44.000000 badger-opt-0.9.1/src/badger/gui_acr/components/search_bar.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      949 2022-06-30 18:26:08.000000 badger-opt-0.9.1/src/badger/gui_acr/components/state_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1291 2022-08-18 18:04:17.000000 badger-opt-0.9.1/src/badger/gui_acr/components/status_bar.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     7164 2022-04-13 21:04:43.000000 badger-opt-0.9.1/src/badger/gui_acr/components/syntax.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1043 2022-07-03 21:32:22.000000 badger-opt-0.9.1/src/badger/gui_acr/components/variable_item.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui_acr/images/
--rw-r--r--   0 zhezhang (1762935258) 1704612529    17885 2022-08-18 17:54:53.000000 badger-opt-0.9.1/src/badger/gui_acr/images/gear.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    46055 2022-08-18 17:51:33.000000 badger-opt-0.9.1/src/badger/gui_acr/images/icon.png
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui_acr/pages/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2022-03-11 21:02:36.000000 badger-opt-0.9.1/src/badger/gui_acr/pages/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    15179 2022-08-25 20:27:22.000000 badger-opt-0.9.1/src/badger/gui_acr/pages/home_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      668 2022-07-03 21:28:31.000000 badger-opt-0.9.1/src/badger/gui_acr/utils.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2022-03-11 21:02:36.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1941 2022-04-13 21:04:01.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/edit_script_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1124 2022-05-08 01:28:03.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/main_window.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      777 2022-04-13 21:04:07.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/review_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5365 2022-08-25 19:58:26.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/settings_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3470 2022-05-27 19:41:47.000000 badger-opt-0.9.1/src/badger/gui_acr/windows/var_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2628 2022-07-29 04:28:24.000000 badger-opt-0.9.1/src/badger/interface.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      955 2022-06-30 03:45:47.000000 badger-opt-0.9.1/src/badger/log.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4236 2022-07-13 07:26:27.000000 badger-opt-0.9.1/src/badger/logbook.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/logger/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4437 2022-06-21 17:28:06.000000 badger-opt-0.9.1/src/badger/logger/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      259 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/logger/event.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      937 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/logger/observer.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1616 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/logger/util.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3101 2022-08-25 19:31:51.000000 badger-opt-0.9.1/src/badger/settings.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      606 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/stats.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2094 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/conftest.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/configs/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       44 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/configs/test.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/__init__.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/silly/
--rw-r--r--   0 zhezhang (1762935258) 1704612529      204 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/silly/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      488 2022-01-20 09:08:38.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/silly/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      108 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/silly/configs.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/simplex/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/simplex/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1036 2022-01-20 09:17:08.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/simplex/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      140 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/simplex/configs.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/environments/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/environments/silly/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/environments/silly/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1051 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/environments/silly/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529       91 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/environments/silly/configs.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/interfaces/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/interfaces/silly/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       57 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/interfaces/silly/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1452 2022-01-20 09:17:08.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/interfaces/silly/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529       70 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/mock/plugins/interfaces/silly/configs.yaml
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1209 2022-08-26 19:18:20.000000 badger-opt-0.9.1/src/badger/tests/test_cli_basic.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      350 2021-11-13 19:54:28.000000 badger-opt-0.9.1/src/badger/tests/test_gui_basic.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2322 2022-05-27 19:37:37.000000 badger-opt-0.9.1/src/badger/tests/test_lib_basic.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     6466 2022-07-21 21:08:59.000000 badger-opt-0.9.1/src/badger/utils.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/
--rw-r--r--   0 zhezhang (1762935258) 1704612529      274 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/PKG-INFO
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4283 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/SOURCES.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529        1 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/dependency_links.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529       48 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/entry_points.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529       95 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/requires.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529        7 2022-08-30 16:50:31.000000 badger-opt-0.9.1/src/badger_opt.egg-info/top_level.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529    80044 2021-11-13 19:54:28.000000 badger-opt-0.9.1/versioneer.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    35149 2021-11-13 19:54:28.000000 badger-opt-0.9.2/LICENSE
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      206 2023-02-01 23:30:17.000000 badger-opt-0.9.2/MANIFEST.in
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      274 2023-02-02 09:05:07.000000 badger-opt-0.9.2/PKG-INFO
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    12158 2021-11-18 00:49:41.000000 badger-opt-0.9.2/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      174 2023-02-02 09:05:07.000000 badger-opt-0.9.2/setup.cfg
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      895 2022-08-26 22:04:03.000000 badger-opt-0.9.2/setup.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       72 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5168 2022-08-25 19:31:51.000000 badger-opt-0.9.2/src/badger/__main__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      497 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/_version.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/actions/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1782 2023-02-01 23:29:35.000000 badger-opt-0.9.2/src/badger/actions/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      603 2022-05-27 18:36:03.000000 badger-opt-0.9.2/src/badger/actions/algo.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3559 2022-07-21 18:16:19.000000 badger-opt-0.9.2/src/badger/actions/config.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      596 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/actions/doctor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      685 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/actions/env.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4749 2022-08-27 04:55:04.000000 badger-opt-0.9.2/src/badger/actions/install.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      603 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/actions/intf.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      966 2022-05-27 19:32:46.000000 badger-opt-0.9.2/src/badger/actions/routine.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4953 2022-07-29 04:58:39.000000 badger-opt-0.9.2/src/badger/actions/run.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1096 2022-08-26 22:01:06.000000 badger-opt-0.9.2/src/badger/actions/uninstall.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3290 2022-07-29 04:11:42.000000 badger-opt-0.9.2/src/badger/archive.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    13695 2022-07-29 04:06:51.000000 badger-opt-0.9.2/src/badger/core.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5961 2022-08-25 19:14:13.000000 badger-opt-0.9.2/src/badger/db.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     7623 2022-09-23 18:20:42.000000 badger-opt-0.9.2/src/badger/environment.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      606 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/extension.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5918 2022-07-05 17:45:00.000000 badger-opt-0.9.2/src/badger/factory.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/gui/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-02-01 23:28:11.000000 badger-opt-0.9.2/src/badger/gui/__init__.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/gui/default/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2443 2023-02-01 23:29:23.000000 badger-opt-0.9.2/src/badger/gui/default/__init__.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/gui/default/components/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2022-03-11 21:02:36.000000 badger-opt-0.9.2/src/badger/gui/default/components/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3533 2022-07-03 21:09:50.000000 badger-opt-0.9.2/src/badger/gui/default/components/algo_cbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3640 2022-07-03 20:54:23.000000 badger-opt-0.9.2/src/badger/gui/default/components/collapsible_box.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1917 2022-07-03 21:29:59.000000 badger-opt-0.9.2/src/badger/gui/default/components/constraint_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2775 2023-02-01 23:13:45.000000 badger-opt-0.9.2/src/badger/gui/default/components/data_table.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     9113 2022-07-04 00:12:31.000000 badger-opt-0.9.2/src/badger/gui/default/components/env_cbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2180 2022-08-25 17:29:43.000000 badger-opt-0.9.2/src/badger/gui/default/components/filter_cbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5250 2023-02-01 23:34:22.000000 badger-opt-0.9.2/src/badger/gui/default/components/history_navigator.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      589 2022-04-13 21:05:00.000000 badger-opt-0.9.2/src/badger/gui/default/components/labeled_lineedit.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      859 2022-07-03 21:29:25.000000 badger-opt-0.9.2/src/badger/gui/default/components/labeled_spinbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1091 2022-07-28 22:02:15.000000 badger-opt-0.9.2/src/badger/gui/default/components/objective_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3060 2023-02-01 23:33:32.000000 badger-opt-0.9.2/src/badger/gui/default/components/routine_editor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3249 2022-04-15 08:02:59.000000 badger-opt-0.9.2/src/badger/gui/default/components/routine_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    29456 2023-02-01 23:35:00.000000 badger-opt-0.9.2/src/badger/gui/default/components/routine_page.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3825 2023-02-01 23:34:30.000000 badger-opt-0.9.2/src/badger/gui/default/components/routine_runner.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    31504 2023-02-01 23:33:53.000000 badger-opt-0.9.2/src/badger/gui/default/components/run_monitor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      232 2022-03-11 21:08:44.000000 badger-opt-0.9.2/src/badger/gui/default/components/search_bar.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      949 2022-06-30 18:26:08.000000 badger-opt-0.9.2/src/badger/gui/default/components/state_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1291 2022-08-18 18:04:17.000000 badger-opt-0.9.2/src/badger/gui/default/components/status_bar.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     7164 2022-04-13 21:04:43.000000 badger-opt-0.9.2/src/badger/gui/default/components/syntax.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1043 2022-07-03 21:32:22.000000 badger-opt-0.9.2/src/badger/gui/default/components/variable_item.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/gui/default/images/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    17885 2022-08-18 17:54:53.000000 badger-opt-0.9.2/src/badger/gui/default/images/gear.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    46055 2022-08-18 17:51:33.000000 badger-opt-0.9.2/src/badger/gui/default/images/icon.png
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/gui/default/pages/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2022-03-11 21:02:36.000000 badger-opt-0.9.2/src/badger/gui/default/pages/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    15182 2023-02-01 23:34:10.000000 badger-opt-0.9.2/src/badger/gui/default/pages/home_page.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      668 2022-07-03 21:28:31.000000 badger-opt-0.9.2/src/badger/gui/default/utils.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/gui/default/windows/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2022-03-11 21:02:36.000000 badger-opt-0.9.2/src/badger/gui/default/windows/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1941 2022-04-13 21:04:01.000000 badger-opt-0.9.2/src/badger/gui/default/windows/edit_script_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1124 2022-05-08 01:28:03.000000 badger-opt-0.9.2/src/badger/gui/default/windows/main_window.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      778 2023-02-01 23:34:16.000000 badger-opt-0.9.2/src/badger/gui/default/windows/review_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5366 2023-02-01 23:35:31.000000 badger-opt-0.9.2/src/badger/gui/default/windows/settings_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3471 2023-02-01 23:35:16.000000 badger-opt-0.9.2/src/badger/gui/default/windows/var_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2628 2022-07-29 04:28:24.000000 badger-opt-0.9.2/src/badger/interface.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      955 2022-06-30 03:45:47.000000 badger-opt-0.9.2/src/badger/log.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4236 2022-07-13 07:26:27.000000 badger-opt-0.9.2/src/badger/logbook.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/logger/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4437 2022-06-21 17:28:06.000000 badger-opt-0.9.2/src/badger/logger/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      259 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/logger/event.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      937 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/logger/observer.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1616 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/logger/util.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3101 2022-08-25 19:31:51.000000 badger-opt-0.9.2/src/badger/settings.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      606 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/stats.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2094 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/conftest.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/configs/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       44 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/configs/test.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/__init__.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/silly/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      204 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/silly/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      488 2022-01-20 09:08:38.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/silly/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      108 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/silly/configs.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/simplex/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/simplex/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1036 2022-01-20 09:17:08.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/simplex/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      140 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/simplex/configs.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/environments/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/environments/silly/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/environments/silly/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1051 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/environments/silly/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       91 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/environments/silly/configs.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/interfaces/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/interfaces/silly/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       57 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/interfaces/silly/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1452 2022-01-20 09:17:08.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/interfaces/silly/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       70 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/mock/plugins/interfaces/silly/configs.yaml
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1209 2022-08-26 19:18:20.000000 badger-opt-0.9.2/src/badger/tests/test_cli_basic.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      350 2021-11-13 19:54:28.000000 badger-opt-0.9.2/src/badger/tests/test_gui_basic.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2322 2022-05-27 19:37:37.000000 badger-opt-0.9.2/src/badger/tests/test_lib_basic.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     6466 2022-07-21 21:08:59.000000 badger-opt-0.9.2/src/badger/utils.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      274 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/PKG-INFO
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3567 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        1 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       48 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/entry_points.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       95 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/requires.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        7 2023-02-02 09:05:07.000000 badger-opt-0.9.2/src/badger_opt.egg-info/top_level.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    80044 2021-11-13 19:54:28.000000 badger-opt-0.9.2/versioneer.py
```

### Comparing `badger-opt-0.9.1/LICENSE` & `badger-opt-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/README.md` & `badger-opt-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/setup.py` & `badger-opt-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/__main__.py` & `badger-opt-0.9.2/src/badger/__main__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/__init__.py` & `badger-opt-0.9.2/src/badger/actions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 
 def show_info(args):
     # Change log level for all existed loggers
     set_log_level(args.log)
 
     if args.gui:
-        from ..gui import launch_gui
+        from ..gui.default import launch_gui
 
         launch_gui()
     elif args.gui_acr:
-        from ..gui_acr import launch_gui
+        from ..gui.default import launch_gui
 
         launch_gui()
     else:
         try:
             from ..factory import BADGER_PLUGIN_ROOT, BADGER_EXTENSIONS
         except:
             BADGER_PLUGIN_ROOT = None
```

### Comparing `badger-opt-0.9.1/src/badger/actions/algo.py` & `badger-opt-0.9.2/src/badger/actions/algo.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/config.py` & `badger-opt-0.9.2/src/badger/actions/config.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/doctor.py` & `badger-opt-0.9.2/src/badger/actions/doctor.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/env.py` & `badger-opt-0.9.2/src/badger/actions/env.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/install.py` & `badger-opt-0.9.2/src/badger/actions/install.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/intf.py` & `badger-opt-0.9.2/src/badger/actions/intf.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/routine.py` & `badger-opt-0.9.2/src/badger/actions/routine.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/run.py` & `badger-opt-0.9.2/src/badger/actions/run.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/actions/uninstall.py` & `badger-opt-0.9.2/src/badger/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/archive.py` & `badger-opt-0.9.2/src/badger/archive.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/core.py` & `badger-opt-0.9.2/src/badger/core.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/db.py` & `badger-opt-0.9.2/src/badger/db.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/environment.py` & `badger-opt-0.9.2/src/badger/environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import numpy as np
 import time
 from abc import ABC, abstractmethod
 from typing import List
 from .interface import Interface
 from .utils import merge_params
+from .settings import read_value
+
+
+BADGER_CHECK_VAR_INTERVAL = float(read_value('BADGER_CHECK_VAR_INTERVAL'))
+BADGER_CHECK_VAR_TIMEOUT = float(read_value('BADGER_CHECK_VAR_TIMEOUT'))
 
 
 class Environment(ABC):
 
     @property
     @abstractmethod
     def name(self) -> str:
@@ -113,17 +118,21 @@
         if var not in self.list_vars():
             raise Exception(f'Variable {var} doesn\'t exist!')
 
         self._set_var(var, x)
 
         # Wait until check_var returns 0
         status = 1
+        time_start = time.time()
         while status:
+            time_elapsed = time.time() - time_start
+            if time_elapsed > BADGER_CHECK_VAR_TIMEOUT:
+                raise Exception(f'Set variable {var} timeout!')
             status = self._check_var(var)
-            time.sleep(0.1)
+            time.sleep(BADGER_CHECK_VAR_INTERVAL)
 
     # Safe version of _get_obs
     def get_obs(self, obs: str):
         if obs not in self.list_obses():
             raise Exception(f'Observation {obs} doesn\'t exist!')
 
         return self._get_obs(obs)
@@ -156,56 +165,72 @@
             values), 'Variables and values number mismatch!'
 
         for idx, var in enumerate(vars):
             self.set_var(var, values[idx])
 
         # Wait until all check_var calls return 0
         status = np.ones(len(vars))
+        time_start = time.time()
         while np.any(status):
+            time_elapsed = time.time() - time_start
+            if time_elapsed > BADGER_CHECK_VAR_TIMEOUT:
+                raise Exception(f'Set variable {vars[np.argmax(status)]} timeout!')
             for idx, var in enumerate(vars):
                 status[idx] = self._check_var(var)
-            time.sleep(0.1)
+            time.sleep(BADGER_CHECK_VAR_INTERVAL)
 
     # Unsafe version of set_vars
     def _set_vars(self, vars: List[str], values: list):
         assert len(vars) == len(
             values), 'Variables and values number mismatch!'
 
         for idx, var in enumerate(vars):
             self._set_var(var, values[idx])
 
         # Wait until all check_var calls return 0
         status = np.ones(len(vars))
+        time_start = time.time()
         while np.any(status):
+            time_elapsed = time.time() - time_start
+            if time_elapsed > BADGER_CHECK_VAR_TIMEOUT:
+                raise Exception(f'Set variable {vars[np.argmax(status)]} timeout!')
             for idx, var in enumerate(vars):
                 status[idx] = self._check_var(var)
-            time.sleep(0.1)
+            time.sleep(BADGER_CHECK_VAR_INTERVAL)
 
     def set_vars_dict(self, book: dict):
         for var, val in book.items():
             self.set_var(var, val)
 
         # Wait until all check_var calls return 0
         status = np.ones(len(book))
+        time_start = time.time()
         while np.any(status):
+            time_elapsed = time.time() - time_start
+            if time_elapsed > BADGER_CHECK_VAR_TIMEOUT:
+                raise Exception(f'Set variable {list(book.keys())[np.argmax(status)]} timeout!')
             for idx, var in enumerate(book.keys()):
                 status[idx] = self._check_var(var)
-            time.sleep(0.1)
+            time.sleep(BADGER_CHECK_VAR_INTERVAL)
 
     # Unsafe version of set_vars_dict
     def _set_vars_dict(self, book: dict):
         for var, val in book.items():
             self._set_var(var, val)
 
         # Wait until all check_var calls return 0
         status = np.ones(len(book))
+        time_start = time.time()
         while np.any(status):
+            time_elapsed = time.time() - time_start
+            if time_elapsed > BADGER_CHECK_VAR_TIMEOUT:
+                raise Exception(f'Set variable {list(book.keys())[np.argmax(status)]} timeout!')
             for idx, var in enumerate(book.keys()):
                 status[idx] = self._check_var(var)
-            time.sleep(0.1)
+            time.sleep(BADGER_CHECK_VAR_INTERVAL)
 
     def get_obses(self, obses: List[str]) -> list:
         values = []
         for obs in obses:
             values.append(self.get_obs(obs))
 
         return values
```

### Comparing `badger-opt-0.9.1/src/badger/extension.py` & `badger-opt-0.9.2/src/badger/extension.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/factory.py` & `badger-opt-0.9.2/src/badger/factory.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui/__init__.py` & `badger-opt-0.9.2/src/badger/gui/default/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pkg_resources import resource_filename
 import signal
 import time
-from PyQt5.QtWidgets import QApplication
+from PyQt5.QtWidgets import QApplication, QMessageBox
 from PyQt5.QtGui import QFont, QIcon
 from PyQt5 import QtCore
 import sys
 # import ctypes
 from qdarkstyle import load_stylesheet, LightPalette, DarkPalette
+from ...settings import read_value
 from .windows.main_window import BadgerMainWindow
 
 # Fix the scaling issue on multiple monitors w/ different scaling settings
 # if sys.platform == 'win32':
 #     ctypes.windll.shcore.SetProcessDpiAwareness(1)
 
 if hasattr(QtCore.Qt, 'AA_EnableHighDpiScaling'):
@@ -56,22 +57,16 @@
     app.setWindowIcon(QIcon(icon_path))
 
     font = QFont()
     font.setPixelSize(13)
     # font.setWeight(QFont.DemiBold)
     app.setFont(font)
 
-    # Configure app settings
-    settings = QtCore.QSettings('SLAC-ML', 'Badger')
-    theme = settings.value('theme')
-    if not theme:
-        settings.setValue('theme', 'dark')
-        theme = settings.value('theme')
-
     # Set up stylesheet
+    theme = read_value('BADGER_THEME')
     if theme == 'dark':
         app.setStyleSheet(load_stylesheet(palette=DarkPalette))
     elif theme == 'light':
         app.setStyleSheet(load_stylesheet(palette=LightPalette))
     else:
         app.setStyleSheet('')
 
@@ -82,8 +77,13 @@
     signal.signal(signal.SIGINT, on_exit)
     # Let the interpreter run each 0.2 s
     timer = QtCore.QTimer()
     timer.timeout.connect(on_timeout)
     timer.start(200)
 
     window.show()
+
+    # Show the saving SCORE heads-up
+    QMessageBox.information(
+            window, 'Heads-up!', 'This might be a good time to save a SCORE.')
+
     sys.exit(app.exec())
```

### Comparing `badger-opt-0.9.1/src/badger/gui/components/constraint_item.py` & `badger-opt-0.9.2/src/badger/gui/default/components/constraint_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from PyQt5.QtWidgets import QHBoxLayout, QPushButton, QWidget, QDoubleSpinBox, QAbstractSpinBox
 from PyQt5.QtWidgets import QComboBox, QCheckBox, QStyledItemDelegate
-from PyQt5.QtCore import QPropertyAnimation, QSize
+from PyQt5.QtCore import Qt
+from ..utils import MouseWheelWidgetAdjustmentGuard
 
 
 def constraint_item(options, remove_item, name=None, relation=0, threshold=0, critical=False, decimals=4):
     # relation: 0 for >, 1 for <, 2 for =
     widget = QWidget()
     hbox = QHBoxLayout(widget)
-    # hbox.setContentsMargins(0, 0, 0, 0)
+    hbox.setContentsMargins(2, 2, 2, 2)
     # hbox.setSpacing(0)
     widget.cb_obs = cb_obs = QComboBox()
+    cb_obs.setFixedWidth(200)
     cb_obs.setItemDelegate(QStyledItemDelegate())
     cb_obs.addItems(options)
     try:
         idx = options.index(name)
     except:
         idx = 0
     cb_obs.setCurrentIndex(idx)
@@ -22,14 +24,16 @@
     cb_rel.setItemDelegate(QStyledItemDelegate())
     cb_rel.addItems(['>', '<', '='])
     cb_rel.setFixedWidth(64)
     cb_rel.setCurrentIndex(relation)
 
     widget.sb = sb = QDoubleSpinBox()
     sb.setDecimals(decimals)
+    sb.setFocusPolicy(Qt.StrongFocus)
+    sb.installEventFilter(MouseWheelWidgetAdjustmentGuard(sb))
     default_value = threshold
     lb = default_value - 1e3
     ub = default_value + 1e3
     sb.setRange(lb, ub)
     sb.setStepType(QAbstractSpinBox.AdaptiveDecimalStepType)
     sb.setValue(default_value)
 
@@ -37,15 +41,15 @@
     check_crit.setChecked(critical)
 
     widget.btn_del = btn_del = QPushButton('Remove')
     btn_del.setFixedSize(72, 24)
     btn_del.hide()
 
     hbox.addWidget(check_crit)
-    hbox.addWidget(cb_obs, 1)
+    hbox.addWidget(cb_obs)
     hbox.addWidget(cb_rel)
     hbox.addWidget(sb, 1)
     hbox.addWidget(btn_del)
 
     btn_del.clicked.connect(remove_item)
 
     def show_button(event):
```

### Comparing `badger-opt-0.9.1/src/badger/gui/components/labeled_lineedit.py` & `badger-opt-0.9.2/src/badger/gui/default/components/labeled_lineedit.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui/components/labeled_spinbox.py` & `badger-opt-0.9.2/src/badger/gui/default/components/labeled_spinbox.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from PyQt5.QtWidgets import QHBoxLayout, QLabel, QWidget, QDoubleSpinBox, QAbstractSpinBox
+from PyQt5.QtCore import Qt
+from ..utils import MouseWheelWidgetAdjustmentGuard
 
 
 def labeled_spinbox(name, default_value, lb, ub, decimals=4):
     widget = QWidget()
     hbox = QHBoxLayout(widget)
     hbox.setContentsMargins(0, 0, 0, 0)
     label = QLabel(name)
     widget.sb = sb = QDoubleSpinBox()
     sb.setDecimals(decimals)
+    sb.setFocusPolicy(Qt.StrongFocus)
+    sb.installEventFilter(MouseWheelWidgetAdjustmentGuard(sb))
 
     # Sanity check
     if lb is None:
         lb = -1e3
     if ub is None:
         ub = 1e3
     if default_value is None:
```

### Comparing `badger-opt-0.9.1/src/badger/gui/components/objective_item.py` & `badger-opt-0.9.2/src/badger/gui/default/components/objective_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from PyQt5.QtWidgets import QHBoxLayout, QWidget, QVBoxLayout, QCheckBox, QLabel
+from PyQt5.QtWidgets import QHBoxLayout, QWidget, QCheckBox, QLabel
 from PyQt5.QtWidgets import QComboBox, QStyledItemDelegate
 
 
 def objective_item(name, rule, callback=None):
     # rule: 0 for MINIMIZE, 1 for MAXIMIZE
     widget = QWidget()
-    vbox = QVBoxLayout(widget)
-    vbox.setSpacing(0)
+    hbox = QHBoxLayout(widget)
+    hbox.setContentsMargins(2, 2, 2, 2)
     widget.check_name = check_name = QCheckBox(name)
+    check_name.setFixedWidth(200)
     check_name.setChecked(True)
-    vbox.addWidget(check_name)
+    hbox.addWidget(check_name)
     widget_rule = QWidget()
-    hbox = QHBoxLayout(widget_rule)
-    hbox.setContentsMargins(0, 0, 0, 0)
+    hbox.addWidget(widget_rule)
+    hbox_rule = QHBoxLayout(widget_rule)
+    hbox_rule.setContentsMargins(0, 0, 0, 0)
     label = QLabel('rule')
     widget.cb_rule = cb_rule = QComboBox()
     cb_rule.setItemDelegate(QStyledItemDelegate())
     cb_rule.addItems(['MINIMIZE', 'MAXIMIZE'])
     cb_rule.setCurrentIndex(rule)
-    hbox.addWidget(label)
-    hbox.addWidget(cb_rule, 1)
-    vbox.addWidget(widget_rule)
+    hbox_rule.addWidget(label)
+    hbox_rule.addWidget(cb_rule, 1)
 
     def toggle_item():
         widget_rule.setDisabled(not check_name.isChecked())
         if callback is not None:
             callback(name)
 
     check_name.stateChanged.connect(toggle_item)
```

### Comparing `badger-opt-0.9.1/src/badger/gui/components/routine_runner.py` & `badger-opt-0.9.2/src/badger/gui/default/components/routine_runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,63 @@
+import logging
+logger = logging.getLogger(__name__)
 import time
 import pandas as pd
 from PyQt5.QtCore import pyqtSignal, QObject, QRunnable
-from ...utils import curr_ts, ts_to_str
-from ...core import run_routine
+from ....utils import curr_ts, ts_to_str
+from ....core import run_routine
 
 
 class BadgerRoutineSignals(QObject):
     env_ready = pyqtSignal(list)
     finished = pyqtSignal()
-    progress = pyqtSignal(list, list, list)
+    progress = pyqtSignal(list, list, list, list, float)
     error = pyqtSignal(Exception)
     info = pyqtSignal(str)
 
 
 class BadgerRoutineRunner(QRunnable):
 
     def __init__(self, routine, save, verbose=2, use_full_ts=False):
         super().__init__()
 
         # Signals should belong to instance rather than class
         # Since there could be multiple runners runing in parallel
         self.signals = BadgerRoutineSignals()
 
         self.routine = routine
+        self.run_filename = None
         self.var_names = var_names = [next(iter(d)) for d in routine['config']['variables']]
         self.obj_names = obj_names = [next(iter(d)) for d in routine['config']['objectives']]
         if routine['config']['constraints']:
             self.con_names = con_names = [next(iter(d)) for d in routine['config']['constraints']]
         else:
             self.con_names = con_names = []
-        self.data = pd.DataFrame(None, columns=['timestamp_raw', 'timestamp'] + obj_names + con_names + var_names)
+        try:
+            self.sta_names = sta_names = routine['config']['states'] or []
+        except KeyError:  # this would happen when rerun an old version routine
+            self.sta_names = sta_names = []
+        self.data = pd.DataFrame(None, columns=['timestamp_raw', 'timestamp'] + obj_names + con_names + var_names + sta_names)
+        self.states = None  # system states to be saved at start of a run
         self.save = save
         self.verbose = verbose
         self.use_full_ts = use_full_ts
 
         self.is_paused = False
         self.is_killed = False
 
     def run(self):
         error = None
         try:
             run_routine(self.routine, True, self.save, self.verbose,
                         self.before_evaluate, self.after_evaluate,
-                        self.env_ready, self.pf_ready)
+                        self.env_ready, self.pf_ready, self.states_ready)
         except Exception as e:
+            if str(e) != 'Optimization run has been terminated!':
+                logger.exception(e)
             error = e
 
         self.signals.finished.emit()
         if error:
             if str(error) == 'Optimization run has been terminated!':
                 self.signals.info.emit(str(error))
                 return
@@ -60,35 +70,39 @@
             time.sleep(0)
             if self.is_killed:
                 raise Exception('Optimization run has been terminated!')
 
         if self.is_killed:
             raise Exception('Optimization run has been terminated!')
 
-    def after_evaluate(self, vars, obses, cons):
+    def after_evaluate(self, vars, obses, cons, stas):
         # vars: ndarray
         # obses: ndarray
         # cons: ndarray
-        self.signals.progress.emit(list(vars), list(obses), list(cons))
+        # stas: list
+        ts = curr_ts()
+        self.signals.progress.emit(list(vars), list(obses), list(cons), list(stas), ts.timestamp())
 
         # Append solution to data
         fmt = 'lcls-log-full' if self.use_full_ts else 'lcls-log'
-        ts = curr_ts()
-        solution = [ts.timestamp(), ts_to_str(ts, fmt)] + list(obses) + list(cons) + list(vars)
+        solution = [ts.timestamp(), ts_to_str(ts, fmt)] + list(obses) + list(cons) + list(vars) + list(stas)
         self.data = self.data.append(pd.Series(solution, index=self.data.columns), ignore_index=True)
 
         # take a break to let the outside signal to change the status
         time.sleep(0.1)
 
     def env_ready(self, env):
         self.env = env
         init_vars = env._get_vars(self.var_names)
         self.signals.env_ready.emit(init_vars)
 
     def pf_ready(self, pf):
         self.pf = pf
 
+    def states_ready(self, states):
+        self.states = states
+
     def ctrl_routine(self, pause):
         self.is_paused = pause
 
     def stop_routine(self):
         self.is_killed = True
```

### Comparing `badger-opt-0.9.1/src/badger/gui/components/syntax.py` & `badger-opt-0.9.2/src/badger/gui/default/components/syntax.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui/images/icon.png` & `badger-opt-0.9.2/src/badger/gui/default/images/icon.png`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui/pages/routine_page.py` & `badger-opt-0.9.2/src/badger/gui/default/components/routine_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,287 +1,238 @@
-from PyQt5.QtWidgets import QLineEdit, QListWidget, QListWidgetItem, QWidget, QVBoxLayout, QHBoxLayout
-from PyQt5.QtWidgets import QPushButton, QGroupBox, QComboBox, QLineEdit, QPlainTextEdit, QCheckBox
-from PyQt5.QtWidgets import QMessageBox, QStyledItemDelegate
+from PyQt5.QtWidgets import QLineEdit, QListWidgetItem, QWidget, QVBoxLayout, QHBoxLayout, QFrame
+from PyQt5.QtWidgets import QGroupBox, QLineEdit, QLabel, QMessageBox, QComboBox, QStyledItemDelegate
 from PyQt5.QtCore import QSize
-from PyQt5.QtGui import QFont
+import sqlite3
 from coolname import generate_slug
-from ...factory import list_algo, list_env, get_algo, get_env
-from ...utils import ystring, load_config, config_list_to_dict
-from ...core import normalize_routine, instantiate_env
-from ..components.variable_item import variable_item
-from ..components.objective_item import objective_item
-from ..components.constraint_item import constraint_item
+from ....factory import list_algo, list_env, get_algo, get_env
+from ....utils import ystring, load_config, config_list_to_dict
+from ....core import normalize_routine, instantiate_env, list_scaling_func, get_scaling_default_params
+from ....db import save_routine, remove_routine
+from .variable_item import variable_item
+from .objective_item import objective_item
+from .constraint_item import constraint_item
+from .state_item import state_item
+from .algo_cbox import BadgerAlgoBox
+from .env_cbox import BadgerEnvBox
 from ..windows.review_dialog import BadgerReviewDialog
-from ..windows.opt_monitor import BadgerOptMonitor
 from ..windows.var_dialog import BadgerVariableDialog
 from ..windows.edit_script_dialog import BadgerEditScriptDialog
 
 
 CONS_RELATION_DICT = {
     '>': 'GREATER_THAN',
     '<': 'LESS_THAN',
     '=': 'EQUAL_TO',
 }
 
 
 class BadgerRoutinePage(QWidget):
-    def __init__(self, go_home=None):
+    def __init__(self):
         super().__init__()
 
-        self.go_home = go_home
-
         self.algos = list_algo()
         self.envs = list_env()
         self.env = None
+        self.routine = None
         self.script = ''
+        self.scaling_functions = list_scaling_func()
 
         self.init_ui()
         self.config_logic()
 
     def init_ui(self):
         # Set up the layout
         vbox = QVBoxLayout(self)
+        vbox.setContentsMargins(11, 11, 19, 11)
 
-        # Algo and env configs
-        panel_int = QWidget()
-        hbox_int = QHBoxLayout(panel_int)
-        hbox_int.setContentsMargins(0, 0, 0, 0)
-
-        group_algo = QGroupBox('Algorithm')
-        vbox_algo = QVBoxLayout(group_algo)
-        action_algo = QWidget()
-        hbox_action_algo = QHBoxLayout(action_algo)
-        hbox_action_algo.setContentsMargins(0, 0, 0, 0)
-        self.cb_algo = cb_algo = QComboBox()
-        cb_algo.setItemDelegate(QStyledItemDelegate())
-        cb_algo.addItems(self.algos)
-        cb_algo.setCurrentIndex(-1)
-        self.check_use_script = check_use_script = QCheckBox('Use Script')
-        check_use_script.setChecked(False)
-        self.btn_edit_script = btn_edit_script = QPushButton('Edit Script')
-        btn_edit_script.setFixedSize(96, 24)
-        btn_edit_script.hide()
-        hbox_action_algo.addWidget(cb_algo, 1)
-        hbox_action_algo.addWidget(check_use_script)
-        hbox_action_algo.addWidget(btn_edit_script)
-        vbox_algo.addWidget(action_algo)
-        self.edit_algo = edit_algo = QPlainTextEdit()
-        edit_algo.setFixedHeight(128)
-        vbox_algo.addWidget(edit_algo)
-        hbox_int.addWidget(group_algo)
-
-        group_env = QGroupBox('Environment')
-        vbox_env = QVBoxLayout(group_env)
-        action_env = QWidget()
-        hbox_action_env = QHBoxLayout(action_env)
-        hbox_action_env.setContentsMargins(0, 0, 0, 0)
-        self.cb_env = cb_env = QComboBox()
-        cb_env.setItemDelegate(QStyledItemDelegate())
-        cb_env.addItems(self.envs)
-        cb_env.setCurrentIndex(-1)
-        self.btn_env_play = btn_env_play = QPushButton('Playground')
-        btn_env_play.setFixedSize(96, 24)
-        btn_env_play.hide()  # hide for now to prevent confusions
-        hbox_action_env.addWidget(cb_env, 1)
-        hbox_action_env.addWidget(btn_env_play)
-        vbox_env.addWidget(action_env)
-        self.edit_env = edit_env = QPlainTextEdit()
-        edit_env.setFixedHeight(128)
-        vbox_env.addWidget(edit_env)
-        hbox_int.addWidget(group_env)
-        vbox.addWidget(panel_int)
-
-        # Configs group
-        group_ext = QGroupBox('Configs')
-        hbox_ext = QHBoxLayout(group_ext)
-
-        group_var = QGroupBox('Variables')
-        vbox_var = QVBoxLayout(group_var)
-        action_var = QWidget()
-        hbox_action_var = QHBoxLayout(action_var)
-        hbox_action_var.setContentsMargins(0, 0, 0, 0)
-        self.btn_all_var = btn_all_var = QPushButton('Check All')
-        self.btn_un_all_var = btn_un_all_var = QPushButton('Uncheck All')
-        btn_all_var.setFixedSize(96, 24)
-        btn_un_all_var.setFixedSize(96, 24)
-        self.btn_add_var = btn_add_var = QPushButton('Add')
-        btn_add_var.setFixedSize(96, 24)
-        btn_add_var.setDisabled(True)
-        self.check_only_var = check_only_var = QCheckBox('Checked Only')
-        check_only_var.setChecked(False)
-        hbox_action_var.addWidget(btn_all_var)
-        hbox_action_var.addWidget(btn_un_all_var)
-        hbox_action_var.addWidget(btn_add_var)
-        hbox_action_var.addStretch()
-        hbox_action_var.addWidget(check_only_var)
-        vbox_var.addWidget(action_var)
-        self.list_var = list_var = QListWidget()
-        self.dict_var = {}
-        vbox_var.addWidget(list_var)
-        hbox_ext.addWidget(group_var)
-
-        group_obj = QGroupBox('Objectives')
-        vbox_obj = QVBoxLayout(group_obj)
-        action_obj = QWidget()
-        hbox_action_obj = QHBoxLayout(action_obj)
-        hbox_action_obj.setContentsMargins(0, 0, 0, 0)
-        self.btn_all_obj = btn_all_obj = QPushButton('Check All')
-        self.btn_un_all_obj = btn_un_all_obj = QPushButton('Uncheck All')
-        btn_all_obj.setFixedSize(96, 24)
-        btn_un_all_obj.setFixedSize(96, 24)
-        self.check_only_obj = check_only_obj = QCheckBox('Checked Only')
-        check_only_obj.setChecked(False)
-        hbox_action_obj.addWidget(btn_all_obj)
-        hbox_action_obj.addWidget(btn_un_all_obj)
-        hbox_action_obj.addStretch()
-        hbox_action_obj.addWidget(check_only_obj)
-        vbox_obj.addWidget(action_obj)
-        self.list_obj = list_obj = QListWidget()
-        self.dict_obj = {}
-        vbox_obj.addWidget(list_obj)
-        hbox_ext.addWidget(group_obj)
-
-        group_con = QGroupBox('Constraints')
-        vbox_con = QVBoxLayout(group_con)
-        action_con = QWidget()
-        hbox_action_con = QHBoxLayout(action_con)
-        hbox_action_con.setContentsMargins(0, 0, 0, 0)
-        self.btn_add_con = btn_add_con = QPushButton('Add')
-        btn_add_con.setFixedSize(96, 24)
-        btn_add_con.setDisabled(True)
-        hbox_action_con.addWidget(btn_add_con)
-        hbox_action_con.addStretch()
-        vbox_con.addWidget(action_con)
-        self.list_con = list_con = QListWidget()
-        self.dict_con = {}
-        vbox_con.addWidget(list_con)
-        hbox_ext.addWidget(group_con)
-
-        vbox.addWidget(group_ext, 1)
-
-        # Misc group
-        group_misc = QGroupBox('Misc')
-        hbox_misc = QHBoxLayout(group_misc)
-        self.check_save = check_save = QCheckBox('Save as')
-        check_save.setChecked(False)
+        # Meta group
+        group_meta = QGroupBox('Metadata')
+        vbox_meta = QVBoxLayout(group_meta)
+
+        # Name
+        name = QWidget()
+        hbox_name = QHBoxLayout(name)
+        hbox_name.setContentsMargins(0, 0, 0, 0)
+        label = QLabel('Name')
+        label.setFixedWidth(64)
         self.edit_save = edit_save = QLineEdit()
         edit_save.setPlaceholderText(generate_slug(2))
-        edit_save.setDisabled(True)
-        hbox_misc.addWidget(check_save)
-        hbox_misc.addWidget(edit_save, 1)
-        hbox_misc.addStretch(2)
-
-        vbox.addWidget(group_misc)
-
-        # Action bar
-        action_bar = QWidget()
-        hbox_action = QHBoxLayout(action_bar)
-        hbox_action.setContentsMargins(0, 0, 0, 0)
-        self.btn_back = btn_back = QPushButton('Back')
-        self.btn_review = btn_review = QPushButton('Review')
-        self.btn_run = btn_run = QPushButton('Run Routine')
-
-        cool_font = QFont()
-        cool_font.setWeight(QFont.DemiBold)
-        # cool_font.setPixelSize(16)
-
-        btn_back.setFixedSize(64, 64)
-        btn_back.setFont(cool_font)
-        btn_review.setFixedSize(64, 64)
-        btn_review.setFont(cool_font)
-        btn_run.setFixedSize(256, 64)
-        btn_run.setFont(cool_font)
-        hbox_action.addWidget(btn_back)
-        hbox_action.addWidget(btn_review)
-        hbox_action.addStretch(1)
-        hbox_action.addWidget(btn_run)
+        hbox_name.addWidget(label)
+        hbox_name.addWidget(edit_save, 1)
+        vbox_meta.addWidget(name)
+
+        seperator = QFrame()
+        seperator.setFrameShape(QFrame.HLine)
+        seperator.setFrameShadow(QFrame.Sunken)
+        seperator.setLineWidth(0)
+        seperator.setMidLineWidth(0)
+        vbox_meta.addWidget(seperator)
+
+        # Obj tag
+        obj = QWidget()
+        hbox_obj = QHBoxLayout(obj)
+        hbox_obj.setContentsMargins(0, 0, 0, 0)
+        lbl = QLabel('Objective')
+        lbl.setFixedWidth(64)
+        self.cb_obj = cb_obj = QComboBox()
+        cb_obj.setItemDelegate(QStyledItemDelegate())
+        cb_obj.addItems(['', 'HXR', 'SXR'])
+        cb_obj.setCurrentIndex(-1)
+        hbox_obj.addWidget(lbl)
+        hbox_obj.addWidget(cb_obj, 1)
+        vbox_meta.addWidget(obj)
+
+        # Region tag
+        region = QWidget()
+        hbox_reg = QHBoxLayout(region)
+        hbox_reg.setContentsMargins(0, 0, 0, 0)
+        lbl = QLabel('Region')
+        lbl.setFixedWidth(64)
+        self.cb_reg = cb_reg = QComboBox()
+        cb_reg.setItemDelegate(QStyledItemDelegate())
+        cb_reg.addItems([
+            '',
+            'LI21:201, 211, 271, 278',
+            'LI26:201, 301, 401, 501',
+            'LI26:601, 701, 801, 901',
+            'IN20:361, 371, 425, 441, 511, 525',
+            'LTUH:620, 640, 660, 680',
+            'LTUS:620, 640, 660, 680',
+        ])
+        cb_reg.setCurrentIndex(-1)
+        hbox_reg.addWidget(lbl)
+        hbox_reg.addWidget(cb_reg, 1)
+        vbox_meta.addWidget(region)
+
+        # Gain tag
+        gain = QWidget()
+        hbox_gain = QHBoxLayout(gain)
+        hbox_gain.setContentsMargins(0, 0, 0, 0)
+        lbl = QLabel('Gain')
+        lbl.setFixedWidth(64)
+        self.cb_gain = cb_gain = QComboBox()
+        cb_gain.setItemDelegate(QStyledItemDelegate())
+        cb_gain.addItems([
+            '',
+            '1',
+            '2',
+            '4',
+            '8',
+        ])
+        cb_gain.setCurrentIndex(-1)
+        hbox_gain.addWidget(lbl)
+        hbox_gain.addWidget(cb_gain, 1)
+        vbox_meta.addWidget(gain)
+
+        # hbox_meta.addStretch(2)
+        vbox.addWidget(group_meta)
+
+        # Algo box
+        self.algo_box = BadgerAlgoBox(self.algos, self.scaling_functions)
+        self.algo_box.expand()  # expand the box initially
+        vbox.addWidget(self.algo_box)
+
+        # Env box
+        self.env_box = BadgerEnvBox(self.envs)
+        self.env_box.expand()  # expand the box initially
+        vbox.addWidget(self.env_box)
 
-        # vbox.addSpacing(16)
-        vbox.addWidget(action_bar)
+        vbox.addStretch()
 
     def config_logic(self):
-        self.btn_back.clicked.connect(self.go_home)
-        self.cb_algo.currentIndexChanged.connect(self.select_algo)
-        self.check_use_script.stateChanged.connect(self.toggle_use_script)
-        self.btn_edit_script.clicked.connect(self.edit_script)
-        self.cb_env.currentIndexChanged.connect(self.select_env)
-        self.btn_env_play.clicked.connect(self.open_playground)
-        self.btn_all_var.clicked.connect(self.check_all_var)
-        self.btn_un_all_var.clicked.connect(self.uncheck_all_var)
-        self.btn_add_var.clicked.connect(self.add_var)
-        self.btn_all_obj.clicked.connect(self.check_all_obj)
-        self.btn_un_all_obj.clicked.connect(self.uncheck_all_obj)
-        self.check_only_var.stateChanged.connect(self.toggle_check_only_var)
-        self.check_only_obj.stateChanged.connect(self.toggle_check_only_obj)
-        self.btn_add_con.clicked.connect(self.add_constraint)
-        self.check_save.stateChanged.connect(self.toggle_save)
-        self.btn_review.clicked.connect(self.review)
-        self.btn_run.clicked.connect(self.run)
+        self.algo_box.cb.currentIndexChanged.connect(self.select_algo)
+        self.algo_box.check_use_script.stateChanged.connect(self.toggle_use_script)
+        self.algo_box.btn_edit_script.clicked.connect(self.edit_script)
+        self.algo_box.cb_scaling.currentIndexChanged.connect(self.select_scaling_func)
+        self.env_box.cb.currentIndexChanged.connect(self.select_env)
+        self.env_box.btn_env_play.clicked.connect(self.open_playground)
+        self.env_box.btn_all_var.clicked.connect(self.check_all_var)
+        self.env_box.btn_un_all_var.clicked.connect(self.uncheck_all_var)
+        self.env_box.btn_add_var.clicked.connect(self.add_var)
+        self.env_box.btn_all_obj.clicked.connect(self.check_all_obj)
+        self.env_box.btn_un_all_obj.clicked.connect(self.uncheck_all_obj)
+        self.env_box.check_only_var.stateChanged.connect(self.toggle_check_only_var)
+        self.env_box.check_only_obj.stateChanged.connect(self.toggle_check_only_obj)
+        self.env_box.btn_add_con.clicked.connect(self.add_constraint)
+        self.env_box.btn_add_sta.clicked.connect(self.add_state)
 
     def refresh_ui(self, routine):
         self.routine = routine  # save routine for future reference
 
         self.algos = list_algo()
         self.envs = list_env()
-        # Clean up the constraints list
-        self.list_con.clear()
+        # Clean up the constraints/states list
+        self.env_box.list_con.clear()
+        self.env_box.list_sta.clear()
 
         if routine is None:
             # Reset the algo and env configs
-            self.cb_algo.setCurrentIndex(-1)
-            self.cb_env.setCurrentIndex(-1)
+            self.algo_box.cb.setCurrentIndex(-1)
+            self.env_box.cb.setCurrentIndex(-1)
 
             # Reset the routine configs check box status
-            self.check_only_var.setChecked(False)
-            self.check_only_obj.setChecked(False)
+            self.env_box.check_only_var.setChecked(False)
+            self.env_box.check_only_obj.setChecked(False)
 
             # Reset the save settings
             name = generate_slug(2)
             self.edit_save.setText('')
             self.edit_save.setPlaceholderText(name)
-            self.check_save.setChecked(False)
 
             return
 
         # Fill in the algo and env configs
         name_algo = routine['algo']
         idx_algo = self.algos.index(name_algo)
-        self.cb_algo.setCurrentIndex(idx_algo)
-        self.edit_algo.setPlainText(ystring(routine['algo_params']))
+        self.algo_box.cb.setCurrentIndex(idx_algo)
+        self.algo_box.edit.setPlainText(ystring(routine['algo_params']))
         try:
             self.script = routine['config']['script']
         except KeyError:
             self.script = None
+        try:
+            name_scaling = routine['config']['domain_scaling']['func']
+            params_scaling = routine['config']['domain_scaling'].copy()
+            del params_scaling['func']
+        except:
+            name_scaling = None
+            params_scaling = None
+        try:
+            idx_scaling = self.scaling_functions.index(name_scaling)
+        except ValueError:
+            idx_scaling = -1
+        self.algo_box.cb_scaling.setCurrentIndex(idx_scaling)
+        self.algo_box.edit_scaling.setPlainText(ystring(params_scaling))
 
         name_env = routine['env']
         idx_env = self.envs.index(name_env)
-        self.cb_env.setCurrentIndex(idx_env)
-        self.edit_env.setPlainText(ystring(routine['env_params']))
+        self.env_box.cb.setCurrentIndex(idx_env)
+        self.env_box.edit.setPlainText(ystring(routine['env_params']))
 
         # Config the vocs panel
-        self.check_only_var.setChecked(True)
+        self.env_box.check_only_var.setChecked(True)
         variables = [next(iter(v)) for v in routine['config']['variables']]
-        for i in range(self.list_var.count()):
-            item = self.list_var.item(i)
-            item_widget = self.list_var.itemWidget(item)
+        for i in range(self.env_box.list_var.count()):
+            item = self.env_box.list_var.item(i)
+            item_widget = self.env_box.list_var.itemWidget(item)
             var_name = item_widget.check_name.text()
             try:
                 idx = variables.index(var_name)
                 vrange = routine['config']['variables'][idx][var_name]
                 item_widget.sb_lower.sb.setValue(vrange[0])
                 item_widget.sb_upper.sb.setValue(vrange[1])
                 item_widget.check_name.setChecked(True)
             except ValueError:
                 item_widget.check_name.setChecked(False)
 
-        self.check_only_obj.setChecked(True)
+        self.env_box.check_only_obj.setChecked(True)
         objectives = [next(iter(v)) for v in routine['config']['objectives']]
-        for i in range(self.list_obj.count()):
-            item = self.list_obj.item(i)
-            item_widget = self.list_obj.itemWidget(item)
+        for i in range(self.env_box.list_obj.count()):
+            item = self.env_box.list_obj.item(i)
+            item_widget = self.env_box.list_obj.itemWidget(item)
             obj_name = item_widget.check_name.text()
             try:
                 idx = objectives.index(obj_name)
                 rule = routine['config']['objectives'][idx][obj_name]
                 idx_rule = 0 if rule == 'MINIMIZE' else 1
                 item_widget.cb_rule.setCurrentIndex(idx_rule)
                 item_widget.check_name.setChecked(True)
@@ -297,51 +248,74 @@
                     critical = True
                 except:
                     critical = False
                 relation = ['GREATER_THAN', 'LESS_THAN',
                             'EQUAL_TO'].index(relation)
                 self.add_constraint(name, relation, thres, critical)
 
-        # Config the save settings
+        try:
+            config_states = routine['config']['states']
+        except KeyError:
+            config_states = None
+        if config_states is not None:
+            for name_sta in config_states:
+                self.add_state(name_sta)
+
+        # Config the metadata
         name = routine['name']
         self.edit_save.setPlaceholderText(generate_slug(2))
         self.edit_save.setText(name)
-        self.check_save.setChecked(False)
+        try:
+            tags = routine['config']['tags']
+        except:
+            tags = {}
+        try:
+            self.cb_obj.setCurrentText(tags['objective'])
+        except:
+            self.cb_obj.setCurrentIndex(0)
+        try:
+            self.cb_reg.setCurrentText(tags['region'])
+        except:
+            self.cb_reg.setCurrentIndex(0)
+        try:
+            self.cb_gain.setCurrentText(tags['gain'])
+        except:
+            self.cb_gain.setCurrentIndex(0)
 
-        if self.script:
-            self.check_use_script.setChecked(True)
+        self.algo_box.check_use_script.setChecked(not not self.script)
 
     def select_algo(self, i):
         # Reset the script
         self.script = ''
-        self.check_use_script.setChecked(False)
+        self.algo_box.check_use_script.setChecked(False)
 
         if i == -1:
-            self.edit_algo.setPlainText('')
+            self.algo_box.edit.setPlainText('')
+            self.algo_box.cb_scaling.setCurrentIndex(-1)
             return
 
         name = self.algos[i]
         try:
             _, configs = get_algo(name)
-            self.edit_algo.setPlainText(ystring(configs['params']))
+            self.algo_box.edit.setPlainText(ystring(configs['params']))
         except Exception as e:
-            self.cb_algo.setCurrentIndex(-1)
+            self.algo_box.cb.setCurrentIndex(-1)
             return QMessageBox.critical(self, 'Error!', str(e))
 
     def toggle_use_script(self):
-        if self.check_use_script.isChecked():
-            self.btn_edit_script.show()
-            self.edit_algo.setReadOnly(True)
+        if self.algo_box.check_use_script.isChecked():
+            self.algo_box.btn_edit_script.show()
+            self.algo_box.edit.setReadOnly(True)
             self.refresh_params_algo()
         else:
-            self.btn_edit_script.hide()
-            self.edit_algo.setReadOnly(False)
+            self.algo_box.btn_edit_script.hide()
+            self.algo_box.edit.setReadOnly(False)
 
     def edit_script(self):
-        algo = self.cb_algo.currentText()
+        algo = self.algo_box.cb.currentText()
         dlg = BadgerEditScriptDialog(self, algo, self.script, self.script_updated)
         dlg.exec()
 
     def script_updated(self, text):
         self.script = text
         self.refresh_params_algo()
 
@@ -354,15 +328,15 @@
             exec(self.script, tmp)
             try:
                 tmp['generate']  # test if generate function is defined
             except Exception as e:
                 QMessageBox.warning(self, 'Please define a valid generate function!', str(e))
                 return
 
-            env_params = load_config(self.edit_env.toPlainText())
+            env_params = load_config(self.env_box.edit.toPlainText())
             try:
                 intf_name = self.configs['interface'][0]
             except KeyError:
                 intf_name = None
             configs = {
                 'params': env_params,
                 'interface': [intf_name]
@@ -371,53 +345,69 @@
             # Get vocs
             try:
                 vocs = self._compose_vocs()
             except Exception:
                 vocs = None
             # Function generate comes from the script
             params_algo = tmp['generate'](env, vocs)
-            self.edit_algo.setPlainText(ystring(params_algo))
+            self.algo_box.edit.setPlainText(ystring(params_algo))
         except Exception as e:
             QMessageBox.warning(self, 'Invalid script!', str(e))
 
+    def select_scaling_func(self, i):
+        if i == -1:
+            self.algo_box.edit_scaling.setPlainText('')
+            return
+
+        try:
+            name = self.scaling_functions[i]
+            default_params = get_scaling_default_params(name)
+            self.algo_box.edit_scaling.setPlainText(ystring(default_params))
+        except Exception as e:
+            self.algo_box.cb.setCurrentIndex(-1)
+            return QMessageBox.critical(self, 'Error!', str(e))
+
     def select_env(self, i):
         if i == -1:
-            self.edit_env.setPlainText('')
-            self.list_var.clear()
-            self.dict_var.clear()
-            self.list_obj.clear()
-            self.dict_obj.clear()
+            self.env_box.edit.setPlainText('')
+            self.env_box.list_var.clear()
+            self.env_box.dict_var.clear()
+            self.env_box.list_obj.clear()
+            self.env_box.dict_obj.clear()
             self.configs = None
             self.env = None
-            self.btn_add_con.setDisabled(True)
-            self.btn_add_var.setDisabled(True)
+            self.env_box.btn_add_con.setDisabled(True)
+            self.env_box.btn_add_sta.setDisabled(True)
+            self.env_box.btn_add_var.setDisabled(True)
             self.routine = None
             return
 
         name = self.envs[i]
         try:
             env, configs = get_env(name)
             self.configs = configs
             self.env = env
-            self.btn_add_con.setDisabled(False)
-            self.btn_add_var.setDisabled(False)
-            if self.check_use_script.isChecked():
+            self.env_box.btn_add_con.setDisabled(False)
+            self.env_box.btn_add_sta.setDisabled(False)
+            self.env_box.btn_add_var.setDisabled(False)
+            if self.algo_box.check_use_script.isChecked():
                 self.refresh_params_algo()
         except Exception as e:
             self.configs = None
             self.env = None
-            self.cb_env.setCurrentIndex(-1)
-            self.btn_add_con.setDisabled(True)
-            self.btn_add_var.setDisabled(True)
+            self.env_box.cb.setCurrentIndex(-1)
+            self.env_box.btn_add_con.setDisabled(True)
+            self.env_box.btn_add_sta.setDisabled(True)
+            self.env_box.btn_add_var.setDisabled(True)
             self.routine = None
             return QMessageBox.critical(self, 'Error!', str(e))
 
-        self.edit_env.setPlainText(ystring(configs['params']))
+        self.env_box.edit.setPlainText(ystring(configs['params']))
 
-        self.list_var.clear()
+        self.env_box.list_var.clear()
         vars_env = configs['variables']
         vars_combine = [*vars_env]
         if self.routine:  # check for the temp variables in vocs
             vars_vocs = self.routine['config']['variables']
             var_names_vocs = [next(iter(var)) for var in vars_vocs]
             var_names_env = [next(iter(var)) for var in vars_env]
             env_instance = instantiate_env(env, configs)
@@ -427,51 +417,53 @@
 
                 _var = {}
                 _var[name] = env_instance._get_vrange(name)
                 vars_combine.append(_var)
         for var in vars_combine:
             name = next(iter(var))
             vrange = var[name]
-            item = QListWidgetItem(self.list_var)
+            item = QListWidgetItem(self.env_box.list_var)
             var_item = variable_item(name, vrange, self.toggle_var)
             item.setSizeHint(var_item.sizeHint())
-            self.list_var.addItem(item)
-            self.list_var.setItemWidget(item, var_item)
-            self.dict_var[name] = item
+            self.env_box.list_var.addItem(item)
+            self.env_box.list_var.setItemWidget(item, var_item)
+            self.env_box.dict_var[name] = item
 
-        self.list_obj.clear()
+        self.env_box.list_obj.clear()
         for obj in configs['observations']:
-            item = QListWidgetItem(self.list_obj)
+            item = QListWidgetItem(self.env_box.list_obj)
             obj_item = objective_item(obj, 0, self.toggle_obj)
             item.setSizeHint(obj_item.sizeHint())
-            self.list_obj.addItem(item)
-            self.list_obj.setItemWidget(item, obj_item)
-            self.dict_obj[obj] = item
-
-        self.list_con.clear()
+            self.env_box.list_obj.addItem(item)
+            self.env_box.list_obj.setItemWidget(item, obj_item)
+            self.env_box.dict_obj[obj] = item
+
+        self.env_box.list_con.clear()
+        self.env_box.list_sta.clear()
+        self.env_box.fit_content()
         self.routine = None
 
     def open_playground(self):
         pass
 
     def check_all_var(self):
-        for i in range(self.list_var.count()):
-            item = self.list_var.item(i)
-            item_widget = self.list_var.itemWidget(item)
+        for i in range(self.env_box.list_var.count()):
+            item = self.env_box.list_var.item(i)
+            item_widget = self.env_box.list_var.itemWidget(item)
             item_widget.check_name.setChecked(True)
 
     def uncheck_all_var(self):
-        for i in range(self.list_var.count()):
-            item = self.list_var.item(i)
-            item_widget = self.list_var.itemWidget(item)
+        for i in range(self.env_box.list_var.count()):
+            item = self.env_box.list_var.item(i)
+            item_widget = self.env_box.list_var.itemWidget(item)
             item_widget.check_name.setChecked(False)
 
     def add_var(self):
         # TODO: Use a cached env
-        env_params = load_config(self.edit_env.toPlainText())
+        env_params = load_config(self.env_box.edit.toPlainText())
         try:
             intf_name = self.configs['interface'][0]
         except KeyError:
             intf_name = None
         configs = {
             'params': env_params,
             'interface': [intf_name]
@@ -480,255 +472,309 @@
         dlg = BadgerVariableDialog(self, self.env, configs, self.add_var_to_list)
         dlg.exec()
 
     def add_var_to_list(self, name, min, max):
         # Check if already in the list
         ok = False
         try:
-            self.dict_var[name]
+            self.env_box.dict_var[name]
         except:
             ok = True
 
         if not ok:
             QMessageBox.warning(self, 'Variable already exists!', f'Variable {name} already exists!')
             return 1
 
-        item = QListWidgetItem(self.list_var)
+        item = QListWidgetItem(self.env_box.list_var)
         var_item = variable_item(name, [min, max], self.toggle_var)
         var_item.check_name.setChecked(True)
         item.setSizeHint(var_item.sizeHint())
-        self.list_var.addItem(item)
-        self.list_var.setItemWidget(item, var_item)
-        self.dict_var[name] = item
+        self.env_box.list_var.addItem(item)
+        self.env_box.list_var.setItemWidget(item, var_item)
+        self.env_box.dict_var[name] = item
+        self.env_box.fit_content()
 
         return 0
 
     def check_all_obj(self):
-        for i in range(self.list_obj.count()):
-            item = self.list_obj.item(i)
-            item_widget = self.list_obj.itemWidget(item)
+        for i in range(self.env_box.list_obj.count()):
+            item = self.env_box.list_obj.item(i)
+            item_widget = self.env_box.list_obj.itemWidget(item)
             item_widget.check_name.setChecked(True)
 
     def uncheck_all_obj(self):
-        for i in range(self.list_obj.count()):
-            item = self.list_obj.item(i)
-            item_widget = self.list_obj.itemWidget(item)
+        for i in range(self.env_box.list_obj.count()):
+            item = self.env_box.list_obj.item(i)
+            item_widget = self.env_box.list_obj.itemWidget(item)
             item_widget.check_name.setChecked(False)
 
     def toggle_check_only_var(self):
-        if self.check_only_var.isChecked():
-            for i in range(self.list_var.count()):
-                item = self.list_var.item(i)
-                item_widget = self.list_var.itemWidget(item)
+        if self.env_box.check_only_var.isChecked():
+            for i in range(self.env_box.list_var.count()):
+                item = self.env_box.list_var.item(i)
+                item_widget = self.env_box.list_var.itemWidget(item)
                 if not item_widget.check_name.isChecked():
                     item_widget.hide()
                     item.setSizeHint(QSize(0, 0))
         else:
-            for i in range(self.list_var.count()):
-                item = self.list_var.item(i)
-                item_widget = self.list_var.itemWidget(item)
+            for i in range(self.env_box.list_var.count()):
+                item = self.env_box.list_var.item(i)
+                item_widget = self.env_box.list_var.itemWidget(item)
                 item_widget.show()
                 item.setSizeHint(item_widget.sizeHint())
+        self.env_box.fit_content()
 
     def toggle_var(self, name):
-        if self.check_only_var.isChecked():
-            item = self.dict_var[name]
-            item_widget = self.list_var.itemWidget(item)
+        if self.env_box.check_only_var.isChecked():
+            item = self.env_box.dict_var[name]
+            item_widget = self.env_box.list_var.itemWidget(item)
             if item_widget.check_name.isChecked():
                 item_widget.show()
                 item.setSizeHint(item_widget.sizeHint())
             else:
                 item_widget.hide()
                 item.setSizeHint(QSize(0, 0))
+            self.env_box.fit_content()
 
     def toggle_check_only_obj(self):
-        if self.check_only_obj.isChecked():
-            for i in range(self.list_obj.count()):
-                item = self.list_obj.item(i)
-                item_widget = self.list_obj.itemWidget(item)
+        if self.env_box.check_only_obj.isChecked():
+            for i in range(self.env_box.list_obj.count()):
+                item = self.env_box.list_obj.item(i)
+                item_widget = self.env_box.list_obj.itemWidget(item)
                 if not item_widget.check_name.isChecked():
                     item_widget.hide()
                     item.setSizeHint(QSize(0, 0))
         else:
-            for i in range(self.list_obj.count()):
-                item = self.list_obj.item(i)
-                item_widget = self.list_obj.itemWidget(item)
+            for i in range(self.env_box.list_obj.count()):
+                item = self.env_box.list_obj.item(i)
+                item_widget = self.env_box.list_obj.itemWidget(item)
                 item_widget.show()
                 item.setSizeHint(item_widget.sizeHint())
+        self.env_box.fit_content()
 
     def toggle_obj(self, name):
-        if self.check_only_obj.isChecked():
-            item = self.dict_obj[name]
-            item_widget = self.list_obj.itemWidget(item)
+        if self.env_box.check_only_obj.isChecked():
+            item = self.env_box.dict_obj[name]
+            item_widget = self.env_box.list_obj.itemWidget(item)
             if item_widget.check_name.isChecked():
                 item_widget.show()
                 item.setSizeHint(item_widget.sizeHint())
             else:
                 item_widget.hide()
                 item.setSizeHint(QSize(0, 0))
-
-    def toggle_save(self):
-        if self.check_save.isChecked():
-            self.edit_save.setDisabled(False)
-        else:
-            self.edit_save.setDisabled(True)
+            self.env_box.fit_content()
 
     def add_constraint(self, name=None, relation=0, threshold=0, critical=False):
         if self.configs is None:
             return
 
         options = self.configs['observations']
-        item = QListWidgetItem(self.list_con)
+        item = QListWidgetItem(self.env_box.list_con)
         con_item = constraint_item(options,
-                                   lambda: self.list_con.takeItem(
-                                       self.list_con.row(item)),
+                                   lambda: self.env_box.list_con.takeItem(
+                                       self.env_box.list_con.row(item)),
                                    name, relation, threshold, critical)
         item.setSizeHint(con_item.sizeHint())
-        self.list_con.addItem(item)
-        self.list_con.setItemWidget(item, con_item)
-        # self.dict_con[''] = item
+        self.env_box.list_con.addItem(item)
+        self.env_box.list_con.setItemWidget(item, con_item)
+        # self.env_box.dict_con[''] = item
+        self.env_box.fit_content()
 
-    def _compose_routine(self):
-        # Compose the routine
-        name = self.edit_save.text() or self.edit_save.placeholderText()
-        algo = self.cb_algo.currentText()
-        env = self.cb_env.currentText()
-        algo_params = load_config(self.edit_algo.toPlainText())
-        env_params = load_config(self.edit_env.toPlainText())
+    def add_state(self, name=None):
+        if self.configs is None:
+            return
+
+        var_names = [next(iter(d)) for d in self.configs['variables']]
+        options = self.configs['observations'] + var_names
+        item = QListWidgetItem(self.env_box.list_sta)
+        sta_item = state_item(options,
+                              lambda: self.env_box.list_sta.takeItem(
+                                  self.env_box.list_sta.row(item)), name)
+        item.setSizeHint(sta_item.sizeHint())
+        self.env_box.list_sta.addItem(item)
+        self.env_box.list_sta.setItemWidget(item, sta_item)
+        self.env_box.fit_content()
 
+    def _compose_vocs(self):
+        # Compose the VOCS settings
         variables = []
-        for i in range(self.list_var.count()):
-            item = self.list_var.item(i)
-            item_widget = self.list_var.itemWidget(item)
+        for i in range(self.env_box.list_var.count()):
+            item = self.env_box.list_var.item(i)
+            item_widget = self.env_box.list_var.itemWidget(item)
             if item_widget.check_name.isChecked():
                 var_name = item_widget.check_name.text()
                 lb = item_widget.sb_lower.sb.value()
                 ub = item_widget.sb_upper.sb.value()
                 _dict = {}
                 _dict[var_name] = [lb, ub]
                 variables.append(_dict)
 
         objectives = []
-        for i in range(self.list_obj.count()):
-            item = self.list_obj.item(i)
-            item_widget = self.list_obj.itemWidget(item)
+        for i in range(self.env_box.list_obj.count()):
+            item = self.env_box.list_obj.item(i)
+            item_widget = self.env_box.list_obj.itemWidget(item)
             if item_widget.check_name.isChecked():
                 obj_name = item_widget.check_name.text()
                 rule = item_widget.cb_rule.currentText()
                 _dict = {}
                 _dict[obj_name] = rule
                 objectives.append(_dict)
 
         constraints = []
-        for i in range(self.list_con.count()):
-            item = self.list_con.item(i)
-            item_widget = self.list_con.itemWidget(item)
+        for i in range(self.env_box.list_con.count()):
+            item = self.env_box.list_con.item(i)
+            item_widget = self.env_box.list_con.itemWidget(item)
             critical = item_widget.check_crit.isChecked()
             con_name = item_widget.cb_obs.currentText()
             relation = CONS_RELATION_DICT[item_widget.cb_rel.currentText()]
             value = item_widget.sb.value()
             _dict = {}
             _dict[con_name] = [relation, value]
             if critical:
                 _dict[con_name].append('CRITICAL')
             constraints.append(_dict)
 
-        configs = {
+        states = []
+        for i in range(self.env_box.list_sta.count()):
+            item = self.env_box.list_sta.item(i)
+            item_widget = self.env_box.list_sta.itemWidget(item)
+            sta_name = item_widget.cb_sta.currentText()
+            states.append(sta_name)
+
+        vocs = {
             'variables': variables,
             'objectives': objectives,
             'constraints': constraints,
-        }
-        if self.check_use_script.isChecked():
-            configs['script'] = self.script
-
-        routine = {
-            'name': name,
-            'algo': algo,
-            'env': env,
-            'algo_params': algo_params,
-            'env_params': env_params,
-            'env_vranges': config_list_to_dict(variables),
-            'config': configs,
+            'states': states,
         }
 
-        # Sanity check and config normalization
-        try:
-            routine = normalize_routine(routine)
-        except Exception as e:
-            raise e
+        return vocs
 
-        return routine
+    def _compose_routine(self):
+        # Compose the routine
+        name = self.edit_save.text() or self.edit_save.placeholderText()
+        algo = self.algo_box.cb.currentText()
+        assert algo, 'Please specify algorithm'
+        env = self.env_box.cb.currentText()
+        assert env, 'Please specify environment'
+        algo_params = load_config(self.algo_box.edit.toPlainText())
+        env_params = load_config(self.env_box.edit.toPlainText())
 
-    def _compose_vocs(self):
-        # Compose the VOCS settings
         variables = []
-        for i in range(self.list_var.count()):
-            item = self.list_var.item(i)
-            item_widget = self.list_var.itemWidget(item)
+        for i in range(self.env_box.list_var.count()):
+            item = self.env_box.list_var.item(i)
+            item_widget = self.env_box.list_var.itemWidget(item)
             if item_widget.check_name.isChecked():
                 var_name = item_widget.check_name.text()
                 lb = item_widget.sb_lower.sb.value()
                 ub = item_widget.sb_upper.sb.value()
                 _dict = {}
                 _dict[var_name] = [lb, ub]
                 variables.append(_dict)
 
         objectives = []
-        for i in range(self.list_obj.count()):
-            item = self.list_obj.item(i)
-            item_widget = self.list_obj.itemWidget(item)
+        for i in range(self.env_box.list_obj.count()):
+            item = self.env_box.list_obj.item(i)
+            item_widget = self.env_box.list_obj.itemWidget(item)
             if item_widget.check_name.isChecked():
                 obj_name = item_widget.check_name.text()
                 rule = item_widget.cb_rule.currentText()
                 _dict = {}
                 _dict[obj_name] = rule
                 objectives.append(_dict)
 
         constraints = []
-        for i in range(self.list_con.count()):
-            item = self.list_con.item(i)
-            item_widget = self.list_con.itemWidget(item)
+        for i in range(self.env_box.list_con.count()):
+            item = self.env_box.list_con.item(i)
+            item_widget = self.env_box.list_con.itemWidget(item)
             critical = item_widget.check_crit.isChecked()
             con_name = item_widget.cb_obs.currentText()
             relation = CONS_RELATION_DICT[item_widget.cb_rel.currentText()]
             value = item_widget.sb.value()
             _dict = {}
             _dict[con_name] = [relation, value]
             if critical:
                 _dict[con_name].append('CRITICAL')
             constraints.append(_dict)
 
-        vocs = {
+        states = []
+        for i in range(self.env_box.list_sta.count()):
+            item = self.env_box.list_sta.item(i)
+            item_widget = self.env_box.list_sta.itemWidget(item)
+            sta_name = item_widget.cb_sta.currentText()
+            states.append(sta_name)
+
+        # Domain scaling
+        try:
+            scaling = self.algo_box.cb_scaling.currentText()
+            scaling_params = load_config(self.algo_box.edit_scaling.toPlainText())
+            domain_scaling = {'func': scaling, **scaling_params}
+        except:
+            domain_scaling = None
+
+        # Tags
+        tag_obj = self.cb_obj.currentText()
+        tag_reg = self.cb_reg.currentText()
+        tag_gain = self.cb_gain.currentText()
+        tags = {}
+        if tag_obj: tags['objective'] = tag_obj
+        if tag_reg: tags['region'] = tag_reg
+        if tag_gain: tags['gain'] = tag_gain
+        if not tags: tags = None
+
+        configs = {
             'variables': variables,
             'objectives': objectives,
             'constraints': constraints,
+            'states': states,
+            'domain_scaling': domain_scaling,
+            'tags': tags,
         }
+        if self.algo_box.check_use_script.isChecked():
+            configs['script'] = self.script
 
-        return vocs
+        routine = {
+            'name': name,
+            'algo': algo,
+            'env': env,
+            'algo_params': algo_params,
+            'env_params': env_params,
+            'env_vranges': config_list_to_dict(variables),
+            'config': configs,
+        }
+
+        # Sanity check and config normalization
+        try:
+            routine = normalize_routine(routine)
+        except Exception as e:
+            raise e
+
+        return routine
 
     def review(self):
         try:
             routine = self._compose_routine()
         except Exception as e:
             return QMessageBox.critical(self, 'Error!', str(e))
 
         dlg = BadgerReviewDialog(self, routine)
         dlg.exec()
 
-    def run_routine(self, routine, save):
-        self.monitor = BadgerOptMonitor(self, routine, save)
-        self.monitor.show()
-        self.monitor.start()
-
-    def run(self):
+    def save(self):
         try:
             routine = self._compose_routine()
         except Exception as e:
             return QMessageBox.critical(self, 'Error!', str(e))
 
-        save = self.check_save.isChecked()
-
         try:
-            self.run_routine(routine, save)
-        except Exception as e:
-            # raise e
-            QMessageBox.critical(self, 'Error!', str(e))
+            save_routine(routine)
+        except sqlite3.IntegrityError:
+            return QMessageBox.critical(self, 'Error!',
+                f'Routine {routine["name"]} already existed in the database! Please choose another name.')
+
+        return 0
+
+    def delete(self):
+        name = self.edit_save.text() or self.edit_save.placeholderText()
+        remove_routine(name)
+
+        return 0
```

### Comparing `badger-opt-0.9.1/src/badger/gui/windows/edit_script_dialog.py` & `badger-opt-0.9.2/src/badger/gui/default/windows/edit_script_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui/windows/main_window.py` & `badger-opt-0.9.2/src/badger/gui/default/components/routine_editor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,100 @@
-from pkg_resources import get_distribution
-from PyQt5.QtWidgets import QMainWindow, QMessageBox, QStackedWidget, QDesktopWidget
-# from PyQt5.QtWidgets import QMenuBar, QMenu
-from ..pages.home_page import BadgerHomePage
-from ..pages.routine_page import BadgerRoutinePage
-from ..pages.run_page import BadgerRunPage
+from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QWidget, QPushButton
+from PyQt5.QtWidgets import QTextEdit, QStackedWidget, QScrollArea
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtGui import QFont
+from .routine_page import BadgerRoutinePage
+from ....utils import ystring
 
 
-class BadgerMainWindow(QMainWindow):
+class BadgerRoutineEditor(QWidget):
+    sig_saved = pyqtSignal()
+    sig_canceled = pyqtSignal()
+    sig_deleted = pyqtSignal()
+
     def __init__(self):
         super().__init__()
 
         self.init_ui()
         self.config_logic()
 
     def init_ui(self):
-        version = get_distribution('badger-opt').version
-        self.setWindowTitle(f'Badger v{version}')
-        self.resize(960, 720)
-        self.center()
-
-        # Add menu bar
-        # menu_bar = self.menuBar()
-        # edit_menu = menu_bar.addMenu('Edit')
-        # edit_menu.addAction('New')
-
-        # Add pages
-        self.home_page = BadgerHomePage(self.show_routine_page, self.show_run_page)
-        self.routine_page = BadgerRoutinePage(self.show_home_page)
-        self.run_page = BadgerRunPage(self.show_routine_page, self.show_home_page)
-
-        self.stacks = stacks = QStackedWidget()
-        stacks.addWidget(self.home_page)
-        stacks.addWidget(self.routine_page)
-        stacks.addWidget(self.run_page)
+        vbox = QVBoxLayout(self)
+        vbox.setContentsMargins(0, 0, 0, 0)
 
-        stacks.setCurrentIndex(0)
+        # self.seperator = seperator = QFrame()
+        # seperator.setFrameShape(QFrame.HLine)
+        # seperator.setFrameShadow(QFrame.Sunken)
+        # seperator.setLineWidth(0)
+        # seperator.setMidLineWidth(0)
+        # vbox.addWidget(seperator)
 
-        self.setCentralWidget(self.stacks)
-
-    def center(self):
-        qr = self.frameGeometry()
-        cp = QDesktopWidget().availableGeometry().center()
+        # Routine stacks
+        self.stacks = stacks = QStackedWidget()
 
-        qr.moveCenter(cp)
-        self.move(qr.topLeft())
+        self.routine_edit = routine_edit = QTextEdit()
+        routine_edit.setReadOnly(True)
+        stacks.addWidget(routine_edit)
+
+        self.scroll_area = scroll_area = QScrollArea()
+        self.routine_page = routine_page = BadgerRoutinePage()
+        scroll_area.setWidgetResizable(True)
+        scroll_area.setWidget(routine_page)
+        stacks.addWidget(scroll_area)
+
+        stacks.setCurrentIndex(1)
+        vbox.addWidget(stacks)
+
+        # Action bar
+        self.action_bar = action_bar = QWidget()
+        # action_bar.hide()
+        hbox_action = QHBoxLayout(action_bar)
+        hbox_action.setContentsMargins(8, 0, 8, 0)
+
+        cool_font = QFont()
+        cool_font.setWeight(QFont.DemiBold)
+        # cool_font.setPixelSize(16)
+
+        # Only show when create new routine
+        self.btn_cancel = btn_cancel = QPushButton('Cancel')
+        btn_cancel.setFixedSize(64, 32)
+        btn_cancel.setFont(cool_font)
+        btn_cancel.hide()
+
+        self.btn_save = btn_save = QPushButton('Save')
+        btn_save.setFixedSize(128, 32)
+        btn_save.setFont(cool_font)
+        hbox_action.addWidget(btn_cancel)
+        hbox_action.addStretch(1)
+        hbox_action.addWidget(btn_save)
+        vbox.addWidget(action_bar)
 
     def config_logic(self):
-        pass
+        self.btn_cancel.clicked.connect(self.cancel_create_routine)
+        self.btn_save.clicked.connect(self.save_routine)
 
-    def show_routine_page(self, routine=None):
-        try:
-            self.routine_page.refresh_ui(routine)
-        except Exception as e:
-            return QMessageBox.critical(self, 'Error!', str(e))
+    def set_routine(self, routine):
+        self.routine_edit.setText(ystring(routine))
+        self.routine_page.refresh_ui(routine)
 
+    def edit_routine(self):
         self.stacks.setCurrentIndex(1)
 
-    def show_home_page(self):
-        self.routine_page.refresh_ui(None)  # clean up to prevent bugs
-        self.home_page.refresh_ui()
-        self.home_page.reconfig_logic()
-        self.stacks.setCurrentIndex(0)
-
-    def show_run_page(self):
-        try:
-            self.run_page.refresh_ui()
-            self.run_page.reconfig_logic()
-        except Exception as e:
-            return QMessageBox.critical(self, 'Error!', str(e))
-
-        self.stacks.setCurrentIndex(2)
+    def del_routine(self):
+        if self.routine_page.delete() == 0:
+            self.sig_deleted.emit()
+
+    def cancel_create_routine(self):
+        self.sig_canceled.emit()
+
+    def save_routine(self):
+        if self.routine_page.save() == 0:
+            self.sig_saved.emit()
+
+    def clear(self):
+        self.routine_edit.clear()
+
+    def switch_mode(self, mode):
+        if mode == 'regular':
+            self.btn_cancel.hide()
+        elif mode == 'new routine':
+            self.btn_cancel.show()
```

### Comparing `badger-opt-0.9.1/src/badger/gui/windows/review_dialog.py` & `badger-opt-0.9.2/src/badger/gui/default/windows/review_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PyQt5.QtWidgets import QDialog, QDialogButtonBox, QTextBrowser, QVBoxLayout
-from ...utils import ystring
+from ....utils import ystring
 
 
 class BadgerReviewDialog(QDialog):
     def __init__(self, parent, routine):
         super().__init__(parent)
 
         self.routine = routine
```

### Comparing `badger-opt-0.9.1/src/badger/gui/windows/var_dialog.py` & `badger-opt-0.9.2/src/badger/gui/default/windows/var_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt5.QtWidgets import QDialog, QWidget, QHBoxLayout, QLineEdit, QPushButton, QVBoxLayout
 from PyQt5.QtWidgets import QGroupBox, QMessageBox
 from ..components.labeled_lineedit import labeled_lineedit
-from ...core import instantiate_env
+from ....core import instantiate_env
 
 
 class BadgerVariableDialog(QDialog):
     def __init__(self, parent, env_class, configs, callback):
         super().__init__(parent)
 
         self.env = instantiate_env(env_class, configs)
```

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/algo_cbox.py` & `badger-opt-0.9.2/src/badger/gui/default/components/algo_cbox.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/collapsible_box.py` & `badger-opt-0.9.2/src/badger/gui/default/components/collapsible_box.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/data_table.py` & `badger-opt-0.9.2/src/badger/gui/default/components/data_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,9 +78,9 @@
     return table
 
 
 def data_table(data=None):
     table = TableWithCopy()
     table.setAlternatingRowColors(True)
     table.setStyleSheet('alternate-background-color: #262E38;')
-    table.horizontalHeader().setResizeMode(QHeaderView.Stretch)
+    table.horizontalHeader().setSectionResizeMode(QHeaderView.Stretch)
     return update_table(table, data)
```

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/env_cbox.py` & `badger-opt-0.9.2/src/badger/gui/default/components/env_cbox.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/filter_cbox.py` & `badger-opt-0.9.2/src/badger/gui/default/components/filter_cbox.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/history_navigator.py` & `badger-opt-0.9.2/src/badger/gui/default/components/history_navigator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt5.QtWidgets import QComboBox, QTreeWidget, QTreeWidgetItem
 from PyQt5.QtCore import QModelIndex, Qt
-from ...utils import run_names_to_dict
+from ....utils import run_names_to_dict
 
 
 # Modified based on the following solution
 # https://stackoverflow.com/a/9672359/4263605
 class HistoryNavigator(QComboBox):
     def __init__(self):
         super().__init__()
```

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/objective_item.py` & `badger-opt-0.9.2/src/badger/gui/default/components/variable_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from PyQt5.QtWidgets import QHBoxLayout, QWidget, QCheckBox, QLabel
-from PyQt5.QtWidgets import QComboBox, QStyledItemDelegate
+from PyQt5.QtWidgets import QHBoxLayout, QWidget, QCheckBox
+from .labeled_spinbox import labeled_spinbox
 
 
-def objective_item(name, rule, callback=None):
-    # rule: 0 for MINIMIZE, 1 for MAXIMIZE
+def variable_item(name, vrange, callback=None):
     widget = QWidget()
     hbox = QHBoxLayout(widget)
     hbox.setContentsMargins(2, 2, 2, 2)
     widget.check_name = check_name = QCheckBox(name)
     check_name.setFixedWidth(200)
     check_name.setChecked(True)
     hbox.addWidget(check_name)
-    widget_rule = QWidget()
-    hbox.addWidget(widget_rule)
-    hbox_rule = QHBoxLayout(widget_rule)
-    hbox_rule.setContentsMargins(0, 0, 0, 0)
-    label = QLabel('rule')
-    widget.cb_rule = cb_rule = QComboBox()
-    cb_rule.setItemDelegate(QStyledItemDelegate())
-    cb_rule.addItems(['MINIMIZE', 'MAXIMIZE'])
-    cb_rule.setCurrentIndex(rule)
-    hbox_rule.addWidget(label)
-    hbox_rule.addWidget(cb_rule, 1)
+    # hbox.addSpacing(8)
+    widget_range = QWidget()
+    hbox.addWidget(widget_range)
+    hbox_range = QHBoxLayout(widget_range)
+    hbox_range.setContentsMargins(0, 0, 0, 0)
+    widget.sb_lower = sb_lower = labeled_spinbox('min', vrange[0], vrange[0], vrange[1])
+    widget.sb_upper = sb_upper = labeled_spinbox('max', vrange[1], vrange[0], vrange[1])
+    hbox_range.addWidget(sb_lower, 1)
+    hbox_range.addWidget(sb_upper, 1)
 
     def toggle_item():
-        widget_rule.setDisabled(not check_name.isChecked())
+        widget_range.setDisabled(not check_name.isChecked())
         if callback is not None:
             callback(name)
 
     check_name.stateChanged.connect(toggle_item)
 
     return widget
```

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/routine_item.py` & `badger-opt-0.9.2/src/badger/gui/default/components/routine_item.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/run_monitor.py` & `badger-opt-0.9.2/src/badger/gui/default/components/run_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QWidget, QPushButton, QCheckBox
 from PyQt5.QtWidgets import QMessageBox, QComboBox, QLabel, QStyledItemDelegate
 from PyQt5.QtCore import pyqtSignal, QThreadPool
 from PyQt5.QtGui import QFont
 import pyqtgraph as pg
 from .routine_runner import BadgerRoutineRunner
 # from ...utils import AURORA_PALETTE, FROST_PALETTE
-from ...utils import norm, ParetoFront
-from ...logbook import send_to_logbook, BADGER_LOGBOOK_ROOT
-from ...archive import archive_run, BADGER_ARCHIVE_ROOT
+from ....utils import norm, ParetoFront
+from ....logbook import send_to_logbook, BADGER_LOGBOOK_ROOT
+from ....archive import archive_run, BADGER_ARCHIVE_ROOT
 
 
 stylesheet_del = '''
 QPushButton:hover:pressed
 {
     background-color: #C7737B;
 }
```

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/state_item.py` & `badger-opt-0.9.2/src/badger/gui/default/components/state_item.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/components/status_bar.py` & `badger-opt-0.9.2/src/badger/gui/default/components/status_bar.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/images/gear.png` & `badger-opt-0.9.2/src/badger/gui/default/images/gear.png`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/pages/home_page.py` & `badger-opt-0.9.2/src/badger/gui/default/pages/home_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from ..components.data_table import data_table, update_table, reset_table, add_row
 from ..components.routine_item import BadgerRoutineItem
 from ..components.history_navigator import HistoryNavigator
 from ..components.run_monitor import BadgerOptMonitor
 from ..components.routine_editor import BadgerRoutineEditor
 from ..components.status_bar import BadgerStatusBar
 from ..components.filter_cbox import BadgerFilterBox
-from ...db import list_routine, load_routine, remove_routine, get_runs_by_routine, get_runs
-from ...archive import load_run, delete_run
-from ...utils import get_header
+from ....db import list_routine, load_routine, remove_routine, get_runs_by_routine, get_runs
+from ....archive import load_run, delete_run
+from ....utils import get_header
 
 
 stylesheet = '''
 QPushButton:hover:pressed
 {
     background-color: #C7737B;
 }
```

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/utils.py` & `badger-opt-0.9.2/src/badger/gui/default/utils.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/windows/main_window.py` & `badger-opt-0.9.2/src/badger/gui/default/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/gui_acr/windows/settings_dialog.py` & `badger-opt-0.9.2/src/badger/gui/default/windows/settings_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQt5.QtCore import QRegExp
 from PyQt5.QtGui import QRegExpValidator
 from PyQt5.QtWidgets import QComboBox, QGridLayout, QVBoxLayout, QWidget, QLabel, QLineEdit
 from PyQt5.QtWidgets import QDialog, QDialogButtonBox, QApplication, QStyledItemDelegate
 from qdarkstyle import load_stylesheet, DarkPalette, LightPalette
-from ...settings import list_settings, read_value, write_value
+from ....settings import list_settings, read_value, write_value
 
 
 class BadgerSettingsDialog(QDialog):
     theme_list = ['default', 'light', 'dark']
     theme_idx_dict = {
         'default': 0,
         'light': 1,
```

### Comparing `badger-opt-0.9.1/src/badger/interface.py` & `badger-opt-0.9.2/src/badger/interface.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/log.py` & `badger-opt-0.9.2/src/badger/log.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/logbook.py` & `badger-opt-0.9.2/src/badger/logbook.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/logger/__init__.py` & `badger-opt-0.9.2/src/badger/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/logger/observer.py` & `badger-opt-0.9.2/src/badger/logger/observer.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/logger/util.py` & `badger-opt-0.9.2/src/badger/logger/util.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/settings.py` & `badger-opt-0.9.2/src/badger/settings.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/stats.py` & `badger-opt-0.9.2/src/badger/stats.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/tests/conftest.py` & `badger-opt-0.9.2/src/badger/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/tests/mock/plugins/algorithms/simplex/__init__.py` & `badger-opt-0.9.2/src/badger/tests/mock/plugins/algorithms/simplex/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/tests/mock/plugins/environments/silly/__init__.py` & `badger-opt-0.9.2/src/badger/tests/mock/plugins/environments/silly/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/tests/mock/plugins/interfaces/silly/__init__.py` & `badger-opt-0.9.2/src/badger/tests/mock/plugins/interfaces/silly/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/tests/test_cli_basic.py` & `badger-opt-0.9.2/src/badger/tests/test_cli_basic.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/tests/test_lib_basic.py` & `badger-opt-0.9.2/src/badger/tests/test_lib_basic.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger/utils.py` & `badger-opt-0.9.2/src/badger/utils.py`

 * *Files identical despite different names*

### Comparing `badger-opt-0.9.1/src/badger_opt.egg-info/SOURCES.txt` & `badger-opt-0.9.2/src/badger_opt.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -26,69 +26,47 @@
 src/badger/actions/env.py
 src/badger/actions/install.py
 src/badger/actions/intf.py
 src/badger/actions/routine.py
 src/badger/actions/run.py
 src/badger/actions/uninstall.py
 src/badger/gui/__init__.py
-src/badger/gui/utils.py
-src/badger/gui/components/__init__.py
-src/badger/gui/components/constraint_item.py
-src/badger/gui/components/labeled_lineedit.py
-src/badger/gui/components/labeled_spinbox.py
-src/badger/gui/components/objective_item.py
-src/badger/gui/components/routine_runner.py
-src/badger/gui/components/search_bar.py
-src/badger/gui/components/syntax.py
-src/badger/gui/components/variable_item.py
-src/badger/gui/images/icon.png
-src/badger/gui/pages/__init__.py
-src/badger/gui/pages/home_page.py
-src/badger/gui/pages/routine_page.py
-src/badger/gui/pages/run_page.py
-src/badger/gui/windows/__init__.py
-src/badger/gui/windows/edit_script_dialog.py
-src/badger/gui/windows/main_window.py
-src/badger/gui/windows/opt_monitor.py
-src/badger/gui/windows/review_dialog.py
-src/badger/gui/windows/settings_dialog.py
-src/badger/gui/windows/var_dialog.py
-src/badger/gui_acr/__init__.py
-src/badger/gui_acr/utils.py
-src/badger/gui_acr/components/__init__.py
-src/badger/gui_acr/components/algo_cbox.py
-src/badger/gui_acr/components/collapsible_box.py
-src/badger/gui_acr/components/constraint_item.py
-src/badger/gui_acr/components/data_table.py
-src/badger/gui_acr/components/env_cbox.py
-src/badger/gui_acr/components/filter_cbox.py
-src/badger/gui_acr/components/history_navigator.py
-src/badger/gui_acr/components/labeled_lineedit.py
-src/badger/gui_acr/components/labeled_spinbox.py
-src/badger/gui_acr/components/objective_item.py
-src/badger/gui_acr/components/routine_editor.py
-src/badger/gui_acr/components/routine_item.py
-src/badger/gui_acr/components/routine_page.py
-src/badger/gui_acr/components/routine_runner.py
-src/badger/gui_acr/components/run_monitor.py
-src/badger/gui_acr/components/search_bar.py
-src/badger/gui_acr/components/state_item.py
-src/badger/gui_acr/components/status_bar.py
-src/badger/gui_acr/components/syntax.py
-src/badger/gui_acr/components/variable_item.py
-src/badger/gui_acr/images/gear.png
-src/badger/gui_acr/images/icon.png
-src/badger/gui_acr/pages/__init__.py
-src/badger/gui_acr/pages/home_page.py
-src/badger/gui_acr/windows/__init__.py
-src/badger/gui_acr/windows/edit_script_dialog.py
-src/badger/gui_acr/windows/main_window.py
-src/badger/gui_acr/windows/review_dialog.py
-src/badger/gui_acr/windows/settings_dialog.py
-src/badger/gui_acr/windows/var_dialog.py
+src/badger/gui/default/__init__.py
+src/badger/gui/default/utils.py
+src/badger/gui/default/components/__init__.py
+src/badger/gui/default/components/algo_cbox.py
+src/badger/gui/default/components/collapsible_box.py
+src/badger/gui/default/components/constraint_item.py
+src/badger/gui/default/components/data_table.py
+src/badger/gui/default/components/env_cbox.py
+src/badger/gui/default/components/filter_cbox.py
+src/badger/gui/default/components/history_navigator.py
+src/badger/gui/default/components/labeled_lineedit.py
+src/badger/gui/default/components/labeled_spinbox.py
+src/badger/gui/default/components/objective_item.py
+src/badger/gui/default/components/routine_editor.py
+src/badger/gui/default/components/routine_item.py
+src/badger/gui/default/components/routine_page.py
+src/badger/gui/default/components/routine_runner.py
+src/badger/gui/default/components/run_monitor.py
+src/badger/gui/default/components/search_bar.py
+src/badger/gui/default/components/state_item.py
+src/badger/gui/default/components/status_bar.py
+src/badger/gui/default/components/syntax.py
+src/badger/gui/default/components/variable_item.py
+src/badger/gui/default/images/gear.png
+src/badger/gui/default/images/icon.png
+src/badger/gui/default/pages/__init__.py
+src/badger/gui/default/pages/home_page.py
+src/badger/gui/default/windows/__init__.py
+src/badger/gui/default/windows/edit_script_dialog.py
+src/badger/gui/default/windows/main_window.py
+src/badger/gui/default/windows/review_dialog.py
+src/badger/gui/default/windows/settings_dialog.py
+src/badger/gui/default/windows/var_dialog.py
 src/badger/logger/__init__.py
 src/badger/logger/event.py
 src/badger/logger/observer.py
 src/badger/logger/util.py
 src/badger/tests/__init__.py
 src/badger/tests/conftest.py
 src/badger/tests/test_cli_basic.py
```

### Comparing `badger-opt-0.9.1/versioneer.py` & `badger-opt-0.9.2/versioneer.py`

 * *Files identical despite different names*

