# Comparing `tmp/spy-der-0.4.0.tar.gz` & `tmp/spy-der-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spy-der-0.4.0.tar", last modified: Fri Mar 17 21:44:36 2023, max compression
+gzip compressed data, was "spy-der-0.4.1.tar", last modified: Thu Jun 29 19:55:10 2023, max compression
```

## Comparing `spy-der-0.4.0.tar` & `spy-der-0.4.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.993557 spy-der-0.4.0/
--rw-r--r--   0 desh       (501) staff       (20)     1065 2021-02-20 22:41:54.000000 spy-der-0.4.0/LICENSE
--rw-r--r--   0 desh       (501) staff       (20)      107 2023-03-17 21:40:59.000000 spy-der-0.4.0/MANIFEST.in
--rw-r--r--   0 desh       (501) staff       (20)    16504 2023-03-17 21:44:36.993299 spy-der-0.4.0/PKG-INFO
--rw-r--r--   0 desh       (501) staff       (20)    14418 2023-03-17 21:28:25.000000 spy-der-0.4.0/README.md
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.975530 spy-der-0.4.0/lib/
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.975784 spy-der-0.4.0/lib/pybind11/
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.975629 spy-der-0.4.0/lib/pybind11/include/
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.984076 spy-der-0.4.0/lib/pybind11/include/pybind11/
--rw-r--r--   0 desh       (501) staff       (20)    21412 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/attr.h
--rw-r--r--   0 desh       (501) staff       (20)     6118 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 desh       (501) staff       (20)    95557 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/cast.h
--rw-r--r--   0 desh       (501) staff       (20)     8185 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 desh       (501) staff       (20)      120 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/common.h
--rw-r--r--   0 desh       (501) staff       (20)     2037 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.986155 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/
--rw-r--r--   0 desh       (501) staff       (20)    27823 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 desh       (501) staff       (20)    40452 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 desh       (501) staff       (20)     3602 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 desh       (501) staff       (20)    16397 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 desh       (501) staff       (20)    16375 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 desh       (501) staff       (20)     1486 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 desh       (501) staff       (20)    29086 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 desh       (501) staff       (20)     7843 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/embed.h
--rw-r--r--   0 desh       (501) staff       (20)     5079 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/eval.h
--rw-r--r--   0 desh       (501) staff       (20)     3709 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/functional.h
--rw-r--r--   0 desh       (501) staff       (20)     6084 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 desh       (501) staff       (20)    69310 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 desh       (501) staff       (20)     9085 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/operators.h
--rw-r--r--   0 desh       (501) staff       (20)     2049 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/options.h
--rw-r--r--   0 desh       (501) staff       (20)   111558 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 desh       (501) staff       (20)    66118 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 desh       (501) staff       (20)    14136 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/stl.h
--rw-r--r--   0 desh       (501) staff       (20)    23912 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.987379 spy-der-0.4.0/lib/pybind11/tests/
--rw-r--r--   0 desh       (501) staff       (20)    11157 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/tests/constructor_stats.h
--rw-r--r--   0 desh       (501) staff       (20)     2144 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/tests/local_bindings.h
--rw-r--r--   0 desh       (501) staff       (20)     5389 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/tests/object.h
--rw-r--r--   0 desh       (501) staff       (20)     2733 2021-02-24 23:35:35.000000 spy-der-0.4.0/lib/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 desh       (501) staff       (20)      127 2023-03-14 15:25:22.000000 spy-der-0.4.0/pyproject.toml
--rw-r--r--   0 desh       (501) staff       (20)       38 2023-03-17 21:44:36.993644 spy-der-0.4.0/setup.cfg
--rw-r--r--   0 desh       (501) staff       (20)     1698 2023-03-16 20:04:47.000000 spy-der-0.4.0/setup.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.975974 spy-der-0.4.0/src/
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.989049 spy-der-0.4.0/src/spy_der.egg-info/
--rw-r--r--   0 desh       (501) staff       (20)    16504 2023-03-17 21:44:36.000000 spy-der-0.4.0/src/spy_der.egg-info/PKG-INFO
--rw-r--r--   0 desh       (501) staff       (20)     1679 2023-03-17 21:44:36.000000 spy-der-0.4.0/src/spy_der.egg-info/SOURCES.txt
--rw-r--r--   0 desh       (501) staff       (20)        1 2023-03-17 21:44:36.000000 spy-der-0.4.0/src/spy_der.egg-info/dependency_links.txt
--rw-r--r--   0 desh       (501) staff       (20)       61 2023-03-17 21:44:36.000000 spy-der-0.4.0/src/spy_der.egg-info/entry_points.txt
--rw-r--r--   0 desh       (501) staff       (20)        1 2021-03-05 18:51:35.000000 spy-der-0.4.0/src/spy_der.egg-info/not-zip-safe
--rw-r--r--   0 desh       (501) staff       (20)       29 2023-03-17 21:44:36.000000 spy-der-0.4.0/src/spy_der.egg-info/requires.txt
--rw-r--r--   0 desh       (501) staff       (20)       15 2023-03-17 21:44:36.000000 spy-der-0.4.0/src/spy_der.egg-info/top_level.txt
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-03-17 21:44:36.992617 spy-der-0.4.0/src/spyder/
--rw-r--r--   0 desh       (501) staff       (20)     2438 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/GroupBy.h
--rw-r--r--   0 desh       (501) staff       (20)       69 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     2800 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/bindings.cc
--rw-r--r--   0 desh       (501) staff       (20)     4849 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/containers.cc
--rw-r--r--   0 desh       (501) staff       (20)     4497 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/containers.h
--rw-r--r--   0 desh       (501) staff       (20)     3847 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/der.cc
--rw-r--r--   0 desh       (501) staff       (20)     2739 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/der.h
--rw-r--r--   0 desh       (501) staff       (20)    10735 2023-03-17 21:28:25.000000 spy-der-0.4.0/src/spyder/der.py
--rw-r--r--   0 desh       (501) staff       (20)    13022 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/hungarian.cc
--rw-r--r--   0 desh       (501) staff       (20)     2373 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/hungarian.h
--rw-r--r--   0 desh       (501) staff       (20)     7928 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/utils.cc
--rw-r--r--   0 desh       (501) staff       (20)     3425 2023-03-17 14:38:14.000000 spy-der-0.4.0/src/spyder/utils.h
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.379645 spy-der-0.4.1/
+-rw-r--r--   0 desh       (501) staff       (20)     1065 2021-02-20 22:41:54.000000 spy-der-0.4.1/LICENSE
+-rw-r--r--   0 desh       (501) staff       (20)      107 2023-03-18 12:14:07.000000 spy-der-0.4.1/MANIFEST.in
+-rw-r--r--   0 desh       (501) staff       (20)    14831 2023-06-29 19:55:10.379466 spy-der-0.4.1/PKG-INFO
+-rw-r--r--   0 desh       (501) staff       (20)    14521 2023-06-29 19:51:59.000000 spy-der-0.4.1/README.md
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.369091 spy-der-0.4.1/lib/
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.369364 spy-der-0.4.1/lib/pybind11/
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.369209 spy-der-0.4.1/lib/pybind11/include/
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.374282 spy-der-0.4.1/lib/pybind11/include/pybind11/
+-rw-r--r--   0 desh       (501) staff       (20)    21412 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 desh       (501) staff       (20)     6118 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 desh       (501) staff       (20)    95557 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 desh       (501) staff       (20)     8185 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 desh       (501) staff       (20)      120 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/common.h
+-rw-r--r--   0 desh       (501) staff       (20)     2037 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.375392 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/
+-rw-r--r--   0 desh       (501) staff       (20)    27823 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 desh       (501) staff       (20)    40452 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 desh       (501) staff       (20)     3602 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 desh       (501) staff       (20)    16397 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 desh       (501) staff       (20)    16375 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 desh       (501) staff       (20)     1486 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 desh       (501) staff       (20)    29086 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 desh       (501) staff       (20)     7843 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 desh       (501) staff       (20)     5079 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 desh       (501) staff       (20)     3709 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 desh       (501) staff       (20)     6084 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 desh       (501) staff       (20)    69310 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 desh       (501) staff       (20)     9085 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 desh       (501) staff       (20)     2049 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/options.h
+-rw-r--r--   0 desh       (501) staff       (20)   111558 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 desh       (501) staff       (20)    66118 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 desh       (501) staff       (20)    14136 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 desh       (501) staff       (20)    23912 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.376212 spy-der-0.4.1/lib/pybind11/tests/
+-rw-r--r--   0 desh       (501) staff       (20)    11157 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 desh       (501) staff       (20)     2144 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/tests/local_bindings.h
+-rw-r--r--   0 desh       (501) staff       (20)     5389 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/tests/object.h
+-rw-r--r--   0 desh       (501) staff       (20)     2733 2021-02-24 23:35:35.000000 spy-der-0.4.1/lib/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 desh       (501) staff       (20)      127 2023-06-29 19:51:59.000000 spy-der-0.4.1/pyproject.toml
+-rw-r--r--   0 desh       (501) staff       (20)       38 2023-06-29 19:55:10.379690 spy-der-0.4.1/setup.cfg
+-rw-r--r--   0 desh       (501) staff       (20)     2043 2023-06-29 19:54:56.000000 spy-der-0.4.1/setup.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.369561 spy-der-0.4.1/src/
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.377221 spy-der-0.4.1/src/spy_der.egg-info/
+-rw-r--r--   0 desh       (501) staff       (20)    14831 2023-06-29 19:55:10.000000 spy-der-0.4.1/src/spy_der.egg-info/PKG-INFO
+-rw-r--r--   0 desh       (501) staff       (20)     1679 2023-06-29 19:55:10.000000 spy-der-0.4.1/src/spy_der.egg-info/SOURCES.txt
+-rw-r--r--   0 desh       (501) staff       (20)        1 2023-06-29 19:55:10.000000 spy-der-0.4.1/src/spy_der.egg-info/dependency_links.txt
+-rw-r--r--   0 desh       (501) staff       (20)       60 2023-06-29 19:55:10.000000 spy-der-0.4.1/src/spy_der.egg-info/entry_points.txt
+-rw-r--r--   0 desh       (501) staff       (20)        1 2021-03-05 18:51:35.000000 spy-der-0.4.1/src/spy_der.egg-info/not-zip-safe
+-rw-r--r--   0 desh       (501) staff       (20)      420 2023-06-29 19:55:10.000000 spy-der-0.4.1/src/spy_der.egg-info/requires.txt
+-rw-r--r--   0 desh       (501) staff       (20)       15 2023-06-29 19:55:10.000000 spy-der-0.4.1/src/spy_der.egg-info/top_level.txt
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-29 19:55:10.379244 spy-der-0.4.1/src/spyder/
+-rw-r--r--   0 desh       (501) staff       (20)     2438 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/GroupBy.h
+-rw-r--r--   0 desh       (501) staff       (20)       69 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     2800 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/bindings.cc
+-rw-r--r--   0 desh       (501) staff       (20)     4849 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/containers.cc
+-rw-r--r--   0 desh       (501) staff       (20)     4497 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/containers.h
+-rw-r--r--   0 desh       (501) staff       (20)     3847 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/der.cc
+-rw-r--r--   0 desh       (501) staff       (20)     2739 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/der.h
+-rw-r--r--   0 desh       (501) staff       (20)    10911 2023-06-29 19:51:59.000000 spy-der-0.4.1/src/spyder/der.py
+-rw-r--r--   0 desh       (501) staff       (20)    13022 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/hungarian.cc
+-rw-r--r--   0 desh       (501) staff       (20)     2373 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/hungarian.h
+-rw-r--r--   0 desh       (501) staff       (20)     7928 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/utils.cc
+-rw-r--r--   0 desh       (501) staff       (20)     3425 2023-03-17 14:38:14.000000 spy-der-0.4.1/src/spyder/utils.h
```

### Comparing `spy-der-0.4.0/LICENSE` & `spy-der-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/PKG-INFO` & `spy-der-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,235 +1,226 @@
-Metadata-Version: 2.1
-Name: spy-der
-Version: 0.4.0
-Summary: A simple Python package for fast DER computation
-Home-page: https://github.com/desh2608/spyder
-Author: Desh Raj
-Author-email: r.desh26@gmail.com
-License: UNKNOWN
-Description: <h1 align="center">SPYDER</h1>
-        
-        A simple Python package for fast DER computation.
-        
-        ## Installation
-        
-        ```shell
-        pip install spy-der
-        ```
-        
-        To install version with latest features directly from Github:
-        
-        ```shell
-        pip install git+https://github.com/desh2608/spyder.git@main
-        ```
-        
-        For development, clone this repository and run:
-        
-        ```shell
-        pip install --editable .
-        ```
-        
-        ## Usage
-        ### Compute DER for a single pair of reference and hypothesis
-        
-        ```python
-        import spyder
-        
-        # reference (ground truth)
-        ref = [("A", 0.0, 2.0), # (speaker, start, end)
-               ("B", 1.5, 3.5),
-               ("A", 4.0, 5.1)]
-        
-        # hypothesis (diarization result from your algorithm)
-        hyp = [("1", 0.0, 0.8),
-               ("2", 0.6, 2.3),
-               ("3", 2.1, 3.9),
-               ("1", 3.8, 5.2)]
-        
-        # compute DER on full recording
-        print(spyder.DER(ref, hyp))
-        # DERMetrics(duration=5.10,miss=9.80%,falarm=21.57%,conf=25.49%,der=56.86%)
-        
-        # compute DER on single-speaker regions only
-        print(spyder.DER(ref, hyp, regions="single"))
-        # DERMetrics(duration=4.10,miss=0.00%,falarm=26.83%,conf=19.51%,der=46.34%)
-        
-        # compute DER using UEM segments
-        uem = [(0.5, 5.0)]
-        print(spyder.DER(ref, hyp, uem=uem))
-        # DERMetrics(duration=4.50,miss=11.11%,falarm=22.22%,conf=26.67%,der=60.00%)
-        
-        # compute DER using collar
-        print(spyder.DER(ref, hyp, collar=0.2))
-        # DERMetrics(duration=3.10,miss=3.23%,falarm=12.90%,conf=19.35%,der=35.48%)
-        
-        # get speaker mapping between reference and hypothesis
-        metrics = spyder.DER(ref, hyp)
-        print(f"Reference speaker map: {metrics.ref_map}")
-        print(f"Hypothesis speaker map: {metrics.hyp_map}")
-        ```
-        
-        ### Compute DER for multiple pairs of reference and hypothesis
-        
-        ```python
-        import spyder
-        
-        # for multiple pairs, reference and hypothesis should be lists or dicts
-        # if lists, ref and hyp must have same length
-        
-        # reference (ground truth)
-        ref = {"uttr0":[("A", 0.0, 2.0), # (speaker, start, end)
-                        ("B", 1.5, 3.5),
-                        ("A", 4.0, 5.1)],
-               "uttr2":[("A", 0.0, 4.3), # (speaker, start, end)
-                        ("C", 6.0, 8.1),
-                        ("B", 2.0, 8.5)]}
-        
-        # hypothesis (diarization result from your algorithm)
-        hyp = {"uttr0":[("1", 0.0, 0.8),
-                        ("2", 0.6, 2.3),
-                        ("3", 2.1, 3.9),
-                        ("1", 3.8, 5.2)],
-               "uttr2":[("1", 0.0, 4.5),
-                        ("2", 2.5, 8.7)]}
-        
-        metrics = spyder.DER(ref, hyp)
-        print(metrics)
-        # {'Overall': DERMetrics(duration=18.00,miss=17.22%,falarm=8.33%,conf=7.22%,der=32.78%)}
-        
-        metrics2 = spyder.DER(ref, hyp, per_file=True, verbose=True)  # verbose=True to prints per-file results
-        ```
-        Output:
-        ```
-        Evaluated 2 recordings on `all` regions. Results:
-        ╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
-        │ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
-        ╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
-        │ uttr0       │           5.10 │   9.80% │     21.57% │  25.49% │ 56.86% │
-        ├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ uttr2       │          12.90 │  20.16% │      3.10% │   0.00% │ 23.26% │
-        ├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ Overall     │          18.00 │  17.22% │      8.33% │   7.22% │ 32.78% │
-        ╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
-        ```
-        
-        Additionally, you can provide UEM and collar parameters similar to single pair case.
-        
-        ### Compute per-file and overall DERs between reference and hypothesis RTTMs using command line tool
-        
-        Alternatively, __spyder__ can also be invoked from the command line to compute the per-file
-        and average DERs between reference and hypothesis RTTMs.
-        
-        ```shell
-        Usage: spyder [OPTIONS] REF_RTTM HYP_RTTM
-        
-        Options:
-          -u, --uem PATH                  UEM file (format: <recording_id> <channel>
-                                          <start> <end>)
-        
-          -p, --per-file                  If this flag is set, print per file results.
-                                          [default: False]
-        
-          -s, --skip-missing              Skip recordings which are missing in
-                                          hypothesis (i.e., not counted in missed
-                                          speech).  [default: False]
-        
-          -r, --regions [all|single|overlap|nonoverlap]
-                                          Only evaluate on the selected region type.
-                                          Default is all.  - all: all regions.  -
-                                          single: only single-speaker regions (ignore
-                                          silence and multiple speaker).  - overlap:
-                                          only regions with multiple speakers in the
-                                          reference.  - nonoverlap: only regions
-                                          without multiple speakers in the reference.
-                                          [default: all]
-        
-          -c, --collar FLOAT RANGE        Collar size.  [default: 0.0]
-          -m, --print-speaker-map         Print speaker mapping for reference and
-                                          hypothesis speakers.  [default: False]
-        
-          --help                          Show this message and exit.
-        ```
-        
-        Examples:
-        
-        ```shell
-        > spyder ref_rttm hyp_rttm
-        Evaluated 16 recordings on `all` regions. Results:
-        ╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
-        │ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
-        ╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
-        │ Overall     │       33952.95 │  11.48% │      2.27% │   9.81% │ 23.56% │
-        ╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
-        
-        > spyder ref_rttm hyp_rttm -r single -p -c 0.25
-        Evaluated 16 recordings on `single` regions. Results:
-        ╒═════════════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
-        │ Recording           │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
-        ╞═════════════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
-        │ EN2002a.Mix-Headset │        1032.05 │   0.00% │      2.98% │   4.97% │  7.94% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ EN2002b.Mix-Headset │         853.56 │   0.00% │      3.40% │   5.39% │  8.80% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ EN2002c.Mix-Headset │        1641.68 │   0.00% │      1.42% │   1.05% │  2.47% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ EN2002d.Mix-Headset │        1006.27 │   0.00% │      3.12% │   7.14% │ 10.26% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004a.Mix-Headset │         539.48 │   0.00% │      1.62% │   5.12% │  6.74% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004b.Mix-Headset │        1582.05 │   0.00% │      0.82% │   1.39% │  2.21% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004c.Mix-Headset │        1526.84 │   0.00% │      0.45% │   1.27% │  1.72% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004d.Mix-Headset │        1172.72 │   0.00% │      1.77% │   9.60% │ 11.37% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009a.Mix-Headset │         425.51 │   0.00% │      3.94% │   4.60% │  8.54% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009b.Mix-Headset │        1412.03 │   0.00% │      1.23% │   0.85% │  2.08% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009c.Mix-Headset │        1283.21 │   0.00% │      2.74% │   1.00% │  3.75% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009d.Mix-Headset │        1164.49 │   0.00% │      2.27% │   3.37% │  5.64% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003a.Mix-Headset │         804.27 │   0.00% │      0.00% │  11.28% │ 11.28% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003b.Mix-Headset │        1509.49 │   0.00% │      0.36% │   0.75% │  1.11% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003c.Mix-Headset │        1566.84 │   0.00% │      1.76% │   1.74% │  3.50% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003d.Mix-Headset │        1357.45 │   0.00% │      2.42% │   2.93% │  5.35% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ Overall             │       18877.94 │   0.00% │      1.72% │   3.29% │  5.01% │
-        ╘═════════════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
-        ```
-        
-        ## Why spyder?
-        
-        * __Fast:__ Implemented in pure C++, and faster than the alternatives (md-eval.pl,
-        dscore, pyannote.metrics). See this [benchmark](https://desh2608.github.io/2021-03-05-spyder/)
-        for comparisons with other tools.
-        * __Stand-alone:__ It has no dependency on any other library. We have our own
-        implementation of the Hungarian algorithm, for example, instead of using `scipy`.
-        * __Easy-to-use:__ No need to write the reference and hypothesis turns to files and
-        read md-eval output with complex regex patterns.
-        * __Overlap:__ Spyder supports overlapping speech in reference and hypothesis. In addition,
-        you can compute metrics on just the single-speaker or overlap regions by passing the
-        keyword argument `regions="single"` or `regions="overlap"`, respectively.
-        
-        
-        ## Contributing
-        
-        Contributions for core improvements or new recipes are welcome. Please run the following
-        before creating a pull request.
-        
-        ```bash
-        pre-commit install
-        pre-commit run # Running linter checks
-        ```
-        
-        
-        ## Bugs/issues
-        
-        Please raise an issue in the [issue tracker](https://github.com/desh2608/spyder/issues).
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+<h1 align="center">SPYDER</h1>
+
+A simple Python package for fast DER computation.
+
+## Installation
+
+```shell
+pip install spy-der
+```
+
+To install version with latest features directly from Github:
+
+```shell
+pip install git+https://github.com/desh2608/spyder.git@main
+```
+
+For development, clone this repository and run:
+
+```shell
+pip install --editable .
+```
+
+## Usage
+### Compute DER for a single pair of reference and hypothesis
+
+```python
+import spyder
+
+# reference (ground truth)
+ref = [("A", 0.0, 2.0), # (speaker, start, end)
+       ("B", 1.5, 3.5),
+       ("A", 4.0, 5.1)]
+
+# hypothesis (diarization result from your algorithm)
+hyp = [("1", 0.0, 0.8),
+       ("2", 0.6, 2.3),
+       ("3", 2.1, 3.9),
+       ("1", 3.8, 5.2)]
+
+# compute DER on full recording
+print(spyder.DER(ref, hyp))
+# DERMetrics(duration=5.10,miss=9.80%,falarm=21.57%,conf=25.49%,der=56.86%)
+
+# compute DER on single-speaker regions only
+print(spyder.DER(ref, hyp, regions="single"))
+# DERMetrics(duration=4.10,miss=0.00%,falarm=26.83%,conf=19.51%,der=46.34%)
+
+# compute DER using UEM segments
+uem = [(0.5, 5.0)]
+print(spyder.DER(ref, hyp, uem=uem))
+# DERMetrics(duration=4.50,miss=11.11%,falarm=22.22%,conf=26.67%,der=60.00%)
+
+# compute DER using collar
+print(spyder.DER(ref, hyp, collar=0.2))
+# DERMetrics(duration=3.10,miss=3.23%,falarm=12.90%,conf=19.35%,der=35.48%)
+
+# get speaker mapping between reference and hypothesis
+metrics = spyder.DER(ref, hyp)
+print(f"Reference speaker map: {metrics.ref_map}")
+print(f"Hypothesis speaker map: {metrics.hyp_map}")
+# Reference speaker map: {'A': '0', 'B': '1'}
+# Hypothesis speaker map: {'1': '0', '2': '2', '3': '1'}
+```
+
+### Compute DER for multiple pairs of reference and hypothesis
+
+```python
+import spyder
+
+# for multiple pairs, reference and hypothesis should be lists or dicts
+# if lists, ref and hyp must have same length
+
+# reference (ground truth)
+ref = {"uttr0":[("A", 0.0, 2.0), # (speaker, start, end)
+                ("B", 1.5, 3.5),
+                ("A", 4.0, 5.1)],
+       "uttr2":[("A", 0.0, 4.3), # (speaker, start, end)
+                ("C", 6.0, 8.1),
+                ("B", 2.0, 8.5)]}
+
+# hypothesis (diarization result from your algorithm)
+hyp = {"uttr0":[("1", 0.0, 0.8),
+                ("2", 0.6, 2.3),
+                ("3", 2.1, 3.9),
+                ("1", 3.8, 5.2)],
+       "uttr2":[("1", 0.0, 4.5),
+                ("2", 2.5, 8.7)]}
+
+metrics = spyder.DER(ref, hyp)
+print(metrics)
+# {'Overall': DERMetrics(duration=18.00,miss=17.22%,falarm=8.33%,conf=7.22%,der=32.78%)}
+
+metrics2 = spyder.DER(ref, hyp, per_file=True, verbose=True)  # verbose=True to prints per-file results
+```
+Output:
+```
+Evaluated 2 recordings on `all` regions. Results:
+╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
+│ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
+╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
+│ uttr0       │           5.10 │   9.80% │     21.57% │  25.49% │ 56.86% │
+├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ uttr2       │          12.90 │  20.16% │      3.10% │   0.00% │ 23.26% │
+├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ Overall     │          18.00 │  17.22% │      8.33% │   7.22% │ 32.78% │
+╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
+```
+
+Additionally, you can provide UEM and collar parameters similar to single pair case.
+
+### Compute per-file and overall DERs between reference and hypothesis RTTMs using command line tool
+
+Alternatively, __spyder__ can also be invoked from the command line to compute the per-file
+and average DERs between reference and hypothesis RTTMs.
+
+```shell
+Usage: spyder [OPTIONS] REF_RTTM HYP_RTTM
+
+Options:
+  -u, --uem PATH                  UEM file (format: <recording_id> <channel>
+                                  <start> <end>)
+
+  -p, --per-file                  If this flag is set, print per file results.
+                                  [default: False]
+
+  -s, --skip-missing              Skip recordings which are missing in
+                                  hypothesis (i.e., not counted in missed
+                                  speech).  [default: False]
+
+  -r, --regions [all|single|overlap|nonoverlap]
+                                  Only evaluate on the selected region type.
+                                  Default is all.  - all: all regions.  -
+                                  single: only single-speaker regions (ignore
+                                  silence and multiple speaker).  - overlap:
+                                  only regions with multiple speakers in the
+                                  reference.  - nonoverlap: only regions
+                                  without multiple speakers in the reference.
+                                  [default: all]
+
+  -c, --collar FLOAT RANGE        Collar size.  [default: 0.0]
+  -m, --print-speaker-map         Print speaker mapping for reference and
+                                  hypothesis speakers.  [default: False]
+
+  --help                          Show this message and exit.
+```
+
+Examples:
+
+```shell
+> spyder ref_rttm hyp_rttm
+Evaluated 16 recordings on `all` regions. Results:
+╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
+│ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
+╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
+│ Overall     │       33952.95 │  11.48% │      2.27% │   9.81% │ 23.56% │
+╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
+
+> spyder ref_rttm hyp_rttm -r single -p -c 0.25
+Evaluated 16 recordings on `single` regions. Results:
+╒═════════════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
+│ Recording           │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
+╞═════════════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
+│ EN2002a.Mix-Headset │        1032.05 │   0.00% │      2.98% │   4.97% │  7.94% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ EN2002b.Mix-Headset │         853.56 │   0.00% │      3.40% │   5.39% │  8.80% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ EN2002c.Mix-Headset │        1641.68 │   0.00% │      1.42% │   1.05% │  2.47% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ EN2002d.Mix-Headset │        1006.27 │   0.00% │      3.12% │   7.14% │ 10.26% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004a.Mix-Headset │         539.48 │   0.00% │      1.62% │   5.12% │  6.74% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004b.Mix-Headset │        1582.05 │   0.00% │      0.82% │   1.39% │  2.21% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004c.Mix-Headset │        1526.84 │   0.00% │      0.45% │   1.27% │  1.72% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004d.Mix-Headset │        1172.72 │   0.00% │      1.77% │   9.60% │ 11.37% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009a.Mix-Headset │         425.51 │   0.00% │      3.94% │   4.60% │  8.54% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009b.Mix-Headset │        1412.03 │   0.00% │      1.23% │   0.85% │  2.08% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009c.Mix-Headset │        1283.21 │   0.00% │      2.74% │   1.00% │  3.75% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009d.Mix-Headset │        1164.49 │   0.00% │      2.27% │   3.37% │  5.64% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003a.Mix-Headset │         804.27 │   0.00% │      0.00% │  11.28% │ 11.28% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003b.Mix-Headset │        1509.49 │   0.00% │      0.36% │   0.75% │  1.11% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003c.Mix-Headset │        1566.84 │   0.00% │      1.76% │   1.74% │  3.50% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003d.Mix-Headset │        1357.45 │   0.00% │      2.42% │   2.93% │  5.35% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ Overall             │       18877.94 │   0.00% │      1.72% │   3.29% │  5.01% │
+╘═════════════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
+```
+
+## Why spyder?
+
+* __Fast:__ Implemented in pure C++, and faster than the alternatives (md-eval.pl,
+dscore, pyannote.metrics). See this [benchmark](https://desh2608.github.io/2021-03-05-spyder/)
+for comparisons with other tools.
+* __Stand-alone:__ It has no dependency on any other library. We have our own
+implementation of the Hungarian algorithm, for example, instead of using `scipy`.
+* __Easy-to-use:__ No need to write the reference and hypothesis turns to files and
+read md-eval output with complex regex patterns.
+* __Overlap:__ Spyder supports overlapping speech in reference and hypothesis. In addition,
+you can compute metrics on just the single-speaker or overlap regions by passing the
+keyword argument `regions="single"` or `regions="overlap"`, respectively.
+
+
+## Contributing
+
+Contributions for core improvements or new recipes are welcome. Please run the following
+before creating a pull request.
+
+```bash
+pre-commit install
+pre-commit run # Running linter checks
+```
+
+
+## Bugs/issues
+
+Please raise an issue in the [issue tracker](https://github.com/desh2608/spyder/issues).
```

### Comparing `spy-der-0.4.0/README.md` & `spy-der-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: spy-der
+Version: 0.4.1
+Summary: A simple Python package for fast DER computation
+Home-page: https://github.com/desh2608/spyder
+Author: Desh Raj
+Author-email: r.desh26@gmail.com
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: all
+License-File: LICENSE
+
 <h1 align="center">SPYDER</h1>
 
 A simple Python package for fast DER computation.
 
 ## Installation
 
 ```shell
@@ -54,14 +66,16 @@
 print(spyder.DER(ref, hyp, collar=0.2))
 # DERMetrics(duration=3.10,miss=3.23%,falarm=12.90%,conf=19.35%,der=35.48%)
 
 # get speaker mapping between reference and hypothesis
 metrics = spyder.DER(ref, hyp)
 print(f"Reference speaker map: {metrics.ref_map}")
 print(f"Hypothesis speaker map: {metrics.hyp_map}")
+# Reference speaker map: {'A': '0', 'B': '1'}
+# Hypothesis speaker map: {'1': '0', '2': '2', '3': '1'}
 ```
 
 ### Compute DER for multiple pairs of reference and hypothesis
 
 ```python
 import spyder
```

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/attr.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/buffer_info.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/cast.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/chrono.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/complex.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/detail/class.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/detail/common.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/detail/descr.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/detail/init.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/detail/internals.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/detail/typeid.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/eigen.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/embed.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/eval.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/functional.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/iostream.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/numpy.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/operators.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/options.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/pybind11.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/pytypes.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/stl.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/include/pybind11/stl_bind.h` & `spy-der-0.4.1/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/tests/constructor_stats.h` & `spy-der-0.4.1/lib/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/tests/local_bindings.h` & `spy-der-0.4.1/lib/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/tests/object.h` & `spy-der-0.4.1/lib/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/lib/pybind11/tests/pybind11_tests.h` & `spy-der-0.4.1/lib/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/setup.py` & `spy-der-0.4.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pybind11 import get_cmake_dir
 
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import find_packages, setup
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
@@ -25,15 +25,26 @@
         # Example: passing in the version to the compiled code
         define_macros=[("VERSION_INFO", __version__)],
     ),
 ]
 
 long_description = open("README.md").read()
 
-install_requires = ["click>=7.0.0", "tabulate>=0.8.9"]
+install_requires = ["click>=7.0.0", "tabulate>=0.8.9", "numpy>=1.18.1"]
+tests_require = [
+    "pytest==7.1.3",
+    "pytest-forked==1.4.0",
+    "pytest-xdist==2.5.0",
+    "pytest-cov==4.0.0",
+    "flake8==5.0.4",
+    "coverage==6.5.0",
+    "black==22.3.0",
+    "isort==5.10.1",
+    "pre-commit>=2.17.0,<=2.19.0",
+]
 
 setup(
     name="spy-der",
     version=__version__,
     author="Desh Raj",
     author_email="r.desh26@gmail.com",
     url="https://github.com/desh2608/spyder",
@@ -44,9 +55,10 @@
     packages=find_packages("src"),
     ext_modules=ext_modules,
     # Currently, build_ext only provides an optional "highest supported C++
     # level" feature, but in the future it may provide more features.
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     install_requires=install_requires,
+    extras_require={"tests": tests_require, "all": install_requires + tests_require},
     entry_points={"console_scripts": ["spyder=spyder.der:compute_der_from_rttm"]},
 )
```

### Comparing `spy-der-0.4.0/src/spy_der.egg-info/PKG-INFO` & `spy-der-0.4.1/src/spy_der.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,235 +1,238 @@
 Metadata-Version: 2.1
 Name: spy-der
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple Python package for fast DER computation
 Home-page: https://github.com/desh2608/spyder
 Author: Desh Raj
 Author-email: r.desh26@gmail.com
-License: UNKNOWN
-Description: <h1 align="center">SPYDER</h1>
-        
-        A simple Python package for fast DER computation.
-        
-        ## Installation
-        
-        ```shell
-        pip install spy-der
-        ```
-        
-        To install version with latest features directly from Github:
-        
-        ```shell
-        pip install git+https://github.com/desh2608/spyder.git@main
-        ```
-        
-        For development, clone this repository and run:
-        
-        ```shell
-        pip install --editable .
-        ```
-        
-        ## Usage
-        ### Compute DER for a single pair of reference and hypothesis
-        
-        ```python
-        import spyder
-        
-        # reference (ground truth)
-        ref = [("A", 0.0, 2.0), # (speaker, start, end)
-               ("B", 1.5, 3.5),
-               ("A", 4.0, 5.1)]
-        
-        # hypothesis (diarization result from your algorithm)
-        hyp = [("1", 0.0, 0.8),
-               ("2", 0.6, 2.3),
-               ("3", 2.1, 3.9),
-               ("1", 3.8, 5.2)]
-        
-        # compute DER on full recording
-        print(spyder.DER(ref, hyp))
-        # DERMetrics(duration=5.10,miss=9.80%,falarm=21.57%,conf=25.49%,der=56.86%)
-        
-        # compute DER on single-speaker regions only
-        print(spyder.DER(ref, hyp, regions="single"))
-        # DERMetrics(duration=4.10,miss=0.00%,falarm=26.83%,conf=19.51%,der=46.34%)
-        
-        # compute DER using UEM segments
-        uem = [(0.5, 5.0)]
-        print(spyder.DER(ref, hyp, uem=uem))
-        # DERMetrics(duration=4.50,miss=11.11%,falarm=22.22%,conf=26.67%,der=60.00%)
-        
-        # compute DER using collar
-        print(spyder.DER(ref, hyp, collar=0.2))
-        # DERMetrics(duration=3.10,miss=3.23%,falarm=12.90%,conf=19.35%,der=35.48%)
-        
-        # get speaker mapping between reference and hypothesis
-        metrics = spyder.DER(ref, hyp)
-        print(f"Reference speaker map: {metrics.ref_map}")
-        print(f"Hypothesis speaker map: {metrics.hyp_map}")
-        ```
-        
-        ### Compute DER for multiple pairs of reference and hypothesis
-        
-        ```python
-        import spyder
-        
-        # for multiple pairs, reference and hypothesis should be lists or dicts
-        # if lists, ref and hyp must have same length
-        
-        # reference (ground truth)
-        ref = {"uttr0":[("A", 0.0, 2.0), # (speaker, start, end)
-                        ("B", 1.5, 3.5),
-                        ("A", 4.0, 5.1)],
-               "uttr2":[("A", 0.0, 4.3), # (speaker, start, end)
-                        ("C", 6.0, 8.1),
-                        ("B", 2.0, 8.5)]}
-        
-        # hypothesis (diarization result from your algorithm)
-        hyp = {"uttr0":[("1", 0.0, 0.8),
-                        ("2", 0.6, 2.3),
-                        ("3", 2.1, 3.9),
-                        ("1", 3.8, 5.2)],
-               "uttr2":[("1", 0.0, 4.5),
-                        ("2", 2.5, 8.7)]}
-        
-        metrics = spyder.DER(ref, hyp)
-        print(metrics)
-        # {'Overall': DERMetrics(duration=18.00,miss=17.22%,falarm=8.33%,conf=7.22%,der=32.78%)}
-        
-        metrics2 = spyder.DER(ref, hyp, per_file=True, verbose=True)  # verbose=True to prints per-file results
-        ```
-        Output:
-        ```
-        Evaluated 2 recordings on `all` regions. Results:
-        ╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
-        │ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
-        ╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
-        │ uttr0       │           5.10 │   9.80% │     21.57% │  25.49% │ 56.86% │
-        ├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ uttr2       │          12.90 │  20.16% │      3.10% │   0.00% │ 23.26% │
-        ├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ Overall     │          18.00 │  17.22% │      8.33% │   7.22% │ 32.78% │
-        ╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
-        ```
-        
-        Additionally, you can provide UEM and collar parameters similar to single pair case.
-        
-        ### Compute per-file and overall DERs between reference and hypothesis RTTMs using command line tool
-        
-        Alternatively, __spyder__ can also be invoked from the command line to compute the per-file
-        and average DERs between reference and hypothesis RTTMs.
-        
-        ```shell
-        Usage: spyder [OPTIONS] REF_RTTM HYP_RTTM
-        
-        Options:
-          -u, --uem PATH                  UEM file (format: <recording_id> <channel>
-                                          <start> <end>)
-        
-          -p, --per-file                  If this flag is set, print per file results.
-                                          [default: False]
-        
-          -s, --skip-missing              Skip recordings which are missing in
-                                          hypothesis (i.e., not counted in missed
-                                          speech).  [default: False]
-        
-          -r, --regions [all|single|overlap|nonoverlap]
-                                          Only evaluate on the selected region type.
-                                          Default is all.  - all: all regions.  -
-                                          single: only single-speaker regions (ignore
-                                          silence and multiple speaker).  - overlap:
-                                          only regions with multiple speakers in the
-                                          reference.  - nonoverlap: only regions
-                                          without multiple speakers in the reference.
-                                          [default: all]
-        
-          -c, --collar FLOAT RANGE        Collar size.  [default: 0.0]
-          -m, --print-speaker-map         Print speaker mapping for reference and
-                                          hypothesis speakers.  [default: False]
-        
-          --help                          Show this message and exit.
-        ```
-        
-        Examples:
-        
-        ```shell
-        > spyder ref_rttm hyp_rttm
-        Evaluated 16 recordings on `all` regions. Results:
-        ╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
-        │ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
-        ╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
-        │ Overall     │       33952.95 │  11.48% │      2.27% │   9.81% │ 23.56% │
-        ╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
-        
-        > spyder ref_rttm hyp_rttm -r single -p -c 0.25
-        Evaluated 16 recordings on `single` regions. Results:
-        ╒═════════════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
-        │ Recording           │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
-        ╞═════════════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
-        │ EN2002a.Mix-Headset │        1032.05 │   0.00% │      2.98% │   4.97% │  7.94% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ EN2002b.Mix-Headset │         853.56 │   0.00% │      3.40% │   5.39% │  8.80% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ EN2002c.Mix-Headset │        1641.68 │   0.00% │      1.42% │   1.05% │  2.47% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ EN2002d.Mix-Headset │        1006.27 │   0.00% │      3.12% │   7.14% │ 10.26% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004a.Mix-Headset │         539.48 │   0.00% │      1.62% │   5.12% │  6.74% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004b.Mix-Headset │        1582.05 │   0.00% │      0.82% │   1.39% │  2.21% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004c.Mix-Headset │        1526.84 │   0.00% │      0.45% │   1.27% │  1.72% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ ES2004d.Mix-Headset │        1172.72 │   0.00% │      1.77% │   9.60% │ 11.37% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009a.Mix-Headset │         425.51 │   0.00% │      3.94% │   4.60% │  8.54% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009b.Mix-Headset │        1412.03 │   0.00% │      1.23% │   0.85% │  2.08% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009c.Mix-Headset │        1283.21 │   0.00% │      2.74% │   1.00% │  3.75% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ IS1009d.Mix-Headset │        1164.49 │   0.00% │      2.27% │   3.37% │  5.64% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003a.Mix-Headset │         804.27 │   0.00% │      0.00% │  11.28% │ 11.28% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003b.Mix-Headset │        1509.49 │   0.00% │      0.36% │   0.75% │  1.11% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003c.Mix-Headset │        1566.84 │   0.00% │      1.76% │   1.74% │  3.50% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ TS3003d.Mix-Headset │        1357.45 │   0.00% │      2.42% │   2.93% │  5.35% │
-        ├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
-        │ Overall             │       18877.94 │   0.00% │      1.72% │   3.29% │  5.01% │
-        ╘═════════════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
-        ```
-        
-        ## Why spyder?
-        
-        * __Fast:__ Implemented in pure C++, and faster than the alternatives (md-eval.pl,
-        dscore, pyannote.metrics). See this [benchmark](https://desh2608.github.io/2021-03-05-spyder/)
-        for comparisons with other tools.
-        * __Stand-alone:__ It has no dependency on any other library. We have our own
-        implementation of the Hungarian algorithm, for example, instead of using `scipy`.
-        * __Easy-to-use:__ No need to write the reference and hypothesis turns to files and
-        read md-eval output with complex regex patterns.
-        * __Overlap:__ Spyder supports overlapping speech in reference and hypothesis. In addition,
-        you can compute metrics on just the single-speaker or overlap regions by passing the
-        keyword argument `regions="single"` or `regions="overlap"`, respectively.
-        
-        
-        ## Contributing
-        
-        Contributions for core improvements or new recipes are welcome. Please run the following
-        before creating a pull request.
-        
-        ```bash
-        pre-commit install
-        pre-commit run # Running linter checks
-        ```
-        
-        
-        ## Bugs/issues
-        
-        Please raise an issue in the [issue tracker](https://github.com/desh2608/spyder/issues).
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: all
+License-File: LICENSE
+
+<h1 align="center">SPYDER</h1>
+
+A simple Python package for fast DER computation.
+
+## Installation
+
+```shell
+pip install spy-der
+```
+
+To install version with latest features directly from Github:
+
+```shell
+pip install git+https://github.com/desh2608/spyder.git@main
+```
+
+For development, clone this repository and run:
+
+```shell
+pip install --editable .
+```
+
+## Usage
+### Compute DER for a single pair of reference and hypothesis
+
+```python
+import spyder
+
+# reference (ground truth)
+ref = [("A", 0.0, 2.0), # (speaker, start, end)
+       ("B", 1.5, 3.5),
+       ("A", 4.0, 5.1)]
+
+# hypothesis (diarization result from your algorithm)
+hyp = [("1", 0.0, 0.8),
+       ("2", 0.6, 2.3),
+       ("3", 2.1, 3.9),
+       ("1", 3.8, 5.2)]
+
+# compute DER on full recording
+print(spyder.DER(ref, hyp))
+# DERMetrics(duration=5.10,miss=9.80%,falarm=21.57%,conf=25.49%,der=56.86%)
+
+# compute DER on single-speaker regions only
+print(spyder.DER(ref, hyp, regions="single"))
+# DERMetrics(duration=4.10,miss=0.00%,falarm=26.83%,conf=19.51%,der=46.34%)
+
+# compute DER using UEM segments
+uem = [(0.5, 5.0)]
+print(spyder.DER(ref, hyp, uem=uem))
+# DERMetrics(duration=4.50,miss=11.11%,falarm=22.22%,conf=26.67%,der=60.00%)
+
+# compute DER using collar
+print(spyder.DER(ref, hyp, collar=0.2))
+# DERMetrics(duration=3.10,miss=3.23%,falarm=12.90%,conf=19.35%,der=35.48%)
+
+# get speaker mapping between reference and hypothesis
+metrics = spyder.DER(ref, hyp)
+print(f"Reference speaker map: {metrics.ref_map}")
+print(f"Hypothesis speaker map: {metrics.hyp_map}")
+# Reference speaker map: {'A': '0', 'B': '1'}
+# Hypothesis speaker map: {'1': '0', '2': '2', '3': '1'}
+```
+
+### Compute DER for multiple pairs of reference and hypothesis
+
+```python
+import spyder
+
+# for multiple pairs, reference and hypothesis should be lists or dicts
+# if lists, ref and hyp must have same length
+
+# reference (ground truth)
+ref = {"uttr0":[("A", 0.0, 2.0), # (speaker, start, end)
+                ("B", 1.5, 3.5),
+                ("A", 4.0, 5.1)],
+       "uttr2":[("A", 0.0, 4.3), # (speaker, start, end)
+                ("C", 6.0, 8.1),
+                ("B", 2.0, 8.5)]}
+
+# hypothesis (diarization result from your algorithm)
+hyp = {"uttr0":[("1", 0.0, 0.8),
+                ("2", 0.6, 2.3),
+                ("3", 2.1, 3.9),
+                ("1", 3.8, 5.2)],
+       "uttr2":[("1", 0.0, 4.5),
+                ("2", 2.5, 8.7)]}
+
+metrics = spyder.DER(ref, hyp)
+print(metrics)
+# {'Overall': DERMetrics(duration=18.00,miss=17.22%,falarm=8.33%,conf=7.22%,der=32.78%)}
+
+metrics2 = spyder.DER(ref, hyp, per_file=True, verbose=True)  # verbose=True to prints per-file results
+```
+Output:
+```
+Evaluated 2 recordings on `all` regions. Results:
+╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
+│ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
+╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
+│ uttr0       │           5.10 │   9.80% │     21.57% │  25.49% │ 56.86% │
+├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ uttr2       │          12.90 │  20.16% │      3.10% │   0.00% │ 23.26% │
+├─────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ Overall     │          18.00 │  17.22% │      8.33% │   7.22% │ 32.78% │
+╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
+```
+
+Additionally, you can provide UEM and collar parameters similar to single pair case.
+
+### Compute per-file and overall DERs between reference and hypothesis RTTMs using command line tool
+
+Alternatively, __spyder__ can also be invoked from the command line to compute the per-file
+and average DERs between reference and hypothesis RTTMs.
+
+```shell
+Usage: spyder [OPTIONS] REF_RTTM HYP_RTTM
+
+Options:
+  -u, --uem PATH                  UEM file (format: <recording_id> <channel>
+                                  <start> <end>)
+
+  -p, --per-file                  If this flag is set, print per file results.
+                                  [default: False]
+
+  -s, --skip-missing              Skip recordings which are missing in
+                                  hypothesis (i.e., not counted in missed
+                                  speech).  [default: False]
+
+  -r, --regions [all|single|overlap|nonoverlap]
+                                  Only evaluate on the selected region type.
+                                  Default is all.  - all: all regions.  -
+                                  single: only single-speaker regions (ignore
+                                  silence and multiple speaker).  - overlap:
+                                  only regions with multiple speakers in the
+                                  reference.  - nonoverlap: only regions
+                                  without multiple speakers in the reference.
+                                  [default: all]
+
+  -c, --collar FLOAT RANGE        Collar size.  [default: 0.0]
+  -m, --print-speaker-map         Print speaker mapping for reference and
+                                  hypothesis speakers.  [default: False]
+
+  --help                          Show this message and exit.
+```
+
+Examples:
+
+```shell
+> spyder ref_rttm hyp_rttm
+Evaluated 16 recordings on `all` regions. Results:
+╒═════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
+│ Recording   │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
+╞═════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
+│ Overall     │       33952.95 │  11.48% │      2.27% │   9.81% │ 23.56% │
+╘═════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
+
+> spyder ref_rttm hyp_rttm -r single -p -c 0.25
+Evaluated 16 recordings on `single` regions. Results:
+╒═════════════════════╤════════════════╤═════════╤════════════╤═════════╤════════╕
+│ Recording           │   Duration (s) │   Miss. │   F.Alarm. │   Conf. │    DER │
+╞═════════════════════╪════════════════╪═════════╪════════════╪═════════╪════════╡
+│ EN2002a.Mix-Headset │        1032.05 │   0.00% │      2.98% │   4.97% │  7.94% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ EN2002b.Mix-Headset │         853.56 │   0.00% │      3.40% │   5.39% │  8.80% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ EN2002c.Mix-Headset │        1641.68 │   0.00% │      1.42% │   1.05% │  2.47% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ EN2002d.Mix-Headset │        1006.27 │   0.00% │      3.12% │   7.14% │ 10.26% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004a.Mix-Headset │         539.48 │   0.00% │      1.62% │   5.12% │  6.74% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004b.Mix-Headset │        1582.05 │   0.00% │      0.82% │   1.39% │  2.21% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004c.Mix-Headset │        1526.84 │   0.00% │      0.45% │   1.27% │  1.72% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ ES2004d.Mix-Headset │        1172.72 │   0.00% │      1.77% │   9.60% │ 11.37% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009a.Mix-Headset │         425.51 │   0.00% │      3.94% │   4.60% │  8.54% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009b.Mix-Headset │        1412.03 │   0.00% │      1.23% │   0.85% │  2.08% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009c.Mix-Headset │        1283.21 │   0.00% │      2.74% │   1.00% │  3.75% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ IS1009d.Mix-Headset │        1164.49 │   0.00% │      2.27% │   3.37% │  5.64% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003a.Mix-Headset │         804.27 │   0.00% │      0.00% │  11.28% │ 11.28% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003b.Mix-Headset │        1509.49 │   0.00% │      0.36% │   0.75% │  1.11% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003c.Mix-Headset │        1566.84 │   0.00% │      1.76% │   1.74% │  3.50% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ TS3003d.Mix-Headset │        1357.45 │   0.00% │      2.42% │   2.93% │  5.35% │
+├─────────────────────┼────────────────┼─────────┼────────────┼─────────┼────────┤
+│ Overall             │       18877.94 │   0.00% │      1.72% │   3.29% │  5.01% │
+╘═════════════════════╧════════════════╧═════════╧════════════╧═════════╧════════╛
+```
+
+## Why spyder?
+
+* __Fast:__ Implemented in pure C++, and faster than the alternatives (md-eval.pl,
+dscore, pyannote.metrics). See this [benchmark](https://desh2608.github.io/2021-03-05-spyder/)
+for comparisons with other tools.
+* __Stand-alone:__ It has no dependency on any other library. We have our own
+implementation of the Hungarian algorithm, for example, instead of using `scipy`.
+* __Easy-to-use:__ No need to write the reference and hypothesis turns to files and
+read md-eval output with complex regex patterns.
+* __Overlap:__ Spyder supports overlapping speech in reference and hypothesis. In addition,
+you can compute metrics on just the single-speaker or overlap regions by passing the
+keyword argument `regions="single"` or `regions="overlap"`, respectively.
+
+
+## Contributing
+
+Contributions for core improvements or new recipes are welcome. Please run the following
+before creating a pull request.
+
+```bash
+pre-commit install
+pre-commit run # Running linter checks
+```
+
+
+## Bugs/issues
+
+Please raise an issue in the [issue tracker](https://github.com/desh2608/spyder/issues).
```

### Comparing `spy-der-0.4.0/src/spy_der.egg-info/SOURCES.txt` & `spy-der-0.4.1/src/spy_der.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/GroupBy.h` & `spy-der-0.4.1/src/spyder/GroupBy.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/bindings.cc` & `spy-der-0.4.1/src/spyder/bindings.cc`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/containers.cc` & `spy-der-0.4.1/src/spyder/containers.cc`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/containers.h` & `spy-der-0.4.1/src/spyder/containers.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/der.cc` & `spy-der-0.4.1/src/spyder/der.cc`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/der.h` & `spy-der-0.4.1/src/spyder/der.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/der.py` & `spy-der-0.4.1/src/spyder/der.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     ref,
     hyp,
     uem=None,
     per_file=False,
     skip_missing=False,
     regions="all",
     collar=0.0,
+    print_speaker_map=False,
     verbose=False,
 ):
     """
     Compute DER between ref and hyp.
     The following formats are supported for `ref` and `hyp`:
         - list of tuples: list of turns of single recording
         - dict: {recording_id: list of turns}
@@ -186,15 +187,23 @@
             - hyp_map: Speaker map from hypothesis to common labels.
     """
     if uem is None:
         uem = get_uem_turns(ref, hyp)
     if isinstance(ref, dict) and isinstance(hyp, dict):
         assert isinstance(uem, dict), "UEM must be dict if ref and hyp are dict"
         metrics = _DER_multi(
-            ref, hyp, uem, per_file, skip_missing, regions, collar, verbose
+            ref,
+            hyp,
+            uem,
+            per_file,
+            skip_missing,
+            regions,
+            collar,
+            print_speaker_map,
+            verbose,
         )
     elif np.ndim(ref[-1]) == 2 and np.ndim(hyp[-1]) == 2:
         # the first dimension is the number of utterances
         # in this case ref and hyp must have same length
         if len(ref) != len(hyp):
             raise ValueError("if ref and hyp are not dict, they must have same length")
 
@@ -209,14 +218,15 @@
             ref_turns,
             hyp_turns,
             uem_turns,
             per_file,
             skip_missing,
             regions,
             collar,
+            print_speaker_map,
             verbose,
         )
     elif np.ndim(ref[-1]) == 1 and np.ndim(hyp[-1]) == 1:
         assert isinstance(uem, list), "UEM must be list if ref and hyp are list"
         # only one utterance
         metrics = _DER(ref, hyp, uem, regions, collar)
         if verbose:
```

### Comparing `spy-der-0.4.0/src/spyder/hungarian.cc` & `spy-der-0.4.1/src/spyder/hungarian.cc`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/hungarian.h` & `spy-der-0.4.1/src/spyder/hungarian.h`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/utils.cc` & `spy-der-0.4.1/src/spyder/utils.cc`

 * *Files identical despite different names*

### Comparing `spy-der-0.4.0/src/spyder/utils.h` & `spy-der-0.4.1/src/spyder/utils.h`

 * *Files identical despite different names*

