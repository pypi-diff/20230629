# Comparing `tmp/climy-0.0.0.tar.gz` & `tmp/climy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climy-0.0.0.tar", max compression
+gzip compressed data, was "climy-0.1.0.tar", max compression
```

## Comparing `climy-0.0.0.tar` & `climy-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-31 11:59:05.924021 climy-0.0.0/LICENSE
--rw-r--r--   0        0        0       37 2023-06-02 10:18:51.449890 climy-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 12:04:03.762465 climy-0.0.0/climy/__init__.py
--rw-r--r--   0        0        0      394 2023-06-02 10:18:32.154542 climy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 climy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 11:59:05.924021 climy-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1236 2023-06-29 12:11:02.677187 climy-0.1.0/README.md
+-rw-r--r--   0        0        0      136 2023-06-29 11:45:06.580415 climy-0.1.0/climy/__init__.py
+-rw-r--r--   0        0        0     1107 2023-06-29 11:45:06.584415 climy-0.1.0/climy/application.py
+-rw-r--r--   0        0        0     5202 2023-06-29 11:57:03.904048 climy-0.1.0/climy/command.py
+-rw-r--r--   0        0        0       25 2023-06-16 10:11:53.677630 climy-0.1.0/climy/manager.py
+-rw-r--r--   0        0        0      922 2023-06-29 11:45:06.596415 climy-0.1.0/climy/option.py
+-rw-r--r--   0        0        0      394 2023-06-29 12:12:35.247273 climy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 climy-0.1.0/PKG-INFO
```

### Comparing `climy-0.0.0/LICENSE` & `climy-0.1.0/LICENSE`

 * *Files identical despite different names*

