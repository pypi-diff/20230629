# Comparing `tmp/nimpa-2.6.0.tar.gz` & `tmp/nimpa-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimpa-2.6.0.tar", last modified: Tue Jun 20 21:27:05 2023, max compression
+gzip compressed data, was "nimpa-2.6.1.tar", last modified: Thu Jun 29 15:16:44 2023, max compression
```

## Comparing `nimpa-2.6.0.tar` & `nimpa-2.6.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.408407 nimpa-2.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.376407 nimpa-2.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-20 21:26:36.000000 nimpa-2.6.0/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-20 21:26:36.000000 nimpa-2.6.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 21:26:36.000000 nimpa-2.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 21:26:36.000000 nimpa-2.6.0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 21:26:36.000000 nimpa-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 21:26:36.000000 nimpa-2.6.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-20 21:26:36.000000 nimpa-2.6.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-20 21:27:05.408407 nimpa-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-20 21:26:36.000000 nimpa-2.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/niftypet/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/niftypet/nimpa/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 21:27:05.000000 nimpa-2.6.0/niftypet/nimpa/_dist_ver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/niftypet/nimpa/acr/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/ioaux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.380407 nimpa-2.6.0/niftypet/nimpa/acr_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.392407 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/
--rwxr-xr-x   0 runner    (1001) docker     (123)    29032 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-bone-screw.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43475 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-bottom.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    64947 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-inserts-bottoms.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    74141 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-inserts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    51732 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-lid0.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    49716 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-lid1.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    29661 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-0.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    31700 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-1.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    32804 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-2.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    54619 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-compartment.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    36432 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-screws.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.396407 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30028 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-cap.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    52702 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-inserts.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    42033 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-main.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    49854 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-rng.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.396407 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/
--rwxr-xr-x   0 runner    (1001) docker     (123)    90448 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-ends-water.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    85997 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-ends.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   104781 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-water.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    87513 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/
--rwxr-xr-x   0 runner    (1001) docker     (123)    50067 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-air-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   144632 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-bckg-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    50022 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-bone-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    50154 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-h2o-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43625 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot1-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43546 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot2-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43417 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot3-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43385 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot4-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   157319 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-insrt-bckg-sampling.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   443005 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-rods-sampling.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/auxdata/PSF-17_scl-1.npy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/auxdata/PSF-17_scl-2.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/img/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/img/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/img/signa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/conv.h
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/cuhelpers.h
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/isub.h
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/nlm.h
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/rsmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.404407 nimpa-2.6.0/niftypet/nimpa/prc/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39801 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/imio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/num.py
--rw-r--r--   0 runner    (1001) docker     (123)    55780 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/prc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40726 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/regseg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.404407 nimpa-2.6.0/niftypet/nimpa/prc/src/
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/conv.cu
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/cuhelpers.cu
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/img_module.cu
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/isub.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/nlm.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/rsmpl.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.404407 nimpa-2.6.0/nimpa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-20 21:26:36.000000 nimpa-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:27:05.408407 nimpa-2.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2664 2023-06-20 21:26:36.000000 nimpa-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.408407 nimpa-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:36.000000 nimpa-2.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-20 21:26:36.000000 nimpa-2.6.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-20 21:26:36.000000 nimpa-2.6.0/tests/test_improc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.664133 nimpa-2.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.648133 nimpa-2.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.652133 nimpa-2.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-29 15:16:21.000000 nimpa-2.6.1/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-29 15:16:21.000000 nimpa-2.6.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-29 15:16:21.000000 nimpa-2.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 15:16:21.000000 nimpa-2.6.1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-29 15:16:21.000000 nimpa-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-29 15:16:21.000000 nimpa-2.6.1/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-29 15:16:21.000000 nimpa-2.6.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-29 15:16:44.664133 nimpa-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-29 15:16:21.000000 nimpa-2.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.652133 nimpa-2.6.1/niftypet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.652133 nimpa-2.6.1/niftypet/nimpa/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 15:16:44.000000 nimpa-2.6.1/niftypet/nimpa/_dist_ver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.652133 nimpa-2.6.1/niftypet/nimpa/acr/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr/ioaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.648133 nimpa-2.6.1/niftypet/nimpa/acr_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.656133 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29032 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-bone-screw.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43475 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-bottom.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64947 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-inserts-bottoms.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    74141 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-inserts.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51732 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-lid0.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49716 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-lid1.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29661 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-0.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31700 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-1.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32804 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-2.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54619 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-compartment.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36432 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-screws.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.656133 nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30028 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-cap.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52702 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-inserts.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42033 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-main.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49854 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-rng.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.656133 nimpa-2.6.1/niftypet/nimpa/acr_design/rods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    90448 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods-ends-water.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    85997 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods-ends.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104781 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods-water.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87513 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.660133 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50067 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-air-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   144632 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-bckg-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50022 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-bone-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50154 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-h2o-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43625 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot1-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43546 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot2-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43417 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot3-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43385 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot4-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   157319 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-insrt-bckg-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   443005 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-rods-sampling.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.660133 nimpa-2.6.1/niftypet/nimpa/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/auxdata/PSF-17_scl-1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/auxdata/PSF-17_scl-2.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.660133 nimpa-2.6.1/niftypet/nimpa/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/img/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/img/signa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.660133 nimpa-2.6.1/niftypet/nimpa/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/include/conv.h
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/include/cuhelpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/include/isub.h
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/include/nlm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/include/rsmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.660133 nimpa-2.6.1/niftypet/nimpa/prc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40126 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/imio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55780 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/prc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40726 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/regseg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.664133 nimpa-2.6.1/niftypet/nimpa/prc/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/src/conv.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/src/cuhelpers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/src/img_module.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/src/isub.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/src/nlm.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-29 15:16:21.000000 nimpa-2.6.1/niftypet/nimpa/prc/src/rsmpl.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.664133 nimpa-2.6.1/nimpa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-29 15:16:44.000000 nimpa-2.6.1/nimpa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-29 15:16:44.000000 nimpa-2.6.1/nimpa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:16:44.000000 nimpa-2.6.1/nimpa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-29 15:16:44.000000 nimpa-2.6.1/nimpa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 15:16:44.000000 nimpa-2.6.1/nimpa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-29 15:16:21.000000 nimpa-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:16:44.664133 nimpa-2.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2664 2023-06-29 15:16:21.000000 nimpa-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:44.664133 nimpa-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:16:21.000000 nimpa-2.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-29 15:16:21.000000 nimpa-2.6.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-29 15:16:21.000000 nimpa-2.6.1/tests/test_improc.py
```

### Comparing `nimpa-2.6.0/.github/workflows/comment-bot.yml` & `nimpa-2.6.1/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/.github/workflows/test.yml` & `nimpa-2.6.1/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -77,10 +77,10 @@
         password: ${{ secrets.PYPI_TOKEN }}
         upload: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
     - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       name: Release
       run: |
         changelog=$(git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD)
         tag="${GITHUB_REF#refs/tags/}"
