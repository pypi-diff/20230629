# Comparing `tmp/pure_ocean_breeze-3.9.9.tar.gz` & `tmp/pure_ocean_breeze-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.9.tar", last modified: Mon Jun 26 01:28:01 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.0.tar", last modified: Thu Jun 29 13:51:40 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.9.tar` & `pure_ocean_breeze-4.0.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    31577 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    68253 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    50076 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   228559 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.793793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.793793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31577 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.793793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.793793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.797793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   263427 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.797793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.797793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.797793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.797793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.797793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.801793 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.805794 pure_ocean_breeze-4.0.0/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:51:40.793793 pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-29 13:51:40.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-29 13:51:40.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:51:40.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-29 13:51:40.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 13:51:40.000000 pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:51:40.809794 pure_ocean_breeze-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-29 13:51:29.000000 pure_ocean_breeze-4.0.0/setup.py
```

### Comparing `pure_ocean_breeze-3.9.9/LICENSE` & `pure_ocean_breeze-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/PKG-INFO` & `pure_ocean_breeze-4.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.9
+Version: 4.0.0
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: windows
 Provides-Extra: macos
 Provides-Extra: linux
 License-File: LICENSE
 
 # pure_ocean_breeze 
-#### **众人的因子回测框架**
+#### **众人的因子框架**
 ##### 我们的口号是：量价因子才是最牛的！
 ***
 
 ### 全新大版本📢
+* v4.0.0 — 2023.06.28
+> 因子框架4.0版本来啦！逐笔数据&任意秒级数据来啦！
+
 * v3.0.0 — 2022.08.16
+
 >回测框架3.0版本来啦！ 模块拆分&说明文档来啦！[pure_ocean_breeze说明文档](https://chen-001.github.io/pure_ocean_breeze/)
 * v2.0.0 — 2022.07.12
 >回测框架2.0版本来啦！数据库&自动更新&最终因子库功能上线啦！
 
 ### 安装&使用指南🎯
 1. 安装
 > 使用`pip install pure_ocean_breeze`命令进行安装
 2. 初始化
 >* 在初次安装框架时，请进行初始化，以将路径设置到自己的文件里
 >* 使用如下语句进行初始化
 >>```python
->>import pure_ocean_breeze.initialize.initialize
->>pure_ocean_breeze.initialize.initialize.initialize()
+>>import pure_ocean_breeze as p
+>>p.ini()
 >>```
 >* 然后根据提示进行操作即可
 >* 请注意路径不要写反斜杠\，而要写成/
 >* 经过初始化后，以后就可以直接使用，不论重启电脑或者版本升级，都不用再初始化
 >* 如果更换了数据库路径，请重新初始化
 3. 日常调用
 >* **导入框架**
```

### Comparing `pure_ocean_breeze-3.9.9/README.md` & `pure_ocean_breeze-4.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # pure_ocean_breeze 
-#### **众人的因子回测框架**
+#### **众人的因子框架**
 ##### 我们的口号是：量价因子才是最牛的！
 ***
 
 ### 全新大版本📢
+* v4.0.0 — 2023.06.28
+> 因子框架4.0版本来啦！逐笔数据&任意秒级数据来啦！
+
 * v3.0.0 — 2022.08.16
+
 >回测框架3.0版本来啦！ 模块拆分&说明文档来啦！[pure_ocean_breeze说明文档](https://chen-001.github.io/pure_ocean_breeze/)
 * v2.0.0 — 2022.07.12
 >回测框架2.0版本来啦！数据库&自动更新&最终因子库功能上线啦！
 
 ### 安装&使用指南🎯
 1. 安装
 > 使用`pip install pure_ocean_breeze`命令进行安装
 2. 初始化
 >* 在初次安装框架时，请进行初始化，以将路径设置到自己的文件里
 >* 使用如下语句进行初始化
 >>```python
->>import pure_ocean_breeze.initialize.initialize
->>pure_ocean_breeze.initialize.initialize.initialize()
+>>import pure_ocean_breeze as p
+>>p.ini()
 >>```
 >* 然后根据提示进行操作即可
 >* 请注意路径不要写反斜杠\，而要写成/
 >* 经过初始化后，以后就可以直接使用，不论重启电脑或者版本升级，都不用再初始化
 >* 如果更换了数据库路径，请重新初始化
 3. 日常调用
 >* **导入框架**
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-06-21 14:51:14"
-__version__ = "3.9.9"
+__updated__ = "2023-06-29 21:50:43"
+__version__ = "4.0.0"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-05-16 11:40:07"
+__updated__ = "2023-06-28 12:29:06"
 
 import pandas as pd
 import pymysql
 from sqlalchemy import create_engine
 from sqlalchemy import FLOAT, INT, VARCHAR, BIGINT
 from loguru import logger
 import datetime
@@ -728,17 +728,22 @@
             返回的日期是否成以100, by default False
 
         Returns
         -------
         list
             表中所有的日期
         """
-        df = self.get_data(
-            f"select distinct(date) from {self.database_name}.{table_name}"
-        ).sort_values("date")
+        if 'second' in table_name:
+            df = self.get_data(f"select distinct(toYYYYMMDD(date)) from {table_name}").sort_values(
+                "date"
+            )
+        else:
+            df = self.get_data(f"select distinct(date) from {table_name}").sort_values(
+                "date"
+            )
         if mul_100:
             return [i for i in list(df.date) if i != 0]
         else:
             return [int(i / 100) for i in list(df.date) if i != 0]
 
 
 class PostgreSQL(DriverOfPostgre):
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 针对一些不常见的文件格式，读取数据文件的一些工具函数，以及其他数据工具
 """
 
-__updated__ = "2023-06-20 22:25:36"
+__updated__ = "2023-06-28 16:09:30"
 
 import os
 import pandas as pd
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
@@ -44,81 +44,14 @@
         else:
             return False  # Other type (?)
     except NameError:
         return False
 
 
 @do_on_dfs
-@deprecation.deprecated(
-    deprecated_in="3.0",
-    removed_in="4.0",
-    current_version=__version__,
-    details="考虑到h5文件的多样性，4.0版本开始将不再支持一键读入h5文件",
-)
-def read_h5(path: str) -> Dict:
-    """
-    Reads a HDF5 file into a dictionary of pandas DataFrames.
-
-    Parameters
-    ----------
-    path : str
-        The path to the HDF5 file.
-
-    Returns
-    -------
-    `Dict`
-        A dictionary of pandas DataFrames.
-    """
-    res = {}
-    import h5py
-
-    a = h5py.File(path)
-    for k, v in tqdm.tqdm(list(a.items()), desc="数据加载中……"):
-        value = list(v.values())[-1]
-        try:
-            col = [i.decode("utf-8") for i in list(list(v.values())[0])]
-        except Exception:
-            col=list(list(v.values())[0])
-        try:
-            ind = [i.decode("utf-8") for i in list(list(v.values())[1])]
-        except Exception:
-            ind=list(list(v.values())[1])
-        res[k] = pd.DataFrame(value, columns=col, index=ind)
-    return res
-
-
-@do_on_dfs
-@deprecation.deprecated(
-    deprecated_in="3.0",
-    removed_in="4.0",
-    current_version=__version__,
-    details="考虑到h5文件的多样性，4.0版本开始将不再支持一键读入h5文件",
-)
-def read_h5_new(path: str) -> pd.DataFrame:
-    """读取h5文件
-
-    Parameters
-    ----------
-    path : str
-        h5文件路径
-
-    Returns
-    -------
-    `pd.DataFrame`
-        读取字典的第一个value
-    """
-    import h5py
-
-    a = h5py.File(path)
-    v = list(a.values())[0]
-    v = a[v.name][:]
-    return pd.DataFrame(v)
-
-
-@do_on_dfs
 def read_mat(path: str) -> pd.DataFrame:
     """读取mat文件
 
     Parameters
     ----------
     path : str
         mat文件路径
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/data/write_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-06-21 14:50:52"
+__updated__ = "2023-06-27 20:38:39"
 
 import time
 
 try:
     import rqdatac
 
     rqdatac.init()
@@ -49,14 +49,20 @@
 from sqlalchemy import FLOAT, INT, VARCHAR, BIGINT
 from tenacity import retry
 import pickledb
 import tqdm.auto
 from functools import reduce
 from typing import Union, List
 import dcube as dc
+import py7zr
+import unrar
+import zipfile
+import rarfile
+import shutil
+import chardet
 from tenacity import retry, stop_after_attempt
 import questdb.ingress as qdbing
 from pure_ocean_breeze.state.homeplace import HomePlace
 
 try:
     homeplace = HomePlace()
 except Exception:
@@ -85,14 +91,100 @@
     convert_code,
     drop_duplicates_index,
     select_max,
 )
 from pure_ocean_breeze.labor.process import pure_fama
 
 
+
+# 待补充
+def database_update_second_data_to_clickhouse():
+    ...
+    
+    
+    
+def convert_tick_by_tick_data_to_parquet(file_name:str,PATH:str,delete_7z:bool=False):
+    try:
+        files = sorted(os.listdir(file_name))
+        files=[i for i in files if i[0]!='.']
+        files = [file_name + "/" + i for i in files]
+        dfs = []
+        for i in files:
+            with open(i,'rb') as f:
+                tmp = chardet.detect(f.read())
+            df = pd.read_csv(i,encoding=tmp['encoding'])
+            df.Time = file_name.split('/')[-1] + " " + df.Time
+            df.Time = pd.to_datetime(df.Time)
+            df = df.rename(
+                columns={
+                    "TranID": "tranid",
+                    "Time": "date",
+                    "Price": "price",
+                    "Volume": "money",
+                    "SaleOrderVolume": "salemoney",
+                    "BuyOrderVolume": "buymoney",
+                    "Type": "action",
+                    "SaleOrderID": "saleid",
+                    "SaleOrderPrice": "saleprice",
+                    "BuyOrderID": "buyid",
+                    "BuyOrderPrice": "buyprice",
+                }
+            )
+            df = df.assign(code=add_suffix(i.split("/")[-1].split(".")[0]))
+            dfs.append(df)
+        dfs = pd.concat(dfs)
+        dfs.to_parquet(f"{'/'.join(PATH.split('/')[:-2])}/data/{file_name.split('/')[-1]}.parquet")
+        # logger.success(f"{file_name.split('/')[-1]}的逐笔数据已经写入完成！")
+        shutil.rmtree(file_name + "/",True)
+        if delete_7z:
+            os.remove(file_name + ".7z")
+            
+        # logger.warning(f"{file_name.split('/')[-1]}的逐笔数据csv版已经删除")
+    except Exception:
+        file_name=file_name+'/'+file_name.split('/')[-1]
+        convert_tick_by_tick_data_to_parquet(file_name,PATH)
+        
+        
+def convert_tick_by_tick_data_daily(day_path:str,PATH:str):
+    try:
+        olds=os.listdir('/Volumes/My Passport/data/')
+        theday=day_path.split('/')[-1].split('.')[0]
+        olds_ok=[i for i in olds if theday in i]
+        if len(olds_ok)==0:
+            if os.path.exists(day_path.split('.')[0]):
+                ...
+                # print(f"{day_path.split('.')[0]}已存在")
+            elif day_path.endswith('.7z'):
+                archive = py7zr.SevenZipFile(day_path, mode='r')
+                archive.extractall(path='/'.join(day_path.split('/')[:-1]))
+                archive.close()
+            elif day_path.endswith('.zip'):
+                f = zipfile.ZipFile(day_path,'r') # 压缩文件位置
+                f.extractall('/'.join(day_path.split('/')[:-1]))             # 解压位置
+                f.close()
+            elif day_path.endswith('.rar'):
+                f=rarfile.RarFile(day_path,'r')
+                f.extractall('/'.join(day_path.split('/')[:-1]))
+                f.close()
+            convert_tick_by_tick_data_to_parquet(day_path.split('.')[0],PATH)
+        else:
+            print(f'{theday}已经有了，跳过')
+    except Exception:
+        logger.error(f'{day_path}出错了，请当心！！！')
+        
+
+def convert_tick_by_tick_data_monthly(month_path:str,PATH:str):
+    files=os.listdir(month_path)
+    files=[i for i in files if i.startswith('20')]
+    date=month_path.split('/')[-1]
+    files=[month_path+'/'+i for i in files] # 每个形如2018-01-02.7z
+    for i in tqdm.auto.tqdm(files,f'{date}的进度'):
+        convert_tick_by_tick_data_daily(i,PATH)
+        
+        
 def database_update_minute_data_to_clickhouse_and_questdb(
     kind: str, web_port: str = "9001"
 ) -> None:
     """使用米筐更新分钟数据至clickhouse和questdb中
 
     Parameters
     ----------
@@ -552,15 +644,15 @@
         partpe_new = partpe_new[sorted(list(partpe_new.columns))]
         partpe_new = drop_duplicates_index(partpe_new)
         partpe_new.to_parquet(homeplace.daily_data_file + "pe.parquet")
         logger.success("市盈率更新完成")
         
         # pettm
         partpe = df2s[["date", "code", "pe_ttm"]].pivot(
-            index="date", columns="code", values="pe"
+            index="date", columns="code", values="pe_ttm"
         )
         partpe_old = pd.read_parquet(homeplace.daily_data_file + "pettm.parquet")
         partpe_new = pd.concat([partpe_old, partpe])
         partpe_new = partpe_new.drop_duplicates()
         partpe_new = partpe_new[closes.columns]
         partpe_new = partpe_new[sorted(list(partpe_new.columns))]
         partpe_new = drop_duplicates_index(partpe_new)
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,102 +1,93 @@
-__updated__ = "2023-06-26 09:24:10"
+__updated__ = "2022-11-05 00:16:56"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
 import os
-import tqdm.auto
+import tqdm
 import scipy.stats as ss
-from scipy.optimize import linprog
 import statsmodels.formula.api as smf
 import matplotlib as mpl
 
 mpl.rcParams.update(mpl.rcParamsDefault)
 import matplotlib.pyplot as plt
 
+plt.style.use(["science", "no-latex", "notebook"])
 plt.rcParams["axes.unicode_minus"] = False
 
 from functools import reduce, lru_cache, partial
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 import datetime
 from collections.abc import Iterable
 import plotly.express as pe
 import plotly.io as pio
 from plotly.tools import FigureFactory as FF
+import plotly.graph_objects as go
+import plotly.tools as plyoo
 import pyfinance.ols as po
 from texttable import Texttable
 from xpinyin import Pinyin
-import tradetime as tt
 import cufflinks as cf
-import deprecation
-from mpire import WorkerPool
-from scipy.optimize import minimize
-from pure_ocean_breeze import __version__
 
 cf.set_config_file(offline=True)
-from typing import Callable, Union, Dict, List, Tuple
-from pure_ocean_breeze.data.read_data import (
+from typing import Callable, Union
+from pure_ocean_breeze.legacy_version.v3p4.data.read_data import (
     read_daily,
     read_market,
     get_industry_dummies,
     read_swindustry_prices,
     read_zxindustry_prices,
     database_read_final_factors,
-    read_index_single,
 )
-from pure_ocean_breeze.state.homeplace import HomePlace
+from pure_ocean_breeze.legacy_version.v3p4.state.homeplace import HomePlace
 
-try:
-    homeplace = HomePlace()
-except Exception:
-    print("您暂未初始化，功能将受限")
-from pure_ocean_breeze.state.states import STATES
-from pure_ocean_breeze.state.decorators import do_on_dfs
-from pure_ocean_breeze.data.database import *
-from pure_ocean_breeze.data.dicts import INDUS_DICT
-from pure_ocean_breeze.data.tools import (
+homeplace = HomePlace()
+from pure_ocean_breeze.legacy_version.v3p4.state.states import STATES, is_notebook
+from pure_ocean_breeze.legacy_version.v3p4.data.database import *
+from pure_ocean_breeze.legacy_version.v3p4.data.dicts import INDUS_DICT
+from pure_ocean_breeze.legacy_version.v3p4.data.tools import (
     indus_name,
     drop_duplicates_index,
     to_percent,
     to_group,
-    standardlize,
-    select_max,
-    select_min,
 )
-from pure_ocean_breeze.labor.comment import (
+from pure_ocean_breeze.legacy_version.v3p4.labor.comment import (
     comments_on_twins,
     make_relative_comments,
     make_relative_comments_plot,
 )
 
 
-@do_on_dfs
 def daily_factor_on300500(
     fac: pd.DataFrame,
     hs300: bool = 0,
     zz500: bool = 0,
+    zz800: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     other: bool = 0,
 ) -> pd.DataFrame:
     """输入日频或月频因子值，将其限定在某指数成分股的股票池内，
-    目前仅支持沪深300、中证500、中证1000、国证2000成分股，以及这四种指数成分股的组合叠加，和除沪深300、中证500、中证1000以外的股票的成分股
+    目前仅支持沪深300、中证500、中证800、中证1000、国证2000成分股，和除沪深300、中证500、中证1000以外的股票的成分股
 
     Parameters
     ----------
     fac : pd.DataFrame
         未限定股票池的因子值，index为时间，columns为股票代码
     hs300 : bool, optional
         限定股票池为沪深300, by default 0
     zz500 : bool, optional
         限定股票池为中证500, by default 0
+    zz800 : bool, optional
+        限定股票池为中证800, by default 0
     zz1000 : bool, optional
         限定股票池为中证1000, by default 0
     gz2000 : bool, optional
         限定股票池为国证2000, by default 0
     other : bool, optional
         限定股票池为除沪深300、中证500、中证1000以外的股票的成分股, by default 0
 
@@ -108,105 +99,142 @@
     Raises
     ------
     `ValueError`
         如果未指定任何一种指数的成分股，将报错
     """
     last = fac.resample("M").last()
     homeplace = HomePlace()
-    dummies = []
     if fac.shape[0] / last.shape[0] > 2:
         if hs300:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "沪深300日成分股.parquet"
-            ).fillna(0)
-            dummies.append(df)
-        if zz500:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "中证500日成分股.parquet"
-            ).fillna(0)
-            dummies.append(df)
-        if zz1000:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "中证1000日成分股.parquet"
-            ).fillna(0)
-            dummies.append(df)
-        if gz2000:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "国证2000日成分股.parquet"
-            ).fillna(0)
-            dummies.append(df)
-        if other:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "沪深300日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
+            df = df * fac
+            df = df.dropna(how="all")
+        elif zz500:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "中证500日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
+            df = df * fac
+            df = df.dropna(how="all")
+        elif zz800:
+            df1 = pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
+            df1 = df1.set_index(list(df1.columns)[0])
+            df2 = pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
+            df2 = df2.set_index(list(df2.columns)[0])
+            df = df1 + df2
+            df = df.replace(0, np.nan)
+            df = df * fac
+            df = df.dropna(how="all")
+        elif zz1000:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "中证1000日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
+            df = df * fac
+            df = df.dropna(how="all")
+        elif gz2000:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "国证2000日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
+            df = df * fac
+            df = df.dropna(how="all")
+        elif other:
             tr = read_daily(tr=1).fillna(0).replace(0, 1)
             tr = np.sign(tr)
             df1 = (
-                tr * pd.read_parquet(homeplace.daily_data_file + "沪深300日成分股.parquet")
+                tr * pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
             ).fillna(0)
+            df1 = df1.set_index(list(df1.columns)[0])
             df2 = (
-                tr * pd.read_parquet(homeplace.daily_data_file + "中证500日成分股.parquet")
+                tr * pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
             ).fillna(0)
+            df2 = df2.set_index(list(df2.columns)[0])
             df3 = (
-                tr * pd.read_parquet(homeplace.daily_data_file + "中证1000日成分股.parquet")
+                tr * pd.read_feather(homeplace.daily_data_file + "中证1000日成分股.feather")
             ).fillna(0)
+            df3 = df3.set_index(list(df3.columns)[0])
             df = (1 - df1) * (1 - df2) * (1 - df3) * tr
             df = df.replace(0, np.nan) * fac
             df = df.dropna(how="all")
-        if (hs300 + zz500 + zz1000 + gz2000 + other) == 0:
+        else:
             raise ValueError("总得指定一下是哪个成分股吧🤒")
     else:
         if hs300:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "沪深300日成分股.parquet"
-            ).fillna(0)
+            df = pd.read_feather(
+                homeplace.daily_data_file + "沪深300日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
             df = df.resample("M").last()
-            dummies.append(df)
-        if zz500:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "中证500日成分股.parquet"
-            ).fillna(0)
+            df = df * fac
+            df = df.dropna(how="all")
+        elif zz500:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "中证500日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
             df = df.resample("M").last()
-            dummies.append(df)
-        if zz1000:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "中证1000日成分股.parquet"
-            ).fillna(0)
+            df = df * fac
+            df = df.dropna(how="all")
+        elif zz800:
+            df1 = pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
+            df1 = df1.set_index(list(df1.columns)[0])
+            df1 = df1.resample("M").last()
+            df2 = pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
+            df2 = df2.set_index(list(df2.columns)[0])
+            df2 = df2.resample("M").last()
+            df = df1 + df2
+            df = df.replace(0, np.nan)
+            df = df * fac
+            df = df.dropna(how="all")
+        elif zz1000:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "中证1000日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
             df = df.resample("M").last()
-            dummies.append(df)
-        if gz2000:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "国证2000日成分股.parquet"
-            ).fillna(0)
+            df = df * fac
+            df = df.dropna(how="all")
+        elif gz2000:
+            df = pd.read_feather(
+                homeplace.daily_data_file + "国证2000日成分股.feather"
+            ).replace(0, np.nan)
+            df = df.set_index(list(df.columns)[0])
             df = df.resample("M").last()
-            dummies.append(df)
-        if other:
+            df = df * fac
+            df = df.dropna(how="all")
+        elif other:
             tr = read_daily(tr=1).fillna(0).replace(0, 1).resample("M").last()
             tr = np.sign(tr)
             df1 = (
-                tr * pd.read_parquet(homeplace.daily_data_file + "沪深300日成分股.parquet")
+                tr * pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
             ).fillna(0)
+            df1 = df1.set_index(list(df1.columns)[0])
             df1 = df1.resample("M").last()
             df2 = (
-                tr * pd.read_parquet(homeplace.daily_data_file + "中证500日成分股.parquet")
+                tr * pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
             ).fillna(0)
+            df2 = df2.set_index(list(df2.columns)[0])
             df2 = df2.resample("M").last()
             df3 = (
-                tr * pd.read_parquet(homeplace.daily_data_file + "中证1000日成分股.parquet")
+                tr * pd.read_feather(homeplace.daily_data_file + "中证1000日成分股.feather")
             ).fillna(0)
+            df3 = df3.set_index(list(df3.columns)[0])
             df3 = df3.resample("M").last()
             df = (1 - df1) * (1 - df2) * (1 - df3)
             df = df.replace(0, np.nan) * fac
             df = df.dropna(how="all")
-        if (hs300 + zz500 + zz1000 + gz2000 + other) == 0:
+        else:
             raise ValueError("总得指定一下是哪个成分股吧🤒")
-    if len(dummies) > 0:
-        dummies = sum(dummies).replace(0, np.nan)
-        df = (dummies * fac).dropna(how="all")
     return df
 
 
-@do_on_dfs
 def daily_factor_on_industry(
     df: pd.DataFrame, swindustry: bool = 0, zxindustry: bool = 0
 ) -> dict:
     """将一个因子变为仅在某个申万一级行业上的股票
 
     Parameters
     ----------
@@ -237,33 +265,29 @@
         swindustry=swindustry,
         zxindustry=zxindustry,
     )
     ress = {k: v * df for k, v in ress.items()}
     return ress
 
 
-@do_on_dfs
 def group_test_on_industry(
     df: pd.DataFrame,
     group_num: int = 10,
-    trade_cost_double_side: float = 0,
     net_values_writer: pd.ExcelWriter = None,
     swindustry: bool = 0,
     zxindustry: bool = 0,
 ) -> pd.DataFrame:
     """在申万一级行业上测试每个行业的分组回测
 
     Parameters
     ----------
     df : pd.DataFrame
         全市场的因子值，index是时间，columns是股票代码
     group_num : int, optional
         分组数量, by default 10
-    trade_cost_double_side : float, optional
-        交易的双边手续费率, by default 0
     net_values_writer : pd.ExcelWriter, optional
         用于存储各个行业分组及多空对冲净值序列的excel文件, by default None
     swindustry : bool, optional
         选择使用申万一级行业, by default 0
     zxindustry : bool, optional
         选择使用中信一级行业, by default 0
 
@@ -277,41 +301,38 @@
     ks = []
     vs = []
     if swindustry:
         for k, v in dfs.items():
             shen = pure_moonnight(
                 v,
                 groups_num=group_num,
-                trade_cost_double_side=trade_cost_double_side,
                 net_values_writer=net_values_writer,
                 sheetname=INDUS_DICT[k],
                 plt_plot=0,
             )
             ks.append(k)
             vs.append(shen.shen.total_comments.T)
         vs = pd.concat(vs)
         vs.index = [INDUS_DICT[i] for i in ks]
     else:
         for k, v in dfs.items():
             shen = pure_moonnight(
                 v,
                 groups_num=group_num,
-                trade_cost_double_side=trade_cost_double_side,
                 net_values_writer=net_values_writer,
                 sheetname=k,
                 plt_plot=0,
             )
             ks.append(k)
             vs.append(shen.shen.total_comments.T)
         vs = pd.concat(vs)
         vs.index = ks
     return vs
 
 
-@do_on_dfs
 def rankic_test_on_industry(
     df: pd.DataFrame,
     excel_name: str = "行业rankic.xlsx",
     png_name: str = "行业rankic图.png",
     swindustry: bool = 0,
     zxindustry: bool = 0,
 ) -> pd.DataFrame:
@@ -333,32 +354,30 @@
     Returns
     -------
     pd.DataFrame
         行业名称与对应的Rank IC
     """
     vs = group_test_on_industry(df, swindustry=swindustry, zxindustry=zxindustry)
     rankics = vs[["RankIC"]].T
-    if excel_name is not None:
-        rankics.to_excel(excel_name)
+    rankics.to_excel(excel_name)
     rankics.plot(kind="bar")
     plt.show()
     plt.savefig(png_name)
     return rankics
 
 
-@do_on_dfs
 def long_test_on_industry(
     df: pd.DataFrame,
     nums: list,
     pos: bool = 0,
     neg: bool = 0,
     save_stock_list: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
-) -> List[dict]:
+) -> list[dict]:
     """对每个申万/中信一级行业成分股，使用某因子挑选出最多头的n值股票，考察其超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Parameters
     ----------
     df : pd.DataFrame
         使用的因子，index为时间，columns为股票代码
     nums : list
@@ -371,32 +390,32 @@
         是否保存每月每个行业的多头名单，会降低运行速度, by default 0
     swindustry : bool, optional
         在申万一级行业上测试, by default 0
     zxindusrty : bool, optional
         在中信一级行业上测试, by default 0
     Returns
     -------
-    List[dict]
+    list[dict]
         超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Raises
     ------
     IOError
         pos和neg必须有一个为1，否则将报错
     """
     fac = decap_industry(df, monthly=True)
 
     if swindustry:
-        industry_dummy = pd.read_parquet(
-            homeplace.daily_data_file + "申万行业2021版哑变量.parquet"
+        industry_dummy = pd.read_feather(
+            homeplace.daily_data_file + "申万行业2021版哑变量.feather"
         ).fillna(0)
         indus = read_swindustry_prices()
     else:
-        industry_dummy = pd.read_parquet(
-            homeplace.daily_data_file + "中信一级行业哑变量名称版.parquet"
+        industry_dummy = pd.read_feather(
+            homeplace.daily_data_file + "中信一级行业哑变量名称版.feather"
         ).fillna(0)
         indus = read_zxindustry_prices()
     inds = list(industry_dummy.columns)
     ret_next = (
         read_daily(close=1).resample("M").last()
         / read_daily(open=1).resample("M").first()
         - 1
@@ -431,18 +450,24 @@
         fi = fi.T.apply(sing).T
         fi = fi.replace(0, np.nan)
         fi = fi * ret_next
         ret_long = fi.mean(axis=1)
         return ret_long
 
     ret_longs = {k: [] for k in nums}
-    for num in tqdm.auto.tqdm(nums):
-        for code in inds[2:]:
-            df = save_ind(code, num).to_frame(code)
-            ret_longs[num] = ret_longs[num] + [df]
+    if is_notebook():
+        for num in tqdm.tqdm_notebook(nums):
+            for code in inds[2:]:
+                df = save_ind(code, num).to_frame(code)
+                ret_longs[num] = ret_longs[num] + [df]
+    else:
+        for num in tqdm.tqdm(nums):
+            for code in inds[2:]:
+                df = save_ind(code, num).to_frame(code)
+                ret_longs[num] = ret_longs[num] + [df]
 
     indus = indus.resample("M").last().pct_change()
 
     if swindustry:
         coms = {
             k: indus_name(pd.concat(v, axis=1).dropna(how="all").T).T
             for k, v in ret_longs.items()
@@ -523,18 +548,22 @@
                     raise IOError("您需要指定一下因子方向🤒")
                 return tuple(thr.index)
 
             fi = fi.T.apply(sing)
             return fi
 
         stocks_longs = {k: {} for k in nums}
-
-        for num in tqdm.auto.tqdm(nums):
-            for code in inds[2:]:
-                stocks_longs[num][code] = save_ind_stocks(code, num)
+        if is_notebook():
+            for num in tqdm.tqdm_notebook(nums):
+                for code in inds[2:]:
+                    stocks_longs[num][code] = save_ind_stocks(code, num)
+        else:
+            for num in tqdm.tqdm(nums):
+                for code in inds[2:]:
+                    stocks_longs[num][code] = save_ind_stocks(code, num)
 
         for num in nums:
             w1 = pd.ExcelWriter(f"各个{name}一级行业买{num}只的股票名单.xlsx")
             for k, v in stocks_longs[num].items():
                 v = v.T
                 v.index = v.index.strftime("%Y/%m/%d")
                 v.to_excel(w1, sheet_name=INDUS_DICT[k])
@@ -542,22 +571,21 @@
             w1.close()
 
         return [coms_finals, rets_save, stocks_longs]
     else:
         return [coms_finals, rets_save]
 
 
-@do_on_dfs
 def long_test_on_swindustry(
     df: pd.DataFrame,
     nums: list,
     pos: bool = 0,
     neg: bool = 0,
     save_stock_list: bool = 0,
-) -> List[dict]:
+) -> list[dict]:
     """对每个申万一级行业成分股，使用某因子挑选出最多头的n值股票，考察其超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Parameters
     ----------
     df : pd.DataFrame
         使用的因子，index为时间，columns为股票代码
     nums : list
@@ -566,15 +594,15 @@
         因子方向为正，即Rank IC为正，则指定此处为True, by default 0
     neg : bool, optional
         因子方向为负，即Rank IC为负，则指定此处为False, by default 0
     save_stock_list : bool, optional
         是否保存每月每个行业的多头名单，会降低运行速度, by default 0
     Returns
     -------
-    List[dict]
+    list[dict]
         超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Raises
     ------
     IOError
         pos和neg必须有一个为1，否则将报错
     """
@@ -585,22 +613,21 @@
         neg=neg,
         save_stock_list=save_stock_list,
         swindustry=1,
     )
     return res
 
 
-@do_on_dfs
 def long_test_on_zxindustry(
     df: pd.DataFrame,
     nums: list,
     pos: bool = 0,
     neg: bool = 0,
     save_stock_list: bool = 0,
-) -> List[dict]:
+) -> list[dict]:
     """对每个中信一级行业成分股，使用某因子挑选出最多头的n值股票，考察其超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Parameters
     ----------
     df : pd.DataFrame
         使用的因子，index为时间，columns为股票代码
     nums : list
@@ -609,15 +636,15 @@
         因子方向为正，即Rank IC为正，则指定此处为True, by default 0
     neg : bool, optional
         因子方向为负，即Rank IC为负，则指定此处为False, by default 0
     save_stock_list : bool, optional
         是否保存每月每个行业的多头名单，会降低运行速度, by default 0
     Returns
     -------
-    List[dict]
+    list[dict]
         超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Raises
     ------
     IOError
         pos和neg必须有一个为1，否则将报错
     """
@@ -628,15 +655,14 @@
         neg=neg,
         save_stock_list=save_stock_list,
         zxindustry=1,
     )
     return res
 
 
-@do_on_dfs
 @kk.desktop_sender(title="嘿，行业中性化做完啦～🛁")
 def decap(df: pd.DataFrame, daily: bool = 0, monthly: bool = 0) -> pd.DataFrame:
     """对因子做市值中性化
 
     Parameters
     ----------
     df : pd.DataFrame
@@ -652,15 +678,18 @@
         市值中性化之后的因子
 
     Raises
     ------
     `NotImplementedError`
         如果未指定日频或月频，将报错
     """
-    tqdm.auto.tqdm.pandas()
+    if is_notebook():
+        tqdm.tqdm_notebook().pandas()
+    else:
+        tqdm.tqdm.pandas()
     share = read_daily(sharenum=1)
     undi_close = read_daily(close=1, unadjust=1)
     cap = (share * undi_close).stack().reset_index()
     cap.columns = ["date", "code", "cap"]
     cap.cap = ss.boxcox(cap.cap)[0]
 
     def single(x):
@@ -681,15 +710,14 @@
     elif monthly:
         df = (pure_fallmount(df) - (pure_fallmount(cap_monthly),))()
     else:
         raise NotImplementedError("必须指定频率")
     return df
 
 
-@do_on_dfs
 @kk.desktop_sender(title="嘿，行业市值中性化做完啦～🛁")
 def decap_industry(
     df: pd.DataFrame,
     daily: bool = 0,
     monthly: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
@@ -758,49 +786,51 @@
         df.fac = df.fac - ols_w * df.cap - ols_b
         for k, v in ols_bs.items():
             df.fac = df.fac - v * df[k]
         df = df[["fac"]]
         return df
 
     if swindustry:
-        file_name = "申万行业2021版哑变量.parquet"
+        file_name = "申万行业2021版哑变量.feather"
     else:
-        file_name = "中信一级行业哑变量代码版.parquet"
+        file_name = "中信一级行业哑变量代码版.feather"
 
     if monthly:
         industry_dummy = (
-            pd.read_parquet(homeplace.daily_data_file + file_name)
+            pd.read_feather(homeplace.daily_data_file + file_name)
             .fillna(0)
             .set_index("date")
             .groupby("code")
             .resample("M")
             .last()
         )
         industry_dummy = industry_dummy.fillna(0).drop(columns=["code"]).reset_index()
         industry_ws = [f"w{i}" for i in range(1, industry_dummy.shape[1] - 1)]
         col = ["code", "date"] + industry_ws
     elif daily:
-        industry_dummy = pd.read_parquet(homeplace.daily_data_file + file_name).fillna(
+        industry_dummy = pd.read_feather(homeplace.daily_data_file + file_name).fillna(
             0
         )
         industry_ws = [f"w{i}" for i in range(1, industry_dummy.shape[1] - 1)]
         col = ["date", "code"] + industry_ws
     else:
         raise NotImplementedError("必须指定频率")
     industry_dummy.columns = col
     df = pd.merge(df, industry_dummy, on=["date", "code"])
     df = df.set_index(["date", "code"])
-    tqdm.auto.tqdm.pandas()
+    if is_notebook():
+        tqdm.tqdm_notebook().pandas()
+    else:
+        tqdm.tqdm.pandas()
     df = df.groupby(["date"]).progress_apply(neutralize_factors)
     df = df.unstack()
     df.columns = [i[1] for i in list(df.columns)]
     return df
 
 
-@do_on_dfs
 def deboth(df: pd.DataFrame) -> pd.DataFrame:
     """通过回测的方式，对月频因子做行业市值中性化
 
     Parameters
     ----------
     df : pd.DataFrame
         未中性化的因子
@@ -810,33 +840,17 @@
     `pd.DataFrame`
         行业市值中性化之后的因子
     """
     shen = pure_moonnight(df, boxcox=1, plt_plot=0, print_comments=0)
     return shen()
 
 
-@do_on_dfs
-def boom_one(
-    df: pd.DataFrame, backsee: int = 20, daily: bool = 0, min_periods: int = None
-) -> pd.DataFrame:
-    if min_periods is None:
-        min_periods = int(backsee * 0.5)
-    if not daily:
-        df_mean = (
-            df.rolling(backsee, min_periods=min_periods).mean().resample("M").last()
-        )
-    else:
-        df_mean = df.rolling(backsee, min_periods=min_periods).mean()
-    return df_mean
-
-
-@do_on_dfs
 def boom_four(
     df: pd.DataFrame, backsee: int = 20, daily: bool = 0, min_periods: int = None
-) -> Tuple[pd.DataFrame]:
+) -> tuple[pd.DataFrame]:
     """生成20天均值，20天标准差，及二者正向z-score合成，正向排序合成，负向z-score合成，负向排序合成这6个因子
 
     Parameters
     ----------
     df : pd.DataFrame
         原日频因子
     backsee : int, optional
@@ -844,15 +858,15 @@
     daily : bool, optional
         为1是每天都滚动，为0则仅保留月底值, by default 0
     min_periods : int, optional
         rolling时的最小期, by default backsee的一半
 
     Returns
     -------
-    `Tuple[pd.DataFrame]`
+    `tuple[pd.DataFrame]`
         6个因子的元组
     """
     if min_periods is None:
         min_periods = int(backsee * 0.5)
     if not daily:
         df_mean = (
             df.rolling(backsee, min_periods=min_periods).mean().resample("M").last()
@@ -868,42 +882,14 @@
         twins_add = (pure_fallmount(df_mean) + (pure_fallmount(df_std),))()
         rtwins_add = df_mean.rank(axis=1) + df_std.rank(axis=1)
         twins_minus = (pure_fallmount(df_mean) + (pure_fallmount(-df_std),))()
         rtwins_minus = df_mean.rank(axis=1) - df_std.rank(axis=1)
     return df_mean, df_std, twins_add, rtwins_add, twins_minus, rtwins_minus
 
 
-def boom_fours(
-    dfs: List[pd.DataFrame],
-    backsee: Union[int, List[int]] = 20,
-    daily: Union[bool, List[bool]] = 0,
-    min_periods: Union[int, List[int]] = None,
-) -> List[List[pd.DataFrame]]:
-    """对多个因子，每个因子都进行boom_four的操作
-
-    Parameters
-    ----------
-    dfs : List[pd.DataFrame]
-        多个因子的dataframe组成的list
-    backsee : Union[int,List[int]], optional
-        每个因子回看期数, by default 20
-    daily : Union[bool,List[bool]], optional
-        每个因子是否逐日计算, by default 0
-    min_periods : Union[int,List[int]], optional
-        每个因子计算的最小期, by default None
-
-    Returns
-    -------
-    List[List[pd.DataFrame]]
-        每个因子进行boom_four后的结果
-    """
-    return boom_four(df=dfs, backsee=backsee, daily=daily, min_periods=min_periods)
-
-
-@do_on_dfs
 def add_cross_standardlize(*args: list) -> pd.DataFrame:
     """将众多因子横截面做z-score标准化之后相加
 
     Returns
     -------
     `pd.DataFrame`
         合成后的因子
@@ -911,42 +897,37 @@
     fms = [pure_fallmount(i) for i in args]
     one = fms[0]
     others = fms[1:]
     final = one + others
     return final()
 
 
-@do_on_dfs
 def to_tradeends(df: pd.DataFrame) -> pd.DataFrame:
     """将最后一个自然日改变为最后一个交易日
 
     Parameters
     ----------
     df : pd.DataFrame
         index为时间，为每个月的最后一天
 
     Returns
     -------
     `pd.DataFrame`
         修改为交易日标注后的pd.DataFrame
     """
     """"""
-    start = df.index.min()
-    start = start - pd.tseries.offsets.MonthBegin()
-    start = datetime.datetime.strftime(start, "%Y%m%d")
-    trs = read_daily(tr=1, start=start)
+    trs = read_daily(tr=1)
     trs = trs.assign(tradeends=list(trs.index))
     trs = trs[["tradeends"]]
     trs = trs.resample("M").last()
     df = pd.concat([trs, df], axis=1)
     df = df.set_index(["tradeends"])
     return df
 
 
-@do_on_dfs
 def market_kind(
     df: pd.DataFrame,
     zhuban: bool = 0,
     chuangye: bool = 0,
     kechuang: bool = 0,
     beijing: bool = 0,
 ) -> pd.DataFrame:
@@ -1020,41 +1001,38 @@
         返回相关性的序列，而非均值
 
     Returns
     -------
     `float`
         平均截面相关系数
     """
-    if method == "spearman":
-        corr = show_x_with_func(fac1, fac2, lambda x: x.rank().corr().iloc[0, 1])
-    else:
-        corr = show_x_with_func(fac1, fac2, lambda x: x.corr(method=method).iloc[0, 1])
+    corr = show_x_with_func(fac1, fac2, lambda x: x.corr(method=method).iloc[0, 1])
     if show_series:
         return corr
     else:
         if plt_plot:
             corr.plot(rot=60)
             plt.show()
         return corr.mean()
 
 
 def show_corrs(
-    factors: List[pd.DataFrame],
-    factor_names: List[str] = None,
+    factors: list[pd.DataFrame],
+    factor_names: list[str] = None,
     print_bool: bool = True,
     show_percent: bool = True,
     method: str = "spearman",
 ) -> pd.DataFrame:
     """展示很多因子两两之间的截面相关性
 
     Parameters
     ----------
-    factors : List[pd.DataFrame]
+    factors : list[pd.DataFrame]
         所有因子构成的列表, by default None
-    factor_names : List[str], optional
+    factor_names : list[str], optional
         上述因子依次的名字, by default None
     print_bool : bool, optional
         是否打印出两两之间相关系数的表格, by default True
     show_percent : bool, optional
         是否以百分数的形式展示, by default True
     method : str, optional
         计算相关系数的方法, by default "spearman"
@@ -1076,17 +1054,16 @@
     corrs = pd.DataFrame(corrs, columns=factor_names, index=factor_names)
     np.fill_diagonal(corrs.to_numpy(), 1)
     if show_percent:
         pcorrs = corrs.applymap(to_percent)
     else:
         pcorrs = corrs.copy()
     if print_bool:
-        return pcorrs
-    else:
-        return corrs
+        print(pcorrs)
+    return corrs
 
 
 def show_cov(
     fac1: pd.DataFrame,
     fac2: pd.DataFrame,
     plt_plot: bool = 1,
     show_series: bool = 0,
@@ -1149,31 +1126,34 @@
     befo1.columns = ["date", "code", "befo"]
     twins = pd.merge(both1, befo1, on=["date", "code"]).set_index(["date", "code"])
     corr = twins.groupby("date").apply(the_func)
     return corr
 
 
 def show_covs(
-    factors: List[pd.DataFrame],
-    factor_names: List[str] = None,
+    factors: list[pd.DataFrame],
+    factor_names: list[str] = None,
     print_bool: bool = True,
     show_percent: bool = True,
+    method: str = "spearman",
 ) -> pd.DataFrame:
     """展示很多因子两两之间的截面相关性
 
     Parameters
     ----------
-    factors : List[pd.DataFrame]
+    factors : list[pd.DataFrame]
         所有因子构成的列表, by default None
-    factor_names : List[str], optional
+    factor_names : list[str], optional
         上述因子依次的名字, by default None
     print_bool : bool, optional
         是否打印出两两之间相关系数的表格, by default True
     show_percent : bool, optional
         是否以百分数的形式展示, by default True
+    method : str, optional
+        计算相关系数的方法, by default "spearman"
 
     Returns
     -------
     `pd.DataFrame`
         两两之间相关系数的表格
     """
     corrs = []
@@ -1193,166 +1173,82 @@
         pcorrs = corrs.copy()
     if print_bool:
         print(pcorrs)
     return corrs
 
 
 def de_cross(
-    y: pd.DataFrame, xs: Union[List[pd.DataFrame], pd.DataFrame]
+    y: pd.DataFrame, xs: Union[list[pd.DataFrame], pd.DataFrame]
 ) -> pd.DataFrame:
     """使用若干因子对某个因子进行正交化处理
 
     Parameters
     ----------
     y : pd.DataFrame
         研究的目标，回归中的y
-    xs : Union[List[pd.DataFrame],pd.DataFrame]
+    xs : Union[list[pd.DataFrame],pd.DataFrame]
         用于正交化的若干因子，回归中的x
 
     Returns
     -------
     pd.DataFrame
         正交化之后的因子
     """
     if not isinstance(xs, list):
         xs = [xs]
     y = pure_fallmount(y)
     xs = [pure_fallmount(i) for i in xs]
     return (y - xs)()
 
 
-@do_on_dfs
 def show_corrs_with_old(
-    df: pd.DataFrame = None, method: str = "spearman", only_new: bool = 1
+    df: pd.DataFrame = None, method: str = "spearman"
 ) -> pd.DataFrame:
     """计算新因子和已有因子的相关系数
 
     Parameters
     ----------
     df : pd.DataFrame, optional
         新因子, by default None
     method : str, optional
         求相关系数的方法, by default 'spearman'
-    only_new : bool, optional
-        仅计算新因子与旧因子之间的相关系数, by default 1
 
     Returns
     -------
     pd.DataFrame
         相关系数矩阵
     """
     if df is not None:
         df0 = df.resample("M").last()
         if df.shape[0] / df0.shape[0] > 2:
             daily = 1
         else:
             daily = 0
-    nums = os.listdir(homeplace.final_factor_file)
-    nums = sorted(
-        set(
-            [
-                int(i.split("多因子")[1].split("_月")[0])
-                for i in nums
-                if i.endswith("月.parquet")
-            ]
-        )
-    )
     olds = []
-    for i in nums:
+    for i in range(1, 100):
         try:
             if daily:
                 old = database_read_final_factors(order=i)[0]
             else:
                 old = database_read_final_factors(order=i)[0].resample("M").last()
             olds.append(old)
         except Exception:
             break
     if df is not None:
-        if only_new:
-            corrs = [
-                to_percent(show_corr(df, i, plt_plot=0, method=method)) for i in olds
-            ]
-            corrs = pd.Series(corrs, index=[f"old{i}" for i in nums])
-            corrs = corrs.to_frame(f"{method}相关系数").T
-        else:
-            olds = [df] + olds
-            corrs = show_corrs(olds, ["new"] + [f"old{i}" for i in nums], method=method)
+        olds = [df] + olds
+        corrs = show_corrs(
+            olds, ["new"] + [f"old{i}" for i in range(1, len(olds))], method=method
+        )
     else:
-        corrs = show_corrs(olds, [f"old{i}" for i in nums], method=method)
+        corrs = show_corrs(
+            olds, [f"old{i}" for i in range(1, len(olds))], method=method
+        )
     return corrs
 
 
-@do_on_dfs
-def remove_unavailable(df: pd.DataFrame) -> pd.DataFrame:
-    """对日频或月频因子值，剔除st股、不正常交易的股票和上市不足60天的股票
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        因子值，index是时间，columns是股票代码，values是因子值
-
-    Returns
-    -------
-    pd.DataFrame
-        剔除后的因子值
-    """
-    df0 = df.resample("M").last()
-    if df.shape[0] / df0.shape[0] > 2:
-        daily = 1
-    else:
-        daily = 0
-    if daily:
-        state = read_daily(state=1).replace(0, np.nan)
-        st = read_daily(st=1)
-        age = read_daily(age=1)
-        st = (1 - st).replace(0, np.nan)
-        age = ((age >= 60) + 0).replace(0, np.nan)
-        df = df * age * st * state
-    else:
-        moon = pure_moon(no_read_indu=1)
-        moon.set_basic_data()
-        moon.judge_month()
-        df = moon.tris_monthly * df
-    return df
-
-
-class frequency_controller(object):
-    def __init__(self, freq: str):
-        self.homeplace = HomePlace()
-        self.freq = freq
-
-        if freq == "M":
-            self.counts_one_year = 12
-            self.time_shift = pd.DateOffset(months=1)
-            self.states_files = (
-                self.homeplace.daily_data_file + "states_monthly.parquet"
-            )
-            self.sts_files = self.homeplace.daily_data_file + "sts_monthly.parquet"
-            self.comment_name = "月"
-            self.days_in = 20
-        elif freq == "W":
-            self.counts_one_year = 52
-            self.time_shift = pd.DateOffset(weeks=1)
-            self.states_files = self.homeplace.daily_data_file + "states_weekly.parquet"
-            self.sts_files = self.homeplace.daily_data_file + "sts_weekly.parquet"
-            self.comment_name = "周"
-            self.days_in = 5
-        else:
-            raise ValueError("'暂时不支持此频率哈🤒，目前仅支持月频'M'，和周频'W'")
-
-    def next_end(self, x):
-        """找到下个周期的最后一天"""
-        if self.freq == "M":
-            return x + pd.DateOffset(months=1) + pd.tseries.offsets.MonthEnd()
-        elif self.freq == "W":
-            return x + pd.DateOffset(weeks=1)
-        else:
-            raise ValueError("'暂时不支持此频率哈🤒，目前仅支持月频'M'，和周频'W'")
-
-
 class pure_moon(object):
     __slots__ = [
         "homeplace",
         "sts_monthly_file",
         "states_monthly_file",
         "factors",
         "codes",
@@ -1402,56 +1298,35 @@
         "__factors_out",
         "ics",
         "rankics",
         "factor_turnover_rates",
         "factor_turnover_rate",
         "group_rets_std",
         "group_rets_stds",
-        "group_rets_skews",
-        "group_rets_skew",
         "wind_out",
         "swindustry_dummy",
         "zxindustry_dummy",
         "closes2_monthly",
         "rets_monthly_last",
-        "freq_ctrl",
-        "freq",
-        "factor_cover",
-        "factor_cross_skew",
-        "factor_cross_skew_after_neu",
-        "pos_neg_rate",
-        "corr_itself",
-        "factor_cross_stds",
-        "corr_itself_shift2",
-        "rets_all",
-        "inner_long_ret_yearly",
-        "inner_short_ret_yearly",
-        "inner_long_net_values",
-        "inner_short_net_values",
     ]
 
     @classmethod
     @lru_cache(maxsize=None)
     def __init__(
         cls,
-        freq: str = "M",
         no_read_indu: bool = 0,
         swindustry_dummy: pd.DataFrame = None,
         zxindustry_dummy: pd.DataFrame = None,
         read_in_swindustry_dummy: bool = 0,
     ):
         cls.homeplace = HomePlace()
-        cls.freq = freq
-        cls.freq_ctrl = frequency_controller(freq)
         # 已经算好的月度st状态文件
-        # week_here
-        cls.sts_monthly_file = cls.freq_ctrl.sts_files
+        cls.sts_monthly_file = homeplace.daily_data_file + "sts_monthly.feather"
         # 已经算好的月度交易状态文件
-        # week_here
-        cls.states_monthly_file = cls.freq_ctrl.states_files
+        cls.states_monthly_file = homeplace.daily_data_file + "states_monthly.feather"
 
         if swindustry_dummy is not None:
             cls.swindustry_dummy = swindustry_dummy
         if zxindustry_dummy is not None:
             cls.zxindustry_dummy = zxindustry_dummy
 
         def deal_dummy(industry_dummy):
@@ -1461,37 +1336,37 @@
             industry_dummy.columns = col
             industry_dummy = industry_dummy[
                 industry_dummy.date >= pd.Timestamp("20100101")
             ]
             return industry_dummy
 
         if (swindustry_dummy is None) and (zxindustry_dummy is None):
+
             if not no_read_indu:
                 if read_in_swindustry_dummy:
-                    # week_here
                     cls.swindustry_dummy = (
-                        pd.read_parquet(
-                            cls.homeplace.daily_data_file + "申万行业2021版哑变量.parquet"
+                        pd.read_feather(
+                            cls.homeplace.daily_data_file + "申万行业2021版哑变量.feather"
                         )
                         .fillna(0)
                         .set_index("date")
                         .groupby("code")
-                        .resample(freq)
+                        .resample("M")
                         .last()
                     )
                     cls.swindustry_dummy = deal_dummy(cls.swindustry_dummy)
-                # week_here
+
                 cls.zxindustry_dummy = (
-                    pd.read_parquet(
-                        cls.homeplace.daily_data_file + "中信一级行业哑变量代码版.parquet"
+                    pd.read_feather(
+                        cls.homeplace.daily_data_file + "中信一级行业哑变量代码版.feather"
                     )
                     .fillna(0)
                     .set_index("date")
                     .groupby("code")
-                    .resample(freq)
+                    .resample("M")
                     .last()
                     .fillna(0)
                 )
 
                 cls.zxindustry_dummy = deal_dummy(cls.zxindustry_dummy)
 
     @property
@@ -1499,83 +1374,47 @@
         return self.__factors_out
 
     def __call__(self):
         """调用对象则返回因子值"""
         return self.factors_out
 
     @classmethod
-    @lru_cache(maxsize=None)
     def set_basic_data(
         cls,
-        ages: pd.DataFrame = None,
-        sts: pd.DataFrame = None,
-        states: pd.DataFrame = None,
-        opens: pd.DataFrame = None,
-        closes: pd.DataFrame = None,
-        capitals: pd.DataFrame = None,
-        opens_average_first_day: bool = 0,
-        total_cap: bool = 0,
+        age: pd.DataFrame,
+        st: pd.DataFrame,
+        state: pd.DataFrame,
+        open: pd.DataFrame,
+        close: pd.DataFrame,
+        capital: pd.DataFrame,
     ):
-        if ages is None:
-            ages = read_daily(age=1, start=20100101)
-        if sts is None:
-            sts = read_daily(st=1, start=20100101)
-        if states is None:
-            states = read_daily(state=1, start=20100101)
-        if opens is None:
-            if opens_average_first_day:
-                opens = read_daily(vwap=1, start=20100101)
-            else:
-                opens = read_daily(open=1, start=20100101)
-        if closes is None:
-            closes = read_daily(close=1, start=20100101)
-        if capitals is None:
-            if total_cap:
-                capitals = (
-                    read_daily(total_cap=1, start=20100101).resample(cls.freq).last()
-                )
-            else:
-                capitals = (
-                    read_daily(flow_cap=1, start=20100101).resample(cls.freq).last()
-                )
         # 上市天数文件
-        cls.ages = ages
+        cls.ages = age
         # st日子标志文件
-        cls.sts = sts.fillna(0)
+        cls.sts = st.fillna(0)
         # cls.sts = 1 - cls.sts.fillna(0)
         # 交易状态文件
-        cls.states = states
+        cls.states = state
         # 复权开盘价数据文件
-        cls.opens = opens
+        cls.opens = open
         # 复权收盘价数据文件
-        cls.closes = closes
+        cls.closes = close
         # 月底流通市值数据
-        cls.capital = capitals
-        if cls.opens is not None:
-            cls.opens = cls.opens.replace(0, np.nan)
-        if cls.closes is not None:
-            cls.closes = cls.closes.replace(0, np.nan)
+        cls.capital = capital
+        cls.opens = cls.opens.replace(0, np.nan)
+        cls.closes = cls.closes.replace(0, np.nan)
 
-    def set_factor_df_date_as_index(self, df: pd.DataFrame):
+    def set_factor_df_date_as_index(self, df):
         """设置因子数据的dataframe，因子表列名应为股票代码，索引应为时间"""
-        # week_here
-        self.factors = df.resample(self.freq).last().dropna(how="all")
-        self.factor_cover = np.sign(self.factors.abs() + 1).sum().sum()
-        opens = self.opens[self.opens.index >= self.factors.index.min()]
-        total = np.sign(opens.resample(self.freq).last()).sum().sum()
-        self.factor_cover = min(self.factor_cover / total, 1)
-        self.factor_cross_skew = self.factors.skew(axis=1).mean()
-        pos_num = ((self.factors > 0) + 0).sum().sum()
-        neg_num = ((self.factors < 0) + 0).sum().sum()
-        self.pos_neg_rate = pos_num / (neg_num + pos_num)
-        self.corr_itself = show_corr(self.factors, self.factors.shift(1), plt_plot=0)
-        self.corr_itself_shift2 = show_corr(
-            self.factors, self.factors.shift(2), plt_plot=0
-        )
-        self.factor_cross_stds = self.factors.std(axis=1)
+        df = df.reset_index()
+        df.columns = ["date"] + list(df.columns)[1:]
+        self.factors = df
+        self.factors = self.factors.set_index("date")
+        self.factors = self.factors.resample("M").last()
+        self.factors = self.factors.reset_index()
 
     @classmethod
     def judge_month_st(cls, df):
         """比较一个月内st的天数，如果st天数多，就删除本月，如果正常多，就保留本月"""
         st_count = len(df[df == 1])
         normal_count = len(df[df != 1])
         if st_count >= normal_count:
@@ -1594,93 +1433,62 @@
             return 1
 
     @classmethod
     def read_add(cls, pridf, df, func):
         """由于数据更新，过去计算的月度状态可能需要追加"""
         if pridf.index.max() > df.index.max():
             df_add = pridf[pridf.index > df.index.max()]
-            if df_add.shape[0] > int(cls.freq_ctrl.days_in / 2):
-                df_1 = df_add.index.max()
-                year = df_1.year
-                month = df_1.month
-                last = tt.date.get_close(year=year, m=month).pd_date()
-                if (last == df_1)[0]:
-                    # week_here
-                    df_add = df_add.resample(cls.freq).apply(func)
-                    df = pd.concat([df, df_add])
-                    return df
-                else:
-                    df_add = df_add[
-                        df_add.index < pd.Timestamp(year=year, month=month, day=1)
-                    ]
-                    if df_add.shape[0] > 0:
-                        df_add = df_add.resample(cls.freq).apply(func)
-                        df = pd.concat([df, df_add])
-                        return df
-                    else:
-                        return df
-            else:
-                return df
+            df_add = df_add.resample("M").apply(func)
+            df = pd.concat([df, df_add])
+            return df
         else:
             return df
 
     @classmethod
     def daily_to_monthly(cls, pridf, path, func):
         """把日度的交易状态、st、上市天数，转化为月度的，并生成能否交易的判断
         读取本地已经算好的文件，并追加新的时间段部分，如果本地没有就直接全部重新算"""
         try:
-            month_df = pd.read_parquet(path)
+            month_df = pd.read_feather(path)
+            month_df = month_df.set_index(list(month_df.columns)[0])
             month_df = cls.read_add(pridf, month_df, func)
-            month_df.to_parquet(path)
+            month_df.reset_index().to_feather(path)
         except Exception as e:
             if not STATES["NO_LOG"]:
                 logger.error("error occurs when read state files")
                 logger.error(e)
             print("state file rewriting……")
-            # week_here
-            df_1 = pridf.index.max()
-            year = df_1.year
-            month = df_1.month
-            last = tt.date.get_close(year=year, m=month).pd_date()
-            if not (last == df_1)[0]:
-                pridf = pridf[pridf.index < pd.Timestamp(year=year, month=month, day=1)]
-            month_df = pridf.resample(cls.freq).apply(func)
-            month_df.to_parquet(path)
+            month_df = pridf.resample("M").apply(func)
+            month_df.reset_index().to_feather(path)
         return month_df
 
     @classmethod
     @lru_cache(maxsize=None)
     def judge_month(cls):
         """生成一个月综合判断的表格"""
-        if cls.freq == "M":
-            cls.sts_monthly = cls.daily_to_monthly(
-                cls.sts, cls.sts_monthly_file, cls.judge_month_st
-            )
-            cls.states_monthly = cls.daily_to_monthly(
-                cls.states, cls.states_monthly_file, cls.judge_month_state
-            )
-            # week_here
-            cls.ages_monthly = (cls.ages.resample(cls.freq).last() > 60) + 0
-            cls.tris_monthly = cls.sts_monthly * cls.states_monthly * cls.ages_monthly
-            cls.tris_monthly = cls.tris_monthly.replace(0, np.nan)
-        else:
-            cls.tris_monthly = (
-                (1 - cls.sts).resample(cls.freq).last().ffill(limit=2)
-                * cls.states.resample(cls.freq).last().ffill(limit=2)
-                * ((cls.ages.resample(cls.freq).last() > 60) + 0)
-            ).replace(0, np.nan)
+
+        cls.sts_monthly = cls.daily_to_monthly(
+            cls.sts, cls.sts_monthly_file, cls.judge_month_st
+        )
+        cls.states_monthly = cls.daily_to_monthly(
+            cls.states, cls.states_monthly_file, cls.judge_month_state
+        )
+        cls.ages_monthly = cls.ages.resample("M").last()
+        cls.ages_monthly = np.sign(cls.ages_monthly.applymap(lambda x: x - 60)).replace(
+            -1, 0
+        )
+        cls.tris_monthly = cls.sts_monthly * cls.states_monthly * cls.ages_monthly
+        cls.tris_monthly = cls.tris_monthly.replace(0, np.nan)
 
     @classmethod
     @lru_cache(maxsize=None)
     def get_rets_month(cls):
         """计算每月的收益率，并根据每月做出交易状态，做出删减"""
-        # week_here
-        cls.opens_monthly = cls.opens.resample(cls.freq).first()
-        # week_here
-        cls.closes_monthly = cls.closes.resample(cls.freq).last()
+        cls.opens_monthly = cls.opens.resample("M").first()
+        cls.closes_monthly = cls.closes.resample("M").last()
         cls.rets_monthly = (cls.closes_monthly - cls.opens_monthly) / cls.opens_monthly
         cls.rets_monthly = cls.rets_monthly * cls.tris_monthly
         cls.rets_monthly = cls.rets_monthly.stack().reset_index()
         cls.rets_monthly.columns = ["date", "code", "ret"]
 
     @classmethod
     def neutralize_factors(cls, df):
@@ -1719,27 +1527,24 @@
         else:
             cls.cap["cap_size"] = np.log(cls.cap["cap_size"])
 
     def get_neutral_factors(
         self, zxindustry_dummies=0, swindustry_dummies=0, only_cap=0
     ):
         """对因子进行行业市值中性化"""
-        # week_here
-        self.factors.index = self.factors.index + self.freq_ctrl.time_shift
-        # week_here
-        self.factors = self.factors.resample(self.freq).last()
-        # week_here
-        last_date = self.freq_ctrl.next_end(self.tris_monthly.index.max())
+        self.factors = self.factors.set_index("date")
+        self.factors.index = self.factors.index + pd.DateOffset(months=1)
+        self.factors = self.factors.resample("M").last()
+        last_date = self.tris_monthly.index.max() + pd.DateOffset(months=1)
+        last_date = last_date + pd.tseries.offsets.MonthEnd()
         add_tail = pd.DataFrame(1, index=[last_date], columns=self.tris_monthly.columns)
         tris_monthly = pd.concat([self.tris_monthly, add_tail])
         self.factors = self.factors * tris_monthly
-        # week_here
-        self.factors.index = self.factors.index - self.freq_ctrl.time_shift
-        # week_here
-        self.factors = self.factors.resample(self.freq).last()
+        self.factors.index = self.factors.index - pd.DateOffset(months=1)
+        self.factors = self.factors.resample("M").last()
         self.factors = self.factors.stack().reset_index()
         self.factors.columns = ["date", "code", "fac"]
         self.factors = pd.merge(
             self.factors, self.cap, how="inner", on=["date", "code"]
         )
         if not only_cap:
             if swindustry_dummies:
@@ -1752,33 +1557,31 @@
                 )
         self.factors = self.factors.set_index(["date", "code"])
         self.factors = self.factors.groupby(["date"]).apply(self.neutralize_factors)
         self.factors = self.factors.reset_index()
 
     def deal_with_factors(self):
         """删除不符合交易条件的因子数据"""
+        self.factors = self.factors.set_index("date")
         self.__factors_out = self.factors.copy()
-        # week_here
-        self.factors.index = self.factors.index + self.freq_ctrl.time_shift
-        # week_here
-        self.factors = self.factors.resample(self.freq).last()
+        self.__factors_out.columns = [i[1] for i in list(self.__factors_out.columns)]
+        self.factors.index = self.factors.index + pd.DateOffset(months=1)
+        self.factors = self.factors.resample("M").last()
         self.factors = self.factors * self.tris_monthly
         self.factors = self.factors.stack().reset_index()
         self.factors.columns = ["date", "code", "fac"]
 
     def deal_with_factors_after_neutralize(self):
         """中性化之后的因子处理方法"""
         self.factors = self.factors.set_index(["date", "code"])
         self.factors = self.factors.unstack()
         self.__factors_out = self.factors.copy()
         self.__factors_out.columns = [i[1] for i in list(self.__factors_out.columns)]
-        # week_here
-        self.factors.index = self.factors.index + self.freq_ctrl.time_shift
-        # week_here
-        self.factors = self.factors.resample(self.freq).last()
+        self.factors.index = self.factors.index + pd.DateOffset(months=1)
+        self.factors = self.factors.resample("M").last()
         self.factors.columns = list(map(lambda x: x[1], list(self.factors.columns)))
         self.factors = self.factors.stack().reset_index()
         self.factors.columns = ["date", "code", "fac"]
 
     @classmethod
     def find_limit(cls, df, up=1):
         """计算涨跌幅超过9.8%的股票，并将其存储进一个长列表里
@@ -1797,38 +1600,35 @@
         """找月初第一天就涨停"""
         """或者是月末跌停的股票"""
         cls.opens_monthly_shift = cls.opens_monthly.copy()
         cls.opens_monthly_shift = cls.opens_monthly_shift.shift(-1)
         cls.rets_monthly_begin = (
             cls.opens_monthly_shift - cls.closes_monthly
         ) / cls.closes_monthly
-        # week_here
-        cls.closes2_monthly = cls.closes.shift(1).resample(cls.freq).last()
+        cls.closes2_monthly = cls.closes.shift(1).resample("M").last()
         cls.rets_monthly_last = (
             cls.closes_monthly - cls.closes2_monthly
         ) / cls.closes2_monthly
         cls.limit_ups = cls.find_limit(cls.rets_monthly_begin, up=1)
         cls.limit_downs = cls.find_limit(cls.rets_monthly_last, up=-1)
 
     def get_ic_rankic(cls, df):
         """计算IC和RankIC"""
         df1 = df[["ret", "fac"]]
         ic = df1.corr(method="pearson").iloc[0, 1]
-        rankic = df1.rank().corr().iloc[0, 1]
+        rankic = df1.corr(method="spearman").iloc[0, 1]
         df2 = pd.DataFrame({"ic": [ic], "rankic": [rankic]})
         return df2
 
     def get_icir_rankicir(cls, df):
         """计算ICIR和RankICIR"""
         ic = df.ic.mean()
         rankic = df.rankic.mean()
-        # week_here
-        icir = ic / np.std(df.ic) * (cls.freq_ctrl.counts_one_year ** (0.5))
-        # week_here
-        rankicir = rankic / np.std(df.rankic) * (cls.freq_ctrl.counts_one_year ** (0.5))
+        icir = ic / np.std(df.ic) * (12 ** (0.5))
+        rankicir = rankic / np.std(df.rankic) * (12 ** (0.5))
         return pd.DataFrame(
             {"IC": [ic], "ICIR": [icir], "RankIC": [rankic], "RankICIR": [rankicir]},
             index=["评价指标"],
         )
 
     def get_ic_icir_and_rank(cls, df):
         """计算IC、ICIR、RankIC、RankICIR"""
@@ -1837,15 +1637,15 @@
         cls.rankics = df1.rankic
         cls.ics = cls.ics.reset_index(drop=True, level=1).to_frame()
         cls.rankics = cls.rankics.reset_index(drop=True, level=1).to_frame()
         df2 = cls.get_icir_rankicir(df1)
         df2 = df2.T
         dura = (df.date.max() - df.date.min()).days / 365
         t_value = df2.iloc[3, 0] * (dura ** (1 / 2))
-        df3 = pd.DataFrame({"评价指标": [t_value]}, index=["RankIC.t"])
+        df3 = pd.DataFrame({"评价指标": [t_value]}, index=["RankIC均值t值"])
         df4 = pd.concat([df2, df3])
         return df4
 
     @classmethod
     def get_groups(cls, df, groups_num):
         """依据因子值，判断是在第几组"""
         if "group" in list(df.columns):
@@ -1863,25 +1663,32 @@
         if len(l) < df.shape[0]:
             l = l + [groups_num] * (df.shape[0] - len(l))
         l = l[: df.shape[0]]
         df.insert(0, "group", l)
         return df
 
     @classmethod
+    def next_month_end(cls, x):
+        """找到下个月最后一天"""
+        x1 = x = x + relativedelta(months=1)
+        while x1.month == x.month:
+            x1 = x1 + relativedelta(days=1)
+        return x1 - relativedelta(days=1)
+
+    @classmethod
     def limit_old_to_new(cls, limit, data):
         """获取跌停股在旧月的组号，然后将日期调整到新月里
         涨停股则获得新月里涨停股的代码和时间，然后直接删去"""
         data1 = data.copy()
         data1 = data1.reset_index()
         data1.columns = ["data_index"] + list(data1.columns)[1:]
         old = pd.merge(limit, data1, how="inner", on=["date", "code"])
         old = old.set_index("data_index")
         old = old[["group", "date", "code"]]
-        # week_here
-        old.date = list(map(cls.freq_ctrl.next_end, list(old.date)))
+        old.date = list(map(cls.next_month_end, list(old.date)))
         return old
 
     def get_data(self, groups_num):
         """拼接因子数据和每月收益率数据，并对涨停和跌停股加以处理"""
         self.data = pd.merge(
             self.rets_monthly, self.factors, how="inner", on=["date", "code"]
         )
@@ -1889,124 +1696,91 @@
         self.data = self.data.groupby("date").apply(
             lambda x: self.get_groups(x, groups_num)
         )
         self.wind_out = self.data.copy()
         self.factor_turnover_rates = self.data.pivot(
             index="date", columns="code", values="group"
         )
-        rates = []
-        for i in range(1, groups_num + 1):
-            son = (self.factor_turnover_rates == i) + 0
-            son1 = son.diff()
-            # self.factor_turnover_rates = self.factor_turnover_rates.diff()
-            change = ((np.abs(np.sign(son1)) == 1) + 0).sum(axis=1)
-            still = (((son1 == 0) + 0) * son).sum(axis=1)
-            rate = change / (change + still)
-            rates.append(rate.to_frame(f"group{i}"))
-        rates = pd.concat(rates, axis=1).fillna(0)
-        self.factor_turnover_rates = rates
+        self.factor_turnover_rates = self.factor_turnover_rates.diff()
+        change = ((np.abs(np.sign(self.factor_turnover_rates)) == 1) + 0).sum(axis=1)
+        still = ((self.factor_turnover_rates == 0) + 0).sum(axis=1)
+        self.factor_turnover_rates = change / (change + still)
+        self.factor_turnover_rate = self.factor_turnover_rates.mean()
         self.data = self.data.reset_index(drop=True)
         limit_ups_object = self.limit_old_to_new(self.limit_ups, self.data)
         limit_downs_object = self.limit_old_to_new(self.limit_downs, self.data)
         self.data = self.data.drop(limit_ups_object.index)
         rets_monthly_limit_downs = pd.merge(
             self.rets_monthly, limit_downs_object, how="inner", on=["date", "code"]
         )
         self.data = pd.concat([self.data, rets_monthly_limit_downs])
 
+    def select_data_time(self, time_start, time_end):
+        """筛选特定的时间段"""
+        if time_start:
+            self.data = self.data[self.data.date >= time_start]
+        if time_end:
+            self.data = self.data[self.data.date <= time_end]
+
     def make_start_to_one(self, l):
         """让净值序列的第一个数变成1"""
         min_date = self.factors.date.min()
         add_date = min_date - relativedelta(days=min_date.day)
         add_l = pd.Series([1], index=[add_date])
         l = pd.concat([add_l, l])
         return l
 
     def to_group_ret(self, l):
         """每一组的年化收益率"""
-        # week_here
-        ret = l[-1] ** (self.freq_ctrl.counts_one_year / len(l)) - 1
+        ret = l[-1] ** (12 / len(l)) - 1
         return ret
 
-    def get_group_rets_net_values(
-        self, groups_num=10, value_weighted=False, trade_cost_double_side=0
-    ):
+    def get_group_rets_net_values(self, groups_num=10, value_weighted=False):
         """计算组内每一期的平均收益，生成每日收益率序列和净值序列"""
         if value_weighted:
             cap_value = self.capital.copy()
-            # week_here
-            cap_value = cap_value.resample(self.freq).last().shift(1)
+            cap_value = cap_value.resample("M").last().shift(1)
             cap_value = cap_value * self.tris_monthly
             # cap_value=np.log(cap_value)
             cap_value = cap_value.stack().reset_index()
             cap_value.columns = ["date", "code", "cap_value"]
             self.data = pd.merge(self.data, cap_value, on=["date", "code"])
 
             def in_g(df):
                 df.cap_value = df.cap_value / df.cap_value.sum()
                 df.ret = df.ret * df.cap_value
                 return df.ret.sum()
 
             self.group_rets = self.data.groupby(["date", "group"]).apply(in_g)
-            self.rets_all = self.data.groupby(["date"]).apply(in_g)
             self.group_rets_std = "市值加权暂未设置该功能，敬请期待🌙"
         else:
             self.group_rets = self.data.groupby(["date", "group"]).apply(
                 lambda x: x.ret.mean()
             )
-            self.rets_all = self.data.groupby(["date"]).apply(lambda x: x.ret.mean())
-            self.group_rets_stds = self.data.groupby(["date", "group"]).ret.std()
-            self.group_rets_std = (
-                self.group_rets_stds.reset_index().groupby("group").mean()
-            )
-            self.group_rets_skews = self.data.groupby(["date", "group"]).ret.skew()
-            self.group_rets_skew = (
-                self.group_rets_skews.reset_index().groupby("group").mean()
+            self.group_rets_stds = self.data.groupby(["date", "group"]).apply(
+                lambda x: x.ret.std()
             )
+            self.group_rets_std = self.group_rets_stds.groupby("group").mean()
         # dropna是因为如果股票行情数据比因子数据的截止日期晚，而最后一个月发生月初跌停时，会造成最后某组多出一个月的数据
         self.group_rets = self.group_rets.unstack()
         self.group_rets = self.group_rets[
             self.group_rets.index <= self.factors.date.max()
         ]
         self.group_rets.columns = list(map(str, list(self.group_rets.columns)))
         self.group_rets = self.group_rets.add_prefix("group")
-        self.group_rets = (
-            self.group_rets - self.factor_turnover_rates * trade_cost_double_side
-        )
-        self.rets_all = (
-            self.rets_all
-            - self.factor_turnover_rates.mean(axis=1) * trade_cost_double_side
-        )
         self.long_short_rets = (
             self.group_rets["group1"] - self.group_rets["group" + str(groups_num)]
         )
-        self.inner_rets_long = self.group_rets.group1 - self.rets_all
-        self.inner_rets_short = (
-            self.rets_all - self.group_rets["group" + str(groups_num)]
-        )
-        self.long_short_net_values = self.make_start_to_one(
-            (self.long_short_rets + 1).cumprod()
-        )
+        self.long_short_net_values = (self.long_short_rets + 1).cumprod()
         if self.long_short_net_values[-1] <= self.long_short_net_values[0]:
             self.long_short_rets = (
                 self.group_rets["group" + str(groups_num)] - self.group_rets["group1"]
             )
-            self.long_short_net_values = self.make_start_to_one(
-                (self.long_short_rets + 1).cumprod()
-            )
-            self.inner_rets_long = (
-                self.group_rets["group" + str(groups_num)] - self.rets_all
-            )
-            self.inner_rets_short = self.rets_all - self.group_rets.group1
-        self.inner_long_net_values = self.make_start_to_one(
-            (self.inner_rets_long + 1).cumprod()
-        )
-        self.inner_short_net_values = self.make_start_to_one(
-            (self.inner_rets_short + 1).cumprod()
-        )
+            self.long_short_net_values = (self.long_short_rets + 1).cumprod()
+        self.long_short_net_values = self.make_start_to_one(self.long_short_net_values)
         self.group_rets = self.group_rets.assign(long_short=self.long_short_rets)
         self.group_net_values = self.group_rets.applymap(lambda x: x + 1)
         self.group_net_values = self.group_net_values.cumprod()
         self.group_net_values = self.group_net_values.apply(self.make_start_to_one)
         a = groups_num ** (0.5)
         # 判断是否要两个因子画表格
         if a == int(a):
@@ -2020,34 +1794,18 @@
                 index=list(range(1, int(a) + 1)),
             )
             print("这是self.square_rets", self.square_rets)
 
     def get_long_short_comments(self, on_paper=False):
         """计算多空对冲的相关评价指标
         包括年化收益率、年化波动率、信息比率、月度胜率、最大回撤率"""
-        # week_here
         self.long_short_ret_yearly = (
-            self.long_short_net_values[-1]
-            ** (self.freq_ctrl.counts_one_year / len(self.long_short_net_values))
-            - 1
-        )
-        self.inner_long_ret_yearly = (
-            self.inner_long_net_values[-1]
-            ** (self.freq_ctrl.counts_one_year / len(self.inner_long_net_values))
-            - 1
-        )
-        self.inner_short_ret_yearly = (
-            self.inner_short_net_values[-1]
-            ** (self.freq_ctrl.counts_one_year / len(self.inner_short_net_values))
-            - 1
-        )
-        # week_here
-        self.long_short_vol_yearly = np.std(self.long_short_rets) * (
-            self.freq_ctrl.counts_one_year**0.5
+            self.long_short_net_values[-1] ** (12 / len(self.long_short_net_values)) - 1
         )
+        self.long_short_vol_yearly = np.std(self.long_short_rets) * (12**0.5)
         self.long_short_info_ratio = (
             self.long_short_ret_yearly / self.long_short_vol_yearly
         )
         self.long_short_win_times = len(self.long_short_rets[self.long_short_rets > 0])
         self.long_short_win_ratio = self.long_short_win_times / len(
             self.long_short_rets
         )
@@ -2062,163 +1820,102 @@
                         self.long_short_ret_yearly,
                         self.long_short_vol_yearly,
                         self.long_short_info_ratio,
                         self.long_short_win_ratio,
                         self.max_retreat,
                     ]
                 },
-                # week_here
-                index=[
-                    "年化收益率",
-                    "年化波动率",
-                    "收益波动比",
-                    f"{self.freq_ctrl.comment_name}度胜率",
-                    "最大回撤率",
-                ],
+                index=["年化收益率", "年化波动率", "收益波动比", "月度胜率", "最大回撤率"],
             )
         else:
             self.long_short_comments = pd.DataFrame(
                 {
                     "评价指标": [
                         self.long_short_ret_yearly,
                         self.long_short_vol_yearly,
                         self.long_short_info_ratio,
                         self.long_short_win_ratio,
                         self.max_retreat,
                     ]
                 },
-                # week_here
-                index=[
-                    "年化收益率",
-                    "年化波动率",
-                    "信息比率",
-                    f"{self.freq_ctrl.comment_name}度胜率",
-                    "最大回撤率",
-                ],
+                index=["年化收益率", "年化波动率", "信息比率", "月度胜率", "最大回撤率"],
             )
 
-    def get_total_comments(self, groups_num):
-        """综合IC、ICIR、RankIC、RankICIR,年化收益率、年化波动率、信息比率、胜率、最大回撤率"""
-        rankic = self.rankics.mean()
-        rankic_win = self.rankics[self.rankics * rankic > 0]
-        rankic_win_ratio = rankic_win.dropna().shape[0] / self.rankics.dropna().shape[0]
-        self.factor_cross_skew_after_neu = self.__factors_out.skew(axis=1).mean()
-        if self.ic_icir_and_rank.iloc[2, 0] > 0:
-            self.factor_turnover_rate = self.factor_turnover_rates[
-                f"group{groups_num}"
-            ].mean()
-        else:
-            self.factor_turnover_rate = self.factor_turnover_rates["group1"].mean()
+    def get_total_comments(self):
+        """综合IC、ICIR、RankIC、RankICIR,年化收益率、年化波动率、信息比率、月度胜率、最大回撤率"""
         self.total_comments = pd.concat(
             [
                 self.ic_icir_and_rank,
-                pd.DataFrame(
-                    {"评价指标": [rankic_win_ratio]},
-                    index=["RankIC胜率"],
-                ),
                 self.long_short_comments,
-                # week_here
-                pd.DataFrame(
-                    {
-                        "评价指标": [
-                            self.factor_turnover_rate,
-                            self.factor_cover,
-                            self.pos_neg_rate,
-                            self.factor_cross_skew,
-                            self.inner_long_ret_yearly,
-                            self.inner_long_ret_yearly
-                            / (
-                                self.inner_long_ret_yearly + self.inner_short_ret_yearly
-                            ),
-                            self.corr_itself,
-                        ]
-                    },
-                    index=[
-                        f"多头{self.freq_ctrl.comment_name}均换手",
-                        "因子覆盖率",
-                        "因子正值占比",
-                        "因子截面偏度",
-                        "多头超均收益",
-                        "多头收益占比",
-                        "一阶自相关性",
-                    ],
-                ),
+                pd.DataFrame({"评价指标": [self.factor_turnover_rate]}, index=["月均换手率"]),
             ]
         )
 
-    def plot_net_values(self, y2, filename, iplot=1, ilegend=1, without_breakpoint=0):
+    def plot_net_values(self, y2, filename, iplot=1, ilegend=1):
         """使用matplotlib来画图，y2为是否对多空组合采用双y轴"""
         if not iplot:
             fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(33, 8))
             self.group_net_values.plot(secondary_y=y2, rot=60, ax=ax[0])
             self.group_net_values.plot(secondary_y=y2, ax=ax[0])
             b = self.rankics.copy()
             b.index = [int(i.year) if i.month == 1 else "" for i in list(b.index)]
             b.plot(kind="bar", rot=60, ax=ax[1])
-            self.factor_cross_stds.plot(rot=60, ax=ax[2])
+            self.factor_turnover_rates.plot(rot=60, ax=ax[2])
 
             filename_path = filename + ".png"
             if not STATES["NO_SAVE"]:
                 plt.savefig(filename_path)
         else:
-            tris = (
-                pd.concat(
-                    [self.group_net_values, self.factor_cross_stds, self.rankics],
-                    axis=1,
-                )
-                .rename(columns={0: "因子截面标准差"})
-                .dropna()
-            )
-            if without_breakpoint:
-                tris = tris.dropna()
+            tris = pd.concat(
+                [self.group_net_values, self.factor_turnover_rates, self.rankics],
+                axis=1,
+            ).rename(columns={0: "turnover_rate"})
             figs = cf.figures(
                 tris,
                 [
                     dict(kind="line", y=list(self.group_net_values.columns)),
-                    dict(kind="bar", y="因子截面标准差"),
+                    dict(kind="line", y="turnover_rate"),
                     dict(kind="bar", y="rankic"),
                 ],
                 asList=True,
             )
             comments = (
                 self.total_comments.applymap(lambda x: round(x, 4))
                 .rename(index={"RankIC均值t值": "RankIC.t"})
                 .reset_index()
             )
             here = pd.concat(
                 [
-                    comments.iloc[:6, :].reset_index(drop=True),
-                    comments.iloc[6:12, :].reset_index(drop=True),
-                    comments.iloc[12:, :].reset_index(drop=True),
+                    comments.iloc[:5, :].reset_index(drop=True),
+                    comments.iloc[5:, :].reset_index(drop=True),
                 ],
                 axis=1,
             )
-            here.columns = ["信息系数", "结果", "绩效指标", "结果", "其他指标", "结果"]
+            here.columns = ["信息系数", "结果", "绩效指标", "结果"]
             # here=here.to_numpy().tolist()+[['信息系数','结果','绩效指标','结果']]
             table = FF.create_table(here.iloc[::-1])
             table.update_yaxes(matches=None)
             # table=go.Figure([go.Table(header=dict(values=list(here.columns)),cells=dict(values=here.to_numpy().tolist()))])
             figs.append(table)
             figs = [figs[-1]] + figs[:-1]
             figs[1].update_layout(
                 legend=dict(yanchor="top", y=0.99, xanchor="left", x=0.01)
             )
             base_layout = cf.tools.get_base_layout(figs)
 
             sp = cf.subplots(
                 figs,
-                shape=(2, 11),
+                shape=(2, 10),
                 base_layout=base_layout,
                 vertical_spacing=0.15,
                 horizontal_spacing=0.03,
                 shared_yaxes=False,
                 specs=[
                     [
-                        {"rowspan": 2, "colspan": 4},
-                        None,
+                        {"rowspan": 2, "colspan": 3},
                         None,
                         None,
                         {"rowspan": 2, "colspan": 4},
                         None,
                         None,
                         None,
                         {"colspan": 3},
@@ -2229,21 +1926,20 @@
                         None,
                         None,
                         None,
                         None,
                         None,
                         None,
                         None,
-                        None,
                         {"colspan": 3},
                         None,
                         None,
                     ],
                 ],
-                subplot_titles=["净值曲线", "因子截面标准差", "Rank IC时序图", "绩效指标"],
+                subplot_titles=["净值曲线", "月换手率", "Rank IC时序图", "绩效指标"],
             )
             sp["layout"].update(showlegend=ilegend)
             # los=sp['layout']['annotations']
             # los[0]['font']['color']='#000000'
             # los[1]['font']['color']='#000000'
             # los[2]['font']['color']='#000000'
             # los[3]['font']['color']='#000000'
@@ -2283,40 +1979,41 @@
     @classmethod
     @lru_cache(maxsize=None)
     def prerpare(cls):
         """通用数据准备"""
         cls.judge_month()
         cls.get_rets_month()
 
+    @kk.desktop_sender(title="嘿，回测结束啦～🗓")
     def run(
         self,
         groups_num=10,
         neutralize=False,
         boxcox=False,
-        trade_cost_double_side=0,
         value_weighted=False,
         y2=False,
         plt_plot=True,
         plotly_plot=False,
         filename="分组净值图",
+        time_start=None,
+        time_end=None,
         print_comments=True,
         comments_writer=None,
         net_values_writer=None,
         rets_writer=None,
         comments_sheetname=None,
         net_values_sheetname=None,
         rets_sheetname=None,
         on_paper=False,
         sheetname=None,
         zxindustry_dummies=0,
         swindustry_dummies=0,
         only_cap=0,
         iplot=1,
-        ilegend=0,
-        without_breakpoint=0,
+        ilegend=1,
     ):
         """运行回测部分"""
         if comments_writer and not (comments_sheetname or sheetname):
             raise IOError("把total_comments输出到excel中时，必须指定sheetname🤒")
         if net_values_writer and not (net_values_sheetname or sheetname):
             raise IOError("把group_net_values输出到excel中时，必须指定sheetname🤒")
         if rets_writer and not (rets_sheetname or sheetname):
@@ -2336,21 +2033,20 @@
                 only_cap=only_cap,
             )
             self.deal_with_factors_after_neutralize()
         else:
             self.deal_with_factors()
         self.get_limit_ups_downs()
         self.get_data(groups_num)
+        self.select_data_time(time_start, time_end)
         self.get_group_rets_net_values(
-            groups_num=groups_num,
-            value_weighted=value_weighted,
-            trade_cost_double_side=trade_cost_double_side,
+            groups_num=groups_num, value_weighted=value_weighted
         )
         self.get_long_short_comments(on_paper=on_paper)
-        self.get_total_comments(groups_num=groups_num)
+        self.get_total_comments()
         if on_paper:
             group1_ttest = ss.ttest_1samp(self.group_rets.group1, 0).pvalue
             group10_ttest = ss.ttest_1samp(
                 self.group_rets[f"group{groups_num}"], 0
             ).pvalue
             group_long_short_ttest = ss.ttest_1samp(self.long_short_rets, 0).pvalue
             group1_ret = self.group_rets.group1.mean()
@@ -2378,29 +2074,24 @@
             )
             self.total_comments = pd.concat([papers, self.total_comments])
 
         if plt_plot:
             if not STATES["NO_PLOT"]:
                 if filename:
                     self.plot_net_values(
-                        y2=y2,
-                        filename=filename,
-                        iplot=iplot,
-                        ilegend=bool(ilegend),
-                        without_breakpoint=without_breakpoint,
+                        y2=y2, filename=filename, iplot=iplot, ilegend=bool(ilegend)
                     )
                 else:
                     self.plot_net_values(
                         y2=y2,
                         filename=self.factors_file.split(".")[-2].split("/")[-1]
                         + str(groups_num)
                         + "分组",
                         iplot=iplot,
                         ilegend=bool(ilegend),
-                        without_breakpoint=without_breakpoint,
                     )
                 plt.show()
         if plotly_plot:
             if not STATES["NO_PLOT"]:
                 if filename:
                     self.plotly_net_values(filename=filename)
                 else:
@@ -2408,18 +2099,16 @@
                         filename=self.factors_file.split(".")[-2].split("/")[-1]
                         + str(groups_num)
                         + "分组"
                     )
         if print_comments:
             if not STATES["NO_COMMENT"]:
                 tb = Texttable()
-                tb.set_cols_width(
-                    [8] * 5 + [9] + [8] * 2 + [7] * 2 + [8] + [8] + [9] + [10] * 5
-                )
-                tb.set_cols_dtype(["f"] * 18)
+                tb.set_cols_width([8] * 4 + [12] + [8] * 2 + [7] * 2 + [8] + [10])
+                tb.set_cols_dtype(["f"] * 11)
                 tb.header(list(self.total_comments.T.columns))
                 tb.add_rows(self.total_comments.T.to_numpy(), header=False)
                 print(tb.draw())
         if sheetname:
             if comments_writer:
                 if not on_paper:
                     total_comments = self.total_comments.copy()
@@ -2427,25 +2116,18 @@
                     tc[0] = str(round(tc[0] * 100, 2)) + "%"
                     tc[1] = str(round(tc[1], 2))
                     tc[2] = str(round(tc[2] * 100, 2)) + "%"
                     tc[3] = str(round(tc[3], 2))
                     tc[4] = str(round(tc[4], 2))
                     tc[5] = str(round(tc[5] * 100, 2)) + "%"
                     tc[6] = str(round(tc[6] * 100, 2)) + "%"
-                    tc[7] = str(round(tc[7] * 100, 2)) + "%"
-                    tc[8] = str(round(tc[8], 2))
+                    tc[7] = str(round(tc[7], 2))
+                    tc[8] = str(round(tc[8] * 100, 2)) + "%"
                     tc[9] = str(round(tc[9] * 100, 2)) + "%"
                     tc[10] = str(round(tc[10] * 100, 2)) + "%"
-                    tc[11] = str(round(tc[11] * 100, 2)) + "%"
-                    tc[12] = str(round(tc[12] * 100, 2)) + "%"
-                    tc[13] = str(round(tc[13] * 100, 2)) + "%"
-                    tc[14] = str(round(tc[14], 2))
-                    tc[15] = str(round(tc[15], 2))
-                    tc[16] = str(round(tc[16] * 100, 2)) + "%"
-                    tc[17] = str(round(tc[17] * 100, 2)) + "%"
                     new_total_comments = pd.DataFrame(
                         {sheetname: tc}, index=total_comments.index
                     )
                     new_total_comments.T.to_excel(comments_writer, sheet_name=sheetname)
                 else:
                     self.total_comments.rename(columns={"评价指标": sheetname}).to_excel(
                         comments_writer, sheet_name=sheetname
@@ -2471,25 +2153,18 @@
                 tc[0] = str(round(tc[0] * 100, 2)) + "%"
                 tc[1] = str(round(tc[1], 2))
                 tc[2] = str(round(tc[2] * 100, 2)) + "%"
                 tc[3] = str(round(tc[3], 2))
                 tc[4] = str(round(tc[4], 2))
                 tc[5] = str(round(tc[5] * 100, 2)) + "%"
                 tc[6] = str(round(tc[6] * 100, 2)) + "%"
-                tc[7] = str(round(tc[7] * 100, 2)) + "%"
-                tc[8] = str(round(tc[8], 2))
+                tc[7] = str(round(tc[7], 2))
+                tc[8] = str(round(tc[8] * 100, 2)) + "%"
                 tc[9] = str(round(tc[9] * 100, 2)) + "%"
                 tc[10] = str(round(tc[10] * 100, 2)) + "%"
-                tc[11] = str(round(tc[11] * 100, 2)) + "%"
-                tc[12] = str(round(tc[12] * 100, 2)) + "%"
-                tc[13] = str(round(tc[13] * 100, 2)) + "%"
-                tc[14] = str(round(tc[14], 2))
-                tc[15] = str(round(tc[15], 2))
-                tc[16] = str(round(tc[16] * 100, 2)) + "%"
-                tc[17] = str(round(tc[17] * 100, 2)) + "%"
                 new_total_comments = pd.DataFrame(
                     {comments_sheetname: tc}, index=total_comments.index
                 )
                 new_total_comments.T.to_excel(
                     comments_writer, sheet_name=comments_sheetname
                 )
             if net_values_writer and net_values_sheetname:
@@ -2506,28 +2181,25 @@
                 group_rets.index = group_rets.index.strftime("%Y/%m/%d")
                 group_rets.columns = [
                     f"分组{i}" for i in range(1, len(list(group_rets.columns)))
                 ] + ["多空对冲（右轴）"]
                 group_rets.to_excel(rets_writer, sheet_name=rets_sheetname)
 
 
-@do_on_dfs
 class pure_moonnight(object):
     """封装选股框架"""
 
     __slots__ = ["shen"]
 
     def __init__(
         self,
         factors: pd.DataFrame,
         groups_num: int = 10,
-        freq: str = "M",
         neutralize: bool = 0,
         boxcox: bool = 1,
-        trade_cost_double_side: float = 0,
         value_weighted: bool = 0,
         y2: bool = 0,
         plt_plot: bool = 1,
         plotly_plot: bool = 0,
         filename: str = "分组净值图",
         time_start: int = None,
         time_end: int = None,
@@ -2549,53 +2221,46 @@
         closes: pd.DataFrame = None,
         capitals: pd.DataFrame = None,
         swindustry_dummy: pd.DataFrame = None,
         zxindustry_dummy: pd.DataFrame = None,
         no_read_indu: bool = 0,
         only_cap: bool = 0,
         iplot: bool = 1,
-        ilegend: bool = 0,
-        without_breakpoint: bool = 0,
-        opens_average_first_day: bool = 0,
-        total_cap: bool = 0,
+        ilegend: bool = 1,
     ) -> None:
         """一键回测框架，测试单因子的月频调仓的分组表现
         每月月底计算因子值，月初第一天开盘时买入，月末收盘最后一天收盘时卖出
         剔除上市不足60天的，停牌天数超过一半的，st天数超过一半的
         月末收盘跌停的不卖出，月初开盘涨停的不买入
         由最好组和最差组的多空组合构成多空对冲组
 
         Parameters
         ----------
         factors : pd.DataFrame
             要用于检测的因子值，index是时间，columns是股票代码
         groups_num : int, optional
             分组数量, by default 10
-        freq : str, optional
-            回测频率, by default 'M'
         neutralize : bool, optional
             对流通市值取自然对数，以完成行业市值中性化, by default 0
         boxcox : bool, optional
             对流通市值做截面boxcox变换，以完成行业市值中性化, by default 1
-        trade_cost_double_side : float, optional
-            交易的双边手续费率, by default 0
         value_weighted : bool, optional
             是否用流通市值加权, by default 0
         y2 : bool, optional
             画图时是否启用第二y轴, by default 0
         plt_plot : bool, optional
             将分组净值曲线用matplotlib画出来, by default 1
         plotly_plot : bool, optional
             将分组净值曲线用plotly画出来, by default 0
         filename : str, optional
             分组净值曲线的图保存的名称, by default "分组净值图"
         time_start : int, optional
-            回测起始时间, by default None
+            回测起始时间（此参数已废弃，请在因子上直接截断）, by default None
         time_end : int, optional
-            回测终止时间, by default None
+            回测终止时间（此参数已废弃，请在因子上直接截断）, by default None
         print_comments : bool, optional
             是否打印出评价指标, by default 1
         comments_writer : pd.ExcelWriter, optional
             用于记录评价指标的xlsx文件, by default None
         net_values_writer : pd.ExcelWriter, optional
             用于记录净值序列的xlsx文件, by default None
         rets_writer : pd.ExcelWriter, optional
@@ -2636,163 +2301,98 @@
             不读入行业数据, by default 0
         only_cap : bool, optional
             仅做市值中性化, by default 0
         iplot : bool, optional
             使用cufflinks呈现回测结果, by default 1
         ilegend : bool, optional
             使用cufflinks绘图时，是否显示图例, by default 1
-        without_breakpoint : bool, optional
-            画图的时候是否去除间断点, by default 0
-        opens_average_first_day : bool, optional
-            买入时使用第一天的平均价格, by default 0
-        total_cap : bool, optional
-            加权和行业市值中性化时使用总市值, by default 0
         """
 
         if not isinstance(factors, pd.DataFrame):
             factors = factors()
+        start = datetime.datetime.strftime(factors.index.min(), "%Y%m%d")
+        if ages is None:
+            ages = read_daily(age=1, start=start)
+        if sts is None:
+            sts = read_daily(st=1, start=start)
+        if states is None:
+            states = read_daily(state=1, start=start)
+        if opens is None:
+            opens = read_daily(open=1, start=start)
+        if closes is None:
+            closes = read_daily(close=1, start=start)
+        if capitals is None:
+            capitals = read_daily(flow_cap=1, start=start).resample("M").last()
         if comments_writer is None and sheetname is not None:
-            from pure_ocean_breeze.state.states import COMMENTS_WRITER
+            from pure_ocean_breeze.legacy_version.v3p4.state.states import COMMENTS_WRITER
 
             comments_writer = COMMENTS_WRITER
         if net_values_writer is None and sheetname is not None:
-            from pure_ocean_breeze.state.states import NET_VALUES_WRITER
+            from pure_ocean_breeze.legacy_version.v3p4.state.states import NET_VALUES_WRITER
 
             net_values_writer = NET_VALUES_WRITER
         if not on_paper:
-            from pure_ocean_breeze.state.states import ON_PAPER
+            from pure_ocean_breeze.legacy_version.v3p4.state.states import ON_PAPER
 
             on_paper = ON_PAPER
-        if time_start is None:
-            from pure_ocean_breeze.state.states import MOON_START
+        from pure_ocean_breeze.legacy_version.v3p4.state.states import MOON_START
 
-            if MOON_START is not None:
-                factors = factors[factors.index >= pd.Timestamp(str(MOON_START))]
-        else:
-            factors = factors[factors.index >= pd.Timestamp(str(time_start))]
-        if time_end is None:
-            from pure_ocean_breeze.state.states import MOON_END
+        if MOON_START is not None:
+            factors = factors[factors.index >= pd.Timestamp(str(MOON_START))]
+        from pure_ocean_breeze.legacy_version.v3p4.state.states import MOON_END
 
-            if MOON_END is not None:
-                factors = factors[factors.index <= pd.Timestamp(str(MOON_END))]
-        else:
-            factors = factors[factors.index <= pd.Timestamp(str(time_end))]
+        if MOON_END is not None:
+            factors = factors[factors.index <= pd.Timestamp(str(MOON_END))]
         if boxcox + neutralize == 0:
             no_read_indu = 1
         if only_cap + no_read_indu > 0:
             only_cap = no_read_indu = 1
         if iplot:
             print_comments = 0
-        if total_cap:
-            if opens_average_first_day:
-                if freq == "M":
-                    self.shen = pure_moon_b(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-                elif freq == "W":
-                    self.shen = pure_week_b(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-            else:
-                if freq == "M":
-                    self.shen = pure_moon_c(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-                elif freq == "W":
-                    self.shen = pure_week_c(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-        else:
-            if opens_average_first_day:
-                if freq == "M":
-                    self.shen = pure_moon(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-                elif freq == "W":
-                    self.shen = pure_week(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-            else:
-                if freq == "M":
-                    self.shen = pure_moon_a(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
-                elif freq == "W":
-                    self.shen = pure_week_a(
-                        freq=freq,
-                        no_read_indu=no_read_indu,
-                        swindustry_dummy=swindustry_dummy,
-                        zxindustry_dummy=zxindustry_dummy,
-                        read_in_swindustry_dummy=swindustry_dummies,
-                    )
+        self.shen = pure_moon(
+            no_read_indu=no_read_indu,
+            swindustry_dummy=swindustry_dummy,
+            zxindustry_dummy=zxindustry_dummy,
+            read_in_swindustry_dummy=swindustry_dummies,
+        )
         self.shen.set_basic_data(
-            ages=ages,
-            sts=sts,
-            states=states,
-            opens=opens,
-            closes=closes,
-            capitals=capitals,
-            opens_average_first_day=opens_average_first_day,
-            total_cap=total_cap,
+            age=ages,
+            st=sts,
+            state=states,
+            open=opens,
+            close=closes,
+            capital=capitals,
         )
         self.shen.set_factor_df_date_as_index(factors)
         self.shen.prerpare()
         self.shen.run(
             groups_num=groups_num,
             neutralize=neutralize,
             boxcox=boxcox,
-            trade_cost_double_side=trade_cost_double_side,
             value_weighted=value_weighted,
             y2=y2,
             plt_plot=plt_plot,
             plotly_plot=plotly_plot,
             filename=filename,
+            time_start=time_start,
+            time_end=time_end,
             print_comments=print_comments,
             comments_writer=comments_writer,
             net_values_writer=net_values_writer,
             rets_writer=rets_writer,
             comments_sheetname=comments_sheetname,
             net_values_sheetname=net_values_sheetname,
             rets_sheetname=rets_sheetname,
             on_paper=on_paper,
             sheetname=sheetname,
             swindustry_dummies=swindustry_dummies,
             zxindustry_dummies=zxindustry_dummies,
             only_cap=only_cap,
             iplot=iplot,
             ilegend=ilegend,
-            without_breakpoint=without_breakpoint,
         )
 
     def __call__(self) -> pd.DataFrame:
         """如果做了行业市值中性化，则返回行业市值中性化之后的因子数据
 
         Returns
         -------
@@ -2817,64 +2417,24 @@
             net = self.shen.group_net_values[i]
             com = comments_on_twins(net, ret)
             com = com.to_frame(i)
             coms.append(com)
         df = pd.concat(coms, axis=1)
         return df.T
 
-    def comment_yearly(self) -> pd.DataFrame:
-        """对回测的每年表现给出评价
-
-        Returns
-        -------
-        pd.DataFrame
-            各年度的收益率
-        """
-        df = self.shen.group_net_values.resample("Y").last().pct_change()
-        df.index = df.index.year
-        return df
-
-
-class pure_week(pure_moon):
-    ...
-
-
-class pure_moon_a(pure_moon):
-    ...
-
-
-class pure_week_a(pure_moon):
-    ...
-
-
-class pure_moon_b(pure_moon):
-    ...
-
-
-class pure_week_b(pure_moon):
-    ...
-
-
-class pure_moon_c(pure_moon):
-    ...
-
-
-class pure_week_c(pure_moon):
-    ...
-
 
 class pure_fall(object):
     # DONE：修改为因子文件名可以带“日频_“，也可以不带“日频_“
     def __init__(self, daily_path: str) -> None:
         """一个使用mysql中的分钟数据，来更新因子值的框架
 
         Parameters
         ----------
         daily_path : str
-            日频因子值存储文件的名字，请以'.parquet'结尾
+            日频因子值存储文件的名字，请以'.feather'结尾
         """
         self.homeplace = HomePlace()
         # 将分钟数据拼成一张日频因子表
         self.daily_factors = None
         self.daily_factors_path = self.homeplace.factor_data_file + "日频_" + daily_path
 
     def __call__(self, monthly=False):
@@ -2883,14 +2443,160 @@
             return self.monthly_factors.copy()
         else:
             try:
                 return self.daily_factors.copy()
             except Exception:
                 return self.monthly_factors.copy()
 
+    def __add__(self, selfas):
+        """将几个因子截面标准化之后，因子值相加"""
+        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
+        fac2s = []
+        if not isinstance(selfas, Iterable):
+            if not STATES["NO_LOG"]:
+                logger.warning(f"{selfas} is changed into Iterable")
+            selfas = (selfas,)
+        for selfa in selfas:
+            fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
+            fac2s.append(fac2)
+        for i in fac2s:
+            fac1 = fac1 + i
+        new_pure = pure_fall()
+        new_pure.monthly_factors = fac1
+        return new_pure
+
+    def __mul__(self, selfas):
+        """将几个因子横截面标准化之后，使其都为正数，然后因子值相乘"""
+        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
+        fac1 = fac1 - fac1.min()
+        fac2s = []
+        if not isinstance(selfas, Iterable):
+            if not STATES["NO_LOG"]:
+                logger.warning(f"{selfas} is changed into Iterable")
+            selfas = (selfas,)
+        for selfa in selfas:
+            fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
+            fac2 = fac2 - fac2.min()
+            fac2s.append(fac2)
+        for i in fac2s:
+            fac1 = fac1 * i
+        new_pure = pure_fall()
+        new_pure.monthly_factors = fac1
+        return new_pure
+
+    def __truediv__(self, selfa):
+        """两个一正一副的因子，可以用此方法相减"""
+        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
+        fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
+        fac = fac1 - fac2
+        new_pure = pure_fall()
+        new_pure.monthly_factors = fac
+        return new_pure
+
+    def __floordiv__(self, selfa):
+        """两个因子一正一负，可以用此方法相除"""
+        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
+        fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
+        fac1 = fac1 - fac1.min()
+        fac2 = fac2 - fac2.min()
+        fac = fac1 / fac2
+        fac = fac.replace(np.inf, np.nan)
+        new_pure = pure_fall()
+        new_pure.monthly_factors = fac
+        return new_pure
+
+    @kk.desktop_sender(title="嘿，正交化结束啦～🐬")
+    def __sub__(self, selfa):
+        """用主因子剔除其他相关因子、传统因子等
+        selfa可以为多个因子对象组成的元组或列表，每个辅助因子只需要有月度因子文件路径即可"""
+        if is_notebook():
+            tqdm.tqdm_notebook().pandas()
+        else:
+            tqdm.tqdm.pandas()
+        if not isinstance(selfa, Iterable):
+            if not STATES["NO_LOG"]:
+                logger.warning(f"{selfa} is changed into Iterable")
+            selfa = (selfa,)
+        fac_main = self.wide_to_long(self.monthly_factors, "fac")
+        fac_helps = [i.monthly_factors for i in selfa]
+        help_names = ["help" + str(i) for i in range(1, (len(fac_helps) + 1))]
+        fac_helps = list(map(self.wide_to_long, fac_helps, help_names))
+        fac_helps = pd.concat(fac_helps, axis=1)
+        facs = pd.concat([fac_main, fac_helps], axis=1).dropna()
+        facs = facs.groupby("date").progress_apply(
+            lambda x: self.de_in_group(x, help_names)
+        )
+        facs = facs.unstack()
+        facs.columns = list(map(lambda x: x[1], list(facs.columns)))
+        return facs
+
+    def __gt__(self, selfa):
+        """用于输出25分组表格，使用时，以x>y的形式使用，其中x,y均为pure_fall对象
+        计算时使用的是他们的月度因子表，即self.monthly_factors属性，为宽数据形式的dataframe
+        x应为首先用来的分组的主因子，y为在x分组后的组内继续分组的次因子"""
+        x = self.monthly_factors.copy()
+        y = selfa.monthly_factors.copy()
+        x = x.stack().reset_index()
+        y = y.stack().reset_index()
+        x.columns = ["date", "code", "fac"]
+        y.columns = ["date", "code", "fac"]
+        shen = pure_moon()
+        x = x.groupby("date").apply(lambda df: shen.get_groups(df, 5))
+        x = (
+            x.reset_index(drop=True)
+            .drop(columns=["fac"])
+            .rename(columns={"group": "groupx"})
+        )
+        xy = pd.merge(x, y, on=["date", "code"])
+        xy = xy.groupby(["date", "groupx"]).apply(lambda df: shen.get_groups(df, 5))
+        xy = (
+            xy.reset_index(drop=True)
+            .drop(columns=["fac"])
+            .rename(columns={"group": "groupy"})
+        )
+        xy = xy.assign(fac=xy.groupx * 5 + xy.groupy)
+        xy = xy[["date", "code", "fac"]]
+        xy = xy.set_index(["date", "code"]).unstack()
+        xy.columns = [i[1] for i in list(xy.columns)]
+        new_pure = pure_fall()
+        new_pure.monthly_factors = xy
+        return new_pure
+
+    def __rshift__(self, selfa):
+        """用于输出100分组表格，使用时，以x>>y的形式使用，其中x,y均为pure_fall对象
+        计算时使用的是他们的月度因子表，即self.monthly_factors属性，为宽数据形式的dataframe
+        x应为首先用来的分组的主因子，y为在x分组后的组内继续分组的次因子"""
+        x = self.monthly_factors.copy()
+        y = selfa.monthly_factors.copy()
+        x = x.stack().reset_index()
+        y = y.stack().reset_index()
+        x.columns = ["date", "code", "fac"]
+        y.columns = ["date", "code", "fac"]
+        shen = pure_moon()
+        x = x.groupby("date").apply(lambda df: shen.get_groups(df, 10))
+        x = (
+            x.reset_index(drop=True)
+            .drop(columns=["fac"])
+            .rename(columns={"group": "groupx"})
+        )
+        xy = pd.merge(x, y, on=["date", "code"])
+        xy = xy.groupby(["date", "groupx"]).apply(lambda df: shen.get_groups(df, 10))
+        xy = (
+            xy.reset_index(drop=True)
+            .drop(columns=["fac"])
+            .rename(columns={"group": "groupy"})
+        )
+        xy = xy.assign(fac=xy.groupx * 10 + xy.groupy)
+        xy = xy[["date", "code", "fac"]]
+        xy = xy.set_index(["date", "code"]).unstack()
+        xy.columns = [i[1] for i in list(xy.columns)]
+        new_pure = pure_fall()
+        new_pure.monthly_factors = xy
+        return new_pure
+
     def wide_to_long(self, df, i):
         """将宽数据转化为长数据，用于因子表转化和拼接"""
         df = df.stack().reset_index()
         df.columns = ["date", "code", i]
         df = df.set_index(["date", "code"])
         return df
 
@@ -2922,20 +2628,14 @@
         the_func = partial(func)
         df = df.groupby(["code"]).apply(the_func).to_frame()
         df.columns = [str(day)]
         df = df.T
         df.index = pd.to_datetime(df.index, format="%Y%m%d")
         return df
 
-    @deprecation.deprecated(
-        deprecated_in="3.7.5",
-        removed_in="4.0",
-        current_version=__version__,
-        details="使用mysql提取分钟数据并更新因子值的方法功能局限且严重滞后，将移除👋",
-    )
     @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
     def get_daily_factors_alter(self, func: Callable) -> None:
         """用mysql逐日更新分钟数据构造的因子
 
         Parameters
         ----------
         func : Callable
@@ -2945,50 +2645,61 @@
         ------
         `IOError`
             如果没有历史因子数据，将报错
         """
         """通过minute_data_stock_alter数据库一天一天计算因子值"""
         try:
             try:
-                self.daily_factors = pd.read_parquet(self.daily_factors_path)
+                self.daily_factors = pd.read_feather(self.daily_factors_path)
             except Exception:
                 self.daily_factors_path = self.daily_factors_path.split("日频_")
                 self.daily_factors_path = (
                     self.daily_factors_path[0] + self.daily_factors_path[1]
                 )
-                self.daily_factors = drop_duplicates_index(
-                    pd.read_parquet(self.daily_factors_path)
-                )
+                self.daily_factors = pd.read_feather(self.daily_factors_path)
+            self.daily_factors = self.daily_factors.rename(
+                columns={list(self.daily_factors.columns)[0]: "date"}
+            )
+            self.daily_factors = self.daily_factors.drop_duplicates(
+                subset=["date"], keep="last"
+            )
+            self.daily_factors = self.daily_factors.set_index("date")
             sql = sqlConfig("minute_data_stock_alter")
             now_minute_datas = sql.show_tables(full=False)
             now_minute_data = now_minute_datas[-1]
             now_minute_data = pd.Timestamp(now_minute_data)
             if self.daily_factors.index.max() < now_minute_data:
                 if not STATES["NO_LOG"]:
                     logger.info(
                         f"上次存储的因子值到{self.daily_factors.index.max()}，而分钟数据最新到{now_minute_data}，开始更新……"
                     )
                 old_end = datetime.datetime.strftime(
                     self.daily_factors.index.max(), "%Y%m%d"
                 )
                 now_minute_datas = [i for i in now_minute_datas if i > old_end]
                 dfs = []
-                for c in tqdm.auto.tqdm(now_minute_datas, desc="桂棹兮兰桨，击空明兮遂流光🌊"):
+                for c in tqdm.tqdm(now_minute_datas, desc="桂棹兮兰桨，击空明兮遂流光🌊"):
                     df = self.get_single_day_factor(func, c)
                     dfs.append(df)
                 dfs = pd.concat(dfs)
                 dfs = dfs.sort_index()
                 self.daily_factors = pd.concat([self.daily_factors, dfs])
                 self.daily_factors = self.daily_factors.dropna(how="all")
                 self.daily_factors = self.daily_factors[
                     self.daily_factors.index >= pd.Timestamp(str(STATES["START"]))
                 ]
-            drop_duplicates_index(self.daily_factors).to_parquet(
-                self.daily_factors_path
+            self.daily_factors = self.daily_factors.reset_index()
+            self.daily_factors = self.daily_factors.rename(
+                columns={list(self.daily_factors.columns)[0]: "date"}
             )
+            self.daily_factors = self.daily_factors.drop_duplicates(
+                subset=["date"], keep="first"
+            )
+            self.daily_factors = self.daily_factors.set_index("date")
+            self.daily_factors.reset_index().to_feather(self.daily_factors_path)
             if not STATES["NO_LOG"]:
                 logger.success("更新已完成")
 
         except Exception:
             raise IOError(
                 "您还没有该因子的初级数据，暂时不能更新。请先使用pure_fall_frequent或pure_fall_flexible计算历史因子值。"
             )
@@ -3045,15 +2756,18 @@
             fac1 = fac1 * i
         new_pure = pure_fall()
         new_pure.monthly_factors = fac1
         return new_pure
 
     def __sub__(self, selfa):
         """返回对象，如需表格，请调用对象"""
-        tqdm.auto.tqdm.pandas()
+        if is_notebook():
+            tqdm.tqdm_notebook().pandas()
+        else:
+            tqdm.tqdm.pandas()
         if not isinstance(selfa, Iterable):
             if not STATES["NO_LOG"]:
                 logger.warning(f"{selfa} is changed into Iterable")
             selfa = (selfa,)
         fac_main = self.wide_to_long(self.monthly_factors, "fac")
         fac_helps = [i.monthly_factors for i in selfa]
         help_names = ["help" + str(i) for i in range(1, (len(fac_helps) + 1))]
@@ -3133,115 +2847,112 @@
 
 class pure_fall_frequent(object):
     """对单只股票单日进行操作"""
 
     def __init__(
         self,
         factor_file: str,
-        project: str = None,
         startdate: int = None,
         enddate: int = None,
-        questdb_host: str = "127.0.0.1",
         kind: str = "stock",
         clickhouse: bool = 0,
         questdb: bool = 0,
-        questdb_web_port: str = "9001",
         ignore_history_in_questdb: bool = 0,
         groupby_target: list = ["date", "code"],
     ) -> None:
         """基于clickhouse的分钟数据，计算因子值，每天的因子值只用到当日的数据
 
         Parameters
         ----------
         factor_file : str
-            用于保存因子值的文件名，需为parquet文件，以'.parquet'结尾
-        project : str, optional
-            该因子所属项目，即子文件夹名称, by default None
+            用于保存因子值的文件名，需为feather文件，以'.feather'结尾
         startdate : int, optional
             起始时间，形如20121231，为开区间, by default None
         enddate : int, optional
             截止时间，形如20220814，为闭区间，为空则计算到最近数据, by default None
-        questdb_host: str, optional
-            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
         kind : str, optional
             类型为股票还是指数，指数为'index', by default "stock"
         clickhouse : bool, optional
             使用clickhouse作为数据源，如果postgresql与本参数都为0，将依然从clickhouse中读取, by default 0
         questdb : bool, optional
             使用questdb作为数据源, by default 0
-        questdb_web_port : str, optional
-            questdb的web_port, by default '9001'
         ignore_history_in_questdb : bool, optional
             打断后重新从头计算，清除在questdb中的记录
         groupby_target: list, optional
             groupby计算时，分组的依据，使用此参数时，自定义函数的部分，如果指定按照['date']分组groupby计算，
             则返回时，应当返回一个两列的dataframe，第一列为股票代码，第二列为为因子值, by default ['date','code']
         """
         homeplace = HomePlace()
         self.kind = kind
         self.groupby_target = groupby_target
         if clickhouse == 0 and questdb == 0:
             clickhouse = 1
         self.clickhouse = clickhouse
         self.questdb = questdb
-        self.questdb_web_port = questdb_web_port
         if clickhouse == 1:
             # 连接clickhouse
             self.chc = ClickHouseClient("minute_data")
         elif questdb == 1:
-            self.chc = Questdb(host=questdb_host, web_port=questdb_web_port)
+            self.chc = Questdb()
         # 将计算到一半的因子，存入questdb中，避免中途被打断后重新计算，表名即为因子文件名的汉语拼音
         pinyin = Pinyin()
         self.factor_file_pinyin = pinyin.get_pinyin(
-            factor_file.replace(".parquet", ""), ""
+            factor_file.replace(".feather", ""), ""
         )
-        self.factor_steps = Questdb(host=questdb_host, web_port=questdb_web_port)
-        if project is not None:
-            if not os.path.exists(homeplace.factor_data_file + project):
-                os.makedirs(homeplace.factor_data_file + project)
-            else:
-                logger.info(f"当前正在{project}项目中……")
-        else:
-            logger.warning("当前因子不属于任何项目，这将造成因子数据文件夹的混乱，不便于管理，建议指定一个项目名称")
+        self.factor_steps = Questdb()
         # 完整的因子文件路径
-        if project is not None:
-            factor_file = homeplace.factor_data_file + project + "/" + factor_file
-        else:
-            factor_file = homeplace.factor_data_file + factor_file
+        factor_file = homeplace.factor_data_file + factor_file
         self.factor_file = factor_file
         # 读入之前的因子
         if os.path.exists(factor_file):
-            factor_old = drop_duplicates_index(pd.read_parquet(self.factor_file))
+            factor_old = pd.read_feather(self.factor_file)
+            factor_old.columns = ["date"] + list(factor_old.columns)[1:]
+            factor_old = factor_old.drop_duplicates(subset=["date"])
+            factor_old = factor_old.set_index("date")
             self.factor_old = factor_old
             # 已经算好的日子
             dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
             self.dates_old = dates_old
         elif (not ignore_history_in_questdb) and self.factor_file_pinyin in list(
             self.factor_steps.get_data("show tables").table
         ):
             logger.info(
                 f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，现在将读取上次的数据，继续计算"
             )
-            factor_old = self.factor_steps.get_data_with_tuple(
-                f"select * from '{self.factor_file_pinyin}'"
-            ).drop_duplicates(subset=["date", "code"])
+            factor_old = self.factor_steps.get_data(
+                f"select * from {self.factor_file_pinyin}"
+            )
+            # 判断一下每天是否生成多个数据，单个数据就以float形式存储，多个数据以list形式存储
+            if "f0" in list(factor_old.columns):
+                factor_old = factor_old[factor_old.f0 != "date"]
+                factor_old.columns = ["date", "code", "fac"]
+                try:
+                    factor_old.fac = factor_old.fac.apply(
+                        lambda x: [float(i) for i in x[1:-1].split(" ") if i != ""]
+                    )
+                except Exception:
+                    factor_old.fac = factor_old.fac.apply(
+                        lambda x: [float(i) for i in x[1:-1].split(", ") if i != ""]
+                    )
             factor_old = factor_old.pivot(index="date", columns="code", values="fac")
+            factor_old.index = pd.to_datetime(factor_old.index)
             factor_old = factor_old.sort_index()
+            factor_old = drop_duplicates_index(factor_old)
             self.factor_old = factor_old
             # 已经算好的日子
             dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
             self.dates_old = dates_old
         elif ignore_history_in_questdb and self.factor_file_pinyin in list(
             self.factor_steps.get_data("show tables").table
         ):
             logger.info(
                 f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，但您选择重新计算，所以正在删除原来的数据，从头计算"
             )
             factor_old = self.factor_steps.do_order(
-                f"drop table '{self.factor_file_pinyin}'"
+                f"drop table {self.factor_file_pinyin}"
             )
             self.factor_old = None
             self.dates_old = []
             logger.info("删除完毕，正在重新计算")
         else:
             self.factor_old = None
             self.dates_old = []
@@ -3291,25 +3002,14 @@
         Returns
         -------
         `pd.DataFrame`
             经运算产生的因子值
         """
         return self.factor.copy()
 
-    def forward_dates(self, dates, many_days):
-        dates_index = [self.dates_all.index(i) for i in dates]
-
-        def value(x, a):
-            if x >= 0:
-                return a[x]
-            else:
-                return None
-
-        return [value(i - many_days, self.dates_all) for i in dates_index]
-
     def select_one_calculate(
         self,
         date: pd.Timestamp,
         func: Callable,
         fields: str = "*",
         show_time: bool = 0,
     ) -> None:
@@ -3335,174 +3035,162 @@
             df = df.sort_values(["date", "num"])
         df = df.groupby(self.groupby_target).apply(the_func)
         if self.groupby_target == ["date", "code"]:
             df = df.to_frame("fac").reset_index()
             df.columns = ["date", "code", "fac"]
         else:
             df = df.reset_index()
-        if (df is not None) and (df.shape[0] > 0):
-            df = df.pivot(columns="code", index="date", values="fac")
-            df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-            to_save = df.stack().reset_index()
-            to_save.columns = ["date", "code", "fac"]
-            self.factor_steps.write_via_df(
-                to_save, self.factor_file_pinyin, tuple_col="fac"
-            )
-            return df
+        df = df.pivot(columns="code", index="date", values="fac")
+        df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+        return df
 
     def select_many_calculate(
         self,
-        dates: List[pd.Timestamp],
+        dates: list[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
-        many_days: int = 1,
-        n_jobs: int = 1,
+        tqdm_inside: bool = 0,
     ) -> None:
         the_func = partial(func)
-        factor_new = []
         dates = [int(datetime.datetime.strftime(i, "%Y%m%d")) for i in dates]
-        if many_days == 1:
-            # 将需要更新的日子分块，每200天一组，一起运算
-            dates_new_len = len(dates)
-            cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
-            if cut_points[-1] == cut_points[-2]:
-                cut_points = cut_points[:-1]
-            cuts = tuple(zip(cut_points[:-many_days], cut_points[many_days:]))
-            df_first = self.select_one_calculate(
-                date=dates[0],
-                func=func,
-                fields=fields,
-                show_time=show_time,
-            )
-            factor_new.append(df_first)
-
-            def cal_one(date1, date2):
+        # 将需要更新的日子分块，每200天一组，一起运算
+        dates_new_len = len(dates)
+        cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
+        if cut_points[-1] == cut_points[-2]:
+            cut_points = cut_points[:-1]
+        cut_first = cut_points[0]
+        cuts = tuple(zip(cut_points[:-1], cut_points[1:]))
+        print(f"共{len(cuts)}段")
+        factor_new = []
+        df_first = self.select_one_calculate(
+            date=dates[0],
+            func=func,
+            fields=fields,
+            show_time=show_time,
+        )
+        factor_new.append(df_first)
+        to_save = df_first.stack().reset_index()
+        to_save.columns = ["date", "code", "fac"]
+        self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
+
+        if tqdm_inside == 1:
+            # 开始计算因子值
+            for date1, date2 in cuts:
                 if self.clickhouse == 1:
                     sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
                 else:
-                    sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]} order by code,date,num"
+                    sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]}"
                 if show_time:
                     df = self.chc.get_data_show_time(sql_order)
                 else:
                     df = self.chc.get_data(sql_order)
                 if self.clickhouse == 1:
                     df = ((df.set_index("code")) / 100).reset_index()
                 else:
                     df.num = df.num.astype(int)
                     df.date = df.date.astype(int)
                     df = df.sort_values(["date", "num"])
-                df = df.groupby(self.groupby_target).apply(the_func)
-                if self.groupby_target == ["date", "code"]:
-                    df = df.to_frame("fac").reset_index()
-                    df.columns = ["date", "code", "fac"]
+                if is_notebook():
+                    tqdm.tqdm_notebook().pandas()
                 else:
-                    df = df.reset_index()
+                    tqdm.tqdm.pandas()
+                df = df.groupby(self.groupby_target).progress_apply(the_func)
+                df = df.to_frame("fac").reset_index()
+                df.columns = ["date", "code", "fac"]
                 df = df.pivot(columns="code", index="date", values="fac")
                 df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                factor_new.append(df)
                 to_save = df.stack().reset_index()
                 to_save.columns = ["date", "code", "fac"]
-                self.factor_steps.write_via_df(
-                    to_save, self.factor_file_pinyin, tuple_col="fac"
-                )
-                return df
-
-            if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    factor_new_more = pool.map(cal_one, cuts, progress_bar=True)
-                factor_new = factor_new + factor_new_more
-            else:
+                self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
+        else:
+            if is_notebook():
                 # 开始计算因子值
-                for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
-                    df = cal_one(date1, date2)
+                for date1, date2 in tqdm.tqdm_notebook(cuts, desc="不知乘月几人归，落月摇情满江树。"):
+                    if self.clickhouse == 1:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
+                    else:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1]} and date<={dates[date2]} order by code,date,num"
+                    if show_time:
+                        df = self.chc.get_data_show_time(sql_order)
+                    else:
+                        df = self.chc.get_data(sql_order)
+                    if self.clickhouse == 1:
+                        df = ((df.set_index("code")) / 100).reset_index()
+                    df = df.groupby(self.groupby_target).apply(the_func)
+                    if self.groupby_target == ["date", "code"]:
+                        df = df.to_frame("fac").reset_index()
+                        df.columns = ["date", "code", "fac"]
+                    else:
+                        df = df.reset_index()
+                    df = df.pivot(columns="code", index="date", values="fac")
+                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
                     factor_new.append(df)
-        else:
-
-            def cal_two(date1, date2):
-                if date1 is not None:
+                    to_save = df.stack().reset_index()
+                    to_save.columns = ["date", "code", "fac"]
+                    self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
+            else:
+                # 开始计算因子值
+                for date1, date2 in tqdm.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
                     if self.clickhouse == 1:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{date1*100} and date<={date2*100} order by code,date,num"
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
                     else:
-                        sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{date1} and cast(date as int)<={date2} order by code,date,num"
+                        sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]}"
                     if show_time:
                         df = self.chc.get_data_show_time(sql_order)
                     else:
                         df = self.chc.get_data(sql_order)
                     if self.clickhouse == 1:
                         df = ((df.set_index("code")) / 100).reset_index()
                     else:
                         df.num = df.num.astype(int)
                         df.date = df.date.astype(int)
                         df = df.sort_values(["date", "num"])
-                    if self.groupby_target == [
-                        "date",
-                        "code",
-                    ] or self.groupby_target == ["code"]:
-                        df = df.groupby(["code"]).apply(the_func).reset_index()
+                    df = df.groupby(self.groupby_target).apply(the_func)
+                    if self.groupby_target == ["date", "code"]:
+                        df = df.to_frame("fac").reset_index()
+                        df.columns = ["date", "code", "fac"]
                     else:
-                        df = the_func(df)
-                    df = df.assign(date=date2)
-                    df.columns = ["code", "fac", "date"]
+                        df = df.reset_index()
                     df = df.pivot(columns="code", index="date", values="fac")
                     df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                    factor_new.append(df)
                     to_save = df.stack().reset_index()
                     to_save.columns = ["date", "code", "fac"]
-                    self.factor_steps.write_via_df(
-                        to_save, self.factor_file_pinyin, tuple_col="fac"
-                    )
-                    return df
-
-            pairs = self.forward_dates(dates, many_days=many_days)
-            cuts2 = tuple(zip(pairs, dates))
-            if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    factor_new_more = pool.map(cal_two, cuts2, progress_bar=True)
-                factor_new = factor_new + factor_new_more
-            else:
-                # 开始计算因子值
-                for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
-                    df = cal_two(date1, date2)
-                    factor_new.append(df)
-
-        if len(factor_new) > 0:
-            factor_new = pd.concat(factor_new)
-            return factor_new
-        else:
-            return None
+                    self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
+        factor_new = pd.concat(factor_new)
+        return factor_new
 
     def select_any_calculate(
         self,
-        dates: List[pd.Timestamp],
+        dates: list[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
-        many_days: int = 1,
-        n_jobs: int = 1,
+        tqdm_inside: bool = 0,
     ) -> None:
-        if len(dates) == 1 and many_days == 1:
+        if len(dates) == 1:
             res = self.select_one_calculate(
                 dates[0],
                 func=func,
                 fields=fields,
                 show_time=show_time,
             )
         else:
             res = self.select_many_calculate(
                 dates=dates,
                 func=func,
                 fields=fields,
                 chunksize=chunksize,
                 show_time=show_time,
-                many_days=many_days,
-                n_jobs=n_jobs,
+                tqdm_inside=tqdm_inside,
             )
-        if res is not None:
-            self.factor_new.append(res)
         return res
 
     @staticmethod
     def for_cross_via_str(func):
         """返回值为两层的list，每一个里层的小list为单个股票在这一天的返回值
         例如
         ```python
@@ -3536,45 +3224,31 @@
                 )
         ```
         上例中，每个股票一天返回两个因子值，每个pd.Series对应一个因子值
         """
 
         def full_run(df, *args, **kwargs):
             res = func(df, *args, **kwargs)
-            if isinstance(res, pd.Series):
-                res = res.reset_index()
-                res.columns = ["code", "fac"]
-                return res
-            elif isinstance(res, pd.DataFrame):
-                res.columns = [f"fac{i}" for i in range(len(res.columns))]
-                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
-                res = res[["fac"]].reset_index()
-                res.columns = ["code", "fac"]
-                return res
-            elif res is None:
-                ...
-            else:
-                res = pd.concat(res, axis=1)
-                res.columns = [f"fac{i}" for i in range(len(res.columns))]
-                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
-                res = res[["fac"]].reset_index()
-                res.columns = ["code", "fac"]
-                return res
+            res = pd.concat(res, axis=1)
+            res.columns = [f"fac{i}" for i in range(len(res.columns))]
+            res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+            res = res[["fac"]].reset_index()
+            res.columns = ["code", "fac"]
+            return res
 
         return full_run
 
     @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
     def get_daily_factors(
         self,
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
-        many_days: int = 1,
-        n_jobs: int = 1,
+        tqdm_inside: bool = 0,
     ) -> None:
         """每次抽取chunksize天的截面上全部股票的分钟数据
         对每天的股票的数据计算因子值
 
         Parameters
         ----------
         func : Callable
@@ -3582,67 +3256,292 @@
         fields : str, optional
             股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
             提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
         chunksize : int, optional
             每次读取的截面上的天数, by default 10
         show_time : bool, optional
             展示每次读取数据所需要的时间, by default 0
-        many_days : int, optional
-            计算某天的因子值时，需要使用之前多少天的数据
-        n_jobs : int, optional
-            并行数量，不建议设置为大于2的数，此外当此参数大于1时，请使用questdb数据库来读取分钟数据, by default 1
+        tqdm_inside : bool, optional
+            将进度条加在内部，而非外部，建议仅chunksize较大时使用, by default 0
         """
         if len(self.dates_new) > 0:
             for interval in self.dates_new_intervals:
                 df = self.select_any_calculate(
                     dates=interval,
                     func=func,
                     fields=fields,
                     chunksize=chunksize,
                     show_time=show_time,
-                    many_days=many_days,
-                    n_jobs=n_jobs,
+                    tqdm_inside=tqdm_inside,
                 )
+                self.factor_new.append(df)
             self.factor_new = pd.concat(self.factor_new)
             # 拼接新的和旧的
             self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
-            self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
+            self.factor = self.factor.dropna(how="all")
+            self.factor = self.factor.reset_index()
+            self.factor = self.factor.rename(
+                columns={list(self.factor.columns)[0]: "date"}
+            )
+            self.factor = self.factor.drop_duplicates(subset=["date"], keep="first")
+            self.factor = self.factor.set_index("date")
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             # 存入本地
-            self.factor.to_parquet(self.factor_file)
+            self.factor.reset_index().to_feather(self.factor_file)
             logger.info(f"截止到{new_end_date}的因子值计算完了")
             # 删除存储在questdb的中途备份数据
-            try:
-                self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
-                logger.info("备份在questdb的表格已删除")
-            except Exception:
-                logger.warning("删除questdb中表格时，存在某个未知错误，请当心")
+            self.factor_steps.do_order(f"drop table {self.factor_file_pinyin}")
+            logger.info("备份在questdb的表格已删除")
 
         else:
-            self.factor = drop_duplicates_index(self.factor_old)
+            self.factor = self.factor_old
+            self.factor = self.factor.reset_index()
+            self.factor = self.factor.rename(
+                columns={list(self.factor.columns)[0]: "date"}
+            )
+            self.factor = self.factor.drop_duplicates(subset=["date"], keep="first")
+            self.factor = self.factor.set_index("date")
             # 存入本地
-            self.factor.to_parquet(self.factor_file)
+            self.factor.reset_index().to_feather(self.factor_file)
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
 
-    def drop_table(self):
-        """直接删除存储在questdb中的暂存数据"""
-        try:
-            self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
-            logger.success(f"暂存在questdb中的数据表格'{self.factor_file_pinyin}'已经删除")
-        except Exception:
-            logger.warning(f"您要删除的表格'{self.factor_file_pinyin}'已经不存在了，请检查")
+
+class pure_fall_flexible(object):
+    def __init__(
+        self,
+        factor_file: str,
+        startdate: int = None,
+        enddate: int = None,
+        kind: str = "stock",
+        clickhouse: bool = 0,
+        questdb: bool = 0,
+    ) -> None:
+        """基于clickhouse的分钟数据，计算因子值，每天的因子值用到多日的数据，或者用到截面的数据
+        对一段时间的截面数据进行操作，在get_daily_factors的func函数中
+        请写入df=df.groupby([xxx]).apply(fff)之类的语句
+        然后单独定义一个函数，作为要apply的fff，可以在apply上加进度条
+
+        Parameters
+        ----------
+        factor_file : str
+            用于存储因子的文件名称，请以'.feather'结尾
+        startdate : int, optional
+            计算因子的起始日期，形如20220816, by default None
+        enddate : int, optional
+            计算因子的终止日期，形如20220816, by default None
+        kind : str, optional
+            指定计算股票还是指数，指数则为'index', by default "stock"
+        clickhouse : bool, optional
+            使用clickhouse作为数据源，如果postgresql与本参数都为0，将依然从clickhouse中读取, by default 0
+        questdb : bool, optional
+            使用questdb作为数据源, by default 0
+        """
+        homeplace = HomePlace()
+        self.kind = kind
+        if clickhouse == 0 and questdb == 0:
+            clickhouse = 1
+        self.clickhouse = clickhouse
+        self.questdb = questdb
+        if clickhouse == 1:
+            # 连接clickhouse
+            self.chc = ClickHouseClient("minute_data")
+        elif questdb:
+            self.chc = Questdb()
+        # 完整的因子文件路径
+        factor_file = homeplace.factor_data_file + factor_file
+        self.factor_file = factor_file
+        # 读入之前的因子
+        if os.path.exists(factor_file):
+            factor_old = pd.read_feather(self.factor_file)
+            factor_old.columns = ["date"] + list(factor_old.columns)[1:]
+            factor_old = factor_old.drop_duplicates(subset=["date"])
+            factor_old = factor_old.set_index("date")
+            self.factor_old = factor_old
+            # 已经算好的日子
+            dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
+            self.dates_old = dates_old
+        else:
+            self.factor_old = None
+            self.dates_old = []
+            logger.info("这个因子以前没有，正在重新计算")
+        # 读取当前所有的日子
+        dates_all = self.chc.show_all_dates(f"minute_data_{kind}")
+        if startdate is None:
+            ...
+        else:
+            dates_all = [i for i in dates_all if i >= startdate]
+        if enddate is None:
+            ...
+        else:
+            dates_all = [i for i in dates_all if i <= enddate]
+        self.dates_all = dates_all
+        # 需要新补充的日子
+        self.dates_new = sorted([i for i in dates_all if i not in dates_old])
+
+    def __call__(self) -> pd.DataFrame:
+        """直接返回因子值的pd.DataFrame
+
+        Returns
+        -------
+        `pd.DataFrame`
+            计算出的因子值
+        """
+        return self.factor.copy()
+
+    @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
+    def get_daily_factors(
+        self,
+        func: Callable,
+        fields: str = "*",
+        chunksize: int = 250,
+        show_time: bool = 0,
+        tqdm_inside: bool = 0,
+    ) -> None:
+        """每次抽取chunksize天的截面上全部股票的分钟数据
+        依照定义的函数计算因子值
+
+        Parameters
+        ----------
+        func : Callable
+            用于计算因子值的函数
+        fields : str, optional
+            股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
+            提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
+        chunksize : int, optional
+            每次读取的截面上的天数, by default 10
+        show_time : bool, optional
+            展示每次读取数据所需要的时间, by default 0
+        tqdm_inside : bool, optional
+            将进度条加在内部，而非外部，建议仅chunksize较大时使用, by default 0
+        """
+        the_func = partial(func)
+        # 将需要更新的日子分块，每200天一组，一起运算
+        dates_new_len = len(self.dates_new)
+        if dates_new_len > 0:
+            cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
+            if cut_points[-1] == cut_points[-2]:
+                cut_points = cut_points[:-1]
+            self.cut_points = cut_points
+            self.factor_new = []
+            # 开始计算因子值
+            if tqdm_inside:
+                # 开始计算因子值
+                for date1, date2 in cut_points:
+                    if self.clickhouse == 1:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]*100} and date<={self.dates_new[date2]*100} order by code,date,num"
+                    else:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]} and date<={self.dates_new[date2]}"
+                    if show_time:
+                        df = self.chc.get_data_show_time(sql_order)
+                    else:
+                        df = self.chc.get_data(sql_order)
+                    if self.clickhouse == 1:
+                        df = ((df.set_index("code")) / 100).reset_index()
+                    if is_notebook():
+                        tqdm.tqdm_notebook().pandas()
+                    else:
+                        tqdm.tqdm.pandas()
+                    df = the_func(df)
+                    if isinstance(df, pd.Series):
+                        df = df.reset_index()
+                    df.columns = ["date", "code", "fac"]
+                    df = df.pivot(columns="code", index="date", values="fac")
+                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                    self.factor_new.append(df)
+            else:
+                # 开始计算因子值
+                for date1, date2 in tqdm.tqdm(cut_points, desc="不知乘月几人归，落月摇情满江树。"):
+                    if self.clickhouse == 1:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]*100} and date<={self.dates_new[date2]*100} order by code,date,num"
+                    else:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]} and date<={self.dates_new[date2]} order by code,date,num"
+                    if show_time:
+                        df = self.chc.get_data_show_time(sql_order)
+                    else:
+                        df = self.chc.get_data(sql_order)
+                    if self.clickhouse == 1:
+                        df = ((df.set_index("code")) / 100).reset_index()
+                    df = the_func(df)
+                    if isinstance(df, pd.Series):
+                        df = df.reset_index()
+                    df.columns = ["date", "code", "fac"]
+                    df = df.pivot(columns="code", index="date", values="fac")
+                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                    self.factor_new.append(df)
+            self.factor_new = pd.concat(self.factor_new)
+            # 拼接新的和旧的
+            self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            # 存入本地
+            self.factor.reset_index().to_feather(self.factor_file)
+            logger.info(f"截止到{new_end_date}的因子值计算完了")
+        elif dates_new_len == 1:
+            print("共1天")
+            if tqdm_inside:
+                # 开始计算因子值
+                if self.clickhouse == 1:
+                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]*100} order by code,date,num"
+                else:
+                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]} order by code,date,num"
+                if show_time:
+                    df = self.chc.get_data_show_time(sql_order)
+                else:
+                    df = self.chc.get_data(sql_order)
+                if self.clickhouse == 1:
+                    df = ((df.set_index("code")) / 100).reset_index()
+                tqdm.tqdm.pandas()
+                df = the_func(df)
+                if isinstance(df, pd.Series):
+                    df = df.reset_index()
+                df.columns = ["date", "code", "fac"]
+                df = df.pivot(columns="code", index="date", values="fac")
+                df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+            else:
+                # 开始计算因子值
+                if self.clickhouse == 1:
+                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]*100} order by code,date,num"
+                else:
+                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]} order by code,date,num"
+                if show_time:
+                    df = self.chc.get_data_show_time(sql_order)
+                else:
+                    df = self.chc.get_data(sql_order)
+                if self.clickhouse == 1:
+                    df = ((df.set_index("code")) / 100).reset_index()
+                df = the_func(df)
+                if isinstance(df, pd.Series):
+                    df = df.reset_index()
+                df.columns = ["date", "code", "fac"]
+                df = df.pivot(columns="code", index="date", values="fac")
+                df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                self.factor_new.append(df)
+            self.factor_new = df
+            # 拼接新的和旧的
+            self.factor = (
+                pd.concat([self.factor_old, self.factor_new])
+                .sort_index()
+                .drop_duplicates()
+            )
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            # 存入本地
+            self.factor.reset_index().to_feather(self.factor_file)
+            logger.info(f"补充{self.dates_new[0]}截止到{new_end_date}的因子值计算完了")
+        else:
+            self.factor = self.factor_old
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
 
 
 class pure_coldwinter(object):
     # DONE: 可以自由添加其他要剔除的因子，或者替换某些要剔除的因子
 
     def __init__(
         self,
-        facs_dict: Dict = None,
+        facs_dict: dict = None,
         momentum: bool = 1,
         earningsyield: bool = 1,
         growth: bool = 1,
         liquidity: bool = 1,
         size: bool = 1,
         leverage: bool = 1,
         beta: bool = 1,
@@ -3650,15 +3549,15 @@
         residualvolatility: bool = 1,
         booktoprice: bool = 1,
     ) -> None:
         """读入10种常用风格因子，并可以额外加入其他因子
 
         Parameters
         ----------
-        facs_dict : Dict, optional
+        facs_dict : dict, optional
             额外加入的因子，名字为key，因子矩阵为value，形如`{'反转': ret20, '换手': tr20}`, by default None
         momentum : bool, optional
             是否删去动量因子, by default 1
         earningsyield : bool, optional
             是否删去盈利因子, by default 1
         growth : bool, optional
             是否删去成长因子, by default 1
@@ -3676,19 +3575,21 @@
             是否删去残差波动率因子, by default 1
         booktoprice : bool, optional
             是否删去账面市值比因子, by default 1
         """
         self.homeplace = HomePlace()
         # barra因子数据
         styles = os.listdir(self.homeplace.barra_data_file)
-        styles = [i for i in styles if i.endswith(".parquet")]
+        styles = [i for i in styles if i.endswith(".feather")]
         barras = {}
         for s in styles:
             k = s.split(".")[0]
-            v = pd.read_parquet(self.homeplace.barra_data_file + s)
+            v = pd.read_feather(self.homeplace.barra_data_file + s)
+            v.columns = ["date"] + list(v.columns)[1:]
+            v = v.set_index("date")
             barras[k] = v
         rename_dict = {
             "fac": "因子自身",
             "size": "市值",
             "nonlinearsize": "非线性市值",
             "booktoprice": "估值",
             "earningsyield": "盈利",
@@ -3784,15 +3685,15 @@
             [self.factors] + list(self.barras.values()), axis=1
         ).dropna()
 
     # DONE: 修改风格因子展示顺序至报告的顺序
     def get_corr(self):
         """计算每一期的相关系数，再求平均值"""
         self.corr_by_step = self.corr_pri.groupby(["date"]).apply(
-            lambda x: x.rank().corr().head(1)
+            lambda x: x.corr().head(1)
         )
         self.__corr = self.corr_by_step.mean()
         self.__corr = self.__corr.rename(index=self.rename_dict)
         self.__corr = self.__corr.to_frame("相关系数").T
 
         self.__corr = self.__corr[self.sort_names]
         self.__corr = self.__corr.T
@@ -3835,22 +3736,21 @@
         self.get_monthly_barras_industrys()
         self.get_wide_barras_industrys()
         self.get_corr_pri_ols_pri()
         self.get_corr()
         self.get_snow_fac()
 
 
-@do_on_dfs
 class pure_snowtrain(object):
     """直接返回纯净因子"""
 
     def __init__(
         self,
         factors: pd.DataFrame,
-        facs_dict: Dict = None,
+        facs_dict: dict = None,
         momentum: bool = 1,
         earningsyield: bool = 1,
         growth: bool = 1,
         liquidity: bool = 1,
         size: bool = 1,
         leverage: bool = 1,
         beta: bool = 1,
@@ -3860,36 +3760,36 @@
     ) -> None:
         """计算因子值与10种常用风格因子之间的相关性，并进行纯净化，可以额外加入其他因子
 
         Parameters
         ----------
         factors : pd.DataFrame
             要考察的因子值，index为时间，columns为股票代码，values为因子值
-        facs_dict : Dict, optional
-            额外加入的因子，名字为key，因子矩阵为value，形如`{'反转': ret20, '换手': tr20}`, by default None
+        facs_dict : dict, optional
+            _description_, by default None
         momentum : bool, optional
-            是否删去动量因子, by default 1
+            _description_, by default 1
         earningsyield : bool, optional
-            是否删去盈利因子, by default 1
+            _description_, by default 1
         growth : bool, optional
-            是否删去成长因子, by default 1
+            _description_, by default 1
         liquidity : bool, optional
-            是否删去流动性因子, by default 1
+            _description_, by default 1
         size : bool, optional
-            是否删去规模因子, by default 1
+            _description_, by default 1
         leverage : bool, optional
-            是否删去杠杆因子, by default 1
+            _description_, by default 1
         beta : bool, optional
-            是否删去贝塔因子, by default 1
+            _description_, by default 1
         nonlinearsize : bool, optional
-            是否删去非线性市值因子, by default 1
+            _description_, by default 1
         residualvolatility : bool, optional
-            是否删去残差波动率因子, by default 1
+            _description_, by default 1
         booktoprice : bool, optional
-            是否删去账面市值比因子, by default 1
+            _description_, by default 1
         """
         self.winter = pure_coldwinter(
             facs_dict=facs_dict,
             momentum=momentum,
             earningsyield=earningsyield,
             growth=growth,
             liquidity=liquidity,
@@ -3910,34 +3810,23 @@
         Returns
         -------
         pd.DataFrame
             纯净化之后的因子值
         """
         return self.winter.snow_fac.copy()
 
-    def show_corr(self) -> pd.DataFrame:
-        """展示因子与barra风格因子的相关系数
-
-        Returns
-        -------
-        pd.DataFrame
-            相关系数表格
-        """
-        return self.corr.T.applymap(lambda x: to_percent(x))
-
 
 class pure_newyear(object):
     """转为生成25分组和百分组的收益矩阵而封装"""
 
     def __init__(
         self,
         facx: pd.DataFrame,
         facy: pd.DataFrame,
         group_num_single: int,
-        trade_cost_double_side: float = 0,
         namex: str = "主",
         namey: str = "次",
     ) -> None:
         """条件双变量排序法，先对所有股票，依照因子facx进行排序
         然后在每个组内，依照facy进行排序，最后统计各个组内的平均收益率
 
         Parameters
@@ -3946,33 +3835,27 @@
             首先进行排序的因子，通常为控制变量，相当于正交化中的自变量
             index为时间，columns为股票代码，values为因子值
         facy : pd.DataFrame
             在facx的各个组内，依照facy进行排序，为主要要研究的因子
             index为时间，columns为股票代码，values为因子值
         group_num_single : int
             单个因子分成几组，通常为5或10
-        trade_cost_double_side : float, optional
-            交易的双边手续费率, by default 0
         namex : str, optional
             facx这一因子的名字, by default "主"
         namey : str, optional
             facy这一因子的名字, by default "次"
         """
         homex = pure_fallmount(facx)
         homey = pure_fallmount(facy)
         if group_num_single == 5:
             homexy = homex > homey
         elif group_num_single == 10:
             homexy = homex >> homey
         shen = pure_moonnight(
-            homexy(),
-            group_num_single**2,
-            trade_cost_double_side=trade_cost_double_side,
-            plt_plot=False,
-            print_comments=False,
+            homexy(), group_num_single**2, plt_plot=False, print_comments=False
         )
         sq = shen.shen.square_rets.copy()
         sq.index = [namex + str(i) for i in list(sq.index)]
         sq.columns = [namey + str(i) for i in list(sq.columns)]
         self.square_rets = sq
 
     def __call__(self) -> pd.DataFrame:
@@ -3982,528 +3865,290 @@
         -------
         `pd.DataFrame`
             每个组的年化收益率
         """
         return self.square_rets.copy()
 
 
-@do_on_dfs
+class pure_dawn(object):
+    """
+    因子切割论的母框架，可以对两个因子进行类似于因子切割的操作
+    可用于派生任何"以两个因子生成一个因子"的子类
+    使用举例
+    cut函数里，必须带有输入变量df,df有两个columns，一个名为'fac1'，一个名为'fac2'，df是最近一个回看期内的数据
+    ```python
+    class Cut(pure_dawn):
+
+    def cut(self,df):
+        df=df.sort_values('fac1')
+        df=df.assign(fac3=df.fac1*df.fac2)
+        ret0=df.fac2.iloc[:4].mean()
+        ret1=df.fac2.iloc[4:8].mean()
+        ret2=df.fac2.iloc[8:12].mean()
+        ret3=df.fac2.iloc[12:16].mean()
+        ret4=df.fac2.iloc[16:].mean()
+        aret0=df.fac3.iloc[:4].mean()
+        aret1=df.fac3.iloc[4:8].mean()
+        aret2=df.fac3.iloc[8:12].mean()
+        aret3=df.fac3.iloc[12:16].mean()
+        aret4=df.fac3.iloc[16:].mean()
+        return ret0,ret1,ret2,ret3,ret4,aret0,aret1,aret2,aret3,aret4
+
+    cut=Cut(ct,ret_inday)
+    cut.run(cut.cut)
+
+    cut0=get_value(cut(),0)
+    cut1=get_value(cut(),1)
+    cut2=get_value(cut(),2)
+    cut3=get_value(cut(),3)
+    cut4=get_value(cut(),4)
+    ```
+    """
+
+    def __init__(self, fac1: pd.DataFrame, fac2: pd.DataFrame, *args: list) -> None:
+        """几个因子的操作，每个月操作一次
+
+        Parameters
+        ----------
+        fac1 : pd.DataFrame
+            因子值1，index为时间，columns为股票代码，values为因子值
+        fac2 : pd.DataFrame
+            因子2，index为时间，columns为股票代码，values为因子值
+        """
+        self.fac1 = fac1
+        self.fac1 = self.fac1.stack().reset_index()
+        self.fac1.columns = ["date", "code", "fac1"]
+        self.fac2 = fac2
+        self.fac2 = self.fac2.stack().reset_index()
+        self.fac2.columns = ["date", "code", "fac2"]
+        fac_all = pd.merge(self.fac1, self.fac2, on=["date", "code"])
+        for i, fac in enumerate(args):
+            fac = fac.stack().reset_index()
+            fac.columns = ["date", "code", f"fac{i+3}"]
+            fac_all = pd.merge(fac_all, fac, on=["date", "code"])
+        fac_all = fac_all.sort_values(["date", "code"])
+        self.fac = fac_all.copy()
+
+    def __call__(self) -> pd.DataFrame:
+        """返回最终月度因子值
+
+        Returns
+        -------
+        `pd.DataFrame`
+            最终因子值
+        """
+        return self.fac.copy()
+
+    def get_fac_long_and_tradedays(self):
+        """将两个因子的矩阵转化为长列表"""
+        self.tradedays = sorted(list(set(self.fac.date)))
+
+    def get_month_starts_and_ends(self, backsee=20):
+        """计算出每个月回看期间的起点日和终点日"""
+        self.month_ends = [
+            i
+            for i, j in zip(self.tradedays[:-1], self.tradedays[1:])
+            if i.month != j.month
+        ]
+        self.month_ends.append(self.tradedays[-1])
+        self.month_starts = [
+            self.find_begin(self.tradedays, i, backsee=backsee) for i in self.month_ends
+        ]
+        self.month_starts[0] = self.tradedays[0]
+
+    def find_begin(self, tradedays, end_day, backsee=20):
+        """找出回看若干天的开始日，默认为20"""
+        end_day_index = tradedays.index(end_day)
+        start_day_index = end_day_index - backsee + 1
+        start_day = tradedays[start_day_index]
+        return start_day
+
+    def make_monthly_factors_single_code(self, df, func):
+        """
+        对单一股票来计算月度因子
+        func为单月执行的函数，返回值应为月度因子，如一个float或一个list
+        df为一个股票的四列表，包含时间、代码、因子1和因子2
+        """
+        res = {}
+        for start, end in zip(self.month_starts, self.month_ends):
+            this_month = df[(df.date >= start) & (df.date <= end)]
+            res[end] = func(this_month)
+        dates = list(res.keys())
+        corrs = list(res.values())
+        part = pd.DataFrame({"date": dates, "corr": corrs})
+        return part
+
+    def get_monthly_factor(self, func):
+        """运行自己写的函数，获得月度因子"""
+        if is_notebook():
+            tqdm.tqdm_notebook().pandas()
+        else:
+            tqdm.tqdm.pandas(desc="when the dawn comes, tonight will be a memory too.")
+        self.fac = self.fac.groupby(["code"]).progress_apply(
+            lambda x: self.make_monthly_factors_single_code(x, func)
+        )
+        self.fac = (
+            self.fac.reset_index(level=1, drop=True)
+            .reset_index()
+            .set_index(["date", "code"])
+            .unstack()
+        )
+        self.fac.columns = [i[1] for i in list(self.fac.columns)]
+        self.fac = self.fac.resample("M").last()
+
+    @kk.desktop_sender(title="嘿，切割完成啦🛁")
+    def run(self, func: Callable, backsee: int = 20) -> None:
+        """执行计算的框架，产生因子值
+
+        Parameters
+        ----------
+        func : Callable
+            每个月要进行的操作
+        backsee : int, optional
+            回看期，即每个月月底对过去多少天进行计算, by default 20
+        """
+        self.get_fac_long_and_tradedays()
+        self.get_month_starts_and_ends(backsee=backsee)
+        self.get_monthly_factor(func)
+
+
 def follow_tests(
     fac: pd.DataFrame,
-    trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
-    index_member_value_weighted: bool = 1,
     comments_writer: pd.ExcelWriter = None,
     net_values_writer: pd.ExcelWriter = None,
     pos: bool = 0,
     neg: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
-    nums: List[int] = [3],
-    opens_average_first_day: bool = 0,
-    total_cap: bool = 0,
+    nums: list[int] = [3],
 ):
     """因子完成全A测试后，进行的一些必要的后续测试，包括各个分组表现、相关系数与纯净化、3510的多空和多头、各个行业Rank IC、各个行业买3只超额表现
 
     Parameters
     ----------
     fac : pd.DataFrame
         要进行后续测试的因子值，index是时间，columns是股票代码，values是因子值
-    trade_cost_double_side : float, optional
-        交易的双边手续费率, by default 0
-    index_member_value_weighted : bool, optional
-        成分股多头采取流通市值加权
     comments_writer : pd.ExcelWriter, optional
         写入评价指标的excel, by default None
     net_values_writer : pd.ExcelWriter, optional
         写入净值序列的excel, by default None
     pos : bool, optional
         因子的方向为正, by default 0
     neg : bool, optional
         因子的方向为负, by default 0
     swindustry : bool, optional
         使用申万一级行业, by default 0
     zxindustry : bool, optional
         使用中信一级行业, by default 0
-    nums : List[int], optional
+    nums : list[int], optional
         各个行业买几只股票, by default [3]
-    opens_average_first_day : bool, optional
-        买入时使用第一天的平均价格, by default 0
-    total_cap : bool, optional
-        加权和行业市值中性化时使用总市值, by default 0
 
     Raises
     ------
     IOError
         如果未指定因子正负方向，将报错
     """
     if comments_writer is None:
-        from pure_ocean_breeze.state.states import COMMENTS_WRITER
+        from pure_ocean_breeze.legacy_version.v3p4.state.states import COMMENTS_WRITER
 
         comments_writer = COMMENTS_WRITER
     if net_values_writer is None:
-        from pure_ocean_breeze.state.states import NET_VALUES_WRITER
+        from pure_ocean_breeze.legacy_version.v3p4.state.states import NET_VALUES_WRITER
 
         net_values_writer = NET_VALUES_WRITER
 
-    shen = pure_moonnight(
-        fac,
-        opens_average_first_day=opens_average_first_day,
-    )
-    if (
-        shen.shen.group_net_values.group1.iloc[-1]
-        > shen.shen.group_net_values.group10.iloc[-1]
-    ):
-        neg = 1
-    else:
-        pos = 1
-    if comments_writer is not None:
-        shen.comments_ten().to_excel(comments_writer, sheet_name="十分组")
-    print(shen.comments_ten())
+    shen = pure_moonnight(fac)
+    shen.comments_ten().to_excel(comments_writer, sheet_name="十分组")
     """相关系数与纯净化"""
     pure_fac = pure_snowtrain(fac)
-    if comments_writer is not None:
-        pure_fac.corr.to_excel(comments_writer, sheet_name="相关系数")
-    print(pure_fac.corr)
+    pure_fac.corr.to_excel(comments_writer, sheet_name="相关系数")
     shen = pure_moonnight(
         pure_fac(),
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="纯净",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
     )
     """3510多空和多头"""
     # 300
     fi300 = daily_factor_on300500(fac, hs300=1)
     shen = pure_moonnight(
         fi300,
-        value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="300多空",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
     )
     if pos:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group10, hs300=1).to_excel(
-                comments_writer, sheet_name="300超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group10
-                    - shen.shen.factor_turnover_rates.group10 * i,
-                    hs300=1,
-                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group10, hs300=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group10, hs300=1).to_excel(
-                net_values_writer, sheet_name="300超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group10
-                    - shen.shen.factor_turnover_rates.group10 * i,
-                    hs300=1,
-                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group10, hs300=1)
+        make_relative_comments(shen.shen.group_rets.group10, hs300=1).to_excel(
+            comments_writer, sheet_name="300超额"
+        )
+        make_relative_comments_plot(shen.shen.group_rets.group10, hs300=1).to_excel(
+            net_values_writer, sheet_name="300超额"
+        )
     elif neg:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
-                comments_writer, sheet_name="300超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    hs300=1,
-                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group1, hs300=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
-                net_values_writer, sheet_name="300超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    hs300=1,
-                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1)
+        make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
+            comments_writer, sheet_name="300超额"
+        )
+        make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
+            net_values_writer, sheet_name="300超额"
+        )
     else:
         raise IOError("请指定因子的方向是正是负🤒")
     # 500
     fi500 = daily_factor_on300500(fac, zz500=1)
     shen = pure_moonnight(
         fi500,
-        value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="500多空",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
     )
     if pos:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group10, zz500=1).to_excel(
-                comments_writer, sheet_name="500超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group10
-                    - shen.shen.factor_turnover_rates.group10 * i,
-                    zz500=1,
-                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group10, zz500=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group10, zz500=1).to_excel(
-                net_values_writer, sheet_name="500超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group10
-                    - shen.shen.factor_turnover_rates.group10 * i,
-                    zz500=1,
-                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group10, zz500=1)
+        make_relative_comments(shen.shen.group_rets.group10, zz500=1).to_excel(
+            comments_writer, sheet_name="500超额"
+        )
+        make_relative_comments_plot(shen.shen.group_rets.group10, zz500=1).to_excel(
+            net_values_writer, sheet_name="500超额"
+        )
     else:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
-                comments_writer, sheet_name="500超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz500=1,
-                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group1, zz500=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
-                net_values_writer, sheet_name="500超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz500=1,
-                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1)
+        make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
+            comments_writer, sheet_name="500超额"
+        )
+        make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
+            net_values_writer, sheet_name="500超额"
+        )
     # 1000
     fi1000 = daily_factor_on300500(fac, zz1000=1)
     shen = pure_moonnight(
         fi1000,
-        value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="1000多空",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
     )
     if pos:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group10, zz1000=1).to_excel(
-                comments_writer, sheet_name="1000超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group10
-                    - shen.shen.factor_turnover_rates.group10 * i,
-                    zz1000=1,
-                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group10, zz1000=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(
-                shen.shen.group_rets.group10, zz1000=1
-            ).to_excel(net_values_writer, sheet_name="1000超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group10
-                    - shen.shen.factor_turnover_rates.group10 * i,
-                    zz1000=1,
-                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group10, zz1000=1)
+        make_relative_comments(shen.shen.group_rets.group10, zz1000=1).to_excel(
+            comments_writer, sheet_name="1000超额"
+        )
+        make_relative_comments_plot(shen.shen.group_rets.group10, zz1000=1).to_excel(
+            net_values_writer, sheet_name="1000超额"
+        )
     else:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
-                comments_writer, sheet_name="1000超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz1000=1,
-                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group1, zz1000=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
-                net_values_writer, sheet_name="1000超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz1000=1,
-                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1)
+        make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
+            comments_writer, sheet_name="1000超额"
+        )
+        make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
+            net_values_writer, sheet_name="1000超额"
+        )
     # 各行业Rank IC
     rankics = rankic_test_on_industry(fac, comments_writer)
     # 买3只超额表现
     rets = long_test_on_industry(
         fac, nums, pos=pos, neg=neg, swindustry=swindustry, zxindustry=zxindustry
     )
     logger.success("因子后续的必要测试全部完成")
 
 
-def test_on_index_four_out(
-    fac: pd.DataFrame,
-    value_weighted: bool = 1,
-    trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
-    group_num: int = 10,
-    boxcox: bool = 1,
-    comments_writer: pd.ExcelWriter = None,
-    net_values_writer: pd.ExcelWriter = None,
-    opens_average_first_day: bool = 0,
-    total_cap: bool = 0,
-):
-    if comments_writer is None:
-        from pure_ocean_breeze.state.states import COMMENTS_WRITER
-
-        comments_writer = COMMENTS_WRITER
-    if net_values_writer is None:
-        from pure_ocean_breeze.state.states import NET_VALUES_WRITER
-
-        net_values_writer = NET_VALUES_WRITER
-
-    shen = pure_moonnight(
-        fac,
-        opens_average_first_day=opens_average_first_day,
-    )
-    if (
-        shen.shen.group_net_values.group1.iloc[-1]
-        > shen.shen.group_net_values10.iloc[-1]
-    ):
-        neg = 1
-        pos = 0
-    else:
-        pos = 1
-        neg = 0
-
-    """3510多空和多头"""
-    # 300
-    fi300 = daily_factor_on300500(fac, hs300=1)
-    shen = pure_moonnight(
-        fi300,
-        value_weighted=value_weighted,
-        groups_num=group_num,
-        boxcox=boxcox,
-        comments_writer=comments_writer,
-        net_values_writer=net_values_writer,
-        sheetname="300多空",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
-    )
-    if pos:
-        if comments_writer is not None:
-            make_relative_comments(
-                shen.shen.group_rets[f"group{group_num}"], hs300=1
-            ).to_excel(comments_writer, sheet_name="300超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets[f"group{group_num}"]
-                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
-                    hs300=1,
-                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], hs300=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(
-                shen.shen.group_rets[f"group{group_num}"], hs300=1
-            ).to_excel(net_values_writer, sheet_name="300超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets[f"group{group_num}"]
-                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
-                    hs300=1,
-                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments_plot(
-                shen.shen.group_rets[f"group{group_num}"], hs300=1
-            )
-    elif neg:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
-                comments_writer, sheet_name="300超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    hs300=1,
-                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group1, hs300=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
-                net_values_writer, sheet_name="300超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    hs300=1,
-                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1)
-    else:
-        raise IOError("请指定因子的方向是正是负🤒")
-    # 500
-    fi500 = daily_factor_on300500(fac, zz500=1)
-    shen = pure_moonnight(
-        fi500,
-        value_weighted=value_weighted,
-        groups_num=group_num,
-        boxcox=boxcox,
-        comments_writer=comments_writer,
-        net_values_writer=net_values_writer,
-        sheetname="500多空",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
-    )
-    if pos:
-        if comments_writer is not None:
-            make_relative_comments(
-                shen.shen.group_rets[f"group{group_num}"], zz500=1
-            ).to_excel(comments_writer, sheet_name="500超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets[f"group{group_num}"]
-                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
-                    zz500=1,
-                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], zz500=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(
-                shen.shen.group_rets[f"group{group_num}"], zz500=1
-            ).to_excel(net_values_writer, sheet_name="500超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets[f"group{group_num}"]
-                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
-                    zz500=1,
-                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments_plot(
-                shen.shen.group_rets[f"group{group_num}"], zz500=1
-            )
-    else:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
-                comments_writer, sheet_name="500超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz500=1,
-                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group1, zz500=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
-                net_values_writer, sheet_name="500超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz500=1,
-                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1)
-    # 1000
-    fi1000 = daily_factor_on300500(fac, zz1000=1)
-    shen = pure_moonnight(
-        fi1000,
-        value_weighted=value_weighted,
-        groups_num=group_num,
-        boxcox=boxcox,
-        comments_writer=comments_writer,
-        net_values_writer=net_values_writer,
-        sheetname="1000多空",
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
-    )
-    if pos:
-        if comments_writer is not None:
-            make_relative_comments(
-                shen.shen.group_rets[f"group{group_num}"], zz1000=1
-            ).to_excel(comments_writer, sheet_name="1000超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets[f"group{group_num}"]
-                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
-                    zz1000=1,
-                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], zz1000=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(
-                shen.shen.group_rets[f"group{group_num}"], zz1000=1
-            ).to_excel(net_values_writer, sheet_name="1000超额")
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets[f"group{group_num}"]
-                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
-                    zz1000=1,
-                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments_plot(
-                shen.shen.group_rets[f"group{group_num}"], zz1000=1
-            )
-    else:
-        if comments_writer is not None:
-            make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
-                comments_writer, sheet_name="1000超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz1000=1,
-                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments(shen.shen.group_rets.group1, zz1000=1)
-        if net_values_writer is not None:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
-                net_values_writer, sheet_name="1000超额"
-            )
-            for i in trade_cost_double_side_list:
-                make_relative_comments_plot(
-                    shen.shen.group_rets.group1
-                    - shen.shen.factor_turnover_rates.group1 * i,
-                    zz1000=1,
-                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
-        else:
-            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1)
-
-
 class pure_helper(object):
     def __init__(
         self,
         df_main: pd.DataFrame,
         df_helper: pd.DataFrame,
         func: Callable = None,
         group: int = 10,
@@ -4560,31 +4205,30 @@
         return df
 
 
 class pure_fama(object):
     # @lru_cache(maxsize=None)
     def __init__(
         self,
-        factors: List[pd.DataFrame],
+        factors: list[pd.DataFrame],
         minus_group: Union[list, float] = 3,
         backsee: int = 20,
         rets: pd.DataFrame = None,
         value_weighted: bool = 1,
         add_market: bool = 1,
         add_market_series: pd.Series = None,
         factors_names: list = None,
         betas_rets: bool = 0,
-        total_cap: bool = 0,
     ) -> None:
         """使用fama三因子的方法，将个股的收益率，拆分出各个因子带来的收益率以及特质的收益率
         分别计算每一期，各个因子收益率的值，超额收益率，因子的暴露，以及特质收益率
 
         Parameters
         ----------
-        factors : List[pd.DataFrame]
+        factors : list[pd.DataFrame]
             用于解释收益的各个因子值，每一个都是index为时间，columns为股票代码，values为因子值的dataframe
         minus_group : Union[list, float], optional
             每一个因子将截面上的股票分为几组, by default 3
         backsee : int, optional
             做时序回归时，回看的天数, by default 20
         rets : pd.DataFrame, optional
             每只个股的收益率，index为时间，columns为股票代码，values为收益率，默认使用当日日间收益率, by default None
@@ -4594,16 +4238,14 @@
             是否加入市场收益率因子，默认使用中证全指的每日日间收益率, by default 1
         add_market_series : bool, optional
             加入的市场收益率的数据，如果没指定，则使用中证全指的日间收益率, by default None
         factors_names : list, optional
             各个因子的名字，默认为fac0(市场收益率因子，如果没有，则从fac1开始),fac1,fac2,fac3, by default None
         betas_rets : bool, optional
             是否计算每只个股的由于暴露在每个因子上所带来的收益率, by default 0
-        total_cap : bool, optional
-            加权时使用总市值, by default 0
         """
         start = max(
             [int(datetime.datetime.strftime(i.index.min(), "%Y%m%d")) for i in factors]
         )
         self.backsee = backsee
         self.factors = factors
         self.factors_names = factors_names
@@ -4619,16 +4261,14 @@
         ]
         self.factors_group_long = [(i == 0) + 0 for i in self.factors_group]
         self.factors_group_short = [
             (i == (j - 1)) + 0 for i, j in zip(self.factors_group, self.minus_group)
         ]
         self.value_weighted = value_weighted
         if value_weighted:
-            if total_cap:
-                self.cap = read_daily(total_cap=1, start=start)
             self.cap = read_daily(flow_cap=1, start=start)
             self.factors_group_long = [self.cap * i for i in self.factors_group_long]
             self.factors_group_short = [self.cap * i for i in self.factors_group_short]
             self.factors_group_long = [
                 (i.T / i.T.sum()).T for i in self.factors_group_long
             ]
             self.factors_group_short = [
@@ -4665,15 +4305,18 @@
             else:
                 closes = add_market_series.to_frame("fac0")
             rets = closes / closes.shift(1) - 1
             self.__factors_rets = pd.concat([rets, self.__factors_rets], axis=1)
             if factors_names is not None:
                 factors_names = ["市场"] + factors_names
         self.__data = self.make_df(self.rets, self.__factors_rets)
-        tqdm.auto.tqdm.pandas()
+        if is_notebook():
+            tqdm.tqdm_notebook().pandas()
+        else:
+            tqdm.tqdm.pandas()
         self.__coefficients = (
             self.__data.groupby("code").progress_apply(self.ols_in).reset_index()
         )
         self.__coefficients = self.__coefficients.rename(
             columns={
                 i: "co" + i for i in list(self.__coefficients.columns) if "fac" in i
             }
@@ -4786,29 +4429,29 @@
             ...
 
 
 class pure_rollingols(object):
     def __init__(
         self,
         y: pd.DataFrame,
-        xs: Union[List[pd.DataFrame], pd.DataFrame],
+        xs: Union[list[pd.DataFrame], pd.DataFrame],
         backsee: int = 20,
-        factors_names: List[str] = None,
+        factors_names: list[str] = None,
     ) -> None:
         """使用若干个dataframe，对应的股票进行指定窗口的时序滚动回归
 
         Parameters
         ----------
         y : pd.DataFrame
             滚动回归中的因变量y，index是时间，columns是股票代码
-        xs : Union[List[pd.DataFrame], pd.DataFrame]
+        xs : Union[list[pd.DataFrame], pd.DataFrame]
             滚动回归中的自变量xi，每一个dataframe，index是时间，columns是股票代码
         backsee : int, optional
             滚动回归的时间窗口, by default 20
-        factors_names : List[str], optional
+        factors_names : list[str], optional
             xs中，每个因子的名字, by default None
         """
         self.backsee = backsee
         self.y = y
         if not isinstance(xs, list):
             xs = [xs]
         self.xs = xs
@@ -4822,15 +4465,18 @@
             for j, i in enumerate(xs)
         ]
         xs = [y] + xs
         xs = reduce(lambda x, y: pd.merge(x, y, on=["date", "code"]), xs)
         xs = xs.set_index("date")
         self.__data = xs
         self.haha = xs
-        tqdm.auto.tqdm.pandas()
+        if is_notebook():
+            tqdm.tqdm_notebook().pandas()
+        else:
+            tqdm.tqdm.pandas()
         self.__coefficients = (
             self.__data.groupby("code").progress_apply(self.ols_in).reset_index()
         )
         self.__coefficients = self.__coefficients.rename(
             columns={i: "co" + i for i in list(self.__coefficients.columns) if "x" in i}
         )
         self.__data = pd.merge(
@@ -4851,18 +4497,18 @@
         self.__alphas = self.__data.pivot(
             index="date", columns="code", values="intercept"
         )
         if factors_names is None:
             self.__betas = {
                 i: self.__data.pivot(index="date", columns="code", values=i)
                 for i in list(self.__data.columns)
-                if i.startswith("cox")
+                if i.startswith("x")
             }
         else:
-            facs = [i for i in list(self.__data.columns) if i.startswith("cox")]
+            facs = [i for i in list(self.__data.columns) if i.startswith("x")]
             self.__betas = {
                 factors_names[num]: self.__data.pivot(
                     index="date", columns="code", values=i
                 )
                 for num, i in enumerate(facs)
             }
         if len(list(self.__betas)) == 1:
@@ -4900,77 +4546,51 @@
             return pd.concat([alpha, betas], axis=1)
 
         except Exception:
             # 有些数据总共不足，那就跳过
             ...
 
 
-@do_on_dfs
 def test_on_300500(
     df: pd.DataFrame,
-    trade_cost_double_side: float = 0,
-    group_num: int = 10,
-    value_weighted: bool = 1,
-    boxcox: bool = 0,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     iplot: bool = 1,
-    opens_average_first_day: bool = 0,
-    total_cap: bool = 0,
 ) -> pd.Series:
     """对因子在指数成分股内进行多空和多头测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
-    trade_cost_double_side : float, optional
-        交易的双边手续费率, by default 0
-    group_num : int
-        分组数量, by default 10
-    value_weighted : bool
-        是否进行流通市值加权, by default 0
     hs300 : bool, optional
         在沪深300成分股内测试, by default 0
     zz500 : bool, optional
         在中证500成分股内测试, by default 0
     zz1000 : bool, optional
         在中证1000成分股内测试, by default 0
     gz1000 : bool, optional
         在国证2000成分股内测试, by default 0
-    iplot : bo0l,optional
+    iplot : bol,optional
         多空回测的时候，是否使用cufflinks绘画
-    opens_average_first_day : bool, optional
-        买入时使用第一天的平均价格, by default 0
-    total_cap : bool, optional
-        加权和行业市值中性化时使用总市值, by default 0
 
     Returns
     -------
     pd.Series
         多头组在该指数上的超额收益序列
     """
     fi300 = daily_factor_on300500(
         df, hs300=hs300, zz500=zz500, zz1000=zz1000, gz2000=gz2000
     )
-    shen = pure_moonnight(
-        fi300,
-        value_weighted=value_weighted,
-        groups_num=group_num,
-        trade_cost_double_side=trade_cost_double_side,
-        boxcox=boxcox,
-        iplot=iplot,
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
-    )
+    shen = pure_moonnight(fi300, iplot=iplot)
     if (
         shen.shen.group_net_values.group1.iloc[-1]
-        > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
+        > shen.shen.group_net_values.group10.iloc[-1]
     ):
         print(
             make_relative_comments(
                 shen.shen.group_rets.group1,
                 hs300=hs300,
                 zz500=zz500,
                 zz1000=zz1000,
@@ -4984,177 +4604,96 @@
             zz1000=zz1000,
             gz2000=gz2000,
         )
         return abrets
     else:
         print(
             make_relative_comments(
-                shen.shen.group_rets[f"group{group_num}"],
+                shen.shen.group_rets.group10,
                 hs300=hs300,
                 zz500=zz500,
                 zz1000=zz1000,
                 gz2000=gz2000,
             )
         )
         abrets = make_relative_comments_plot(
-            shen.shen.group_rets[f"group{group_num}"],
+            shen.shen.group_rets.group10,
             hs300=hs300,
             zz500=zz500,
             zz1000=zz1000,
             gz2000=gz2000,
         )
         return abrets
 
 
-@do_on_dfs
 def test_on_index_four(
-    df: pd.DataFrame,
-    value_weighted: bool = 1,
-    group_num: int = 10,
-    trade_cost_double_side: float = 0,
-    iplot: bool = 1,
-    gz2000: bool = 0,
-    boxcox: bool = 1,
-    opens_average_first_day: bool = 0,
-    total_cap: bool = 0,
+    df: pd.DataFrame, iplot: bool = 1, gz2000: bool = 0, boxcox: bool = 1
 ) -> pd.DataFrame:
     """对因子同时在沪深300、中证500、中证1000、国证2000这4个指数成分股内进行多空和多头超额测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
-    value_weighted : bool
-        是否进行流通市值加权, by default 0
-    group_num : int
-        分组数量, by default 10
-    trade_cost_double_side : float, optional
-        交易的双边手续费率, by default 0
     iplot : bol,optional
         多空回测的时候，是否使用cufflinks绘画
     gz2000 : bool, optional
         是否进行国证2000上的测试, by default 0
     boxcox : bool, optional
         是否进行行业市值中性化处理, by default 1
-    opens_average_first_day : bool, optional
-        买入时使用第一天的平均价格, by default 0
-    total_cap : bool, optional
-        加权和行业市值中性化时使用总市值, by default 0
 
     Returns
     -------
     pd.DataFrame
         多头组在各个指数上的超额收益序列
     """
     fi300 = daily_factor_on300500(df, hs300=1)
-    shen = pure_moonnight(
-        fi300,
-        groups_num=group_num,
-        value_weighted=value_weighted,
-        trade_cost_double_side=trade_cost_double_side,
-        iplot=iplot,
-        boxcox=boxcox,
-        opens_average_first_day=opens_average_first_day,
-        total_cap=total_cap,
-    )
+    shen = pure_moonnight(fi300, iplot=iplot, boxcox=boxcox)
     if (
         shen.shen.group_net_values.group1.iloc[-1]
-        > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
+        > shen.shen.group_net_values.group10.iloc[-1]
     ):
         com300, net300 = make_relative_comments(
             shen.shen.group_rets.group1, hs300=1, show_nets=1
         )
         fi500 = daily_factor_on300500(df, zz500=1)
-        shen = pure_moonnight(
-            fi500,
-            groups_num=group_num,
-            value_weighted=value_weighted,
-            trade_cost_double_side=trade_cost_double_side,
-            iplot=iplot,
-            boxcox=boxcox,
-            opens_average_first_day=opens_average_first_day,
-            total_cap=total_cap,
-        )
+        shen = pure_moonnight(fi500, iplot=iplot, boxcox=boxcox)
         com500, net500 = make_relative_comments(
             shen.shen.group_rets.group1, zz500=1, show_nets=1
         )
         fi1000 = daily_factor_on300500(df, zz1000=1)
-        shen = pure_moonnight(
-            fi1000,
-            groups_num=group_num,
-            value_weighted=value_weighted,
-            trade_cost_double_side=trade_cost_double_side,
-            iplot=iplot,
-            boxcox=boxcox,
-            opens_average_first_day=opens_average_first_day,
-            total_cap=total_cap,
-        )
+        shen = pure_moonnight(fi1000, iplot=iplot, boxcox=boxcox)
         com1000, net1000 = make_relative_comments(
             shen.shen.group_rets.group1, zz1000=1, show_nets=1
         )
         if gz2000:
             fi2000 = daily_factor_on300500(df, gz2000=1)
-            shen = pure_moonnight(
-                fi2000,
-                groups_num=group_num,
-                trade_cost_double_side=trade_cost_double_side,
-                iplot=iplot,
-                boxcox=boxcox,
-                opens_average_first_day=opens_average_first_day,
-                total_cap=total_cap,
-            )
+            shen = pure_moonnight(fi2000, iplot=iplot, boxcox=boxcox)
             com2000, net2000 = make_relative_comments(
                 shen.shen.group_rets.group1, gz2000=1, show_nets=1
             )
     else:
         com300, net300 = make_relative_comments(
-            shen.shen.group_rets[f"group{group_num}"], hs300=1, show_nets=1
+            shen.shen.group_rets.group10, hs300=1, show_nets=1
         )
         fi500 = daily_factor_on300500(df, zz500=1)
-        shen = pure_moonnight(
-            fi500,
-            groups_num=group_num,
-            value_weighted=value_weighted,
-            trade_cost_double_side=trade_cost_double_side,
-            iplot=iplot,
-            boxcox=boxcox,
-            opens_average_first_day=opens_average_first_day,
-            total_cap=total_cap,
-        )
+        shen = pure_moonnight(fi500, iplot=iplot, boxcox=boxcox)
         com500, net500 = make_relative_comments(
-            shen.shen.group_rets[f"group{group_num}"], zz500=1, show_nets=1
+            shen.shen.group_rets.group10, zz500=1, show_nets=1
         )
         fi1000 = daily_factor_on300500(df, zz1000=1)
-        shen = pure_moonnight(
-            fi1000,
-            groups_num=group_num,
-            value_weighted=value_weighted,
-            trade_cost_double_side=trade_cost_double_side,
-            iplot=iplot,
-            boxcox=boxcox,
-            opens_average_first_day=opens_average_first_day,
-            total_cap=total_cap,
-        )
+        shen = pure_moonnight(fi1000, iplot=iplot, boxcox=boxcox)
         com1000, net1000 = make_relative_comments(
-            shen.shen.group_rets[f"group{group_num}"], zz1000=1, show_nets=1
+            shen.shen.group_rets.group10, zz1000=1, show_nets=1
         )
         if gz2000:
             fi2000 = daily_factor_on300500(df, gz2000=1)
-            shen = pure_moonnight(
-                fi2000,
-                groups_num=group_num,
-                value_weighted=value_weighted,
-                trade_cost_double_side=trade_cost_double_side,
-                iplot=iplot,
-                boxcox=boxcox,
-                opens_average_first_day=opens_average_first_day,
-                total_cap=total_cap,
-            )
+            shen = pure_moonnight(fi2000, iplot=iplot, boxcox=boxcox)
             com2000, net2000 = make_relative_comments(
-                shen.shen.group_rets[f"group{group_num}"], gz2000=1, show_nets=1
+                shen.shen.group_rets.group10, gz2000=1, show_nets=1
             )
     com300 = com300.to_frame("300超额")
     com500 = com500.to_frame("500超额")
     com1000 = com1000.to_frame("1000超额")
     if gz2000:
         com2000 = com2000.to_frame("2000超额")
         coms = pd.concat([com300, com500, com1000, com2000], axis=1)
@@ -5194,15 +4733,15 @@
                 specs=[
                     [
                         None,
                         {"rowspan": 2, "colspan": 4},
                         None,
                         None,
                         None,
-                        {"rowspan": 2, "colspan": 3},
+                        {"rowspan": 2, "colspan": 5},
                         None,
                         None,
                         None,
                         None,
                     ],
                     [
                         None,
@@ -5228,15 +4767,15 @@
                 shared_yaxes=False,
                 specs=[
                     [
                         None,
                         {"rowspan": 2, "colspan": 3},
                         None,
                         None,
-                        {"rowspan": 2, "colspan": 3},
+                        {"rowspan": 2, "colspan": 6},
                         None,
                         None,
                         None,
                         None,
                         None,
                     ],
                     [
@@ -5262,26 +4801,24 @@
         tb.set_cols_width([8] + [7] + [8] * 2 + [7] * 2 + [8])
         tb.set_cols_dtype(["f"] * 7)
         tb.header(list(coms.T.reset_index().columns))
         tb.add_rows(coms.T.reset_index().to_numpy(), header=True)
         print(tb.draw())
 
 
-@do_on_dfs
 class pure_star(object):
     def __init__(
         self,
         fac: pd.Series,
         code: str = None,
         price_opens: pd.Series = None,
         iplot: bool = 1,
         comments_writer: pd.ExcelWriter = None,
         net_values_writer: pd.ExcelWriter = None,
         sheetname: str = None,
-        questdb_host: str = "127.0.0.1",
     ):
         """择时回测框架，输入仓位比例或信号值，依据信号买入对应的股票或指数，并考察绝对收益、超额收益和基准收益
         回测方式为，t日收盘时获得信号，t+1日开盘时以开盘价买入，t+2开盘时以开盘价卖出
 
         Parameters
         ----------
         fac : pd.Series
@@ -5294,29 +4831,27 @@
             使用cufflinks呈现回测绩效和走势图, by default 1
         comments_writer : pd.ExcelWriter, optional
             绩效评价的存储文件, by default None
         net_values_writer : pd.ExcelWriter, optional
             净值序列的存储文件, by default None
         sheetname : str, optional
             存储文件的工作表的名字, by default None
-        questdb_host: str, optional
-            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
         """
         if code is not None:
             x1 = code.split(".")[0]
             x2 = code.split(".")[1]
             if (x1[0] == "0" or x1[:2] == "30") and x2 == "SZ":
                 kind = "stock"
             elif x1[0] == "6" and x2 == "SH":
                 kind = "stock"
             else:
                 kind = "index"
             self.kind = kind
             if kind == "index":
-                qdb = Questdb(host=questdb_host)
+                qdb = Questdb()
                 price_opens = qdb.get_data(
                     f"select date,num,close from minute_data_{kind} where code='{code}'"
                 )
                 price_opens = price_opens[price_opens.num == "1"]
                 price_opens = price_opens.set_index("date").close
                 price_opens.index = pd.to_datetime(price_opens.index, format="%Y%m%d")
             else:
@@ -5349,20 +4884,20 @@
         self.total_comments.columns = (
             self.total_nets.columns
         ) = self.total_rets.columns = ["因子绝对", "因子超额", "买入持有"]
         self.total_comments = np.around(self.total_comments, 3)
         self.iplot = iplot
         self.plot()
         if comments_writer is None and sheetname is not None:
-            from pure_ocean_breeze.state.states import COMMENTS_WRITER
+            from pure_ocean_breeze.legacy_version.v3p4.state.states import COMMENTS_WRITER
 
             comments_writer = COMMENTS_WRITER
             self.total_comments.to_excel(comments_writer, sheet_name=sheetname)
         if net_values_writer is None and sheetname is not None:
-            from pure_ocean_breeze.state.states import NET_VALUES_WRITER
+            from pure_ocean_breeze.legacy_version.v3p4.state.states import NET_VALUES_WRITER
 
             net_values_writer = NET_VALUES_WRITER
             self.total_nets.to_excel(net_values_writer, sheet_name=sheetname)
 
     def plot(self):
         coms = self.total_comments.copy().reset_index()
         if self.iplot:
@@ -5421,528 +4956,7 @@
             plt.show()
             tb = Texttable()
             tb.set_cols_width([8] + [7] + [8] * 2 + [7] * 2 + [8])
             tb.set_cols_dtype(["f"] * 7)
             tb.header(list(coms.T.reset_index().columns))
             tb.add_rows(coms.T.reset_index().to_numpy(), header=True)
             print(tb.draw())
-
-
-@do_on_dfs
-def get_group(df: pd.DataFrame, group_num: int = 10) -> pd.DataFrame:
-    """使用groupby的方法，将一组因子值改为截面上的分组值，此方法相比qcut的方法更加稳健，但速度更慢一些
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        因子值，index为时间，columns为股票代码，values为因子值
-    group_num : int, optional
-        分组的数量, by default 10
-
-    Returns
-    -------
-    pd.DataFrame
-        转化为分组值后的df，index为时间，columns为股票代码，values为分组值
-    """
-    a = pure_moon(no_read_indu=1)
-    df = df.stack().reset_index()
-    df.columns = ["date", "code", "fac"]
-    df = a.get_groups(df, group_num).pivot(index="date", columns="code", values="group")
-    return df
-
-
-class pure_linprog(object):
-    def __init__(
-        self,
-        facs: pd.DataFrame,
-        total_caps: pd.DataFrame = None,
-        indu_dummys: pd.DataFrame = None,
-        index_weights_hs300: pd.DataFrame = None,
-        index_weights_zz500: pd.DataFrame = None,
-        index_weights_zz1000: pd.DataFrame = None,
-        opens: pd.DataFrame = None,
-        closes: pd.DataFrame = None,
-        hs300_closes: pd.DataFrame = None,
-        zz500_closes: pd.DataFrame = None,
-        zz1000_closes: pd.DataFrame = None,
-    ) -> None:
-        """线性规划求解，目标为预期收益率最大（即因子方向为负时，组合因子值最小）
-        条件为，严格控制市值中性（数据：总市值的对数；含义：组合在市值上的暴露与指数在市值上的暴露相等）
-        严格控制行业中性（数据：使用中信一级行业哑变量），个股偏离在1%以内，成分股权重之和在80%以上
-        分别在沪深300、中证500、中证1000上优化求解
-
-        Parameters
-        ----------
-        facs : pd.DataFrame
-            因子值，index为时间，columns为股票代码，values为因子值
-        total_caps : pd.DataFrame, optional
-            总市值数据，index为时间，columns为股票代码，values为总市值, by default None
-        indu_dummys : pd.DataFrame, optional
-            行业哑变量，包含两列名为date的时间和code的股票代码，以及30+列行业哑变量, by default None
-        index_weights_hs300 : pd.DataFrame, optional
-            沪深300指数成分股权重，月频数据, by default None
-        index_weights_zz500 : pd.DataFrame, optional
-            中证500指数成分股权重，月频数据, by default None
-        index_weights_zz1000 : pd.DataFrame, optional
-            中证1000指数成分股权重，月频数据, by default None
-        opens : pd.DataFrame, optional
-            每月月初开盘价数据, by default None
-        closes : pd.DataFrame, optional
-            每月月末收盘价数据, by default None
-        hs300_closes : pd.DataFrame, optional
-            沪深300每月收盘价数据, by default None
-        zz500_closes : pd.DataFrame, optional
-            中证500每月收盘价数据,, by default None
-        zz1000_closes : pd.DataFrame, optional
-            中证1000每月收盘价数据,, by default None
-        """
-        self.facs = facs.resample("M").last()
-        if total_caps is None:
-            total_caps = standardlize(
-                np.log(read_daily(total_cap=1).resample("M").last())
-            )
-        if indu_dummys is None:
-            indu_dummys = read_daily(zxindustry_dummy_code=1)
-        if index_weights_hs300 is None:
-            index_weights_hs300 = read_daily(hs300_member_weight=1)
-        if index_weights_zz500 is None:
-            index_weights_zz500 = read_daily(zz500_member_weight=1)
-        if index_weights_zz1000 is None:
-            index_weights_zz1000 = read_daily(zz1000_member_weight=1)
-        if opens is None:
-            opens = read_daily(open=1).resample("M").first()
-        if closes is None:
-            closes = read_daily(close=1).resample("M").last()
-        if hs300_closes is None:
-            hs300_closes = read_index_single("000300.SH").resample("M").last()
-        if zz500_closes is None:
-            zz500_closes = read_index_single("000905.SH").resample("M").last()
-        if zz1000_closes is None:
-            zz1000_closes = read_index_single("000852.SH").resample("M").last()
-        self.total_caps = total_caps
-        self.indu_dummys = indu_dummys
-        self.index_weights_hs300 = index_weights_hs300
-        self.index_weights_zz500 = index_weights_zz500
-        self.index_weights_zz1000 = index_weights_zz1000
-        self.hs300_weights = []
-        self.zz500_weights = []
-        self.zz1000_weights = []
-        self.ret_next = closes / opens - 1
-        self.ret_hs300 = hs300_closes.pct_change()
-        self.ret_zz500 = zz500_closes.pct_change()
-        self.ret_zz1000 = zz1000_closes.pct_change()
-
-    def optimize_one_day(
-        self,
-        fac: pd.DataFrame,
-        flow_cap: pd.DataFrame,
-        indu_dummy: pd.DataFrame,
-        index_weight: pd.DataFrame,
-        name: str,
-    ) -> pd.DataFrame:
-        """优化单期求解
-
-        Parameters
-        ----------
-        fac : pd.DataFrame
-            单期因子值，index为code，columns为date，values为因子值
-        flow_cap : pd.DataFrame
-            流通市值，index为code，columns为date，values为截面标准化的流通市值
-        indu_dummy : pd.DataFrame
-            行业哑变量，index为code，columns为行业代码，values为哑变量
-        index_weight : pd.DataFrame
-            指数成分股权重，index为code，columns为date，values为权重
-
-        Returns
-        -------
-        pd.DataFrame
-            当期最佳权重
-        """
-        if fac.shape[0] > 0 and index_weight.shape[1] > 0:
-            date = fac.columns.tolist()[0]
-            codes = list(
-                set(fac.index)
-                | set(flow_cap.index)
-                | set(indu_dummy.index)
-                | set(index_weight.index)
-            )
-            fac, flow_cap, indu_dummy, index_weight = list(
-                map(
-                    lambda x: x.reindex(codes).fillna(0).to_numpy(),
-                    [fac, flow_cap, indu_dummy, index_weight],
-                )
-            )
-            sign_index_weight = np.sign(index_weight)
-            # 个股权重大于零、偏离1%
-            bounds = list(
-                zip(
-                    select_max(index_weight - 0.01, 0).flatten(),
-                    select_min(index_weight + 0.01, 1).flatten(),
-                )
-            )
-            # 市值中性+行业中性+权重和为1
-            huge = np.vstack([flow_cap.T, indu_dummy.T, np.array([1] * len(codes))])
-            target = (
-                list(flow_cap.T @ index_weight.flatten())
-                + list((indu_dummy.T @ index_weight).flatten())
-                + [np.sum(index_weight)]
-            )
-            # 写线性条件
-            c = fac.T.flatten().tolist()
-            a = sign_index_weight.reshape((1, -1)).tolist()
-            b = [0.8]
-            # 优化求解
-            res = linprog(c, a, b, huge, target, bounds)
-            if res.success:
-                return pd.DataFrame({date: res.x.tolist()}, index=codes)
-            else:
-                # raise NotImplementedError(f"{date}这一期的优化失败，请检查")
-                logger.warning(f"{name}在{date}这一期的优化失败，请检查")
-                return None
-        else:
-            return None
-
-    def optimize_many_days(self, startdate: int = 20130101):
-        dates = [i for i in self.facs.index if i >= pd.Timestamp(str(startdate))]
-        for date in tqdm.auto.tqdm(dates):
-            fac = self.facs[self.facs.index == date].T.dropna()
-            total_cap = self.total_caps[self.total_caps.index == date].T.dropna()
-            indu_dummy = self.indu_dummys[self.indu_dummys.date <= date]
-            indu_dummy = (
-                indu_dummy[indu_dummy.date == indu_dummy.date.max()]
-                .drop(columns=["date"])
-                .set_index("code")
-            )
-            index_weight_hs300 = self.index_weights_hs300[
-                self.index_weights_hs300.index == date
-            ].T.dropna()
-            index_weight_zz500 = self.index_weights_zz500[
-                self.index_weights_zz500.index == date
-            ].T.dropna()
-            index_weight_zz1000 = self.index_weights_zz1000[
-                self.index_weights_zz1000.index == date
-            ].T.dropna()
-            weight_hs300 = self.optimize_one_day(
-                fac, total_cap, indu_dummy, index_weight_hs300, "hs300"
-            )
-            weight_zz500 = self.optimize_one_day(
-                fac, total_cap, indu_dummy, index_weight_zz500, "zz500"
-            )
-            weight_zz1000 = self.optimize_one_day(
-                fac, total_cap, indu_dummy, index_weight_zz1000, "zz1000"
-            )
-            self.hs300_weights.append(weight_hs300)
-            self.zz500_weights.append(weight_zz500)
-            self.zz1000_weights.append(weight_zz1000)
-        self.hs300_weights = pd.concat(self.hs300_weights, axis=1).T
-        self.zz500_weights = pd.concat(self.zz500_weights, axis=1).T
-        self.zz1000_weights = pd.concat(self.zz1000_weights, axis=1).T
-
-    def make_contrast(self, weight, index, name) -> list[pd.DataFrame]:
-        ret = (weight.shift(1) * self.ret_next).sum(axis=1)
-        abret = ret - index
-        rets = pd.concat([ret, index, abret], axis=1).dropna()
-        rets.columns = [f"{name}增强组合净值", f"{name}指数净值", f"{name}增强组合超额净值"]
-        rets = (rets + 1).cumprod()
-        rets = rets.apply(lambda x: x / x.iloc[0])
-        comments = comments_on_twins(rets[f"{name}增强组合超额净值"], abret.dropna())
-        return comments, rets
-
-    def run(self, startdate: int = 20130101) -> pd.DataFrame:
-        """运行规划求解
-
-        Parameters
-        ----------
-        startdate : int, optional
-            起始日期, by default 20130101
-
-        Returns
-        -------
-        pd.DataFrame
-            超额绩效指标
-        """
-        self.optimize_many_days(startdate=startdate)
-        self.hs300_comments, self.hs300_nets = self.make_contrast(
-            self.hs300_weights, self.ret_hs300, "沪深300"
-        )
-        self.zz500_comments, self.zz500_nets = self.make_contrast(
-            self.zz500_weights, self.ret_zz500, "中证500"
-        )
-        self.zz1000_comments, self.zz1000_nets = self.make_contrast(
-            self.zz1000_weights, self.ret_zz1000, "中证1000"
-        )
-
-        figs = cf.figures(
-            pd.concat([self.hs300_nets, self.zz500_nets, self.zz1000_nets]),
-            [
-                dict(kind="line", y=list(self.hs300_nets.columns)),
-                dict(kind="line", y=list(self.zz500_nets.columns)),
-                dict(kind="line", y=list(self.zz1000_nets.columns)),
-            ],
-            asList=True,
-        )
-        base_layout = cf.tools.get_base_layout(figs)
-
-        sp = cf.subplots(
-            figs,
-            shape=(1, 3),
-            base_layout=base_layout,
-            vertical_spacing=0.15,
-            horizontal_spacing=0.03,
-            shared_yaxes=False,
-            subplot_titles=["沪深300增强", "中证500增强", "中证1000增强"],
-        )
-        sp["layout"].update(showlegend=True)
-        cf.iplot(sp)
-
-        self.comments = pd.concat(
-            [self.hs300_comments, self.zz500_comments, self.zz1000_comments], axis=1
-        )
-        self.comments.columns = ["沪深300超额", "中证500超额", "中证1000超额"]
-
-        from pure_ocean_breeze.state.states import COMMENTS_WRITER, NET_VALUES_WRITER
-
-        comments_writer = COMMENTS_WRITER
-        net_values_writer = NET_VALUES_WRITER
-        if comments_writer is not None:
-            self.hs300_comments.to_excel(comments_writer, sheet_name="沪深300组合优化超额绩效")
-            self.zz500_comments.to_excel(comments_writer, sheet_name="中证500组合优化超额绩效")
-            self.zz1000_comments.to_excel(comments_writer, sheet_name="中证1000组合优化超额绩效")
-        if net_values_writer is not None:
-            self.hs300_nets.to_excel(net_values_writer, sheet_name="沪深300组合优化净值")
-            self.zz500_nets.to_excel(net_values_writer, sheet_name="中证500组合优化净值")
-            self.zz1000_nets.to_excel(net_values_writer, sheet_name="中证1000组合优化净值")
-
-        return self.comments.T
-
-
-def symmetrically_orthogonalize(dfs: list[pd.DataFrame]) -> list[pd.DataFrame]:
-    """对多个因子做对称正交，每个因子得到正交其他因子后的结果
-
-    Parameters
-    ----------
-    dfs : list[pd.DataFrame]
-        多个要做正交的因子，每个df都是index为时间，columns为股票代码，values为因子值的df
-
-    Returns
-    -------
-    list[pd.DataFrame]
-        对称正交后的各个因子
-    """
-
-    def sing(dfs: list[pd.DataFrame], date: pd.Timestamp):
-        dds = []
-        for num, i in enumerate(dfs):
-            i = i[i.index == date]
-            i.index = [f"fac{num}"]
-            i = i.T
-            dds.append(i)
-        dds = pd.concat(dds, axis=1)
-        cov = dds.cov()
-        d, u = np.linalg.eig(cov)
-        d = np.diag(d ** (-0.5))
-        new_facs = pd.DataFrame(
-            np.dot(dds, np.dot(np.dot(u, d), u.T)), columns=dds.columns, index=dds.index
-        )
-        new_facs = new_facs.stack().reset_index()
-        new_facs.columns = ["code", "fac_number", "fac"]
-        new_facs = new_facs.assign(date=date)
-        dds = []
-        for num, i in enumerate(dfs):
-            i = new_facs[new_facs.fac_number == f"fac{num}"]
-            i = i.pivot(index="date", columns="code", values="fac")
-            dds.append(i)
-        return dds
-
-    dfs = [standardlize(i) for i in dfs]
-    date_first = max([i.index.min() for i in dfs])
-    date_last = min([i.index.max() for i in dfs])
-    dfs = [i[(i.index >= date_first) & (i.index <= date_last)] for i in dfs]
-    fac_num = len(dfs)
-    ddss = [[] for i in range(fac_num)]
-    for date in tqdm.auto.tqdm(dfs[0].index):
-        dds = sing(dfs, date)
-        for num, i in enumerate(dds):
-            ddss[num].append(i)
-    ds = []
-    for i in tqdm.auto.tqdm(ddss):
-        ds.append(pd.concat(i))
-    return ds
-
-
-def icir_weight(
-    facs: list[pd.DataFrame],
-    backsee: int = 6,
-    boxcox: bool = 0,
-    rank_corr: bool = 0,
-    only_ic: bool = 0,
-) -> pd.DataFrame:
-    """使用icir滚动加权的方式，加权合成几个因子
-
-    Parameters
-    ----------
-    facs : list[pd.DataFrame]
-        要合成的若干因子，每个df都是index为时间，columns为股票代码，values为因子值的df
-    backsee : int, optional
-        用来计算icir的过去期数, by default 6
-    boxcox : bool, optional
-        是否对因子进行行业市值中性化, by default 0
-    rank_corr : bool, optional
-        是否计算rankicir, by default 0
-    only_ic : bool, optional
-        是否只计算IC或Rank IC, by default 0
-
-    Returns
-    -------
-    pd.DataFrame
-        合成后的因子
-
-    Raises
-    ------
-    ValueError
-        因子期数少于回看期数时将报错
-    """
-    date_first_max = max([i.index[0] for i in facs])
-    facs = [i[i.index >= date_first_max] for i in facs]
-    date_last_min = min([i.index[-1] for i in facs])
-    facs = [i[i.index <= date_last_min] for i in facs]
-    facs = [i.shift(1) for i in facs]
-    ret = read_daily(
-        close=1, start=datetime.datetime.strftime(date_first_max, "%Y%m%d")
-    )
-    ret = ret / ret.shift(20) - 1
-    if boxcox:
-        facs = [decap_industry(i) for i in facs]
-    facs = [((i.T - i.T.mean()) / i.T.std()).T for i in facs]
-    dates = list(facs[0].index)
-    fis = []
-    for num, date in tqdm.auto.tqdm(list(enumerate(dates))):
-        if num < backsee:
-            ...
-        else:
-            nears = [i.iloc[num - backsee : num, :] for i in facs]
-            targets = [i[i.index == date] for i in facs]
-            if rank_corr:
-                weights = [
-                    show_corr(
-                        i, ret[ret.index.isin(i.index)], plt_plot=0, show_series=1
-                    )
-                    for i in nears
-                ]
-            else:
-                weights = [
-                    show_corr(
-                        i,
-                        ret[ret.index.isin(i.index)],
-                        plt_plot=0,
-                        show_series=1,
-                        method="pearson",
-                    )
-                    for i in nears
-                ]
-            if only_ic:
-                weights = [i.mean() for i in weights]
-            else:
-                weights = [i.mean() / i.std() for i in weights]
-            fi = sum([i * j for i, j in zip(weights, targets)])
-            fis.append(fi)
-    if len(fis) > 0:
-        return pd.concat(fis).shift(-1)
-    else:
-        raise ValueError("输入的因子值长度不太够吧？")
-
-
-def scipy_weight(
-    facs: list[pd.DataFrame],
-    backsee: int = 6,
-    boxcox: bool = 0,
-    rank_corr: bool = 0,
-    only_ic: bool = 0,
-    upper_bound: float = None,
-    lower_bound: float = 0,
-) -> pd.DataFrame:
-    """使用scipy的minimize优化求解的方式，寻找最优的因子合成权重，默认优化条件为最大ICIR
-
-    Parameters
-    ----------
-    facs : list[pd.DataFrame]
-        要合成的因子，每个df都是index为时间，columns为股票代码，values为因子值的df
-    backsee : int, optional
-        用来计算icir的过去期数, by default 6
-    boxcox : bool, optional
-        是否对因子进行行业市值中性化, by default 0
-    rank_corr : bool, optional
-        是否计算rankicir, by default 0
-    only_ic : bool, optional
-        是否只计算IC或Rank IC, by default 0
-    upper_bound : float, optional
-        每个因子的权重上限，如果不指定，则为每个因子平均权重的2倍，即2除以因子数量, by default None
-    lower_bound : float, optional
-        每个因子的权重下限, by default 0
-
-    Returns
-    -------
-    pd.DataFrame
-        合成后的因子
-    """
-    date_first_max = max([i.index[0] for i in facs])
-    facs = [i[i.index >= date_first_max] for i in facs]
-    date_last_min = min([i.index[-1] for i in facs])
-    facs = [i[i.index <= date_last_min] for i in facs]
-    facs = [i.shift(1) for i in facs]
-    ret = read_daily(
-        close=1, start=datetime.datetime.strftime(date_first_max, "%Y%m%d")
-    )
-    ret = ret / ret.shift(20) - 1
-    if boxcox:
-        facs = [decap_industry(i) for i in facs]
-    facs = [((i.T - i.T.mean()) / i.T.std()).T for i in facs]
-    if upper_bound is None:
-        upper_bound = 2 / len(facs)
-    dates = list(facs[0].index)
-    fis = []
-    for num, date in tqdm.auto.tqdm(list(enumerate(dates))):
-        if num <= backsee:
-            ...
-        else:
-            nears = [i.iloc[num - backsee : num, :] for i in facs]
-            targets = [i[i.index == date] for i in facs]
-            if rank_corr:
-                weights = [
-                    show_corr(
-                        i, ret[ret.index.isin(i.index)], plt_plot=0, show_series=1
-                    )
-                    for i in nears
-                ]
-            else:
-                weights = [
-                    show_corr(
-                        i,
-                        ret[ret.index.isin(i.index)],
-                        plt_plot=0,
-                        show_series=1,
-                        method="pearson",
-                    )
-                    for i in nears
-                ]
-            if only_ic:
-                weights = [i.mean() for i in weights]
-            else:
-                weights = [i.mean() / i.std() for i in weights]
-            weights = pd.concat(weights, axis=1)
-
-            def func(x):
-                w = np.array(x).reshape((-1, 1))
-                y = weights @ w
-                return np.mean(y) / np.std(y)
-
-            cons = {"type": "eq", "fun": lambda x: np.sum(x) - 1}
-            res = minimize(
-                func,
-                np.random.rand(weights.shape[1], 1),
-                constraints=cons,
-                bounds=[(lower_bound, upper_bound)] * weights.shape[1],
-            )
-            xs = res.x.tolist()
-            fac = sum([i * j for i, j in zip(xs, targets)])
-            fis.append(fac)
-    return pd.concat(fis).shift(-1)
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/initialize/initialize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import os
 
 
-def initialize():
+def ini():
     user_file = os.path.expanduser("~") + "/"
     # 日频数据路径
     daily_data_file = input("请设置日频数据存放路径(请最终以斜杠结尾，请不要输入反斜杠'',请都替换为'/')：")
     while "/" not in daily_data_file:
         print("请不要输入反斜杠''，请替换为'/'，并以'/'结尾")
         daily_data_file = input("请设置日频数据存放路径(请最终以斜杠结尾，请不要输入反斜杠'',请都替换为'/')：")
     if daily_data_file[-1] != "/":
@@ -35,23 +35,31 @@
     # 最终因子成果路径
     final_factor_file = input("请设置最终因子成果存放路径(请最终以斜杠结尾，请不要输入反斜杠'',请都替换为'/')：")
     while "/" not in final_factor_file:
         print("请不要输入反斜杠''，请替换为'/'，并以'/'结尾")
         final_factor_file = input("请设置最终因子成果存放路径(请最终以斜杠结尾，请不要输入反斜杠'',请都替换为'/')：")
     if final_factor_file[-1] != "/":
         final_factor_file = final_factor_file + "/"
+    # 股票逐笔数据路径
+    tick_by_tick_data=input("请设置股票逐笔数据存放路径(请最终以斜杠结尾，请不要输入反斜杠'',请都替换为'/)：")
+    while "/" not in tick_by_tick_data:
+        print("请不要输入反斜杠''，请替换为'/'，并以'/'结尾")
+        tick_by_tick_data=input("请设置股票逐笔数据存放路径(请最终以斜杠结尾，请不要输入反斜杠'',请都替换为'/)：")
+    if tick_by_tick_data[-1]!='/':
+        tick_by_tick_data=tick_by_tick_data+'/'
     # 数立方token
     api_token = input("请输入您的数立方token：")
     save_dict = {
         "daily_data_file": daily_data_file,
         "factor_data_file": factor_data_file,
         "barra_data_file": barra_data_file,
         "update_data_file": update_data_file,
         "final_factor_file": final_factor_file,
         "api_token": api_token,
+        'tick_by_tick_data': tick_by_tick_data,
     }
     save_dict_file = open(user_file + "paths.settings", "wb")
     pickle.dump(save_dict, save_dict_file)
     save_dict_file.close()
     from loguru import logger
 
     logger.success("恭喜你，回测框架初始化完成，可以开始使用了👏")
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/labor/process.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,103 @@
-__updated__ = "2022-11-05 00:16:56"
+__updated__ = "2023-06-28 16:10:41"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
 import os
-import tqdm
+import tqdm.auto
 import scipy.stats as ss
+from scipy.optimize import linprog
 import statsmodels.formula.api as smf
 import matplotlib as mpl
 
 mpl.rcParams.update(mpl.rcParamsDefault)
 import matplotlib.pyplot as plt
 
-plt.style.use(["science", "no-latex", "notebook"])
 plt.rcParams["axes.unicode_minus"] = False
 
 from functools import reduce, lru_cache, partial
 from dateutil.relativedelta import relativedelta
 from loguru import logger
 import datetime
 from collections.abc import Iterable
 import plotly.express as pe
 import plotly.io as pio
 from plotly.tools import FigureFactory as FF
-import plotly.graph_objects as go
-import plotly.tools as plyoo
 import pyfinance.ols as po
 from texttable import Texttable
 from xpinyin import Pinyin
+import tradetime as tt
 import cufflinks as cf
+import deprecation
+from mpire import WorkerPool
+from scipy.optimize import minimize
+from pure_ocean_breeze import __version__
 
 cf.set_config_file(offline=True)
-from typing import Callable, Union
-from pure_ocean_breeze.legacy_version.v3p4.data.read_data import (
+from typing import Callable, Union, Dict, List, Tuple
+from pure_ocean_breeze.data.read_data import (
     read_daily,
     read_market,
     get_industry_dummies,
     read_swindustry_prices,
     read_zxindustry_prices,
     database_read_final_factors,
+    read_index_single,
 )
-from pure_ocean_breeze.legacy_version.v3p4.state.homeplace import HomePlace
+from pure_ocean_breeze.state.homeplace import HomePlace
 
-homeplace = HomePlace()
-from pure_ocean_breeze.legacy_version.v3p4.state.states import STATES, is_notebook
-from pure_ocean_breeze.legacy_version.v3p4.data.database import *
-from pure_ocean_breeze.legacy_version.v3p4.data.dicts import INDUS_DICT
-from pure_ocean_breeze.legacy_version.v3p4.data.tools import (
+try:
+    homeplace = HomePlace()
+except Exception:
+    print("您暂未初始化，功能将受限")
+from pure_ocean_breeze.state.states import STATES
+from pure_ocean_breeze.state.decorators import do_on_dfs
+from pure_ocean_breeze.data.database import *
+from pure_ocean_breeze.data.dicts import INDUS_DICT
+from pure_ocean_breeze.data.tools import (
     indus_name,
     drop_duplicates_index,
     to_percent,
     to_group,
+    standardlize,
+    select_max,
+    select_min,
+    merge_many,
 )
-from pure_ocean_breeze.legacy_version.v3p4.labor.comment import (
+from pure_ocean_breeze.labor.comment import (
     comments_on_twins,
     make_relative_comments,
     make_relative_comments_plot,
 )
 
 
+@do_on_dfs
 def daily_factor_on300500(
     fac: pd.DataFrame,
     hs300: bool = 0,
     zz500: bool = 0,
-    zz800: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     other: bool = 0,
 ) -> pd.DataFrame:
     """输入日频或月频因子值，将其限定在某指数成分股的股票池内，
-    目前仅支持沪深300、中证500、中证800、中证1000、国证2000成分股，和除沪深300、中证500、中证1000以外的股票的成分股
+    目前仅支持沪深300、中证500、中证1000、国证2000成分股，以及这四种指数成分股的组合叠加，和除沪深300、中证500、中证1000以外的股票的成分股
 
     Parameters
     ----------
     fac : pd.DataFrame
         未限定股票池的因子值，index为时间，columns为股票代码
     hs300 : bool, optional
         限定股票池为沪深300, by default 0
     zz500 : bool, optional
         限定股票池为中证500, by default 0
-    zz800 : bool, optional
-        限定股票池为中证800, by default 0
     zz1000 : bool, optional
         限定股票池为中证1000, by default 0
     gz2000 : bool, optional
         限定股票池为国证2000, by default 0
     other : bool, optional
         限定股票池为除沪深300、中证500、中证1000以外的股票的成分股, by default 0
 
@@ -99,142 +109,105 @@
     Raises
     ------
     `ValueError`
         如果未指定任何一种指数的成分股，将报错
     """
     last = fac.resample("M").last()
     homeplace = HomePlace()
+    dummies = []
     if fac.shape[0] / last.shape[0] > 2:
         if hs300:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "沪深300日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
-            df = df * fac
-            df = df.dropna(how="all")
-        elif zz500:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "中证500日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
-            df = df * fac
-            df = df.dropna(how="all")
-        elif zz800:
-            df1 = pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
-            df1 = df1.set_index(list(df1.columns)[0])
-            df2 = pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
-            df2 = df2.set_index(list(df2.columns)[0])
-            df = df1 + df2
-            df = df.replace(0, np.nan)
-            df = df * fac
-            df = df.dropna(how="all")
-        elif zz1000:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "中证1000日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
-            df = df * fac
-            df = df.dropna(how="all")
-        elif gz2000:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "国证2000日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
-            df = df * fac
-            df = df.dropna(how="all")
-        elif other:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "沪深300日成分股.parquet"
+            ).fillna(0)
+            dummies.append(df)
+        if zz500:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "中证500日成分股.parquet"
+            ).fillna(0)
+            dummies.append(df)
+        if zz1000:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "中证1000日成分股.parquet"
+            ).fillna(0)
+            dummies.append(df)
+        if gz2000:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "国证2000日成分股.parquet"
+            ).fillna(0)
+            dummies.append(df)
+        if other:
             tr = read_daily(tr=1).fillna(0).replace(0, 1)
             tr = np.sign(tr)
             df1 = (
-                tr * pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
+                tr * pd.read_parquet(homeplace.daily_data_file + "沪深300日成分股.parquet")
             ).fillna(0)
-            df1 = df1.set_index(list(df1.columns)[0])
             df2 = (
-                tr * pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
+                tr * pd.read_parquet(homeplace.daily_data_file + "中证500日成分股.parquet")
             ).fillna(0)
-            df2 = df2.set_index(list(df2.columns)[0])
             df3 = (
-                tr * pd.read_feather(homeplace.daily_data_file + "中证1000日成分股.feather")
+                tr * pd.read_parquet(homeplace.daily_data_file + "中证1000日成分股.parquet")
             ).fillna(0)
-            df3 = df3.set_index(list(df3.columns)[0])
             df = (1 - df1) * (1 - df2) * (1 - df3) * tr
             df = df.replace(0, np.nan) * fac
             df = df.dropna(how="all")
-        else:
+        if (hs300 + zz500 + zz1000 + gz2000 + other) == 0:
             raise ValueError("总得指定一下是哪个成分股吧🤒")
     else:
         if hs300:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "沪深300日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "沪深300日成分股.parquet"
+            ).fillna(0)
             df = df.resample("M").last()
-            df = df * fac
-            df = df.dropna(how="all")
-        elif zz500:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "中证500日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
+            dummies.append(df)
+        if zz500:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "中证500日成分股.parquet"
+            ).fillna(0)
             df = df.resample("M").last()
-            df = df * fac
-            df = df.dropna(how="all")
-        elif zz800:
-            df1 = pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
-            df1 = df1.set_index(list(df1.columns)[0])
-            df1 = df1.resample("M").last()
-            df2 = pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
-            df2 = df2.set_index(list(df2.columns)[0])
-            df2 = df2.resample("M").last()
-            df = df1 + df2
-            df = df.replace(0, np.nan)
-            df = df * fac
-            df = df.dropna(how="all")
-        elif zz1000:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "中证1000日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
+            dummies.append(df)
+        if zz1000:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "中证1000日成分股.parquet"
+            ).fillna(0)
             df = df.resample("M").last()
-            df = df * fac
-            df = df.dropna(how="all")
-        elif gz2000:
-            df = pd.read_feather(
-                homeplace.daily_data_file + "国证2000日成分股.feather"
-            ).replace(0, np.nan)
-            df = df.set_index(list(df.columns)[0])
+            dummies.append(df)
+        if gz2000:
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "国证2000日成分股.parquet"
+            ).fillna(0)
             df = df.resample("M").last()
-            df = df * fac
-            df = df.dropna(how="all")
-        elif other:
+            dummies.append(df)
+        if other:
             tr = read_daily(tr=1).fillna(0).replace(0, 1).resample("M").last()
             tr = np.sign(tr)
             df1 = (
-                tr * pd.read_feather(homeplace.daily_data_file + "沪深300日成分股.feather")
+                tr * pd.read_parquet(homeplace.daily_data_file + "沪深300日成分股.parquet")
             ).fillna(0)
-            df1 = df1.set_index(list(df1.columns)[0])
             df1 = df1.resample("M").last()
             df2 = (
-                tr * pd.read_feather(homeplace.daily_data_file + "中证500日成分股.feather")
+                tr * pd.read_parquet(homeplace.daily_data_file + "中证500日成分股.parquet")
             ).fillna(0)
-            df2 = df2.set_index(list(df2.columns)[0])
             df2 = df2.resample("M").last()
             df3 = (
-                tr * pd.read_feather(homeplace.daily_data_file + "中证1000日成分股.feather")
+                tr * pd.read_parquet(homeplace.daily_data_file + "中证1000日成分股.parquet")
             ).fillna(0)
-            df3 = df3.set_index(list(df3.columns)[0])
             df3 = df3.resample("M").last()
             df = (1 - df1) * (1 - df2) * (1 - df3)
             df = df.replace(0, np.nan) * fac
             df = df.dropna(how="all")
-        else:
+        if (hs300 + zz500 + zz1000 + gz2000 + other) == 0:
             raise ValueError("总得指定一下是哪个成分股吧🤒")
+    if len(dummies) > 0:
+        dummies = sum(dummies).replace(0, np.nan)
+        df = (dummies * fac).dropna(how="all")
     return df
 
 
+@do_on_dfs
 def daily_factor_on_industry(
     df: pd.DataFrame, swindustry: bool = 0, zxindustry: bool = 0
 ) -> dict:
     """将一个因子变为仅在某个申万一级行业上的股票
 
     Parameters
     ----------
@@ -265,29 +238,33 @@
         swindustry=swindustry,
         zxindustry=zxindustry,
     )
     ress = {k: v * df for k, v in ress.items()}
     return ress
 
 
+@do_on_dfs
 def group_test_on_industry(
     df: pd.DataFrame,
     group_num: int = 10,
+    trade_cost_double_side: float = 0,
     net_values_writer: pd.ExcelWriter = None,
     swindustry: bool = 0,
     zxindustry: bool = 0,
 ) -> pd.DataFrame:
     """在申万一级行业上测试每个行业的分组回测
 
     Parameters
     ----------
     df : pd.DataFrame
         全市场的因子值，index是时间，columns是股票代码
     group_num : int, optional
         分组数量, by default 10
+    trade_cost_double_side : float, optional
+        交易的双边手续费率, by default 0
     net_values_writer : pd.ExcelWriter, optional
         用于存储各个行业分组及多空对冲净值序列的excel文件, by default None
     swindustry : bool, optional
         选择使用申万一级行业, by default 0
     zxindustry : bool, optional
         选择使用中信一级行业, by default 0
 
@@ -301,38 +278,41 @@
     ks = []
     vs = []
     if swindustry:
         for k, v in dfs.items():
             shen = pure_moonnight(
                 v,
                 groups_num=group_num,
+                trade_cost_double_side=trade_cost_double_side,
                 net_values_writer=net_values_writer,
                 sheetname=INDUS_DICT[k],
                 plt_plot=0,
             )
             ks.append(k)
             vs.append(shen.shen.total_comments.T)
         vs = pd.concat(vs)
         vs.index = [INDUS_DICT[i] for i in ks]
     else:
         for k, v in dfs.items():
             shen = pure_moonnight(
                 v,
                 groups_num=group_num,
+                trade_cost_double_side=trade_cost_double_side,
                 net_values_writer=net_values_writer,
                 sheetname=k,
                 plt_plot=0,
             )
             ks.append(k)
             vs.append(shen.shen.total_comments.T)
         vs = pd.concat(vs)
         vs.index = ks
     return vs
 
 
+@do_on_dfs
 def rankic_test_on_industry(
     df: pd.DataFrame,
     excel_name: str = "行业rankic.xlsx",
     png_name: str = "行业rankic图.png",
     swindustry: bool = 0,
     zxindustry: bool = 0,
 ) -> pd.DataFrame:
@@ -354,30 +334,32 @@
     Returns
     -------
     pd.DataFrame
         行业名称与对应的Rank IC
     """
     vs = group_test_on_industry(df, swindustry=swindustry, zxindustry=zxindustry)
     rankics = vs[["RankIC"]].T
-    rankics.to_excel(excel_name)
+    if excel_name is not None:
+        rankics.to_excel(excel_name)
     rankics.plot(kind="bar")
     plt.show()
     plt.savefig(png_name)
     return rankics
 
 
+@do_on_dfs
 def long_test_on_industry(
     df: pd.DataFrame,
     nums: list,
     pos: bool = 0,
     neg: bool = 0,
     save_stock_list: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
-) -> list[dict]:
+) -> List[dict]:
     """对每个申万/中信一级行业成分股，使用某因子挑选出最多头的n值股票，考察其超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Parameters
     ----------
     df : pd.DataFrame
         使用的因子，index为时间，columns为股票代码
     nums : list
@@ -390,32 +372,32 @@
         是否保存每月每个行业的多头名单，会降低运行速度, by default 0
     swindustry : bool, optional
         在申万一级行业上测试, by default 0
     zxindusrty : bool, optional
         在中信一级行业上测试, by default 0
     Returns
     -------
-    list[dict]
+    List[dict]
         超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Raises
     ------
     IOError
         pos和neg必须有一个为1，否则将报错
     """
     fac = decap_industry(df, monthly=True)
 
     if swindustry:
-        industry_dummy = pd.read_feather(
-            homeplace.daily_data_file + "申万行业2021版哑变量.feather"
+        industry_dummy = pd.read_parquet(
+            homeplace.daily_data_file + "申万行业2021版哑变量.parquet"
         ).fillna(0)
         indus = read_swindustry_prices()
     else:
-        industry_dummy = pd.read_feather(
-            homeplace.daily_data_file + "中信一级行业哑变量名称版.feather"
+        industry_dummy = pd.read_parquet(
+            homeplace.daily_data_file + "中信一级行业哑变量名称版.parquet"
         ).fillna(0)
         indus = read_zxindustry_prices()
     inds = list(industry_dummy.columns)
     ret_next = (
         read_daily(close=1).resample("M").last()
         / read_daily(open=1).resample("M").first()
         - 1
@@ -450,24 +432,18 @@
         fi = fi.T.apply(sing).T
         fi = fi.replace(0, np.nan)
         fi = fi * ret_next
         ret_long = fi.mean(axis=1)
         return ret_long
 
     ret_longs = {k: [] for k in nums}
-    if is_notebook():
-        for num in tqdm.tqdm_notebook(nums):
-            for code in inds[2:]:
-                df = save_ind(code, num).to_frame(code)
-                ret_longs[num] = ret_longs[num] + [df]
-    else:
-        for num in tqdm.tqdm(nums):
-            for code in inds[2:]:
-                df = save_ind(code, num).to_frame(code)
-                ret_longs[num] = ret_longs[num] + [df]
+    for num in tqdm.auto.tqdm(nums):
+        for code in inds[2:]:
+            df = save_ind(code, num).to_frame(code)
+            ret_longs[num] = ret_longs[num] + [df]
 
     indus = indus.resample("M").last().pct_change()
 
     if swindustry:
         coms = {
             k: indus_name(pd.concat(v, axis=1).dropna(how="all").T).T
             for k, v in ret_longs.items()
@@ -548,22 +524,18 @@
                     raise IOError("您需要指定一下因子方向🤒")
                 return tuple(thr.index)
 
             fi = fi.T.apply(sing)
             return fi
 
         stocks_longs = {k: {} for k in nums}
-        if is_notebook():
-            for num in tqdm.tqdm_notebook(nums):
-                for code in inds[2:]:
-                    stocks_longs[num][code] = save_ind_stocks(code, num)
-        else:
-            for num in tqdm.tqdm(nums):
-                for code in inds[2:]:
-                    stocks_longs[num][code] = save_ind_stocks(code, num)
+
+        for num in tqdm.auto.tqdm(nums):
+            for code in inds[2:]:
+                stocks_longs[num][code] = save_ind_stocks(code, num)
 
         for num in nums:
             w1 = pd.ExcelWriter(f"各个{name}一级行业买{num}只的股票名单.xlsx")
             for k, v in stocks_longs[num].items():
                 v = v.T
                 v.index = v.index.strftime("%Y/%m/%d")
                 v.to_excel(w1, sheet_name=INDUS_DICT[k])
@@ -571,21 +543,22 @@
             w1.close()
 
         return [coms_finals, rets_save, stocks_longs]
     else:
         return [coms_finals, rets_save]
 
 
+@do_on_dfs
 def long_test_on_swindustry(
     df: pd.DataFrame,
     nums: list,
     pos: bool = 0,
     neg: bool = 0,
     save_stock_list: bool = 0,
-) -> list[dict]:
+) -> List[dict]:
     """对每个申万一级行业成分股，使用某因子挑选出最多头的n值股票，考察其超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Parameters
     ----------
     df : pd.DataFrame
         使用的因子，index为时间，columns为股票代码
     nums : list
@@ -594,15 +567,15 @@
         因子方向为正，即Rank IC为正，则指定此处为True, by default 0
     neg : bool, optional
         因子方向为负，即Rank IC为负，则指定此处为False, by default 0
     save_stock_list : bool, optional
         是否保存每月每个行业的多头名单，会降低运行速度, by default 0
     Returns
     -------
-    list[dict]
+    List[dict]
         超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Raises
     ------
     IOError
         pos和neg必须有一个为1，否则将报错
     """
@@ -613,21 +586,22 @@
         neg=neg,
         save_stock_list=save_stock_list,
         swindustry=1,
     )
     return res
 
 
+@do_on_dfs
 def long_test_on_zxindustry(
     df: pd.DataFrame,
     nums: list,
     pos: bool = 0,
     neg: bool = 0,
     save_stock_list: bool = 0,
-) -> list[dict]:
+) -> List[dict]:
     """对每个中信一级行业成分股，使用某因子挑选出最多头的n值股票，考察其超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Parameters
     ----------
     df : pd.DataFrame
         使用的因子，index为时间，columns为股票代码
     nums : list
@@ -636,15 +610,15 @@
         因子方向为正，即Rank IC为正，则指定此处为True, by default 0
     neg : bool, optional
         因子方向为负，即Rank IC为负，则指定此处为False, by default 0
     save_stock_list : bool, optional
         是否保存每月每个行业的多头名单，会降低运行速度, by default 0
     Returns
     -------
-    list[dict]
+    List[dict]
         超额收益绩效、每月超额收益、每月每个行业的多头名单
 
     Raises
     ------
     IOError
         pos和neg必须有一个为1，否则将报错
     """
@@ -655,14 +629,15 @@
         neg=neg,
         save_stock_list=save_stock_list,
         zxindustry=1,
     )
     return res
 
 
+@do_on_dfs
 @kk.desktop_sender(title="嘿，行业中性化做完啦～🛁")
 def decap(df: pd.DataFrame, daily: bool = 0, monthly: bool = 0) -> pd.DataFrame:
     """对因子做市值中性化
 
     Parameters
     ----------
     df : pd.DataFrame
@@ -678,18 +653,15 @@
         市值中性化之后的因子
 
     Raises
     ------
     `NotImplementedError`
         如果未指定日频或月频，将报错
     """
-    if is_notebook():
-        tqdm.tqdm_notebook().pandas()
-    else:
-        tqdm.tqdm.pandas()
+    tqdm.auto.tqdm.pandas()
     share = read_daily(sharenum=1)
     undi_close = read_daily(close=1, unadjust=1)
     cap = (share * undi_close).stack().reset_index()
     cap.columns = ["date", "code", "cap"]
     cap.cap = ss.boxcox(cap.cap)[0]
 
     def single(x):
@@ -710,14 +682,15 @@
     elif monthly:
         df = (pure_fallmount(df) - (pure_fallmount(cap_monthly),))()
     else:
         raise NotImplementedError("必须指定频率")
     return df
 
 
+@do_on_dfs
 @kk.desktop_sender(title="嘿，行业市值中性化做完啦～🛁")
 def decap_industry(
     df: pd.DataFrame,
     daily: bool = 0,
     monthly: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
@@ -786,51 +759,49 @@
         df.fac = df.fac - ols_w * df.cap - ols_b
         for k, v in ols_bs.items():
             df.fac = df.fac - v * df[k]
         df = df[["fac"]]
         return df
 
     if swindustry:
-        file_name = "申万行业2021版哑变量.feather"
+        file_name = "申万行业2021版哑变量.parquet"
     else:
-        file_name = "中信一级行业哑变量代码版.feather"
+        file_name = "中信一级行业哑变量代码版.parquet"
 
     if monthly:
         industry_dummy = (
-            pd.read_feather(homeplace.daily_data_file + file_name)
+            pd.read_parquet(homeplace.daily_data_file + file_name)
             .fillna(0)
             .set_index("date")
             .groupby("code")
             .resample("M")
             .last()
         )
         industry_dummy = industry_dummy.fillna(0).drop(columns=["code"]).reset_index()
         industry_ws = [f"w{i}" for i in range(1, industry_dummy.shape[1] - 1)]
         col = ["code", "date"] + industry_ws
     elif daily:
-        industry_dummy = pd.read_feather(homeplace.daily_data_file + file_name).fillna(
+        industry_dummy = pd.read_parquet(homeplace.daily_data_file + file_name).fillna(
             0
         )
         industry_ws = [f"w{i}" for i in range(1, industry_dummy.shape[1] - 1)]
         col = ["date", "code"] + industry_ws
     else:
         raise NotImplementedError("必须指定频率")
     industry_dummy.columns = col
     df = pd.merge(df, industry_dummy, on=["date", "code"])
     df = df.set_index(["date", "code"])
-    if is_notebook():
-        tqdm.tqdm_notebook().pandas()
-    else:
-        tqdm.tqdm.pandas()
+    tqdm.auto.tqdm.pandas()
     df = df.groupby(["date"]).progress_apply(neutralize_factors)
     df = df.unstack()
     df.columns = [i[1] for i in list(df.columns)]
     return df
 
 
+@do_on_dfs
 def deboth(df: pd.DataFrame) -> pd.DataFrame:
     """通过回测的方式，对月频因子做行业市值中性化
 
     Parameters
     ----------
     df : pd.DataFrame
         未中性化的因子
@@ -840,17 +811,33 @@
     `pd.DataFrame`
         行业市值中性化之后的因子
     """
     shen = pure_moonnight(df, boxcox=1, plt_plot=0, print_comments=0)
     return shen()
 
 
+@do_on_dfs
+def boom_one(
+    df: pd.DataFrame, backsee: int = 20, daily: bool = 0, min_periods: int = None
+) -> pd.DataFrame:
+    if min_periods is None:
+        min_periods = int(backsee * 0.5)
+    if not daily:
+        df_mean = (
+            df.rolling(backsee, min_periods=min_periods).mean().resample("M").last()
+        )
+    else:
+        df_mean = df.rolling(backsee, min_periods=min_periods).mean()
+    return df_mean
+
+
+@do_on_dfs
 def boom_four(
     df: pd.DataFrame, backsee: int = 20, daily: bool = 0, min_periods: int = None
-) -> tuple[pd.DataFrame]:
+) -> Tuple[pd.DataFrame]:
     """生成20天均值，20天标准差，及二者正向z-score合成，正向排序合成，负向z-score合成，负向排序合成这6个因子
 
     Parameters
     ----------
     df : pd.DataFrame
         原日频因子
     backsee : int, optional
@@ -858,15 +845,15 @@
     daily : bool, optional
         为1是每天都滚动，为0则仅保留月底值, by default 0
     min_periods : int, optional
         rolling时的最小期, by default backsee的一半
 
     Returns
     -------
-    `tuple[pd.DataFrame]`
+    `Tuple[pd.DataFrame]`
         6个因子的元组
     """
     if min_periods is None:
         min_periods = int(backsee * 0.5)
     if not daily:
         df_mean = (
             df.rolling(backsee, min_periods=min_periods).mean().resample("M").last()
@@ -882,14 +869,42 @@
         twins_add = (pure_fallmount(df_mean) + (pure_fallmount(df_std),))()
         rtwins_add = df_mean.rank(axis=1) + df_std.rank(axis=1)
         twins_minus = (pure_fallmount(df_mean) + (pure_fallmount(-df_std),))()
         rtwins_minus = df_mean.rank(axis=1) - df_std.rank(axis=1)
     return df_mean, df_std, twins_add, rtwins_add, twins_minus, rtwins_minus
 
 
+def boom_fours(
+    dfs: List[pd.DataFrame],
+    backsee: Union[int, List[int]] = 20,
+    daily: Union[bool, List[bool]] = 0,
+    min_periods: Union[int, List[int]] = None,
+) -> List[List[pd.DataFrame]]:
+    """对多个因子，每个因子都进行boom_four的操作
+
+    Parameters
+    ----------
+    dfs : List[pd.DataFrame]
+        多个因子的dataframe组成的list
+    backsee : Union[int,List[int]], optional
+        每个因子回看期数, by default 20
+    daily : Union[bool,List[bool]], optional
+        每个因子是否逐日计算, by default 0
+    min_periods : Union[int,List[int]], optional
+        每个因子计算的最小期, by default None
+
+    Returns
+    -------
+    List[List[pd.DataFrame]]
+        每个因子进行boom_four后的结果
+    """
+    return boom_four(df=dfs, backsee=backsee, daily=daily, min_periods=min_periods)
+
+
+@do_on_dfs
 def add_cross_standardlize(*args: list) -> pd.DataFrame:
     """将众多因子横截面做z-score标准化之后相加
 
     Returns
     -------
     `pd.DataFrame`
         合成后的因子
@@ -897,37 +912,42 @@
     fms = [pure_fallmount(i) for i in args]
     one = fms[0]
     others = fms[1:]
     final = one + others
     return final()
 
 
+@do_on_dfs
 def to_tradeends(df: pd.DataFrame) -> pd.DataFrame:
     """将最后一个自然日改变为最后一个交易日
 
     Parameters
     ----------
     df : pd.DataFrame
         index为时间，为每个月的最后一天
 
     Returns
     -------
     `pd.DataFrame`
         修改为交易日标注后的pd.DataFrame
     """
     """"""
-    trs = read_daily(tr=1)
+    start = df.index.min()
+    start = start - pd.tseries.offsets.MonthBegin()
+    start = datetime.datetime.strftime(start, "%Y%m%d")
+    trs = read_daily(tr=1, start=start)
     trs = trs.assign(tradeends=list(trs.index))
     trs = trs[["tradeends"]]
     trs = trs.resample("M").last()
     df = pd.concat([trs, df], axis=1)
     df = df.set_index(["tradeends"])
     return df
 
 
+@do_on_dfs
 def market_kind(
     df: pd.DataFrame,
     zhuban: bool = 0,
     chuangye: bool = 0,
     kechuang: bool = 0,
     beijing: bool = 0,
 ) -> pd.DataFrame:
@@ -1001,38 +1021,41 @@
         返回相关性的序列，而非均值
 
     Returns
     -------
     `float`
         平均截面相关系数
     """
-    corr = show_x_with_func(fac1, fac2, lambda x: x.corr(method=method).iloc[0, 1])
+    if method == "spearman":
+        corr = show_x_with_func(fac1, fac2, lambda x: x.rank().corr().iloc[0, 1])
+    else:
+        corr = show_x_with_func(fac1, fac2, lambda x: x.corr(method=method).iloc[0, 1])
     if show_series:
         return corr
     else:
         if plt_plot:
             corr.plot(rot=60)
             plt.show()
         return corr.mean()
 
 
 def show_corrs(
-    factors: list[pd.DataFrame],
-    factor_names: list[str] = None,
+    factors: List[pd.DataFrame],
+    factor_names: List[str] = None,
     print_bool: bool = True,
     show_percent: bool = True,
     method: str = "spearman",
 ) -> pd.DataFrame:
     """展示很多因子两两之间的截面相关性
 
     Parameters
     ----------
-    factors : list[pd.DataFrame]
+    factors : List[pd.DataFrame]
         所有因子构成的列表, by default None
-    factor_names : list[str], optional
+    factor_names : List[str], optional
         上述因子依次的名字, by default None
     print_bool : bool, optional
         是否打印出两两之间相关系数的表格, by default True
     show_percent : bool, optional
         是否以百分数的形式展示, by default True
     method : str, optional
         计算相关系数的方法, by default "spearman"
@@ -1054,16 +1077,17 @@
     corrs = pd.DataFrame(corrs, columns=factor_names, index=factor_names)
     np.fill_diagonal(corrs.to_numpy(), 1)
     if show_percent:
         pcorrs = corrs.applymap(to_percent)
     else:
         pcorrs = corrs.copy()
     if print_bool:
-        print(pcorrs)
-    return corrs
+        return pcorrs
+    else:
+        return corrs
 
 
 def show_cov(
     fac1: pd.DataFrame,
     fac2: pd.DataFrame,
     plt_plot: bool = 1,
     show_series: bool = 0,
@@ -1126,34 +1150,31 @@
     befo1.columns = ["date", "code", "befo"]
     twins = pd.merge(both1, befo1, on=["date", "code"]).set_index(["date", "code"])
     corr = twins.groupby("date").apply(the_func)
     return corr
 
 
 def show_covs(
-    factors: list[pd.DataFrame],
-    factor_names: list[str] = None,
+    factors: List[pd.DataFrame],
+    factor_names: List[str] = None,
     print_bool: bool = True,
     show_percent: bool = True,
-    method: str = "spearman",
 ) -> pd.DataFrame:
     """展示很多因子两两之间的截面相关性
 
     Parameters
     ----------
-    factors : list[pd.DataFrame]
+    factors : List[pd.DataFrame]
         所有因子构成的列表, by default None
-    factor_names : list[str], optional
+    factor_names : List[str], optional
         上述因子依次的名字, by default None
     print_bool : bool, optional
         是否打印出两两之间相关系数的表格, by default True
     show_percent : bool, optional
         是否以百分数的形式展示, by default True
-    method : str, optional
-        计算相关系数的方法, by default "spearman"
 
     Returns
     -------
     `pd.DataFrame`
         两两之间相关系数的表格
     """
     corrs = []
@@ -1173,82 +1194,166 @@
         pcorrs = corrs.copy()
     if print_bool:
         print(pcorrs)
     return corrs
 
 
 def de_cross(
-    y: pd.DataFrame, xs: Union[list[pd.DataFrame], pd.DataFrame]
+    y: pd.DataFrame, xs: Union[List[pd.DataFrame], pd.DataFrame]
 ) -> pd.DataFrame:
     """使用若干因子对某个因子进行正交化处理
 
     Parameters
     ----------
     y : pd.DataFrame
         研究的目标，回归中的y
-    xs : Union[list[pd.DataFrame],pd.DataFrame]
+    xs : Union[List[pd.DataFrame],pd.DataFrame]
         用于正交化的若干因子，回归中的x
 
     Returns
     -------
     pd.DataFrame
         正交化之后的因子
     """
     if not isinstance(xs, list):
         xs = [xs]
     y = pure_fallmount(y)
     xs = [pure_fallmount(i) for i in xs]
     return (y - xs)()
 
 
+@do_on_dfs
 def show_corrs_with_old(
-    df: pd.DataFrame = None, method: str = "spearman"
+    df: pd.DataFrame = None, method: str = "spearman", only_new: bool = 1
 ) -> pd.DataFrame:
     """计算新因子和已有因子的相关系数
 
     Parameters
     ----------
     df : pd.DataFrame, optional
         新因子, by default None
     method : str, optional
         求相关系数的方法, by default 'spearman'
+    only_new : bool, optional
+        仅计算新因子与旧因子之间的相关系数, by default 1
 
     Returns
     -------
     pd.DataFrame
         相关系数矩阵
     """
     if df is not None:
         df0 = df.resample("M").last()
         if df.shape[0] / df0.shape[0] > 2:
             daily = 1
         else:
             daily = 0
+    nums = os.listdir(homeplace.final_factor_file)
+    nums = sorted(
+        set(
+            [
+                int(i.split("多因子")[1].split("_月")[0])
+                for i in nums
+                if i.endswith("月.parquet")
+            ]
+        )
+    )
     olds = []
-    for i in range(1, 100):
+    for i in nums:
         try:
             if daily:
                 old = database_read_final_factors(order=i)[0]
             else:
                 old = database_read_final_factors(order=i)[0].resample("M").last()
             olds.append(old)
         except Exception:
             break
     if df is not None:
-        olds = [df] + olds
-        corrs = show_corrs(
-            olds, ["new"] + [f"old{i}" for i in range(1, len(olds))], method=method
-        )
+        if only_new:
+            corrs = [
+                to_percent(show_corr(df, i, plt_plot=0, method=method)) for i in olds
+            ]
+            corrs = pd.Series(corrs, index=[f"old{i}" for i in nums])
+            corrs = corrs.to_frame(f"{method}相关系数").T
+        else:
+            olds = [df] + olds
+            corrs = show_corrs(olds, ["new"] + [f"old{i}" for i in nums], method=method)
     else:
-        corrs = show_corrs(
-            olds, [f"old{i}" for i in range(1, len(olds))], method=method
-        )
+        corrs = show_corrs(olds, [f"old{i}" for i in nums], method=method)
     return corrs
 
 
+@do_on_dfs
+def remove_unavailable(df: pd.DataFrame) -> pd.DataFrame:
+    """对日频或月频因子值，剔除st股、不正常交易的股票和上市不足60天的股票
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        因子值，index是时间，columns是股票代码，values是因子值
+
+    Returns
+    -------
+    pd.DataFrame
+        剔除后的因子值
+    """
+    df0 = df.resample("M").last()
+    if df.shape[0] / df0.shape[0] > 2:
+        daily = 1
+    else:
+        daily = 0
+    if daily:
+        state = read_daily(state=1).replace(0, np.nan)
+        st = read_daily(st=1)
+        age = read_daily(age=1)
+        st = (1 - st).replace(0, np.nan)
+        age = ((age >= 60) + 0).replace(0, np.nan)
+        df = df * age * st * state
+    else:
+        moon = pure_moon(no_read_indu=1)
+        moon.set_basic_data()
+        moon.judge_month()
+        df = moon.tris_monthly * df
+    return df
+
+
+class frequency_controller(object):
+    def __init__(self, freq: str):
+        self.homeplace = HomePlace()
+        self.freq = freq
+
+        if freq == "M":
+            self.counts_one_year = 12
+            self.time_shift = pd.DateOffset(months=1)
+            self.states_files = (
+                self.homeplace.daily_data_file + "states_monthly.parquet"
+            )
+            self.sts_files = self.homeplace.daily_data_file + "sts_monthly.parquet"
+            self.comment_name = "月"
+            self.days_in = 20
+        elif freq == "W":
+            self.counts_one_year = 52
+            self.time_shift = pd.DateOffset(weeks=1)
+            self.states_files = self.homeplace.daily_data_file + "states_weekly.parquet"
+            self.sts_files = self.homeplace.daily_data_file + "sts_weekly.parquet"
+            self.comment_name = "周"
+            self.days_in = 5
+        else:
+            raise ValueError("'暂时不支持此频率哈🤒，目前仅支持月频'M'，和周频'W'")
+
+    def next_end(self, x):
+        """找到下个周期的最后一天"""
+        if self.freq == "M":
+            return x + pd.DateOffset(months=1) + pd.tseries.offsets.MonthEnd()
+        elif self.freq == "W":
+            return x + pd.DateOffset(weeks=1)
+        else:
+            raise ValueError("'暂时不支持此频率哈🤒，目前仅支持月频'M'，和周频'W'")
+
+
 class pure_moon(object):
     __slots__ = [
         "homeplace",
         "sts_monthly_file",
         "states_monthly_file",
         "factors",
         "codes",
@@ -1298,35 +1403,56 @@
         "__factors_out",
         "ics",
         "rankics",
         "factor_turnover_rates",
         "factor_turnover_rate",
         "group_rets_std",
         "group_rets_stds",
+        "group_rets_skews",
+        "group_rets_skew",
         "wind_out",
         "swindustry_dummy",
         "zxindustry_dummy",
         "closes2_monthly",
         "rets_monthly_last",
+        "freq_ctrl",
+        "freq",
+        "factor_cover",
+        "factor_cross_skew",
+        "factor_cross_skew_after_neu",
+        "pos_neg_rate",
+        "corr_itself",
+        "factor_cross_stds",
+        "corr_itself_shift2",
+        "rets_all",
+        "inner_long_ret_yearly",
+        "inner_short_ret_yearly",
+        "inner_long_net_values",
+        "inner_short_net_values",
     ]
 
     @classmethod
     @lru_cache(maxsize=None)
     def __init__(
         cls,
+        freq: str = "M",
         no_read_indu: bool = 0,
         swindustry_dummy: pd.DataFrame = None,
         zxindustry_dummy: pd.DataFrame = None,
         read_in_swindustry_dummy: bool = 0,
     ):
         cls.homeplace = HomePlace()
+        cls.freq = freq
+        cls.freq_ctrl = frequency_controller(freq)
         # 已经算好的月度st状态文件
-        cls.sts_monthly_file = homeplace.daily_data_file + "sts_monthly.feather"
+        # week_here
+        cls.sts_monthly_file = cls.freq_ctrl.sts_files
         # 已经算好的月度交易状态文件
-        cls.states_monthly_file = homeplace.daily_data_file + "states_monthly.feather"
+        # week_here
+        cls.states_monthly_file = cls.freq_ctrl.states_files
 
         if swindustry_dummy is not None:
             cls.swindustry_dummy = swindustry_dummy
         if zxindustry_dummy is not None:
             cls.zxindustry_dummy = zxindustry_dummy
 
         def deal_dummy(industry_dummy):
@@ -1336,37 +1462,37 @@
             industry_dummy.columns = col
             industry_dummy = industry_dummy[
                 industry_dummy.date >= pd.Timestamp("20100101")
             ]
             return industry_dummy
 
         if (swindustry_dummy is None) and (zxindustry_dummy is None):
-
             if not no_read_indu:
                 if read_in_swindustry_dummy:
+                    # week_here
                     cls.swindustry_dummy = (
-                        pd.read_feather(
-                            cls.homeplace.daily_data_file + "申万行业2021版哑变量.feather"
+                        pd.read_parquet(
+                            cls.homeplace.daily_data_file + "申万行业2021版哑变量.parquet"
                         )
                         .fillna(0)
                         .set_index("date")
                         .groupby("code")
-                        .resample("M")
+                        .resample(freq)
                         .last()
                     )
                     cls.swindustry_dummy = deal_dummy(cls.swindustry_dummy)
-
+                # week_here
                 cls.zxindustry_dummy = (
-                    pd.read_feather(
-                        cls.homeplace.daily_data_file + "中信一级行业哑变量代码版.feather"
+                    pd.read_parquet(
+                        cls.homeplace.daily_data_file + "中信一级行业哑变量代码版.parquet"
                     )
                     .fillna(0)
                     .set_index("date")
                     .groupby("code")
-                    .resample("M")
+                    .resample(freq)
                     .last()
                     .fillna(0)
                 )
 
                 cls.zxindustry_dummy = deal_dummy(cls.zxindustry_dummy)
 
     @property
@@ -1374,47 +1500,83 @@
         return self.__factors_out
 
     def __call__(self):
         """调用对象则返回因子值"""
         return self.factors_out
 
     @classmethod
+    @lru_cache(maxsize=None)
     def set_basic_data(
         cls,
-        age: pd.DataFrame,
-        st: pd.DataFrame,
-        state: pd.DataFrame,
-        open: pd.DataFrame,
-        close: pd.DataFrame,
-        capital: pd.DataFrame,
+        ages: pd.DataFrame = None,
+        sts: pd.DataFrame = None,
+        states: pd.DataFrame = None,
+        opens: pd.DataFrame = None,
+        closes: pd.DataFrame = None,
+        capitals: pd.DataFrame = None,
+        opens_average_first_day: bool = 0,
+        total_cap: bool = 0,
     ):
+        if ages is None:
+            ages = read_daily(age=1, start=20100101)
+        if sts is None:
+            sts = read_daily(st=1, start=20100101)
+        if states is None:
+            states = read_daily(state=1, start=20100101)
+        if opens is None:
+            if opens_average_first_day:
+                opens = read_daily(vwap=1, start=20100101)
+            else:
+                opens = read_daily(open=1, start=20100101)
+        if closes is None:
+            closes = read_daily(close=1, start=20100101)
+        if capitals is None:
+            if total_cap:
+                capitals = (
+                    read_daily(total_cap=1, start=20100101).resample(cls.freq).last()
+                )
+            else:
+                capitals = (
+                    read_daily(flow_cap=1, start=20100101).resample(cls.freq).last()
+                )
         # 上市天数文件
-        cls.ages = age
+        cls.ages = ages
         # st日子标志文件
-        cls.sts = st.fillna(0)
+        cls.sts = sts.fillna(0)
         # cls.sts = 1 - cls.sts.fillna(0)
         # 交易状态文件
-        cls.states = state
+        cls.states = states
         # 复权开盘价数据文件
-        cls.opens = open
+        cls.opens = opens
         # 复权收盘价数据文件
-        cls.closes = close
+        cls.closes = closes
         # 月底流通市值数据
-        cls.capital = capital
-        cls.opens = cls.opens.replace(0, np.nan)
-        cls.closes = cls.closes.replace(0, np.nan)
+        cls.capital = capitals
+        if cls.opens is not None:
+            cls.opens = cls.opens.replace(0, np.nan)
+        if cls.closes is not None:
+            cls.closes = cls.closes.replace(0, np.nan)
 
-    def set_factor_df_date_as_index(self, df):
+    def set_factor_df_date_as_index(self, df: pd.DataFrame):
         """设置因子数据的dataframe，因子表列名应为股票代码，索引应为时间"""
-        df = df.reset_index()
-        df.columns = ["date"] + list(df.columns)[1:]
-        self.factors = df
-        self.factors = self.factors.set_index("date")
-        self.factors = self.factors.resample("M").last()
-        self.factors = self.factors.reset_index()
+        # week_here
+        self.factors = df.resample(self.freq).last().dropna(how="all")
+        self.factor_cover = np.sign(self.factors.abs() + 1).sum().sum()
+        opens = self.opens[self.opens.index >= self.factors.index.min()]
+        total = np.sign(opens.resample(self.freq).last()).sum().sum()
+        self.factor_cover = min(self.factor_cover / total, 1)
+        self.factor_cross_skew = self.factors.skew(axis=1).mean()
+        pos_num = ((self.factors > 0) + 0).sum().sum()
+        neg_num = ((self.factors < 0) + 0).sum().sum()
+        self.pos_neg_rate = pos_num / (neg_num + pos_num)
+        self.corr_itself = show_corr(self.factors, self.factors.shift(1), plt_plot=0)
+        self.corr_itself_shift2 = show_corr(
+            self.factors, self.factors.shift(2), plt_plot=0
+        )
+        self.factor_cross_stds = self.factors.std(axis=1)
 
     @classmethod
     def judge_month_st(cls, df):
         """比较一个月内st的天数，如果st天数多，就删除本月，如果正常多，就保留本月"""
         st_count = len(df[df == 1])
         normal_count = len(df[df != 1])
         if st_count >= normal_count:
@@ -1433,62 +1595,93 @@
             return 1
 
     @classmethod
     def read_add(cls, pridf, df, func):
         """由于数据更新，过去计算的月度状态可能需要追加"""
         if pridf.index.max() > df.index.max():
             df_add = pridf[pridf.index > df.index.max()]
-            df_add = df_add.resample("M").apply(func)
-            df = pd.concat([df, df_add])
-            return df
+            if df_add.shape[0] > int(cls.freq_ctrl.days_in / 2):
+                df_1 = df_add.index.max()
+                year = df_1.year
+                month = df_1.month
+                last = tt.date.get_close(year=year, m=month).pd_date()
+                if (last == df_1)[0]:
+                    # week_here
+                    df_add = df_add.resample(cls.freq).apply(func)
+                    df = pd.concat([df, df_add])
+                    return df
+                else:
+                    df_add = df_add[
+                        df_add.index < pd.Timestamp(year=year, month=month, day=1)
+                    ]
+                    if df_add.shape[0] > 0:
+                        df_add = df_add.resample(cls.freq).apply(func)
+                        df = pd.concat([df, df_add])
+                        return df
+                    else:
+                        return df
+            else:
+                return df
         else:
             return df
 
     @classmethod
     def daily_to_monthly(cls, pridf, path, func):
         """把日度的交易状态、st、上市天数，转化为月度的，并生成能否交易的判断
         读取本地已经算好的文件，并追加新的时间段部分，如果本地没有就直接全部重新算"""
         try:
-            month_df = pd.read_feather(path)
-            month_df = month_df.set_index(list(month_df.columns)[0])
+            month_df = pd.read_parquet(path)
             month_df = cls.read_add(pridf, month_df, func)
-            month_df.reset_index().to_feather(path)
+            month_df.to_parquet(path)
         except Exception as e:
             if not STATES["NO_LOG"]:
                 logger.error("error occurs when read state files")
                 logger.error(e)
             print("state file rewriting……")
-            month_df = pridf.resample("M").apply(func)
-            month_df.reset_index().to_feather(path)
+            # week_here
+            df_1 = pridf.index.max()
+            year = df_1.year
+            month = df_1.month
+            last = tt.date.get_close(year=year, m=month).pd_date()
+            if not (last == df_1)[0]:
+                pridf = pridf[pridf.index < pd.Timestamp(year=year, month=month, day=1)]
+            month_df = pridf.resample(cls.freq).apply(func)
+            month_df.to_parquet(path)
         return month_df
 
     @classmethod
     @lru_cache(maxsize=None)
     def judge_month(cls):
         """生成一个月综合判断的表格"""
-
-        cls.sts_monthly = cls.daily_to_monthly(
-            cls.sts, cls.sts_monthly_file, cls.judge_month_st
-        )
-        cls.states_monthly = cls.daily_to_monthly(
-            cls.states, cls.states_monthly_file, cls.judge_month_state
-        )
-        cls.ages_monthly = cls.ages.resample("M").last()
-        cls.ages_monthly = np.sign(cls.ages_monthly.applymap(lambda x: x - 60)).replace(
-            -1, 0
-        )
-        cls.tris_monthly = cls.sts_monthly * cls.states_monthly * cls.ages_monthly
-        cls.tris_monthly = cls.tris_monthly.replace(0, np.nan)
+        if cls.freq == "M":
+            cls.sts_monthly = cls.daily_to_monthly(
+                cls.sts, cls.sts_monthly_file, cls.judge_month_st
+            )
+            cls.states_monthly = cls.daily_to_monthly(
+                cls.states, cls.states_monthly_file, cls.judge_month_state
+            )
+            # week_here
+            cls.ages_monthly = (cls.ages.resample(cls.freq).last() > 60) + 0
+            cls.tris_monthly = cls.sts_monthly * cls.states_monthly * cls.ages_monthly
+            cls.tris_monthly = cls.tris_monthly.replace(0, np.nan)
+        else:
+            cls.tris_monthly = (
+                (1 - cls.sts).resample(cls.freq).last().ffill(limit=2)
+                * cls.states.resample(cls.freq).last().ffill(limit=2)
+                * ((cls.ages.resample(cls.freq).last() > 60) + 0)
+            ).replace(0, np.nan)
 
     @classmethod
     @lru_cache(maxsize=None)
     def get_rets_month(cls):
         """计算每月的收益率，并根据每月做出交易状态，做出删减"""
-        cls.opens_monthly = cls.opens.resample("M").first()
-        cls.closes_monthly = cls.closes.resample("M").last()
+        # week_here
+        cls.opens_monthly = cls.opens.resample(cls.freq).first()
+        # week_here
+        cls.closes_monthly = cls.closes.resample(cls.freq).last()
         cls.rets_monthly = (cls.closes_monthly - cls.opens_monthly) / cls.opens_monthly
         cls.rets_monthly = cls.rets_monthly * cls.tris_monthly
         cls.rets_monthly = cls.rets_monthly.stack().reset_index()
         cls.rets_monthly.columns = ["date", "code", "ret"]
 
     @classmethod
     def neutralize_factors(cls, df):
@@ -1527,24 +1720,27 @@
         else:
             cls.cap["cap_size"] = np.log(cls.cap["cap_size"])
 
     def get_neutral_factors(
         self, zxindustry_dummies=0, swindustry_dummies=0, only_cap=0
     ):
         """对因子进行行业市值中性化"""
-        self.factors = self.factors.set_index("date")
-        self.factors.index = self.factors.index + pd.DateOffset(months=1)
-        self.factors = self.factors.resample("M").last()
-        last_date = self.tris_monthly.index.max() + pd.DateOffset(months=1)
-        last_date = last_date + pd.tseries.offsets.MonthEnd()
+        # week_here
+        self.factors.index = self.factors.index + self.freq_ctrl.time_shift
+        # week_here
+        self.factors = self.factors.resample(self.freq).last()
+        # week_here
+        last_date = self.freq_ctrl.next_end(self.tris_monthly.index.max())
         add_tail = pd.DataFrame(1, index=[last_date], columns=self.tris_monthly.columns)
         tris_monthly = pd.concat([self.tris_monthly, add_tail])
         self.factors = self.factors * tris_monthly
-        self.factors.index = self.factors.index - pd.DateOffset(months=1)
-        self.factors = self.factors.resample("M").last()
+        # week_here
+        self.factors.index = self.factors.index - self.freq_ctrl.time_shift
+        # week_here
+        self.factors = self.factors.resample(self.freq).last()
         self.factors = self.factors.stack().reset_index()
         self.factors.columns = ["date", "code", "fac"]
         self.factors = pd.merge(
             self.factors, self.cap, how="inner", on=["date", "code"]
         )
         if not only_cap:
             if swindustry_dummies:
@@ -1557,31 +1753,33 @@
                 )
         self.factors = self.factors.set_index(["date", "code"])
         self.factors = self.factors.groupby(["date"]).apply(self.neutralize_factors)
         self.factors = self.factors.reset_index()
 
     def deal_with_factors(self):
         """删除不符合交易条件的因子数据"""
-        self.factors = self.factors.set_index("date")
         self.__factors_out = self.factors.copy()
-        self.__factors_out.columns = [i[1] for i in list(self.__factors_out.columns)]
-        self.factors.index = self.factors.index + pd.DateOffset(months=1)
-        self.factors = self.factors.resample("M").last()
+        # week_here
+        self.factors.index = self.factors.index + self.freq_ctrl.time_shift
+        # week_here
+        self.factors = self.factors.resample(self.freq).last()
         self.factors = self.factors * self.tris_monthly
         self.factors = self.factors.stack().reset_index()
         self.factors.columns = ["date", "code", "fac"]
 
     def deal_with_factors_after_neutralize(self):
         """中性化之后的因子处理方法"""
         self.factors = self.factors.set_index(["date", "code"])
         self.factors = self.factors.unstack()
         self.__factors_out = self.factors.copy()
         self.__factors_out.columns = [i[1] for i in list(self.__factors_out.columns)]
-        self.factors.index = self.factors.index + pd.DateOffset(months=1)
-        self.factors = self.factors.resample("M").last()
+        # week_here
+        self.factors.index = self.factors.index + self.freq_ctrl.time_shift
+        # week_here
+        self.factors = self.factors.resample(self.freq).last()
         self.factors.columns = list(map(lambda x: x[1], list(self.factors.columns)))
         self.factors = self.factors.stack().reset_index()
         self.factors.columns = ["date", "code", "fac"]
 
     @classmethod
     def find_limit(cls, df, up=1):
         """计算涨跌幅超过9.8%的股票，并将其存储进一个长列表里
@@ -1600,35 +1798,38 @@
         """找月初第一天就涨停"""
         """或者是月末跌停的股票"""
         cls.opens_monthly_shift = cls.opens_monthly.copy()
         cls.opens_monthly_shift = cls.opens_monthly_shift.shift(-1)
         cls.rets_monthly_begin = (
             cls.opens_monthly_shift - cls.closes_monthly
         ) / cls.closes_monthly
-        cls.closes2_monthly = cls.closes.shift(1).resample("M").last()
+        # week_here
+        cls.closes2_monthly = cls.closes.shift(1).resample(cls.freq).last()
         cls.rets_monthly_last = (
             cls.closes_monthly - cls.closes2_monthly
         ) / cls.closes2_monthly
         cls.limit_ups = cls.find_limit(cls.rets_monthly_begin, up=1)
         cls.limit_downs = cls.find_limit(cls.rets_monthly_last, up=-1)
 
     def get_ic_rankic(cls, df):
         """计算IC和RankIC"""
         df1 = df[["ret", "fac"]]
         ic = df1.corr(method="pearson").iloc[0, 1]
-        rankic = df1.corr(method="spearman").iloc[0, 1]
+        rankic = df1.rank().corr().iloc[0, 1]
         df2 = pd.DataFrame({"ic": [ic], "rankic": [rankic]})
         return df2
 
     def get_icir_rankicir(cls, df):
         """计算ICIR和RankICIR"""
         ic = df.ic.mean()
         rankic = df.rankic.mean()
-        icir = ic / np.std(df.ic) * (12 ** (0.5))
-        rankicir = rankic / np.std(df.rankic) * (12 ** (0.5))
+        # week_here
+        icir = ic / np.std(df.ic) * (cls.freq_ctrl.counts_one_year ** (0.5))
+        # week_here
+        rankicir = rankic / np.std(df.rankic) * (cls.freq_ctrl.counts_one_year ** (0.5))
         return pd.DataFrame(
             {"IC": [ic], "ICIR": [icir], "RankIC": [rankic], "RankICIR": [rankicir]},
             index=["评价指标"],
         )
 
     def get_ic_icir_and_rank(cls, df):
         """计算IC、ICIR、RankIC、RankICIR"""
@@ -1637,15 +1838,15 @@
         cls.rankics = df1.rankic
         cls.ics = cls.ics.reset_index(drop=True, level=1).to_frame()
         cls.rankics = cls.rankics.reset_index(drop=True, level=1).to_frame()
         df2 = cls.get_icir_rankicir(df1)
         df2 = df2.T
         dura = (df.date.max() - df.date.min()).days / 365
         t_value = df2.iloc[3, 0] * (dura ** (1 / 2))
-        df3 = pd.DataFrame({"评价指标": [t_value]}, index=["RankIC均值t值"])
+        df3 = pd.DataFrame({"评价指标": [t_value]}, index=["RankIC.t"])
         df4 = pd.concat([df2, df3])
         return df4
 
     @classmethod
     def get_groups(cls, df, groups_num):
         """依据因子值，判断是在第几组"""
         if "group" in list(df.columns):
@@ -1663,32 +1864,25 @@
         if len(l) < df.shape[0]:
             l = l + [groups_num] * (df.shape[0] - len(l))
         l = l[: df.shape[0]]
         df.insert(0, "group", l)
         return df
 
     @classmethod
-    def next_month_end(cls, x):
-        """找到下个月最后一天"""
-        x1 = x = x + relativedelta(months=1)
-        while x1.month == x.month:
-            x1 = x1 + relativedelta(days=1)
-        return x1 - relativedelta(days=1)
-
-    @classmethod
     def limit_old_to_new(cls, limit, data):
         """获取跌停股在旧月的组号，然后将日期调整到新月里
         涨停股则获得新月里涨停股的代码和时间，然后直接删去"""
         data1 = data.copy()
         data1 = data1.reset_index()
         data1.columns = ["data_index"] + list(data1.columns)[1:]
         old = pd.merge(limit, data1, how="inner", on=["date", "code"])
         old = old.set_index("data_index")
         old = old[["group", "date", "code"]]
-        old.date = list(map(cls.next_month_end, list(old.date)))
+        # week_here
+        old.date = list(map(cls.freq_ctrl.next_end, list(old.date)))
         return old
 
     def get_data(self, groups_num):
         """拼接因子数据和每月收益率数据，并对涨停和跌停股加以处理"""
         self.data = pd.merge(
             self.rets_monthly, self.factors, how="inner", on=["date", "code"]
         )
@@ -1696,91 +1890,124 @@
         self.data = self.data.groupby("date").apply(
             lambda x: self.get_groups(x, groups_num)
         )
         self.wind_out = self.data.copy()
         self.factor_turnover_rates = self.data.pivot(
             index="date", columns="code", values="group"
         )
-        self.factor_turnover_rates = self.factor_turnover_rates.diff()
-        change = ((np.abs(np.sign(self.factor_turnover_rates)) == 1) + 0).sum(axis=1)
-        still = ((self.factor_turnover_rates == 0) + 0).sum(axis=1)
-        self.factor_turnover_rates = change / (change + still)
-        self.factor_turnover_rate = self.factor_turnover_rates.mean()
+        rates = []
+        for i in range(1, groups_num + 1):
+            son = (self.factor_turnover_rates == i) + 0
+            son1 = son.diff()
+            # self.factor_turnover_rates = self.factor_turnover_rates.diff()
+            change = ((np.abs(np.sign(son1)) == 1) + 0).sum(axis=1)
+            still = (((son1 == 0) + 0) * son).sum(axis=1)
+            rate = change / (change + still)
+            rates.append(rate.to_frame(f"group{i}"))
+        rates = pd.concat(rates, axis=1).fillna(0)
+        self.factor_turnover_rates = rates
         self.data = self.data.reset_index(drop=True)
         limit_ups_object = self.limit_old_to_new(self.limit_ups, self.data)
         limit_downs_object = self.limit_old_to_new(self.limit_downs, self.data)
         self.data = self.data.drop(limit_ups_object.index)
         rets_monthly_limit_downs = pd.merge(
             self.rets_monthly, limit_downs_object, how="inner", on=["date", "code"]
         )
         self.data = pd.concat([self.data, rets_monthly_limit_downs])
 
-    def select_data_time(self, time_start, time_end):
-        """筛选特定的时间段"""
-        if time_start:
-            self.data = self.data[self.data.date >= time_start]
-        if time_end:
-            self.data = self.data[self.data.date <= time_end]
-
     def make_start_to_one(self, l):
         """让净值序列的第一个数变成1"""
         min_date = self.factors.date.min()
         add_date = min_date - relativedelta(days=min_date.day)
         add_l = pd.Series([1], index=[add_date])
         l = pd.concat([add_l, l])
         return l
 
     def to_group_ret(self, l):
         """每一组的年化收益率"""
-        ret = l[-1] ** (12 / len(l)) - 1
+        # week_here
+        ret = l[-1] ** (self.freq_ctrl.counts_one_year / len(l)) - 1
         return ret
 
-    def get_group_rets_net_values(self, groups_num=10, value_weighted=False):
+    def get_group_rets_net_values(
+        self, groups_num=10, value_weighted=False, trade_cost_double_side=0
+    ):
         """计算组内每一期的平均收益，生成每日收益率序列和净值序列"""
         if value_weighted:
             cap_value = self.capital.copy()
-            cap_value = cap_value.resample("M").last().shift(1)
+            # week_here
+            cap_value = cap_value.resample(self.freq).last().shift(1)
             cap_value = cap_value * self.tris_monthly
             # cap_value=np.log(cap_value)
             cap_value = cap_value.stack().reset_index()
             cap_value.columns = ["date", "code", "cap_value"]
             self.data = pd.merge(self.data, cap_value, on=["date", "code"])
 
             def in_g(df):
                 df.cap_value = df.cap_value / df.cap_value.sum()
                 df.ret = df.ret * df.cap_value
                 return df.ret.sum()
 
             self.group_rets = self.data.groupby(["date", "group"]).apply(in_g)
+            self.rets_all = self.data.groupby(["date"]).apply(in_g)
             self.group_rets_std = "市值加权暂未设置该功能，敬请期待🌙"
         else:
             self.group_rets = self.data.groupby(["date", "group"]).apply(
                 lambda x: x.ret.mean()
             )
-            self.group_rets_stds = self.data.groupby(["date", "group"]).apply(
-                lambda x: x.ret.std()
+            self.rets_all = self.data.groupby(["date"]).apply(lambda x: x.ret.mean())
+            self.group_rets_stds = self.data.groupby(["date", "group"]).ret.std()
+            self.group_rets_std = (
+                self.group_rets_stds.reset_index().groupby("group").mean()
+            )
+            self.group_rets_skews = self.data.groupby(["date", "group"]).ret.skew()
+            self.group_rets_skew = (
+                self.group_rets_skews.reset_index().groupby("group").mean()
             )
-            self.group_rets_std = self.group_rets_stds.groupby("group").mean()
         # dropna是因为如果股票行情数据比因子数据的截止日期晚，而最后一个月发生月初跌停时，会造成最后某组多出一个月的数据
         self.group_rets = self.group_rets.unstack()
         self.group_rets = self.group_rets[
             self.group_rets.index <= self.factors.date.max()
         ]
         self.group_rets.columns = list(map(str, list(self.group_rets.columns)))
         self.group_rets = self.group_rets.add_prefix("group")
+        self.group_rets = (
+            self.group_rets - self.factor_turnover_rates * trade_cost_double_side
+        )
+        self.rets_all = (
+            self.rets_all
+            - self.factor_turnover_rates.mean(axis=1) * trade_cost_double_side
+        ).dropna()
         self.long_short_rets = (
             self.group_rets["group1"] - self.group_rets["group" + str(groups_num)]
         )
-        self.long_short_net_values = (self.long_short_rets + 1).cumprod()
+        self.inner_rets_long = self.group_rets.group1 - self.rets_all
+        self.inner_rets_short = (
+            self.rets_all - self.group_rets["group" + str(groups_num)]
+        )
+        self.long_short_net_values = self.make_start_to_one(
+            (self.long_short_rets + 1).cumprod()
+        )
         if self.long_short_net_values[-1] <= self.long_short_net_values[0]:
             self.long_short_rets = (
                 self.group_rets["group" + str(groups_num)] - self.group_rets["group1"]
             )
-            self.long_short_net_values = (self.long_short_rets + 1).cumprod()
-        self.long_short_net_values = self.make_start_to_one(self.long_short_net_values)
+            self.long_short_net_values = self.make_start_to_one(
+                (self.long_short_rets + 1).cumprod()
+            )
+            self.inner_rets_long = (
+                self.group_rets["group" + str(groups_num)] - self.rets_all
+            )
+            self.inner_rets_short = self.rets_all - self.group_rets.group1
+        self.inner_long_net_values = self.make_start_to_one(
+            (self.inner_rets_long + 1).cumprod()
+        )
+        self.inner_short_net_values = self.make_start_to_one(
+            (self.inner_rets_short + 1).cumprod()
+        )
         self.group_rets = self.group_rets.assign(long_short=self.long_short_rets)
         self.group_net_values = self.group_rets.applymap(lambda x: x + 1)
         self.group_net_values = self.group_net_values.cumprod()
         self.group_net_values = self.group_net_values.apply(self.make_start_to_one)
         a = groups_num ** (0.5)
         # 判断是否要两个因子画表格
         if a == int(a):
@@ -1794,18 +2021,34 @@
                 index=list(range(1, int(a) + 1)),
             )
             print("这是self.square_rets", self.square_rets)
 
     def get_long_short_comments(self, on_paper=False):
         """计算多空对冲的相关评价指标
         包括年化收益率、年化波动率、信息比率、月度胜率、最大回撤率"""
+        # week_here
         self.long_short_ret_yearly = (
-            self.long_short_net_values[-1] ** (12 / len(self.long_short_net_values)) - 1
+            self.long_short_net_values[-1]
+            ** (self.freq_ctrl.counts_one_year / len(self.long_short_net_values))
+            - 1
+        )
+        self.inner_long_ret_yearly = (
+            self.inner_long_net_values[-1]
+            ** (self.freq_ctrl.counts_one_year / len(self.inner_long_net_values))
+            - 1
+        )
+        self.inner_short_ret_yearly = (
+            self.inner_short_net_values[-1]
+            ** (self.freq_ctrl.counts_one_year / len(self.inner_short_net_values))
+            - 1
+        )
+        # week_here
+        self.long_short_vol_yearly = np.std(self.long_short_rets) * (
+            self.freq_ctrl.counts_one_year**0.5
         )
-        self.long_short_vol_yearly = np.std(self.long_short_rets) * (12**0.5)
         self.long_short_info_ratio = (
             self.long_short_ret_yearly / self.long_short_vol_yearly
         )
         self.long_short_win_times = len(self.long_short_rets[self.long_short_rets > 0])
         self.long_short_win_ratio = self.long_short_win_times / len(
             self.long_short_rets
         )
@@ -1820,102 +2063,163 @@
                         self.long_short_ret_yearly,
                         self.long_short_vol_yearly,
                         self.long_short_info_ratio,
                         self.long_short_win_ratio,
                         self.max_retreat,
                     ]
                 },
-                index=["年化收益率", "年化波动率", "收益波动比", "月度胜率", "最大回撤率"],
+                # week_here
+                index=[
+                    "年化收益率",
+                    "年化波动率",
+                    "收益波动比",
+                    f"{self.freq_ctrl.comment_name}度胜率",
+                    "最大回撤率",
+                ],
             )
         else:
             self.long_short_comments = pd.DataFrame(
                 {
                     "评价指标": [
                         self.long_short_ret_yearly,
                         self.long_short_vol_yearly,
                         self.long_short_info_ratio,
                         self.long_short_win_ratio,
                         self.max_retreat,
                     ]
                 },
-                index=["年化收益率", "年化波动率", "信息比率", "月度胜率", "最大回撤率"],
+                # week_here
+                index=[
+                    "年化收益率",
+                    "年化波动率",
+                    "信息比率",
+                    f"{self.freq_ctrl.comment_name}度胜率",
+                    "最大回撤率",
+                ],
             )
 
-    def get_total_comments(self):
-        """综合IC、ICIR、RankIC、RankICIR,年化收益率、年化波动率、信息比率、月度胜率、最大回撤率"""
+    def get_total_comments(self, groups_num):
+        """综合IC、ICIR、RankIC、RankICIR,年化收益率、年化波动率、信息比率、胜率、最大回撤率"""
+        rankic = self.rankics.mean()
+        rankic_win = self.rankics[self.rankics * rankic > 0]
+        rankic_win_ratio = rankic_win.dropna().shape[0] / self.rankics.dropna().shape[0]
+        self.factor_cross_skew_after_neu = self.__factors_out.skew(axis=1).mean()
+        if self.ic_icir_and_rank.iloc[2, 0] > 0:
+            self.factor_turnover_rate = self.factor_turnover_rates[
+                f"group{groups_num}"
+            ].mean()
+        else:
+            self.factor_turnover_rate = self.factor_turnover_rates["group1"].mean()
         self.total_comments = pd.concat(
             [
                 self.ic_icir_and_rank,
+                pd.DataFrame(
+                    {"评价指标": [rankic_win_ratio]},
+                    index=["RankIC胜率"],
+                ),
                 self.long_short_comments,
-                pd.DataFrame({"评价指标": [self.factor_turnover_rate]}, index=["月均换手率"]),
+                # week_here
+                pd.DataFrame(
+                    {
+                        "评价指标": [
+                            self.factor_turnover_rate,
+                            self.factor_cover,
+                            self.pos_neg_rate,
+                            self.factor_cross_skew,
+                            self.inner_long_ret_yearly,
+                            self.inner_long_ret_yearly
+                            / (
+                                self.inner_long_ret_yearly + self.inner_short_ret_yearly
+                            ),
+                            self.corr_itself,
+                        ]
+                    },
+                    index=[
+                        f"多头{self.freq_ctrl.comment_name}均换手",
+                        "因子覆盖率",
+                        "因子正值占比",
+                        "因子截面偏度",
+                        "多头超均收益",
+                        "多头收益占比",
+                        "一阶自相关性",
+                    ],
+                ),
             ]
         )
 
-    def plot_net_values(self, y2, filename, iplot=1, ilegend=1):
+    def plot_net_values(self, y2, filename, iplot=1, ilegend=1, without_breakpoint=0):
         """使用matplotlib来画图，y2为是否对多空组合采用双y轴"""
         if not iplot:
             fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(33, 8))
             self.group_net_values.plot(secondary_y=y2, rot=60, ax=ax[0])
             self.group_net_values.plot(secondary_y=y2, ax=ax[0])
             b = self.rankics.copy()
             b.index = [int(i.year) if i.month == 1 else "" for i in list(b.index)]
             b.plot(kind="bar", rot=60, ax=ax[1])
-            self.factor_turnover_rates.plot(rot=60, ax=ax[2])
+            self.factor_cross_stds.plot(rot=60, ax=ax[2])
 
             filename_path = filename + ".png"
             if not STATES["NO_SAVE"]:
                 plt.savefig(filename_path)
         else:
-            tris = pd.concat(
-                [self.group_net_values, self.factor_turnover_rates, self.rankics],
-                axis=1,
-            ).rename(columns={0: "turnover_rate"})
+            tris = (
+                pd.concat(
+                    [self.group_net_values, self.factor_cross_stds, self.rankics],
+                    axis=1,
+                )
+                .rename(columns={0: "因子截面标准差"})
+                .dropna()
+            )
+            if without_breakpoint:
+                tris = tris.dropna()
             figs = cf.figures(
                 tris,
                 [
                     dict(kind="line", y=list(self.group_net_values.columns)),
-                    dict(kind="line", y="turnover_rate"),
+                    dict(kind="bar", y="因子截面标准差"),
                     dict(kind="bar", y="rankic"),
                 ],
                 asList=True,
             )
             comments = (
                 self.total_comments.applymap(lambda x: round(x, 4))
                 .rename(index={"RankIC均值t值": "RankIC.t"})
                 .reset_index()
             )
             here = pd.concat(
                 [
-                    comments.iloc[:5, :].reset_index(drop=True),
-                    comments.iloc[5:, :].reset_index(drop=True),
+                    comments.iloc[:6, :].reset_index(drop=True),
+                    comments.iloc[6:12, :].reset_index(drop=True),
+                    comments.iloc[12:, :].reset_index(drop=True),
                 ],
                 axis=1,
             )
-            here.columns = ["信息系数", "结果", "绩效指标", "结果"]
+            here.columns = ["信息系数", "结果", "绩效指标", "结果", "其他指标", "结果"]
             # here=here.to_numpy().tolist()+[['信息系数','结果','绩效指标','结果']]
             table = FF.create_table(here.iloc[::-1])
             table.update_yaxes(matches=None)
             # table=go.Figure([go.Table(header=dict(values=list(here.columns)),cells=dict(values=here.to_numpy().tolist()))])
             figs.append(table)
             figs = [figs[-1]] + figs[:-1]
             figs[1].update_layout(
                 legend=dict(yanchor="top", y=0.99, xanchor="left", x=0.01)
             )
             base_layout = cf.tools.get_base_layout(figs)
 
             sp = cf.subplots(
                 figs,
-                shape=(2, 10),
+                shape=(2, 11),
                 base_layout=base_layout,
                 vertical_spacing=0.15,
                 horizontal_spacing=0.03,
                 shared_yaxes=False,
                 specs=[
                     [
-                        {"rowspan": 2, "colspan": 3},
+                        {"rowspan": 2, "colspan": 4},
+                        None,
                         None,
                         None,
                         {"rowspan": 2, "colspan": 4},
                         None,
                         None,
                         None,
                         {"colspan": 3},
@@ -1926,20 +2230,21 @@
                         None,
                         None,
                         None,
                         None,
                         None,
                         None,
                         None,
+                        None,
                         {"colspan": 3},
                         None,
                         None,
                     ],
                 ],
-                subplot_titles=["净值曲线", "月换手率", "Rank IC时序图", "绩效指标"],
+                subplot_titles=["净值曲线", "因子截面标准差", "Rank IC时序图", "绩效指标"],
             )
             sp["layout"].update(showlegend=ilegend)
             # los=sp['layout']['annotations']
             # los[0]['font']['color']='#000000'
             # los[1]['font']['color']='#000000'
             # los[2]['font']['color']='#000000'
             # los[3]['font']['color']='#000000'
@@ -1979,41 +2284,40 @@
     @classmethod
     @lru_cache(maxsize=None)
     def prerpare(cls):
         """通用数据准备"""
         cls.judge_month()
         cls.get_rets_month()
 
-    @kk.desktop_sender(title="嘿，回测结束啦～🗓")
     def run(
         self,
         groups_num=10,
         neutralize=False,
         boxcox=False,
+        trade_cost_double_side=0,
         value_weighted=False,
         y2=False,
         plt_plot=True,
         plotly_plot=False,
         filename="分组净值图",
-        time_start=None,
-        time_end=None,
         print_comments=True,
         comments_writer=None,
         net_values_writer=None,
         rets_writer=None,
         comments_sheetname=None,
         net_values_sheetname=None,
         rets_sheetname=None,
         on_paper=False,
         sheetname=None,
         zxindustry_dummies=0,
         swindustry_dummies=0,
         only_cap=0,
         iplot=1,
-        ilegend=1,
+        ilegend=0,
+        without_breakpoint=0,
     ):
         """运行回测部分"""
         if comments_writer and not (comments_sheetname or sheetname):
             raise IOError("把total_comments输出到excel中时，必须指定sheetname🤒")
         if net_values_writer and not (net_values_sheetname or sheetname):
             raise IOError("把group_net_values输出到excel中时，必须指定sheetname🤒")
         if rets_writer and not (rets_sheetname or sheetname):
@@ -2033,20 +2337,21 @@
                 only_cap=only_cap,
             )
             self.deal_with_factors_after_neutralize()
         else:
             self.deal_with_factors()
         self.get_limit_ups_downs()
         self.get_data(groups_num)
-        self.select_data_time(time_start, time_end)
         self.get_group_rets_net_values(
-            groups_num=groups_num, value_weighted=value_weighted
+            groups_num=groups_num,
+            value_weighted=value_weighted,
+            trade_cost_double_side=trade_cost_double_side,
         )
         self.get_long_short_comments(on_paper=on_paper)
-        self.get_total_comments()
+        self.get_total_comments(groups_num=groups_num)
         if on_paper:
             group1_ttest = ss.ttest_1samp(self.group_rets.group1, 0).pvalue
             group10_ttest = ss.ttest_1samp(
                 self.group_rets[f"group{groups_num}"], 0
             ).pvalue
             group_long_short_ttest = ss.ttest_1samp(self.long_short_rets, 0).pvalue
             group1_ret = self.group_rets.group1.mean()
@@ -2074,24 +2379,29 @@
             )
             self.total_comments = pd.concat([papers, self.total_comments])
 
         if plt_plot:
             if not STATES["NO_PLOT"]:
                 if filename:
                     self.plot_net_values(
-                        y2=y2, filename=filename, iplot=iplot, ilegend=bool(ilegend)
+                        y2=y2,
+                        filename=filename,
+                        iplot=iplot,
+                        ilegend=bool(ilegend),
+                        without_breakpoint=without_breakpoint,
                     )
                 else:
                     self.plot_net_values(
                         y2=y2,
                         filename=self.factors_file.split(".")[-2].split("/")[-1]
                         + str(groups_num)
                         + "分组",
                         iplot=iplot,
                         ilegend=bool(ilegend),
+                        without_breakpoint=without_breakpoint,
                     )
                 plt.show()
         if plotly_plot:
             if not STATES["NO_PLOT"]:
                 if filename:
                     self.plotly_net_values(filename=filename)
                 else:
@@ -2099,16 +2409,18 @@
                         filename=self.factors_file.split(".")[-2].split("/")[-1]
                         + str(groups_num)
                         + "分组"
                     )
         if print_comments:
             if not STATES["NO_COMMENT"]:
                 tb = Texttable()
-                tb.set_cols_width([8] * 4 + [12] + [8] * 2 + [7] * 2 + [8] + [10])
-                tb.set_cols_dtype(["f"] * 11)
+                tb.set_cols_width(
+                    [8] * 5 + [9] + [8] * 2 + [7] * 2 + [8] + [8] + [9] + [10] * 5
+                )
+                tb.set_cols_dtype(["f"] * 18)
                 tb.header(list(self.total_comments.T.columns))
                 tb.add_rows(self.total_comments.T.to_numpy(), header=False)
                 print(tb.draw())
         if sheetname:
             if comments_writer:
                 if not on_paper:
                     total_comments = self.total_comments.copy()
@@ -2116,18 +2428,25 @@
                     tc[0] = str(round(tc[0] * 100, 2)) + "%"
                     tc[1] = str(round(tc[1], 2))
                     tc[2] = str(round(tc[2] * 100, 2)) + "%"
                     tc[3] = str(round(tc[3], 2))
                     tc[4] = str(round(tc[4], 2))
                     tc[5] = str(round(tc[5] * 100, 2)) + "%"
                     tc[6] = str(round(tc[6] * 100, 2)) + "%"
-                    tc[7] = str(round(tc[7], 2))
-                    tc[8] = str(round(tc[8] * 100, 2)) + "%"
+                    tc[7] = str(round(tc[7] * 100, 2)) + "%"
+                    tc[8] = str(round(tc[8], 2))
                     tc[9] = str(round(tc[9] * 100, 2)) + "%"
                     tc[10] = str(round(tc[10] * 100, 2)) + "%"
+                    tc[11] = str(round(tc[11] * 100, 2)) + "%"
+                    tc[12] = str(round(tc[12] * 100, 2)) + "%"
+                    tc[13] = str(round(tc[13] * 100, 2)) + "%"
+                    tc[14] = str(round(tc[14], 2))
+                    tc[15] = str(round(tc[15], 2))
+                    tc[16] = str(round(tc[16] * 100, 2)) + "%"
+                    tc[17] = str(round(tc[17] * 100, 2)) + "%"
                     new_total_comments = pd.DataFrame(
                         {sheetname: tc}, index=total_comments.index
                     )
                     new_total_comments.T.to_excel(comments_writer, sheet_name=sheetname)
                 else:
                     self.total_comments.rename(columns={"评价指标": sheetname}).to_excel(
                         comments_writer, sheet_name=sheetname
@@ -2153,18 +2472,25 @@
                 tc[0] = str(round(tc[0] * 100, 2)) + "%"
                 tc[1] = str(round(tc[1], 2))
                 tc[2] = str(round(tc[2] * 100, 2)) + "%"
                 tc[3] = str(round(tc[3], 2))
                 tc[4] = str(round(tc[4], 2))
                 tc[5] = str(round(tc[5] * 100, 2)) + "%"
                 tc[6] = str(round(tc[6] * 100, 2)) + "%"
-                tc[7] = str(round(tc[7], 2))
-                tc[8] = str(round(tc[8] * 100, 2)) + "%"
+                tc[7] = str(round(tc[7] * 100, 2)) + "%"
+                tc[8] = str(round(tc[8], 2))
                 tc[9] = str(round(tc[9] * 100, 2)) + "%"
                 tc[10] = str(round(tc[10] * 100, 2)) + "%"
+                tc[11] = str(round(tc[11] * 100, 2)) + "%"
+                tc[12] = str(round(tc[12] * 100, 2)) + "%"
+                tc[13] = str(round(tc[13] * 100, 2)) + "%"
+                tc[14] = str(round(tc[14], 2))
+                tc[15] = str(round(tc[15], 2))
+                tc[16] = str(round(tc[16] * 100, 2)) + "%"
+                tc[17] = str(round(tc[17] * 100, 2)) + "%"
                 new_total_comments = pd.DataFrame(
                     {comments_sheetname: tc}, index=total_comments.index
                 )
                 new_total_comments.T.to_excel(
                     comments_writer, sheet_name=comments_sheetname
                 )
             if net_values_writer and net_values_sheetname:
@@ -2181,25 +2507,28 @@
                 group_rets.index = group_rets.index.strftime("%Y/%m/%d")
                 group_rets.columns = [
                     f"分组{i}" for i in range(1, len(list(group_rets.columns)))
                 ] + ["多空对冲（右轴）"]
                 group_rets.to_excel(rets_writer, sheet_name=rets_sheetname)
 
 
+@do_on_dfs
 class pure_moonnight(object):
     """封装选股框架"""
 
     __slots__ = ["shen"]
 
     def __init__(
         self,
         factors: pd.DataFrame,
         groups_num: int = 10,
+        freq: str = "M",
         neutralize: bool = 0,
         boxcox: bool = 1,
+        trade_cost_double_side: float = 0,
         value_weighted: bool = 0,
         y2: bool = 0,
         plt_plot: bool = 1,
         plotly_plot: bool = 0,
         filename: str = "分组净值图",
         time_start: int = None,
         time_end: int = None,
@@ -2221,46 +2550,53 @@
         closes: pd.DataFrame = None,
         capitals: pd.DataFrame = None,
         swindustry_dummy: pd.DataFrame = None,
         zxindustry_dummy: pd.DataFrame = None,
         no_read_indu: bool = 0,
         only_cap: bool = 0,
         iplot: bool = 1,
-        ilegend: bool = 1,
+        ilegend: bool = 0,
+        without_breakpoint: bool = 0,
+        opens_average_first_day: bool = 0,
+        total_cap: bool = 0,
     ) -> None:
         """一键回测框架，测试单因子的月频调仓的分组表现
         每月月底计算因子值，月初第一天开盘时买入，月末收盘最后一天收盘时卖出
         剔除上市不足60天的，停牌天数超过一半的，st天数超过一半的
         月末收盘跌停的不卖出，月初开盘涨停的不买入
         由最好组和最差组的多空组合构成多空对冲组
 
         Parameters
         ----------
         factors : pd.DataFrame
             要用于检测的因子值，index是时间，columns是股票代码
         groups_num : int, optional
             分组数量, by default 10
+        freq : str, optional
+            回测频率, by default 'M'
         neutralize : bool, optional
             对流通市值取自然对数，以完成行业市值中性化, by default 0
         boxcox : bool, optional
             对流通市值做截面boxcox变换，以完成行业市值中性化, by default 1
+        trade_cost_double_side : float, optional
+            交易的双边手续费率, by default 0
         value_weighted : bool, optional
             是否用流通市值加权, by default 0
         y2 : bool, optional
             画图时是否启用第二y轴, by default 0
         plt_plot : bool, optional
             将分组净值曲线用matplotlib画出来, by default 1
         plotly_plot : bool, optional
             将分组净值曲线用plotly画出来, by default 0
         filename : str, optional
             分组净值曲线的图保存的名称, by default "分组净值图"
         time_start : int, optional
-            回测起始时间（此参数已废弃，请在因子上直接截断）, by default None
+            回测起始时间, by default None
         time_end : int, optional
-            回测终止时间（此参数已废弃，请在因子上直接截断）, by default None
+            回测终止时间, by default None
         print_comments : bool, optional
             是否打印出评价指标, by default 1
         comments_writer : pd.ExcelWriter, optional
             用于记录评价指标的xlsx文件, by default None
         net_values_writer : pd.ExcelWriter, optional
             用于记录净值序列的xlsx文件, by default None
         rets_writer : pd.ExcelWriter, optional
@@ -2301,98 +2637,163 @@
             不读入行业数据, by default 0
         only_cap : bool, optional
             仅做市值中性化, by default 0
         iplot : bool, optional
             使用cufflinks呈现回测结果, by default 1
         ilegend : bool, optional
             使用cufflinks绘图时，是否显示图例, by default 1
+        without_breakpoint : bool, optional
+            画图的时候是否去除间断点, by default 0
+        opens_average_first_day : bool, optional
+            买入时使用第一天的平均价格, by default 0
+        total_cap : bool, optional
+            加权和行业市值中性化时使用总市值, by default 0
         """
 
         if not isinstance(factors, pd.DataFrame):
             factors = factors()
-        start = datetime.datetime.strftime(factors.index.min(), "%Y%m%d")
-        if ages is None:
-            ages = read_daily(age=1, start=start)
-        if sts is None:
-            sts = read_daily(st=1, start=start)
-        if states is None:
-            states = read_daily(state=1, start=start)
-        if opens is None:
-            opens = read_daily(open=1, start=start)
-        if closes is None:
-            closes = read_daily(close=1, start=start)
-        if capitals is None:
-            capitals = read_daily(flow_cap=1, start=start).resample("M").last()
         if comments_writer is None and sheetname is not None:
-            from pure_ocean_breeze.legacy_version.v3p4.state.states import COMMENTS_WRITER
+            from pure_ocean_breeze.state.states import COMMENTS_WRITER
 
             comments_writer = COMMENTS_WRITER
         if net_values_writer is None and sheetname is not None:
-            from pure_ocean_breeze.legacy_version.v3p4.state.states import NET_VALUES_WRITER
+            from pure_ocean_breeze.state.states import NET_VALUES_WRITER
 
             net_values_writer = NET_VALUES_WRITER
         if not on_paper:
-            from pure_ocean_breeze.legacy_version.v3p4.state.states import ON_PAPER
+            from pure_ocean_breeze.state.states import ON_PAPER
 
             on_paper = ON_PAPER
-        from pure_ocean_breeze.legacy_version.v3p4.state.states import MOON_START
+        if time_start is None:
+            from pure_ocean_breeze.state.states import MOON_START
 
-        if MOON_START is not None:
-            factors = factors[factors.index >= pd.Timestamp(str(MOON_START))]
-        from pure_ocean_breeze.legacy_version.v3p4.state.states import MOON_END
+            if MOON_START is not None:
+                factors = factors[factors.index >= pd.Timestamp(str(MOON_START))]
+        else:
+            factors = factors[factors.index >= pd.Timestamp(str(time_start))]
+        if time_end is None:
+            from pure_ocean_breeze.state.states import MOON_END
 
-        if MOON_END is not None:
-            factors = factors[factors.index <= pd.Timestamp(str(MOON_END))]
+            if MOON_END is not None:
+                factors = factors[factors.index <= pd.Timestamp(str(MOON_END))]
+        else:
+            factors = factors[factors.index <= pd.Timestamp(str(time_end))]
         if boxcox + neutralize == 0:
             no_read_indu = 1
         if only_cap + no_read_indu > 0:
             only_cap = no_read_indu = 1
         if iplot:
             print_comments = 0
-        self.shen = pure_moon(
-            no_read_indu=no_read_indu,
-            swindustry_dummy=swindustry_dummy,
-            zxindustry_dummy=zxindustry_dummy,
-            read_in_swindustry_dummy=swindustry_dummies,
-        )
+        if total_cap:
+            if opens_average_first_day:
+                if freq == "M":
+                    self.shen = pure_moon_b(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week_b(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+            else:
+                if freq == "M":
+                    self.shen = pure_moon_c(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week_c(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+        else:
+            if opens_average_first_day:
+                if freq == "M":
+                    self.shen = pure_moon(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+            else:
+                if freq == "M":
+                    self.shen = pure_moon_a(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
+                elif freq == "W":
+                    self.shen = pure_week_a(
+                        freq=freq,
+                        no_read_indu=no_read_indu,
+                        swindustry_dummy=swindustry_dummy,
+                        zxindustry_dummy=zxindustry_dummy,
+                        read_in_swindustry_dummy=swindustry_dummies,
+                    )
         self.shen.set_basic_data(
-            age=ages,
-            st=sts,
-            state=states,
-            open=opens,
-            close=closes,
-            capital=capitals,
+            ages=ages,
+            sts=sts,
+            states=states,
+            opens=opens,
+            closes=closes,
+            capitals=capitals,
+            opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
         )
         self.shen.set_factor_df_date_as_index(factors)
         self.shen.prerpare()
         self.shen.run(
             groups_num=groups_num,
             neutralize=neutralize,
             boxcox=boxcox,
+            trade_cost_double_side=trade_cost_double_side,
             value_weighted=value_weighted,
             y2=y2,
             plt_plot=plt_plot,
             plotly_plot=plotly_plot,
             filename=filename,
-            time_start=time_start,
-            time_end=time_end,
             print_comments=print_comments,
             comments_writer=comments_writer,
             net_values_writer=net_values_writer,
             rets_writer=rets_writer,
             comments_sheetname=comments_sheetname,
             net_values_sheetname=net_values_sheetname,
             rets_sheetname=rets_sheetname,
             on_paper=on_paper,
             sheetname=sheetname,
             swindustry_dummies=swindustry_dummies,
             zxindustry_dummies=zxindustry_dummies,
             only_cap=only_cap,
             iplot=iplot,
             ilegend=ilegend,
+            without_breakpoint=without_breakpoint,
         )
 
     def __call__(self) -> pd.DataFrame:
         """如果做了行业市值中性化，则返回行业市值中性化之后的因子数据
 
         Returns
         -------
@@ -2417,24 +2818,64 @@
             net = self.shen.group_net_values[i]
             com = comments_on_twins(net, ret)
             com = com.to_frame(i)
             coms.append(com)
         df = pd.concat(coms, axis=1)
         return df.T
 
+    def comment_yearly(self) -> pd.DataFrame:
+        """对回测的每年表现给出评价
+
+        Returns
+        -------
+        pd.DataFrame
+            各年度的收益率
+        """
+        df = self.shen.group_net_values.resample("Y").last().pct_change()
+        df.index = df.index.year
+        return df
+
+
+class pure_week(pure_moon):
+    ...
+
+
+class pure_moon_a(pure_moon):
+    ...
+
+
+class pure_week_a(pure_moon):
+    ...
+
+
+class pure_moon_b(pure_moon):
+    ...
+
+
+class pure_week_b(pure_moon):
+    ...
+
+
+class pure_moon_c(pure_moon):
+    ...
+
+
+class pure_week_c(pure_moon):
+    ...
+
 
 class pure_fall(object):
     # DONE：修改为因子文件名可以带“日频_“，也可以不带“日频_“
     def __init__(self, daily_path: str) -> None:
         """一个使用mysql中的分钟数据，来更新因子值的框架
 
         Parameters
         ----------
         daily_path : str
-            日频因子值存储文件的名字，请以'.feather'结尾
+            日频因子值存储文件的名字，请以'.parquet'结尾
         """
         self.homeplace = HomePlace()
         # 将分钟数据拼成一张日频因子表
         self.daily_factors = None
         self.daily_factors_path = self.homeplace.factor_data_file + "日频_" + daily_path
 
     def __call__(self, monthly=False):
@@ -2443,160 +2884,14 @@
             return self.monthly_factors.copy()
         else:
             try:
                 return self.daily_factors.copy()
             except Exception:
                 return self.monthly_factors.copy()
 
-    def __add__(self, selfas):
-        """将几个因子截面标准化之后，因子值相加"""
-        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
-        fac2s = []
-        if not isinstance(selfas, Iterable):
-            if not STATES["NO_LOG"]:
-                logger.warning(f"{selfas} is changed into Iterable")
-            selfas = (selfas,)
-        for selfa in selfas:
-            fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
-            fac2s.append(fac2)
-        for i in fac2s:
-            fac1 = fac1 + i
-        new_pure = pure_fall()
-        new_pure.monthly_factors = fac1
-        return new_pure
-
-    def __mul__(self, selfas):
-        """将几个因子横截面标准化之后，使其都为正数，然后因子值相乘"""
-        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
-        fac1 = fac1 - fac1.min()
-        fac2s = []
-        if not isinstance(selfas, Iterable):
-            if not STATES["NO_LOG"]:
-                logger.warning(f"{selfas} is changed into Iterable")
-            selfas = (selfas,)
-        for selfa in selfas:
-            fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
-            fac2 = fac2 - fac2.min()
-            fac2s.append(fac2)
-        for i in fac2s:
-            fac1 = fac1 * i
-        new_pure = pure_fall()
-        new_pure.monthly_factors = fac1
-        return new_pure
-
-    def __truediv__(self, selfa):
-        """两个一正一副的因子，可以用此方法相减"""
-        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
-        fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
-        fac = fac1 - fac2
-        new_pure = pure_fall()
-        new_pure.monthly_factors = fac
-        return new_pure
-
-    def __floordiv__(self, selfa):
-        """两个因子一正一负，可以用此方法相除"""
-        fac1 = self.standardlize_in_cross_section(self.monthly_factors)
-        fac2 = self.standardlize_in_cross_section(selfa.monthly_factors)
-        fac1 = fac1 - fac1.min()
-        fac2 = fac2 - fac2.min()
-        fac = fac1 / fac2
-        fac = fac.replace(np.inf, np.nan)
-        new_pure = pure_fall()
-        new_pure.monthly_factors = fac
-        return new_pure
-
-    @kk.desktop_sender(title="嘿，正交化结束啦～🐬")
-    def __sub__(self, selfa):
-        """用主因子剔除其他相关因子、传统因子等
-        selfa可以为多个因子对象组成的元组或列表，每个辅助因子只需要有月度因子文件路径即可"""
-        if is_notebook():
-            tqdm.tqdm_notebook().pandas()
-        else:
-            tqdm.tqdm.pandas()
-        if not isinstance(selfa, Iterable):
-            if not STATES["NO_LOG"]:
-                logger.warning(f"{selfa} is changed into Iterable")
-            selfa = (selfa,)
-        fac_main = self.wide_to_long(self.monthly_factors, "fac")
-        fac_helps = [i.monthly_factors for i in selfa]
-        help_names = ["help" + str(i) for i in range(1, (len(fac_helps) + 1))]
-        fac_helps = list(map(self.wide_to_long, fac_helps, help_names))
-        fac_helps = pd.concat(fac_helps, axis=1)
-        facs = pd.concat([fac_main, fac_helps], axis=1).dropna()
-        facs = facs.groupby("date").progress_apply(
-            lambda x: self.de_in_group(x, help_names)
-        )
-        facs = facs.unstack()
-        facs.columns = list(map(lambda x: x[1], list(facs.columns)))
-        return facs
-
-    def __gt__(self, selfa):
-        """用于输出25分组表格，使用时，以x>y的形式使用，其中x,y均为pure_fall对象
-        计算时使用的是他们的月度因子表，即self.monthly_factors属性，为宽数据形式的dataframe
-        x应为首先用来的分组的主因子，y为在x分组后的组内继续分组的次因子"""
-        x = self.monthly_factors.copy()
-        y = selfa.monthly_factors.copy()
-        x = x.stack().reset_index()
-        y = y.stack().reset_index()
-        x.columns = ["date", "code", "fac"]
-        y.columns = ["date", "code", "fac"]
-        shen = pure_moon()
-        x = x.groupby("date").apply(lambda df: shen.get_groups(df, 5))
-        x = (
-            x.reset_index(drop=True)
-            .drop(columns=["fac"])
-            .rename(columns={"group": "groupx"})
-        )
-        xy = pd.merge(x, y, on=["date", "code"])
-        xy = xy.groupby(["date", "groupx"]).apply(lambda df: shen.get_groups(df, 5))
-        xy = (
-            xy.reset_index(drop=True)
-            .drop(columns=["fac"])
-            .rename(columns={"group": "groupy"})
-        )
-        xy = xy.assign(fac=xy.groupx * 5 + xy.groupy)
-        xy = xy[["date", "code", "fac"]]
-        xy = xy.set_index(["date", "code"]).unstack()
-        xy.columns = [i[1] for i in list(xy.columns)]
-        new_pure = pure_fall()
-        new_pure.monthly_factors = xy
-        return new_pure
-
-    def __rshift__(self, selfa):
-        """用于输出100分组表格，使用时，以x>>y的形式使用，其中x,y均为pure_fall对象
-        计算时使用的是他们的月度因子表，即self.monthly_factors属性，为宽数据形式的dataframe
-        x应为首先用来的分组的主因子，y为在x分组后的组内继续分组的次因子"""
-        x = self.monthly_factors.copy()
-        y = selfa.monthly_factors.copy()
-        x = x.stack().reset_index()
-        y = y.stack().reset_index()
-        x.columns = ["date", "code", "fac"]
-        y.columns = ["date", "code", "fac"]
-        shen = pure_moon()
-        x = x.groupby("date").apply(lambda df: shen.get_groups(df, 10))
-        x = (
-            x.reset_index(drop=True)
-            .drop(columns=["fac"])
-            .rename(columns={"group": "groupx"})
-        )
-        xy = pd.merge(x, y, on=["date", "code"])
-        xy = xy.groupby(["date", "groupx"]).apply(lambda df: shen.get_groups(df, 10))
-        xy = (
-            xy.reset_index(drop=True)
-            .drop(columns=["fac"])
-            .rename(columns={"group": "groupy"})
-        )
-        xy = xy.assign(fac=xy.groupx * 10 + xy.groupy)
-        xy = xy[["date", "code", "fac"]]
-        xy = xy.set_index(["date", "code"]).unstack()
-        xy.columns = [i[1] for i in list(xy.columns)]
-        new_pure = pure_fall()
-        new_pure.monthly_factors = xy
-        return new_pure
-
     def wide_to_long(self, df, i):
         """将宽数据转化为长数据，用于因子表转化和拼接"""
         df = df.stack().reset_index()
         df.columns = ["date", "code", i]
         df = df.set_index(["date", "code"])
         return df
 
@@ -2616,97 +2911,15 @@
         在横截面上做标准化
         输入的df应为，列名是股票代码，索引是时间
         """
         df = df.T
         df = (df - df.mean()) / df.std()
         df = df.T
         return df
-
-    def get_single_day_factor(self, func: Callable, day: int) -> pd.DataFrame:
-        """计算单日的因子值，通过sql数据库，读取单日的数据，然后计算因子值"""
-        sql = sqlConfig("minute_data_stock_alter")
-        df = sql.get_data(str(day))
-        the_func = partial(func)
-        df = df.groupby(["code"]).apply(the_func).to_frame()
-        df.columns = [str(day)]
-        df = df.T
-        df.index = pd.to_datetime(df.index, format="%Y%m%d")
-        return df
-
-    @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
-    def get_daily_factors_alter(self, func: Callable) -> None:
-        """用mysql逐日更新分钟数据构造的因子
-
-        Parameters
-        ----------
-        func : Callable
-            构造分钟数据使用的函数
-
-        Raises
-        ------
-        `IOError`
-            如果没有历史因子数据，将报错
-        """
-        """通过minute_data_stock_alter数据库一天一天计算因子值"""
-        try:
-            try:
-                self.daily_factors = pd.read_feather(self.daily_factors_path)
-            except Exception:
-                self.daily_factors_path = self.daily_factors_path.split("日频_")
-                self.daily_factors_path = (
-                    self.daily_factors_path[0] + self.daily_factors_path[1]
-                )
-                self.daily_factors = pd.read_feather(self.daily_factors_path)
-            self.daily_factors = self.daily_factors.rename(
-                columns={list(self.daily_factors.columns)[0]: "date"}
-            )
-            self.daily_factors = self.daily_factors.drop_duplicates(
-                subset=["date"], keep="last"
-            )
-            self.daily_factors = self.daily_factors.set_index("date")
-            sql = sqlConfig("minute_data_stock_alter")
-            now_minute_datas = sql.show_tables(full=False)
-            now_minute_data = now_minute_datas[-1]
-            now_minute_data = pd.Timestamp(now_minute_data)
-            if self.daily_factors.index.max() < now_minute_data:
-                if not STATES["NO_LOG"]:
-                    logger.info(
-                        f"上次存储的因子值到{self.daily_factors.index.max()}，而分钟数据最新到{now_minute_data}，开始更新……"
-                    )
-                old_end = datetime.datetime.strftime(
-                    self.daily_factors.index.max(), "%Y%m%d"
-                )
-                now_minute_datas = [i for i in now_minute_datas if i > old_end]
-                dfs = []
-                for c in tqdm.tqdm(now_minute_datas, desc="桂棹兮兰桨，击空明兮遂流光🌊"):
-                    df = self.get_single_day_factor(func, c)
-                    dfs.append(df)
-                dfs = pd.concat(dfs)
-                dfs = dfs.sort_index()
-                self.daily_factors = pd.concat([self.daily_factors, dfs])
-                self.daily_factors = self.daily_factors.dropna(how="all")
-                self.daily_factors = self.daily_factors[
-                    self.daily_factors.index >= pd.Timestamp(str(STATES["START"]))
-                ]
-            self.daily_factors = self.daily_factors.reset_index()
-            self.daily_factors = self.daily_factors.rename(
-                columns={list(self.daily_factors.columns)[0]: "date"}
-            )
-            self.daily_factors = self.daily_factors.drop_duplicates(
-                subset=["date"], keep="first"
-            )
-            self.daily_factors = self.daily_factors.set_index("date")
-            self.daily_factors.reset_index().to_feather(self.daily_factors_path)
-            if not STATES["NO_LOG"]:
-                logger.success("更新已完成")
-
-        except Exception:
-            raise IOError(
-                "您还没有该因子的初级数据，暂时不能更新。请先使用pure_fall_frequent或pure_fall_flexible计算历史因子值。"
-            )
+    
 
 
 class pure_fallmount(pure_fall):
     """继承自父类，专为做因子截面标准化之后相加和因子剔除其他辅助因子的作用"""
 
     def __init__(self, monthly_factors):
         """输入月度因子值，以设定新的对象"""
@@ -2756,18 +2969,15 @@
             fac1 = fac1 * i
         new_pure = pure_fall()
         new_pure.monthly_factors = fac1
         return new_pure
 
     def __sub__(self, selfa):
         """返回对象，如需表格，请调用对象"""
-        if is_notebook():
-            tqdm.tqdm_notebook().pandas()
-        else:
-            tqdm.tqdm.pandas()
+        tqdm.auto.tqdm.pandas()
         if not isinstance(selfa, Iterable):
             if not STATES["NO_LOG"]:
                 logger.warning(f"{selfa} is changed into Iterable")
             selfa = (selfa,)
         fac_main = self.wide_to_long(self.monthly_factors, "fac")
         fac_helps = [i.monthly_factors for i in selfa]
         help_names = ["help" + str(i) for i in range(1, (len(fac_helps) + 1))]
@@ -2847,112 +3057,115 @@
 
 class pure_fall_frequent(object):
     """对单只股票单日进行操作"""
 
     def __init__(
         self,
         factor_file: str,
+        project: str = None,
         startdate: int = None,
         enddate: int = None,
+        questdb_host: str = "127.0.0.1",
         kind: str = "stock",
         clickhouse: bool = 0,
         questdb: bool = 0,
+        questdb_web_port: str = "9001",
         ignore_history_in_questdb: bool = 0,
         groupby_target: list = ["date", "code"],
     ) -> None:
         """基于clickhouse的分钟数据，计算因子值，每天的因子值只用到当日的数据
 
         Parameters
         ----------
         factor_file : str
-            用于保存因子值的文件名，需为feather文件，以'.feather'结尾
+            用于保存因子值的文件名，需为parquet文件，以'.parquet'结尾
+        project : str, optional
+            该因子所属项目，即子文件夹名称, by default None
         startdate : int, optional
             起始时间，形如20121231，为开区间, by default None
         enddate : int, optional
             截止时间，形如20220814，为闭区间，为空则计算到最近数据, by default None
+        questdb_host: str, optional
+            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
         kind : str, optional
             类型为股票还是指数，指数为'index', by default "stock"
         clickhouse : bool, optional
             使用clickhouse作为数据源，如果postgresql与本参数都为0，将依然从clickhouse中读取, by default 0
         questdb : bool, optional
             使用questdb作为数据源, by default 0
+        questdb_web_port : str, optional
+            questdb的web_port, by default '9001'
         ignore_history_in_questdb : bool, optional
             打断后重新从头计算，清除在questdb中的记录
         groupby_target: list, optional
             groupby计算时，分组的依据，使用此参数时，自定义函数的部分，如果指定按照['date']分组groupby计算，
             则返回时，应当返回一个两列的dataframe，第一列为股票代码，第二列为为因子值, by default ['date','code']
         """
         homeplace = HomePlace()
         self.kind = kind
         self.groupby_target = groupby_target
         if clickhouse == 0 and questdb == 0:
             clickhouse = 1
         self.clickhouse = clickhouse
         self.questdb = questdb
+        self.questdb_web_port = questdb_web_port
         if clickhouse == 1:
             # 连接clickhouse
             self.chc = ClickHouseClient("minute_data")
         elif questdb == 1:
-            self.chc = Questdb()
+            self.chc = Questdb(host=questdb_host, web_port=questdb_web_port)
         # 将计算到一半的因子，存入questdb中，避免中途被打断后重新计算，表名即为因子文件名的汉语拼音
         pinyin = Pinyin()
         self.factor_file_pinyin = pinyin.get_pinyin(
-            factor_file.replace(".feather", ""), ""
+            factor_file.replace(".parquet", ""), ""
         )
-        self.factor_steps = Questdb()
+        self.factor_steps = Questdb(host=questdb_host, web_port=questdb_web_port)
+        if project is not None:
+            if not os.path.exists(homeplace.factor_data_file + project):
+                os.makedirs(homeplace.factor_data_file + project)
+            else:
+                logger.info(f"当前正在{project}项目中……")
+        else:
+            logger.warning("当前因子不属于任何项目，这将造成因子数据文件夹的混乱，不便于管理，建议指定一个项目名称")
         # 完整的因子文件路径
-        factor_file = homeplace.factor_data_file + factor_file
+        if project is not None:
+            factor_file = homeplace.factor_data_file + project + "/" + factor_file
+        else:
+            factor_file = homeplace.factor_data_file + factor_file
         self.factor_file = factor_file
         # 读入之前的因子
         if os.path.exists(factor_file):
-            factor_old = pd.read_feather(self.factor_file)
-            factor_old.columns = ["date"] + list(factor_old.columns)[1:]
-            factor_old = factor_old.drop_duplicates(subset=["date"])
-            factor_old = factor_old.set_index("date")
+            factor_old = drop_duplicates_index(pd.read_parquet(self.factor_file))
             self.factor_old = factor_old
             # 已经算好的日子
             dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
             self.dates_old = dates_old
         elif (not ignore_history_in_questdb) and self.factor_file_pinyin in list(
             self.factor_steps.get_data("show tables").table
         ):
             logger.info(
                 f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，现在将读取上次的数据，继续计算"
             )
-            factor_old = self.factor_steps.get_data(
-                f"select * from {self.factor_file_pinyin}"
-            )
-            # 判断一下每天是否生成多个数据，单个数据就以float形式存储，多个数据以list形式存储
-            if "f0" in list(factor_old.columns):
-                factor_old = factor_old[factor_old.f0 != "date"]
-                factor_old.columns = ["date", "code", "fac"]
-                try:
-                    factor_old.fac = factor_old.fac.apply(
-                        lambda x: [float(i) for i in x[1:-1].split(" ") if i != ""]
-                    )
-                except Exception:
-                    factor_old.fac = factor_old.fac.apply(
-                        lambda x: [float(i) for i in x[1:-1].split(", ") if i != ""]
-                    )
+            factor_old = self.factor_steps.get_data_with_tuple(
+                f"select * from '{self.factor_file_pinyin}'"
+            ).drop_duplicates(subset=["date", "code"])
             factor_old = factor_old.pivot(index="date", columns="code", values="fac")
-            factor_old.index = pd.to_datetime(factor_old.index)
             factor_old = factor_old.sort_index()
-            factor_old = drop_duplicates_index(factor_old)
             self.factor_old = factor_old
             # 已经算好的日子
             dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
             self.dates_old = dates_old
         elif ignore_history_in_questdb and self.factor_file_pinyin in list(
             self.factor_steps.get_data("show tables").table
         ):
             logger.info(
                 f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，但您选择重新计算，所以正在删除原来的数据，从头计算"
             )
             factor_old = self.factor_steps.do_order(
-                f"drop table {self.factor_file_pinyin}"
+                f"drop table '{self.factor_file_pinyin}'"
             )
             self.factor_old = None
             self.dates_old = []
             logger.info("删除完毕，正在重新计算")
         else:
             self.factor_old = None
             self.dates_old = []
@@ -3002,14 +3215,25 @@
         Returns
         -------
         `pd.DataFrame`
             经运算产生的因子值
         """
         return self.factor.copy()
 
+    def forward_dates(self, dates, many_days):
+        dates_index = [self.dates_all.index(i) for i in dates]
+
+        def value(x, a):
+            if x >= 0:
+                return a[x]
+            else:
+                return None
+
+        return [value(i - many_days, self.dates_all) for i in dates_index]
+
     def select_one_calculate(
         self,
         date: pd.Timestamp,
         func: Callable,
         fields: str = "*",
         show_time: bool = 0,
     ) -> None:
@@ -3035,162 +3259,174 @@
             df = df.sort_values(["date", "num"])
         df = df.groupby(self.groupby_target).apply(the_func)
         if self.groupby_target == ["date", "code"]:
             df = df.to_frame("fac").reset_index()
             df.columns = ["date", "code", "fac"]
         else:
             df = df.reset_index()
-        df = df.pivot(columns="code", index="date", values="fac")
-        df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-        return df
+        if (df is not None) and (df.shape[0] > 0):
+            df = df.pivot(columns="code", index="date", values="fac")
+            df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+            to_save = df.stack().reset_index()
+            to_save.columns = ["date", "code", "fac"]
+            self.factor_steps.write_via_df(
+                to_save, self.factor_file_pinyin, tuple_col="fac"
+            )
+            return df
 
     def select_many_calculate(
         self,
-        dates: list[pd.Timestamp],
+        dates: List[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
-        tqdm_inside: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
     ) -> None:
         the_func = partial(func)
-        dates = [int(datetime.datetime.strftime(i, "%Y%m%d")) for i in dates]
-        # 将需要更新的日子分块，每200天一组，一起运算
-        dates_new_len = len(dates)
-        cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
-        if cut_points[-1] == cut_points[-2]:
-            cut_points = cut_points[:-1]
-        cut_first = cut_points[0]
-        cuts = tuple(zip(cut_points[:-1], cut_points[1:]))
-        print(f"共{len(cuts)}段")
         factor_new = []
-        df_first = self.select_one_calculate(
-            date=dates[0],
-            func=func,
-            fields=fields,
-            show_time=show_time,
-        )
-        factor_new.append(df_first)
-        to_save = df_first.stack().reset_index()
-        to_save.columns = ["date", "code", "fac"]
-        self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
-
-        if tqdm_inside == 1:
-            # 开始计算因子值
-            for date1, date2 in cuts:
+        dates = [int(datetime.datetime.strftime(i, "%Y%m%d")) for i in dates]
+        if many_days == 1:
+            # 将需要更新的日子分块，每200天一组，一起运算
+            dates_new_len = len(dates)
+            cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
+            if cut_points[-1] == cut_points[-2]:
+                cut_points = cut_points[:-1]
+            cuts = tuple(zip(cut_points[:-many_days], cut_points[many_days:]))
+            df_first = self.select_one_calculate(
+                date=dates[0],
+                func=func,
+                fields=fields,
+                show_time=show_time,
+            )
+            factor_new.append(df_first)
+
+            def cal_one(date1, date2):
                 if self.clickhouse == 1:
                     sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
                 else:
-                    sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]}"
+                    sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]} order by code,date,num"
                 if show_time:
                     df = self.chc.get_data_show_time(sql_order)
                 else:
                     df = self.chc.get_data(sql_order)
                 if self.clickhouse == 1:
                     df = ((df.set_index("code")) / 100).reset_index()
                 else:
                     df.num = df.num.astype(int)
                     df.date = df.date.astype(int)
                     df = df.sort_values(["date", "num"])
-                if is_notebook():
-                    tqdm.tqdm_notebook().pandas()
+                df = df.groupby(self.groupby_target).apply(the_func)
+                if self.groupby_target == ["date", "code"]:
+                    df = df.to_frame("fac").reset_index()
+                    df.columns = ["date", "code", "fac"]
                 else:
-                    tqdm.tqdm.pandas()
-                df = df.groupby(self.groupby_target).progress_apply(the_func)
-                df = df.to_frame("fac").reset_index()
-                df.columns = ["date", "code", "fac"]
+                    df = df.reset_index()
                 df = df.pivot(columns="code", index="date", values="fac")
                 df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-                factor_new.append(df)
                 to_save = df.stack().reset_index()
                 to_save.columns = ["date", "code", "fac"]
-                self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
-        else:
-            if is_notebook():
-                # 开始计算因子值
-                for date1, date2 in tqdm.tqdm_notebook(cuts, desc="不知乘月几人归，落月摇情满江树。"):
-                    if self.clickhouse == 1:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
-                    else:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1]} and date<={dates[date2]} order by code,date,num"
-                    if show_time:
-                        df = self.chc.get_data_show_time(sql_order)
-                    else:
-                        df = self.chc.get_data(sql_order)
-                    if self.clickhouse == 1:
-                        df = ((df.set_index("code")) / 100).reset_index()
-                    df = df.groupby(self.groupby_target).apply(the_func)
-                    if self.groupby_target == ["date", "code"]:
-                        df = df.to_frame("fac").reset_index()
-                        df.columns = ["date", "code", "fac"]
-                    else:
-                        df = df.reset_index()
-                    df = df.pivot(columns="code", index="date", values="fac")
-                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-                    factor_new.append(df)
-                    to_save = df.stack().reset_index()
-                    to_save.columns = ["date", "code", "fac"]
-                    self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
+                self.factor_steps.write_via_df(
+                    to_save, self.factor_file_pinyin, tuple_col="fac"
+                )
+                return df
+
+            if n_jobs > 1:
+                with WorkerPool(n_jobs=n_jobs) as pool:
+                    factor_new_more = pool.map(cal_one, cuts, progress_bar=True)
+                factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
-                for date1, date2 in tqdm.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
+                for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
+                    df = cal_one(date1, date2)
+                    factor_new.append(df)
+        else:
+
+            def cal_two(date1, date2):
+                if date1 is not None:
                     if self.clickhouse == 1:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{date1*100} and date<={date2*100} order by code,date,num"
                     else:
-                        sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]}"
+                        sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{date1} and cast(date as int)<={date2} order by code,date,num"
                     if show_time:
                         df = self.chc.get_data_show_time(sql_order)
                     else:
                         df = self.chc.get_data(sql_order)
                     if self.clickhouse == 1:
                         df = ((df.set_index("code")) / 100).reset_index()
                     else:
                         df.num = df.num.astype(int)
                         df.date = df.date.astype(int)
                         df = df.sort_values(["date", "num"])
-                    df = df.groupby(self.groupby_target).apply(the_func)
-                    if self.groupby_target == ["date", "code"]:
-                        df = df.to_frame("fac").reset_index()
-                        df.columns = ["date", "code", "fac"]
+                    if self.groupby_target == [
+                        "date",
+                        "code",
+                    ] or self.groupby_target == ["code"]:
+                        df = df.groupby(["code"]).apply(the_func).reset_index()
                     else:
-                        df = df.reset_index()
+                        df = the_func(df)
+                    df = df.assign(date=date2)
+                    df.columns = ["code", "fac", "date"]
                     df = df.pivot(columns="code", index="date", values="fac")
                     df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-                    factor_new.append(df)
                     to_save = df.stack().reset_index()
                     to_save.columns = ["date", "code", "fac"]
-                    self.factor_steps.write_via_csv(to_save, self.factor_file_pinyin)
-        factor_new = pd.concat(factor_new)
-        return factor_new
+                    self.factor_steps.write_via_df(
+                        to_save, self.factor_file_pinyin, tuple_col="fac"
+                    )
+                    return df
+
+            pairs = self.forward_dates(dates, many_days=many_days)
+            cuts2 = tuple(zip(pairs, dates))
+            if n_jobs > 1:
+                with WorkerPool(n_jobs=n_jobs) as pool:
+                    factor_new_more = pool.map(cal_two, cuts2, progress_bar=True)
+                factor_new = factor_new + factor_new_more
+            else:
+                # 开始计算因子值
+                for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
+                    df = cal_two(date1, date2)
+                    factor_new.append(df)
+
+        if len(factor_new) > 0:
+            factor_new = pd.concat(factor_new)
+            return factor_new
+        else:
+            return None
 
     def select_any_calculate(
         self,
-        dates: list[pd.Timestamp],
+        dates: List[pd.Timestamp],
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
-        tqdm_inside: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
     ) -> None:
-        if len(dates) == 1:
+        if len(dates) == 1 and many_days == 1:
             res = self.select_one_calculate(
                 dates[0],
                 func=func,
                 fields=fields,
                 show_time=show_time,
             )
         else:
             res = self.select_many_calculate(
                 dates=dates,
                 func=func,
                 fields=fields,
                 chunksize=chunksize,
                 show_time=show_time,
-                tqdm_inside=tqdm_inside,
+                many_days=many_days,
+                n_jobs=n_jobs,
             )
+        if res is not None:
+            self.factor_new.append(res)
         return res
 
     @staticmethod
     def for_cross_via_str(func):
         """返回值为两层的list，每一个里层的小list为单个股票在这一天的返回值
         例如
         ```python
@@ -3224,31 +3460,45 @@
                 )
         ```
         上例中，每个股票一天返回两个因子值，每个pd.Series对应一个因子值
         """
 
         def full_run(df, *args, **kwargs):
             res = func(df, *args, **kwargs)
-            res = pd.concat(res, axis=1)
-            res.columns = [f"fac{i}" for i in range(len(res.columns))]
-            res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
-            res = res[["fac"]].reset_index()
-            res.columns = ["code", "fac"]
-            return res
+            if isinstance(res, pd.Series):
+                res = res.reset_index()
+                res.columns = ["code", "fac"]
+                return res
+            elif isinstance(res, pd.DataFrame):
+                res.columns = [f"fac{i}" for i in range(len(res.columns))]
+                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+                res = res[["fac"]].reset_index()
+                res.columns = ["code", "fac"]
+                return res
+            elif res is None:
+                ...
+            else:
+                res = pd.concat(res, axis=1)
+                res.columns = [f"fac{i}" for i in range(len(res.columns))]
+                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+                res = res[["fac"]].reset_index()
+                res.columns = ["code", "fac"]
+                return res
 
         return full_run
 
     @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
     def get_daily_factors(
         self,
         func: Callable,
         fields: str = "*",
         chunksize: int = 10,
         show_time: bool = 0,
-        tqdm_inside: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
     ) -> None:
         """每次抽取chunksize天的截面上全部股票的分钟数据
         对每天的股票的数据计算因子值
 
         Parameters
         ----------
         func : Callable
@@ -3256,292 +3506,74 @@
         fields : str, optional
             股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
             提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
         chunksize : int, optional
             每次读取的截面上的天数, by default 10
         show_time : bool, optional
             展示每次读取数据所需要的时间, by default 0
-        tqdm_inside : bool, optional
-            将进度条加在内部，而非外部，建议仅chunksize较大时使用, by default 0
+        many_days : int, optional
+            计算某天的因子值时，需要使用之前多少天的数据
+        n_jobs : int, optional
+            并行数量, by default 1
         """
         if len(self.dates_new) > 0:
             for interval in self.dates_new_intervals:
                 df = self.select_any_calculate(
                     dates=interval,
                     func=func,
                     fields=fields,
                     chunksize=chunksize,
                     show_time=show_time,
-                    tqdm_inside=tqdm_inside,
+                    many_days=many_days,
+                    n_jobs=n_jobs,
                 )
-                self.factor_new.append(df)
-            self.factor_new = pd.concat(self.factor_new)
-            # 拼接新的和旧的
-            self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
-            self.factor = self.factor.dropna(how="all")
-            self.factor = self.factor.reset_index()
-            self.factor = self.factor.rename(
-                columns={list(self.factor.columns)[0]: "date"}
-            )
-            self.factor = self.factor.drop_duplicates(subset=["date"], keep="first")
-            self.factor = self.factor.set_index("date")
-            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
-            # 存入本地
-            self.factor.reset_index().to_feather(self.factor_file)
-            logger.info(f"截止到{new_end_date}的因子值计算完了")
-            # 删除存储在questdb的中途备份数据
-            self.factor_steps.do_order(f"drop table {self.factor_file_pinyin}")
-            logger.info("备份在questdb的表格已删除")
-
-        else:
-            self.factor = self.factor_old
-            self.factor = self.factor.reset_index()
-            self.factor = self.factor.rename(
-                columns={list(self.factor.columns)[0]: "date"}
-            )
-            self.factor = self.factor.drop_duplicates(subset=["date"], keep="first")
-            self.factor = self.factor.set_index("date")
-            # 存入本地
-            self.factor.reset_index().to_feather(self.factor_file)
-            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
-            logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
-
+            if len(self.factor_new)>0:
+                self.factor_new = pd.concat(self.factor_new)
+                # 拼接新的和旧的
+                self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
+                self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
+                new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+                # 存入本地
+                self.factor.to_parquet(self.factor_file)
+                logger.info(f"截止到{new_end_date}的因子值计算完了")
+                # 删除存储在questdb的中途备份数据
+                try:
+                    self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+                    logger.info("备份在questdb的表格已删除")
+                except Exception:
+                    logger.warning("删除questdb中表格时，存在某个未知错误，请当心")
+            else:
+                logger.warning('由于某种原因，更新的因子值计算失败，建议检查🤒')
+                # 拼接新的和旧的
+                self.factor = pd.concat([self.factor_old]).sort_index()
+                self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
 
-class pure_fall_flexible(object):
-    def __init__(
-        self,
-        factor_file: str,
-        startdate: int = None,
-        enddate: int = None,
-        kind: str = "stock",
-        clickhouse: bool = 0,
-        questdb: bool = 0,
-    ) -> None:
-        """基于clickhouse的分钟数据，计算因子值，每天的因子值用到多日的数据，或者用到截面的数据
-        对一段时间的截面数据进行操作，在get_daily_factors的func函数中
-        请写入df=df.groupby([xxx]).apply(fff)之类的语句
-        然后单独定义一个函数，作为要apply的fff，可以在apply上加进度条
 
-        Parameters
-        ----------
-        factor_file : str
-            用于存储因子的文件名称，请以'.feather'结尾
-        startdate : int, optional
-            计算因子的起始日期，形如20220816, by default None
-        enddate : int, optional
-            计算因子的终止日期，形如20220816, by default None
-        kind : str, optional
-            指定计算股票还是指数，指数则为'index', by default "stock"
-        clickhouse : bool, optional
-            使用clickhouse作为数据源，如果postgresql与本参数都为0，将依然从clickhouse中读取, by default 0
-        questdb : bool, optional
-            使用questdb作为数据源, by default 0
-        """
-        homeplace = HomePlace()
-        self.kind = kind
-        if clickhouse == 0 and questdb == 0:
-            clickhouse = 1
-        self.clickhouse = clickhouse
-        self.questdb = questdb
-        if clickhouse == 1:
-            # 连接clickhouse
-            self.chc = ClickHouseClient("minute_data")
-        elif questdb:
-            self.chc = Questdb()
-        # 完整的因子文件路径
-        factor_file = homeplace.factor_data_file + factor_file
-        self.factor_file = factor_file
-        # 读入之前的因子
-        if os.path.exists(factor_file):
-            factor_old = pd.read_feather(self.factor_file)
-            factor_old.columns = ["date"] + list(factor_old.columns)[1:]
-            factor_old = factor_old.drop_duplicates(subset=["date"])
-            factor_old = factor_old.set_index("date")
-            self.factor_old = factor_old
-            # 已经算好的日子
-            dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
-            self.dates_old = dates_old
-        else:
-            self.factor_old = None
-            self.dates_old = []
-            logger.info("这个因子以前没有，正在重新计算")
-        # 读取当前所有的日子
-        dates_all = self.chc.show_all_dates(f"minute_data_{kind}")
-        if startdate is None:
-            ...
-        else:
-            dates_all = [i for i in dates_all if i >= startdate]
-        if enddate is None:
-            ...
         else:
-            dates_all = [i for i in dates_all if i <= enddate]
-        self.dates_all = dates_all
-        # 需要新补充的日子
-        self.dates_new = sorted([i for i in dates_all if i not in dates_old])
-
-    def __call__(self) -> pd.DataFrame:
-        """直接返回因子值的pd.DataFrame
-
-        Returns
-        -------
-        `pd.DataFrame`
-            计算出的因子值
-        """
-        return self.factor.copy()
-
-    @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
-    def get_daily_factors(
-        self,
-        func: Callable,
-        fields: str = "*",
-        chunksize: int = 250,
-        show_time: bool = 0,
-        tqdm_inside: bool = 0,
-    ) -> None:
-        """每次抽取chunksize天的截面上全部股票的分钟数据
-        依照定义的函数计算因子值
-
-        Parameters
-        ----------
-        func : Callable
-            用于计算因子值的函数
-        fields : str, optional
-            股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
-            提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
-        chunksize : int, optional
-            每次读取的截面上的天数, by default 10
-        show_time : bool, optional
-            展示每次读取数据所需要的时间, by default 0
-        tqdm_inside : bool, optional
-            将进度条加在内部，而非外部，建议仅chunksize较大时使用, by default 0
-        """
-        the_func = partial(func)
-        # 将需要更新的日子分块，每200天一组，一起运算
-        dates_new_len = len(self.dates_new)
-        if dates_new_len > 0:
-            cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
-            if cut_points[-1] == cut_points[-2]:
-                cut_points = cut_points[:-1]
-            self.cut_points = cut_points
-            self.factor_new = []
-            # 开始计算因子值
-            if tqdm_inside:
-                # 开始计算因子值
-                for date1, date2 in cut_points:
-                    if self.clickhouse == 1:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]*100} and date<={self.dates_new[date2]*100} order by code,date,num"
-                    else:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]} and date<={self.dates_new[date2]}"
-                    if show_time:
-                        df = self.chc.get_data_show_time(sql_order)
-                    else:
-                        df = self.chc.get_data(sql_order)
-                    if self.clickhouse == 1:
-                        df = ((df.set_index("code")) / 100).reset_index()
-                    if is_notebook():
-                        tqdm.tqdm_notebook().pandas()
-                    else:
-                        tqdm.tqdm.pandas()
-                    df = the_func(df)
-                    if isinstance(df, pd.Series):
-                        df = df.reset_index()
-                    df.columns = ["date", "code", "fac"]
-                    df = df.pivot(columns="code", index="date", values="fac")
-                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-                    self.factor_new.append(df)
-            else:
-                # 开始计算因子值
-                for date1, date2 in tqdm.tqdm(cut_points, desc="不知乘月几人归，落月摇情满江树。"):
-                    if self.clickhouse == 1:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]*100} and date<={self.dates_new[date2]*100} order by code,date,num"
-                    else:
-                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{self.dates_new[date1]} and date<={self.dates_new[date2]} order by code,date,num"
-                    if show_time:
-                        df = self.chc.get_data_show_time(sql_order)
-                    else:
-                        df = self.chc.get_data(sql_order)
-                    if self.clickhouse == 1:
-                        df = ((df.set_index("code")) / 100).reset_index()
-                    df = the_func(df)
-                    if isinstance(df, pd.Series):
-                        df = df.reset_index()
-                    df.columns = ["date", "code", "fac"]
-                    df = df.pivot(columns="code", index="date", values="fac")
-                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-                    self.factor_new.append(df)
-            self.factor_new = pd.concat(self.factor_new)
-            # 拼接新的和旧的
-            self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
-            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
-            # 存入本地
-            self.factor.reset_index().to_feather(self.factor_file)
-            logger.info(f"截止到{new_end_date}的因子值计算完了")
-        elif dates_new_len == 1:
-            print("共1天")
-            if tqdm_inside:
-                # 开始计算因子值
-                if self.clickhouse == 1:
-                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]*100} order by code,date,num"
-                else:
-                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]} order by code,date,num"
-                if show_time:
-                    df = self.chc.get_data_show_time(sql_order)
-                else:
-                    df = self.chc.get_data(sql_order)
-                if self.clickhouse == 1:
-                    df = ((df.set_index("code")) / 100).reset_index()
-                tqdm.tqdm.pandas()
-                df = the_func(df)
-                if isinstance(df, pd.Series):
-                    df = df.reset_index()
-                df.columns = ["date", "code", "fac"]
-                df = df.pivot(columns="code", index="date", values="fac")
-                df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-            else:
-                # 开始计算因子值
-                if self.clickhouse == 1:
-                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]*100} order by code,date,num"
-                else:
-                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date={self.dates_new[0]} order by code,date,num"
-                if show_time:
-                    df = self.chc.get_data_show_time(sql_order)
-                else:
-                    df = self.chc.get_data(sql_order)
-                if self.clickhouse == 1:
-                    df = ((df.set_index("code")) / 100).reset_index()
-                df = the_func(df)
-                if isinstance(df, pd.Series):
-                    df = df.reset_index()
-                df.columns = ["date", "code", "fac"]
-                df = df.pivot(columns="code", index="date", values="fac")
-                df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
-                self.factor_new.append(df)
-            self.factor_new = df
-            # 拼接新的和旧的
-            self.factor = (
-                pd.concat([self.factor_old, self.factor_new])
-                .sort_index()
-                .drop_duplicates()
-            )
-            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            self.factor = drop_duplicates_index(self.factor_old)
             # 存入本地
-            self.factor.reset_index().to_feather(self.factor_file)
-            logger.info(f"补充{self.dates_new[0]}截止到{new_end_date}的因子值计算完了")
-        else:
-            self.factor = self.factor_old
+            self.factor.to_parquet(self.factor_file)
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
 
+    def drop_table(self):
+        """直接删除存储在questdb中的暂存数据"""
+        try:
+            self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+            logger.success(f"暂存在questdb中的数据表格'{self.factor_file_pinyin}'已经删除")
+        except Exception:
+            logger.warning(f"您要删除的表格'{self.factor_file_pinyin}'已经不存在了，请检查")
+
 
 class pure_coldwinter(object):
     # DONE: 可以自由添加其他要剔除的因子，或者替换某些要剔除的因子
 
     def __init__(
         self,
-        facs_dict: dict = None,
+        facs_dict: Dict = None,
         momentum: bool = 1,
         earningsyield: bool = 1,
         growth: bool = 1,
         liquidity: bool = 1,
         size: bool = 1,
         leverage: bool = 1,
         beta: bool = 1,
@@ -3549,15 +3581,15 @@
         residualvolatility: bool = 1,
         booktoprice: bool = 1,
     ) -> None:
         """读入10种常用风格因子，并可以额外加入其他因子
 
         Parameters
         ----------
-        facs_dict : dict, optional
+        facs_dict : Dict, optional
             额外加入的因子，名字为key，因子矩阵为value，形如`{'反转': ret20, '换手': tr20}`, by default None
         momentum : bool, optional
             是否删去动量因子, by default 1
         earningsyield : bool, optional
             是否删去盈利因子, by default 1
         growth : bool, optional
             是否删去成长因子, by default 1
@@ -3575,21 +3607,19 @@
             是否删去残差波动率因子, by default 1
         booktoprice : bool, optional
             是否删去账面市值比因子, by default 1
         """
         self.homeplace = HomePlace()
         # barra因子数据
         styles = os.listdir(self.homeplace.barra_data_file)
-        styles = [i for i in styles if i.endswith(".feather")]
+        styles = [i for i in styles if i.endswith(".parquet")]
         barras = {}
         for s in styles:
             k = s.split(".")[0]
-            v = pd.read_feather(self.homeplace.barra_data_file + s)
-            v.columns = ["date"] + list(v.columns)[1:]
-            v = v.set_index("date")
+            v = pd.read_parquet(self.homeplace.barra_data_file + s)
             barras[k] = v
         rename_dict = {
             "fac": "因子自身",
             "size": "市值",
             "nonlinearsize": "非线性市值",
             "booktoprice": "估值",
             "earningsyield": "盈利",
@@ -3685,15 +3715,15 @@
             [self.factors] + list(self.barras.values()), axis=1
         ).dropna()
 
     # DONE: 修改风格因子展示顺序至报告的顺序
     def get_corr(self):
         """计算每一期的相关系数，再求平均值"""
         self.corr_by_step = self.corr_pri.groupby(["date"]).apply(
-            lambda x: x.corr().head(1)
+            lambda x: x.rank().corr().head(1)
         )
         self.__corr = self.corr_by_step.mean()
         self.__corr = self.__corr.rename(index=self.rename_dict)
         self.__corr = self.__corr.to_frame("相关系数").T
 
         self.__corr = self.__corr[self.sort_names]
         self.__corr = self.__corr.T
@@ -3736,21 +3766,22 @@
         self.get_monthly_barras_industrys()
         self.get_wide_barras_industrys()
         self.get_corr_pri_ols_pri()
         self.get_corr()
         self.get_snow_fac()
 
 
+@do_on_dfs
 class pure_snowtrain(object):
     """直接返回纯净因子"""
 
     def __init__(
         self,
         factors: pd.DataFrame,
-        facs_dict: dict = None,
+        facs_dict: Dict = None,
         momentum: bool = 1,
         earningsyield: bool = 1,
         growth: bool = 1,
         liquidity: bool = 1,
         size: bool = 1,
         leverage: bool = 1,
         beta: bool = 1,
@@ -3760,36 +3791,36 @@
     ) -> None:
         """计算因子值与10种常用风格因子之间的相关性，并进行纯净化，可以额外加入其他因子
 
         Parameters
         ----------
         factors : pd.DataFrame
             要考察的因子值，index为时间，columns为股票代码，values为因子值
-        facs_dict : dict, optional
-            _description_, by default None
+        facs_dict : Dict, optional
+            额外加入的因子，名字为key，因子矩阵为value，形如`{'反转': ret20, '换手': tr20}`, by default None
         momentum : bool, optional
-            _description_, by default 1
+            是否删去动量因子, by default 1
         earningsyield : bool, optional
-            _description_, by default 1
+            是否删去盈利因子, by default 1
         growth : bool, optional
-            _description_, by default 1
+            是否删去成长因子, by default 1
         liquidity : bool, optional
-            _description_, by default 1
+            是否删去流动性因子, by default 1
         size : bool, optional
-            _description_, by default 1
+            是否删去规模因子, by default 1
         leverage : bool, optional
-            _description_, by default 1
+            是否删去杠杆因子, by default 1
         beta : bool, optional
-            _description_, by default 1
+            是否删去贝塔因子, by default 1
         nonlinearsize : bool, optional
-            _description_, by default 1
+            是否删去非线性市值因子, by default 1
         residualvolatility : bool, optional
-            _description_, by default 1
+            是否删去残差波动率因子, by default 1
         booktoprice : bool, optional
-            _description_, by default 1
+            是否删去账面市值比因子, by default 1
         """
         self.winter = pure_coldwinter(
             facs_dict=facs_dict,
             momentum=momentum,
             earningsyield=earningsyield,
             growth=growth,
             liquidity=liquidity,
@@ -3810,23 +3841,34 @@
         Returns
         -------
         pd.DataFrame
             纯净化之后的因子值
         """
         return self.winter.snow_fac.copy()
 
+    def show_corr(self) -> pd.DataFrame:
+        """展示因子与barra风格因子的相关系数
+
+        Returns
+        -------
+        pd.DataFrame
+            相关系数表格
+        """
+        return self.corr.T.applymap(lambda x: to_percent(x))
+
 
 class pure_newyear(object):
     """转为生成25分组和百分组的收益矩阵而封装"""
 
     def __init__(
         self,
         facx: pd.DataFrame,
         facy: pd.DataFrame,
         group_num_single: int,
+        trade_cost_double_side: float = 0,
         namex: str = "主",
         namey: str = "次",
     ) -> None:
         """条件双变量排序法，先对所有股票，依照因子facx进行排序
         然后在每个组内，依照facy进行排序，最后统计各个组内的平均收益率
 
         Parameters
@@ -3835,27 +3877,33 @@
             首先进行排序的因子，通常为控制变量，相当于正交化中的自变量
             index为时间，columns为股票代码，values为因子值
         facy : pd.DataFrame
             在facx的各个组内，依照facy进行排序，为主要要研究的因子
             index为时间，columns为股票代码，values为因子值
         group_num_single : int
             单个因子分成几组，通常为5或10
+        trade_cost_double_side : float, optional
+            交易的双边手续费率, by default 0
         namex : str, optional
             facx这一因子的名字, by default "主"
         namey : str, optional
             facy这一因子的名字, by default "次"
         """
         homex = pure_fallmount(facx)
         homey = pure_fallmount(facy)
         if group_num_single == 5:
             homexy = homex > homey
         elif group_num_single == 10:
             homexy = homex >> homey
         shen = pure_moonnight(
-            homexy(), group_num_single**2, plt_plot=False, print_comments=False
+            homexy(),
+            group_num_single**2,
+            trade_cost_double_side=trade_cost_double_side,
+            plt_plot=False,
+            print_comments=False,
         )
         sq = shen.shen.square_rets.copy()
         sq.index = [namex + str(i) for i in list(sq.index)]
         sq.columns = [namey + str(i) for i in list(sq.columns)]
         self.square_rets = sq
 
     def __call__(self) -> pd.DataFrame:
@@ -3865,290 +3913,528 @@
         -------
         `pd.DataFrame`
             每个组的年化收益率
         """
         return self.square_rets.copy()
 
 
-class pure_dawn(object):
-    """
-    因子切割论的母框架，可以对两个因子进行类似于因子切割的操作
-    可用于派生任何"以两个因子生成一个因子"的子类
-    使用举例
-    cut函数里，必须带有输入变量df,df有两个columns，一个名为'fac1'，一个名为'fac2'，df是最近一个回看期内的数据
-    ```python
-    class Cut(pure_dawn):
-
-    def cut(self,df):
-        df=df.sort_values('fac1')
-        df=df.assign(fac3=df.fac1*df.fac2)
-        ret0=df.fac2.iloc[:4].mean()
-        ret1=df.fac2.iloc[4:8].mean()
-        ret2=df.fac2.iloc[8:12].mean()
-        ret3=df.fac2.iloc[12:16].mean()
-        ret4=df.fac2.iloc[16:].mean()
-        aret0=df.fac3.iloc[:4].mean()
-        aret1=df.fac3.iloc[4:8].mean()
-        aret2=df.fac3.iloc[8:12].mean()
-        aret3=df.fac3.iloc[12:16].mean()
-        aret4=df.fac3.iloc[16:].mean()
-        return ret0,ret1,ret2,ret3,ret4,aret0,aret1,aret2,aret3,aret4
-
-    cut=Cut(ct,ret_inday)
-    cut.run(cut.cut)
-
-    cut0=get_value(cut(),0)
-    cut1=get_value(cut(),1)
-    cut2=get_value(cut(),2)
-    cut3=get_value(cut(),3)
-    cut4=get_value(cut(),4)
-    ```
-    """
-
-    def __init__(self, fac1: pd.DataFrame, fac2: pd.DataFrame, *args: list) -> None:
-        """几个因子的操作，每个月操作一次
-
-        Parameters
-        ----------
-        fac1 : pd.DataFrame
-            因子值1，index为时间，columns为股票代码，values为因子值
-        fac2 : pd.DataFrame
-            因子2，index为时间，columns为股票代码，values为因子值
-        """
-        self.fac1 = fac1
-        self.fac1 = self.fac1.stack().reset_index()
-        self.fac1.columns = ["date", "code", "fac1"]
-        self.fac2 = fac2
-        self.fac2 = self.fac2.stack().reset_index()
-        self.fac2.columns = ["date", "code", "fac2"]
-        fac_all = pd.merge(self.fac1, self.fac2, on=["date", "code"])
-        for i, fac in enumerate(args):
-            fac = fac.stack().reset_index()
-            fac.columns = ["date", "code", f"fac{i+3}"]
-            fac_all = pd.merge(fac_all, fac, on=["date", "code"])
-        fac_all = fac_all.sort_values(["date", "code"])
-        self.fac = fac_all.copy()
-
-    def __call__(self) -> pd.DataFrame:
-        """返回最终月度因子值
-
-        Returns
-        -------
-        `pd.DataFrame`
-            最终因子值
-        """
-        return self.fac.copy()
-
-    def get_fac_long_and_tradedays(self):
-        """将两个因子的矩阵转化为长列表"""
-        self.tradedays = sorted(list(set(self.fac.date)))
-
-    def get_month_starts_and_ends(self, backsee=20):
-        """计算出每个月回看期间的起点日和终点日"""
-        self.month_ends = [
-            i
-            for i, j in zip(self.tradedays[:-1], self.tradedays[1:])
-            if i.month != j.month
-        ]
-        self.month_ends.append(self.tradedays[-1])
-        self.month_starts = [
-            self.find_begin(self.tradedays, i, backsee=backsee) for i in self.month_ends
-        ]
-        self.month_starts[0] = self.tradedays[0]
-
-    def find_begin(self, tradedays, end_day, backsee=20):
-        """找出回看若干天的开始日，默认为20"""
-        end_day_index = tradedays.index(end_day)
-        start_day_index = end_day_index - backsee + 1
-        start_day = tradedays[start_day_index]
-        return start_day
-
-    def make_monthly_factors_single_code(self, df, func):
-        """
-        对单一股票来计算月度因子
-        func为单月执行的函数，返回值应为月度因子，如一个float或一个list
-        df为一个股票的四列表，包含时间、代码、因子1和因子2
-        """
-        res = {}
-        for start, end in zip(self.month_starts, self.month_ends):
-            this_month = df[(df.date >= start) & (df.date <= end)]
-            res[end] = func(this_month)
-        dates = list(res.keys())
-        corrs = list(res.values())
-        part = pd.DataFrame({"date": dates, "corr": corrs})
-        return part
-
-    def get_monthly_factor(self, func):
-        """运行自己写的函数，获得月度因子"""
-        if is_notebook():
-            tqdm.tqdm_notebook().pandas()
-        else:
-            tqdm.tqdm.pandas(desc="when the dawn comes, tonight will be a memory too.")
-        self.fac = self.fac.groupby(["code"]).progress_apply(
-            lambda x: self.make_monthly_factors_single_code(x, func)
-        )
-        self.fac = (
-            self.fac.reset_index(level=1, drop=True)
-            .reset_index()
-            .set_index(["date", "code"])
-            .unstack()
-        )
-        self.fac.columns = [i[1] for i in list(self.fac.columns)]
-        self.fac = self.fac.resample("M").last()
-
-    @kk.desktop_sender(title="嘿，切割完成啦🛁")
-    def run(self, func: Callable, backsee: int = 20) -> None:
-        """执行计算的框架，产生因子值
-
-        Parameters
-        ----------
-        func : Callable
-            每个月要进行的操作
-        backsee : int, optional
-            回看期，即每个月月底对过去多少天进行计算, by default 20
-        """
-        self.get_fac_long_and_tradedays()
-        self.get_month_starts_and_ends(backsee=backsee)
-        self.get_monthly_factor(func)
-
-
+@do_on_dfs
 def follow_tests(
     fac: pd.DataFrame,
+    trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
+    index_member_value_weighted: bool = 1,
     comments_writer: pd.ExcelWriter = None,
     net_values_writer: pd.ExcelWriter = None,
     pos: bool = 0,
     neg: bool = 0,
     swindustry: bool = 0,
     zxindustry: bool = 0,
-    nums: list[int] = [3],
+    nums: List[int] = [3],
+    opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
 ):
     """因子完成全A测试后，进行的一些必要的后续测试，包括各个分组表现、相关系数与纯净化、3510的多空和多头、各个行业Rank IC、各个行业买3只超额表现
 
     Parameters
     ----------
     fac : pd.DataFrame
         要进行后续测试的因子值，index是时间，columns是股票代码，values是因子值
+    trade_cost_double_side : float, optional
+        交易的双边手续费率, by default 0
+    index_member_value_weighted : bool, optional
+        成分股多头采取流通市值加权
     comments_writer : pd.ExcelWriter, optional
         写入评价指标的excel, by default None
     net_values_writer : pd.ExcelWriter, optional
         写入净值序列的excel, by default None
     pos : bool, optional
         因子的方向为正, by default 0
     neg : bool, optional
         因子的方向为负, by default 0
     swindustry : bool, optional
         使用申万一级行业, by default 0
     zxindustry : bool, optional
         使用中信一级行业, by default 0
-    nums : list[int], optional
+    nums : List[int], optional
         各个行业买几只股票, by default [3]
+    opens_average_first_day : bool, optional
+        买入时使用第一天的平均价格, by default 0
+    total_cap : bool, optional
+        加权和行业市值中性化时使用总市值, by default 0
 
     Raises
     ------
     IOError
         如果未指定因子正负方向，将报错
     """
     if comments_writer is None:
-        from pure_ocean_breeze.legacy_version.v3p4.state.states import COMMENTS_WRITER
+        from pure_ocean_breeze.state.states import COMMENTS_WRITER
 
         comments_writer = COMMENTS_WRITER
     if net_values_writer is None:
-        from pure_ocean_breeze.legacy_version.v3p4.state.states import NET_VALUES_WRITER
+        from pure_ocean_breeze.state.states import NET_VALUES_WRITER
 
         net_values_writer = NET_VALUES_WRITER
 
-    shen = pure_moonnight(fac)
-    shen.comments_ten().to_excel(comments_writer, sheet_name="十分组")
+    shen = pure_moonnight(
+        fac,
+        opens_average_first_day=opens_average_first_day,
+    )
+    if (
+        shen.shen.group_net_values.group1.iloc[-1]
+        > shen.shen.group_net_values.group10.iloc[-1]
+    ):
+        neg = 1
+    else:
+        pos = 1
+    if comments_writer is not None:
+        shen.comments_ten().to_excel(comments_writer, sheet_name="十分组")
+    print(shen.comments_ten())
     """相关系数与纯净化"""
     pure_fac = pure_snowtrain(fac)
-    pure_fac.corr.to_excel(comments_writer, sheet_name="相关系数")
+    if comments_writer is not None:
+        pure_fac.corr.to_excel(comments_writer, sheet_name="相关系数")
+    print(pure_fac.corr)
     shen = pure_moonnight(
         pure_fac(),
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="纯净",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     """3510多空和多头"""
     # 300
     fi300 = daily_factor_on300500(fac, hs300=1)
     shen = pure_moonnight(
         fi300,
+        value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="300多空",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
-        make_relative_comments(shen.shen.group_rets.group10, hs300=1).to_excel(
-            comments_writer, sheet_name="300超额"
-        )
-        make_relative_comments_plot(shen.shen.group_rets.group10, hs300=1).to_excel(
-            net_values_writer, sheet_name="300超额"
-        )
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group10, hs300=1).to_excel(
+                comments_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group10
+                    - shen.shen.factor_turnover_rates.group10 * i,
+                    hs300=1,
+                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group10, hs300=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group10, hs300=1).to_excel(
+                net_values_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group10
+                    - shen.shen.factor_turnover_rates.group10 * i,
+                    hs300=1,
+                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group10, hs300=1)
     elif neg:
-        make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
-            comments_writer, sheet_name="300超额"
-        )
-        make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
-            net_values_writer, sheet_name="300超额"
-        )
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
+                comments_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    hs300=1,
+                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, hs300=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
+                net_values_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    hs300=1,
+                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1)
     else:
         raise IOError("请指定因子的方向是正是负🤒")
     # 500
     fi500 = daily_factor_on300500(fac, zz500=1)
     shen = pure_moonnight(
         fi500,
+        value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="500多空",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
-        make_relative_comments(shen.shen.group_rets.group10, zz500=1).to_excel(
-            comments_writer, sheet_name="500超额"
-        )
-        make_relative_comments_plot(shen.shen.group_rets.group10, zz500=1).to_excel(
-            net_values_writer, sheet_name="500超额"
-        )
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group10, zz500=1).to_excel(
+                comments_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group10
+                    - shen.shen.factor_turnover_rates.group10 * i,
+                    zz500=1,
+                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group10, zz500=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group10, zz500=1).to_excel(
+                net_values_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group10
+                    - shen.shen.factor_turnover_rates.group10 * i,
+                    zz500=1,
+                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group10, zz500=1)
     else:
-        make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
-            comments_writer, sheet_name="500超额"
-        )
-        make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
-            net_values_writer, sheet_name="500超额"
-        )
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
+                comments_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz500=1,
+                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, zz500=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
+                net_values_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz500=1,
+                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1)
     # 1000
     fi1000 = daily_factor_on300500(fac, zz1000=1)
     shen = pure_moonnight(
         fi1000,
+        value_weighted=index_member_value_weighted,
         comments_writer=comments_writer,
         net_values_writer=net_values_writer,
         sheetname="1000多空",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
     )
     if pos:
-        make_relative_comments(shen.shen.group_rets.group10, zz1000=1).to_excel(
-            comments_writer, sheet_name="1000超额"
-        )
-        make_relative_comments_plot(shen.shen.group_rets.group10, zz1000=1).to_excel(
-            net_values_writer, sheet_name="1000超额"
-        )
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group10, zz1000=1).to_excel(
+                comments_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group10
+                    - shen.shen.factor_turnover_rates.group10 * i,
+                    zz1000=1,
+                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group10, zz1000=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets.group10, zz1000=1
+            ).to_excel(net_values_writer, sheet_name="1000超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group10
+                    - shen.shen.factor_turnover_rates.group10 * i,
+                    zz1000=1,
+                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group10, zz1000=1)
     else:
-        make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
-            comments_writer, sheet_name="1000超额"
-        )
-        make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
-            net_values_writer, sheet_name="1000超额"
-        )
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
+                comments_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz1000=1,
+                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, zz1000=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
+                net_values_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz1000=1,
+                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1)
     # 各行业Rank IC
     rankics = rankic_test_on_industry(fac, comments_writer)
     # 买3只超额表现
     rets = long_test_on_industry(
         fac, nums, pos=pos, neg=neg, swindustry=swindustry, zxindustry=zxindustry
     )
     logger.success("因子后续的必要测试全部完成")
 
 
+def test_on_index_four_out(
+    fac: pd.DataFrame,
+    value_weighted: bool = 1,
+    trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
+    group_num: int = 10,
+    boxcox: bool = 1,
+    comments_writer: pd.ExcelWriter = None,
+    net_values_writer: pd.ExcelWriter = None,
+    opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
+):
+    if comments_writer is None:
+        from pure_ocean_breeze.state.states import COMMENTS_WRITER
+
+        comments_writer = COMMENTS_WRITER
+    if net_values_writer is None:
+        from pure_ocean_breeze.state.states import NET_VALUES_WRITER
+
+        net_values_writer = NET_VALUES_WRITER
+
+    shen = pure_moonnight(
+        fac,
+        opens_average_first_day=opens_average_first_day,
+    )
+    if (
+        shen.shen.group_net_values.group1.iloc[-1]
+        > shen.shen.group_net_values10.iloc[-1]
+    ):
+        neg = 1
+        pos = 0
+    else:
+        pos = 1
+        neg = 0
+
+    """3510多空和多头"""
+    # 300
+    fi300 = daily_factor_on300500(fac, hs300=1)
+    shen = pure_moonnight(
+        fi300,
+        value_weighted=value_weighted,
+        groups_num=group_num,
+        boxcox=boxcox,
+        comments_writer=comments_writer,
+        net_values_writer=net_values_writer,
+        sheetname="300多空",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
+    )
+    if pos:
+        if comments_writer is not None:
+            make_relative_comments(
+                shen.shen.group_rets[f"group{group_num}"], hs300=1
+            ).to_excel(comments_writer, sheet_name="300超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    hs300=1,
+                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], hs300=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], hs300=1
+            ).to_excel(net_values_writer, sheet_name="300超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    hs300=1,
+                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], hs300=1
+            )
+    elif neg:
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
+                comments_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    hs300=1,
+                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, hs300=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
+                net_values_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    hs300=1,
+                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1)
+    else:
+        raise IOError("请指定因子的方向是正是负🤒")
+    # 500
+    fi500 = daily_factor_on300500(fac, zz500=1)
+    shen = pure_moonnight(
+        fi500,
+        value_weighted=value_weighted,
+        groups_num=group_num,
+        boxcox=boxcox,
+        comments_writer=comments_writer,
+        net_values_writer=net_values_writer,
+        sheetname="500多空",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
+    )
+    if pos:
+        if comments_writer is not None:
+            make_relative_comments(
+                shen.shen.group_rets[f"group{group_num}"], zz500=1
+            ).to_excel(comments_writer, sheet_name="500超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz500=1,
+                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], zz500=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz500=1
+            ).to_excel(net_values_writer, sheet_name="500超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz500=1,
+                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz500=1
+            )
+    else:
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
+                comments_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz500=1,
+                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, zz500=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
+                net_values_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz500=1,
+                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1)
+    # 1000
+    fi1000 = daily_factor_on300500(fac, zz1000=1)
+    shen = pure_moonnight(
+        fi1000,
+        value_weighted=value_weighted,
+        groups_num=group_num,
+        boxcox=boxcox,
+        comments_writer=comments_writer,
+        net_values_writer=net_values_writer,
+        sheetname="1000多空",
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
+    )
+    if pos:
+        if comments_writer is not None:
+            make_relative_comments(
+                shen.shen.group_rets[f"group{group_num}"], zz1000=1
+            ).to_excel(comments_writer, sheet_name="1000超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz1000=1,
+                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], zz1000=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz1000=1
+            ).to_excel(net_values_writer, sheet_name="1000超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz1000=1,
+                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz1000=1
+            )
+    else:
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
+                comments_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz1000=1,
+                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, zz1000=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
+                net_values_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz1000=1,
+                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1)
+
+
 class pure_helper(object):
     def __init__(
         self,
         df_main: pd.DataFrame,
         df_helper: pd.DataFrame,
         func: Callable = None,
         group: int = 10,
@@ -4205,30 +4491,31 @@
         return df
 
 
 class pure_fama(object):
     # @lru_cache(maxsize=None)
     def __init__(
         self,
-        factors: list[pd.DataFrame],
+        factors: List[pd.DataFrame],
         minus_group: Union[list, float] = 3,
         backsee: int = 20,
         rets: pd.DataFrame = None,
         value_weighted: bool = 1,
         add_market: bool = 1,
         add_market_series: pd.Series = None,
         factors_names: list = None,
         betas_rets: bool = 0,
+        total_cap: bool = 0,
     ) -> None:
         """使用fama三因子的方法，将个股的收益率，拆分出各个因子带来的收益率以及特质的收益率
         分别计算每一期，各个因子收益率的值，超额收益率，因子的暴露，以及特质收益率
 
         Parameters
         ----------
-        factors : list[pd.DataFrame]
+        factors : List[pd.DataFrame]
             用于解释收益的各个因子值，每一个都是index为时间，columns为股票代码，values为因子值的dataframe
         minus_group : Union[list, float], optional
             每一个因子将截面上的股票分为几组, by default 3
         backsee : int, optional
             做时序回归时，回看的天数, by default 20
         rets : pd.DataFrame, optional
             每只个股的收益率，index为时间，columns为股票代码，values为收益率，默认使用当日日间收益率, by default None
@@ -4238,14 +4525,16 @@
             是否加入市场收益率因子，默认使用中证全指的每日日间收益率, by default 1
         add_market_series : bool, optional
             加入的市场收益率的数据，如果没指定，则使用中证全指的日间收益率, by default None
         factors_names : list, optional
             各个因子的名字，默认为fac0(市场收益率因子，如果没有，则从fac1开始),fac1,fac2,fac3, by default None
         betas_rets : bool, optional
             是否计算每只个股的由于暴露在每个因子上所带来的收益率, by default 0
+        total_cap : bool, optional
+            加权时使用总市值, by default 0
         """
         start = max(
             [int(datetime.datetime.strftime(i.index.min(), "%Y%m%d")) for i in factors]
         )
         self.backsee = backsee
         self.factors = factors
         self.factors_names = factors_names
@@ -4261,14 +4550,16 @@
         ]
         self.factors_group_long = [(i == 0) + 0 for i in self.factors_group]
         self.factors_group_short = [
             (i == (j - 1)) + 0 for i, j in zip(self.factors_group, self.minus_group)
         ]
         self.value_weighted = value_weighted
         if value_weighted:
+            if total_cap:
+                self.cap = read_daily(total_cap=1, start=start)
             self.cap = read_daily(flow_cap=1, start=start)
             self.factors_group_long = [self.cap * i for i in self.factors_group_long]
             self.factors_group_short = [self.cap * i for i in self.factors_group_short]
             self.factors_group_long = [
                 (i.T / i.T.sum()).T for i in self.factors_group_long
             ]
             self.factors_group_short = [
@@ -4305,18 +4596,15 @@
             else:
                 closes = add_market_series.to_frame("fac0")
             rets = closes / closes.shift(1) - 1
             self.__factors_rets = pd.concat([rets, self.__factors_rets], axis=1)
             if factors_names is not None:
                 factors_names = ["市场"] + factors_names
         self.__data = self.make_df(self.rets, self.__factors_rets)
-        if is_notebook():
-            tqdm.tqdm_notebook().pandas()
-        else:
-            tqdm.tqdm.pandas()
+        tqdm.auto.tqdm.pandas()
         self.__coefficients = (
             self.__data.groupby("code").progress_apply(self.ols_in).reset_index()
         )
         self.__coefficients = self.__coefficients.rename(
             columns={
                 i: "co" + i for i in list(self.__coefficients.columns) if "fac" in i
             }
@@ -4429,29 +4717,29 @@
             ...
 
 
 class pure_rollingols(object):
     def __init__(
         self,
         y: pd.DataFrame,
-        xs: Union[list[pd.DataFrame], pd.DataFrame],
+        xs: Union[List[pd.DataFrame], pd.DataFrame],
         backsee: int = 20,
-        factors_names: list[str] = None,
+        factors_names: List[str] = None,
     ) -> None:
         """使用若干个dataframe，对应的股票进行指定窗口的时序滚动回归
 
         Parameters
         ----------
         y : pd.DataFrame
             滚动回归中的因变量y，index是时间，columns是股票代码
-        xs : Union[list[pd.DataFrame], pd.DataFrame]
+        xs : Union[List[pd.DataFrame], pd.DataFrame]
             滚动回归中的自变量xi，每一个dataframe，index是时间，columns是股票代码
         backsee : int, optional
             滚动回归的时间窗口, by default 20
-        factors_names : list[str], optional
+        factors_names : List[str], optional
             xs中，每个因子的名字, by default None
         """
         self.backsee = backsee
         self.y = y
         if not isinstance(xs, list):
             xs = [xs]
         self.xs = xs
@@ -4465,18 +4753,15 @@
             for j, i in enumerate(xs)
         ]
         xs = [y] + xs
         xs = reduce(lambda x, y: pd.merge(x, y, on=["date", "code"]), xs)
         xs = xs.set_index("date")
         self.__data = xs
         self.haha = xs
-        if is_notebook():
-            tqdm.tqdm_notebook().pandas()
-        else:
-            tqdm.tqdm.pandas()
+        tqdm.auto.tqdm.pandas()
         self.__coefficients = (
             self.__data.groupby("code").progress_apply(self.ols_in).reset_index()
         )
         self.__coefficients = self.__coefficients.rename(
             columns={i: "co" + i for i in list(self.__coefficients.columns) if "x" in i}
         )
         self.__data = pd.merge(
@@ -4497,18 +4782,18 @@
         self.__alphas = self.__data.pivot(
             index="date", columns="code", values="intercept"
         )
         if factors_names is None:
             self.__betas = {
                 i: self.__data.pivot(index="date", columns="code", values=i)
                 for i in list(self.__data.columns)
-                if i.startswith("x")
+                if i.startswith("cox")
             }
         else:
-            facs = [i for i in list(self.__data.columns) if i.startswith("x")]
+            facs = [i for i in list(self.__data.columns) if i.startswith("cox")]
             self.__betas = {
                 factors_names[num]: self.__data.pivot(
                     index="date", columns="code", values=i
                 )
                 for num, i in enumerate(facs)
             }
         if len(list(self.__betas)) == 1:
@@ -4546,51 +4831,77 @@
             return pd.concat([alpha, betas], axis=1)
 
         except Exception:
             # 有些数据总共不足，那就跳过
             ...
 
 
+@do_on_dfs
 def test_on_300500(
     df: pd.DataFrame,
+    trade_cost_double_side: float = 0,
+    group_num: int = 10,
+    value_weighted: bool = 1,
+    boxcox: bool = 0,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     iplot: bool = 1,
+    opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
 ) -> pd.Series:
     """对因子在指数成分股内进行多空和多头测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
+    trade_cost_double_side : float, optional
+        交易的双边手续费率, by default 0
+    group_num : int
+        分组数量, by default 10
+    value_weighted : bool
+        是否进行流通市值加权, by default 0
     hs300 : bool, optional
         在沪深300成分股内测试, by default 0
     zz500 : bool, optional
         在中证500成分股内测试, by default 0
     zz1000 : bool, optional
         在中证1000成分股内测试, by default 0
     gz1000 : bool, optional
         在国证2000成分股内测试, by default 0
-    iplot : bol,optional
+    iplot : bo0l,optional
         多空回测的时候，是否使用cufflinks绘画
+    opens_average_first_day : bool, optional
+        买入时使用第一天的平均价格, by default 0
+    total_cap : bool, optional
+        加权和行业市值中性化时使用总市值, by default 0
 
     Returns
     -------
     pd.Series
         多头组在该指数上的超额收益序列
     """
     fi300 = daily_factor_on300500(
         df, hs300=hs300, zz500=zz500, zz1000=zz1000, gz2000=gz2000
     )
-    shen = pure_moonnight(fi300, iplot=iplot)
+    shen = pure_moonnight(
+        fi300,
+        value_weighted=value_weighted,
+        groups_num=group_num,
+        trade_cost_double_side=trade_cost_double_side,
+        boxcox=boxcox,
+        iplot=iplot,
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
+    )
     if (
         shen.shen.group_net_values.group1.iloc[-1]
-        > shen.shen.group_net_values.group10.iloc[-1]
+        > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
     ):
         print(
             make_relative_comments(
                 shen.shen.group_rets.group1,
                 hs300=hs300,
                 zz500=zz500,
                 zz1000=zz1000,
@@ -4604,96 +4915,177 @@
             zz1000=zz1000,
             gz2000=gz2000,
         )
         return abrets
     else:
         print(
             make_relative_comments(
-                shen.shen.group_rets.group10,
+                shen.shen.group_rets[f"group{group_num}"],
                 hs300=hs300,
                 zz500=zz500,
                 zz1000=zz1000,
                 gz2000=gz2000,
             )
         )
         abrets = make_relative_comments_plot(
-            shen.shen.group_rets.group10,
+            shen.shen.group_rets[f"group{group_num}"],
             hs300=hs300,
             zz500=zz500,
             zz1000=zz1000,
             gz2000=gz2000,
         )
         return abrets
 
 
+@do_on_dfs
 def test_on_index_four(
-    df: pd.DataFrame, iplot: bool = 1, gz2000: bool = 0, boxcox: bool = 1
+    df: pd.DataFrame,
+    value_weighted: bool = 1,
+    group_num: int = 10,
+    trade_cost_double_side: float = 0,
+    iplot: bool = 1,
+    gz2000: bool = 0,
+    boxcox: bool = 1,
+    opens_average_first_day: bool = 0,
+    total_cap: bool = 0,
 ) -> pd.DataFrame:
     """对因子同时在沪深300、中证500、中证1000、国证2000这4个指数成分股内进行多空和多头超额测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
+    value_weighted : bool
+        是否进行流通市值加权, by default 0
+    group_num : int
+        分组数量, by default 10
+    trade_cost_double_side : float, optional
+        交易的双边手续费率, by default 0
     iplot : bol,optional
         多空回测的时候，是否使用cufflinks绘画
     gz2000 : bool, optional
         是否进行国证2000上的测试, by default 0
     boxcox : bool, optional
         是否进行行业市值中性化处理, by default 1
+    opens_average_first_day : bool, optional
+        买入时使用第一天的平均价格, by default 0
+    total_cap : bool, optional
+        加权和行业市值中性化时使用总市值, by default 0
 
     Returns
     -------
     pd.DataFrame
         多头组在各个指数上的超额收益序列
     """
     fi300 = daily_factor_on300500(df, hs300=1)
-    shen = pure_moonnight(fi300, iplot=iplot, boxcox=boxcox)
+    shen = pure_moonnight(
+        fi300,
+        groups_num=group_num,
+        value_weighted=value_weighted,
+        trade_cost_double_side=trade_cost_double_side,
+        iplot=iplot,
+        boxcox=boxcox,
+        opens_average_first_day=opens_average_first_day,
+        total_cap=total_cap,
+    )
     if (
         shen.shen.group_net_values.group1.iloc[-1]
-        > shen.shen.group_net_values.group10.iloc[-1]
+        > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
     ):
         com300, net300 = make_relative_comments(
             shen.shen.group_rets.group1, hs300=1, show_nets=1
         )
         fi500 = daily_factor_on300500(df, zz500=1)
-        shen = pure_moonnight(fi500, iplot=iplot, boxcox=boxcox)
+        shen = pure_moonnight(
+            fi500,
+            groups_num=group_num,
+            value_weighted=value_weighted,
+            trade_cost_double_side=trade_cost_double_side,
+            iplot=iplot,
+            boxcox=boxcox,
+            opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
+        )
         com500, net500 = make_relative_comments(
             shen.shen.group_rets.group1, zz500=1, show_nets=1
         )
         fi1000 = daily_factor_on300500(df, zz1000=1)
-        shen = pure_moonnight(fi1000, iplot=iplot, boxcox=boxcox)
+        shen = pure_moonnight(
+            fi1000,
+            groups_num=group_num,
+            value_weighted=value_weighted,
+            trade_cost_double_side=trade_cost_double_side,
+            iplot=iplot,
+            boxcox=boxcox,
+            opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
+        )
         com1000, net1000 = make_relative_comments(
             shen.shen.group_rets.group1, zz1000=1, show_nets=1
         )
         if gz2000:
             fi2000 = daily_factor_on300500(df, gz2000=1)
-            shen = pure_moonnight(fi2000, iplot=iplot, boxcox=boxcox)
+            shen = pure_moonnight(
+                fi2000,
+                groups_num=group_num,
+                trade_cost_double_side=trade_cost_double_side,
+                iplot=iplot,
+                boxcox=boxcox,
+                opens_average_first_day=opens_average_first_day,
+                total_cap=total_cap,
+            )
             com2000, net2000 = make_relative_comments(
                 shen.shen.group_rets.group1, gz2000=1, show_nets=1
             )
     else:
         com300, net300 = make_relative_comments(
-            shen.shen.group_rets.group10, hs300=1, show_nets=1
+            shen.shen.group_rets[f"group{group_num}"], hs300=1, show_nets=1
         )
         fi500 = daily_factor_on300500(df, zz500=1)
-        shen = pure_moonnight(fi500, iplot=iplot, boxcox=boxcox)
+        shen = pure_moonnight(
+            fi500,
+            groups_num=group_num,
+            value_weighted=value_weighted,
+            trade_cost_double_side=trade_cost_double_side,
+            iplot=iplot,
+            boxcox=boxcox,
+            opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
+        )
         com500, net500 = make_relative_comments(
-            shen.shen.group_rets.group10, zz500=1, show_nets=1
+            shen.shen.group_rets[f"group{group_num}"], zz500=1, show_nets=1
         )
         fi1000 = daily_factor_on300500(df, zz1000=1)
-        shen = pure_moonnight(fi1000, iplot=iplot, boxcox=boxcox)
+        shen = pure_moonnight(
+            fi1000,
+            groups_num=group_num,
+            value_weighted=value_weighted,
+            trade_cost_double_side=trade_cost_double_side,
+            iplot=iplot,
+            boxcox=boxcox,
+            opens_average_first_day=opens_average_first_day,
+            total_cap=total_cap,
+        )
         com1000, net1000 = make_relative_comments(
-            shen.shen.group_rets.group10, zz1000=1, show_nets=1
+            shen.shen.group_rets[f"group{group_num}"], zz1000=1, show_nets=1
         )
         if gz2000:
             fi2000 = daily_factor_on300500(df, gz2000=1)
-            shen = pure_moonnight(fi2000, iplot=iplot, boxcox=boxcox)
+            shen = pure_moonnight(
+                fi2000,
+                groups_num=group_num,
+                value_weighted=value_weighted,
+                trade_cost_double_side=trade_cost_double_side,
+                iplot=iplot,
+                boxcox=boxcox,
+                opens_average_first_day=opens_average_first_day,
+                total_cap=total_cap,
+            )
             com2000, net2000 = make_relative_comments(
-                shen.shen.group_rets.group10, gz2000=1, show_nets=1
+                shen.shen.group_rets[f"group{group_num}"], gz2000=1, show_nets=1
             )
     com300 = com300.to_frame("300超额")
     com500 = com500.to_frame("500超额")
     com1000 = com1000.to_frame("1000超额")
     if gz2000:
         com2000 = com2000.to_frame("2000超额")
         coms = pd.concat([com300, com500, com1000, com2000], axis=1)
@@ -4733,15 +5125,15 @@
                 specs=[
                     [
                         None,
                         {"rowspan": 2, "colspan": 4},
                         None,
                         None,
                         None,
-                        {"rowspan": 2, "colspan": 5},
+                        {"rowspan": 2, "colspan": 3},
                         None,
                         None,
                         None,
                         None,
                     ],
                     [
                         None,
@@ -4767,15 +5159,15 @@
                 shared_yaxes=False,
                 specs=[
                     [
                         None,
                         {"rowspan": 2, "colspan": 3},
                         None,
                         None,
-                        {"rowspan": 2, "colspan": 6},
+                        {"rowspan": 2, "colspan": 3},
                         None,
                         None,
                         None,
                         None,
                         None,
                     ],
                     [
@@ -4801,24 +5193,26 @@
         tb.set_cols_width([8] + [7] + [8] * 2 + [7] * 2 + [8])
         tb.set_cols_dtype(["f"] * 7)
         tb.header(list(coms.T.reset_index().columns))
         tb.add_rows(coms.T.reset_index().to_numpy(), header=True)
         print(tb.draw())
 
 
+@do_on_dfs
 class pure_star(object):
     def __init__(
         self,
         fac: pd.Series,
         code: str = None,
         price_opens: pd.Series = None,
         iplot: bool = 1,
         comments_writer: pd.ExcelWriter = None,
         net_values_writer: pd.ExcelWriter = None,
         sheetname: str = None,
+        questdb_host: str = "127.0.0.1",
     ):
         """择时回测框架，输入仓位比例或信号值，依据信号买入对应的股票或指数，并考察绝对收益、超额收益和基准收益
         回测方式为，t日收盘时获得信号，t+1日开盘时以开盘价买入，t+2开盘时以开盘价卖出
 
         Parameters
         ----------
         fac : pd.Series
@@ -4831,27 +5225,29 @@
             使用cufflinks呈现回测绩效和走势图, by default 1
         comments_writer : pd.ExcelWriter, optional
             绩效评价的存储文件, by default None
         net_values_writer : pd.ExcelWriter, optional
             净值序列的存储文件, by default None
         sheetname : str, optional
             存储文件的工作表的名字, by default None
+        questdb_host: str, optional
+            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
         """
         if code is not None:
             x1 = code.split(".")[0]
             x2 = code.split(".")[1]
             if (x1[0] == "0" or x1[:2] == "30") and x2 == "SZ":
                 kind = "stock"
             elif x1[0] == "6" and x2 == "SH":
                 kind = "stock"
             else:
                 kind = "index"
             self.kind = kind
             if kind == "index":
-                qdb = Questdb()
+                qdb = Questdb(host=questdb_host)
                 price_opens = qdb.get_data(
                     f"select date,num,close from minute_data_{kind} where code='{code}'"
                 )
                 price_opens = price_opens[price_opens.num == "1"]
                 price_opens = price_opens.set_index("date").close
                 price_opens.index = pd.to_datetime(price_opens.index, format="%Y%m%d")
             else:
@@ -4884,20 +5280,20 @@
         self.total_comments.columns = (
             self.total_nets.columns
         ) = self.total_rets.columns = ["因子绝对", "因子超额", "买入持有"]
         self.total_comments = np.around(self.total_comments, 3)
         self.iplot = iplot
         self.plot()
         if comments_writer is None and sheetname is not None:
-            from pure_ocean_breeze.legacy_version.v3p4.state.states import COMMENTS_WRITER
+            from pure_ocean_breeze.state.states import COMMENTS_WRITER
 
             comments_writer = COMMENTS_WRITER
             self.total_comments.to_excel(comments_writer, sheet_name=sheetname)
         if net_values_writer is None and sheetname is not None:
-            from pure_ocean_breeze.legacy_version.v3p4.state.states import NET_VALUES_WRITER
+            from pure_ocean_breeze.state.states import NET_VALUES_WRITER
 
             net_values_writer = NET_VALUES_WRITER
             self.total_nets.to_excel(net_values_writer, sheet_name=sheetname)
 
     def plot(self):
         coms = self.total_comments.copy().reset_index()
         if self.iplot:
@@ -4956,7 +5352,1373 @@
             plt.show()
             tb = Texttable()
             tb.set_cols_width([8] + [7] + [8] * 2 + [7] * 2 + [8])
             tb.set_cols_dtype(["f"] * 7)
             tb.header(list(coms.T.reset_index().columns))
             tb.add_rows(coms.T.reset_index().to_numpy(), header=True)
             print(tb.draw())
+
+
+@do_on_dfs
+def get_group(df: pd.DataFrame, group_num: int = 10) -> pd.DataFrame:
+    """使用groupby的方法，将一组因子值改为截面上的分组值，此方法相比qcut的方法更加稳健，但速度更慢一些
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        因子值，index为时间，columns为股票代码，values为因子值
+    group_num : int, optional
+        分组的数量, by default 10
+
+    Returns
+    -------
+    pd.DataFrame
+        转化为分组值后的df，index为时间，columns为股票代码，values为分组值
+    """
+    a = pure_moon(no_read_indu=1)
+    df = df.stack().reset_index()
+    df.columns = ["date", "code", "fac"]
+    df = a.get_groups(df, group_num).pivot(index="date", columns="code", values="group")
+    return df
+
+
+class pure_linprog(object):
+    def __init__(
+        self,
+        facs: pd.DataFrame,
+        total_caps: pd.DataFrame = None,
+        indu_dummys: pd.DataFrame = None,
+        index_weights_hs300: pd.DataFrame = None,
+        index_weights_zz500: pd.DataFrame = None,
+        index_weights_zz1000: pd.DataFrame = None,
+        opens: pd.DataFrame = None,
+        closes: pd.DataFrame = None,
+        hs300_closes: pd.DataFrame = None,
+        zz500_closes: pd.DataFrame = None,
+        zz1000_closes: pd.DataFrame = None,
+    ) -> None:
+        """线性规划求解，目标为预期收益率最大（即因子方向为负时，组合因子值最小）
+        条件为，严格控制市值中性（数据：总市值的对数；含义：组合在市值上的暴露与指数在市值上的暴露相等）
+        严格控制行业中性（数据：使用中信一级行业哑变量），个股偏离在1%以内，成分股权重之和在80%以上
+        分别在沪深300、中证500、中证1000上优化求解
+
+        Parameters
+        ----------
+        facs : pd.DataFrame
+            因子值，index为时间，columns为股票代码，values为因子值
+        total_caps : pd.DataFrame, optional
+            总市值数据，index为时间，columns为股票代码，values为总市值, by default None
+        indu_dummys : pd.DataFrame, optional
+            行业哑变量，包含两列名为date的时间和code的股票代码，以及30+列行业哑变量, by default None
+        index_weights_hs300 : pd.DataFrame, optional
+            沪深300指数成分股权重，月频数据, by default None
+        index_weights_zz500 : pd.DataFrame, optional
+            中证500指数成分股权重，月频数据, by default None
+        index_weights_zz1000 : pd.DataFrame, optional
+            中证1000指数成分股权重，月频数据, by default None
+        opens : pd.DataFrame, optional
+            每月月初开盘价数据, by default None
+        closes : pd.DataFrame, optional
+            每月月末收盘价数据, by default None
+        hs300_closes : pd.DataFrame, optional
+            沪深300每月收盘价数据, by default None
+        zz500_closes : pd.DataFrame, optional
+            中证500每月收盘价数据,, by default None
+        zz1000_closes : pd.DataFrame, optional
+            中证1000每月收盘价数据,, by default None
+        """
+        self.facs = facs.resample("M").last()
+        if total_caps is None:
+            total_caps = standardlize(
+                np.log(read_daily(total_cap=1).resample("M").last())
+            )
+        if indu_dummys is None:
+            indu_dummys = read_daily(zxindustry_dummy_code=1)
+        if index_weights_hs300 is None:
+            index_weights_hs300 = read_daily(hs300_member_weight=1)
+        if index_weights_zz500 is None:
+            index_weights_zz500 = read_daily(zz500_member_weight=1)
+        if index_weights_zz1000 is None:
+            index_weights_zz1000 = read_daily(zz1000_member_weight=1)
+        if opens is None:
+            opens = read_daily(open=1).resample("M").first()
+        if closes is None:
+            closes = read_daily(close=1).resample("M").last()
+        if hs300_closes is None:
+            hs300_closes = read_index_single("000300.SH").resample("M").last()
+        if zz500_closes is None:
+            zz500_closes = read_index_single("000905.SH").resample("M").last()
+        if zz1000_closes is None:
+            zz1000_closes = read_index_single("000852.SH").resample("M").last()
+        self.total_caps = total_caps
+        self.indu_dummys = indu_dummys
+        self.index_weights_hs300 = index_weights_hs300
+        self.index_weights_zz500 = index_weights_zz500
+        self.index_weights_zz1000 = index_weights_zz1000
+        self.hs300_weights = []
+        self.zz500_weights = []
+        self.zz1000_weights = []
+        self.ret_next = closes / opens - 1
+        self.ret_hs300 = hs300_closes.pct_change()
+        self.ret_zz500 = zz500_closes.pct_change()
+        self.ret_zz1000 = zz1000_closes.pct_change()
+
+    def optimize_one_day(
+        self,
+        fac: pd.DataFrame,
+        flow_cap: pd.DataFrame,
+        indu_dummy: pd.DataFrame,
+        index_weight: pd.DataFrame,
+        name: str,
+    ) -> pd.DataFrame:
+        """优化单期求解
+
+        Parameters
+        ----------
+        fac : pd.DataFrame
+            单期因子值，index为code，columns为date，values为因子值
+        flow_cap : pd.DataFrame
+            流通市值，index为code，columns为date，values为截面标准化的流通市值
+        indu_dummy : pd.DataFrame
+            行业哑变量，index为code，columns为行业代码，values为哑变量
+        index_weight : pd.DataFrame
+            指数成分股权重，index为code，columns为date，values为权重
+
+        Returns
+        -------
+        pd.DataFrame
+            当期最佳权重
+        """
+        if fac.shape[0] > 0 and index_weight.shape[1] > 0:
+            date = fac.columns.tolist()[0]
+            codes = list(
+                set(fac.index)
+                | set(flow_cap.index)
+                | set(indu_dummy.index)
+                | set(index_weight.index)
+            )
+            fac, flow_cap, indu_dummy, index_weight = list(
+                map(
+                    lambda x: x.reindex(codes).fillna(0).to_numpy(),
+                    [fac, flow_cap, indu_dummy, index_weight],
+                )
+            )
+            sign_index_weight = np.sign(index_weight)
+            # 个股权重大于零、偏离1%
+            bounds = list(
+                zip(
+                    select_max(index_weight - 0.01, 0).flatten(),
+                    select_min(index_weight + 0.01, 1).flatten(),
+                )
+            )
+            # 市值中性+行业中性+权重和为1
+            huge = np.vstack([flow_cap.T, indu_dummy.T, np.array([1] * len(codes))])
+            target = (
+                list(flow_cap.T @ index_weight.flatten())
+                + list((indu_dummy.T @ index_weight).flatten())
+                + [np.sum(index_weight)]
+            )
+            # 写线性条件
+            c = fac.T.flatten().tolist()
+            a = sign_index_weight.reshape((1, -1)).tolist()
+            b = [0.8]
+            # 优化求解
+            res = linprog(c, a, b, huge, target, bounds)
+            if res.success:
+                return pd.DataFrame({date: res.x.tolist()}, index=codes)
+            else:
+                # raise NotImplementedError(f"{date}这一期的优化失败，请检查")
+                logger.warning(f"{name}在{date}这一期的优化失败，请检查")
+                return None
+        else:
+            return None
+
+    def optimize_many_days(self, startdate: int = 20130101):
+        dates = [i for i in self.facs.index if i >= pd.Timestamp(str(startdate))]
+        for date in tqdm.auto.tqdm(dates):
+            fac = self.facs[self.facs.index == date].T.dropna()
+            total_cap = self.total_caps[self.total_caps.index == date].T.dropna()
+            indu_dummy = self.indu_dummys[self.indu_dummys.date <= date]
+            indu_dummy = (
+                indu_dummy[indu_dummy.date == indu_dummy.date.max()]
+                .drop(columns=["date"])
+                .set_index("code")
+            )
+            index_weight_hs300 = self.index_weights_hs300[
+                self.index_weights_hs300.index == date
+            ].T.dropna()
+            index_weight_zz500 = self.index_weights_zz500[
+                self.index_weights_zz500.index == date
+            ].T.dropna()
+            index_weight_zz1000 = self.index_weights_zz1000[
+                self.index_weights_zz1000.index == date
+            ].T.dropna()
+            weight_hs300 = self.optimize_one_day(
+                fac, total_cap, indu_dummy, index_weight_hs300, "hs300"
+            )
+            weight_zz500 = self.optimize_one_day(
+                fac, total_cap, indu_dummy, index_weight_zz500, "zz500"
+            )
+            weight_zz1000 = self.optimize_one_day(
+                fac, total_cap, indu_dummy, index_weight_zz1000, "zz1000"
+            )
+            self.hs300_weights.append(weight_hs300)
+            self.zz500_weights.append(weight_zz500)
+            self.zz1000_weights.append(weight_zz1000)
+        self.hs300_weights = pd.concat(self.hs300_weights, axis=1).T
+        self.zz500_weights = pd.concat(self.zz500_weights, axis=1).T
+        self.zz1000_weights = pd.concat(self.zz1000_weights, axis=1).T
+
+    def make_contrast(self, weight, index, name) -> list[pd.DataFrame]:
+        ret = (weight.shift(1) * self.ret_next).sum(axis=1)
+        abret = ret - index
+        rets = pd.concat([ret, index, abret], axis=1).dropna()
+        rets.columns = [f"{name}增强组合净值", f"{name}指数净值", f"{name}增强组合超额净值"]
+        rets = (rets + 1).cumprod()
+        rets = rets.apply(lambda x: x / x.iloc[0])
+        comments = comments_on_twins(rets[f"{name}增强组合超额净值"], abret.dropna())
+        return comments, rets
+
+    def run(self, startdate: int = 20130101) -> pd.DataFrame:
+        """运行规划求解
+
+        Parameters
+        ----------
+        startdate : int, optional
+            起始日期, by default 20130101
+
+        Returns
+        -------
+        pd.DataFrame
+            超额绩效指标
+        """
+        self.optimize_many_days(startdate=startdate)
+        self.hs300_comments, self.hs300_nets = self.make_contrast(
+            self.hs300_weights, self.ret_hs300, "沪深300"
+        )
+        self.zz500_comments, self.zz500_nets = self.make_contrast(
+            self.zz500_weights, self.ret_zz500, "中证500"
+        )
+        self.zz1000_comments, self.zz1000_nets = self.make_contrast(
+            self.zz1000_weights, self.ret_zz1000, "中证1000"
+        )
+
+        figs = cf.figures(
+            pd.concat([self.hs300_nets, self.zz500_nets, self.zz1000_nets]),
+            [
+                dict(kind="line", y=list(self.hs300_nets.columns)),
+                dict(kind="line", y=list(self.zz500_nets.columns)),
+                dict(kind="line", y=list(self.zz1000_nets.columns)),
+            ],
+            asList=True,
+        )
+        base_layout = cf.tools.get_base_layout(figs)
+
+        sp = cf.subplots(
+            figs,
+            shape=(1, 3),
+            base_layout=base_layout,
+            vertical_spacing=0.15,
+            horizontal_spacing=0.03,
+            shared_yaxes=False,
+            subplot_titles=["沪深300增强", "中证500增强", "中证1000增强"],
+        )
+        sp["layout"].update(showlegend=True)
+        cf.iplot(sp)
+
+        self.comments = pd.concat(
+            [self.hs300_comments, self.zz500_comments, self.zz1000_comments], axis=1
+        )
+        self.comments.columns = ["沪深300超额", "中证500超额", "中证1000超额"]
+
+        from pure_ocean_breeze.state.states import COMMENTS_WRITER, NET_VALUES_WRITER
+
+        comments_writer = COMMENTS_WRITER
+        net_values_writer = NET_VALUES_WRITER
+        if comments_writer is not None:
+            self.hs300_comments.to_excel(comments_writer, sheet_name="沪深300组合优化超额绩效")
+            self.zz500_comments.to_excel(comments_writer, sheet_name="中证500组合优化超额绩效")
+            self.zz1000_comments.to_excel(comments_writer, sheet_name="中证1000组合优化超额绩效")
+        if net_values_writer is not None:
+            self.hs300_nets.to_excel(net_values_writer, sheet_name="沪深300组合优化净值")
+            self.zz500_nets.to_excel(net_values_writer, sheet_name="中证500组合优化净值")
+            self.zz1000_nets.to_excel(net_values_writer, sheet_name="中证1000组合优化净值")
+
+        return self.comments.T
+
+
+def symmetrically_orthogonalize(dfs: list[pd.DataFrame]) -> list[pd.DataFrame]:
+    """对多个因子做对称正交，每个因子得到正交其他因子后的结果
+
+    Parameters
+    ----------
+    dfs : list[pd.DataFrame]
+        多个要做正交的因子，每个df都是index为时间，columns为股票代码，values为因子值的df
+
+    Returns
+    -------
+    list[pd.DataFrame]
+        对称正交后的各个因子
+    """
+
+    def sing(dfs: list[pd.DataFrame], date: pd.Timestamp):
+        dds = []
+        for num, i in enumerate(dfs):
+            i = i[i.index == date]
+            i.index = [f"fac{num}"]
+            i = i.T
+            dds.append(i)
+        dds = pd.concat(dds, axis=1)
+        cov = dds.cov()
+        d, u = np.linalg.eig(cov)
+        d = np.diag(d ** (-0.5))
+        new_facs = pd.DataFrame(
+            np.dot(dds, np.dot(np.dot(u, d), u.T)), columns=dds.columns, index=dds.index
+        )
+        new_facs = new_facs.stack().reset_index()
+        new_facs.columns = ["code", "fac_number", "fac"]
+        new_facs = new_facs.assign(date=date)
+        dds = []
+        for num, i in enumerate(dfs):
+            i = new_facs[new_facs.fac_number == f"fac{num}"]
+            i = i.pivot(index="date", columns="code", values="fac")
+            dds.append(i)
+        return dds
+
+    dfs = [standardlize(i) for i in dfs]
+    date_first = max([i.index.min() for i in dfs])
+    date_last = min([i.index.max() for i in dfs])
+    dfs = [i[(i.index >= date_first) & (i.index <= date_last)] for i in dfs]
+    fac_num = len(dfs)
+    ddss = [[] for i in range(fac_num)]
+    for date in tqdm.auto.tqdm(dfs[0].index):
+        dds = sing(dfs, date)
+        for num, i in enumerate(dds):
+            ddss[num].append(i)
+    ds = []
+    for i in tqdm.auto.tqdm(ddss):
+        ds.append(pd.concat(i))
+    return ds
+
+
+def icir_weight(
+    facs: list[pd.DataFrame],
+    backsee: int = 6,
+    boxcox: bool = 0,
+    rank_corr: bool = 0,
+    only_ic: bool = 0,
+) -> pd.DataFrame:
+    """使用icir滚动加权的方式，加权合成几个因子
+
+    Parameters
+    ----------
+    facs : list[pd.DataFrame]
+        要合成的若干因子，每个df都是index为时间，columns为股票代码，values为因子值的df
+    backsee : int, optional
+        用来计算icir的过去期数, by default 6
+    boxcox : bool, optional
+        是否对因子进行行业市值中性化, by default 0
+    rank_corr : bool, optional
+        是否计算rankicir, by default 0
+    only_ic : bool, optional
+        是否只计算IC或Rank IC, by default 0
+
+    Returns
+    -------
+    pd.DataFrame
+        合成后的因子
+
+    Raises
+    ------
+    ValueError
+        因子期数少于回看期数时将报错
+    """
+    date_first_max = max([i.index[0] for i in facs])
+    facs = [i[i.index >= date_first_max] for i in facs]
+    date_last_min = min([i.index[-1] for i in facs])
+    facs = [i[i.index <= date_last_min] for i in facs]
+    facs = [i.shift(1) for i in facs]
+    ret = read_daily(
+        close=1, start=datetime.datetime.strftime(date_first_max, "%Y%m%d")
+    )
+    ret = ret / ret.shift(20) - 1
+    if boxcox:
+        facs = [decap_industry(i) for i in facs]
+    facs = [((i.T - i.T.mean()) / i.T.std()).T for i in facs]
+    dates = list(facs[0].index)
+    fis = []
+    for num, date in tqdm.auto.tqdm(list(enumerate(dates))):
+        if num < backsee:
+            ...
+        else:
+            nears = [i.iloc[num - backsee : num, :] for i in facs]
+            targets = [i[i.index == date] for i in facs]
+            if rank_corr:
+                weights = [
+                    show_corr(
+                        i, ret[ret.index.isin(i.index)], plt_plot=0, show_series=1
+                    )
+                    for i in nears
+                ]
+            else:
+                weights = [
+                    show_corr(
+                        i,
+                        ret[ret.index.isin(i.index)],
+                        plt_plot=0,
+                        show_series=1,
+                        method="pearson",
+                    )
+                    for i in nears
+                ]
+            if only_ic:
+                weights = [i.mean() for i in weights]
+            else:
+                weights = [i.mean() / i.std() for i in weights]
+            fi = sum([i * j for i, j in zip(weights, targets)])
+            fis.append(fi)
+    if len(fis) > 0:
+        return pd.concat(fis).shift(-1)
+    else:
+        raise ValueError("输入的因子值长度不太够吧？")
+
+
+def scipy_weight(
+    facs: list[pd.DataFrame],
+    backsee: int = 6,
+    boxcox: bool = 0,
+    rank_corr: bool = 0,
+    only_ic: bool = 0,
+    upper_bound: float = None,
+    lower_bound: float = 0,
+) -> pd.DataFrame:
+    """使用scipy的minimize优化求解的方式，寻找最优的因子合成权重，默认优化条件为最大ICIR
+
+    Parameters
+    ----------
+    facs : list[pd.DataFrame]
+        要合成的因子，每个df都是index为时间，columns为股票代码，values为因子值的df
+    backsee : int, optional
+        用来计算icir的过去期数, by default 6
+    boxcox : bool, optional
+        是否对因子进行行业市值中性化, by default 0
+    rank_corr : bool, optional
+        是否计算rankicir, by default 0
+    only_ic : bool, optional
+        是否只计算IC或Rank IC, by default 0
+    upper_bound : float, optional
+        每个因子的权重上限，如果不指定，则为每个因子平均权重的2倍，即2除以因子数量, by default None
+    lower_bound : float, optional
+        每个因子的权重下限, by default 0
+
+    Returns
+    -------
+    pd.DataFrame
+        合成后的因子
+    """
+    date_first_max = max([i.index[0] for i in facs])
+    facs = [i[i.index >= date_first_max] for i in facs]
+    date_last_min = min([i.index[-1] for i in facs])
+    facs = [i[i.index <= date_last_min] for i in facs]
+    facs = [i.shift(1) for i in facs]
+    ret = read_daily(
+        close=1, start=datetime.datetime.strftime(date_first_max, "%Y%m%d")
+    )
+    ret = ret / ret.shift(20) - 1
+    if boxcox:
+        facs = [decap_industry(i) for i in facs]
+    facs = [((i.T - i.T.mean()) / i.T.std()).T for i in facs]
+    if upper_bound is None:
+        upper_bound = 2 / len(facs)
+    dates = list(facs[0].index)
+    fis = []
+    for num, date in tqdm.auto.tqdm(list(enumerate(dates))):
+        if num <= backsee:
+            ...
+        else:
+            nears = [i.iloc[num - backsee : num, :] for i in facs]
+            targets = [i[i.index == date] for i in facs]
+            if rank_corr:
+                weights = [
+                    show_corr(
+                        i, ret[ret.index.isin(i.index)], plt_plot=0, show_series=1
+                    )
+                    for i in nears
+                ]
+            else:
+                weights = [
+                    show_corr(
+                        i,
+                        ret[ret.index.isin(i.index)],
+                        plt_plot=0,
+                        show_series=1,
+                        method="pearson",
+                    )
+                    for i in nears
+                ]
+            if only_ic:
+                weights = [i.mean() for i in weights]
+            else:
+                weights = [i.mean() / i.std() for i in weights]
+            weights = pd.concat(weights, axis=1)
+
+            def func(x):
+                w = np.array(x).reshape((-1, 1))
+                y = weights @ w
+                return np.mean(y) / np.std(y)
+
+            cons = {"type": "eq", "fun": lambda x: np.sum(x) - 1}
+            res = minimize(
+                func,
+                np.random.rand(weights.shape[1], 1),
+                constraints=cons,
+                bounds=[(lower_bound, upper_bound)] * weights.shape[1],
+            )
+            xs = res.x.tolist()
+            fac = sum([i * j for i, j in zip(xs, targets)])
+            fis.append(fac)
+    return pd.concat(fis).shift(-1)
+
+
+# 此处未完成，待改写
+class pure_fall_second(object):
+    """对单只股票单日进行操作"""
+
+    def __init__(
+        self,
+        factor_file: str,
+        project: str = None,
+        startdate: int = None,
+        enddate: int = None,
+        questdb_host: str = "127.0.0.1",
+        ignore_history_in_questdb: bool = 0,
+        groupby_target: list = ["date", "code"],
+    ) -> None:
+        """基于clickhouse的分钟数据，计算因子值，每天的因子值只用到当日的数据
+
+        Parameters
+        ----------
+        factor_file : str
+            用于保存因子值的文件名，需为parquet文件，以'.parquet'结尾
+        project : str, optional
+            该因子所属项目，即子文件夹名称, by default None
+        startdate : int, optional
+            起始时间，形如20121231，为开区间, by default None
+        enddate : int, optional
+            截止时间，形如20220814，为闭区间，为空则计算到最近数据, by default None
+        questdb_host: str, optional
+            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
+        ignore_history_in_questdb : bool, optional
+            打断后重新从头计算，清除在questdb中的记录
+        groupby_target: list, optional
+            groupby计算时，分组的依据，使用此参数时，自定义函数的部分，如果指定按照['date']分组groupby计算，
+            则返回时，应当返回一个两列的dataframe，第一列为股票代码，第二列为为因子值, by default ['date','code']
+        """
+        homeplace = HomePlace()
+        self.groupby_target = groupby_target
+        self.chc = ClickHouseClient("second_data")
+        # 将计算到一半的因子，存入questdb中，避免中途被打断后重新计算，表名即为因子文件名的汉语拼音
+        pinyin = Pinyin()
+        self.factor_file_pinyin = pinyin.get_pinyin(
+            factor_file.replace(".parquet", ""), ""
+        )
+        self.factor_steps = Questdb(host=questdb_host)
+        if project is not None:
+            if not os.path.exists(homeplace.factor_data_file + project):
+                os.makedirs(homeplace.factor_data_file + project)
+            else:
+                logger.info(f"当前正在{project}项目中……")
+        else:
+            logger.warning("当前因子不属于任何项目，这将造成因子数据文件夹的混乱，不便于管理，建议指定一个项目名称")
+        # 完整的因子文件路径
+        if project is not None:
+            factor_file = homeplace.factor_data_file + project + "/" + factor_file
+        else:
+            factor_file = homeplace.factor_data_file + factor_file
+        self.factor_file = factor_file
+        # 读入之前的因子
+        if os.path.exists(factor_file):
+            factor_old = drop_duplicates_index(pd.read_parquet(self.factor_file))
+            self.factor_old = factor_old
+            # 已经算好的日子
+            dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
+            self.dates_old = dates_old
+        elif (not ignore_history_in_questdb) and self.factor_file_pinyin in list(
+            self.factor_steps.get_data("show tables").table
+        ):
+            logger.info(
+                f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，现在将读取上次的数据，继续计算"
+            )
+            factor_old = self.factor_steps.get_data_with_tuple(
+                f"select * from '{self.factor_file_pinyin}'"
+            ).drop_duplicates(subset=["date", "code"])
+            factor_old = factor_old.pivot(index="date", columns="code", values="fac")
+            factor_old = factor_old.sort_index()
+            self.factor_old = factor_old
+            # 已经算好的日子
+            dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
+            self.dates_old = dates_old
+        elif ignore_history_in_questdb and self.factor_file_pinyin in list(
+            self.factor_steps.get_data("show tables").table
+        ):
+            logger.info(
+                f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，但您选择重新计算，所以正在删除原来的数据，从头计算"
+            )
+            factor_old = self.factor_steps.do_order(
+                f"drop table '{self.factor_file_pinyin}'"
+            )
+            self.factor_old = None
+            self.dates_old = []
+            logger.info("删除完毕，正在重新计算")
+        else:
+            self.factor_old = None
+            self.dates_old = []
+            logger.info("这个因子以前没有，正在重新计算")
+        # 读取当前所有的日子
+        dates_all = self.chc.show_all_dates(f"second_data_stock_10s")
+        dates_all = [int(i) for i in dates_all]
+        if startdate is None:
+            ...
+        else:
+            dates_all = [i for i in dates_all if i >= startdate]
+        if enddate is None:
+            ...
+        else:
+            dates_all = [i for i in dates_all if i <= enddate]
+        self.dates_all = dates_all
+        # 需要新补充的日子
+        self.dates_new = sorted([i for i in dates_all if i not in self.dates_old])
+        if len(self.dates_new) == 0:
+            ...
+        elif len(self.dates_new) == 1:
+            self.dates_new_intervals = [[pd.Timestamp(str(self.dates_new[0]))]]
+            print(f"只缺一天{self.dates_new[0]}")
+        else:
+            dates = [pd.Timestamp(str(i)) for i in self.dates_new]
+            intervals = [[]] * len(dates)
+            interbee = 0
+            intervals[0] = intervals[0] + [dates[0]]
+            for i in range(len(dates) - 1):
+                val1 = dates[i]
+                val2 = dates[i + 1]
+                if val2 - val1 < pd.Timedelta(days=30):
+                    ...
+                else:
+                    interbee = interbee + 1
+                intervals[interbee] = intervals[interbee] + [val2]
+            intervals = [i for i in intervals if len(i) > 0]
+            print(f"共{len(intervals)}个时间区间，分别是")
+            for date in intervals:
+                print(f"从{date[0]}到{date[-1]}")
+            self.dates_new_intervals = intervals
+        self.factor_new = []
+
+    def __call__(self) -> pd.DataFrame:
+        """获得经运算产生的因子
+
+        Returns
+        -------
+        `pd.DataFrame`
+            经运算产生的因子值
+        """
+        return self.factor.copy()
+
+    def forward_dates(self, dates, many_days):
+        dates_index = [self.dates_all.index(i) for i in dates]
+
+        def value(x, a):
+            if x >= 0:
+                return a[x]
+            else:
+                return None
+
+        return [value(i - many_days, self.dates_all) for i in dates_index]
+
+    def select_one_calculate(
+        self,
+        date: pd.Timestamp,
+        func: Callable,
+        fields: str = "*",
+    ) -> None:
+        the_func = partial(func)
+        if not isinstance(date, int):
+            date = int(datetime.datetime.strftime(date, "%Y%m%d"))
+        # 开始计算因子值
+
+        sql_order = f"select {fields} from second_data.second_data_stock_10s where toYYYYMMDD(date)=date order by code,date"
+        df = self.chc.get_data(sql_order)
+        df = ((df.set_index(["code", "date"])) / 100).reset_index()
+        df = df.groupby(self.groupby_target).apply(the_func)
+        if self.groupby_target == ["date", "code"]:
+            df = df.to_frame("fac").reset_index()
+            df.columns = ["date", "code", "fac"]
+        else:
+            df = df.reset_index()
+        if (df is not None) and (df.shape[0] > 0):
+            df = df.pivot(columns="code", index="date", values="fac")
+            df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+            to_save = df.stack().reset_index()
+            to_save.columns = ["date", "code", "fac"]
+            self.factor_steps.write_via_df(
+                to_save, self.factor_file_pinyin, tuple_col="fac"
+            )
+            return df
+
+    def select_many_calculate(
+        self,
+        dates: List[pd.Timestamp],
+        func: Callable,
+        fields: str = "*",
+        chunksize: int = 10,
+        many_days: int = 1,
+        n_jobs: int = 1,
+    ) -> None:
+        the_func = partial(func)
+        factor_new = []
+        dates = [int(datetime.datetime.strftime(i, "%Y%m%d")) for i in dates]
+        if many_days == 1:
+            # 将需要更新的日子分块，每200天一组，一起运算
+            dates_new_len = len(dates)
+            cut_points = list(range(0, dates_new_len, chunksize)) + [dates_new_len - 1]
+            if cut_points[-1] == cut_points[-2]:
+                cut_points = cut_points[:-1]
+            cuts = tuple(zip(cut_points[:-many_days], cut_points[many_days:]))
+            df_first = self.select_one_calculate(
+                date=dates[0],
+                func=func,
+                fields=fields,
+            )
+            factor_new.append(df_first)
+
+            def cal_one(date1, date2):
+                if self.clickhouse == 1:
+                    sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{dates[date1] * 100} and date<={dates[date2] * 100} order by code,date,num"
+                else:
+                    sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{dates[date1]} and cast(date as int)<={dates[date2]} order by code,date,num"
+
+                df = self.chc.get_data(sql_order)
+                if self.clickhouse == 1:
+                    df = ((df.set_index("code")) / 100).reset_index()
+                else:
+                    df.num = df.num.astype(int)
+                    df.date = df.date.astype(int)
+                    df = df.sort_values(["date", "num"])
+                df = df.groupby(self.groupby_target).apply(the_func)
+                if self.groupby_target == ["date", "code"]:
+                    df = df.to_frame("fac").reset_index()
+                    df.columns = ["date", "code", "fac"]
+                else:
+                    df = df.reset_index()
+                df = df.pivot(columns="code", index="date", values="fac")
+                df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                to_save = df.stack().reset_index()
+                to_save.columns = ["date", "code", "fac"]
+                self.factor_steps.write_via_df(
+                    to_save, self.factor_file_pinyin, tuple_col="fac"
+                )
+                return df
+
+            if n_jobs > 1:
+                with WorkerPool(n_jobs=n_jobs) as pool:
+                    factor_new_more = pool.map(cal_one, cuts, progress_bar=True)
+                factor_new = factor_new + factor_new_more
+            else:
+                # 开始计算因子值
+                for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
+                    df = cal_one(date1, date2)
+                    factor_new.append(df)
+        else:
+
+            def cal_two(date1, date2):
+                if date1 is not None:
+                    if self.clickhouse == 1:
+                        sql_order = f"select {fields} from minute_data.minute_data_{self.kind} where date>{date1*100} and date<={date2*100} order by code,date,num"
+                    else:
+                        sql_order = f"select {fields} from minute_data_{self.kind} where cast(date as int)>{date1} and cast(date as int)<={date2} order by code,date,num"
+
+                    df = self.chc.get_data(sql_order)
+                    if self.clickhouse == 1:
+                        df = ((df.set_index("code")) / 100).reset_index()
+                    else:
+                        df.num = df.num.astype(int)
+                        df.date = df.date.astype(int)
+                        df = df.sort_values(["date", "num"])
+                    if self.groupby_target == [
+                        "date",
+                        "code",
+                    ] or self.groupby_target == ["code"]:
+                        df = df.groupby(["code"]).apply(the_func).reset_index()
+                    else:
+                        df = the_func(df)
+                    df = df.assign(date=date2)
+                    df.columns = ["code", "fac", "date"]
+                    df = df.pivot(columns="code", index="date", values="fac")
+                    df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
+                    to_save = df.stack().reset_index()
+                    to_save.columns = ["date", "code", "fac"]
+                    self.factor_steps.write_via_df(
+                        to_save, self.factor_file_pinyin, tuple_col="fac"
+                    )
+                    return df
+
+            pairs = self.forward_dates(dates, many_days=many_days)
+            cuts2 = tuple(zip(pairs, dates))
+            if n_jobs > 1:
+                with WorkerPool(n_jobs=n_jobs) as pool:
+                    factor_new_more = pool.map(cal_two, cuts2, progress_bar=True)
+                factor_new = factor_new + factor_new_more
+            else:
+                # 开始计算因子值
+                for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
+                    df = cal_two(date1, date2)
+                    factor_new.append(df)
+
+        if len(factor_new) > 0:
+            factor_new = pd.concat(factor_new)
+            return factor_new
+        else:
+            return None
+
+    def select_any_calculate(
+        self,
+        dates: List[pd.Timestamp],
+        func: Callable,
+        fields: str = "*",
+        chunksize: int = 10,
+        show_time: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
+    ) -> None:
+        if len(dates) == 1 and many_days == 1:
+            res = self.select_one_calculate(
+                dates[0],
+                func=func,
+                fields=fields,
+                show_time=show_time,
+            )
+        else:
+            res = self.select_many_calculate(
+                dates=dates,
+                func=func,
+                fields=fields,
+                chunksize=chunksize,
+                show_time=show_time,
+                many_days=many_days,
+                n_jobs=n_jobs,
+            )
+        if res is not None:
+            self.factor_new.append(res)
+        return res
+
+    @staticmethod
+    def for_cross_via_str(func):
+        """返回值为两层的list，每一个里层的小list为单个股票在这一天的返回值
+        例如
+        ```python
+        return [[0.11,0.24,0.55],[2.59,1.99,0.43],[1.32,8.88,7.77]……]
+        ```
+        上例中，每个股票一天返回三个因子值，里层的list按照股票代码顺序排列"""
+
+        def full_run(df, *args, **kwargs):
+            codes = sorted(list(set(df.code)))
+            res = func(df, *args, **kwargs)
+            if isinstance(res[0], list):
+                kind = 1
+                res = [",".join(i) for i in res]
+            else:
+                kind = 0
+            df = pd.DataFrame({"code": codes, "fac": res})
+            if kind:
+                df.fac = df.fac.apply(lambda x: [float(i) for i in x.split(",")])
+            return df
+
+        return full_run
+
+    @staticmethod
+    def for_cross_via_zip(func):
+        """返回值为多个pd.Series，每个pd.Series的index为股票代码，values为单个因子值
+        例如
+        ```python
+        return (
+                    pd.Series([1.54,8.77,9.99……],index=['000001.SZ','000002.SZ','000004.SZ'……]),
+                    pd.Series([3.54,6.98,9.01……],index=['000001.SZ','000002.SZ','000004.SZ'……]),
+                )
+        ```
+        上例中，每个股票一天返回两个因子值，每个pd.Series对应一个因子值
+        """
+
+        def full_run(df, *args, **kwargs):
+            res = func(df, *args, **kwargs)
+            if isinstance(res, pd.Series):
+                res = res.reset_index()
+                res.columns = ["code", "fac"]
+                return res
+            elif isinstance(res, pd.DataFrame):
+                res.columns = [f"fac{i}" for i in range(len(res.columns))]
+                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+                res = res[["fac"]].reset_index()
+                res.columns = ["code", "fac"]
+                return res
+            elif res is None:
+                ...
+            else:
+                res = pd.concat(res, axis=1)
+                res.columns = [f"fac{i}" for i in range(len(res.columns))]
+                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+                res = res[["fac"]].reset_index()
+                res.columns = ["code", "fac"]
+                return res
+
+        return full_run
+
+    @kk.desktop_sender(title="嘿，分钟数据处理完啦～🎈")
+    def get_daily_factors(
+        self,
+        func: Callable,
+        fields: str = "*",
+        chunksize: int = 10,
+        show_time: bool = 0,
+        many_days: int = 1,
+        n_jobs: int = 1,
+    ) -> None:
+        """每次抽取chunksize天的截面上全部股票的分钟数据
+        对每天的股票的数据计算因子值
+
+        Parameters
+        ----------
+        func : Callable
+            用于计算因子值的函数
+        fields : str, optional
+            股票数据涉及到哪些字段，排除不必要的字段，可以节约读取数据的时间，形如'date,code,num,close,amount,open'
+            提取出的数据，自动按照code,date,num排序，因此code,date,num是必不可少的字段, by default "*"
+        chunksize : int, optional
+            每次读取的截面上的天数, by default 10
+        show_time : bool, optional
+            展示每次读取数据所需要的时间, by default 0
+        many_days : int, optional
+            计算某天的因子值时，需要使用之前多少天的数据
+        n_jobs : int, optional
+            并行数量，不建议设置为大于2的数，此外当此参数大于1时，请使用questdb数据库来读取分钟数据, by default 1
+        """
+        if len(self.dates_new) > 0:
+            for interval in self.dates_new_intervals:
+                df = self.select_any_calculate(
+                    dates=interval,
+                    func=func,
+                    fields=fields,
+                    chunksize=chunksize,
+                    show_time=show_time,
+                    many_days=many_days,
+                    n_jobs=n_jobs,
+                )
+            self.factor_new = pd.concat(self.factor_new)
+            # 拼接新的和旧的
+            self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
+            self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            # 存入本地
+            self.factor.to_parquet(self.factor_file)
+            logger.info(f"截止到{new_end_date}的因子值计算完了")
+            # 删除存储在questdb的中途备份数据
+            try:
+                self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+                logger.info("备份在questdb的表格已删除")
+            except Exception:
+                logger.warning("删除questdb中表格时，存在某个未知错误，请当心")
+
+        else:
+            self.factor = drop_duplicates_index(self.factor_old)
+            # 存入本地
+            self.factor.to_parquet(self.factor_file)
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
+
+    def drop_table(self):
+        """直接删除存储在questdb中的暂存数据"""
+        try:
+            self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+            logger.success(f"暂存在questdb中的数据表格'{self.factor_file_pinyin}'已经删除")
+        except Exception:
+            logger.warning(f"您要删除的表格'{self.factor_file_pinyin}'已经不存在了，请检查")
+
+
+class pure_fall_nature:
+    def __init__(
+        self,
+        factor_file: str,
+        project: str = None,
+        startdate: int = None,
+        enddate: int = None,
+        questdb_host: str = "127.0.0.1",
+        ignore_history_in_questdb: bool = 0,
+        groupby_code: bool = 1,
+    ) -> None:
+        """基于股票逐笔数据，计算因子值，每天的因子值只用到当日的数据
+
+        Parameters
+        ----------
+        factor_file : str
+            用于保存因子值的文件名，需为parquet文件，以'.parquet'结尾
+        project : str, optional
+            该因子所属项目，即子文件夹名称, by default None
+        startdate : int, optional
+            起始时间，形如20121231，为开区间, by default None
+        enddate : int, optional
+            截止时间，形如20220814，为闭区间，为空则计算到最近数据, by default None
+        questdb_host: str, optional
+            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
+        ignore_history_in_questdb : bool, optional
+            打断后重新从头计算，清除在questdb中的记录
+        groupby_target: list, optional
+            groupby计算时，分组的依据, by default ['code']
+        """
+        homeplace = HomePlace()
+        self.groupby_code = groupby_code
+        # 将计算到一半的因子，存入questdb中，避免中途被打断后重新计算，表名即为因子文件名的汉语拼音
+        pinyin = Pinyin()
+        self.factor_file_pinyin = pinyin.get_pinyin(
+            factor_file.replace(".parquet", ""), ""
+        )
+        self.factor_steps = Questdb(host=questdb_host)
+        if project is not None:
+            if not os.path.exists(homeplace.factor_data_file + project):
+                os.makedirs(homeplace.factor_data_file + project)
+            else:
+                logger.info(f"当前正在{project}项目中……")
+        else:
+            logger.warning("当前因子不属于任何项目，这将造成因子数据文件夹的混乱，不便于管理，建议指定一个项目名称")
+        # 完整的因子文件路径
+        if project is not None:
+            factor_file = homeplace.factor_data_file + project + "/" + factor_file
+        else:
+            factor_file = homeplace.factor_data_file + factor_file
+        self.factor_file = factor_file
+        # 读入之前的因子
+        if os.path.exists(factor_file):
+            factor_old = drop_duplicates_index(pd.read_parquet(self.factor_file))
+            self.factor_old = factor_old
+            # 已经算好的日子
+            dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
+            self.dates_old = dates_old
+        elif (not ignore_history_in_questdb) and self.factor_file_pinyin in list(
+            self.factor_steps.get_data("show tables").table
+        ):
+            logger.info(
+                f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，现在将读取上次的数据，继续计算"
+            )
+            factor_old = self.factor_steps.get_data_with_tuple(
+                f"select * from '{self.factor_file_pinyin}'"
+            ).drop_duplicates(subset=["date", "code"])
+            factor_old = factor_old.pivot(index="date", columns="code", values="fac")
+            factor_old = factor_old.sort_index()
+            self.factor_old = factor_old
+            # 已经算好的日子
+            dates_old = sorted(list(factor_old.index.strftime("%Y%m%d").astype(int)))
+            self.dates_old = dates_old
+        elif ignore_history_in_questdb and self.factor_file_pinyin in list(
+            self.factor_steps.get_data("show tables").table
+        ):
+            logger.info(
+                f"上次计算途中被打断，已经将数据备份在questdb数据库的表{self.factor_file_pinyin}中，但您选择重新计算，所以正在删除原来的数据，从头计算"
+            )
+            factor_old = self.factor_steps.do_order(
+                f"drop table '{self.factor_file_pinyin}'"
+            )
+            self.factor_old = None
+            self.dates_old = []
+            logger.info("删除完毕，正在重新计算")
+        else:
+            self.factor_old = None
+            self.dates_old = []
+            logger.info("这个因子以前没有，正在重新计算")
+        # 读取当前所有的日子
+        dates_all = os.listdir(homeplace.tick_by_tick_data)
+        dates_all = [i.split(".")[0] for i in dates_all if i.endswith(".parquet")]
+        dates_all = [i.replace("-", "") for i in dates_all]
+        dates_all = [int(i) for i in dates_all if "20" if i]
+        if startdate is None:
+            ...
+        else:
+            dates_all = [i for i in dates_all if i >= startdate]
+        if enddate is None:
+            ...
+        else:
+            dates_all = [i for i in dates_all if i <= enddate]
+        self.dates_all = dates_all
+        # 需要新补充的日子
+        self.dates_new = sorted([i for i in dates_all if i not in self.dates_old])
+        if len(self.dates_new) == 0:
+            ...
+        elif len(self.dates_new) == 1:
+            self.dates_new_intervals = [[pd.Timestamp(str(self.dates_new[0]))]]
+            print(f"只缺一天{self.dates_new[0]}")
+        else:
+            dates = [pd.Timestamp(str(i)) for i in self.dates_new]
+            intervals = [[]] * len(dates)
+            interbee = 0
+            intervals[0] = intervals[0] + [dates[0]]
+            for i in range(len(dates) - 1):
+                val1 = dates[i]
+                val2 = dates[i + 1]
+                if val2 - val1 < pd.Timedelta(days=30):
+                    ...
+                else:
+                    interbee = interbee + 1
+                intervals[interbee] = intervals[interbee] + [val2]
+            intervals = [i for i in intervals if len(i) > 0]
+            print(f"共{len(intervals)}个时间区间，分别是")
+            for date in intervals:
+                print(f"从{date[0]}到{date[-1]}")
+            self.dates_new_intervals = intervals
+        self.factor_new = []
+        self.age = read_daily(age=1)
+        self.state = read_daily(state=1)
+        self.closes_unadj = read_daily(close=1, unadjust=1).shift(1)
+
+    def __call__(self) -> pd.DataFrame:
+        """获得经运算产生的因子
+
+        Returns
+        -------
+        `pd.DataFrame`
+            经运算产生的因子值
+        """
+        return self.factor.copy()
+
+    def select_one_calculate(
+        self,
+        date: pd.Timestamp,
+        func: Callable,
+        resample_frequency: str = None,
+        opens_in: bool = 0,
+        highs_in: bool = 0,
+        lows_in: bool = 0,
+        moneys_in: bool = 0,
+        merge_them: bool = 0,
+    ) -> None:
+        the_func = partial(func)
+        if not isinstance(date, int):
+            date = int(datetime.datetime.strftime(date, "%Y%m%d"))
+        # 开始计算因子值
+        df = pd.read_parquet(
+            homeplace.tick_by_tick_data
+            + str(date)[:4]
+            + "-"
+            + str(date)[4:6]
+            + "-"
+            + str(date)[6:]
+            + ".parquet"
+        )
+        date = df.date.iloc[0]
+        date0 = pd.Timestamp(year=date.year, month=date.month, day=date.day)
+        age_here = self.age.loc[pd.Timestamp(pd.Timestamp(df.date.iloc[0]).date())]
+        age_here = age_here.where(age_here > 180, np.nan).dropna()
+        state_here = self.state.loc[pd.Timestamp(pd.Timestamp(df.date.iloc[0]).date())]
+        state_here = state_here.where(state_here > 0, np.nan).dropna()
+        df = df[df.code.isin(age_here.index)]
+        df = df[df.code.isin(state_here.index)]
+
+        if resample_frequency is not None:
+            date = df.date.iloc[0]
+            date0 = pd.Timestamp(year=date.year, month=date.month, day=date.day)
+            head = self.closes_unadj.loc[date0].to_frame("head_temp").T
+            df = df[df.code.isin(head.columns)]
+            price = df.drop_duplicates(subset=["code", "date"], keep="last").pivot(
+                index="date", columns="code", values="price"
+            )
+            closes = price.resample(resample_frequency).last()
+            head = head[[i for i in head.columns if i in closes.columns]]
+            price = pd.concat([head, closes])
+            closes = closes.ffill().iloc[1:, :]
+            self.closes = closes
+            names = []
+
+            if opens_in:
+                price = df.drop_duplicates(subset=["code", "date"], keep="first").pivot(
+                    index="date", columns="code", values="price"
+                )
+                opens = price.resample(resample_frequency).first()
+                opens = np.isnan(opens).replace(True, 1).replace(
+                    False, 0
+                ) * closes.shift(1) + opens.fillna(0)
+                self.opens = opens
+                names.append("open")
+            else:
+                self.opens = None
+
+            if highs_in:
+                price = (
+                    df.sort_values(["code", "date", "price"])
+                    .drop_duplicates(subset=["code", "date"], keep="last")
+                    .pivot(index="date", columns="code", values="price")
+                )
+                highs = price.resample(resample_frequency).max()
+                highs = np.isnan(highs).replace(True, 1).replace(
+                    False, 0
+                ) * closes.shift(1) + highs.fillna(0)
+                self.highs = highs
+                names.append("high")
+            else:
+                self.highs = None
+
+            if lows_in:
+                price = (
+                    df.sort_values(["code", "date", "price"])
+                    .drop_duplicates(subset=["code", "date"], keep="first")
+                    .pivot(index="date", columns="code", values="price")
+                )
+                lows = price.resample(resample_frequency).min()
+                lows = np.isnan(lows).replace(True, 1).replace(False, 0) * closes.shift(
+                    1
+                ) + lows.fillna(0)
+                self.lows = lows
+                names.append("low")
+            else:
+                self.low = None
+
+            names.append("close")
+            if moneys_in:
+                moneys = df.groupby(["code", "date"]).money.sum().reset_index()
+                moneys = moneys.pivot(index="date", columns="code", values="money")
+                moneys = moneys.resample(resample_frequency).sum().fillna(0)
+                self.moneys = moneys
+                names.append("money")
+            else:
+                self.moneys = None
+
+            if merge_them:
+                self.data = merge_many(
+                    [
+                        i
+                        for i in [
+                            self.opens,
+                            self.highs,
+                            self.lows,
+                            self.closes,
+                            self.moneys,
+                        ]
+                        if i is not None
+                    ],
+                    names,
+                )
+
+        if self.groupby_code:
+            df = df.groupby(["code"]).apply(the_func)
+        else:
+            df = the_func(df)
+            if isinstance(df, pd.DataFrame):
+                df.columns = [f"fac{i}" for i in range(len(df.columns))]
+                df = df.assign(fac=list(zip(*[df[i] for i in list(df.columns)])))
+                df = df[["fac"]]
+            elif isinstance(df, list) or isinstance(df, tuple):
+                df = pd.concat(list(df), axis=1)
+                df.columns = [f"fac{i}" for i in range(len(df.columns))]
+                df = df.assign(fac=list(zip(*[df[i] for i in list(df.columns)])))
+                df = df[["fac"]]
+        df = df.reset_index()
+        df.columns = ["code", "fac"]
+        df.insert(
+            0, "date", pd.Timestamp(year=date.year, month=date.month, day=date.day)
+        )
+        if (df is not None) and (df.shape[0] > 0):
+            self.factor_steps.write_via_df(df, self.factor_file_pinyin, tuple_col="fac")
+            df = df.pivot(columns="code", index="date", values="fac")
+            return df
+
+    @kk.desktop_sender(title="铛铛，逐笔数据处理完啦～🎈")
+    def get_daily_factors(
+        self,
+        func: Callable,
+        n_jobs: int = 1,
+        resample_frequency: str = None,
+        opens_in: bool = 0,
+        highs_in: bool = 0,
+        lows_in: bool = 0,
+        moneys_in: bool = 0,
+        merge_them: bool = 0,
+    ) -> None:
+        """每次抽取chunksize天的截面上全部股票的分钟数据
+        对每天的股票的数据计算因子值
+
+        Parameters
+        ----------
+        func : Callable
+            用于计算因子值的函数
+        n_jobs : int, optional
+            并行数量, by default 1
+        resample_frequency : str, optional
+            将逐笔数据转化为秒级或分钟频数据，可以填写要转化的频率，如'3s'（3秒数据），'1m'（1分钟数据），
+            指定此参数后，将自动生成一个self.closes的收盘价矩阵(index为时间,columns为股票代码,values为收盘价)，
+            可在循环计算的函数中使用`self.closes`来调用计算好的值, by default None
+        opens_in : bool, optional
+            在resample_frequency不为None的情况下，可以使用此参数，提前计算好开盘价矩阵(index为时间,columns为股票代码,values为开盘价)，
+            可在循环计算的函数中使用`self.opens`来调用计算好的值，by default 0
+        highs_in : bool, optional
+            在resample_frequency不为None的情况下，可以使用此参数，提前计算好最高价矩阵(index为时间,columns为股票代码,values为最高价)，
+            可在循环计算的函数中使用`self.highs`来调用计算好的值，by default 0
+        lows_in : bool, optional
+            在resample_frequency不为None的情况下，可以使用此参数，提前计算好最低价矩阵(index为时间,columns为股票代码,values为最低价)，
+            可在循环计算的函数中使用`self.lows`来调用计算好的值，by default 0
+        moneys_in : bool, optional
+            在resample_frequency不为None的情况下，可以使用此参数，提前计算好成交额矩阵(index为时间,columns为股票代码,values为成交额)，
+            可在循环计算的函数中使用`self.moneys`来调用计算好的值，by default 0
+        merge_them : bool, optional
+            在resample_frequency不为None的情况下，可以使用此参数，将计算好的因子值合并到一起，生成类似于分钟数据的sql形式，by default 0
+        """
+        if len(self.dates_new) > 0:
+            if n_jobs > 1:
+                with WorkerPool(n_jobs=n_jobs) as pool:
+                    self.factor_new = pool.map(
+                        lambda x: self.select_one_calculate(
+                            date=x,
+                            func=func,
+                            resample_frequency=resample_frequency,
+                            opens_in=opens_in,
+                            highs_in=highs_in,
+                            lows_in=lows_in,
+                            moneys_in=moneys_in,
+                            merge_them=merge_them,
+                        ),
+                        self.dates_new,
+                        progress_bar=True,
+                    )
+            else:
+                for date in tqdm.auto.tqdm(self.dates_new, "您现在处于单核运算状态，建议仅在调试时使用单核"):
+                    df = self.select_one_calculate(
+                        date=date,
+                        func=func,
+                        resample_frequency=resample_frequency,
+                        opens_in=opens_in,
+                        highs_in=highs_in,
+                        lows_in=lows_in,
+                        moneys_in=moneys_in,
+                        merge_them=merge_them,
+                    )
+                    self.factor_new.append(df)
+            # 拼接新的和旧的
+            self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
+            self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            # 存入本地
+            self.factor.to_parquet(self.factor_file)
+            logger.info(f"截止到{new_end_date}的因子值计算完了")
+            # 删除存储在questdb的中途备份数据
+            try:
+                self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+                logger.info("备份在questdb的表格已删除")
+            except Exception:
+                logger.warning("删除questdb中表格时，存在某个未知错误，请当心")
+
+        else:
+            self.factor = drop_duplicates_index(self.factor_old)
+            # 存入本地
+            self.factor.to_parquet(self.factor_file)
+            new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+            logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
+
+    def drop_table(self):
+        """直接删除存储在questdb中的暂存数据"""
+        try:
+            self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+            logger.success(f"暂存在questdb中的数据表格'{self.factor_file_pinyin}'已经删除")
+        except Exception:
+            logger.warning(f"您要删除的表格'{self.factor_file_pinyin}'已经不存在了，请检查")
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/homeplace.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 初始化时保存的路径
 """
 
-__updated__ = "2023-05-11 22:01:50"
+__updated__ = "2023-06-26 10:01:23"
 
 import os
 import pickle
 
 
 class HomePlace(object):
     """
     ```
     daily_data_file: 日频数据存放位置
     factor_data_file: （辅助、初级）因子数据存放位置
     barra_data_file: 十种常用风格因子的存放位置
     update_data_file: 更新辅助数据的存放位置
     api_token: dcube的api
     final_factor_file: 最终因子数据的存放位置
+    tick_by_tick_data: 股票逐笔数据的存放位置
     ```
     """
 
     __slots__ = [
         "daily_data_file",
         "factor_data_file",
         "barra_data_file",
         "update_data_file",
         "api_token",
         "final_factor_file",
+        'tick_by_tick_data',
     ]
 
     def __init__(self):
         user_file = os.path.expanduser("~") + "/"
         path_file = open(user_file + "paths.settings", "rb")
         paths = pickle.load(path_file)
         for k in self.__slots__:
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.9
+Version: 4.0.0
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: windows
 Provides-Extra: macos
 Provides-Extra: linux
 License-File: LICENSE
 
 # pure_ocean_breeze 
-#### **众人的因子回测框架**
+#### **众人的因子框架**
 ##### 我们的口号是：量价因子才是最牛的！
 ***
 
 ### 全新大版本📢
+* v4.0.0 — 2023.06.28
+> 因子框架4.0版本来啦！逐笔数据&任意秒级数据来啦！
+
 * v3.0.0 — 2022.08.16
+
 >回测框架3.0版本来啦！ 模块拆分&说明文档来啦！[pure_ocean_breeze说明文档](https://chen-001.github.io/pure_ocean_breeze/)
 * v2.0.0 — 2022.07.12
 >回测框架2.0版本来啦！数据库&自动更新&最终因子库功能上线啦！
 
 ### 安装&使用指南🎯
 1. 安装
 > 使用`pip install pure_ocean_breeze`命令进行安装
 2. 初始化
 >* 在初次安装框架时，请进行初始化，以将路径设置到自己的文件里
 >* 使用如下语句进行初始化
 >>```python
->>import pure_ocean_breeze.initialize.initialize
->>pure_ocean_breeze.initialize.initialize.initialize()
+>>import pure_ocean_breeze as p
+>>p.ini()
 >>```
 >* 然后根据提示进行操作即可
 >* 请注意路径不要写反斜杠\，而要写成/
 >* 经过初始化后，以后就可以直接使用，不论重启电脑或者版本升级，都不用再初始化
 >* 如果更换了数据库路径，请重新初始化
 3. 日常调用
 >* **导入框架**
```

### Comparing `pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.0/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.9/setup.py` & `pure_ocean_breeze-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-03-23 19:10:06"
+__updated__ = "2023-06-28 13:20:31"
 
 from setuptools import setup
 import setuptools
 import re
 import os
 import sys
 
@@ -13,15 +13,15 @@
 def get_version(package):
     """Return package version as listed in `__version__` in `init.py`."""
     init_py = open(os.path.join(package, "__init__.py")).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
 install_requires=[
     "numpy",
-    "pandas",
+    "pandas<=1.5.3",
     "scipy",
     "statsmodels",
     "plotly",
     "matplotlib",
     "pyarrow",
     "loguru",
     "knockknock",
```

