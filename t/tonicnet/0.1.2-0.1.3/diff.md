# Comparing `tmp/tonicnet-0.1.2.tar.gz` & `tmp/tonicnet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonicnet-0.1.2.tar", max compression
+gzip compressed data, was "tonicnet-0.1.3.tar", max compression
```

## Comparing `tonicnet-0.1.2.tar` & `tonicnet-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-29 12:56:29.047282 tonicnet-0.1.2/README.md
--rw-r--r--   0        0        0      259 2023-06-29 12:56:29.047282 tonicnet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 12:56:29.047282 tonicnet-0.1.2/tonicnet/__init__.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 tonicnet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-29 13:38:02.774442 tonicnet-0.1.3/README.md
+-rw-r--r--   0        0        0      276 2023-06-29 13:38:02.774442 tonicnet-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 13:38:02.774442 tonicnet-0.1.3/tonicnet/__init__.py
+-rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 tonicnet-0.1.3/PKG-INFO
```

