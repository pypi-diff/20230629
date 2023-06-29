# Comparing `tmp/ubiquity-student-1.1.0.tar.gz` & `tmp/ubiquity-student-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiquity-student-1.1.0.tar", last modified: Wed Jun 28 07:59:33 2023, max compression
+gzip compressed data, was "ubiquity-student-1.1.1.tar", last modified: Thu Jun 29 08:50:52 2023, max compression
```

## Comparing `ubiquity-student-1.1.0.tar` & `ubiquity-student-1.1.1.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.066023 ubiquity-student-1.1.0/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2516 2023-06-28 07:59:33.066023 ubiquity-student-1.1.0/PKG-INFO
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     1554 2022-06-20 11:36:26.000000 ubiquity-student-1.1.0/README.md
--rw-rw-r--   0 houchard  (1000) houchard  (1000)       38 2023-06-28 07:59:33.066023 ubiquity-student-1.1.0/setup.cfg
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2993 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/setup.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.042023 ubiquity-student-1.1.0/src/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)        5 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/VERSION
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      854 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/__init__.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     8936 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/argument_parser.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/controllers/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/controllers/__init__.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     8795 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/controllers/config_file.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)    10841 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/controllers/main_controller.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     6247 2023-05-24 06:47:03.000000 ubiquity-student-1.1.0/src/ubiquity/controllers/worker.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/images/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2139 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/images/ubiquity_icon.png
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.042023 ubiquity-student-1.1.0/src/ubiquity/locale/
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.042023 ubiquity-student-1.1.0/src/ubiquity/locale/fr/
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     6756 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/locale/fr/LC_MESSAGES/ubiquity-student.mo
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     5594 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/model.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     3348 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/ubiquity_student.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2080 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/version.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/__init__.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/cui/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/cui/__init__.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     8398 2023-01-12 13:40:26.000000 ubiquity-student-1.1.0/src/ubiquity/views/cui/main_view.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/gui/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/__init__.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      995 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/__init__.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2001 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/about.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2000 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/base.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     1901 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/choice.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2395 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/confirm.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     3606 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/form.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     6555 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/open.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     3320 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/preference.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     4862 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/main_view.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     6535 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/menu_bar.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2368 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/__init__.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     1221 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/base.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     1253 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sun_valley_dark.py
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     1259 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sun_valley_light.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     1063 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/LICENSE
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)     1383 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/__init__.py
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)     2961 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.046023 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.054023 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      270 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-down.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      261 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-right.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-up.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      262 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      373 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      363 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      377 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      301 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      276 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      288 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-pressed.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      301 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      245 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      238 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      386 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/card.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      383 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      474 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      460 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      475 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      294 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      362 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      358 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      363 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      312 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      353 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      353 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      129 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/empty.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      273 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      335 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-focus.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      269 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-invalid.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      297 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      337 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook-border.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      186 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      193 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-hor.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      214 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-vert.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      157 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-hor.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      160 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-vert.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      553 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      853 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      786 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      830 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      552 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      602 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      616 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      621 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      724 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      808 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      735 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      771 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      216 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-hor.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      215 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-vert.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      226 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-down.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      254 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-thumb.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      338 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-trough.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      233 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-left.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      227 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-right.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      236 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-up.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      264 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-thumb.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      343 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-trough.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      128 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/separator.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      276 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/sizegrip.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      733 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      945 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      963 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      895 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      623 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      927 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      936 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      859 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      265 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      164 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      319 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-selected.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      295 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      317 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-pressed.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      321 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)    19668 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.062023 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      278 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-down.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      273 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-right.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      285 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-up.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      271 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      374 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      367 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      384 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      326 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      316 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      307 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      306 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      289 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      303 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      238 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      225 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      394 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/card.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      381 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      476 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      467 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      473 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      299 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      365 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      362 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      367 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      334 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      333 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      129 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/empty.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      289 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      331 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-focus.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-invalid.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      308 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      298 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook-border.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      185 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      192 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-hor.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      216 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-vert.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      158 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-hor.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      161 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-vert.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      523 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      837 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      764 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      773 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      521 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      573 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      636 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      576 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      658 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      749 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      675 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      701 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      208 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-hor.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      214 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-vert.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      229 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-down.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      234 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-thumb.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      321 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-trough.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      232 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-left.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      223 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-right.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      237 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-up.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      262 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-thumb.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-trough.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      128 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/separator.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      272 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/sizegrip.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      726 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      867 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      880 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      814 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      590 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      906 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      916 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      857 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      295 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-hover.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      164 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-rest.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      318 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-selected.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      338 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-hover.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)      318 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-pressed.png
--rw-rw-r--   0 houchard  (1000) houchard  (1000)      330 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-rest.png
--rwxrwxr-x   0 houchard  (1000) houchard  (1000)    19846 2022-09-19 07:02:28.000000 ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     6745 2023-06-28 07:49:41.000000 ubiquity-student-1.1.0/src/ubiquity/views/utils.py
-drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-28 07:59:33.066023 ubiquity-student-1.1.0/ubiquity_student.egg-info/
--rw-rw-r--   0 houchard  (1000) houchard  (1000)     2516 2023-06-28 07:59:33.000000 ubiquity-student-1.1.0/ubiquity_student.egg-info/PKG-INFO
--rw-rw-r--   0 houchard  (1000) houchard  (1000)    12313 2023-06-28 07:59:33.000000 ubiquity-student-1.1.0/ubiquity_student.egg-info/SOURCES.txt
--rw-rw-r--   0 houchard  (1000) houchard  (1000)        1 2023-06-28 07:59:33.000000 ubiquity-student-1.1.0/ubiquity_student.egg-info/dependency_links.txt
--rw-rw-r--   0 houchard  (1000) houchard  (1000)       72 2023-06-28 07:59:33.000000 ubiquity-student-1.1.0/ubiquity_student.egg-info/entry_points.txt
--rw-rw-r--   0 houchard  (1000) houchard  (1000)       17 2023-06-28 07:59:33.000000 ubiquity-student-1.1.0/ubiquity_student.egg-info/requires.txt
--rw-rw-r--   0 houchard  (1000) houchard  (1000)        4 2023-06-28 07:59:33.000000 ubiquity-student-1.1.0/ubiquity_student.egg-info/top_level.txt
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.032840 ubiquity-student-1.1.1/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2516 2023-06-29 08:50:52.032840 ubiquity-student-1.1.1/PKG-INFO
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1554 2022-06-20 11:36:26.000000 ubiquity-student-1.1.1/README.md
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)       38 2023-06-29 08:50:52.032840 ubiquity-student-1.1.1/setup.cfg
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2993 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/setup.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.008840 ubiquity-student-1.1.1/src/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)        5 2023-06-29 08:47:04.000000 ubiquity-student-1.1.1/src/VERSION
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      854 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     8936 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/argument_parser.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/controllers/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/controllers/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     8795 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/controllers/config_file.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)    10841 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/controllers/main_controller.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6247 2023-06-29 08:42:31.000000 ubiquity-student-1.1.1/src/ubiquity/controllers/worker.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/images/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2139 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/images/ubiquity_icon.png
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.008840 ubiquity-student-1.1.1/src/ubiquity/locale/
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.008840 ubiquity-student-1.1.1/src/ubiquity/locale/fr/
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6756 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/locale/fr/LC_MESSAGES/ubiquity-student.mo
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     5594 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/model.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     3348 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/ubiquity_student.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2080 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/version.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/__init__.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/cui/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/cui/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     8398 2023-01-12 13:40:26.000000 ubiquity-student-1.1.1/src/ubiquity/views/cui/main_view.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/gui/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      757 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/__init__.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      995 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2001 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/about.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2000 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/base.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1901 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/choice.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2395 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/confirm.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     3606 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/form.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6555 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/open.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     3320 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/preference.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     4862 2023-06-29 08:42:31.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/main_view.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6535 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/menu_bar.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2368 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/__init__.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1221 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/base.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1253 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sun_valley_dark.py
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1259 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sun_valley_light.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     1063 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/LICENSE
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)     1383 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/__init__.py
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)     2961 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.012840 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.024840 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      270 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      261 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-right.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/arrow-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      262 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      373 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      363 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      377 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-accent-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      274 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-close-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      301 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      276 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      288 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      301 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      245 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      238 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/button-titlebar-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      386 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/card.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      383 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      474 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      460 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      475 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      294 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      362 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      358 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      363 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-tri-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      312 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      353 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      353 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/check-unsel-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      129 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/empty.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      273 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      335 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-focus.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      269 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-invalid.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      297 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/entry-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      337 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook-border.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      186 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/notebook.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      193 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      214 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-pbar-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      157 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      160 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/progress-trough-vert.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      553 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      853 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      786 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      830 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      552 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      602 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      616 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      621 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      724 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      808 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      735 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      771 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      216 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      215 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-trough-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      226 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      254 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-thumb.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      338 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-hor-trough.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      233 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-left.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      227 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-right.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      236 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      264 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-thumb.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      343 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scroll-vert-trough.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      128 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/separator.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      276 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/sizegrip.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      733 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      945 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      963 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      895 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      623 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      927 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      936 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      859 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      265 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      164 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      319 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/tab-selected.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      295 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      317 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      321 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/treeheading-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)    19668 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.032840 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      278 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      273 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-right.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      285 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/arrow-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      271 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      374 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      367 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      384 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-accent-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      326 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      316 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-close-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      307 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      306 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      289 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      303 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      238 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      225 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/button-titlebar-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      394 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/card.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      381 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      476 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      467 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      473 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      299 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      365 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      362 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      367 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-tri-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      334 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      333 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/check-unsel-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      129 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/empty.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      289 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      331 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-focus.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      302 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-invalid.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      308 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/entry-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      298 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook-border.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      185 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/notebook.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      192 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      216 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-pbar-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      158 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      161 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/progress-trough-vert.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      523 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      837 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      764 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      773 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      521 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      573 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      636 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      576 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      658 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      749 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      675 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      701 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      208 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-hor.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      214 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-trough-vert.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      229 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-down.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      234 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-thumb.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      321 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-hor-trough.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      232 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-left.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      223 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-right.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      237 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-up.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      262 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-thumb.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      324 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scroll-vert-trough.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      128 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/separator.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      272 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/sizegrip.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      726 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      867 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      880 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      814 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      590 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      906 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      916 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      857 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      295 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-hover.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      164 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-rest.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      318 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/tab-selected.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      338 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-hover.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)      318 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-pressed.png
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)      330 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/treeheading-rest.png
+-rwxrwxr-x   0 houchard  (1000) houchard  (1000)    19846 2022-09-19 07:02:28.000000 ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     6745 2023-06-28 07:49:41.000000 ubiquity-student-1.1.1/src/ubiquity/views/utils.py
+drwxrwxr-x   0 houchard  (1000) houchard  (1000)        0 2023-06-29 08:50:52.032840 ubiquity-student-1.1.1/ubiquity_student.egg-info/
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)     2516 2023-06-29 08:50:51.000000 ubiquity-student-1.1.1/ubiquity_student.egg-info/PKG-INFO
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)    12313 2023-06-29 08:50:52.000000 ubiquity-student-1.1.1/ubiquity_student.egg-info/SOURCES.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)        1 2023-06-29 08:50:51.000000 ubiquity-student-1.1.1/ubiquity_student.egg-info/dependency_links.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)       72 2023-06-29 08:50:51.000000 ubiquity-student-1.1.1/ubiquity_student.egg-info/entry_points.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)       17 2023-06-29 08:50:51.000000 ubiquity-student-1.1.1/ubiquity_student.egg-info/requires.txt
+-rw-rw-r--   0 houchard  (1000) houchard  (1000)        4 2023-06-29 08:50:51.000000 ubiquity-student-1.1.1/ubiquity_student.egg-info/top_level.txt
```

### Comparing `ubiquity-student-1.1.0/PKG-INFO` & `ubiquity-student-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiquity-student
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ubiquity permet le suivi de TP de développement informatique
 Home-page: https://gitlab.insa-rouen.fr/cip/ubiquity
 Download-URL: https://gitlab.insa-rouen.fr/cip/ubiquity/-/tags
 Project-URL: Documentation, https://gitlab.insa-rouen.fr/cip/ubiquity/-/wikis/home
 Project-URL: Bug Tracker, https://gitlab.insa-rouen.fr/cip/ubiquity/-/issues
 Classifier: Topic :: Education
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ubiquity-student-1.1.0/README.md` & `ubiquity-student-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/setup.py` & `ubiquity-student-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/argument_parser.py` & `ubiquity-student-1.1.1/src/ubiquity/argument_parser.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/controllers/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/controllers/config_file.py` & `ubiquity-student-1.1.1/src/ubiquity/controllers/config_file.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/controllers/main_controller.py` & `ubiquity-student-1.1.1/src/ubiquity/controllers/main_controller.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/controllers/worker.py` & `ubiquity-student-1.1.1/src/ubiquity/controllers/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 self._files_watching[file_path] = time_updated_file(file_path)
                 print(f'File {file_path} {"created" if response.status_code == StatusCode.CREATED else "updated" } '
                       f'successfully at {get_current_time()}')
                 if not self._has_gui and self.running:
                     self._get_progress()
             elif response.status_code == StatusCode.SUSPENDED:
                 self.running = False
