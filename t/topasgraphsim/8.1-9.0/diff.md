# Comparing `tmp/topasgraphsim-8.1.tar.gz` & `tmp/topasgraphsim-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topasgraphsim-8.1.tar", last modified: Fri Jan 28 14:28:03 2022, max compression
+gzip compressed data, was "topasgraphsim-9.0.tar", last modified: Fri Jan 28 14:17:05 2022, max compression
```

## Comparing `topasgraphsim-8.1.tar` & `topasgraphsim-9.0.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.551877 topasgraphsim-8.1/
--rw-rw-rw-   0        0        0     1096 2022-01-15 17:04:44.000000 topasgraphsim-8.1/LICENSE
--rw-rw-rw-   0        0        0       99 2022-01-18 11:15:19.000000 topasgraphsim-8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3348 2022-01-28 14:28:03.551877 topasgraphsim-8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2682 2022-01-24 16:10:30.000000 topasgraphsim-8.1/README.md
--rw-rw-rw-   0        0        0      108 2022-01-17 11:32:09.000000 topasgraphsim-8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-01-28 14:28:03.551877 topasgraphsim-8.1/setup.cfg
--rw-rw-rw-   0        0        0     1242 2022-01-28 14:27:11.000000 topasgraphsim-8.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.395879 topasgraphsim-8.1/topasgraphsim/
--rw-rw-rw-   0        0        0       41 2022-01-18 10:57:52.000000 topasgraphsim-8.1/topasgraphsim/__init__.py
--rw-rw-rw-   0        0        0       67 2022-01-18 11:05:03.000000 topasgraphsim-8.1/topasgraphsim/__main__.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.423875 topasgraphsim-8.1/topasgraphsim/src/
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.430876 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/
--rw-rw-rw-   0        0        0       64 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/.git
--rw-rw-rw-   0        0        0     1928 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/.gitignore
--rw-rw-rw-   0        0        0   418679 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/Dark screenshot.png
--rw-rw-rw-   0        0        0     1085 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/LICENSE
--rw-rw-rw-   0        0        0   418500 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/Light screenshot.png
--rw-rw-rw-   0        0        0     4621 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/README.md
--rw-rw-rw-   0        0        0     3299 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/azure.tcl
--rw-rw-rw-   0        0        0    11829 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/example.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.432878 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.483874 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/
--rw-rw-rw-   0        0        0      424 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-accent.png
--rw-rw-rw-   0        0        0      330 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-basic.png
--rw-rw-rw-   0        0        0      357 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-hover.png
--rw-rw-rw-   0        0        0      405 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-invalid.png
--rw-rw-rw-   0        0        0      346 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/button-hover.png
--rw-rw-rw-   0        0        0      457 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/card.png
--rw-rw-rw-   0        0        0      482 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-accent.png
--rw-rw-rw-   0        0        0      423 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-basic.png
--rw-rw-rw-   0        0        0      453 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-hover.png
--rw-rw-rw-   0        0        0      346 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-tri-accent.png
--rw-rw-rw-   0        0        0      310 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-tri-basic.png
--rw-rw-rw-   0        0        0      326 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-tri-hover.png
--rw-rw-rw-   0        0        0      484 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/circle-accent.png
--rw-rw-rw-   0        0        0      437 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/circle-basic.png
--rw-rw-rw-   0        0        0      470 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/circle-hover.png
--rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/combo-button-basic.png
--rw-rw-rw-   0        0        0      248 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/combo-button-focus.png
--rw-rw-rw-   0        0        0      297 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/combo-button-hover.png
--rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/down-accent.png
--rw-rw-rw-   0        0        0      261 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/down.png
--rw-rw-rw-   0        0        0      130 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/empty.png
--rw-rw-rw-   0        0        0      154 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/hor-accent.png
--rw-rw-rw-   0        0        0      156 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/hor-basic.png
--rw-rw-rw-   0        0        0      154 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/hor-hover.png
--rw-rw-rw-   0        0        0      410 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/notebook.png
--rw-rw-rw-   0        0        0      677 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/off-basic.png
--rw-rw-rw-   0        0        0      736 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-accent.png
--rw-rw-rw-   0        0        0      668 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-basic.png
--rw-rw-rw-   0        0        0      587 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-basic.png
--rw-rw-rw-   0        0        0      644 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-hover.png
--rw-rw-rw-   0        0        0      629 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-accent.png
--rw-rw-rw-   0        0        0      561 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-basic.png
--rw-rw-rw-   0        0        0      625 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-hover.png
--rw-rw-rw-   0        0        0      524 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-accent.png
--rw-rw-rw-   0        0        0      505 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-basic.png
--rw-rw-rw-   0        0        0      466 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-hover.png
--rw-rw-rw-   0        0        0      289 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-accent-hover.png
--rw-rw-rw-   0        0        0      319 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-accent.png
--rw-rw-rw-   0        0        0      286 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-basic.png
--rw-rw-rw-   0        0        0      297 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-hover.png
--rw-rw-rw-   0        0        0      255 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/right.png
--rw-rw-rw-   0        0        0      161 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/scale-hor.png
--rw-rw-rw-   0        0        0      161 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/scale-vert.png
--rw-rw-rw-   0        0        0      128 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/separator.png
--rw-rw-rw-   0        0        0      477 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/size.png
--rw-rw-rw-   0        0        0      249 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tab-basic.png
--rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tab-disabled.png
--rw-rw-rw-   0        0        0      260 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tab-hover.png
--rw-rw-rw-   0        0        0      302 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-hor-accent.png
--rw-rw-rw-   0        0        0      267 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-hor-basic.png
--rw-rw-rw-   0        0        0      280 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-hor-hover.png
--rw-rw-rw-   0        0        0      295 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-vert-accent.png
--rw-rw-rw-   0        0        0      257 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-vert-basic.png
--rw-rw-rw-   0        0        0      277 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-vert-hover.png
--rw-rw-rw-   0        0        0      149 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tree-basic.png
--rw-rw-rw-   0        0        0      168 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/tree-pressed.png
--rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/up-accent.png
--rw-rw-rw-   0        0        0      271 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/up.png
--rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/vert-accent.png
--rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/vert-basic.png
--rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/vert-hover.png
--rw-rw-rw-   0        0        0    19369 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark.tcl
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.539876 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/
--rw-rw-rw-   0        0        0      346 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/box-accent.png
--rw-rw-rw-   0        0        0      319 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/box-basic.png
--rw-rw-rw-   0        0        0      329 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/box-hover.png
--rw-rw-rw-   0        0        0      285 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/box-invalid.png
--rw-rw-rw-   0        0        0      326 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/button-hover.png
--rw-rw-rw-   0        0        0      444 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/card.png
--rw-rw-rw-   0        0        0      442 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/check-accent.png
--rw-rw-rw-   0        0        0      390 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/check-basic.png
--rw-rw-rw-   0        0        0      451 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/check-hover.png
--rw-rw-rw-   0        0        0      314 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/check-tri-accent.png
--rw-rw-rw-   0        0        0      281 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/check-tri-basic.png
--rw-rw-rw-   0        0        0      319 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/check-tri-hover.png
--rw-rw-rw-   0        0        0      440 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/circle-accent.png
--rw-rw-rw-   0        0        0      128 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/circle-basic.png
--rw-rw-rw-   0        0        0      429 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/circle-hover.png
--rw-rw-rw-   0        0        0      247 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/combo-button-basic.png
--rw-rw-rw-   0        0        0      254 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/combo-button-focus.png
--rw-rw-rw-   0        0        0      299 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/combo-button-hover.png
--rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/down-accent.png
--rw-rw-rw-   0        0        0      271 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/down.png
--rw-rw-rw-   0        0        0      130 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/empty.png
--rw-rw-rw-   0        0        0      153 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/hor-accent.png
--rw-rw-rw-   0        0        0      157 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/hor-basic.png
--rw-rw-rw-   0        0        0      154 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/hor-hover.png
--rw-rw-rw-   0        0        0      389 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/notebook.png
--rw-rw-rw-   0        0        0      547 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/off-basic.png
--rw-rw-rw-   0        0        0      663 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/off-hover.png
--rw-rw-rw-   0        0        0      635 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/on-accent.png
--rw-rw-rw-   0        0        0      538 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/on-basic.png
--rw-rw-rw-   0        0        0      649 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/on-hover.png
--rw-rw-rw-   0        0        0      508 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/outline-basic.png
--rw-rw-rw-   0        0        0      598 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/outline-hover.png
--rw-rw-rw-   0        0        0      554 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-accent.png
--rw-rw-rw-   0        0        0      482 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-basic.png
--rw-rw-rw-   0        0        0      583 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-hover.png
--rw-rw-rw-   0        0        0      471 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-tri-accent.png
--rw-rw-rw-   0        0        0      400 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-tri-basic.png
--rw-rw-rw-   0        0        0      465 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-tri-hover.png
--rw-rw-rw-   0        0        0      283 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-accent-hover.png
--rw-rw-rw-   0        0        0      292 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-accent.png
--rw-rw-rw-   0        0        0      250 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-basic.png
--rw-rw-rw-   0        0        0      294 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-hover.png
--rw-rw-rw-   0        0        0      266 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/right.png
--rw-rw-rw-   0        0        0      161 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/scale-hor.png
--rw-rw-rw-   0        0        0      162 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/scale-vert.png
--rw-rw-rw-   0        0        0      128 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/separator.png
--rw-rw-rw-   0        0        0      471 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/size.png
--rw-rw-rw-   0        0        0      219 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tab-basic.png
--rw-rw-rw-   0        0        0      220 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tab-disabled.png
--rw-rw-rw-   0        0        0      263 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tab-hover.png
--rw-rw-rw-   0        0        0      274 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-hor-accent.png
--rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-hor-basic.png
--rw-rw-rw-   0        0        0      273 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-hor-hover.png
--rw-rw-rw-   0        0        0      273 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-vert-accent.png
--rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-vert-basic.png
--rw-rw-rw-   0        0        0      266 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-vert-hover.png
--rw-rw-rw-   0        0        0      149 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tree-basic.png
--rw-rw-rw-   0        0        0      169 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/tree-pressed.png
--rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/up-accent.png
--rw-rw-rw-   0        0        0      270 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/up.png
--rw-rw-rw-   0        0        0      152 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/vert-accent.png
--rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/vert-basic.png
--rw-rw-rw-   0        0        0      157 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/vert-hover.png
--rw-rw-rw-   0        0        0    19367 2022-01-18 12:00:54.000000 topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light.tcl
--rw-rw-rw-   0        0        0        0 2022-01-18 09:10:51.000000 topasgraphsim-8.1/topasgraphsim/src/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.545876 topasgraphsim-8.1/topasgraphsim/src/classes/
--rw-rw-rw-   0        0        0        2 2022-01-18 07:29:35.000000 topasgraphsim-8.1/topasgraphsim/src/classes/__init__.py
--rw-rw-rw-   0        0        0    17365 2022-01-28 12:36:57.000000 topasgraphsim-8.1/topasgraphsim/src/classes/dose_figure_handler.py
--rw-rw-rw-   0        0        0    28688 2022-01-28 12:45:45.000000 topasgraphsim-8.1/topasgraphsim/src/classes/main_viewer.py
--rw-rw-rw-   0        0        0     2033 2022-01-28 09:17:38.000000 topasgraphsim-8.1/topasgraphsim/src/classes/measurement_import.py
--rw-rw-rw-   0        0        0      747 2022-01-22 04:23:08.000000 topasgraphsim-8.1/topasgraphsim/src/classes/profile.py
--rw-rw-rw-   0        0        0     3971 2022-01-28 09:17:38.000000 topasgraphsim-8.1/topasgraphsim/src/classes/ptw_import.py
--rw-rw-rw-   0        0        0     3368 2022-01-28 09:17:38.000000 topasgraphsim-8.1/topasgraphsim/src/classes/sim_import.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.546878 topasgraphsim-8.1/topasgraphsim/src/functions/
--rw-rw-rw-   0        0        0     3941 2022-01-28 10:56:15.000000 topasgraphsim-8.1/topasgraphsim/src/functions/dp.py
--rw-rw-rw-   0        0        0     2080 2022-01-21 13:33:28.000000 topasgraphsim-8.1/topasgraphsim/src/functions/pdd.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.549875 topasgraphsim-8.1/topasgraphsim/src/resources/
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.550876 topasgraphsim-8.1/topasgraphsim/src/resources/__pycache__/
--rw-rw-rw-   0        0        0     3478 2022-01-28 12:38:47.000000 topasgraphsim-8.1/topasgraphsim/src/resources/__pycache__/language.cpython-38.pyc
--rw-rw-rw-   0        0        0    15913 2022-01-18 07:08:03.000000 topasgraphsim-8.1/topasgraphsim/src/resources/icon.ico
--rw-rw-rw-   0        0        0     4286 2022-01-28 12:36:57.000000 topasgraphsim-8.1/topasgraphsim/src/resources/language.py
--rw-rw-rw-   0        0        0      190 2022-01-28 14:16:26.000000 topasgraphsim-8.1/topasgraphsim/src/resources/profile.json
--rw-rw-rw-   0        0        0      942 2022-01-28 14:27:16.000000 topasgraphsim-8.1/topasgraphsim/topasgraphsim.py
-drwxrwxrwx   0        0        0        0 2022-01-28 14:28:03.422878 topasgraphsim-8.1/topasgraphsim.egg-info/
--rw-rw-rw-   0        0        0     3348 2022-01-28 14:28:03.000000 topasgraphsim-8.1/topasgraphsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9005 2022-01-28 14:28:03.000000 topasgraphsim-8.1/topasgraphsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-28 14:28:03.000000 topasgraphsim-8.1/topasgraphsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-01-28 14:28:03.000000 topasgraphsim-8.1/topasgraphsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-01-28 14:28:03.000000 topasgraphsim-8.1/topasgraphsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.369585 topasgraphsim-9.0/
+-rw-rw-rw-   0        0        0     1096 2022-01-15 17:04:44.000000 topasgraphsim-9.0/LICENSE
+-rw-rw-rw-   0        0        0       99 2022-01-18 11:15:19.000000 topasgraphsim-9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3348 2022-01-28 14:17:05.368587 topasgraphsim-9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2682 2022-01-24 16:10:30.000000 topasgraphsim-9.0/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-17 11:32:09.000000 topasgraphsim-9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-01-28 14:17:05.369585 topasgraphsim-9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2022-01-28 14:16:34.000000 topasgraphsim-9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.059949 topasgraphsim-9.0/topasgraphsim/
+-rw-rw-rw-   0        0        0       41 2022-01-18 10:57:52.000000 topasgraphsim-9.0/topasgraphsim/__init__.py
+-rw-rw-rw-   0        0        0       67 2022-01-18 11:05:03.000000 topasgraphsim-9.0/topasgraphsim/__main__.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.081586 topasgraphsim-9.0/topasgraphsim/src/
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.128586 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/
+-rw-rw-rw-   0        0        0       64 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/.git
+-rw-rw-rw-   0        0        0     1928 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/.gitignore
+-rw-rw-rw-   0        0        0   418679 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/Dark screenshot.png
+-rw-rw-rw-   0        0        0     1085 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/LICENSE
+-rw-rw-rw-   0        0        0   418500 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/Light screenshot.png
+-rw-rw-rw-   0        0        0     4621 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/README.md
+-rw-rw-rw-   0        0        0     3299 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/azure.tcl
+-rw-rw-rw-   0        0        0    11829 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/example.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.131586 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.235585 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/
+-rw-rw-rw-   0        0        0      424 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-accent.png
+-rw-rw-rw-   0        0        0      330 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-basic.png
+-rw-rw-rw-   0        0        0      357 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-hover.png
+-rw-rw-rw-   0        0        0      405 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/box-invalid.png
+-rw-rw-rw-   0        0        0      346 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/button-hover.png
+-rw-rw-rw-   0        0        0      457 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/card.png
+-rw-rw-rw-   0        0        0      482 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-accent.png
+-rw-rw-rw-   0        0        0      423 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-basic.png
+-rw-rw-rw-   0        0        0      453 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-hover.png
+-rw-rw-rw-   0        0        0      346 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-tri-accent.png
+-rw-rw-rw-   0        0        0      310 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-tri-basic.png
+-rw-rw-rw-   0        0        0      326 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/check-tri-hover.png
+-rw-rw-rw-   0        0        0      484 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/circle-accent.png
+-rw-rw-rw-   0        0        0      437 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/circle-basic.png
+-rw-rw-rw-   0        0        0      470 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/circle-hover.png
+-rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/combo-button-basic.png
+-rw-rw-rw-   0        0        0      248 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/combo-button-focus.png
+-rw-rw-rw-   0        0        0      297 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/combo-button-hover.png
+-rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/down-accent.png
+-rw-rw-rw-   0        0        0      261 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/down.png
+-rw-rw-rw-   0        0        0      130 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/empty.png
+-rw-rw-rw-   0        0        0      154 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/hor-accent.png
+-rw-rw-rw-   0        0        0      156 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/hor-basic.png
+-rw-rw-rw-   0        0        0      154 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/hor-hover.png
+-rw-rw-rw-   0        0        0      410 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/notebook.png
+-rw-rw-rw-   0        0        0      677 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/off-basic.png
+-rw-rw-rw-   0        0        0      736 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-accent.png
+-rw-rw-rw-   0        0        0      668 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-basic.png
+-rw-rw-rw-   0        0        0      587 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-basic.png
+-rw-rw-rw-   0        0        0      644 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-hover.png
+-rw-rw-rw-   0        0        0      629 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-accent.png
+-rw-rw-rw-   0        0        0      561 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-basic.png
+-rw-rw-rw-   0        0        0      625 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-hover.png
+-rw-rw-rw-   0        0        0      524 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-accent.png
+-rw-rw-rw-   0        0        0      505 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-basic.png
+-rw-rw-rw-   0        0        0      466 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-hover.png
+-rw-rw-rw-   0        0        0      289 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-accent-hover.png
+-rw-rw-rw-   0        0        0      319 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-accent.png
+-rw-rw-rw-   0        0        0      286 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-basic.png
+-rw-rw-rw-   0        0        0      297 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/rect-hover.png
+-rw-rw-rw-   0        0        0      255 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/right.png
+-rw-rw-rw-   0        0        0      161 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/scale-hor.png
+-rw-rw-rw-   0        0        0      161 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/scale-vert.png
+-rw-rw-rw-   0        0        0      128 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/separator.png
+-rw-rw-rw-   0        0        0      477 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/size.png
+-rw-rw-rw-   0        0        0      249 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tab-basic.png
+-rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tab-disabled.png
+-rw-rw-rw-   0        0        0      260 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tab-hover.png
+-rw-rw-rw-   0        0        0      302 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-hor-accent.png
+-rw-rw-rw-   0        0        0      267 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-hor-basic.png
+-rw-rw-rw-   0        0        0      280 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-hor-hover.png
+-rw-rw-rw-   0        0        0      295 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-vert-accent.png
+-rw-rw-rw-   0        0        0      257 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-vert-basic.png
+-rw-rw-rw-   0        0        0      277 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tick-vert-hover.png
+-rw-rw-rw-   0        0        0      149 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tree-basic.png
+-rw-rw-rw-   0        0        0      168 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/tree-pressed.png
+-rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/up-accent.png
+-rw-rw-rw-   0        0        0      271 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/up.png
+-rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/vert-accent.png
+-rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/vert-basic.png
+-rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/vert-hover.png
+-rw-rw-rw-   0        0        0    19369 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark.tcl
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.322585 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/
+-rw-rw-rw-   0        0        0      346 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/box-accent.png
+-rw-rw-rw-   0        0        0      319 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/box-basic.png
+-rw-rw-rw-   0        0        0      329 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/box-hover.png
+-rw-rw-rw-   0        0        0      285 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/box-invalid.png
+-rw-rw-rw-   0        0        0      326 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/button-hover.png
+-rw-rw-rw-   0        0        0      444 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/card.png
+-rw-rw-rw-   0        0        0      442 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/check-accent.png
+-rw-rw-rw-   0        0        0      390 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/check-basic.png
+-rw-rw-rw-   0        0        0      451 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/check-hover.png
+-rw-rw-rw-   0        0        0      314 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/check-tri-accent.png
+-rw-rw-rw-   0        0        0      281 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/check-tri-basic.png
+-rw-rw-rw-   0        0        0      319 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/check-tri-hover.png
+-rw-rw-rw-   0        0        0      440 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/circle-accent.png
+-rw-rw-rw-   0        0        0      128 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/circle-basic.png
+-rw-rw-rw-   0        0        0      429 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/circle-hover.png
+-rw-rw-rw-   0        0        0      247 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/combo-button-basic.png
+-rw-rw-rw-   0        0        0      254 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/combo-button-focus.png
+-rw-rw-rw-   0        0        0      299 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/combo-button-hover.png
+-rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/down-accent.png
+-rw-rw-rw-   0        0        0      271 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/down.png
+-rw-rw-rw-   0        0        0      130 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/empty.png
+-rw-rw-rw-   0        0        0      153 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/hor-accent.png
+-rw-rw-rw-   0        0        0      157 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/hor-basic.png
+-rw-rw-rw-   0        0        0      154 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/hor-hover.png
+-rw-rw-rw-   0        0        0      389 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/notebook.png
+-rw-rw-rw-   0        0        0      547 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/off-basic.png
+-rw-rw-rw-   0        0        0      663 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/off-hover.png
+-rw-rw-rw-   0        0        0      635 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/on-accent.png
+-rw-rw-rw-   0        0        0      538 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/on-basic.png
+-rw-rw-rw-   0        0        0      649 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/on-hover.png
+-rw-rw-rw-   0        0        0      508 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/outline-basic.png
+-rw-rw-rw-   0        0        0      598 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/outline-hover.png
+-rw-rw-rw-   0        0        0      554 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-accent.png
+-rw-rw-rw-   0        0        0      482 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-basic.png
+-rw-rw-rw-   0        0        0      583 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-hover.png
+-rw-rw-rw-   0        0        0      471 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-tri-accent.png
+-rw-rw-rw-   0        0        0      400 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-tri-basic.png
+-rw-rw-rw-   0        0        0      465 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-tri-hover.png
+-rw-rw-rw-   0        0        0      283 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-accent-hover.png
+-rw-rw-rw-   0        0        0      292 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-accent.png
+-rw-rw-rw-   0        0        0      250 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-basic.png
+-rw-rw-rw-   0        0        0      294 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/rect-hover.png
+-rw-rw-rw-   0        0        0      266 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/right.png
+-rw-rw-rw-   0        0        0      161 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/scale-hor.png
+-rw-rw-rw-   0        0        0      162 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/scale-vert.png
+-rw-rw-rw-   0        0        0      128 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/separator.png
+-rw-rw-rw-   0        0        0      471 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/size.png
+-rw-rw-rw-   0        0        0      219 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tab-basic.png
+-rw-rw-rw-   0        0        0      220 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tab-disabled.png
+-rw-rw-rw-   0        0        0      263 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tab-hover.png
+-rw-rw-rw-   0        0        0      274 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-hor-accent.png
+-rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-hor-basic.png
+-rw-rw-rw-   0        0        0      273 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-hor-hover.png
+-rw-rw-rw-   0        0        0      273 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-vert-accent.png
+-rw-rw-rw-   0        0        0      234 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-vert-basic.png
+-rw-rw-rw-   0        0        0      266 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tick-vert-hover.png
+-rw-rw-rw-   0        0        0      149 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tree-basic.png
+-rw-rw-rw-   0        0        0      169 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/tree-pressed.png
+-rw-rw-rw-   0        0        0      242 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/up-accent.png
+-rw-rw-rw-   0        0        0      270 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/up.png
+-rw-rw-rw-   0        0        0      152 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/vert-accent.png
+-rw-rw-rw-   0        0        0      158 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/vert-basic.png
+-rw-rw-rw-   0        0        0      157 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/vert-hover.png
+-rw-rw-rw-   0        0        0    19367 2022-01-18 12:00:54.000000 topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light.tcl
+-rw-rw-rw-   0        0        0        0 2022-01-18 09:10:51.000000 topasgraphsim-9.0/topasgraphsim/src/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.338586 topasgraphsim-9.0/topasgraphsim/src/classes/
+-rw-rw-rw-   0        0        0        2 2022-01-18 07:29:35.000000 topasgraphsim-9.0/topasgraphsim/src/classes/__init__.py
+-rw-rw-rw-   0        0        0    17365 2022-01-28 12:36:57.000000 topasgraphsim-9.0/topasgraphsim/src/classes/dose_figure_handler.py
+-rw-rw-rw-   0        0        0    28688 2022-01-28 12:45:45.000000 topasgraphsim-9.0/topasgraphsim/src/classes/main_viewer.py
+-rw-rw-rw-   0        0        0     2033 2022-01-28 09:17:38.000000 topasgraphsim-9.0/topasgraphsim/src/classes/measurement_import.py
+-rw-rw-rw-   0        0        0      747 2022-01-22 04:23:08.000000 topasgraphsim-9.0/topasgraphsim/src/classes/profile.py
+-rw-rw-rw-   0        0        0     3971 2022-01-28 09:17:38.000000 topasgraphsim-9.0/topasgraphsim/src/classes/ptw_import.py
+-rw-rw-rw-   0        0        0     3368 2022-01-28 09:17:38.000000 topasgraphsim-9.0/topasgraphsim/src/classes/sim_import.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.348591 topasgraphsim-9.0/topasgraphsim/src/functions/
+-rw-rw-rw-   0        0        0     3941 2022-01-28 10:56:15.000000 topasgraphsim-9.0/topasgraphsim/src/functions/dp.py
+-rw-rw-rw-   0        0        0     2080 2022-01-21 13:33:28.000000 topasgraphsim-9.0/topasgraphsim/src/functions/pdd.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.359587 topasgraphsim-9.0/topasgraphsim/src/resources/
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.367584 topasgraphsim-9.0/topasgraphsim/src/resources/__pycache__/
+-rw-rw-rw-   0        0        0     3478 2022-01-28 12:38:47.000000 topasgraphsim-9.0/topasgraphsim/src/resources/__pycache__/language.cpython-38.pyc
+-rw-rw-rw-   0        0        0    15913 2022-01-18 07:08:03.000000 topasgraphsim-9.0/topasgraphsim/src/resources/icon.ico
+-rw-rw-rw-   0        0        0     4286 2022-01-28 12:36:57.000000 topasgraphsim-9.0/topasgraphsim/src/resources/language.py
+-rw-rw-rw-   0        0        0      190 2022-01-28 14:16:26.000000 topasgraphsim-9.0/topasgraphsim/src/resources/profile.json
+-rw-rw-rw-   0        0        0      942 2022-01-28 14:16:42.000000 topasgraphsim-9.0/topasgraphsim/topasgraphsim.py
+drwxrwxrwx   0        0        0        0 2022-01-28 14:17:05.080586 topasgraphsim-9.0/topasgraphsim.egg-info/
+-rw-rw-rw-   0        0        0     3348 2022-01-28 14:17:04.000000 topasgraphsim-9.0/topasgraphsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9005 2022-01-28 14:17:05.000000 topasgraphsim-9.0/topasgraphsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-28 14:17:04.000000 topasgraphsim-9.0/topasgraphsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2022-01-28 14:17:04.000000 topasgraphsim-9.0/topasgraphsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-01-28 14:17:04.000000 topasgraphsim-9.0/topasgraphsim.egg-info/top_level.txt
```

### Comparing `topasgraphsim-8.1/LICENSE` & `topasgraphsim-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/PKG-INFO` & `topasgraphsim-9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: topasgraphsim
-Version: 8.1
+Version: 9.0
 Summary: GUI to plot the results of a topas simulation
 Home-page: https://github.com/sebasj13/topas-create-graphs
 Author: Sebastian Schäfer
 Author-email: sebastian.schaefer@student.uni-halle.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sebasj13/topas-create-graphs/issues
 Keywords: topas,monte-carlo,python,simulation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # topasgraphsim
 
 ## Am interface to automatically plot and interpret the results of TOPAS simulations
