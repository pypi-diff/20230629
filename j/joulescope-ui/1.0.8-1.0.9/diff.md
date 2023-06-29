# Comparing `tmp/joulescope_ui-1.0.8.tar.gz` & `tmp/joulescope_ui-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.0.8.tar", last modified: Thu Apr 13 20:58:46 2023, max compression
+gzip compressed data, was "joulescope_ui-1.0.9.tar", last modified: Wed Apr 19 20:45:42 2023, max compression
```

## Comparing `joulescope_ui-1.0.8.tar` & `joulescope_ui-1.0.9.tar`

### file list

```diff
@@ -1,282 +1,294 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.384179 joulescope_ui-1.0.8/
--rw-rw-rw-   0        0        0    37019 2023-04-13 20:54:02.000000 joulescope_ui-1.0.8/CHANGELOG.md
--rw-rw-rw-   0        0        0    13225 2023-04-04 17:19:13.000000 joulescope_ui-1.0.8/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 joulescope_ui-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      160 2023-03-10 02:18:44.000000 joulescope_ui-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6885 2023-04-13 20:58:46.384179 joulescope_ui-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5309 2023-03-10 14:30:22.000000 joulescope_ui-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.157685 joulescope_ui-1.0.8/joulescope_ui/
--rw-rw-rw-   0        0        0     2976 2023-03-29 15:40:51.000000 joulescope_ui-1.0.8/joulescope_ui/__init__.py
--rw-rw-rw-   0        0        0      902 2023-03-09 20:16:57.000000 joulescope_ui-1.0.8/joulescope_ui/__main__.py
--rw-rw-rw-   0        0        0     1886 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/about.py
--rw-rw-rw-   0        0        0     3935 2023-03-12 15:18:01.000000 joulescope_ui-1.0.8/joulescope_ui/api.py
--rw-rw-rw-   0        0        0     7197 2023-04-12 21:24:46.000000 joulescope_ui-1.0.8/joulescope_ui/app.py
--rw-rw-rw-   0        0        0     7516 2023-03-20 12:38:29.000000 joulescope_ui-1.0.8/joulescope_ui/capabilities.py
--rw-rw-rw-   0        0        0     6226 2023-03-29 15:41:11.000000 joulescope_ui-1.0.8/joulescope_ui/dev_signal_buffer_source.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.169204 joulescope_ui-1.0.8/joulescope_ui/devices/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/devices/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.171204 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/__init__.py
--rw-rw-rw-   0        0        0     3917 2023-03-19 13:46:25.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/device.py
--rw-rw-rw-   0        0        0    24570 2023-04-13 14:57:50.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js110.py
--rw-rw-rw-   0        0        0    28183 2023-04-13 14:57:31.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js220.py
--rw-rw-rw-   0        0        0    14980 2023-04-12 18:27:36.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-rw-rw-   0        0        0     7170 2023-03-17 12:14:59.000000 joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.177219 joulescope_ui-1.0.8/joulescope_ui/entry_points/
--rw-rw-rw-   0        0        0        0 2020-04-07 21:08:41.000000 joulescope_ui-1.0.8/joulescope_ui/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2318 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/entry_points/ui.py
--rw-rw-rw-   0        0        0     3168 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/error_window.py
--rw-rw-rw-   0        0        0     4917 2023-03-15 21:06:26.000000 joulescope_ui-1.0.8/joulescope_ui/expanding_widget.py
--rw-rw-rw-   0        0        0    11849 2023-03-31 21:30:44.000000 joulescope_ui-1.0.8/joulescope_ui/exporter.py
--rw-rw-rw-   0        0        0     3179 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.088346 joulescope_ui-1.0.8/joulescope_ui/fonts/
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.181226 joulescope_ui-1.0.8/joulescope_ui/fonts/DSEG14-Modern/
--rw-rw-rw-   0        0        0     4487 2020-03-14 16:24:02.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.190247 joulescope_ui-1.0.8/joulescope_ui/fonts/Hack/
--rw-rw-rw-   0        0        0     3744 2023-04-04 17:09:37.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/Hack/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.193250 joulescope_ui-1.0.8/joulescope_ui/fonts/Lato/
--rw-rw-rw-   0        0        0     4500 2010-12-15 04:00:00.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/Lato/OFL.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.197263 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceCodePro/
--rw-rw-rw-   0        0        0     4566 2023-04-04 17:17:39.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.201270 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceSerifPro/
--rw-rw-rw-   0        0        0     4615 2014-05-30 04:00:00.000000 joulescope_ui-1.0.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-rw-rw-   0        0        0  3411435 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui/fonts.rcc
--rw-rw-rw-   0        0        0     2642 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/getting_started.html
--rw-rw-rw-   0        0        0     4994 2023-03-18 21:45:09.000000 joulescope_ui-1.0.8/joulescope_ui/help_ui.py
--rw-rw-rw-   0        0        0     6488 2023-03-18 13:34:03.000000 joulescope_ui-1.0.8/joulescope_ui/jls_source.py
--rw-rw-rw-   0        0        0     9069 2023-03-29 15:41:27.000000 joulescope_ui-1.0.8/joulescope_ui/jls_v1.py
--rw-rw-rw-   0        0        0     8262 2023-03-29 22:24:39.000000 joulescope_ui-1.0.8/joulescope_ui/jls_v2.py
--rw-rw-rw-   0        0        0     3109 2023-03-20 14:51:40.000000 joulescope_ui-1.0.8/joulescope_ui/json.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.201769 joulescope_ui-1.0.8/joulescope_ui/locale/
--rw-rw-rw-   0        0        0      965 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/locale/__init__.py
--rw-rw-rw-   0        0        0     5629 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/logging_util.py
--rw-rw-rw-   0        0        0    25310 2023-04-13 20:24:51.000000 joulescope_ui-1.0.8/joulescope_ui/main.py
--rw-rw-rw-   0        0        0     2171 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/mem_leak_debugger.py
--rw-rw-rw-   0        0        0     9118 2023-03-18 18:14:25.000000 joulescope_ui-1.0.8/joulescope_ui/metadata.py
--rw-rw-rw-   0        0        0     5808 2023-04-12 17:49:24.000000 joulescope_ui-1.0.8/joulescope_ui/paths.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.208789 joulescope_ui-1.0.8/joulescope_ui/plugins/
--rw-rw-rw-   0        0        0      792 2023-03-20 13:23:46.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/__init__.py
--rw-rw-rw-   0        0        0     8662 2023-04-12 17:48:45.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/cdf.py
--rw-rw-rw-   0        0        0    10906 2023-04-12 17:49:28.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/frequency.py
--rw-rw-rw-   0        0        0     9174 2023-04-12 17:49:32.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/histogram.py
--rw-rw-rw-   0        0        0     6270 2023-03-29 15:41:27.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/max_window.py
--rw-rw-rw-   0        0        0     2219 2023-03-20 13:10:43.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/plugin_helpers.py
--rw-rw-rw-   0        0        0     4247 2023-03-13 18:49:46.000000 joulescope_ui-1.0.8/joulescope_ui/plugins/usb_inrush.py
--rw-rw-rw-   0        0        0     2130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/process_monitor.py
--rw-rw-rw-   0        0        0     1008 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/profile.py
--rw-rw-rw-   0        0        0    63957 2023-04-13 20:12:00.000000 joulescope_ui-1.0.8/joulescope_ui/pubsub.py
--rw-rw-rw-   0        0        0    12868 2023-03-19 18:14:07.000000 joulescope_ui-1.0.8/joulescope_ui/range_tool.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.211293 joulescope_ui-1.0.8/joulescope_ui/resources/
--rw-rw-rw-   0        0        0    11509 2019-07-27 15:33:28.000000 joulescope_ui-1.0.8/joulescope_ui/resources/dmg_background.svg
--rw-rw-rw-   0        0        0     3357 2020-11-05 22:48:01.000000 joulescope_ui-1.0.8/joulescope_ui/resources/icons.svg
--rw-rw-rw-   0        0        0    11282 2020-08-12 18:43:24.000000 joulescope_ui-1.0.8/joulescope_ui/resources/zoom.svg
--rw-rw-rw-   0        0        0     1989 2023-04-04 16:57:10.000000 joulescope_ui-1.0.8/joulescope_ui/resources.py
--rw-rw-rw-   0        0        0    22839 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui/resources.rcc
--rw-rw-rw-   0        0        0     1840 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/sanitize.py
--rw-rw-rw-   0        0        0     1304 2023-04-13 20:26:58.000000 joulescope_ui-1.0.8/joulescope_ui/shortcuts.py
--rw-rw-rw-   0        0        0    10890 2023-03-20 18:55:58.000000 joulescope_ui-1.0.8/joulescope_ui/software_update.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.233838 joulescope_ui-1.0.8/joulescope_ui/styles/
--rw-rw-rw-   0        0        0     3239 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/README.md
--rw-rw-rw-   0        0        0      834 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/__init__.py
--rw-rw-rw-   0        0        0     4354 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_editor.py
--rw-rw-rw-   0        0        0     4369 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_file.py
--rw-rw-rw-   0        0        0     6822 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_picker.py
--rw-rw-rw-   0        0        0      944 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme.py
--rw-rw-rw-   0        0        0     1383 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0     2346 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      778 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/font_scheme.py
--rw-rw-rw-   0        0        0       30 2023-03-31 19:50:28.000000 joulescope_ui-1.0.8/joulescope_ui/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0     3405 2023-04-04 16:50:03.000000 joulescope_ui-1.0.8/joulescope_ui/styles/fonts.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.250384 joulescope_ui-1.0.8/joulescope_ui/styles/js1/
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_down.svg
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_left.svg
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_right.svg
--rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/arrow_up.svg
--rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_closed.svg
--rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_end.svg
--rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_end_open.svg
--rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_more.svg
--rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_open.svg
--rw-rw-rw-   0        0        0       93 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/branch_vline.svg
--rw-rw-rw-   0        0        0      335 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-rw-rw-   0        0        0      499 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-rw-rw-   0        0        0      264 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-rw-rw-   0        0        0      234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/close.svg
--rw-rw-rw-   0        0        0     1907 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/detach.svg
--rw-rw-rw-   0        0        0      259 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-rw-rw-   0        0        0      191 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-rw-rw-   0        0        0     2382 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/index.json
--rw-rw-rw-   0        0        0      432 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/radio_checked.svg
--rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-rw-rw-   0        0        0      263 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/sizegrip.svg
--rw-rw-rw-   0        0        0      419 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/style.html
--rw-rw-rw-   0        0        0    19524 2023-04-04 14:57:41.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/style.qss
--rw-rw-rw-   0        0        0      526 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/tabs_menu.svg
--rw-rw-rw-   0        0        0       31 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/transparent.svg
--rw-rw-rw-   0        0        0      760 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-rw-rw-   0        0        0      653 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-rw-rw-   0        0        0    15079 2023-03-18 21:39:13.000000 joulescope_ui-1.0.8/joulescope_ui/styles/manager.py
--rw-rw-rw-   0        0        0     3635 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/parameter_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.274408 joulescope_ui-1.0.8/joulescope_ui/styles/system/
--rw-rw-rw-   0        0        0      350 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/index.json
--rw-rw-rw-   0        0        0       17 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/style.html
--rw-rw-rw-   0        0        0     3222 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/style.qss
--rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_all.svg
--rw-rw-rw-   0        0        0      481 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_in.svg
--rw-rw-rw-   0        0        0      393 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_out.svg
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.285919 joulescope_ui-1.0.8/joulescope_ui/styles/test/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/__init__.py
--rw-rw-rw-   0        0        0     2816 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/test_color_file.py
--rw-rw-rw-   0        0        0     2156 2023-03-18 18:42:17.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/test_manager.py
--rw-rw-rw-   0        0        0     1959 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/styles/test/test_parameter_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.315480 joulescope_ui-1.0.8/joulescope_ui/test/
--rw-rw-rw-   0        0        0        0 2018-04-10 21:33:42.000000 joulescope_ui-1.0.8/joulescope_ui/test/__init__.py
--rw-rw-rw-   0        0        0     1139 2023-03-10 14:49:52.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_capabilities.py
--rw-rw-rw-   0        0        0     6851 2023-04-12 17:49:35.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_metadata.py
--rw-rw-rw-   0        0        0    10861 2023-04-13 20:09:56.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub.py
--rw-rw-rw-   0        0        0    12814 2023-03-12 15:57:42.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub_registry.py
--rw-rw-rw-   0        0        0     5147 2023-03-16 16:02:02.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_range_tool.py
--rw-rw-rw-   0        0        0     2582 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_sanitize.py
--rw-rw-rw-   0        0        0     2034 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_software_update.py
--rw-rw-rw-   0        0        0     4055 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_time_map.py
--rw-rw-rw-   0        0        0     1601 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_tooltip.py
--rw-rw-rw-   0        0        0     5229 2023-04-12 21:57:44.000000 joulescope_ui-1.0.8/joulescope_ui/test/test_units.py
--rw-rw-rw-   0        0        0     3197 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/time_map.py
--rw-rw-rw-   0        0        0     2234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/tooltip.py
--rw-rw-rw-   0        0        0     7060 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/ui_util.py
--rw-rw-rw-   0        0        0     7261 2023-04-12 21:56:15.000000 joulescope_ui-1.0.8/joulescope_ui/units.py
--rw-rw-rw-   0        0        0       23 2023-04-04 19:20:04.000000 joulescope_ui-1.0.8/joulescope_ui/version.py
--rw-rw-rw-   0        0        0    12791 2023-04-13 12:57:34.000000 joulescope_ui-1.0.8/joulescope_ui/view.py
--rw-rw-rw-   0        0        0     1042 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widget_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.318493 joulescope_ui-1.0.8/joulescope_ui/widgets/
--rw-rw-rw-   0        0        0     1160 2023-04-12 20:18:29.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.320001 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/
--rw-rw-rw-   0        0        0      642 2023-04-12 20:02:06.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/__init__.py
--rw-rw-rw-   0        0        0     6954 2023-04-12 21:59:19.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/accumulator_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.330516 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/
--rw-rw-rw-   0        0        0      109 2023-04-12 20:03:25.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      109 2023-04-12 20:03:47.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0       37 2023-04-12 20:36:04.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/index.json
--rw-rw-rw-   0        0        0      762 2023-04-12 20:35:40.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.333017 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/
--rw-rw-rw-   0        0        0      647 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/__init__.py
--rw-rw-rw-   0        0        0     3177 2023-03-15 21:07:03.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-rw-rw-   0        0        0     3397 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-rw-rw-   0        0        0    20306 2023-04-12 17:47:44.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.337021 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/
--rw-rw-rw-   0        0        0      180 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-rw-rw-   0        0        0       78 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      216 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-rw-rw-   0        0        0     1936 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/index.json
--rw-rw-rw-   0        0        0     1749 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/info.svg
--rw-rw-rw-   0        0        0      125 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/open.svg
--rw-rw-rw-   0        0        0     4466 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/style.qss
--rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/target_power.svg
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.344052 joulescope_ui-1.0.8/joulescope_ui/widgets/example/
--rw-rw-rw-   0        0        0      639 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/__init__.py
--rw-rw-rw-   0        0        0     2100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/example_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.353611 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/
--rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0       80 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/index.json
--rw-rw-rw-   0        0        0      242 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/example/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.354611 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/
--rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/__init__.py
--rw-rw-rw-   0        0        0     4010 2023-03-17 14:48:42.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.356112 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/index.json
--rw-rw-rw-   0        0        0      692 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.357116 joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/
--rw-rw-rw-   0        0        0      638 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/__init__.py
--rw-rw-rw-   0        0        0     2164 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.358125 joulescope_ui-1.0.8/joulescope_ui/widgets/help/
--rw-rw-rw-   0        0        0      628 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/help/__init__.py
--rw-rw-rw-   0        0        0     2350 2023-03-10 14:01:14.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/help/help_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.358630 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/
--rw-rw-rw-   0        0        0      632 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/__init__.py
--rw-rw-rw-   0        0        0    10815 2023-04-12 19:57:12.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/memory_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.360633 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/
--rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/index.json
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/memory/styles/style.qss
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.361637 joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/
--rw-rw-rw-   0        0        0      643 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/__init__.py
--rw-rw-rw-   0        0        0     5816 2023-04-05 17:16:31.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.362137 joulescope_ui-1.0.8/joulescope_ui/widgets/settings/
--rw-rw-rw-   0        0        0      641 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/settings/__init__.py
--rw-rw-rw-   0        0        0    21759 2023-04-13 19:27:43.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/settings/settings_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.363137 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/
--rw-rw-rw-   0        0        0      633 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/__init__.py
--rw-rw-rw-   0        0        0     9819 2023-04-13 18:54:20.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.369645 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/
--rw-rw-rw-   0        0        0      575 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      216 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      358 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-rw-rw-   0        0        0     4413 2023-04-13 15:29:15.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/index.json
--rw-rw-rw-   0        0        0      421 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-rw-rw-   0        0        0      274 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/misc.svg
--rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-rw-rw-   0        0        0      241 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-rw-rw-   0        0        0      205 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-rw-rw-   0        0        0      511 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-rw-rw-   0        0        0     5528 2023-04-13 15:30:01.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-rw-rw-   0        0        0      207 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/target_power.svg
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.371148 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/
--rw-rw-rw-   0        0        0      699 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/__init__.py
--rw-rw-rw-   0        0        0     6727 2023-03-29 19:41:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record.py
--rw-rw-rw-   0        0        0     7983 2023-03-18 13:24:49.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.372652 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/
--rw-rw-rw-   0        0        0      715 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-03-18 13:36:54.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-rw-rw-   0        0        0     6501 2023-03-18 13:25:13.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-rw-rw-   0        0        0     6078 2023-01-24 22:12:47.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/switch.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.373652 joulescope_ui-1.0.8/joulescope_ui/widgets/value/
--rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.375652 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/
--rw-rw-rw-   0        0        0      152 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0      106 2023-04-04 15:40:17.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/index.json
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/styles/style.qss
--rw-rw-rw-   0        0        0    26822 2023-04-12 21:58:36.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/value/value_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.377156 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/
--rw-rw-rw-   0        0        0      636 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/__init__.py
--rw-rw-rw-   0        0        0     8426 2023-03-30 13:55:55.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/line_segments.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.383679 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/
--rw-rw-rw-   0        0        0      841 2023-03-17 14:15:26.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-rw-rw-   0        0        0       34 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-rw-rw-   0        0        0      754 2023-03-18 15:01:04.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/index.json
--rw-rw-rw-   0        0        0      121 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-rw-rw-   0        0        0      198 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-rw-rw-   0        0        0      228 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-rw-rw-   0        0        0     3520 2023-03-18 15:02:05.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/style.qss
--rw-rw-rw-   0        0        0      597 2023-03-18 15:06:21.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-rw-rw-   0        0        0      471 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-rw-rw-   0        0        0      388 2023-03-09 18:33:57.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.383679 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/test/
--rw-rw-rw-   0        0        0        0 2023-03-08 16:08:46.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/test/__init__.py
--rw-rw-rw-   0        0        0    13485 2023-03-18 15:03:45.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_control.py
--rw-rw-rw-   0        0        0   122898 2023-04-13 20:41:07.000000 joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:58:46.168703 joulescope_ui-1.0.8/joulescope_ui.egg-info/
--rw-rw-rw-   0        0        0     6885 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9841 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      363 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 20:58:45.000000 joulescope_ui-1.0.8/joulescope_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-04-13 20:58:46.387683 joulescope_ui-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     8932 2023-04-13 20:52:43.000000 joulescope_ui-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.912522 joulescope_ui-1.0.9/
+-rw-rw-rw-   0        0        0    37919 2023-04-19 16:43:39.000000 joulescope_ui-1.0.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0    13225 2023-04-04 17:19:13.000000 joulescope_ui-1.0.9/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 joulescope_ui-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      160 2023-03-10 02:18:44.000000 joulescope_ui-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6885 2023-04-19 20:45:42.912522 joulescope_ui-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5309 2023-03-10 14:30:22.000000 joulescope_ui-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.814854 joulescope_ui-1.0.9/joulescope_ui/
+-rw-rw-rw-   0        0        0     2976 2023-03-29 15:40:51.000000 joulescope_ui-1.0.9/joulescope_ui/__init__.py
+-rw-rw-rw-   0        0        0      902 2023-03-09 20:16:57.000000 joulescope_ui-1.0.9/joulescope_ui/__main__.py
+-rw-rw-rw-   0        0        0     1886 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/about.py
+-rw-rw-rw-   0        0        0     3935 2023-03-12 15:18:01.000000 joulescope_ui-1.0.9/joulescope_ui/api.py
+-rw-rw-rw-   0        0        0     7197 2023-04-12 21:24:46.000000 joulescope_ui-1.0.9/joulescope_ui/app.py
+-rw-rw-rw-   0        0        0     7516 2023-03-20 12:38:29.000000 joulescope_ui-1.0.9/joulescope_ui/capabilities.py
+-rw-rw-rw-   0        0        0     6226 2023-03-29 15:41:11.000000 joulescope_ui-1.0.9/joulescope_ui/dev_signal_buffer_source.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.831380 joulescope_ui-1.0.9/joulescope_ui/devices/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.835387 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/__init__.py
+-rw-rw-rw-   0        0        0     4017 2023-04-18 21:58:55.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/device.py
+-rw-rw-rw-   0        0        0    24887 2023-04-18 21:59:46.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/js110.py
+-rw-rw-rw-   0        0        0    27453 2023-04-18 21:59:10.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/js220.py
+-rw-rw-rw-   0        0        0    11428 2023-04-15 17:24:24.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/js220_updater.py
+-rw-rw-rw-   0        0        0    18214 2023-04-18 21:32:39.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-rw-rw-   0        0        0     7444 2023-04-18 21:05:59.000000 joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.835887 joulescope_ui-1.0.9/joulescope_ui/entry_points/
+-rw-rw-rw-   0        0        0        0 2020-04-07 21:08:41.000000 joulescope_ui-1.0.9/joulescope_ui/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2318 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/entry_points/ui.py
+-rw-rw-rw-   0        0        0     3168 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/error_window.py
+-rw-rw-rw-   0        0        0     4917 2023-03-15 21:06:26.000000 joulescope_ui-1.0.9/joulescope_ui/expanding_widget.py
+-rw-rw-rw-   0        0        0    11849 2023-03-31 21:30:44.000000 joulescope_ui-1.0.9/joulescope_ui/exporter.py
+-rw-rw-rw-   0        0        0     3179 2023-01-24 22:12:47.000000 joulescope_ui-1.0.9/joulescope_ui/file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.788810 joulescope_ui-1.0.9/joulescope_ui/fonts/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.836387 joulescope_ui-1.0.9/joulescope_ui/fonts/DSEG14-Modern/
+-rw-rw-rw-   0        0        0     4487 2020-03-14 16:24:02.000000 joulescope_ui-1.0.9/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.836888 joulescope_ui-1.0.9/joulescope_ui/fonts/Hack/
+-rw-rw-rw-   0        0        0     3744 2023-04-04 17:09:37.000000 joulescope_ui-1.0.9/joulescope_ui/fonts/Hack/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.836888 joulescope_ui-1.0.9/joulescope_ui/fonts/Lato/
+-rw-rw-rw-   0        0        0     4500 2010-12-15 04:00:00.000000 joulescope_ui-1.0.9/joulescope_ui/fonts/Lato/OFL.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.836888 joulescope_ui-1.0.9/joulescope_ui/fonts/SourceCodePro/
+-rw-rw-rw-   0        0        0     4566 2023-04-04 17:17:39.000000 joulescope_ui-1.0.9/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.837891 joulescope_ui-1.0.9/joulescope_ui/fonts/SourceSerifPro/
+-rw-rw-rw-   0        0        0     4615 2014-05-30 04:00:00.000000 joulescope_ui-1.0.9/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-rw-rw-   0        0        0  3411435 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui/fonts.rcc
+-rw-rw-rw-   0        0        0     2642 2023-01-24 22:12:47.000000 joulescope_ui-1.0.9/joulescope_ui/getting_started.html
+-rw-rw-rw-   0        0        0     4994 2023-03-18 21:45:09.000000 joulescope_ui-1.0.9/joulescope_ui/help_ui.py
+-rw-rw-rw-   0        0        0     6488 2023-03-18 13:34:03.000000 joulescope_ui-1.0.9/joulescope_ui/jls_source.py
+-rw-rw-rw-   0        0        0     9069 2023-03-29 15:41:27.000000 joulescope_ui-1.0.9/joulescope_ui/jls_v1.py
+-rw-rw-rw-   0        0        0     8262 2023-03-29 22:24:39.000000 joulescope_ui-1.0.9/joulescope_ui/jls_v2.py
+-rw-rw-rw-   0        0        0     3109 2023-03-20 14:51:40.000000 joulescope_ui-1.0.9/joulescope_ui/json.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.838396 joulescope_ui-1.0.9/joulescope_ui/locale/
+-rw-rw-rw-   0        0        0      965 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/locale/__init__.py
+-rw-rw-rw-   0        0        0     5629 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/logging_util.py
+-rw-rw-rw-   0        0        0    25818 2023-04-19 15:46:59.000000 joulescope_ui-1.0.9/joulescope_ui/main.py
+-rw-rw-rw-   0        0        0     2171 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/mem_leak_debugger.py
+-rw-rw-rw-   0        0        0     9118 2023-03-18 18:14:25.000000 joulescope_ui-1.0.9/joulescope_ui/metadata.py
+-rw-rw-rw-   0        0        0     5808 2023-04-12 17:49:24.000000 joulescope_ui-1.0.9/joulescope_ui/paths.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.841403 joulescope_ui-1.0.9/joulescope_ui/plugins/
+-rw-rw-rw-   0        0        0      792 2023-03-20 13:23:46.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/__init__.py
+-rw-rw-rw-   0        0        0     8662 2023-04-12 17:48:45.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/cdf.py
+-rw-rw-rw-   0        0        0    10906 2023-04-12 17:49:28.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/frequency.py
+-rw-rw-rw-   0        0        0     9174 2023-04-12 17:49:32.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/histogram.py
+-rw-rw-rw-   0        0        0     6270 2023-03-29 15:41:27.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/max_window.py
+-rw-rw-rw-   0        0        0     2219 2023-03-20 13:10:43.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/plugin_helpers.py
+-rw-rw-rw-   0        0        0     4247 2023-03-13 18:49:46.000000 joulescope_ui-1.0.9/joulescope_ui/plugins/usb_inrush.py
+-rw-rw-rw-   0        0        0     2130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/process_monitor.py
+-rw-rw-rw-   0        0        0     1008 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/profile.py
+-rw-rw-rw-   0        0        0    66542 2023-04-19 13:39:06.000000 joulescope_ui-1.0.9/joulescope_ui/pubsub.py
+-rw-rw-rw-   0        0        0    12868 2023-03-19 18:14:07.000000 joulescope_ui-1.0.9/joulescope_ui/range_tool.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.841903 joulescope_ui-1.0.9/joulescope_ui/resources/
+-rw-rw-rw-   0        0        0    11509 2019-07-27 15:33:28.000000 joulescope_ui-1.0.9/joulescope_ui/resources/dmg_background.svg
+-rw-rw-rw-   0        0        0     3357 2020-11-05 22:48:01.000000 joulescope_ui-1.0.9/joulescope_ui/resources/icons.svg
+-rw-rw-rw-   0        0        0    11282 2020-08-12 18:43:24.000000 joulescope_ui-1.0.9/joulescope_ui/resources/zoom.svg
+-rw-rw-rw-   0        0        0     1989 2023-04-04 16:57:10.000000 joulescope_ui-1.0.9/joulescope_ui/resources.py
+-rw-rw-rw-   0        0        0    22839 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui/resources.rcc
+-rw-rw-rw-   0        0        0     1840 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/sanitize.py
+-rw-rw-rw-   0        0        0     1304 2023-04-13 20:26:58.000000 joulescope_ui-1.0.9/joulescope_ui/shortcuts.py
+-rw-rw-rw-   0        0        0    10890 2023-03-20 18:55:58.000000 joulescope_ui-1.0.9/joulescope_ui/software_update.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.847407 joulescope_ui-1.0.9/joulescope_ui/styles/
+-rw-rw-rw-   0        0        0     3239 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/README.md
+-rw-rw-rw-   0        0        0      870 2023-04-18 13:02:13.000000 joulescope_ui-1.0.9/joulescope_ui/styles/__init__.py
+-rw-rw-rw-   0        0        0     4354 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/color_editor.py
+-rw-rw-rw-   0        0        0     4369 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/color_file.py
+-rw-rw-rw-   0        0        0     7155 2023-04-18 13:11:29.000000 joulescope_ui-1.0.9/joulescope_ui/styles/color_picker.py
+-rw-rw-rw-   0        0        0      944 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/color_scheme.py
+-rw-rw-rw-   0        0        0     1383 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0     1383 2023-04-17 21:01:22.000000 joulescope_ui-1.0.9/joulescope_ui/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      778 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/font_scheme.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 19:50:28.000000 joulescope_ui-1.0.9/joulescope_ui/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0     3405 2023-04-04 16:50:03.000000 joulescope_ui-1.0.9/joulescope_ui/styles/fonts.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.858928 joulescope_ui-1.0.9/joulescope_ui/styles/js1/
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/arrow_down.svg
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/arrow_left.svg
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/arrow_right.svg
+-rw-rw-rw-   0        0        0      179 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/arrow_up.svg
+-rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/branch_closed.svg
+-rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/branch_end.svg
+-rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-rw-rw-   0        0        0      177 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/branch_more.svg
+-rw-rw-rw-   0        0        0       86 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/branch_open.svg
+-rw-rw-rw-   0        0        0       93 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/branch_vline.svg
+-rw-rw-rw-   0        0        0      335 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-rw-rw-   0        0        0      499 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-rw-rw-   0        0        0      264 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-rw-rw-   0        0        0      234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/close.svg
+-rw-rw-rw-   0        0        0     1907 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/detach.svg
+-rw-rw-rw-   0        0        0      259 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-rw-rw-   0        0        0      191 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-rw-rw-   0        0        0     2382 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/index.json
+-rw-rw-rw-   0        0        0      432 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/radio_checked.svg
+-rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-rw-rw-   0        0        0      263 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/sizegrip.svg
+-rw-rw-rw-   0        0        0      419 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/style.html
+-rw-rw-rw-   0        0        0    19524 2023-04-04 14:57:41.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/style.qss
+-rw-rw-rw-   0        0        0      526 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-rw-rw-   0        0        0       31 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/transparent.svg
+-rw-rw-rw-   0        0        0      760 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-rw-rw-   0        0        0      653 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-rw-rw-   0        0        0    15284 2023-04-18 14:51:28.000000 joulescope_ui-1.0.9/joulescope_ui/styles/manager.py
+-rw-rw-rw-   0        0        0     3635 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/parameter_file.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.861438 joulescope_ui-1.0.9/joulescope_ui/styles/system/
+-rw-rw-rw-   0        0        0      350 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/system/index.json
+-rw-rw-rw-   0        0        0       17 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/system/style.html
+-rw-rw-rw-   0        0        0     3222 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/system/style.qss
+-rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/system/zoom_all.svg
+-rw-rw-rw-   0        0        0      481 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/system/zoom_in.svg
+-rw-rw-rw-   0        0        0      393 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/system/zoom_out.svg
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.862938 joulescope_ui-1.0.9/joulescope_ui/styles/test/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/test/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/test/test_color_file.py
+-rw-rw-rw-   0        0        0     2156 2023-03-18 18:42:17.000000 joulescope_ui-1.0.9/joulescope_ui/styles/test/test_manager.py
+-rw-rw-rw-   0        0        0     1959 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/styles/test/test_parameter_file.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.867444 joulescope_ui-1.0.9/joulescope_ui/test/
+-rw-rw-rw-   0        0        0        0 2018-04-10 21:33:42.000000 joulescope_ui-1.0.9/joulescope_ui/test/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-03-10 14:49:52.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_capabilities.py
+-rw-rw-rw-   0        0        0     6851 2023-04-12 17:49:35.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_metadata.py
+-rw-rw-rw-   0        0        0    10861 2023-04-13 20:09:56.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_pubsub.py
+-rw-rw-rw-   0        0        0    16639 2023-04-19 14:30:33.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_pubsub_registry.py
+-rw-rw-rw-   0        0        0     5147 2023-03-16 16:02:02.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_range_tool.py
+-rw-rw-rw-   0        0        0     2582 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_sanitize.py
+-rw-rw-rw-   0        0        0     2034 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_software_update.py
+-rw-rw-rw-   0        0        0     4055 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_time_map.py
+-rw-rw-rw-   0        0        0     1601 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_tooltip.py
+-rw-rw-rw-   0        0        0     5229 2023-04-12 21:57:44.000000 joulescope_ui-1.0.9/joulescope_ui/test/test_units.py
+-rw-rw-rw-   0        0        0     3197 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/time_map.py
+-rw-rw-rw-   0        0        0     2234 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/tooltip.py
+-rw-rw-rw-   0        0        0     7060 2023-01-24 22:12:47.000000 joulescope_ui-1.0.9/joulescope_ui/ui_util.py
+-rw-rw-rw-   0        0        0     7261 2023-04-12 21:56:15.000000 joulescope_ui-1.0.9/joulescope_ui/units.py
+-rw-rw-rw-   0        0        0       23 2023-04-15 15:56:23.000000 joulescope_ui-1.0.9/joulescope_ui/version.py
+-rw-rw-rw-   0        0        0    12344 2023-04-18 15:21:27.000000 joulescope_ui-1.0.9/joulescope_ui/view.py
+-rw-rw-rw-   0        0        0     1042 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widget_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.868444 joulescope_ui-1.0.9/joulescope_ui/widgets/
+-rw-rw-rw-   0        0        0     1207 2023-04-17 17:53:53.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.869447 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/
+-rw-rw-rw-   0        0        0      642 2023-04-12 20:02:06.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     6954 2023-04-12 21:59:19.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.871461 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/
+-rw-rw-rw-   0        0        0      109 2023-04-12 20:03:25.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      107 2023-04-17 21:21:42.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0       37 2023-04-12 20:36:04.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-rw-rw-   0        0        0      762 2023-04-12 20:35:40.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.873461 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/
+-rw-rw-rw-   0        0        0      647 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/__init__.py
+-rw-rw-rw-   0        0        0     3307 2023-04-15 15:00:22.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-rw-rw-   0        0        0     3397 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-rw-rw-   0        0        0    20370 2023-04-19 15:54:50.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.877968 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/
+-rw-rw-rw-   0        0        0      180 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-rw-rw-   0        0        0      129 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-rw-rw-   0        0        0       78 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0       78 2023-04-17 20:49:04.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-rw-rw-   0        0        0     1936 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/index.json
+-rw-rw-rw-   0        0        0     1749 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-rw-rw-   0        0        0      125 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-rw-rw-   0        0        0     4466 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-rw-rw-   0        0        0      240 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/target_power.svg
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.878469 joulescope_ui-1.0.9/joulescope_ui/widgets/example/
+-rw-rw-rw-   0        0        0      639 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/__init__.py
+-rw-rw-rw-   0        0        0     2100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/example_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.880475 joulescope_ui-1.0.9/joulescope_ui/widgets/example/styles/
+-rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      100 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0       80 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/styles/index.json
+-rw-rw-rw-   0        0        0      242 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/example/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.881476 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/
+-rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/__init__.py
+-rw-rw-rw-   0        0        0     4010 2023-03-17 14:48:42.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.882975 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/styles/
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      130 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/styles/index.json
+-rw-rw-rw-   0        0        0      692 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.883976 joulescope_ui-1.0.9/joulescope_ui/widgets/hamburger/
+-rw-rw-rw-   0        0        0      638 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/hamburger/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.883976 joulescope_ui-1.0.9/joulescope_ui/widgets/help/
+-rw-rw-rw-   0        0        0      628 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/help/__init__.py
+-rw-rw-rw-   0        0        0     2350 2023-03-10 14:01:14.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/help/help_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.885481 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/
+-rw-rw-rw-   0        0        0      632 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/__init__.py
+-rw-rw-rw-   0        0        0    10815 2023-04-12 19:57:12.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/memory_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.886982 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/styles/
+-rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      105 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/styles/index.json
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/memory/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.887982 joulescope_ui-1.0.9/joulescope_ui/widgets/progress_bar/
+-rw-rw-rw-   0        0        0      643 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-rw-rw-   0        0        0     5816 2023-04-05 17:16:31.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.888481 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/
+-rw-rw-rw-   0        0        0      645 2023-04-17 17:53:35.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/__init__.py
+-rw-rw-rw-   0        0        0     2782 2023-04-17 18:46:53.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/record_status_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.890987 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/styles/
+-rw-rw-rw-   0        0        0      105 2023-04-17 18:20:41.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      105 2023-04-17 20:57:39.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      668 2023-04-17 18:43:02.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/styles/index.json
+-rw-rw-rw-   0        0        0      205 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/styles/record.svg
+-rw-rw-rw-   0        0        0      886 2023-04-17 18:44:04.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/record_status/styles/style.qss
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.891491 joulescope_ui-1.0.9/joulescope_ui/widgets/settings/
+-rw-rw-rw-   0        0        0      641 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/settings/__init__.py
+-rw-rw-rw-   0        0        0    22299 2023-04-18 15:04:23.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/settings/settings_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.892494 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/
+-rw-rw-rw-   0        0        0      633 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/__init__.py
+-rw-rw-rw-   0        0        0     9819 2023-04-13 18:54:20.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.898003 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/
+-rw-rw-rw-   0        0        0      575 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      579 2023-04-17 20:58:38.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      358 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-rw-rw-   0        0        0      345 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-rw-rw-   0        0        0     4413 2023-04-13 15:29:15.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-rw-rw-   0        0        0      421 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-rw-rw-   0        0        0      274 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-rw-rw-   0        0        0      241 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-rw-rw-   0        0        0      205 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-rw-rw-   0        0        0      511 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-rw-rw-   0        0        0      309 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-rw-rw-   0        0        0     5528 2023-04-13 15:30:01.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-rw-rw-   0        0        0      207 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/target_power.svg
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.899003 joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/
+-rw-rw-rw-   0        0        0      699 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/__init__.py
+-rw-rw-rw-   0        0        0     6727 2023-03-29 19:41:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-rw-rw-   0        0        0     7983 2023-03-18 13:24:49.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.900511 joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/
+-rw-rw-rw-   0        0        0      715 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-03-18 13:36:54.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-rw-rw-   0        0        0     6501 2023-03-18 13:25:13.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-rw-rw-   0        0        0     6078 2023-01-24 22:12:47.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/switch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.901511 joulescope_ui-1.0.9/joulescope_ui/widgets/value/
+-rw-rw-rw-   0        0        0      630 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.904011 joulescope_ui-1.0.9/joulescope_ui/widgets/value/styles/
+-rw-rw-rw-   0        0        0      152 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      152 2023-04-17 20:59:52.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0      106 2023-04-04 15:40:17.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      122 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/styles/index.json
+-rw-rw-rw-   0        0        0        0 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/styles/style.qss
+-rw-rw-rw-   0        0        0    27003 2023-04-19 14:39:04.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/value/value_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.906014 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/
+-rw-rw-rw-   0        0        0      636 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/__init__.py
+-rw-rw-rw-   0        0        0     8426 2023-03-30 13:55:55.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/line_segments.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.912022 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/
+-rw-rw-rw-   0        0        0      722 2023-04-18 13:21:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-rw-rw-   0        0        0      724 2023-04-18 15:41:46.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-rw-rw-   0        0        0       34 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-rw-rw-   0        0        0      754 2023-03-18 15:01:04.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/index.json
+-rw-rw-rw-   0        0        0      121 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-rw-rw-   0        0        0      198 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-rw-rw-   0        0        0      228 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-rw-rw-   0        0        0      237 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-rw-rw-   0        0        0     3878 2023-04-18 17:49:13.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-rw-rw-   0        0        0      167 2023-04-18 13:35:30.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/style_defines.txt
+-rw-rw-rw-   0        0        0      597 2023-03-18 15:06:21.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-rw-rw-   0        0        0      558 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-rw-rw-   0        0        0      471 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-rw-rw-   0        0        0      388 2023-03-09 18:33:57.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.912022 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 16:08:46.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-rw-rw-   0        0        0    13484 2023-04-18 17:52:06.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-rw-rw-   0        0        0     2891 2023-04-18 19:24:04.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/waveform_source_widget.py
+-rw-rw-rw-   0        0        0   125758 2023-04-19 15:41:39.000000 joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/waveform_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:45:42.831380 joulescope_ui-1.0.9/joulescope_ui.egg-info/
+-rw-rw-rw-   0        0        0     6885 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10399 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      363 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 20:45:42.000000 joulescope_ui-1.0.9/joulescope_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-04-19 20:45:42.916524 joulescope_ui-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     8932 2023-04-15 16:45:58.000000 joulescope_ui-1.0.9/setup.py
```

### Comparing `joulescope_ui-1.0.8/CHANGELOG.md` & `joulescope_ui-1.0.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,37 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 
+## 1.0.9
+
+<span style="color:yellow">⚠ ALPHA RELEASE - USE WITH CAUTION ⚠</span> 
+
+Improves upon 1.0.7 but still alpha quality.  See the 1.0.0 release
+notes below for additional usage guidelines.
+
+2023 Apr 19
+
+* Improved pyjoulescope_driver stability (version 1.3.3).
+* Improved firmware update.
+  * Does not block Qt event thread.
+  * Added recovery (handles JS220's in updater).
+* Improved JS220 close error handling. 
+* Removed unnecessary timeouts for driver publish that lock Qt event thread.
+* Added record status to status bar.
+* Switched to monochromatic waveform traces. (prep for multiple traces)
+* Added light color scheme.
+* Fixed defect with settings widget not populating current value.
+* Fixed waveform widget to work with device open/close & insert/remove.
+* Fixed pubsub reregister for class properties.
+* Fixed multimeter not respected default source.
+
+
 ## 1.0.8
 
 <span style="color:yellow">⚠ ALPHA RELEASE - USE WITH CAUTION ⚠</span> 
 
 Improves upon 1.0.7 but still alpha quality.  See the 1.0.0 release
 notes below for additional usage guidelines.
```

### Comparing `joulescope_ui-1.0.8/CREDITS.html` & `joulescope_ui-1.0.9/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/LICENSE.txt` & `joulescope_ui-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/PKG-INFO` & `joulescope_ui-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.0.8
+Version: 1.0.9
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.0.8/README.md` & `joulescope_ui-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/__main__.py` & `joulescope_ui-1.0.9/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/about.py` & `joulescope_ui-1.0.9/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/api.py` & `joulescope_ui-1.0.9/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/app.py` & `joulescope_ui-1.0.9/joulescope_ui/app.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/capabilities.py` & `joulescope_ui-1.0.9/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.0.9/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 from joulescope_ui.metadata import Metadata
 import logging
 
 
 CAPABILITIES_CLASS = [CAPABILITIES.DEVICE_CLASS]
 CAPABILITIES_OBJECT = [
     CAPABILITIES.DEVICE_OBJECT,
+]
+
+
+CAPABILITIES_OBJECT_OPEN = [
+    # dynamically added when the open opens, removed on close
     CAPABILITIES.SOURCE,
     CAPABILITIES.STATISTIC_STREAM_SOURCE,
     CAPABILITIES.SIGNAL_STREAM_SOURCE,
 ]
 
 
 class Device:
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/js110.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from joulescope_ui import N_, CAPABILITIES, register, Metadata, get_topic_name
-from .device import Device
+from .device import Device, CAPABILITIES_OBJECT_OPEN
 import copy
 import numpy as np
 import queue
 import threading
 
 
 EVENTS = {
@@ -510,51 +510,51 @@
 
     def _run_cmd_settings(self, topic, value):
         self._log.info(f'js110 setting(%s): %s <= %s', self, topic, value)
         if topic.endswith('/enable'):
             signal_id = topic.split('/')[1]
             t = _SIGNALS[signal_id]['topics'][0]
             if t is not None:
-                self._driver_publish(t, bool(value))
+                self._driver_publish(t, bool(value), timeout=0)
             else:
                 self._log.warning('invalid enable: %s', topic)
         elif topic in ['target_power', 'current_range']:
             self._current_range_update()
         elif topic == 'statistics_frequency':
             scnt = 2_000_000 // value
-            self._driver_publish('s/stats/scnt', scnt)
+            self._driver_publish('s/stats/scnt', scnt, timeout=0)
         elif topic == 'current_ranging/samples_window':
             if value in [1, 'm']:
-                self._driver_publish('s/i/range/win', 'm')
+                self._driver_publish('s/i/range/win', 'm', timeout=0)
             if value in [2, 'n']:
-                self._driver_publish('s/i/range/win', 'n')
+                self._driver_publish('s/i/range/win', 'n', timeout=0)
             else:
-                self._driver_publish('s/i/range/win_sz', int(value) - 256)
-                self._driver_publish('s/i/range/win', 'manual')
+                self._driver_publish('s/i/range/win_sz', int(value) - 256, timeout=0)
+                self._driver_publish('s/i/range/win', 'manual', timeout=0)
         elif topic in self._param_map:
             device_topic = self._param_map[topic]
-            self._driver_publish(device_topic, value)
+            self._driver_publish(device_topic, value, timeout=0)
         elif topic == 'name':
             self._ui_publish('settings/sources/1/name', value)
         elif topic in ['info', 'state', 'state_req', 'out', 'enable',
                        'sources', 'sources/1', 'sources/1/info', 'sources/1/name',
                        'signals', 'current_ranging']:
             pass
         elif topic.startswith('signals/'):
             pass
         else:
             self._log.warning('Unsupported topic %s', f'{get_topic_name(self)}/settings/{topic}')
 
     def _current_range_update(self):
         if self._target_power_app and self.target_power:
             self._log.info('current_range on %s', self.current_range)
-            self._driver_publish('s/i/range/select', self.current_range)
+            self._driver_publish('s/i/range/select', self.current_range, timeout=0)
         else:
             self._log.info('current_range off')
-            self._driver_publish('s/i/range/select', 'off')
+            self._driver_publish('s/i/range/select', 'off', timeout=0)
 
     def _run_cmd(self, cmd, args):
         if cmd == 'settings':
             self._run_cmd_settings(*args)
         elif cmd == 'current_range_update':
             self._current_range_update()
         elif cmd == 'close':
@@ -565,23 +565,25 @@
     def _run(self):
         self._log.info('thread start')
         if self._open():
             self._log.info('thread exit due to open fail')
             return 1
         self._ui_publish('settings/state', 'open')
         self._log.info('thread open complete')
+        self._pubsub.capabilities_append(self, CAPABILITIES_OBJECT_OPEN)
         while not self._quit:
             try:
                 cmd, args = self._queue.get(timeout=0.1)
             except queue.Empty:
                 continue
             if cmd == 'close':
                 break
             self._run_cmd(cmd, args)
         self._close()
+        self._pubsub.capabilities_remove(self, CAPABILITIES_OBJECT_OPEN)
         self._log.info('thread stop')
         return 0
 
     def _open(self):
         self._log.info('open start')
         try:
             self._driver.open(self._path, 'restore')
@@ -589,17 +591,17 @@
             self._log.warning('driver open failed')
             self._ui_publish('settings/state', 'closing')
             return 1
         try:
             self._info['version'] = {'hw': 1}  # could get more info
             self._info = copy.deepcopy(self._info)
             self._ui_publish('settings/info', self._info)
-            self._driver_publish('s/i/lsb_src', 2)
-            self._driver_publish('s/v/lsb_src', 3)
-            self._driver_publish('s/stats/ctrl', 1)
+            self._driver_publish('s/i/lsb_src', 2, timeout=0)
+            self._driver_publish('s/v/lsb_src', 3, timeout=0)
+            self._driver_publish('s/stats/ctrl', 1, timeout=0)
             self._driver_subscribe('s/stats/value', 'pub', self._on_stats_fn)
             self._ui_subscribe('settings', self._on_settings_fn, ['pub', 'retain'])
         except Exception:
             self._log.exception('driver config failed')
             self._ui_publish('settings/state', 'closing')
             return 1
         self._log.info('open %s done', self.unique_id)
@@ -610,15 +612,15 @@
             return
         self._log.info('close %s start', self.unique_id)
         self._ui_unsubscribe('settings', self._on_settings_fn)
         self._ui_publish('settings/state', 'closing')
         self._driver_unsubscribe('s/stats/value', self._on_stats_fn)
         try:
             for t in _SIGNALS.values():
-                self._driver_publish(t['topics'][0], 0)
+                self._driver_publish(t['topics'][0], 0, timeout=0)
             self._driver_publish('s/stats/ctrl', 0)
         except RuntimeError as ex:
             self._log.info('Exception during close cleanup: %s', ex)
         self._driver.close(self._path)
         self._log.info('close %s done', self.unique_id)
 
     def _on_stats(self, topic, value):
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/js220.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from joulescope_ui.capabilities import CAPABILITIES
-from .device import Device
+from .device import Device, CAPABILITIES_OBJECT_OPEN
 from joulescope_ui import N_, get_topic_name, register
 from joulescope_ui.metadata import Metadata
 from pyjoulescope_driver import release, program
 import copy
 import queue
 import threading
 
@@ -536,40 +535,40 @@
 
     def _run_cmd_settings(self, topic, value):
         self._log.info(f'setting(%s): %s <= %s', self, topic, value)
         if topic.endswith('/enable'):
             signal_id = topic.split('/')[1]
             t = _SIGNALS[signal_id]['topics'][0]
             if t is not None:
-                self._driver_publish(t, bool(value))
+                self._driver_publish(t, bool(value), timeout=0)
             else:
                 self._log.warning('invalid enable: %s', topic)
         elif topic.startswith('out/'):
             v = _GPO_BIT[topic[4:]]
             t = 's/gpo/+/!set' if bool(value) else 's/gpo/+/!clr'
-            self._driver_publish(t, v)
+            self._driver_publish(t, v, timeout=0)
         elif topic == 'signal_frequency':
-            self._driver_publish('h/fs', int(value))
+            self._driver_publish('h/fs', int(value), timeout=0)
         elif topic == 'statistics_frequency':
             scnt = 1_000_000 // value
-            self._driver_publish('s/stats/scnt', scnt)
+            self._driver_publish('s/stats/scnt', scnt, timeout=0)
         elif topic == 'target_power':
             self._current_range_update()
         elif topic == 'current_range':
             self._current_range_update()
         elif topic == 'voltage_range':
             if value == -1:
-                self._driver_publish('s/v/range/mode', 'auto')
+                self._driver_publish('s/v/range/mode', 'auto', timeout=0)
             else:
-                self._driver_publish('s/v/range/mode', 'manual')
-                self._driver_publish('s/v/range/select', value)
+                self._driver_publish('s/v/range/mode', 'manual', timeout=0)
+                self._driver_publish('s/v/range/select', value, timeout=0)
         elif topic == 'trigger_dir':
-            self._driver_publish('c/trigger/dir', value)
+            self._driver_publish('c/trigger/dir', value, timeout=0)
         elif topic == 'gpio_voltage':
-            self._driver_publish('c/gpio/vref', value)
+            self._driver_publish('c/gpio/vref', value, timeout=0)
         elif topic == 'name':
             self._ui_publish('settings/sources/1/name', value)
         elif topic in ['info', 'state', 'state_req', 'out', 'enable',
                        'sources', 'sources/1', 'sources/1/info', 'sources/1/name',
                        'signals',
                        'firmware_available', 'firmware_channel']:
             pass
@@ -578,22 +577,22 @@
         else:
             self._log.warning('Unsupported topic %s', f'{get_topic_name(self)}/settings/{topic}')
 
     def _current_range_update(self):
         if self._target_power_app and self.target_power:
             if self.current_range == -1:
                 self._log.info('current_range auto')
-                self._driver_publish('s/i/range/mode', 'auto')
+                self._driver_publish('s/i/range/mode', 'auto', timeout=0)
             else:
                 self._log.info('current_range manual %s', self.current_range)
-                self._driver_publish('s/i/range/select', self.current_range)
-                self._driver_publish('s/i/range/mode', 'manual')
+                self._driver_publish('s/i/range/select', self.current_range, timeout=0)
+                self._driver_publish('s/i/range/mode', 'manual', timeout=0)
         else:
             self._log.info('current_range off')
-            self._driver_publish('s/i/range/mode', 'off')
+            self._driver_publish('s/i/range/mode', 'off', timeout=0)
 
     def _run_cmd(self, cmd, args):
         if cmd == 'settings':
             self._run_cmd_settings(*args)
         elif cmd == 'current_range_update':
             self._current_range_update()
         elif cmd == 'close':
@@ -619,67 +618,39 @@
         rv = {
             'ctrl_app': [v(ctrl_app_now), v(ctrl_app['version'])],
             'fpga': [v(fpga_now), v(fpga['version'])]
         }
         self._log.info('firmware_update_available %s: %s', self.unique_id, rv)
         return rv
 
-    def _firmware_update(self):
-        if self.firmware_available is None:
-            return False
-        try:
-            image = release.release_get(self.firmware_channel)
-        except Exception:
-            self._log.info('Could not parse firmware image')
-            return False
-        self._close()
-        self._log.info('firmware_update: start')
-        self.firmware_available = None
-        self._driver.open(self._path, 'restore')
-
-        def on_progress(completion, msg):
-            value = {
-                'id': f'{self.unique_id}.firmware_update',
-                'progress': completion,
-                'name': N_('Update') + ' ' + self.unique_id,
-                'brief': msg,
-            }
-            self._pubsub.publish(_PROGRESS_TOPIC, value)
-
-        rv = program.release_program(self._driver, self.device_path, image,
-                                     progress=on_progress)
-        versions_before = dict(rv[0])
-        result = ['firmware_update: complete']
-        for key, value in rv[1]:
-            v = versions_before.get(key, '?.?.?')
-            result.append(f'    {key:10s}  {v} => {value}')
-        self._log.info('\n'.join(result))
-        self._ui_publish('')
-        return True
-
     def _run(self):
         self._log.info('thread start')
         if self._open():
             self._log.info('thread exit due to open fail')
             return 1
         self._ui_publish('settings/state', 'open')
         self._log.info('thread open complete')
         self.firmware_available = self._is_firmware_update_available()
         if self.firmware_available is not None:
-            self._quit |= self._firmware_update()
+            self._log.info('firmware_update: start by reset to update1')
+            self._driver_publish('h/!reset', 'update1')
+            self._quit = True
+        else:
+            self._pubsub.capabilities_append(self, CAPABILITIES_OBJECT_OPEN)
 
         while not self._quit:
             try:
                 cmd, args = self._queue.get(timeout=0.1)
             except queue.Empty:
                 continue
             if cmd == 'close':
                 break
             self._run_cmd(cmd, args)
         self._close()
+        self._pubsub.capabilities_remove(self, CAPABILITIES_OBJECT_OPEN)
         self._log.info('thread stop')
         return 0
 
     def _open(self):
         self._log.info('open start')
         try:
             self._driver.open(self._path, 'restore')
@@ -691,15 +662,15 @@
             self._info['version'] = {
                 'hw': str(self._driver_query('c/hw/version') >> 24),
                 'fw': _version_u32_to_str(self._driver_query('c/fw/version')),
                 'fpga': _version_u32_to_str(self._driver_query('s/fpga/version')),
             }
             self._info = copy.deepcopy(self._info)
             self._ui_publish('settings/info', self._info)
-            self._driver_publish('s/stats/ctrl', 1)
+            self._driver_publish('s/stats/ctrl', 1, timeout=0)
             self._driver_subscribe('s/stats/value', 'pub', self._on_stats_fn)
             self._ui_subscribe('settings', self._on_settings_fn, ['pub', 'retain'])
         except Exception:
             self._log.exception('driver config failed')
             self._ui_publish('settings/state', 'closing')
             return 1
         self._driver_device_open = True
@@ -712,19 +683,22 @@
             return
         self._log.info('close %s start', self.unique_id)
         self._ui_unsubscribe('settings', self._on_settings_fn)
         self._ui_publish('settings/state', 'closing')
         self._driver_unsubscribe('s/stats/value', self._on_stats_fn)
         try:
             for t in _SIGNALS.values():
-                self._driver_publish(t['topics'][0], 0)
+                self._driver_publish(t['topics'][0], 0, timeout=0)
             self._driver_publish('s/stats/ctrl', 0)
-        except RuntimeError as ex:
+        except Exception as ex:
             self._log.info('Exception during close cleanup: %s', ex)
-        self._driver.close(self._path)
+        try:
+            self._driver.close(self._path)
+        except Exception as ex:
+            self._log.info('Exception during driver close: %s', ex)
         self._driver_device_open = False
         self._log.info('close %s done', self.unique_id)
 
     def _on_stats(self, topic, value):
         if self._statistics_offsets is None:
             accum_sample_start = value['time']['accum_samples']['value'][-1]
             charge = value['accumulators']['charge']['value']
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from joulescope_ui import CAPABILITIES, N_, Metadata, get_topic_name
+from joulescope_ui import CAPABILITIES, N_, Metadata, get_topic_name, get_unique_id, get_instance
 from pyjoulescope_driver import time64
 from .device import Device
 import copy
 import logging
 import time
 
 
@@ -147,82 +147,154 @@
         self.SETTINGS = _SETTINGS
         self._wrapper = wrapper  #: JsdrvWrapper
         self._initialize_cache = []
         self._id = f'{int(stream_buffer_id):03d}'
         self._rsp_topic = f'm/mem/{self._id}/!rsp'
         self._log = logging.getLogger(f'{__name__}.{self._id}')
         self._driver_subscriptions = []
-        self._sources: dict[str, Device] = {}  # device unique_id -> instance
+        self._sources: dict[str, str] = {}  # device unique_id -> device_path
         self._signals: dict[str, [int, object]] = {}     # signal id ui_str -> [buffer_id, meta]
         self._signals_reverse: dict[int, str] = {}  # signal id buffer_id -> ui_str
         self._device_signal_id_next = 1
         self._device_subscriptions = {}
         self._pubsub_subscriptions = []
+        self._pubsub_device_subscriptions = {}  # device_id: [(topic, fn), ...]
 
         self._signals_free = list(range(1, 256))
         self._req_fwd = {}  # (pubsub_rsp_topic, pubsub_rsp_id): device_rsp_id
         self._req_bwd = {}  # device_rsp_id: (pubsub_rsp_topic, pubsub_rsp_id)
         self._req_time = {}  # device_rsp_id: time_last_used
         self._collect_time = time.time()
 
     def __str__(self):
         return f'JsdrvStreamBuffer({self._id})'
 
-    def on_action_device_add(self, device: Device):
-        self._log.info('device_add %s', device.unique_id)
-        self._sources[device.unique_id] = device
+    def _on_device_ids(self, value):
+        self._log.info('_on_device_ids %s', value)
+        existing = set(self._sources.keys())
+        for unique_id in value:
+            if unique_id not in self._sources:
+                self._on_device_add(unique_id)
+            try:
+                existing.remove(unique_id)
+            except KeyError:
+                pass
+        for device in existing:
+            self._on_device_remove(device)
+
+    def _on_device_add(self, device):
+        unique_id = get_unique_id(device)
+        device = get_instance(unique_id)
+        if '-UPDATER' in device.unique_id:
+            return
+        self._log.info('device_add %s', unique_id)
+        self._sources[unique_id] = device.device_path
         topic = get_topic_name(self.unique_id)
-        source_topic = f'{topic}/settings/sources/{device.unique_id}'
+        source_topic = f'{topic}/settings/sources/{unique_id}'
         for name, meta in _SETTINGS_PER_SOURCE.items():
             self.pubsub.topic_add(f'{source_topic}/{name}', meta, exists_ok=True)
         self.pubsub.publish(f'{source_topic}/name', device.name)
         self.pubsub.publish(f'{source_topic}/info', device.info)
-        device_topic = get_topic_name(device)
+        self._ui_device_subscribe(device, 'settings/state',
+                                  self._on_device_state, ['pub', 'retain'])
+
+    def _on_device_state(self, topic, value):
+        unique_id = topic.split('/')[1]
+        if '-UPDATER' in unique_id:
+            return
+        if value == 2:  # open
+            self._on_device_open(unique_id)
+        else:
+            self._on_device_close(unique_id)  # may have duplicate close
+
+    def _on_device_open(self, device):
+        device_id = get_unique_id(device)
+        self._log.info('device_open %s', device_id)
+        device_topic = get_topic_name(device_id)
         for signal in self.pubsub.enumerate(f'{device_topic}/settings/signals'):
-            self.pubsub.subscribe(f'{device_topic}/settings/signals/{signal}/enable',
-                                  self._on_signal_enable, ['pub', 'retain'])
-        self.pubsub.publish(f'{topic}/events/sources/!add', device.unique_id)
+            self._ui_device_subscribe(device_id, f'settings/signals/{signal}/enable',
+                                      self._on_signal_enable, ['pub', 'retain'])
+        topic = get_topic_name(self.unique_id)
+        self.pubsub.publish(f'{topic}/events/sources/!add', device_id)
 
-    def on_action_device_remove(self, device):
-        self._log.info('device_remove %s', device.unique_id)
+    def _on_device_close(self, device):
+        device_id = get_unique_id(device)
+        if len(self._pubsub_device_subscriptions.get(device_id, [])) <= 1:
+            return
+        self._log.info('device_close %s', device_id)
         topic = get_topic_name(self.unique_id)
+        self.pubsub.publish(f'{topic}/events/sources/!remove', device_id)
         signals = list(self._signals.keys())
         for signal_id in signals:
-            if signal_id.split('.')[0] == device.unique_id:
+            if signal_id.split('.')[0] == device_id:
                 self.on_action_remove(signal_id)
-        source_topic = f'{topic}/settings/{device.unique_id}'
-        self.pubsub.publish(f'{topic}/events/sources/!remove', device.unique_id)
+        subs, self._pubsub_device_subscriptions[device_id] = self._pubsub_device_subscriptions[device_id], []
+        for topic, fn in subs:
+            if '/settings/state' in topic:
+                self._pubsub_device_subscriptions[device_id].append((topic, fn))
+            else:
+                self.pubsub.unsubscribe(topic, fn)
+        self._pubsub_device_subscriptions[device_id] = self._pubsub_device_subscriptions[device_id][:1]
+
+    def _on_device_remove(self, device):
+        unique_id = get_unique_id(device)
+        device_path = self._sources.pop(unique_id)
+        if '-UPDATER' in unique_id:
+            return
+        self._log.info('device_remove %s', unique_id)
+        topic = get_topic_name(self.unique_id)
+        source_topic = f'{topic}/settings/{unique_id}'
+        for topic, fn in self._pubsub_device_subscriptions.pop(unique_id, []):
+            self.pubsub.unsubscribe(topic, fn)
         for name, meta in _SETTINGS_PER_SOURCE.items():
             self.pubsub.topic_remove(f'{source_topic}/{name}')
         for topic in list(self._device_subscriptions.keys()):
-            if topic.startswith(device.device_path):
+            if topic.startswith(device_path):
                 fn = self._device_subscriptions.pop(topic)
                 self._wrapper.driver.unsubscribe(topic, fn)
-        del self._sources[device.unique_id]
 
     def _device_subscribe(self, topic, flags, fn):
         self._device_subscriptions[topic] = fn
         self._wrapper.driver.subscribe(topic, flags, fn)
 
     def _driver_publish(self, topic, value, timeout=None):
         if self._wrapper.driver is not None:
             self._wrapper.driver.publish(topic, value, timeout)
 
+    def _ui_subscribe(self, topic, fn, flags=None):
+        self.pubsub.subscribe(topic, fn, flags)
+        self._pubsub_subscriptions.append((topic, fn))
+
+    def _ui_device_subscribe(self, device, topic, fn, flags=None):
+        unique_id = get_unique_id(device)
+        if unique_id not in self._pubsub_device_subscriptions:
+            self._pubsub_device_subscriptions[unique_id] = []
+        base_topic = get_topic_name(unique_id)
+        topic = f'{base_topic}/{topic}'
+        self.pubsub.subscribe(topic, fn, flags)
+        self._pubsub_device_subscriptions[unique_id].append((topic, fn))
+
     def on_pubsub_register(self):
         topic = get_topic_name(self)
         for t in self.pubsub.enumerate(f'{topic}/settings/sources', absolute=True):
             self.pubsub.topic_remove(t)
         for t in self.pubsub.enumerate(f'{topic}/settings/signals', absolute=True):
             self.pubsub.topic_remove(t)
         self._driver_publish('m/@/!add', int(self._id))
         self._device_subscribe(self._rsp_topic, 'pub', self._on_buf_response)
         for fn, value in self._initialize_cache:
             fn(self, value)
         self._initialize_cache = None
-        self.pubsub.subscribe('registry/app/settings/signal_stream_enable', self._on_signal_steam_enable, ['pub', 'retain'])
+        self._ui_subscribe('registry/jsdrv/settings/device_ids', self._on_device_ids, ['pub', 'retain'])
+        self._ui_subscribe('registry/app/settings/signal_stream_enable', self._on_signal_steam_enable, ['pub', 'retain'])
+
+    def on_pubsub_unregister(self):
+        for topic, fn in self._pubsub_subscriptions:
+            self.pubsub.unsubscribe(topic, fn)
+        self._pubsub_subscriptions.clear()
 
     def _on_signal_steam_enable(self, value):
         if value and self.clear_on_play:
             self.on_action_clear()
         self.on_setting_hold(not bool(value))
 
     def on_pubsub_unregister(self):
@@ -274,22 +346,24 @@
     def on_action_add(self, signal_id):
         if signal_id in self._signals:
             self._log.info('add duplicate %s', signal_id)
             return
         self._log.info('add %s', signal_id)
         buf_id = self._signals_free.pop(0)
         unique_id, signal = signal_id.split('.')
-        device = self._sources[unique_id]
+        device = get_instance(unique_id)
+        device_path = self._sources[unique_id]
+        device_topic = get_topic_name(unique_id)
         signal_meta = copy.deepcopy(device.info)
         self._signals[signal_id] = [buf_id, signal_meta]
         self._signals_reverse[buf_id] = signal_id
-        device_path = device.device_path
+        device_path = device_path
 
         device_signal_id = signal_id.split('.')[1]
-        signal_name = self.pubsub.query(f'{get_topic_name(device)}/settings/signals/{device_signal_id}/name')
+        signal_name = self.pubsub.query(f'{device_topic}/settings/signals/{device_signal_id}/name')
         ui_prefix = get_topic_name(self)
         ui_signal_prefix = f'{ui_prefix}/settings/signals/{signal_id}'
         for key, meta in _SETTINGS_PER_SIGNAL.items():
             self.pubsub.topic_add(f'{ui_signal_prefix}/{key}', meta, exists_ok=True)
         self.pubsub.publish(f'{ui_signal_prefix}/name', signal_name)
         self.pubsub.publish(f'{ui_signal_prefix}/meta', signal_meta)
         self._driver_publish(f'm/{self._id}/a/!add', buf_id)
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.0.9/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 
 from pyjoulescope_driver import Driver
 from joulescope_ui import get_unique_id, get_topic_name, Metadata, N_
 from joulescope_ui.capabilities import CAPABILITIES
 from .jsdrv_stream_buffer import JsdrvStreamBuffer
 from .js110 import Js110
 from .js220 import Js220
+from .js220_updater import Js220Updater
 import logging
 
 
 class JsdrvWrapper:
     """The singleton Joulescope driver wrapper.
 
     Provide access to Joulescope devices including the JS220 and JS110.
     This class wraps a pyjoulescope_driver.Driver instance and relays
     messages between the UI's pubsub instance and the jsdrv pubsub
     instance.
     """
     CAPABILITIES = []
     EVENTS = {
-        '!publish': Metadata('obj', 'Resync to UI publish thread')
+        '!publish': Metadata('obj', 'Resync to UI publish thread'),
     }
     SETTINGS = {
         'log_level': {
             'dtype': 'str',
             'brief': N_('The pyjoulescope_driver log level.'),
             'options': [
                 ['off', 'off'],
@@ -48,14 +49,20 @@
                 ['debug1', 'debug1'],
                 ['debug2', 'debug2'],
                 ['debug3', 'debug3'],
                 ['debug3', 'all'],
             ],
             'default': 'info',
         },
+        'device_ids': {
+            'dtype': 'obj',  # list of unique_id
+            'brief': 'The connected jsdrv devices',
+            'default': None,
+            'flags': ['hide', 'tmp', 'noinit']
+        }
     }
 
     def __init__(self):
         self.CAPABILITIES = [CAPABILITIES.DEVICE_FACTORY]
         self._parent = None
         self._log = logging.getLogger(__name__)
         self.pubsub = None
@@ -67,14 +74,16 @@
         self._stream_buffers = {}
 
     def on_pubsub_register(self, pubsub):
         topic = get_topic_name(self)
         self._log.info('on_pubsub_register start %s', topic)
         self.pubsub = pubsub
         self._topic = topic
+        self.devices = {}
+        self.device_ids = []
         self.driver = Driver()
         self._ui_subscribe(f'{topic}/settings/log_level', self._on_log_level, ['retain', 'pub'])
         self._ui_subscribe(f'{topic}/events/!publish', self._on_event_publish, ['pub'])
         self.driver.subscribe('@', 'pub', self._on_driver_publish)
         for d in self.driver.device_paths():
             self._log.info('on_pubsub_register add %s', d)
             self._on_driver_publish('@/!add', d)
@@ -156,33 +165,31 @@
                 self._on_device_remove(value)
 
     def _on_device_add(self, value):
         _, model, serial_number = value.split('/')
         unique_id = f'{model.upper()}-{serial_number}'
         if value in self.devices:
             return
-        if 'js220' in value:
+        if '/js220/' in value:
             cls = Js220
-        elif 'js110' in value:
+        elif '/js110/' in value:
             cls = Js110
+        elif '/&js220/' in value:
+            unique_id = unique_id[1:] + '-UPDATER'
+            cls = Js220Updater
         else:
             self._log.info('Unsupported device: %s', value)
             return
         self._log.info('_on_device_add %s', unique_id)
         d = cls(self, value)
         self.pubsub.register(d, unique_id)
         self.devices[value] = d
-        for b in self._stream_buffers.values():
-            topic = get_topic_name(b)
-            self.pubsub.publish(f'{topic}/actions/!device_add', d)
+        self.device_ids = sorted([d.unique_id for d in self.devices.values()])
 
     def _on_device_remove(self, value):
         d = self.devices.pop(value, None)
         if d is not None:
-            for b in self._stream_buffers.values():
-                topic = get_topic_name(b)
-                self.pubsub.publish(f'{topic}/actions/!device_remove', d)
             self._log.info('_on_device_remove %s', get_unique_id(d))
             topic = get_topic_name(d)
             self.pubsub.publish(f'{topic}/actions/!finalize', None)
             self.pubsub.unregister(d)
-
+            self.device_ids = sorted([d.unique_id for d in self.devices.values()])
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.0.9/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/error_window.py` & `joulescope_ui-1.0.9/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/exporter.py` & `joulescope_ui-1.0.9/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/file_dialog.py` & `joulescope_ui-1.0.9/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.0.9/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.0.9/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.0.9/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.0.9/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.0.9/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/fonts.rcc` & `joulescope_ui-1.0.9/joulescope_ui/fonts.rcc`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/getting_started.html` & `joulescope_ui-1.0.9/joulescope_ui/getting_started.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/help_ui.py` & `joulescope_ui-1.0.9/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/jls_source.py` & `joulescope_ui-1.0.9/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/jls_v1.py` & `joulescope_ui-1.0.9/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/jls_v2.py` & `joulescope_ui-1.0.9/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/json.py` & `joulescope_ui-1.0.9/joulescope_ui/json.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/locale/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/logging_util.py` & `joulescope_ui-1.0.9/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/main.py` & `joulescope_ui-1.0.9/joulescope_ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,22 @@
 
         # Create the singleton sidebar widget
         self._side_bar = SideBar(self._central_widget)
         self._side_bar.register()
         self._central_layout.addWidget(self._side_bar)
         self._central_layout.addWidget(self._dock_widget)
 
+        self._signal_record_status = RecordStatusWidget(self, 'SignalRecord')
+        self._pubsub.register(self._signal_record_status, 'SignalRecord:0', parent='ui')
+        self._status_bar.addPermanentWidget(self._signal_record_status)
+
+        self._statistics_record_status = RecordStatusWidget(self, 'StatisticsRecord')
+        self._pubsub.register(self._statistics_record_status, 'StatisticsRecord:0', parent='ui')
+        self._status_bar.addPermanentWidget(self._statistics_record_status)
+
         self._menu_bar = QtWidgets.QMenuBar(self)
         self._menu_items = _menu_setup(self._menu_bar, [
             ['file_menu', N_('&File'), [
                 ['open', N_('Open'), ['registry/ui/actions/!file_open_request', '']],
                 ['open_recent_menu', N_('Open recent'), []],  # dynamically populated from MRU
                 # '&Preferences': self.on_preferences,
                 ['exit_cfg', N_('Clear config and exit'), ['registry/ui/actions/!close', {'config_clear': True}]],
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.0.9/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/metadata.py` & `joulescope_ui-1.0.9/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/paths.py` & `joulescope_ui-1.0.9/joulescope_ui/paths.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/cdf.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/cdf.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/frequency.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/frequency.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/histogram.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/histogram.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/max_window.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/plugin_helpers.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/plugins/usb_inrush.py` & `joulescope_ui-1.0.9/joulescope_ui/plugins/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/process_monitor.py` & `joulescope_ui-1.0.9/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/profile.py` & `joulescope_ui-1.0.9/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/pubsub.py` & `joulescope_ui-1.0.9/joulescope_ui/pubsub.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 CLS_CALLBACK_PREFIX = 'on_cls_callback_'
 CLS_EVENT_PREFIX = 'on_cls_event_'
 CLS_SETTING_PREFIX = 'on_cls_setting_'
 ACTION_PREFIX = 'on_action_'
 CALLBACK_PREFIX = 'on_callback_'
 SETTING_PREFIX = 'on_setting_'
 EVENT_PREFIX = 'on_event_'
-_PUBSUB_ATTR = '__pubsub__'
+_PUBSUB_CLS_ATTR = '__pubsub_cls__'
+_PUBSUB_OBJ_ATTR = '__pubsub_obj__'
 
 
 class PUBSUB_TOPICS:  # todo
     PUBSUB_APP_NAME = 'common/settings/name'
     PUBSUB_PROFILE_ACTION_ADD = 'common/actions/profile/!add'
     PUBSUB_PROFILE_ACTION_REMOVE = 'common/actions/profile/!remove'
     PUBSUB_PROFILE_ACTION_SAVE = 'common/actions/profile/!save'
@@ -67,14 +68,18 @@
     CAPABILITY_REMOVE = 'registry_manager/actions/capability/!remove'
     REGISTRY_ADD = 'registry_manager/actions/registry/!add'
     REGISTRY_REMOVE = 'registry_manager/actions/registry/!remove'
     CAPABILITIES = f'registry_manager/capabilities'
     NEXT_UNIQUE_ID = f'registry_manager/next_unique_id'
 
 
+def _pubsub_attr(x):
+    return _PUBSUB_CLS_ATTR if isinstance(x, type) else _PUBSUB_OBJ_ATTR
+
+
 def get_unique_id(obj):
     """Get the unique_id.
 
     :param obj: The source for the unique id, which can be any of:
         * The topic name string
         * The unique id string (simply returned)
         * A registered class or object
@@ -329,15 +334,15 @@
 
     Patching must handle the following scenarios:
     * property (on class)
     * class attribute
     * instance attribute
     * on_setting_{name} function
 
-    This relies upon the class already having the _PUBSUB_ATTR
+    This relies upon the class already having the _PUBSUB_CLS_ATTR
     attribute initialized with 'setting_cls' dict.
 
     This data descriptor intentionally using __init__ rather
     than using __set_name__ to more easily support monkey patching.
 
     See https://docs.python.org/3/howto/descriptor.html
     """
@@ -345,42 +350,43 @@
         self.pubsub = pubsub
         self.name = name
         self.attr_name = subtopic_to_name(name)
         self.item = None
         self._log = logging.getLogger(f'{__name__}.Setting.{self.attr_name}')
         if hasattr(cls, name):
             self.item = cls.__dict__[name]
-        cls.__dict__[_PUBSUB_ATTR]['setting_cls'][self.name] = self
+        cls.__dict__[_PUBSUB_CLS_ATTR]['setting_cls'][self.name] = self
         setattr(cls, name, self)
 
     # def __set_name__(self, owner, name):
 
     def __get__(self, obj, objtype=None):
         if obj is None:
             raise AttributeError(f'{self.name}')
-        attr = obj.__class__.__dict__[_PUBSUB_ATTR]['setting_cls']
+        attr = obj.__class__.__dict__[_PUBSUB_CLS_ATTR]['setting_cls']
         if self.name in attr:
             item = attr[self.name]
             if isinstance(item, property) and item.fget is not None:
                 return item.fget(obj)
             elif not self.name in obj.__dict__:
                 obj.__dict__[self.attr_name] = item
         return obj.__dict__[self.attr_name]
 
     def __set__(self, obj, value):
         self._set(obj, value)
         try:
-            unique_id = obj.__dict__[_PUBSUB_ATTR]['unique_id']
+            unique_id = obj.__dict__[_PUBSUB_OBJ_ATTR]['unique_id']
         except KeyError:
             return
         self.pubsub.publish(f'registry/{unique_id}/settings/{self.name}', value)
 
     def _set(self, obj, value):
-        if _PUBSUB_ATTR in obj.__class__.__dict__:
-            attr = obj.__class__.__dict__[_PUBSUB_ATTR]
+        cls = obj.__class__
+        if _PUBSUB_CLS_ATTR in cls.__dict__:
+            attr = cls.__dict__[_PUBSUB_CLS_ATTR]
             if 'setting_cls' in attr:
                 attr = attr['setting_cls']
                 if self.name in attr:
                     item = attr[self.name].item
                     if isinstance(item, property) and item.fset is not None:
                         item.fset(obj, value)
         obj.__dict__[self.attr_name] = value
@@ -388,18 +394,18 @@
     def on_publish_factory(self, obj):
         def fn(pubsub, topic: str, value):
             return self.on_publish(obj, pubsub, topic, value)
         return fn
 
     def on_publish(self, obj, pubsub, topic: str, value):
         self._set(obj, value)
-        if _PUBSUB_ATTR not in obj.__dict__:
+        if _PUBSUB_OBJ_ATTR not in obj.__dict__:
             self._log.warning('on_publish but no __pubsub__ attr')
             return
-        attr = obj.__dict__[_PUBSUB_ATTR]
+        attr = obj.__dict__[_PUBSUB_OBJ_ATTR]
         if 'setting' not in attr:
             self._log.warning('on_publish but no setting attr')
             return
         attr = attr['setting']
         fn_name = f'{SETTING_PREFIX}{subtopic_to_name(self.name)}'
         if fn_name not in attr:
             fn = getattr(obj, fn_name, None)
@@ -1078,15 +1084,16 @@
         :param unique_id: The unique_id to use for this class.
             None (default) determines a suitable unique_id.
             For classes, the class name.
             For instances, a randomly generated value.
         :type unique_id: str, optional
         :param parent: The optional parent unique_id, topic, or object.
         """
-        if _PUBSUB_ATTR in obj.__dict__ and len(obj.__dict__[_PUBSUB_ATTR]):
+        pubsub_attr = _pubsub_attr(obj)
+        if pubsub_attr in obj.__dict__ and len(obj.__dict__[pubsub_attr]):
             self._log.info('Duplicate registration for %s', obj)
             if parent is not None:
                 self._parent_add(obj, parent)
             return
         if unique_id is None:
             if isinstance(obj, type):
                 # Use the unqualified class name
@@ -1096,23 +1103,23 @@
                 cls_unique_id = getattr(obj.__class__, 'unique_id', obj.__class__.__name__)
                 t = self._topic_by_name[REGISTRY_MANAGER_TOPICS.NEXT_UNIQUE_ID]
                 v = t.value
                 t.value += 1
                 unique_id = f'{cls_unique_id}:{v:08x}'
         else:
             unique_id = get_unique_id(unique_id)
-        setattr(obj, _PUBSUB_ATTR, {
+        setattr(obj, pubsub_attr, {
             'unique_id': unique_id,
             'functions': {},    # topic: callable
             'setting_cls': {},  # topic: object, for existing class attribute
             'setting': {},
         })
         if not isinstance(obj, type):
             cls = obj.__class__
-            if _PUBSUB_ATTR not in cls.__dict__ or not len(cls.__dict__[_PUBSUB_ATTR]):
+            if _PUBSUB_CLS_ATTR not in cls.__dict__ or not len(cls.__dict__[_PUBSUB_CLS_ATTR]):
                 self.register(cls, cls.__name__ + '.class')
         self._log.info('register(unique_id=%s, obj=%s) start', unique_id, obj)
         doc = obj.__doc__
         if doc is None:
             doc = obj.__init__.__doc__
         doc = _parse_docstr(doc, unique_id)
         meta = Metadata(dtype='node', brief=doc)
@@ -1137,15 +1144,15 @@
                     self.publish(instances_topic, instances + [unique_id])
             self._reg_topic(f'{topic_name}/parent',
                             Metadata(dtype='str', brief='unique id for the parent', default=''))
             self._reg_topic(f'{topic_name}/children',
                             Metadata(dtype='obj', brief='list of unique ids for children', default=[]))
 
         self._register_events(obj, unique_id)
-        self._register_functions(obj, unique_id)
+        self._register_functions(obj, unique_id)  # on_action and on_callback, but not on_setting
         self._register_settings_create(obj, unique_id)
         obj.pubsub = self
         obj.unique_id = unique_id
         obj.topic = topic_name
         self._register_settings_connect(obj, unique_id)
         if parent is not None:
             self._parent_add(obj, parent)
@@ -1186,15 +1193,16 @@
 
     def _register_events(self, obj, unique_id: str):
         topic_name = get_topic_name(unique_id)
         for event, meta in getattr(obj, 'EVENTS', {}).items():
             self.topic_add(f'{topic_name}/events/{event}', meta, exists_ok=True)
 
     def _register_functions(self, obj, unique_id: str):
-        functions = obj.__dict__[_PUBSUB_ATTR]['functions']
+        pubsub_attr = _pubsub_attr(obj)
+        functions = obj.__dict__[pubsub_attr]['functions']
         topic_name = get_topic_name(unique_id)
         if isinstance(obj, type):
             while obj != object:
                 for name, attr in obj.__dict__.items():
                     if isinstance(attr, staticmethod):
                         if name.startswith(CLS_ACTION_PREFIX):
                             fn_name = name[len(CLS_ACTION_PREFIX):]
@@ -1227,15 +1235,15 @@
                         fn_topic = _fn_name_to_topic(fn_name)
                         topic = f'{topic_name}/callbacks/{fn_topic}'
                         if topic not in functions:
                             functions[topic] = self.register_command(topic, getattr(obj, name))
                 cls = cls.__base__
 
     def _unregister_functions(self, obj, unique_id: str = None):
-        functions = obj.__dict__[_PUBSUB_ATTR].pop('functions')
+        functions = obj.__dict__[_pubsub_attr(obj)].pop('functions')
         settings_topic = f'{obj.topic}/settings/'
         while len(functions):
             topic, fn = functions.popitem()
             if topic.startswith(settings_topic):
                 self.unsubscribe(topic, fn, flags=['pub'])
             else:
                 self.unsubscribe(topic, fn, flags=['command'])
@@ -1247,15 +1255,15 @@
             obj._pubsub_setting_to_topic = {}
         for setting_name, meta in settings.items():
             topic_name = f'{topic_base_name}/settings/{setting_name}'
             if topic_name not in self:
                 meta = Metadata(meta)
                 if not isinstance(obj, type) and 'noinit' not in meta.flags:
                     # attempt to set instance default value from class
-                    cls_unique_id = obj.__class__.__dict__[_PUBSUB_ATTR]['unique_id']
+                    cls_unique_id = obj.__class__.__dict__[_PUBSUB_CLS_ATTR]['unique_id']
                     cls_topic = get_topic_name(cls_unique_id)
                     if cls_topic in self:
                         try:
                             meta.default = self.query(f'{cls_topic}/settings/{setting_name}')
                         except KeyError:
                             pass  # use meta default
                 self.topic_add(topic_name, meta=meta)
@@ -1271,26 +1279,26 @@
             topic_name = f'{topic_base_name}/settings/{setting_name}'
             if isinstance(obj, type):
                 self._setting_cls_connect(obj, topic_name, setting_name)
             else:
                 self._setting_connect(obj, topic_name, setting_name)
 
     def _setting_cls_connect(self, cls, topic_name, setting_name):
-        functions = cls.__dict__[_PUBSUB_ATTR]['functions']
+        functions = cls.__dict__[_PUBSUB_CLS_ATTR]['functions']
         cls_fn_name = f'{CLS_SETTING_PREFIX}{subtopic_to_name(setting_name)}'
         if hasattr(cls, cls_fn_name):
             fn = getattr(cls, cls_fn_name)
             self.subscribe(topic_name, fn, flags=['pub', 'retain'])
             functions[topic_name] = fn
 
     def _setting_connect(self, obj, topic_name, setting_name):
-        functions = obj.__dict__[_PUBSUB_ATTR]['functions']
+        functions = obj.__dict__[_PUBSUB_OBJ_ATTR]['functions']
         cls = obj.__class__
-        cls_attr = cls.__dict__[_PUBSUB_ATTR]
-        if setting_name not in cls_attr:
+        cls_attr = cls.__dict__[_PUBSUB_CLS_ATTR]
+        if setting_name not in cls_attr['setting_cls']:
             _Setting(self, cls, setting_name)
         setting = cls_attr['setting_cls'][setting_name]
         fn = setting.on_publish_factory(obj)
         self.subscribe(topic_name, fn, flags=['pub', 'retain'])
         functions[topic_name] = fn
 
     def _register_capabilities(self, obj, unique_id):
@@ -1379,22 +1387,71 @@
         self._unregister_invoke_callback(obj, unique_id)
         self._registry_remove(unique_id)
         if bool(delete):
             self._parent_remove(unique_id)
         # settings unsubscribe handled by _unregister_functions
         self._unregister_functions(obj, unique_id)
         self._cmd_topic_remove({'topic': instance_topic_name})  # skip undo, do not want instance in undo list
-        delattr(obj, _PUBSUB_ATTR)
-        # obj.__dict__[_PUBSUB_ATTR].clear()
+        if isinstance(obj, type):
+            self._unregister_class_settings(obj)
+        delattr(obj, _pubsub_attr(obj))
         del obj.unique_id
         del obj.topic
         del obj.pubsub
         if bool(delete):
             self._unregister_delete(obj, unique_id)
 
+    def _unregister_class_settings(self, cls):
+        attr = cls.__dict__[_PUBSUB_CLS_ATTR]
+        for setting, v in attr['setting_cls'].items():
+            if v.item is not None:
+                setattr(cls, setting, v.item)
+
+    @_immediate
+    def capabilities_append(self, spec, capabilities):
+        """Dynamically add new capabilities to a registered instance.
+
+        :param spec: The target instance, topic name or unique id.
+        :param capabilities: The list of capabilities to add.
+        """
+        obj = get_instance(spec)
+        unique_id = get_unique_id(obj)
+        obj_caps = getattr(obj, 'CAPABILITIES', [])
+        capabilities = [str(c) for c in capabilities]
+        existing_capabilities = self.enumerate(REGISTRY_MANAGER_TOPICS.CAPABILITIES)
+        for capability in capabilities:
+            if capability in obj_caps:
+                continue
+            if capability not in existing_capabilities:
+                self._log.warning(f'unregistered capability: {capability} in {obj}: SKIP')
+                continue
+            capability_topic = REGISTRY_MANAGER_TOPICS.CAPABILITIES + f'/{capability}'
+            self.publish(f'{capability_topic}/!add', unique_id)
+            obj_caps.append(capability)
+        setattr(obj, 'CAPABILITIES', copy.deepcopy(obj_caps))
+
+    @_immediate
+    def capabilities_remove(self, spec, capabilities):
+        """Dynamically remove capabilities from a registered instance.
+
+        :param spec: The target instance, topic name or unique id.
+        :param capabilities: The list of capabilities to remove.
+        """
+        obj = get_instance(spec)
+        unique_id = get_unique_id(obj)
+        obj_caps = getattr(obj, 'CAPABILITIES', [])
+        capabilities = [str(c) for c in capabilities]
+        for capability in capabilities:
+            if capability not in obj_caps:
+                continue
+            capability_topic = REGISTRY_MANAGER_TOPICS.CAPABILITIES + f'/{capability}'
+            self.publish(f'{capability_topic}/!remove', unique_id)
+            obj_caps.remove(capability)
+        setattr(obj, 'CAPABILITIES', copy.deepcopy(obj_caps))
+
     def _unregister_delete(self, obj, unique_id):
         if not isinstance(obj, type):
             instance_of = self.query(f'{get_topic_name(unique_id)}/instance_of')
             cls_instance = get_instance(instance_of, default=None)
             if cls_instance:
                 instances_topic = f'{get_topic_name(cls_instance)}/instances'
                 instances = self.query(instances_topic)
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/range_tool.py` & `joulescope_ui-1.0.9/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.0.9/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.0.9/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.0.9/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/resources.py` & `joulescope_ui-1.0.9/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/resources.rcc` & `joulescope_ui-1.0.9/joulescope_ui/resources.rcc`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/sanitize.py` & `joulescope_ui-1.0.9/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/shortcuts.py` & `joulescope_ui-1.0.9/joulescope_ui/shortcuts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/software_update.py` & `joulescope_ui-1.0.9/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/README.md` & `joulescope_ui-1.0.9/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .manager import StyleManager, styled_widget
 from .fonts import font_as_qfont, font_as_qss
-from .color_picker import color_as_qcolor
+from .color_picker import color_as_qcolor, color_as_string
 
-__all__ = ['StyleManager', 'styled_widget', 'color_as_qcolor', 'font_as_qfont', 'font_as_qss']
+__all__ = ['StyleManager', 'styled_widget', 'color_as_qcolor', 'color_as_string', 'font_as_qfont', 'font_as_qss']
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/color_picker.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,25 +16,34 @@
 from PySide6 import QtCore, QtGui, QtWidgets
 import re
 
 
 _re_color_pattern = re.compile('#[0-9a-fA-F]+')
 
 
-def color_as_string(color):
+def color_as_string(color, alpha=None):
     if isinstance(color, QtGui.QColor):
         value = f'{color.rgba():08X}'
-        return f'#{value[2:]}{value[:2]}'  # convert AARRGGBB to RRGGBBAA
+        color = f'#{value[2:]}{value[:2]}'  # convert AARRGGBB to RRGGBBAA
     elif isinstance(color, str):
-        return color
+        pass
     else:
         raise ValueError(f'Invalid color type: {type(color)}')
+    if alpha is not None:
+        if isinstance(alpha, str):
+            opacity = int(alpha, 0)
+        elif isinstance(alpha, float):
+            opacity = int(alpha * 255)
+        color = f'{color[:-2]}{alpha:02x}'
+    return color
 
 
-def color_as_qcolor(color):
+def color_as_qcolor(color, alpha=None):
+    if alpha is not None:
+        color = color_as_string(color, alpha)
     if isinstance(color, str):
         clen = len(color)
         if clen == 9:
             color = f'#{color[7:]}{color[1:7]}'  # convert RRGGBBAA to AARRGGBB
         elif clen != 7:
             raise ValueError(f'Invalid color {color}')
         return QtGui.QColor(color)
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.0.9/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.0.9/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.0.9/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/styles/js1/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/js1/tabs_menu.svg` & `joulescope_ui-1.0.9/joulescope_ui/styles/js1/tabs_menu.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.0.9/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.0.9/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/manager.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,16 +277,15 @@
         cls_mirror = True
         cls = pubsub_singleton.query('registry/view/instance')
     else:
         cls_mirror = False
         cls = obj.__class__
     path = os.path.join(path, str_to_filename(obj.unique_id))
     if hasattr(cls, 'unique_id'):
-        if getattr(cls, '_style_cls', None) is None:
-            _render_cls(cls, theme, color_scheme, font_scheme)
+        _render_cls(cls, theme, color_scheme, font_scheme)
         style_cls = cls._style_cls
         if cls_mirror:
             obj.__class__._style_cls = style_cls
         style_vars = style_cls['vars']
     else:
         style_vars = {}
     parent = pubsub_singleton.query(f'{get_topic_name(obj)}/parent', default=None)
@@ -353,20 +352,23 @@
         obj = get_instance(value)
         if isinstance(obj, type):
             objs = _objs_in_view()
             for child in pubsub_singleton.query(f'{get_topic_name(obj)}/children'):
                 if child in objs:
                     self.on_action_render(child)
             return
-        theme = self.pubsub.query('registry/style/settings/theme', default='js1')
-        color_scheme = self.pubsub.query('registry/style/settings/color_scheme', default='dark')
-        font_scheme = self.pubsub.query('registry/style/settings/font_scheme', default='js1')
+        active_view = self.pubsub.query('registry/view/settings/active', default='view')
+        active_view_topic = get_topic_name(active_view)
+        theme = self.pubsub.query(f'{active_view_topic}/settings/theme', default='js1')
+        color_scheme = self.pubsub.query(f'{active_view_topic}/settings/color_scheme', default='dark')
+        font_scheme = self.pubsub.query(f'{active_view_topic}/settings/font_scheme', default='js1')
         is_styled = _render_obj(obj, self.path, theme, color_scheme, font_scheme)
         children = self.pubsub.query(f'{get_topic_name(obj)}/children', default=[])
-        _log.info('rendered %s in %.3f', value, time.time() - t_start)
+        _log.info('rendered %s [theme=%s, color_scheme=%s, font_scheme=%s], in %.3f',
+                  value, theme, color_scheme, font_scheme, time.time() - t_start)
         for child in children:
             self._render(child)
         if is_styled:
             stylesheet = obj.style_obj['templates'].get('style.qss')
             if obj.unique_id.startswith('view:'):
                 obj = self.pubsub.query('registry/ui/instance')
             if stylesheet is not None and stylesheet != obj.styleSheet():
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.0.9/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.0.9/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_pubsub_registry.py`

 * *Files 19% similar despite different names*

```diff
@@ -267,96 +267,190 @@
         self.p.register(c)
         c.calls.clear()
         self.p.publish(f'registry/{c.unique_id}/actions/!view1', 'v1')
         self.p.publish(f'registry/{c.unique_id}/actions/!view2', 'v2')
         self.assertEqual([['sub_action_view1', 'v1'], ['action_view2', 'v2']], c.calls)
 
 
-class SimpleClass:
+class SettingsClass:
 
     SETTINGS = {
         'name': {
             'dtype': 'str',
             'brief': 'The name of this instance',
             'default': 'SimpleClass',
         },
         'param1': {
             'dtype': 'str',
             'brief': 'My first simple parameter',
-            'default': 'param1_default',
+            'default': 'param1_default_in_settings',
         },
         'param2': {
             'dtype': 'str',
             'brief': 'My second parameter with existing getter/setter',
             'default': 'param2_default',
         },
         'param3': {
             'dtype': 'str',
             'brief': 'My third parameter with no defs',
             'default': 'param3_default',
         },
+        'param4': {
+            'dtype': 'str',
+            'brief': 'My fourth parameter with function',
+            'default': 'param4_default',
+        },
     }
 
     def __init__(self):
         self.name = 'instance name'         # assignment ignored, but makes IDEs happy
         self.param1 = 'instance param1'     # assignment ignored, but makes IDEs happy
-        self._param2 = 'instance param2'    # assignment ignored, but makes IDEs happy
+        self.param2_value = 'instance param2'    # assignment ignored, but makes IDEs happy
+        self.param4_value = 'instance param4'
         # param3 not defined here, generated automatically
 
     @property
     def param2(self):
-        return self._param2
+        return self.param2_value
 
     @param2.setter
     def param2(self, value):
-        self._param2 = value
+        self.param2_value = value
+
+    def on_setting_param4(self, value):
+        self.param4_value = value
+
+
+class TestRegistryClassSettings(unittest.TestCase):
 
+    def test_settings(self):
+        p = PubSub()
+        calls = []
+        p.registry_initialize()
+        p.register(SettingsClass)
+
+        for iteration in range(5):
+            with self.subTest(iteration=iteration):
+                if iteration >= 3:
+                    p.unregister(SettingsClass, delete=(iteration == 4))
+                    p.register(SettingsClass)
+
+                # change class default topic
+                param1_cls_topic = f'registry/{SettingsClass.unique_id}/settings/param1'
+                p.publish(param1_cls_topic, 'param1_default')
+
+                obj = SettingsClass()
+                p.register(obj, 'obj')
+                prefix = f'registry/{obj.unique_id}/settings'
+
+                def on_value(topic, value):
+                    calls.append([topic, value])
+
+                if iteration in [0, 2]:
+                    self.assertEqual('param1_default', obj.param1)
+                    self.assertEqual('param2_default', obj.param2)
+                    self.assertEqual('param2_default', obj.param2_value)
+                    self.assertEqual('param3_default', obj.param3)
+                    self.assertEqual('param4_default', obj.param4_value)
+                else:
+                    self.assertEqual('1', obj.param1)
+                    self.assertEqual('2', obj.param2)
+                    self.assertEqual('2', obj.param2_value)
+                    self.assertEqual('3', obj.param3)
+                    self.assertEqual('4', obj.param4_value)
+
+                for i in range(1, 5):
+                    self.assertEqual(getattr(obj, f'param{i}'), p.query(f'{prefix}/param{i}'))
+
+                # instance
+                p.subscribe(prefix, on_value, ['pub'])
+                self.assertEqual([], calls)
+                obj.param1 = 'p1'
+                obj.param2 = 'p2'
+                obj.param3 = 'p3'
+                obj.param4 = 'p4'
+                expect = [
+                    [f'{prefix}/param1', 'p1'],
+                    [f'{prefix}/param2', 'p2'],
+                    [f'{prefix}/param3', 'p3'],
+                    [f'{prefix}/param4', 'p4'],
+                ]
+                self.assertEqual(expect, calls)
+                calls.clear()
+
+                # Set from pubsub
+                p.publish(f'{prefix}/param1', 'v1')
+                p.publish(f'{prefix}/param2', 'v2')
+                p.publish(f'{prefix}/param3', 'v3')
+                p.publish(f'{prefix}/param4', 'v4')
+                self.assertEqual('v1', obj.param1)
+                self.assertEqual('v2', obj.param2_value)
+                self.assertEqual('v3', obj.param3)
+                self.assertEqual('v4', obj.param4_value)
+
+                # Set from instance
+                obj.param1 = '1'
+                obj.param2 = '2'
+                obj.param3 = '3'
+                obj.param4 = '4'
+                self.assertEqual('1', p.query(f'{prefix}/param1'))
+                self.assertEqual('2', p.query(f'{prefix}/param2'))
+                self.assertEqual('2', obj.param2_value)
+                self.assertEqual('3', p.query(f'{prefix}/param3'))
+                self.assertEqual('4', p.query(f'{prefix}/param4'))
+                self.assertEqual('4', obj.param4_value)
+
+                p.unregister(obj, delete=(iteration == 1))
+                calls.clear()
+                obj.param1 = 'no_pub'
+                self.assertEqual([], calls)
+                p.unsubscribe(prefix, on_value)
+
+
+class DynamicCapabilities:
+    CAPABILITIES = ['cls']
+
+    def __init__(self):
+        self.CAPABILITIES = ['obj']
 
-class TestRegistryForSimpleClass(unittest.TestCase):
+
+class TestDynamicCapabilities(unittest.TestCase):
 
     def setUp(self):
+        self.calls = []
         self.p = PubSub()
         self.p.registry_initialize()
-        self.calls = []
-
-    def teardown(self):
-        self.p.unregister(SimpleClass)
+        for cap in ['cls', 'obj', '1', '2', '3']:
+            self.p.register_capability(cap)
+            self.p.subscribe(f'registry_manager/capabilities/{cap}/list', self.on_cap_list, ['pub'])
+
+    def tearDown(self) -> None:
+        pass
+
+    def on_cap_list(self, topic, value):
+        self.calls.append((topic, value))
+
+    def test_static(self):
+        self.p.register(DynamicCapabilities)
+        self.assertEqual([('registry_manager/capabilities/cls/list', ['DynamicCapabilities'])], self.calls)
+        self.calls.clear()
+        obj = DynamicCapabilities()
 
-    def on_value(self, topic, value):
-        self.calls.append([topic, value])
+        self.p.register(obj, 'caps')
+        self.assertEqual([('registry_manager/capabilities/obj/list', ['caps'])], self.calls)
+        self.calls.clear()
 
-    def test_settings_simple(self):
-        self.p.register(SimpleClass)
-        param1_cls_topic = f'registry/{SimpleClass.unique_id}/settings/param1'
-        self.assertEqual('param1_default', self.p.query(param1_cls_topic))
-        self.p.publish(param1_cls_topic, 'new_value')
-
-        # instance
-        obj = SimpleClass()
-        self.p.register(obj)
-        prefix = f'registry/{obj.unique_id}/settings'
-        self.p.subscribe(prefix, self.on_value, ['pub'])
-        self.assertEqual('new_value', obj.param1)
-        self.assertEqual('param2_default', obj.param2)
-        self.assertEqual('param3_default', obj.param3)
-        self.assertEqual([], self.calls)
-        obj.param1 = 'p1'
-        obj.param2 = 'p2'
-        obj.param3 = 'p3'
+        self.p.capabilities_append(obj, ['1', '2'])
         expect = [
-            [f'{prefix}/param1', 'p1'],
-            [f'{prefix}/param2', 'p2'],
-            [f'{prefix}/param3', 'p3']
+            ('registry_manager/capabilities/1/list', ['caps']),
+            ('registry_manager/capabilities/2/list', ['caps'])
         ]
         self.assertEqual(expect, self.calls)
         self.calls.clear()
-        self.p.publish(f'{prefix}/param1', 'v1')
-        self.p.publish(f'{prefix}/param2', 'v2')
-        self.p.publish(f'{prefix}/param3', 'v3')
-        self.assertEqual('v1', obj.param1)
-        self.assertEqual('v2', obj.param2)
-        self.assertEqual('v3', obj.param3)
 
-        self.p.unregister(obj)
+        self.p.capabilities_remove(obj, ['1'])
+        self.assertEqual([('registry_manager/capabilities/1/list', [])], self.calls)
+        self.calls.clear()
+
+        self.p.capabilities_append(obj, ['1'])
+        self.assertEqual([('registry_manager/capabilities/1/list', ['caps'])], self.calls)
         self.calls.clear()
-        obj.param1 = 'no_pub'
-        self.assertEqual([], self.calls)
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/test/test_units.py` & `joulescope_ui-1.0.9/joulescope_ui/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/time_map.py` & `joulescope_ui-1.0.9/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/tooltip.py` & `joulescope_ui-1.0.9/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/ui_util.py` & `joulescope_ui-1.0.9/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/units.py` & `joulescope_ui-1.0.9/joulescope_ui/units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/view.py` & `joulescope_ui-1.0.9/joulescope_ui/view.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,20 +54,22 @@
 
 
 VIEW_SETTINGS = {
     'active': {
         'dtype': 'str',
         'brief': 'The unique_id for the active view instance.',
         'default': '',
+        'flags': ['hide'],
     },
     'theme': {
         'dtype': 'str',
         'brief': N_('The active theme.'),
         'default': 'js1',
         'options': [['js1', N_('Joulescope standard theme')], ['system', N_('System OS-specific theme')]],
+        'flags': ['hide'],
     },
     'color_scheme': {
         'dtype': 'str',
         'brief': N_('The color scheme name.'),
         'default': 'dark',
         'options': [['dark', N_('Dark background')], ['light', N_('Light background')]],
     },
@@ -97,17 +99,14 @@
     SETTINGS = {**VIEW_SETTINGS, **style_settings(N_('View'))}
     _ui = None
     _dock_manager = None
     _active_instance = None
 
     def __init__(self):
         self.name = 'Unnamed view'
-        self._theme = 'js1'
-        self._color_scheme = 'dark'
-        self._colors = None
 
     @property
     def is_active(self):
         return self == View._active_instance
 
     @staticmethod
     def on_cls_setting_active(value):
@@ -151,42 +150,23 @@
         geometry = pubsub_singleton.query(f'{topic}/settings/geometry', default=None)
         if ui is not None and geometry is not None:
             ui.restoreGeometry(geometry)
         pubsub_singleton.publish(style_enable_topic, True)
         view._render()
         _log.info('active view %s: setup done', view.unique_id)
 
-    @property
-    def theme(self):
-        return self._theme
-
-    @theme.setter
-    def theme(self, value):
-        self._theme = value
+    def on_setting_theme(self):
         if self.is_active:
             self._render()
 
-    @property
-    def color_scheme(self):
-        return self._color_scheme
-
-    @color_scheme.setter
-    def color_scheme(self, value):
-        self._color_scheme = value
-        self._colors = None
+    def on_setting_color_scheme(self):
         if self.is_active:
             self._render()
 
-    @property
-    def colors(self):
-        return self.colors
-
-    @colors.setter
-    def colors(self, value):
-        self._colors = value
+    def on_setting_colors(self):
         if self.is_active:
             self._render()
 
     def on_action_widget_open(self, value):
         """Create a widget, possibly reusing existing settings.
 
         :param value: One of several options:
@@ -328,11 +308,11 @@
     @staticmethod
     def on_cls_action_ui_connect(value):
         """Connect the UI to the widget"""
         View._ui = value['ui']
         View._dock_manager = value['dock_manager']
 
     def _render(self):
-        pubsub_singleton.publish('registry/style/actions/!render', get_unique_id(self))
+        pubsub_singleton.publish('registry/style/actions/!render', None)
 
 
 register(View, 'view')
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widget_tools.py` & `joulescope_ui-1.0.9/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 from .accumulator import AccumulatorWidget
 from .device_control import DeviceControlWidget
 # from .example import ExampleWidget
 from .memory import MemoryWidget
 from .hamburger import HamburgerWidget
 from .help import HelpWidget
 from .progress_bar import ProgressBarWidget
+from .record_status import RecordStatusWidget
 from .sidebar import SideBar
 from .settings import SettingsWidget
 from .signal_record import SignalRecordConfigWidget, SignalRecord
 from .statistics_record import StatisticsRecordConfigWidget, StatisticsRecord
 from .value import ValueWidget
 from .waveform import WaveformWidget
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/accumulator_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/accumulator_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/accumulator/styles/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/widgets/accumulator/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,25 @@
                 self._device_remove(unique_id)
         for unique_id in value:
             if unique_id not in self._device_widgets:
                 self._device_add(unique_id)
 
     def _device_remove(self, unique_id):
         self._log.info('remove %s', unique_id)
+        if '-UPDATER' in unique_id:
+            return  # todo
         w = self._device_widgets.pop(unique_id)
         self._layout.removeWidget(w)
         w.close()
         w.deleteLater()
 
     def _device_add(self, unique_id):
         self._log.info('add %s', unique_id)
+        if '-UPDATER' in unique_id:
+            return  # todo
         w = Js220CtrlWidget(self, unique_id)
         w.expanded = True
         self._device_widgets[unique_id] = w
         self._layout.insertWidget(self._layout.count() - 1, w)
 
     def closeEvent(self, event):
         for topic, fn in self._subscribers:
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     def _reset_to_defaults(self, checked):
         self._log.info('reset to defaults')
         topic_base = f'{get_topic_name(self.unique_id)}/settings'
         # disable all streaming
         for name in self._DEVICE_SETTINGS.keys():
             if name.endswith('/enable'):
                 pubsub_singleton.publish(f'{topic_base}/{name}', False)
+        pubsub_singleton.publish(f'{topic_base}/state_req', 0)
         for name, meta in self._DEVICE_SETTINGS.items():
             meta = Metadata(meta)
             value = meta.default
             if name == 'name':
                 value = self.unique_id
             pubsub_singleton.publish(f'{topic_base}/{name}', value)
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,31 +173,35 @@
             default = options[values.index(meta.default)]
         else:
             default = meta.default
         comboBoxConfig(widget, options, default)
         widget.currentIndexChanged.connect(lambda idx: pubsub_singleton.publish(topic, options[idx]))
 
         def handle(v):
-            if isinstance(v, str):
-                comboBoxSelectItemByText(widget, v, block=True)
-            elif isinstance(v, int):
+            if v in values:
                 widget.setCurrentIndex(values.index(v))
+            elif v in options:
+                widget.setCurrentIndex(options.index(v))
+            else:
+                raise ValueError(f'Unable to match {v} in {values} or {options}')
 
         self._subscribe(topic, handle)
         return widget
 
 
 class ColorEditorWidget(_GridWidget):
 
     def __init__(self, parent=None):
         self._colors = None
         self._obj = None
         self._topic = None
         self._log = logging.getLogger(__name__ + '.color')
-        self._color_scheme = pubsub_singleton.query('registry/style/settings/color_scheme', default='dark')
+        active_view = pubsub_singleton.query('registry/view/settings/active', default='view')
+        active_view_topic = get_topic_name(active_view)
+        self._color_scheme = pubsub_singleton.query(f'{active_view_topic}/settings/color_scheme', default='dark')
         super().__init__(parent)
         self.setObjectName('color_editor_widget')
         self._color_widgets = []
 
     def _on_change(self, name, color):
         if len(color) == 7:
             color += 'ff'
@@ -247,15 +251,15 @@
         cls = obj.__class__
         colors = copy.deepcopy(cls._style_cls['load']['colors'][self._color_scheme])
         cls_colors = pubsub_singleton.query(f'{get_topic_name(obj.__class__)}/settings/colors')
         if cls_colors is not None:
             for color_name, color_value in cls_colors[self._color_scheme].items():
                 colors[color_name] = color_value
         if not isinstance(obj, type):
-            if obj.colors is not None:
+            if obj.colors is not None and obj.colors.get(self._color_scheme) is not None:
                 for key, value in obj.colors[self._color_scheme].items():
                     colors[key] = value
         self._colors = colors
 
         name_label = QtWidgets.QLabel(N_('Name'), self)
         self._grid.addWidget(name_label, 0, 0, 1, 1)
         self._widgets.append(name_label)
@@ -311,15 +315,17 @@
 class FontEditorWidget(_GridWidget):
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self._fonts = None
         self._obj = None
         self._topic = None
-        self._font_scheme = pubsub_singleton.query('registry/style/settings/font_scheme', default='js1')
+        active_view = pubsub_singleton.query('registry/view/settings/active', default='view')
+        active_view_topic = get_topic_name(active_view)
+        self._font_scheme = pubsub_singleton.query(f'{active_view_topic}/settings/font_scheme', default='js1')
         self._log = logging.getLogger(__name__ + '.font')
         self.setObjectName('font_editor_widget')
 
     @property
     def object(self):
         return self._obj
 
@@ -427,18 +433,21 @@
 
         for row, (name, value) in enumerate(self._entries.items()):
             name_label = QtWidgets.QLabel(name, self)
             self._grid.addWidget(name_label, row + 1, 0, 1, 1)
             self._widgets.append(name_label)
             w = QtWidgets.QLineEdit(self)
             w.setText(value)
-            w.changed.connect(self._on_change)  # todo
+            self._connect(name, w)
             self._grid.addWidget(w, row + 1, 1, 1, 1)
             self._widgets.append(w)
 
+    def _connect(self, name, w):
+        w.textChanged.connect(lambda value: self._on_change(name, value))
+
     def _on_change(self, name, value):
         self._entries[name] = value
         pubsub_singleton.publish(f'{self._topic}/settings/style_defines', dict(self._entries))
 
 
 def _class_items(capability):
     entries = []
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/value/value_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,23 +534,30 @@
 
         self.mousePressEvent = self._on_mousePressEvent
 
     def on_pubsub_register(self):
         for topic, fn in self._subscribers:
             pubsub_singleton.subscribe(topic, fn, ['pub', 'retain'])
 
-    def closeEvent(self, event):
+    def on_pubsub_unregister(self):
+        self._pubsub_disconnect()
+
+    def _pubsub_disconnect(self):
         self._disconnect()
+        for topic, fn in self._subscribers:
+            pubsub_singleton.unsubscribe(topic, fn)
+        self._subscribers.clear()
         self._statistics = None
+
+    def closeEvent(self, event):
+        self._pubsub_disconnect()
         return super().closeEvent(event)
 
     def _disconnect(self):
         pubsub_singleton.unsubscribe_all(self._on_statistics_fn)
-        for topic, fn in self._subscribers:
-            pubsub_singleton.unsubscribe(topic, fn)
         self.repaint()
 
     @property
     def source(self):
         source = self._statistics_stream_source
         if source in [None, 'default']:
             source = self._default_statistics_stream_source
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,24 +6,22 @@
 waveform.grid_major = #ffffff40
 waveform.grid_minor = #80808010
 waveform.plot_separator = #B0B0ff60
 waveform.plot_border = #ffffff80
 
 waveform.hover = #e0e0e0a0
 
-waveform.summary_missing = #C0C04030
 waveform.summary_trace = #ffff00ff
-waveform.summary_min_max_fill = #FF404060
-waveform.summary_view = #4050FF80
+waveform.summary_view = #1260a080
 
-waveform.plot1_trace = #ffff00ff
-waveform.plot1_min_max_trace = #FF4040A0
-waveform.plot1_min_max_fill = #FF404060
-waveform.plot1_std_fill = #80FF4040
-waveform.plot1_missing = #C0C04030
+# Use yellow, cyan, magenta, green
+waveform.trace1 = #ffff00ff
+waveform.trace2 = #00ffffff
+waveform.trace3 = #ff00ffff
+waveform.trace4 = #00ff00ff
 
 waveform.marker_label = #101010A0
 waveform.marker1 = #40c040A0
 waveform.marker2 = #4080c8A0
 waveform.marker3 = #a040a0A0
 waveform.marker4 = #40a0a0A0
 waveform.marker5 = #e29740A0
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files 16% similar despite different names*

```diff
@@ -62,7 +62,24 @@
 QPushButton#pin_right:enabled       { image: url("{% path %}/pin_right_enabled.svg"); }
 QPushButton#pin_right:enabled:hover { image: url("{% path %}/pin_right_hover.svg"); }
 QPushButton#pin_right:checked       { image: url("{% path %}/pin_right_pressed.svg"); }
 
 QPushButton#y_zoom_all:disabled      { image: url("{% path %}/y_zoom_all_disabled.svg"); }
 QPushButton#y_zoom_all:enabled       { image: url("{% path %}/y_zoom_all_enabled.svg"); }
 QPushButton#y_zoom_all:enabled:hover { image: url("{% path %}/y_zoom_all_hover.svg"); }
+
+
+QLabel#WaveformSingleSourceColor_0 {
+    background-color: {% waveform.trace1 %};
+}
+
+QLabel#WaveformSingleSourceColor_1 {
+    background-color: {% waveform.trace2 %};
+}
+
+QLabel#WaveformSingleSourceColor_2 {
+    background-color: {% waveform.trace3 %};
+}
+
+QLabel#WaveformSingleSourceColor_3 {
+    background-color: {% waveform.trace4 %};
+}
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         self._signal_layout.setContentsMargins(3, 0, 3, 0)
         self._signal_layout.setSpacing(3)
         self._signal_holder.setLayout(self._signal_layout)
 
         self._signals = {}
         for signal in _SIGNALS:
             self._add_signal(signal)
-#
+
         self._spacer = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding,
                                              QtWidgets.QSizePolicy.Minimum)
         self._layout.addItem(self._spacer)
 
     def _subscribe(self, topic, fn, flags=None):
         self._pubsub.subscribe(topic, fn, flags)
         self._subscribe_entries.append((topic, fn))
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.0.9/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore, QtOpenGLWidgets, QtOpenGL
 from OpenGL import GL as gl
 from joulescope_ui import CAPABILITIES, register, pubsub_singleton, N_, get_topic_name, get_instance, time64
 from joulescope_ui.shortcuts import Shortcuts
-from joulescope_ui.styles import styled_widget, color_as_qcolor, font_as_qfont
+from joulescope_ui.styles import styled_widget, color_as_qcolor, color_as_string, font_as_qfont
 from joulescope_ui.widget_tools import settings_action_create
 from .line_segments import PointsF
 from .waveform_control import WaveformControlWidget
 from joulescope_ui.time_map import TimeMap
 import copy
 import logging
 import numpy as np
@@ -530,14 +530,15 @@
         self._mouse_action = None
         self._clipboard_image = None
         self._signals = {}
         self._signals_by_rsp_id = {}
         self._signals_rsp_id_next = 2  # reserve 1 for summary
         self._signals_data = {}
         self._marker_data = {}  # rsp_id -> data,
+        self._subsource_order = []
 
         self._refresh_timer = QtCore.QTimer()
         self._refresh_timer.setTimerType(QtGui.Qt.PreciseTimer)
         self._refresh_timer.timeout.connect(self._on_refresh_timer)
         self._repaint_request = False
         self._fps = {
             'start': time.time(),
@@ -600,15 +601,15 @@
         source = topic.split('/')[1]
         signal = value
         item = (source, signal)
         for plot in self.state['plots']:
             if item in plot['signals']:
                 plot['signals'].remove(item)
         if item in self._signals:
-            self._signals[item]['enabled'] = False
+            del self._signals[item]
         self._repaint_request = True
 
     def is_signal_active(self, source_signal):
         if not self._signals[source_signal]['enabled']:
             return False
         for plot in self.state['plots']:
             if not plot['enabled']:
@@ -1027,37 +1028,79 @@
         y_tick_size = axis_font_metrics.boundingRect('888.888')
 
         statistics_name_size = axis_font_metrics.boundingRect('maxx').width()
         statistics_value_size = axis_font_metrics.boundingRect('+888.888x').width()
         statistics_unit_size = axis_font_metrics.boundingRect('mW').width()
         statistics_size = _MARGIN * 2 + statistics_name_size + statistics_value_size + statistics_unit_size
 
+        trace_alpha = int(v['waveform.trace_alpha'], 0)
+        min_max_trace_alpha = int(v['waveform.min_max_trace_alpha'], 0)
+        min_max_fill_alpha = int(v['waveform.min_max_fill_alpha'], 0)
+        std_fill_alpha = int(v['waveform.std_fill_alpha'], 0)
+        missing_alpha = int(v['waveform.missing_alpha'], 0)
+
+        summary_trace = color_as_string(v['waveform.summary_trace'], alpha=0xff)
+        trace1 = color_as_string(v['waveform.trace1'], alpha=0xff)
+        trace2 = color_as_string(v['waveform.trace2'], alpha=0xff)
+        trace3 = color_as_string(v['waveform.trace3'], alpha=0xff)
+        trace4 = color_as_string(v['waveform.trace4'], alpha=0xff)
+
         self._style_cache = {
             'background_brush': QtGui.QBrush(color_as_qcolor(v['waveform.background'])),
 
             'text_pen': QtGui.QPen(color_as_qcolor(v['waveform.text_foreground'])),
             'text_brush': QtGui.QBrush(color_as_qcolor(v['waveform.text_background'])),
             'grid_major_pen': QtGui.QPen(color_as_qcolor(v['waveform.grid_major'])),
             'grid_minor_pen': QtGui.QPen(color_as_qcolor(v['waveform.grid_minor'])),
             'plot_border_pen': QtGui.QPen(color_as_qcolor(v['waveform.plot_border'])),
             'plot_separator_brush': QtGui.QBrush(color_as_qcolor(v['waveform.plot_separator'])),
 
             'waveform.hover': QBrush(color_as_qcolor(v['waveform.hover'])),
 
-            'summary_missing': QBrush(color_as_qcolor(v['waveform.summary_missing'])),
-            'summary_trace': QPen(color_as_qcolor(v['waveform.summary_trace'])),
-            'summary_min_max_fill': QBrush(color_as_qcolor(v['waveform.summary_min_max_fill'])),
+            'summary_missing': QBrush(color_as_qcolor(summary_trace, alpha=missing_alpha)),
+            'summary_trace': QPen(color_as_qcolor(summary_trace, alpha=trace_alpha)),
+            'summary_min_max_fill': QBrush(color_as_qcolor(summary_trace, alpha=min_max_fill_alpha)),
             'summary_view': QBrush(color_as_qcolor(v['waveform.summary_view'])),
 
-            'plot1_trace': QPen(color_as_qcolor(v['waveform.plot1_trace'])),
-            'plot1_min_max_trace': QPen(color_as_qcolor(v['waveform.plot1_min_max_trace'])),
-            'plot1_min_max_fill_pen': QPen(color_as_qcolor(v['waveform.plot1_min_max_fill'])),
-            'plot1_min_max_fill_brush': QBrush(color_as_qcolor(v['waveform.plot1_min_max_fill'])),
-            'plot1_std_fill': QBrush(color_as_qcolor(v['waveform.plot1_std_fill'])),
-            'plot1_missing': QBrush(color_as_qcolor(v['waveform.plot1_missing'])),
+            'plot_trace': [
+                QPen(color_as_qcolor(trace1, alpha=trace_alpha)),
+                QPen(color_as_qcolor(trace2, alpha=trace_alpha)),
+                QPen(color_as_qcolor(trace3, alpha=trace_alpha)),
+                QPen(color_as_qcolor(trace4, alpha=trace_alpha)),
+            ],
+            'plot_min_max_trace': [
+                QPen(color_as_qcolor(trace1, alpha=min_max_trace_alpha)),
+                QPen(color_as_qcolor(trace2, alpha=min_max_trace_alpha)),
+                QPen(color_as_qcolor(trace3, alpha=min_max_trace_alpha)),
+                QPen(color_as_qcolor(trace4, alpha=min_max_trace_alpha)),
+            ],
+            'plot_min_max_fill_pen': [
+                QPen(color_as_qcolor(trace1, alpha=min_max_fill_alpha)),
+                QPen(color_as_qcolor(trace2, alpha=min_max_fill_alpha)),
+                QPen(color_as_qcolor(trace3, alpha=min_max_fill_alpha)),
+                QPen(color_as_qcolor(trace4, alpha=min_max_fill_alpha)),
+            ],
+            'plot_min_max_fill_brush': [
+                QBrush(color_as_qcolor(trace1, alpha=min_max_fill_alpha)),
+                QBrush(color_as_qcolor(trace2, alpha=min_max_fill_alpha)),
+                QBrush(color_as_qcolor(trace3, alpha=min_max_fill_alpha)),
+                QBrush(color_as_qcolor(trace4, alpha=min_max_fill_alpha)),
+            ],
+            'plot_std_fill': [
+                QBrush(color_as_qcolor(trace1, alpha=std_fill_alpha)),
+                QBrush(color_as_qcolor(trace2, alpha=std_fill_alpha)),
+                QBrush(color_as_qcolor(trace3, alpha=std_fill_alpha)),
+                QBrush(color_as_qcolor(trace4, alpha=std_fill_alpha)),
+            ],
+            'plot_missing': [
+                QBrush(color_as_qcolor(trace1, alpha=missing_alpha)),
+                QBrush(color_as_qcolor(trace2, alpha=missing_alpha)),
+                QBrush(color_as_qcolor(trace3, alpha=missing_alpha)),
+                QBrush(color_as_qcolor(trace4, alpha=missing_alpha)),
+            ],
 
             'axis_font': axis_font,
             'axis_font_metrics': QtGui.QFontMetrics(axis_font),
             'plot_label_size': axis_font_metrics.boundingRect('WW'),
             'y_tick_size': y_tick_size,
             'y_tick_height_pixels_min': 1.5 * y_tick_size.height(),
             'utc_width_pixels': axis_font_metrics.boundingRect('8888-88-88W88:88:88.888888').width(),
@@ -1071,17 +1114,27 @@
 
         for k in range(1, 7):
             c = v[f'waveform.marker{k}']
             self._style_cache[f'marker{k}_pen'] = QPen(color_as_qcolor(c))
             self._style_cache[f'marker{k}_fg'] = QBrush(color_as_qcolor(c))
             self._style_cache[f'marker{k}_bg'] = QBrush(color_as_qcolor(c[:-2] + '20'))
 
-        self._style_cache['plot1_trace'].setWidth(self.trace_width)
+        for trace in self._style_cache['plot_trace']:
+            trace.setWidth(self.trace_width)
         return self._style_cache
 
+    def _subsource_order_update(self):
+        sources = set()
+        for (source_id, signal_id), signal in self._signals.items():
+            if not signal['enabled']:
+                continue
+            subsource = signal_id.split('.')[0]
+            sources.add(f'{source_id}/{subsource}')
+        self._subsource_order = list(sources)
+
     def _plot_range_auto_update(self, plot):
         if plot['range_mode'] != 'auto':
             return
         y_min = []
         y_max = []
         for signal in plot['signals']:
             d = self._signals.get(signal)
@@ -1245,14 +1298,15 @@
         self._draw_background(p, size)
         self._draw_summary(p)
         self._draw_x_axis(p)
         self._x_markers_remove_expired()
         self._draw_markers_background(p)
 
         # Draw each plot
+        self._subsource_order_update()
         for plot in self.state['plots']:
             if plot['enabled']:
                 self._draw_plot(p, plot)
                 self._draw_plot_statistics(p, plot)
         self._draw_spacers(p)
         self._draw_markers(p, size)
         self._draw_hover(p)
@@ -1292,21 +1346,20 @@
 
         xp = self._x_summary_map.time64_to_counter(x)
         p.setClipRect(x0, y0, w, h)
         finite_idx = np.logical_not(np.isnan(d['avg']))
         segment_idx = _idx_to_segments(finite_idx)
 
         p.setPen(self._NO_PEN)
-        p.setBrush(s['plot1_missing'])
         if len(segment_idx) > 1:
             segment_idx_last = segment_idx[0][1]
             for idx_start, idx_stop in segment_idx[1:]:
                 z1 = xp[segment_idx_last]
                 z2 = xp[idx_start]
-                p.drawRect(z1, y0, max(1, z2 - z1), h)
+                p.fillRect(z1, y0, max(1, z2 - z1), h, s['summary_missing'])
                 segment_idx_last = idx_stop
 
         xp_range = np.rint(self._x_summary_map.time64_to_counter(np.array(self.x_range)))
         pr0, pr1 = int(xp_range[0]), int(xp_range[-1])
         pr0, pr1 = max(0, min(pr0, w)), max(0, min(pr1, w))
         p.fillRect(x0 + pr0, y0, max(1, pr1 - pr0), h, s['summary_view'])
 
@@ -1491,32 +1544,34 @@
             s_label = f"{y_grid['unit_prefix']}{plot_units}"
         p.drawText(left, y0 + (h + axis_font_metrics.ascent()) // 2, s_label)
 
         p.setClipRect(x0, y0, w, h)
 
         for signal in plot['signals']:
             d = self._signals.get(signal)
-            if d is None:
+            if d is None or not d['enabled']:
                 continue
             sig_d = self._signals_data.get(signal)
             if sig_d is None:
                 continue
+            subsource = f'{signal[0]}/{signal[1].split(".")[0]}'
+            trace_idx = self._subsource_order.index(subsource)
             d = sig_d['data']
             d_x = self._x_map.time64_to_counter(d['x'])
             if len(d_x) == w:
                 d_x, d_x2 = np.rint(d_x), d_x
                 if np.any(np.abs(d_x - d_x2) > 0.5):
                     self._log.warning('x does not conform to pixels')
                     d_x = d_x2
 
             finite_idx = self._finite_idx(d)
             segment_idx = _idx_to_segments(finite_idx)
 
             p.setPen(self._NO_PEN)
-            p.setBrush(s['plot1_missing'])
+            p.setBrush(s['plot_missing'][trace_idx])
             if len(segment_idx) > 1:
                 segment_idx_last = segment_idx[0][1]
                 for idx_start, idx_stop in segment_idx[1:]:
                     xa = d_x[segment_idx_last]
                     xb = d_x[idx_start]
                     p.drawRect(xa, y0, max(1, xb - xa), h)
                     segment_idx_last = idx_stop
@@ -1524,38 +1579,38 @@
             for idx_start, idx_stop in segment_idx:
                 d_x_segment = d_x[idx_start:idx_stop]
                 d_avg = d['avg'][idx_start:idx_stop]
                 if self.show_min_max and d['min'] is not None and d['max'] is not None:
                     d_y_min = self._y_value_to_pixel(plot, d['min'][idx_start:idx_stop])
                     d_y_max = self._y_value_to_pixel(plot, d['max'][idx_start:idx_stop])
                     if 1 == self.show_min_max:
-                        p.setPen(s['plot1_min_max_trace'])
+                        p.setPen(s['plot_min_max_trace'][trace_idx])
                         segs, nsegs = sig_d['line_min'].set_line(d_x_segment, d_y_min)
                         p.drawPolyline(segs)
                         segs, nsegs = sig_d['line_max'].set_line(d_x_segment, d_y_max)
                         p.drawPolyline(segs)
                     else:
                         segs, nsegs = sig_d['points_min_max'].set_fill(d_x_segment, d_y_min, d_y_max)
-                        p.setPen(s['plot1_min_max_fill_pen'])
-                        p.setBrush(s['plot1_min_max_fill_brush'])
+                        p.setPen(s['plot_min_max_fill_pen'][trace_idx])
+                        p.setBrush(s['plot_min_max_fill_brush'][trace_idx])
                         p.drawPolygon(segs)
                         if 3 == self.show_min_max:
                             d_std = d['std'][idx_start:idx_stop]
                             d_y_std_min = self._y_value_to_pixel(plot, d_avg - d_std)
                             d_y_std_max = self._y_value_to_pixel(plot, d_avg + d_std)
                             d_y_std_min = np.amin(np.vstack([d_y_std_min, d_y_min]), axis=0)
                             d_y_std_max = np.amax(np.vstack([d_y_std_max, d_y_max]), axis=0)
                             segs, nsegs = sig_d['points_std'].set_fill(d_x_segment, d_y_std_min, d_y_std_max)
                             p.setPen(self._NO_PEN)
-                            p.setBrush(s['plot1_std_fill'])
+                            p.setBrush(s['plot_std_fill'][trace_idx])
                             p.drawPolygon(segs)
 
                 d_y = self._y_value_to_pixel(plot, d_avg)
                 segs, nsegs = sig_d['points_avg'].set_line(d_x_segment, d_y)
-                p.setPen(s['plot1_trace'])
+                p.setPen(s['plot_trace'][trace_idx])
                 p.drawPolyline(segs)
 
         p.setBrush(s['text_brush'])
         f_a = s['axis_font_metrics'].ascent()
         for m in plot['y_markers']:
             color_index = ((m['id'] - 1) % 6) + 1
             pen = s[f'marker{color_index}_pen']
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.0.9/joulescope_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope-ui
-Version: 1.0.8
+Version: 1.0.9
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.0.8/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.0.9/joulescope_ui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 joulescope_ui.egg-info/requires.txt
 joulescope_ui.egg-info/top_level.txt
 joulescope_ui/devices/__init__.py
 joulescope_ui/devices/jsdrv/__init__.py
 joulescope_ui/devices/jsdrv/device.py
 joulescope_ui/devices/jsdrv/js110.py
 joulescope_ui/devices/jsdrv/js220.py
+joulescope_ui/devices/jsdrv/js220_updater.py
 joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
 joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
 joulescope_ui/entry_points/__init__.py
 joulescope_ui/entry_points/ui.py
 joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
 joulescope_ui/fonts/Hack/LICENSE.md
 joulescope_ui/fonts/Lato/OFL.txt
@@ -181,14 +182,21 @@
 joulescope_ui/widgets/memory/memory_widget.py
 joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
 joulescope_ui/widgets/memory/styles/color_scheme_light.txt
 joulescope_ui/widgets/memory/styles/index.json
 joulescope_ui/widgets/memory/styles/style.qss
 joulescope_ui/widgets/progress_bar/__init__.py
 joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+joulescope_ui/widgets/record_status/__init__.py
+joulescope_ui/widgets/record_status/record_status_widget.py
+joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+joulescope_ui/widgets/record_status/styles/index.json
+joulescope_ui/widgets/record_status/styles/record.svg
+joulescope_ui/widgets/record_status/styles/style.qss
 joulescope_ui/widgets/settings/__init__.py
 joulescope_ui/widgets/settings/settings_widget.py
 joulescope_ui/widgets/sidebar/__init__.py
 joulescope_ui/widgets/sidebar/sidebar_widget.py
 joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
 joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
 joulescope_ui/widgets/sidebar/styles/device.svg
@@ -215,23 +223,25 @@
 joulescope_ui/widgets/value/styles/color_scheme_light.txt
 joulescope_ui/widgets/value/styles/font_scheme_js1.txt
 joulescope_ui/widgets/value/styles/index.json
 joulescope_ui/widgets/value/styles/style.qss
 joulescope_ui/widgets/waveform/__init__.py
 joulescope_ui/widgets/waveform/line_segments.py
 joulescope_ui/widgets/waveform/waveform_control.py
+joulescope_ui/widgets/waveform/waveform_source_widget.py
 joulescope_ui/widgets/waveform/waveform_widget.py
 joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
 joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
 joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
 joulescope_ui/widgets/waveform/styles/index.json
 joulescope_ui/widgets/waveform/styles/marker_add1.svg
 joulescope_ui/widgets/waveform/styles/marker_add2.svg
 joulescope_ui/widgets/waveform/styles/marker_clear.svg
 joulescope_ui/widgets/waveform/styles/pin_left.svg
 joulescope_ui/widgets/waveform/styles/pin_right.svg
 joulescope_ui/widgets/waveform/styles/style.qss
+joulescope_ui/widgets/waveform/styles/style_defines.txt
 joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
 joulescope_ui/widgets/waveform/styles/zoom_all.svg
 joulescope_ui/widgets/waveform/styles/zoom_in.svg
 joulescope_ui/widgets/waveform/styles/zoom_out.svg
 joulescope_ui/widgets/waveform/test/__init__.py
```

### Comparing `joulescope_ui-1.0.8/setup.py` & `joulescope_ui-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 import platform
 import sys
 import subprocess
 import shutil
 
 
-JOULESCOPE_DRIVER_VERSION_MIN = '1.3.2'  # also update requirements.txt
+JOULESCOPE_DRIVER_VERSION_MIN = '1.3.3'  # also update requirements.txt
 JOULESCOPE_VERSION_MIN = '1.1.3'         # also update requirements.txt
 MYPATH = os.path.abspath(os.path.dirname(__file__))
 VERSION_PATH = os.path.join(MYPATH, 'joulescope_ui', 'version.py')
 
 
 def qt_rcc_path():
     # As of PySide 5.15.0, the pySide6-rcc executable ignores the --binary flag
```