-        gh release create --title "nimpa $tag beta" --draft --notes "$changelog" "$tag" dist/${{ steps.dist.outputs.targz }} dist/${{ steps.dist.outputs.targz_asc }}
+        gh release create --title "nimpa $tag stable" --draft --notes "$changelog" "$tag" dist/${{ steps.dist.outputs.targz }} dist/${{ steps.dist.outputs.targz_asc }}
       env:
-        GH_TOKEN: ${{ github.token }}
+        GH_TOKEN: ${{ secrets.GH_TOKEN || github.token }}
```

### Comparing `nimpa-2.6.0/.pre-commit-config.yaml` & `nimpa-2.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/.zenodo.json` & `nimpa-2.6.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/LICENCE` & `nimpa-2.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/PKG-INFO` & `nimpa-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimpa
-Version: 2.6.0
+Version: 2.6.1
 Summary: CUDA-accelerated Python utilities for high-throughput neuroimage processing and analysis
 Author-email: Pawel Markiewicz <p.markiewicz@ucl.ac.uk>
 Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
 License: Apache-2.0
 Project-URL: documentation, https://niftypet.readthedocs.io
 Project-URL: repository, https://github.com/NiftyPET/NIMPA
 Project-URL: changelog, https://github.com/NiftyPET/NIMPA/releases