```

### Comparing `topasgraphsim-8.1/README.md` & `topasgraphsim-9.0/README.md`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/setup.py` & `topasgraphsim-9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="topasgraphsim",
-    version="8.1",
+    version="9.0",
     author="Sebastian Schäfer",
     author_email="sebastian.schaefer@student.uni-halle.de",
     description="GUI to plot the results of a topas simulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sebasj13/topas-create-graphs",
     project_urls={
@@ -33,10 +33,10 @@
     packages=[
         "topasgraphsim",
         "topasgraphsim.src",
         "topasgraphsim.src.classes",
         "topasgraphsim.src.functions",
     ],
     keywords=["topas", "monte-carlo", "python", "simulation"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/.gitignore` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/.gitignore`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/Dark screenshot.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/Dark screenshot.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/LICENSE` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/LICENSE`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/Light screenshot.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/Light screenshot.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/README.md` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/README.md`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/azure.tcl` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/azure.tcl`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/example.py` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/example.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/off-basic.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/off-basic.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-accent.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-accent.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-basic.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/on-basic.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-basic.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-basic.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-hover.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/outline-hover.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-accent.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-accent.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-basic.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-basic.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-hover.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-accent.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark/radio-tri-accent.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/dark.tcl` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/off-basic.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/off-basic.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/off-hover.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/off-hover.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/on-accent.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/on-accent.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/on-basic.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/on-basic.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/on-hover.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/on-hover.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/outline-hover.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/outline-hover.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-accent.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-accent.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-hover.png` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/Azure-ttk-theme/theme/light.tcl` & `topasgraphsim-9.0/topasgraphsim/src/Azure-ttk-theme/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/classes/dose_figure_handler.py` & `topasgraphsim-9.0/topasgraphsim/src/classes/dose_figure_handler.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/classes/main_viewer.py` & `topasgraphsim-9.0/topasgraphsim/src/classes/main_viewer.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/classes/measurement_import.py` & `topasgraphsim-9.0/topasgraphsim/src/classes/measurement_import.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/classes/profile.py` & `topasgraphsim-9.0/topasgraphsim/src/classes/profile.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/classes/ptw_import.py` & `topasgraphsim-9.0/topasgraphsim/src/classes/ptw_import.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/classes/sim_import.py` & `topasgraphsim-9.0/topasgraphsim/src/classes/sim_import.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/functions/dp.py` & `topasgraphsim-9.0/topasgraphsim/src/functions/dp.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/functions/pdd.py` & `topasgraphsim-9.0/topasgraphsim/src/functions/pdd.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/resources/__pycache__/language.cpython-38.pyc` & `topasgraphsim-9.0/topasgraphsim/src/resources/__pycache__/language.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/resources/icon.ico` & `topasgraphsim-9.0/topasgraphsim/src/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/src/resources/language.py` & `topasgraphsim-9.0/topasgraphsim/src/resources/language.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim/topasgraphsim.py` & `topasgraphsim-9.0/topasgraphsim/topasgraphsim.py`

 * *Files identical despite different names*

### Comparing `topasgraphsim-8.1/topasgraphsim.egg-info/PKG-INFO` & `topasgraphsim-9.0/topasgraphsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: topasgraphsim
-Version: 8.1
+Version: 9.0
 Summary: GUI to plot the results of a topas simulation
 Home-page: https://github.com/sebasj13/topas-create-graphs
 Author: Sebastian Schäfer
 Author-email: sebastian.schaefer@student.uni-halle.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sebasj13/topas-create-graphs/issues
 Keywords: topas,monte-carlo,python,simulation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # topasgraphsim
 
 ## Am interface to automatically plot and interpret the results of TOPAS simulations
```

### Comparing `topasgraphsim-8.1/topasgraphsim.egg-info/SOURCES.txt` & `topasgraphsim-9.0/topasgraphsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