-                signal.raise_signal(signal.SIGUSR1)
+                signal.raise_signal(signal.SIGTERM)
         except UnicodeDecodeError:
             pass
 
     def _delete(self, file_path) -> None:
         file_name = file_path[len(self._model.directory.get()):]
         response = requests.delete(self._model.url_api_action_file(file_name))
         if response.status_code == StatusCode.OK:
@@ -157,15 +157,15 @@
             except KeyError:
                 pass
             print(f'File {file_path} deleted successfully at {get_current_time()}')
             if not self._has_gui and self.running:
                 self._get_progress()
         elif response.status_code == StatusCode.SUSPENDED:
             self.running = False
-            signal.raise_signal(signal.SIGUSR1)
+            signal.raise_signal(signal.SIGTERM)
 
     def _get_files_to_follow(self) -> List[str]:
         """Method getting the server file paths
 
         :return: The list of file paths
         """
         response = requests.get(self._model.url_api_file_paths())
```

### Comparing `ubiquity-student-1.1.0/src/ubiquity/images/ubiquity_icon.png` & `ubiquity-student-1.1.1/src/ubiquity/images/ubiquity_icon.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/locale/fr/LC_MESSAGES/ubiquity-student.mo` & `ubiquity-student-1.1.1/src/ubiquity/locale/fr/LC_MESSAGES/ubiquity-student.mo`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/model.py` & `ubiquity-student-1.1.1/src/ubiquity/model.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/ubiquity_student.py` & `ubiquity-student-1.1.1/src/ubiquity/ubiquity_student.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/version.py` & `ubiquity-student-1.1.1/src/ubiquity/version.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/cui/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/views/cui/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/cui/main_view.py` & `ubiquity-student-1.1.1/src/ubiquity/views/cui/main_view.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/about.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/base.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/base.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/choice.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/choice.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/confirm.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/confirm.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/form.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/form.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/open.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/open.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/dialogs/preference.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/dialogs/preference.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/main_view.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/main_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.menu_bar = parent.menu_bar
         self.model: Model = parent.model
         self.main_controller: MainController = parent.controller
         self._has_form: bool = has_form
         self._has_color: bool = has_color
         self.mainframe = ttk.Frame()
         self.mainframe.pack()
-        signal.signal(signal.SIGUSR1, self.stop_suspend)
+        signal.signal(signal.SIGTERM, self.stop_suspend)
         if has_form:
             self.main_controller.init_values()
             self._ui_setup()
         else:
             self.submit()
 
     def _ui_setup(self):
```

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/menu_bar.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/base.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/base.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sun_valley_dark.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sun_valley_dark.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sun_valley_light.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sun_valley_light.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/LICENSE` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/__init__.py` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/sun-valley.tcl`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl` & `ubiquity-student-1.1.1/src/ubiquity/views/gui/themes/sv_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/src/ubiquity/views/utils.py` & `ubiquity-student-1.1.1/src/ubiquity/views/utils.py`

 * *Files identical despite different names*

### Comparing `ubiquity-student-1.1.0/ubiquity_student.egg-info/PKG-INFO` & `ubiquity-student-1.1.1/ubiquity_student.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiquity-student
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ubiquity permet le suivi de TP de développement informatique
 Home-page: https://gitlab.insa-rouen.fr/cip/ubiquity
 Download-URL: https://gitlab.insa-rouen.fr/cip/ubiquity/-/tags
 Project-URL: Documentation, https://gitlab.insa-rouen.fr/cip/ubiquity/-/wikis/home
 Project-URL: Bug Tracker, https://gitlab.insa-rouen.fr/cip/ubiquity/-/issues
 Classifier: Topic :: Education
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ubiquity-student-1.1.0/ubiquity_student.egg-info/SOURCES.txt` & `ubiquity-student-1.1.1/ubiquity_student.egg-info/SOURCES.txt`

 * *Files identical despite different names*