```

### Comparing `nimpa-2.6.0/README.rst` & `nimpa-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/CMakeLists.txt` & `nimpa-2.6.1/niftypet/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/__init__.py` & `nimpa-2.6.1/niftypet/nimpa/__init__.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr/__init__.py` & `nimpa-2.6.1/niftypet/nimpa/acr/__init__.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr/analysis.py` & `nimpa-2.6.1/niftypet/nimpa/acr/analysis.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr/ioaux.py` & `nimpa-2.6.1/niftypet/nimpa/acr/ioaux.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr/params.py` & `nimpa-2.6.1/niftypet/nimpa/acr/params.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr/proc.py` & `nimpa-2.6.1/niftypet/nimpa/acr/proc.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr/templates.py` & `nimpa-2.6.1/niftypet/nimpa/acr/templates.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-bone-screw.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-bone-screw.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-bottom.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-bottom.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-inserts-bottoms.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-inserts-bottoms.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-inserts.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-inserts.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-lid0.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-lid0.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-lid1.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-lid1.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-0.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-0.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-1.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-1.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-2.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-2.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-compartment.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-main-compartment.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-screws.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_mumap/acr-screws.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-cap.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-cap.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-inserts.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-inserts.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-main.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-main.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-rng.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/core_nac/acr-rng.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-ends-water.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods-ends-water.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-ends.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods-ends.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-water.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods-water.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/rods/acr-rods.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-air-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-air-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-bckg-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-bckg-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-bone-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-bone-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-h2o-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-h2o-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot1-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot1-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot2-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot2-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot3-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot3-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot4-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-hot4-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-insrt-bckg-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-insrt-bckg-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-rods-sampling.png` & `nimpa-2.6.1/niftypet/nimpa/acr_design/sampling/acr-rods-sampling.png`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/img/gen.py` & `nimpa-2.6.1/niftypet/nimpa/img/gen.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/img/signa.py` & `nimpa-2.6.1/niftypet/nimpa/img/signa.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/include/conv.h` & `nimpa-2.6.1/niftypet/nimpa/include/conv.h`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/include/rsmpl.h` & `nimpa-2.6.1/niftypet/nimpa/include/rsmpl.h`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/CMakeLists.txt` & `nimpa-2.6.1/niftypet/nimpa/prc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/__init__.py` & `nimpa-2.6.1/niftypet/nimpa/prc/__init__.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/imio.py` & `nimpa-2.6.1/niftypet/nimpa/prc/imio.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,20 +690,27 @@
 
         # > time of tracer administration (start)
         tinjct = None
         # > PET tracer if present
         trcr = None
         if [0x054, 0x016] in dhdr:
             trinf = dhdr[0x054, 0x016][0]
+
             if [0x018, 0x1078] in trinf:
                 val = trinf[0x018, 0x1078].value
                 if '.' in val:
                     tinjct = datetime.datetime.strptime(val, '%Y%m%d%H%M%S.%f')
                 else:
                     tinjct = datetime.datetime.strptime(val, '%Y%m%d%H%M%S')
+            elif [0x018, 0x1072] in trinf:
+                val = trinf[0x018, 0x1072].value
+                if '.' in val:
+                    tinjct = datetime.datetime.strptime(std_date + val, '%Y%m%d%H%M%S.%f')
+                else:
+                    tinjct = datetime.datetime.strptime(std_date + val, '%Y%m%d%H%M%S')
 
             if [0x018, 0x031] in trinf:
                 trcr = trinf[0x018, 0x031].value
         # --------------------------------
 
         log.debug(
             dedent('''\
```

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/num.py` & `nimpa-2.6.1/niftypet/nimpa/prc/num.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/prc.py` & `nimpa-2.6.1/niftypet/nimpa/prc/prc.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/regseg.py` & `nimpa-2.6.1/niftypet/nimpa/prc/regseg.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/src/conv.cu` & `nimpa-2.6.1/niftypet/nimpa/prc/src/conv.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/src/cuhelpers.cu` & `nimpa-2.6.1/niftypet/nimpa/prc/src/cuhelpers.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/src/img_module.cu` & `nimpa-2.6.1/niftypet/nimpa/prc/src/img_module.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/src/isub.cu` & `nimpa-2.6.1/niftypet/nimpa/prc/src/isub.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/src/nlm.cu` & `nimpa-2.6.1/niftypet/nimpa/prc/src/nlm.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/niftypet/nimpa/prc/src/rsmpl.cu` & `nimpa-2.6.1/niftypet/nimpa/prc/src/rsmpl.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/nimpa.egg-info/PKG-INFO` & `nimpa-2.6.1/nimpa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimpa
-Version: 2.6.0
+Version: 2.6.1
 Summary: CUDA-accelerated Python utilities for high-throughput neuroimage processing and analysis
 Author-email: Pawel Markiewicz <p.markiewicz@ucl.ac.uk>
 Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
 License: Apache-2.0
 Project-URL: documentation, https://niftypet.readthedocs.io
 Project-URL: repository, https://github.com/NiftyPET/NIMPA
 Project-URL: changelog, https://github.com/NiftyPET/NIMPA/releases
```

### Comparing `nimpa-2.6.0/nimpa.egg-info/SOURCES.txt` & `nimpa-2.6.1/nimpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/pyproject.toml` & `nimpa-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/setup.py` & `nimpa-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.6.0/tests/test_improc.py` & `nimpa-2.6.1/tests/test_improc.py`

 * *Files identical despite different names*

