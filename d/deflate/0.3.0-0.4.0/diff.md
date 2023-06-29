# Comparing `tmp/deflate-0.3.0.tar.gz` & `tmp/deflate-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deflate-0.3.0.tar", last modified: Mon Dec 14 20:41:59 2020, max compression
+gzip compressed data, was "deflate-0.4.0.tar", last modified: Thu Jun 29 16:09:17 2023, max compression
```

## Comparing `deflate-0.3.0.tar` & `deflate-0.4.0.tar`

### file list

```diff
@@ -1,113 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-12-14 20:41:56.000000 deflate-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      800 2020-12-14 20:41:59.531224 deflate-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      421 2020-12-14 20:41:56.000000 deflate-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     4070 2020-12-14 20:41:56.000000 deflate-0.3.0/deflate.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.519224 deflate-0.3.0/deflate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      800 2020-12-14 20:41:59.000000 deflate-0.3.0/deflate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3121 2020-12-14 20:41:59.000000 deflate-0.3.0/deflate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-14 20:41:59.000000 deflate-0.3.0/deflate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-14 20:41:59.000000 deflate-0.3.0/deflate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.523224 deflate-0.3.0/libdeflate/
--rw-r--r--   0 runner    (1001) docker     (116)      185 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (116)       35 2020-12-14 20:41:56.000000 deflate-0.3.0/libdeflate/.git
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     2434 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1052 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/COPYING
--rw-r--r--   0 runner    (1001) docker     (116)    12072 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     1370 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (116)     6789 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/NEWS
--rw-r--r--   0 runner    (1001) docker     (116)    12148 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.523224 deflate-0.3.0/libdeflate/common/
--rw-r--r--   0 runner    (1001) docker     (116)     9618 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/common/common_defs.h
--rw-r--r--   0 runner    (1001) docker     (116)     6858 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/common/compiler_gcc.h
--rw-r--r--   0 runner    (1001) docker     (116)     1629 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/common/compiler_msc.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.527224 deflate-0.3.0/libdeflate/lib/
--rw-r--r--   0 runner    (1001) docker     (116)     3638 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (116)     3918 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/adler32_vec_template.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.527224 deflate-0.3.0/libdeflate/lib/arm/
--rw-r--r--   0 runner    (1001) docker     (116)     4427 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/arm/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)     3738 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/arm/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (116)      860 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/arm/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (116)     7501 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/arm/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)     2727 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/arm/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)    12154 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/bt_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (116)     2602 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/cpu_features_common.h
--rw-r--r--   0 runner    (1001) docker     (116)    10495 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (116)    25448 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/crc32_table.h
--rw-r--r--   0 runner    (1001) docker     (116)     2114 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/crc32_vec_template.h
--rw-r--r--   0 runner    (1001) docker     (116)    12768 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/decompress_template.h
--rw-r--r--   0 runner    (1001) docker     (116)    94567 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/deflate_compress.c
--rw-r--r--   0 runner    (1001) docker     (116)      392 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/deflate_compress.h
--rw-r--r--   0 runner    (1001) docker     (116)     2243 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/deflate_constants.h
--rw-r--r--   0 runner    (1001) docker     (116)    38908 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/deflate_decompress.c
--rw-r--r--   0 runner    (1001) docker     (116)     2818 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/gzip_compress.c
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/gzip_constants.h
--rw-r--r--   0 runner    (1001) docker     (116)     4128 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/gzip_decompress.c
--rw-r--r--   0 runner    (1001) docker     (116)    14244 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/hc_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (116)     2548 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/lib_common.h
--rw-r--r--   0 runner    (1001) docker     (116)     5012 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/matchfinder_common.h
--rw-r--r--   0 runner    (1001) docker     (116)     5645 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/unaligned.h
--rw-r--r--   0 runner    (1001) docker     (116)     3193 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.527224 deflate-0.3.0/libdeflate/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (116)    12049 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)     4567 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (116)      931 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (116)     3139 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)    10451 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/crc32_pclmul_template.h
--rw-r--r--   0 runner    (1001) docker     (116)      625 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/decompress_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)     3630 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/x86/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)     2771 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/zlib_compress.c
--rw-r--r--   0 runner    (1001) docker     (116)      488 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/zlib_constants.h
--rw-r--r--   0 runner    (1001) docker     (116)     3270 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/lib/zlib_decompress.c
--rw-r--r--   0 runner    (1001) docker     (116)    15152 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/libdeflate.h
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.527224 deflate-0.3.0/libdeflate/programs/
--rw-r--r--   0 runner    (1001) docker     (116)    17372 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/benchmark.c
--rw-r--r--   0 runner    (1001) docker     (116)     4605 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/checksum.c
--rw-r--r--   0 runner    (1001) docker     (116)    15983 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/gzip.c
--rw-r--r--   0 runner    (1001) docker     (116)    11265 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/prog_util.c
--rw-r--r--   0 runner    (1001) docker     (116)     4720 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/prog_util.h
--rw-r--r--   0 runner    (1001) docker     (116)     5012 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_checksums.c
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_custom_malloc.c
--rw-r--r--   0 runner    (1001) docker     (116)    11890 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_incomplete_codes.c
--rw-r--r--   0 runner    (1001) docker     (116)     2207 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_litrunlen_overflow.c
--rw-r--r--   0 runner    (1001) docker     (116)    22742 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_slow_decompression.c
--rw-r--r--   0 runner    (1001) docker     (116)     5221 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_trailing_bytes.c
--rw-r--r--   0 runner    (1001) docker     (116)     5695 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_util.c
--rw-r--r--   0 runner    (1001) docker     (116)     2127 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/test_util.h
--rw-r--r--   0 runner    (1001) docker     (116)     3530 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/programs/tgetopt.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/
--rw-r--r--   0 runner    (1001) docker     (116)      154 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_compress/
--rw-r--r--   0 runner    (1001) docker     (116)      921 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_compress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_compress/inputs/
--rw-r--r--   0 runner    (1001) docker     (116)      500 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_compress/inputs/0
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_decompress/
--rw-r--r--   0 runner    (1001) docker     (116)      573 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_decompress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/
--rw-r--r--   0 runner    (1001) docker     (116)      169 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/0
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/gzip_decompress/
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/gzip_decompress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/
--rw-r--r--   0 runner    (1001) docker     (116)      187 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/0
--rwxr-xr-x   0 runner    (1001) docker     (116)      251 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/prepare_for_fuzz.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/zlib_decompress/
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/zlib_decompress/fuzz.c
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-14 20:41:59.531224 deflate-0.3.0/libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/
--rw-r--r--   0 runner    (1001) docker     (116)      175 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/0
--rwxr-xr-x   0 runner    (1001) docker     (116)     1894 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/android_build.sh
--rw-r--r--   0 runner    (1001) docker     (116)     1832 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/android_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)     3374 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/checksum_benchmarks.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)     1512 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/detect.sh
--rw-r--r--   0 runner    (1001) docker     (116)      662 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/exec_tests.sh
--rw-r--r--   0 runner    (1001) docker     (116)     3637 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/gen_crc32_multipliers.c
--rw-r--r--   0 runner    (1001) docker     (116)     3230 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/gen_crc32_table.c
--rwxr-xr-x   0 runner    (1001) docker     (116)    10805 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/gzip_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      600 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/make-windows-releases.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)       75 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/msc_test.bat
--rwxr-xr-x   0 runner    (1001) docker     (116)      617 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/pgo_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      845 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/produce_gzip_benchmark_table.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)     7849 2020-12-14 20:41:57.000000 deflate-0.3.0/libdeflate/scripts/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-14 20:41:59.531224 deflate-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1228 2020-12-14 20:41:56.000000 deflate-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 16:09:14.000000 deflate-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 16:09:14.000000 deflate-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-29 16:09:17.369842 deflate-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-29 16:09:14.000000 deflate-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-29 16:09:14.000000 deflate-0.4.0/deflate.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.357842 deflate-0.4.0/deflate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-29 16:09:17.000000 deflate-0.4.0/deflate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-29 16:09:17.000000 deflate-0.4.0/deflate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:09:17.000000 deflate-0.4.0/deflate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 16:09:17.000000 deflate-0.4.0/deflate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.357842 deflate-0.4.0/libdeflate/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 16:09:15.000000 deflate-0.4.0/libdeflate/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.357842 deflate-0.4.0/libdeflate/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.361842 deflate-0.4.0/libdeflate/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    15586 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/common_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.361842 deflate-0.4.0/libdeflate/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/adler32_vec_template.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.361842 deflate-0.4.0/libdeflate/lib/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/crc32_pmull_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/crc32_pmull_wide.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/arm/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/bt_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/cpu_features_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/crc32_multipliers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28471 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/crc32_tables.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/decompress_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)   135284 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/deflate_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/deflate_compress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/deflate_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47754 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/deflate_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/gzip_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/gzip_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/gzip_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/hc_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/ht_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/lib_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/matchfinder_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.361842 deflate-0.4.0/libdeflate/lib/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/crc32_pclmul_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/decompress_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/x86/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/zlib_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/zlib_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/lib/zlib_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/libdeflate-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/libdeflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/libdeflate.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.365842 deflate-0.4.0/libdeflate/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/checksum.c
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/gzip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/prog_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/prog_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_checksums.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_custom_malloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_incomplete_codes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_invalid_streams.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_litrunlen_overflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_overread.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22742 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_slow_decompression.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_trailing_bytes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/test_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/programs/tgetopt.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.365842 deflate-0.4.0/libdeflate/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/android_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1994 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/android_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      247 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/benchmark.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      245 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/checksum.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3379 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/checksum_benchmarks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      471 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/cmake-helper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/deflate_benchmarks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/exec_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/gen_bitreverse_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/gen_crc32_multipliers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/gen_crc32_tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/gen_default_litlen_costs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/gen_offset_slot_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11897 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/gzip_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_compress/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_decompress/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_decompress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/deflate_decompress/fuzz.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1608 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/fuzz.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/gzip_decompress/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/gzip_decompress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/gzip_decompress/fuzz.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/zlib_decompress/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:09:17.369842 deflate-0.4.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/zlib_decompress/corpus/0
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/libFuzzer/zlib_decompress/fuzz.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/make-windows-releases.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9314 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-29 16:09:16.000000 deflate-0.4.0/libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 16:09:17.369842 deflate-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-29 16:09:14.000000 deflate-0.4.0/setup.py
```

### Comparing `deflate-0.3.0/deflate.c` & `deflate-0.4.0/deflate.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,164 @@
 #define PY_SSIZE_T_CLEAN
+#include "libdeflate.h"
 #include <Python.h>
-#include "libdeflate/libdeflate.h"
+
+#define MODULE_VERSION "0.4.0"
 
 static PyObject *DeflateError;
 
-static PyObject *deflate_gzip_compress(PyObject *self, PyObject *args, PyObject *kwargs)
-{
+static PyObject *deflate_gzip_compress(PyObject *self, PyObject *args,
+                                       PyObject *kwargs) {
     static char *keywords[] = {"data", "compresslevel", NULL};
     Py_buffer data;
     int compression_level = 6;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i", keywords, &data, &compression_level))
-    {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*|i", keywords, &data,
+                                     &compression_level)) {
         return NULL;
     }
 
-    if (compression_level < 1 || compression_level > 12)
-    {
+    if (compression_level < 1 || compression_level > 12) {
         PyBuffer_Release(&data);
         PyErr_SetString(PyExc_ValueError, "compresslevel must be between 1 and 12.");
         return NULL;
     }
 
-    struct libdeflate_compressor *compressor = libdeflate_alloc_compressor(compression_level);
+    struct libdeflate_compressor *compressor =
+        libdeflate_alloc_compressor(compression_level);
     size_t bound = libdeflate_gzip_compress_bound(compressor, data.len);
-    void *compressed_data = PyMem_RawMalloc(bound);
-    if (compressed_data == NULL)
-    {
+
+    PyObject *bytes = PyBytes_FromStringAndSize(NULL, bound);
+    if (bytes == NULL) {
         libdeflate_free_compressor(compressor);
         PyBuffer_Release(&data);
         return PyErr_NoMemory();
     }
-    size_t compressed_size = libdeflate_gzip_compress(compressor, data.buf, data.len, compressed_data, bound);
+
+    size_t compressed_size = libdeflate_gzip_compress(compressor, data.buf, data.len,
+                                                      PyBytes_AsString(bytes), bound);
     libdeflate_free_compressor(compressor);
+    PyBuffer_Release(&data);
 
-    if (compressed_size == 0)
-    {
-        PyMem_RawFree(compressed_data);
-        PyBuffer_Release(&data);
+    if (compressed_size == 0) {
+        Py_DECREF(bytes);
         PyErr_SetString(DeflateError, "Compression failed.");
         return NULL;
     }
 
-    PyObject *bytes = PyBytes_FromStringAndSize(compressed_data, compressed_size);
-    PyMem_RawFree(compressed_data);
-    PyBuffer_Release(&data);
+    _PyBytes_Resize(&bytes, compressed_size);
 
     return bytes;
 }
 
-static PyObject *deflate_gzip_decompress(PyObject *self, PyObject *args)
-{
+static PyObject *deflate_gzip_decompress(PyObject *self, PyObject *args) {
     Py_buffer data;
 
-    if (!PyArg_ParseTuple(args, "y*", &data))
-    {
+    if (!PyArg_ParseTuple(args, "y*", &data)) {
         return NULL;
     }
 
-    if (data.len < 6)
-    {
+    if (data.len < 6) {
         PyErr_SetString(DeflateError, "Invalid gzip data.");
         PyBuffer_Release(&data);
         return NULL;
     }
 
     // Very basic gzip header check before we go allocating memory.
     uint8_t *bytes = (uint8_t *)data.buf;
-    if (bytes[0] != 0x1F || bytes[1] != 0x8B)
-    {
+    if (bytes[0] != 0x1F || bytes[1] != 0x8B) {
         PyErr_SetString(DeflateError, "Invalid gzip data.");
         PyBuffer_Release(&data);
         return NULL;
     }
 
-    // The last 4 bytes of a gzip archive are the original data size, in little endian.
+    // The last 4 bytes of a gzip archive are the original data size, in little
+    // endian.
     bytes = (uint8_t *)data.buf + (data.len - 4);
-    uint32_t size = (bytes[0] << 0) | (bytes[1] << 8) | (bytes[2] << 16) | (bytes[3] << 24);
+    uint32_t size =
+        (bytes[0] << 0) | (bytes[1] << 8) | (bytes[2] << 16) | (bytes[3] << 24);
     // TODO: upper bound on decompression size?
 
-    size_t decompressed_size;
-    void *decompressed_data = PyMem_RawMalloc(size);
-    if (decompressed_data == NULL)
+    PyObject *output = PyBytes_FromStringAndSize(NULL, size);
+    if (output == NULL) {
+        PyBuffer_Release(&data);
         return PyErr_NoMemory();
+    }
+
+    size_t decompressed_size;
     struct libdeflate_decompressor *decompressor = libdeflate_alloc_decompressor();
-    enum libdeflate_result result = libdeflate_gzip_decompress(
-        decompressor, data.buf, data.len, decompressed_data, size, &decompressed_size);
+    enum libdeflate_result result =
+        libdeflate_gzip_decompress(decompressor, data.buf, data.len,
+                                   PyBytes_AsString(output), size, &decompressed_size);
     libdeflate_free_decompressor(decompressor);
 
-    PyObject *output = NULL;
+    // Resize the bytes object to the decompressed size and release the input buffer.
+    _PyBytes_Resize(&output, decompressed_size);
+    PyBuffer_Release(&data);
 
-    switch (result)
-    {
-    case LIBDEFLATE_SUCCESS:
-        output = PyBytes_FromStringAndSize(decompressed_data, decompressed_size);
-        PyMem_RawFree(decompressed_data);
-        PyBuffer_Release(&data);
-        break;
-    default:
-        PyMem_RawFree(decompressed_data);
-        PyBuffer_Release(&data);
+    if (result != LIBDEFLATE_SUCCESS) {
+        Py_DECREF(output);
         PyErr_SetString(DeflateError, "Decompression failed.");
+        return NULL;
     }
 
     return output;
 }
 
+static PyObject *deflate_crc32(PyObject *self, PyObject *args) {
+    Py_buffer data;
+    unsigned int crc = 0;
+
+    if (!PyArg_ParseTuple(args, "y*|I", &data, &crc)) {
+        return NULL;
+    }
+
+    crc = libdeflate_crc32(crc, data.buf, data.len);
+    PyBuffer_Release(&data);
+
+    return Py_BuildValue("I", crc);
+}
+
+static PyObject *deflate_adler32(PyObject *self, PyObject *args) {
+    Py_buffer data;
+    unsigned int adler = 1;
+
+    if (!PyArg_ParseTuple(args, "y*|I", &data, &adler)) {
+        return NULL;
+    }
+
+    adler = libdeflate_adler32(adler, data.buf, data.len);
+    PyBuffer_Release(&data);
+
+    return Py_BuildValue("I", adler);
+}
+
 static PyMethodDef deflate_methods[] = {
-    {"gzip_compress", (PyCFunction)deflate_gzip_compress, METH_VARARGS | METH_KEYWORDS, "Compress data using gzip."},
-    {"gzip_decompress", (PyCFunction)deflate_gzip_decompress, METH_VARARGS, "Decompress gzip data."},
+    {"gzip_compress", (PyCFunction)deflate_gzip_compress, METH_VARARGS | METH_KEYWORDS,
+     "Compress data using gzip."},
+    {"gzip_decompress", (PyCFunction)deflate_gzip_decompress, METH_VARARGS,
+     "Decompress gzip data."},
+    {"crc32", (PyCFunction)deflate_crc32, METH_VARARGS,
+     "CRC32 algorithm from libdeflate"},
+    {"adler32", (PyCFunction)deflate_adler32, METH_VARARGS,
+     "adler32 algorithm from libdeflate"},
     {NULL, NULL, 0, NULL}};
 
-static struct PyModuleDef deflate_module = {
-    PyModuleDef_HEAD_INIT,
-    "deflate",
-    "Python wrapper module for libdeflate.",
-    -1,
-    deflate_methods};
+static struct PyModuleDef deflate_module = {PyModuleDef_HEAD_INIT, "deflate",
+                                            "Python wrapper module for libdeflate.", -1,
+                                            deflate_methods};
 
-PyMODINIT_FUNC PyInit_deflate(void)
-{
+PyMODINIT_FUNC PyInit_deflate(void) {
     Py_Initialize();
 
     PyObject *module = PyModule_Create(&deflate_module);
     if (module == NULL)
         return NULL;
 
+    PyModule_AddStringConstant(module, "__version__", MODULE_VERSION);
+
     DeflateError = PyErr_NewException("deflate.DeflateError", NULL, NULL);
     Py_INCREF(DeflateError);
+    PyModule_AddObject(module, "DeflateError", DeflateError);
 
     return module;
 }
```

### Comparing `deflate-0.3.0/deflate.egg-info/SOURCES.txt` & `deflate-0.4.0/deflate.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,105 @@
+LICENSE
 MANIFEST.in
 README.md
 deflate.c
+setup.cfg
 setup.py
 deflate.egg-info/PKG-INFO
 deflate.egg-info/SOURCES.txt
 deflate.egg-info/dependency_links.txt
 deflate.egg-info/top_level.txt
 libdeflate/.cirrus.yml
 libdeflate/.git
 libdeflate/.gitignore
-libdeflate/.travis.yml
+libdeflate/CMakeLists.txt
 libdeflate/COPYING
-libdeflate/Makefile
-libdeflate/Makefile.msc
-libdeflate/NEWS
+libdeflate/NEWS.md
 libdeflate/README.md
+libdeflate/common_defs.h
+libdeflate/libdeflate-config.cmake.in
 libdeflate/libdeflate.h
-libdeflate/common/common_defs.h
-libdeflate/common/compiler_gcc.h
-libdeflate/common/compiler_msc.h
+libdeflate/libdeflate.pc.in
+libdeflate/.github/workflows/ci.yml
 libdeflate/lib/adler32.c
 libdeflate/lib/adler32_vec_template.h
 libdeflate/lib/bt_matchfinder.h
 libdeflate/lib/cpu_features_common.h
 libdeflate/lib/crc32.c
-libdeflate/lib/crc32_table.h
-libdeflate/lib/crc32_vec_template.h
+libdeflate/lib/crc32_multipliers.h
+libdeflate/lib/crc32_tables.h
 libdeflate/lib/decompress_template.h
 libdeflate/lib/deflate_compress.c
 libdeflate/lib/deflate_compress.h
 libdeflate/lib/deflate_constants.h
 libdeflate/lib/deflate_decompress.c
 libdeflate/lib/gzip_compress.c
 libdeflate/lib/gzip_constants.h
 libdeflate/lib/gzip_decompress.c
 libdeflate/lib/hc_matchfinder.h
+libdeflate/lib/ht_matchfinder.h
 libdeflate/lib/lib_common.h
 libdeflate/lib/matchfinder_common.h
-libdeflate/lib/unaligned.h
 libdeflate/lib/utils.c
 libdeflate/lib/zlib_compress.c
 libdeflate/lib/zlib_constants.h
 libdeflate/lib/zlib_decompress.c
 libdeflate/lib/arm/adler32_impl.h
 libdeflate/lib/arm/cpu_features.c
 libdeflate/lib/arm/cpu_features.h
 libdeflate/lib/arm/crc32_impl.h
+libdeflate/lib/arm/crc32_pmull_helpers.h
+libdeflate/lib/arm/crc32_pmull_wide.h
 libdeflate/lib/arm/matchfinder_impl.h
 libdeflate/lib/x86/adler32_impl.h
 libdeflate/lib/x86/cpu_features.c
 libdeflate/lib/x86/cpu_features.h
 libdeflate/lib/x86/crc32_impl.h
 libdeflate/lib/x86/crc32_pclmul_template.h
 libdeflate/lib/x86/decompress_impl.h
 libdeflate/lib/x86/matchfinder_impl.h
+libdeflate/programs/CMakeLists.txt
 libdeflate/programs/benchmark.c
 libdeflate/programs/checksum.c
+libdeflate/programs/config.h.in
 libdeflate/programs/gzip.c
 libdeflate/programs/prog_util.c
 libdeflate/programs/prog_util.h
 libdeflate/programs/test_checksums.c
 libdeflate/programs/test_custom_malloc.c
 libdeflate/programs/test_incomplete_codes.c
+libdeflate/programs/test_invalid_streams.c
 libdeflate/programs/test_litrunlen_overflow.c
+libdeflate/programs/test_overread.c
 libdeflate/programs/test_slow_decompression.c
 libdeflate/programs/test_trailing_bytes.c
 libdeflate/programs/test_util.c
 libdeflate/programs/test_util.h
 libdeflate/programs/tgetopt.c
 libdeflate/scripts/android_build.sh
 libdeflate/scripts/android_tests.sh
+libdeflate/scripts/benchmark.sh
+libdeflate/scripts/checksum.sh
 libdeflate/scripts/checksum_benchmarks.sh
-libdeflate/scripts/detect.sh
+libdeflate/scripts/cmake-helper.sh
+libdeflate/scripts/deflate_benchmarks.sh
 libdeflate/scripts/exec_tests.sh
+libdeflate/scripts/gen_bitreverse_tab.py
 libdeflate/scripts/gen_crc32_multipliers.c
-libdeflate/scripts/gen_crc32_table.c
+libdeflate/scripts/gen_crc32_tables.c
+libdeflate/scripts/gen_default_litlen_costs.py
+libdeflate/scripts/gen_offset_slot_map.py
 libdeflate/scripts/gzip_tests.sh
 libdeflate/scripts/make-windows-releases.sh
-libdeflate/scripts/msc_test.bat
-libdeflate/scripts/pgo_build.sh
-libdeflate/scripts/produce_gzip_benchmark_table.sh
 libdeflate/scripts/run_tests.sh
-libdeflate/scripts/afl-fuzz/Makefile
-libdeflate/scripts/afl-fuzz/prepare_for_fuzz.sh
-libdeflate/scripts/afl-fuzz/deflate_compress/fuzz.c
-libdeflate/scripts/afl-fuzz/deflate_compress/inputs/0
-libdeflate/scripts/afl-fuzz/deflate_decompress/fuzz.c
-libdeflate/scripts/afl-fuzz/deflate_decompress/inputs/0
-libdeflate/scripts/afl-fuzz/gzip_decompress/fuzz.c
-libdeflate/scripts/afl-fuzz/gzip_decompress/inputs/0
-libdeflate/scripts/afl-fuzz/zlib_decompress/fuzz.c
-libdeflate/scripts/afl-fuzz/zlib_decompress/inputs/0
+libdeflate/scripts/toolchain-i686-w64-mingw32.cmake
+libdeflate/scripts/toolchain-x86_64-w64-mingw32.cmake
+libdeflate/scripts/libFuzzer/.gitignore
+libdeflate/scripts/libFuzzer/fuzz.sh
+libdeflate/scripts/libFuzzer/deflate_compress/fuzz.c
+libdeflate/scripts/libFuzzer/deflate_compress/corpus/0
+libdeflate/scripts/libFuzzer/deflate_decompress/fuzz.c
+libdeflate/scripts/libFuzzer/deflate_decompress/corpus/0
+libdeflate/scripts/libFuzzer/gzip_decompress/fuzz.c
+libdeflate/scripts/libFuzzer/gzip_decompress/corpus/0
+libdeflate/scripts/libFuzzer/zlib_decompress/fuzz.c
+libdeflate/scripts/libFuzzer/zlib_decompress/corpus/0
```

### Comparing `deflate-0.3.0/libdeflate/COPYING` & `deflate-0.4.0/libdeflate/COPYING`

 * *Files identical despite different names*

### Comparing `deflate-0.3.0/libdeflate/lib/adler32.c` & `deflate-0.4.0/libdeflate/lib/adler32.c`

 * *Files 17% similar despite different names*

```diff
@@ -22,23 +22,22 @@
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "lib_common.h"
-#include "libdeflate.h"
 
-/* The Adler-32 divisor, or "base", value. */
+/* The Adler-32 divisor, or "base", value */
 #define DIVISOR 65521
 
 /*
- * MAX_CHUNK_SIZE is the most bytes that can be processed without the
- * possibility of s2 overflowing when it is represented as an unsigned 32-bit
- * integer.  This value was computed using the following Python script:
+ * MAX_CHUNK_LEN is the most bytes that can be processed without the possibility
+ * of s2 overflowing when it is represented as an unsigned 32-bit integer.  This
+ * value was computed using the following Python script:
  *
  *	divisor = 65521
  *	count = 0
  *	s1 = divisor - 1
  *	s2 = divisor - 1
  *	while True:
  *		s1 += 0xFF
@@ -48,40 +47,27 @@
  *		count += 1
  *	print(count)
  *
  * Note that to get the correct worst-case value, we must assume that every byte
  * has value 0xFF and that s1 and s2 started with the highest possible values
  * modulo the divisor.
  */
-#define MAX_CHUNK_SIZE	5552
+#define MAX_CHUNK_LEN	5552
 
-typedef u32 (*adler32_func_t)(u32, const u8 *, size_t);
-
-/* Include architecture-specific implementations if available */
-#undef DEFAULT_IMPL
-#undef DISPATCH
-#if defined(__arm__) || defined(__aarch64__)
-#  include "arm/adler32_impl.h"
-#elif defined(__i386__) || defined(__x86_64__)
-#  include "x86/adler32_impl.h"
-#endif
-
-/* Define a generic implementation if needed */
-#ifndef DEFAULT_IMPL
-#define DEFAULT_IMPL adler32_generic
-static u32 adler32_generic(u32 adler, const u8 *p, size_t size)
+static u32 MAYBE_UNUSED
+adler32_generic(u32 adler, const u8 *p, size_t len)
 {
 	u32 s1 = adler & 0xFFFF;
 	u32 s2 = adler >> 16;
-	const u8 * const end = p + size;
+	const u8 * const end = p + len;
 
 	while (p != end) {
-		size_t chunk_size = MIN(end - p, MAX_CHUNK_SIZE);
-		const u8 *chunk_end = p + chunk_size;
-		size_t num_unrolled_iterations = chunk_size / 4;
+		size_t chunk_len = MIN(end - p, MAX_CHUNK_LEN);
+		const u8 *chunk_end = p + chunk_len;
+		size_t num_unrolled_iterations = chunk_len / 4;
 
 		while (num_unrolled_iterations--) {
 			s1 += *p++;
 			s2 += s1;
 			s1 += *p++;
 			s2 += s1;
 			s1 += *p++;
@@ -95,36 +81,50 @@
 		}
 		s1 %= DIVISOR;
 		s2 %= DIVISOR;
 	}
 
 	return (s2 << 16) | s1;
 }
-#endif /* !DEFAULT_IMPL */
 
-#ifdef DISPATCH
-static u32 dispatch(u32, const u8 *, size_t);
+/* Include architecture-specific implementation(s) if available. */
+#undef DEFAULT_IMPL
+#undef arch_select_adler32_func
+typedef u32 (*adler32_func_t)(u32 adler, const u8 *p, size_t len);
+#if defined(ARCH_ARM32) || defined(ARCH_ARM64)
+#  include "arm/adler32_impl.h"
+#elif defined(ARCH_X86_32) || defined(ARCH_X86_64)
+#  include "x86/adler32_impl.h"
+#endif
+
+#ifndef DEFAULT_IMPL
+#  define DEFAULT_IMPL adler32_generic
+#endif
+
+#ifdef arch_select_adler32_func
+static u32 dispatch_adler32(u32 adler, const u8 *p, size_t len);
 
-static volatile adler32_func_t adler32_impl = dispatch;
+static volatile adler32_func_t adler32_impl = dispatch_adler32;
 
-/* Choose the fastest implementation at runtime */
-static u32 dispatch(u32 adler, const u8 *buffer, size_t size)
+/* Choose the best implementation at runtime. */
+static u32 dispatch_adler32(u32 adler, const u8 *p, size_t len)
 {
 	adler32_func_t f = arch_select_adler32_func();
 
 	if (f == NULL)
 		f = DEFAULT_IMPL;
 
 	adler32_impl = f;
-	return adler32_impl(adler, buffer, size);
+	return f(adler, p, len);
 }
 #else
-#  define adler32_impl DEFAULT_IMPL /* only one implementation, use it */
+/* The best implementation is statically known, so call it directly. */
+#define adler32_impl DEFAULT_IMPL
 #endif
 
-LIBDEFLATEEXPORT u32 LIBDEFLATEAPI
-libdeflate_adler32(u32 adler, const void *buffer, size_t size)
+LIBDEFLATEAPI u32
+libdeflate_adler32(u32 adler, const void *buffer, size_t len)
 {
-	if (buffer == NULL) /* return initial value */
+	if (buffer == NULL) /* Return initial value. */
 		return 1;
-	return adler32_impl(adler, buffer, size);
+	return adler32_impl(adler, buffer, len);
 }
```

### Comparing `deflate-0.3.0/libdeflate/lib/adler32_vec_template.h` & `deflate-0.4.0/libdeflate/lib/adler32_vec_template.h`

 * *Files 8% similar despite different names*

```diff
@@ -55,59 +55,58 @@
  *
  *	s2 += s1 * N
  *
  * Furthermore, like s1, "s2" can actually be multiple counters which are
  * eventually summed together.
  */
 
-static u32 ATTRIBUTES
-FUNCNAME(u32 adler, const u8 *p, size_t size)
+static u32 ATTRIBUTES MAYBE_UNUSED
+FUNCNAME(u32 adler, const u8 *p, size_t len)
 {
+	const size_t max_chunk_len =
+		MIN(MAX_CHUNK_LEN, IMPL_MAX_CHUNK_LEN) -
+		(MIN(MAX_CHUNK_LEN, IMPL_MAX_CHUNK_LEN) % IMPL_SEGMENT_LEN);
 	u32 s1 = adler & 0xFFFF;
 	u32 s2 = adler >> 16;
-	const u8 * const end = p + size;
+	const u8 * const end = p + len;
 	const u8 *vend;
-	const size_t max_chunk_size =
-		MIN(MAX_CHUNK_SIZE, IMPL_MAX_CHUNK_SIZE) -
-		(MIN(MAX_CHUNK_SIZE, IMPL_MAX_CHUNK_SIZE) %
-		 IMPL_SEGMENT_SIZE);
 
-	/* Process a byte at a time until the needed alignment is reached */
+	/* Process a byte at a time until the needed alignment is reached. */
 	if (p != end && (uintptr_t)p % IMPL_ALIGNMENT) {
 		do {
 			s1 += *p++;
 			s2 += s1;
 		} while (p != end && (uintptr_t)p % IMPL_ALIGNMENT);
 		s1 %= DIVISOR;
 		s2 %= DIVISOR;
 	}
 
 	/*
-	 * Process "chunks" of bytes using vector instructions.  Chunk sizes are
-	 * limited to MAX_CHUNK_SIZE, which guarantees that s1 and s2 never
+	 * Process "chunks" of bytes using vector instructions.  Chunk lengths
+	 * are limited to MAX_CHUNK_LEN, which guarantees that s1 and s2 never
 	 * overflow before being reduced modulo DIVISOR.  For vector processing,
-	 * chunk sizes are also made evenly divisible by IMPL_SEGMENT_SIZE and
-	 * may be further limited to IMPL_MAX_CHUNK_SIZE.
+	 * chunk lengths are also made evenly divisible by IMPL_SEGMENT_LEN and
+	 * may be further limited to IMPL_MAX_CHUNK_LEN.
 	 */
-	STATIC_ASSERT(IMPL_SEGMENT_SIZE % IMPL_ALIGNMENT == 0);
-	vend = end - ((size_t)(end - p) % IMPL_SEGMENT_SIZE);
+	STATIC_ASSERT(IMPL_SEGMENT_LEN % IMPL_ALIGNMENT == 0);
+	vend = end - ((size_t)(end - p) % IMPL_SEGMENT_LEN);
 	while (p != vend) {
-		size_t chunk_size = MIN((size_t)(vend - p), max_chunk_size);
+		size_t chunk_len = MIN((size_t)(vend - p), max_chunk_len);
 
-		s2 += s1 * chunk_size;
+		s2 += s1 * chunk_len;
 
-		FUNCNAME_CHUNK((const void *)p, (const void *)(p + chunk_size),
+		FUNCNAME_CHUNK((const void *)p, (const void *)(p + chunk_len),
 			       &s1, &s2);
 
-		p += chunk_size;
+		p += chunk_len;
 		s1 %= DIVISOR;
 		s2 %= DIVISOR;
 	}
 
-	/* Process any remaining bytes */
+	/* Process any remaining bytes. */
 	if (p != end) {
 		do {
 			s1 += *p++;
 			s2 += s1;
 		} while (p != end);
 		s1 %= DIVISOR;
 		s2 %= DIVISOR;
@@ -116,9 +115,9 @@
 	return (s2 << 16) | s1;
 }
 
 #undef FUNCNAME
 #undef FUNCNAME_CHUNK
 #undef ATTRIBUTES
 #undef IMPL_ALIGNMENT
-#undef IMPL_SEGMENT_SIZE
-#undef IMPL_MAX_CHUNK_SIZE
+#undef IMPL_SEGMENT_LEN
+#undef IMPL_MAX_CHUNK_LEN
```

### Comparing `deflate-0.3.0/libdeflate/lib/bt_matchfinder.h` & `deflate-0.4.0/libdeflate/lib/bt_matchfinder.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * bt_matchfinder.h - Lempel-Ziv matchfinding with a hash table of binary trees
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -60,14 +58,16 @@
  * need matches.  Generally, when doing fast compression on small buffers,
  * binary trees are the wrong approach.  They are best suited for thorough
  * compression and/or large buffers.
  *
  * ----------------------------------------------------------------------------
  */
 
+#ifndef LIB_BT_MATCHFINDER_H
+#define LIB_BT_MATCHFINDER_H
 
 #include "matchfinder_common.h"
 
 #define BT_MATCHFINDER_HASH3_ORDER 16
 #define BT_MATCHFINDER_HASH3_WAYS  2
 #define BT_MATCHFINDER_HASH4_ORDER 16
 
@@ -81,33 +81,28 @@
 	/* The number of bytes matched.  */
 	u16 length;
 
 	/* The offset back from the current position that was matched.  */
 	u16 offset;
 };
 
-struct bt_matchfinder {
+struct MATCHFINDER_ALIGNED bt_matchfinder {
 
 	/* The hash table for finding length 3 matches  */
 	mf_pos_t hash3_tab[1UL << BT_MATCHFINDER_HASH3_ORDER][BT_MATCHFINDER_HASH3_WAYS];
 
 	/* The hash table which contains the roots of the binary trees for
 	 * finding length 4+ matches  */
 	mf_pos_t hash4_tab[1UL << BT_MATCHFINDER_HASH4_ORDER];
 
 	/* The child node references for the binary trees.  The left and right
 	 * children of the node for the sequence with position 'pos' are
 	 * 'child_tab[pos * 2]' and 'child_tab[pos * 2 + 1]', respectively.  */
 	mf_pos_t child_tab[2UL * MATCHFINDER_WINDOW_SIZE];
-
-}
-#ifdef _aligned_attribute
-_aligned_attribute(MATCHFINDER_MEM_ALIGNMENT)
-#endif
-;
+};
 
 /* Prepare the matchfinder for a new input buffer.  */
 static forceinline void
 bt_matchfinder_init(struct bt_matchfinder *mf)
 {
 	STATIC_ASSERT(BT_MATCHFINDER_TOTAL_HASH_SIZE %
 		      MATCHFINDER_SIZE_ALIGNMENT == 0);
@@ -132,30 +127,29 @@
 static forceinline mf_pos_t *
 bt_right_child(struct bt_matchfinder *mf, s32 node)
 {
 	return &mf->child_tab[2 * (node & (MATCHFINDER_WINDOW_SIZE - 1)) + 1];
 }
 
 /* The minimum permissible value of 'max_len' for bt_matchfinder_get_matches()
- * and bt_matchfinder_skip_position().  There must be sufficiently many bytes
+ * and bt_matchfinder_skip_byte().  There must be sufficiently many bytes
  * remaining to load a 32-bit integer from the *next* position.  */
 #define BT_MATCHFINDER_REQUIRED_NBYTES	5
 
 /* Advance the binary tree matchfinder by one byte, optionally recording
  * matches.  @record_matches should be a compile-time constant.  */
 static forceinline struct lz_match *
-bt_matchfinder_advance_one_byte(struct bt_matchfinder * const restrict mf,
-				const u8 * const restrict in_base,
+bt_matchfinder_advance_one_byte(struct bt_matchfinder * const mf,
+				const u8 * const in_base,
 				const ptrdiff_t cur_pos,
 				const u32 max_len,
 				const u32 nice_len,
 				const u32 max_search_depth,
-				u32 * const restrict next_hashes,
-				u32 * const restrict best_len_ret,
-				struct lz_match * restrict lz_matchptr,
+				u32 * const next_hashes,
+				struct lz_match *lz_matchptr,
 				const bool record_matches)
 {
 	const u8 *in_next = in_base + cur_pos;
 	u32 depth_remaining = max_search_depth;
 	const s32 cutoff = cur_pos - MATCHFINDER_WINDOW_SIZE;
 	u32 next_hashseq;
 	u32 hash3;
@@ -212,15 +206,14 @@
 
 	pending_lt_ptr = bt_left_child(mf, cur_pos);
 	pending_gt_ptr = bt_right_child(mf, cur_pos);
 
 	if (cur_node <= cutoff) {
 		*pending_lt_ptr = MATCHFINDER_INITVAL;
 		*pending_gt_ptr = MATCHFINDER_INITVAL;
-		*best_len_ret = best_len;
 		return lz_matchptr;
 	}
 
 	best_lt_len = 0;
 	best_gt_len = 0;
 	len = 0;
 
@@ -235,15 +228,14 @@
 					lz_matchptr->length = len;
 					lz_matchptr->offset = in_next - matchptr;
 					lz_matchptr++;
 				}
 				if (len >= nice_len) {
 					*pending_lt_ptr = *bt_left_child(mf, cur_node);
 					*pending_gt_ptr = *bt_right_child(mf, cur_node);
-					*best_len_ret = best_len;
 					return lz_matchptr;
 				}
 			}
 		}
 
 		if (matchptr[len] < in_next[len]) {
 			*pending_lt_ptr = cur_node;
@@ -260,15 +252,14 @@
 			if (best_lt_len < len)
 				len = best_lt_len;
 		}
 
 		if (cur_node <= cutoff || !--depth_remaining) {
 			*pending_lt_ptr = MATCHFINDER_INITVAL;
 			*pending_gt_ptr = MATCHFINDER_INITVAL;
-			*best_len_ret = best_len;
 			return lz_matchptr;
 		}
 	}
 }
 
 /*
  * Retrieve a list of matches with the current position.
@@ -289,20 +280,14 @@
  *	Must be <= @max_len.
  * @max_search_depth
  *	Limit on the number of potential matches to consider.  Must be >= 1.
  * @next_hashes
  *	The precomputed hash codes for the sequence beginning at @in_next.
  *	These will be used and then updated with the precomputed hashcodes for
  *	the sequence beginning at @in_next + 1.
- * @best_len_ret
- *	If a match of length >= 4 was found, then the length of the longest such
- *	match is written here; otherwise 3 is written here.  (Note: this is
- *	redundant with the 'struct lz_match' array, but this is easier for the
- *	compiler to optimize when inlined and the caller immediately does a
- *	check against 'best_len'.)
  * @lz_matchptr
  *	An array in which this function will record the matches.  The recorded
  *	matches will be sorted by strictly increasing length and (non-strictly)
  *	increasing offset.  The maximum number of matches that may be found is
  *	'nice_len - 2'.
  *
  * The return value is a pointer to the next available slot in the @lz_matchptr
@@ -312,48 +297,46 @@
 bt_matchfinder_get_matches(struct bt_matchfinder *mf,
 			   const u8 *in_base,
 			   ptrdiff_t cur_pos,
 			   u32 max_len,
 			   u32 nice_len,
 			   u32 max_search_depth,
 			   u32 next_hashes[2],
-			   u32 *best_len_ret,
 			   struct lz_match *lz_matchptr)
 {
 	return bt_matchfinder_advance_one_byte(mf,
 					       in_base,
 					       cur_pos,
 					       max_len,
 					       nice_len,
 					       max_search_depth,
 					       next_hashes,
-					       best_len_ret,
 					       lz_matchptr,
 					       true);
 }
 
 /*
  * Advance the matchfinder, but don't record any matches.
  *
  * This is very similar to bt_matchfinder_get_matches() because both functions
  * must do hashing and tree re-rooting.
  */
 static forceinline void
-bt_matchfinder_skip_position(struct bt_matchfinder *mf,
-			     const u8 *in_base,
-			     ptrdiff_t cur_pos,
-			     u32 nice_len,
-			     u32 max_search_depth,
-			     u32 next_hashes[2])
+bt_matchfinder_skip_byte(struct bt_matchfinder *mf,
+			 const u8 *in_base,
+			 ptrdiff_t cur_pos,
+			 u32 nice_len,
+			 u32 max_search_depth,
+			 u32 next_hashes[2])
 {
-	u32 best_len;
 	bt_matchfinder_advance_one_byte(mf,
 					in_base,
 					cur_pos,
 					nice_len,
 					nice_len,
 					max_search_depth,
 					next_hashes,
-					&best_len,
 					NULL,
 					false);
 }
+
+#endif /* LIB_BT_MATCHFINDER_H */
```

### Comparing `deflate-0.3.0/libdeflate/lib/cpu_features_common.h` & `deflate-0.4.0/libdeflate/lib/cpu_features_common.h`

 * *Files 13% similar despite different names*

```diff
@@ -21,16 +21,24 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
+#ifndef LIB_CPU_FEATURES_COMMON_H
+#define LIB_CPU_FEATURES_COMMON_H
+
 #if defined(TEST_SUPPORT__DO_NOT_USE) && !defined(FREESTANDING)
-#  define _GNU_SOURCE 1 /* for strdup() and strtok_r() */
+   /* for strdup() and strtok_r() */
+#  undef _ANSI_SOURCE
+#  ifndef __APPLE__
+#    undef _GNU_SOURCE
+#    define _GNU_SOURCE
+#  endif
 #  include <stdio.h>
 #  include <stdlib.h>
 #  include <string.h>
 #endif
 
 #include "lib_common.h"
 
@@ -77,7 +85,9 @@
 static inline void
 disable_cpu_features_for_testing(u32 *features,
 				 const struct cpu_feature *feature_table,
 				 size_t feature_table_length)
 {
 }
 #endif /* !TEST_SUPPORT__DO_NOT_USE */
+
+#endif /* LIB_CPU_FEATURES_COMMON_H */
```

### Comparing `deflate-0.3.0/libdeflate/lib/crc32.c` & `deflate-0.4.0/libdeflate/lib/crc32.c`

 * *Files 21% similar despite different names*

```diff
@@ -66,85 +66,85 @@
  * We can compute R(x) through "long division", maintaining only 32 bits of
  * state at any given time.  Multiplication by 'x' can be implemented as
  * right-shifting by 1 (assuming the polynomial<=>bitstring mapping where the
  * highest order bit represents the coefficient of x^0), and both addition and
  * subtraction can be implemented as bitwise exclusive OR (since we are working
  * in GF(2)).  Here is an unoptimized implementation:
  *
- *	static u32 crc32_gzip(const u8 *buffer, size_t size)
+ *	static u32 crc32_gzip(const u8 *p, size_t len)
  *	{
- *		u32 remainder = 0;
+ *		u32 crc = 0;
  *		const u32 divisor = 0xEDB88320;
  *
- *		for (size_t i = 0; i < size * 8 + 32; i++) {
+ *		for (size_t i = 0; i < len * 8 + 32; i++) {
  *			int bit;
  *			u32 multiple;
  *
- *			if (i < size * 8)
- *				bit = (buffer[i / 8] >> (i % 8)) & 1;
+ *			if (i < len * 8)
+ *				bit = (p[i / 8] >> (i % 8)) & 1;
  *			else
  *				bit = 0; // one of the 32 appended 0 bits
  *
  *			if (i < 32) // the first 32 bits are inverted
  *				bit ^= 1;
  *
- *			if (remainder & 1)
+ *			if (crc & 1)
  *				multiple = divisor;
  *			else
  *				multiple = 0;
  *
- *			remainder >>= 1;
- *			remainder |= (u32)bit << 31;
- *			remainder ^= multiple;
+ *			crc >>= 1;
+ *			crc |= (u32)bit << 31;
+ *			crc ^= multiple;
  *		}
  *
- *		return ~remainder;
+ *		return ~crc;
  *	}
  *
- * In this implementation, the 32-bit integer 'remainder' maintains the
- * remainder of the currently processed portion of the message (with 32 zero
- * bits appended) when divided by the generator polynomial.  'remainder' is the
- * representation of R(x), and 'divisor' is the representation of G(x) excluding
- * the x^32 coefficient.  For each bit to process, we multiply R(x) by 'x^1',
- * then add 'x^0' if the new bit is a 1.  If this causes R(x) to gain a nonzero
- * x^32 term, then we subtract G(x) from R(x).
+ * In this implementation, the 32-bit integer 'crc' maintains the remainder of
+ * the currently processed portion of the message (with 32 zero bits appended)
+ * when divided by the generator polynomial.  'crc' is the representation of
+ * R(x), and 'divisor' is the representation of G(x) excluding the x^32
+ * coefficient.  For each bit to process, we multiply R(x) by 'x^1', then add
+ * 'x^0' if the new bit is a 1.  If this causes R(x) to gain a nonzero x^32
+ * term, then we subtract G(x) from R(x).
  *
  * We can speed this up by taking advantage of the fact that XOR is commutative
- * and associative, so the order in which we combine the inputs into 'remainder'
- * is unimportant.  And since each message bit we add doesn't affect the choice
- * of 'multiple' until 32 bits later, we need not actually add each message bit
+ * and associative, so the order in which we combine the inputs into 'crc' is
+ * unimportant.  And since each message bit we add doesn't affect the choice of
+ * 'multiple' until 32 bits later, we need not actually add each message bit
  * until that point:
  *
- *	static u32 crc32_gzip(const u8 *buffer, size_t size)
+ *	static u32 crc32_gzip(const u8 *p, size_t len)
  *	{
- *		u32 remainder = ~0;
+ *		u32 crc = ~0;
  *		const u32 divisor = 0xEDB88320;
  *
- *		for (size_t i = 0; i < size * 8; i++) {
+ *		for (size_t i = 0; i < len * 8; i++) {
  *			int bit;
  *			u32 multiple;
  *
- *			bit = (buffer[i / 8] >> (i % 8)) & 1;
- *			remainder ^= bit;
- *			if (remainder & 1)
+ *			bit = (p[i / 8] >> (i % 8)) & 1;
+ *			crc ^= bit;
+ *			if (crc & 1)
  *				multiple = divisor;
  *			else
  *				multiple = 0;
- *			remainder >>= 1;
- *			remainder ^= multiple;
+ *			crc >>= 1;
+ *			crc ^= multiple;
  *		}
  *
- *		return ~remainder;
+ *		return ~crc;
  *	}
  *
  * With the above implementation we get the effect of 32 appended 0 bits for
  * free; they never affect the choice of a divisor, nor would they change the
- * value of 'remainder' if they were to be actually XOR'ed in.  And by starting
- * with a remainder of all 1 bits, we get the effect of complementing the first
- * 32 message bits.
+ * value of 'crc' if they were to be actually XOR'ed in.  And by starting with a
+ * remainder of all 1 bits, we get the effect of complementing the first 32
+ * message bits.
  *
  * The next optimization is to process the input in multi-bit units.  Suppose
  * that we insert the next 'n' message bits into the remainder.  Then we get an
  * intermediate remainder of length '32 + n' bits, and the CRC of the extra 'n'
  * bits is the amount by which the low 32 bits of the remainder will change as a
  * result of cancelling out those 'n' bits.  Taking n=8 (one byte) and
  * precomputing a table containing the CRC of each possible byte, we get
@@ -155,159 +155,108 @@
  * (1024 bytes) to 65536 entries (262144 bytes), which wastes memory and won't
  * fit in L1 cache on typical processors.
  *
  * However, we can actually process 4 bytes at a time using 4 different tables
  * with 256 entries each.  Logically, we form a 64-bit intermediate remainder
  * and cancel out the high 32 bits in 8-bit chunks.  Bits 32-39 are cancelled
  * out by the CRC of those bits, whereas bits 40-47 are be cancelled out by the
- * CRC of those bits with 8 zero bits appended, and so on.  This method is
- * implemented in crc32_slice4(), defined below.
+ * CRC of those bits with 8 zero bits appended, and so on.
  *
  * In crc32_slice8(), this method is extended to 8 bytes at a time.  The
  * intermediate remainder (which we never actually store explicitly) is 96 bits.
  *
  * On CPUs that support fast carryless multiplication, CRCs can be computed even
  * more quickly via "folding".  See e.g. the x86 PCLMUL implementation.
  */
 
 #include "lib_common.h"
-#include "libdeflate.h"
+#include "crc32_multipliers.h"
+#include "crc32_tables.h"
 
-typedef u32 (*crc32_func_t)(u32, const u8 *, size_t);
-
-/* Include architecture-specific implementations if available */
-#undef CRC32_SLICE1
-#undef CRC32_SLICE4
-#undef CRC32_SLICE8
-#undef DEFAULT_IMPL
-#undef DISPATCH
-#if defined(__arm__) || defined(__aarch64__)
-#  include "arm/crc32_impl.h"
-#elif defined(__i386__) || defined(__x86_64__)
-#  include "x86/crc32_impl.h"
-#endif
-
-/*
- * Define a generic implementation (crc32_slice8()) if needed.  crc32_slice1()
- * may also be needed as a fallback for architecture-specific implementations.
- */
-
-#ifndef DEFAULT_IMPL
-#  define CRC32_SLICE8	1
-#  define DEFAULT_IMPL	crc32_slice8
-#endif
-
-#if defined(CRC32_SLICE1) || defined(CRC32_SLICE4) || defined(CRC32_SLICE8)
-#include "crc32_table.h"
-static forceinline u32
-crc32_update_byte(u32 remainder, u8 next_byte)
-{
-	return (remainder >> 8) ^ crc32_table[(u8)remainder ^ next_byte];
-}
-#endif
-
-#ifdef CRC32_SLICE1
-static u32
-crc32_slice1(u32 remainder, const u8 *buffer, size_t size)
-{
-	size_t i;
-
-	STATIC_ASSERT(ARRAY_LEN(crc32_table) >= 0x100);
-
-	for (i = 0; i < size; i++)
-		remainder = crc32_update_byte(remainder, buffer[i]);
-	return remainder;
-}
-#endif /* CRC32_SLICE1 */
-
-#ifdef CRC32_SLICE4
-static u32
-crc32_slice4(u32 remainder, const u8 *buffer, size_t size)
-{
-	const u8 *p = buffer;
-	const u8 *end = buffer + size;
-	const u8 *end32;
-
-	STATIC_ASSERT(ARRAY_LEN(crc32_table) >= 0x400);
-
-	for (; ((uintptr_t)p & 3) && p != end; p++)
-		remainder = crc32_update_byte(remainder, *p);
-
-	end32 = p + ((end - p) & ~3);
-	for (; p != end32; p += 4) {
-		u32 v = le32_bswap(*(const u32 *)p);
-		remainder =
-		    crc32_table[0x300 + (u8)((remainder ^ v) >>  0)] ^
-		    crc32_table[0x200 + (u8)((remainder ^ v) >>  8)] ^
-		    crc32_table[0x100 + (u8)((remainder ^ v) >> 16)] ^
-		    crc32_table[0x000 + (u8)((remainder ^ v) >> 24)];
-	}
-
-	for (; p != end; p++)
-		remainder = crc32_update_byte(remainder, *p);
-
-	return remainder;
-}
-#endif /* CRC32_SLICE4 */
-
-#ifdef CRC32_SLICE8
-static u32
-crc32_slice8(u32 remainder, const u8 *buffer, size_t size)
+/* This is the default implementation.  It uses the slice-by-8 method. */
+static u32 MAYBE_UNUSED
+crc32_slice8(u32 crc, const u8 *p, size_t len)
 {
-	const u8 *p = buffer;
-	const u8 *end = buffer + size;
+	const u8 * const end = p + len;
 	const u8 *end64;
 
-	STATIC_ASSERT(ARRAY_LEN(crc32_table) >= 0x800);
-
 	for (; ((uintptr_t)p & 7) && p != end; p++)
-		remainder = crc32_update_byte(remainder, *p);
+		crc = (crc >> 8) ^ crc32_slice8_table[(u8)crc ^ *p];
 
 	end64 = p + ((end - p) & ~7);
 	for (; p != end64; p += 8) {
 		u32 v1 = le32_bswap(*(const u32 *)(p + 0));
 		u32 v2 = le32_bswap(*(const u32 *)(p + 4));
-		remainder =
-		    crc32_table[0x700 + (u8)((remainder ^ v1) >>  0)] ^
-		    crc32_table[0x600 + (u8)((remainder ^ v1) >>  8)] ^
-		    crc32_table[0x500 + (u8)((remainder ^ v1) >> 16)] ^
-		    crc32_table[0x400 + (u8)((remainder ^ v1) >> 24)] ^
-		    crc32_table[0x300 + (u8)(v2 >>  0)] ^
-		    crc32_table[0x200 + (u8)(v2 >>  8)] ^
-		    crc32_table[0x100 + (u8)(v2 >> 16)] ^
-		    crc32_table[0x000 + (u8)(v2 >> 24)];
+
+		crc = crc32_slice8_table[0x700 + (u8)((crc ^ v1) >> 0)] ^
+		      crc32_slice8_table[0x600 + (u8)((crc ^ v1) >> 8)] ^
+		      crc32_slice8_table[0x500 + (u8)((crc ^ v1) >> 16)] ^
+		      crc32_slice8_table[0x400 + (u8)((crc ^ v1) >> 24)] ^
+		      crc32_slice8_table[0x300 + (u8)(v2 >> 0)] ^
+		      crc32_slice8_table[0x200 + (u8)(v2 >> 8)] ^
+		      crc32_slice8_table[0x100 + (u8)(v2 >> 16)] ^
+		      crc32_slice8_table[0x000 + (u8)(v2 >> 24)];
 	}
 
 	for (; p != end; p++)
-		remainder = crc32_update_byte(remainder, *p);
+		crc = (crc >> 8) ^ crc32_slice8_table[(u8)crc ^ *p];
 
-	return remainder;
+	return crc;
 }
-#endif /* CRC32_SLICE8 */
 
-#ifdef DISPATCH
-static u32 dispatch(u32, const u8 *, size_t);
+/*
+ * This is a more lightweight generic implementation, which can be used as a
+ * subroutine by architecture-specific implementations to process small amounts
+ * of unaligned data at the beginning and/or end of the buffer.
+ */
+static forceinline u32 MAYBE_UNUSED
+crc32_slice1(u32 crc, const u8 *p, size_t len)
+{
+	size_t i;
+
+	for (i = 0; i < len; i++)
+		crc = (crc >> 8) ^ crc32_slice1_table[(u8)crc ^ p[i]];
+	return crc;
+}
+
+/* Include architecture-specific implementation(s) if available. */
+#undef DEFAULT_IMPL
+#undef arch_select_crc32_func
+typedef u32 (*crc32_func_t)(u32 crc, const u8 *p, size_t len);
+#if defined(ARCH_ARM32) || defined(ARCH_ARM64)
+#  include "arm/crc32_impl.h"
+#elif defined(ARCH_X86_32) || defined(ARCH_X86_64)
+#  include "x86/crc32_impl.h"
+#endif
+
+#ifndef DEFAULT_IMPL
+#  define DEFAULT_IMPL crc32_slice8
+#endif
+
+#ifdef arch_select_crc32_func
+static u32 dispatch_crc32(u32 crc, const u8 *p, size_t len);
 
-static volatile crc32_func_t crc32_impl = dispatch;
+static volatile crc32_func_t crc32_impl = dispatch_crc32;
 
-/* Choose the fastest implementation at runtime */
-static u32 dispatch(u32 remainder, const u8 *buffer, size_t size)
+/* Choose the best implementation at runtime. */
+static u32 dispatch_crc32(u32 crc, const u8 *p, size_t len)
 {
 	crc32_func_t f = arch_select_crc32_func();
 
 	if (f == NULL)
 		f = DEFAULT_IMPL;
 
 	crc32_impl = f;
-	return crc32_impl(remainder, buffer, size);
+	return f(crc, p, len);
 }
 #else
-#  define crc32_impl DEFAULT_IMPL /* only one implementation, use it */
+/* The best implementation is statically known, so call it directly. */
+#define crc32_impl DEFAULT_IMPL
 #endif
 
-LIBDEFLATEEXPORT u32 LIBDEFLATEAPI
-libdeflate_crc32(u32 remainder, const void *buffer, size_t size)
+LIBDEFLATEAPI u32
+libdeflate_crc32(u32 crc, const void *p, size_t len)
 {
-	if (buffer == NULL) /* return initial value */
+	if (p == NULL) /* Return initial value. */
 		return 0;
-	return ~crc32_impl(~remainder, buffer, size);
+	return ~crc32_impl(~crc, p, len);
 }
```

### Comparing `deflate-0.3.0/libdeflate/lib/crc32_table.h` & `deflate-0.4.0/libdeflate/lib/crc32_tables.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,81 @@
 /*
- * crc32_table.h - data table to accelerate CRC-32 computation
+ * crc32_tables.h - data tables for CRC-32 computation
  *
- * THIS FILE WAS AUTOMATICALLY GENERATED BY gen_crc32_table.c.  DO NOT EDIT.
+ * THIS FILE WAS GENERATED BY gen_crc32_tables.c.  DO NOT EDIT.
  */
 
-#include <stdint.h>
+static const u32 crc32_slice1_table[] MAYBE_UNUSED = {
+	0x00000000, 0x77073096, 0xee0e612c, 0x990951ba,
+	0x076dc419, 0x706af48f, 0xe963a535, 0x9e6495a3,
+	0x0edb8832, 0x79dcb8a4, 0xe0d5e91e, 0x97d2d988,
+	0x09b64c2b, 0x7eb17cbd, 0xe7b82d07, 0x90bf1d91,
+	0x1db71064, 0x6ab020f2, 0xf3b97148, 0x84be41de,
+	0x1adad47d, 0x6ddde4eb, 0xf4d4b551, 0x83d385c7,
+	0x136c9856, 0x646ba8c0, 0xfd62f97a, 0x8a65c9ec,
+	0x14015c4f, 0x63066cd9, 0xfa0f3d63, 0x8d080df5,
+	0x3b6e20c8, 0x4c69105e, 0xd56041e4, 0xa2677172,
+	0x3c03e4d1, 0x4b04d447, 0xd20d85fd, 0xa50ab56b,
+	0x35b5a8fa, 0x42b2986c, 0xdbbbc9d6, 0xacbcf940,
+	0x32d86ce3, 0x45df5c75, 0xdcd60dcf, 0xabd13d59,
+	0x26d930ac, 0x51de003a, 0xc8d75180, 0xbfd06116,
+	0x21b4f4b5, 0x56b3c423, 0xcfba9599, 0xb8bda50f,
+	0x2802b89e, 0x5f058808, 0xc60cd9b2, 0xb10be924,
+	0x2f6f7c87, 0x58684c11, 0xc1611dab, 0xb6662d3d,
+	0x76dc4190, 0x01db7106, 0x98d220bc, 0xefd5102a,
+	0x71b18589, 0x06b6b51f, 0x9fbfe4a5, 0xe8b8d433,
+	0x7807c9a2, 0x0f00f934, 0x9609a88e, 0xe10e9818,
+	0x7f6a0dbb, 0x086d3d2d, 0x91646c97, 0xe6635c01,
+	0x6b6b51f4, 0x1c6c6162, 0x856530d8, 0xf262004e,
+	0x6c0695ed, 0x1b01a57b, 0x8208f4c1, 0xf50fc457,
+	0x65b0d9c6, 0x12b7e950, 0x8bbeb8ea, 0xfcb9887c,
+	0x62dd1ddf, 0x15da2d49, 0x8cd37cf3, 0xfbd44c65,
+	0x4db26158, 0x3ab551ce, 0xa3bc0074, 0xd4bb30e2,
+	0x4adfa541, 0x3dd895d7, 0xa4d1c46d, 0xd3d6f4fb,
+	0x4369e96a, 0x346ed9fc, 0xad678846, 0xda60b8d0,
+	0x44042d73, 0x33031de5, 0xaa0a4c5f, 0xdd0d7cc9,
+	0x5005713c, 0x270241aa, 0xbe0b1010, 0xc90c2086,
+	0x5768b525, 0x206f85b3, 0xb966d409, 0xce61e49f,
+	0x5edef90e, 0x29d9c998, 0xb0d09822, 0xc7d7a8b4,
+	0x59b33d17, 0x2eb40d81, 0xb7bd5c3b, 0xc0ba6cad,
+	0xedb88320, 0x9abfb3b6, 0x03b6e20c, 0x74b1d29a,
+	0xead54739, 0x9dd277af, 0x04db2615, 0x73dc1683,
+	0xe3630b12, 0x94643b84, 0x0d6d6a3e, 0x7a6a5aa8,
+	0xe40ecf0b, 0x9309ff9d, 0x0a00ae27, 0x7d079eb1,
+	0xf00f9344, 0x8708a3d2, 0x1e01f268, 0x6906c2fe,
+	0xf762575d, 0x806567cb, 0x196c3671, 0x6e6b06e7,
+	0xfed41b76, 0x89d32be0, 0x10da7a5a, 0x67dd4acc,
+	0xf9b9df6f, 0x8ebeeff9, 0x17b7be43, 0x60b08ed5,
+	0xd6d6a3e8, 0xa1d1937e, 0x38d8c2c4, 0x4fdff252,
+	0xd1bb67f1, 0xa6bc5767, 0x3fb506dd, 0x48b2364b,
+	0xd80d2bda, 0xaf0a1b4c, 0x36034af6, 0x41047a60,
+	0xdf60efc3, 0xa867df55, 0x316e8eef, 0x4669be79,
+	0xcb61b38c, 0xbc66831a, 0x256fd2a0, 0x5268e236,
+	0xcc0c7795, 0xbb0b4703, 0x220216b9, 0x5505262f,
+	0xc5ba3bbe, 0xb2bd0b28, 0x2bb45a92, 0x5cb36a04,
+	0xc2d7ffa7, 0xb5d0cf31, 0x2cd99e8b, 0x5bdeae1d,
+	0x9b64c2b0, 0xec63f226, 0x756aa39c, 0x026d930a,
+	0x9c0906a9, 0xeb0e363f, 0x72076785, 0x05005713,
+	0x95bf4a82, 0xe2b87a14, 0x7bb12bae, 0x0cb61b38,
+	0x92d28e9b, 0xe5d5be0d, 0x7cdcefb7, 0x0bdbdf21,
+	0x86d3d2d4, 0xf1d4e242, 0x68ddb3f8, 0x1fda836e,
+	0x81be16cd, 0xf6b9265b, 0x6fb077e1, 0x18b74777,
+	0x88085ae6, 0xff0f6a70, 0x66063bca, 0x11010b5c,
+	0x8f659eff, 0xf862ae69, 0x616bffd3, 0x166ccf45,
+	0xa00ae278, 0xd70dd2ee, 0x4e048354, 0x3903b3c2,
+	0xa7672661, 0xd06016f7, 0x4969474d, 0x3e6e77db,
+	0xaed16a4a, 0xd9d65adc, 0x40df0b66, 0x37d83bf0,
+	0xa9bcae53, 0xdebb9ec5, 0x47b2cf7f, 0x30b5ffe9,
+	0xbdbdf21c, 0xcabac28a, 0x53b39330, 0x24b4a3a6,
+	0xbad03605, 0xcdd70693, 0x54de5729, 0x23d967bf,
+	0xb3667a2e, 0xc4614ab8, 0x5d681b02, 0x2a6f2b94,
+	0xb40bbe37, 0xc30c8ea1, 0x5a05df1b, 0x2d02ef8d,
+};
 
-static const uint32_t crc32_table[] = {
+static const u32 crc32_slice8_table[] MAYBE_UNUSED = {
 	0x00000000, 0x77073096, 0xee0e612c, 0x990951ba,
 	0x076dc419, 0x706af48f, 0xe963a535, 0x9e6495a3,
 	0x0edb8832, 0x79dcb8a4, 0xe0d5e91e, 0x97d2d988,
 	0x09b64c2b, 0x7eb17cbd, 0xe7b82d07, 0x90bf1d91,
 	0x1db71064, 0x6ab020f2, 0xf3b97148, 0x84be41de,
 	0x1adad47d, 0x6ddde4eb, 0xf4d4b551, 0x83d385c7,
 	0x136c9856, 0x646ba8c0, 0xfd62f97a, 0x8a65c9ec,
@@ -67,15 +132,14 @@
 	0xa7672661, 0xd06016f7, 0x4969474d, 0x3e6e77db,
 	0xaed16a4a, 0xd9d65adc, 0x40df0b66, 0x37d83bf0,
 	0xa9bcae53, 0xdebb9ec5, 0x47b2cf7f, 0x30b5ffe9,
 	0xbdbdf21c, 0xcabac28a, 0x53b39330, 0x24b4a3a6,
 	0xbad03605, 0xcdd70693, 0x54de5729, 0x23d967bf,
 	0xb3667a2e, 0xc4614ab8, 0x5d681b02, 0x2a6f2b94,
 	0xb40bbe37, 0xc30c8ea1, 0x5a05df1b, 0x2d02ef8d,
-#if defined(CRC32_SLICE4) || defined(CRC32_SLICE8)
 	0x00000000, 0x191b3141, 0x32366282, 0x2b2d53c3,
 	0x646cc504, 0x7d77f445, 0x565aa786, 0x4f4196c7,
 	0xc8d98a08, 0xd1c2bb49, 0xfaefe88a, 0xe3f4d9cb,
 	0xacb54f0c, 0xb5ae7e4d, 0x9e832d8e, 0x87981ccf,
 	0x4ac21251, 0x53d92310, 0x78f470d3, 0x61ef4192,
 	0x2eaed755, 0x37b5e614, 0x1c98b5d7, 0x05838496,
 	0x821b9859, 0x9b00a918, 0xb02dfadb, 0xa936cb9a,
@@ -260,16 +324,14 @@
 	0x591dd66f, 0xe1a1b10a, 0xf3141ee4, 0x4ba87981,
 	0x13cb69d7, 0xab770eb2, 0xb9c2a15c, 0x017ec639,
 	0x9ca9fe80, 0x241599e5, 0x36a0360b, 0x8e1c516e,
 	0x866616a7, 0x3eda71c2, 0x2c6fde2c, 0x94d3b949,
 	0x090481f0, 0xb1b8e695, 0xa30d497b, 0x1bb12e1e,
 	0x43d23e48, 0xfb6e592d, 0xe9dbf6c3, 0x516791a6,
 	0xccb0a91f, 0x740cce7a, 0x66b96194, 0xde0506f1,
-#endif /* CRC32_SLICE4 || CRC32_SLICE8 */
-#if defined(CRC32_SLICE8)
 	0x00000000, 0x3d6029b0, 0x7ac05360, 0x47a07ad0,
 	0xf580a6c0, 0xc8e08f70, 0x8f40f5a0, 0xb220dc10,
 	0x30704bc1, 0x0d106271, 0x4ab018a1, 0x77d03111,
 	0xc5f0ed01, 0xf890c4b1, 0xbf30be61, 0x825097d1,
 	0x60e09782, 0x5d80be32, 0x1a20c4e2, 0x2740ed52,
 	0x95603142, 0xa80018f2, 0xefa06222, 0xd2c04b92,
 	0x5090dc43, 0x6df0f5f3, 0x2a508f23, 0x1730a693,
@@ -518,9 +580,8 @@
 	0x079a2b9b, 0xcb302b05, 0x45bf2ce6, 0x89152c78,
 	0x50353ed4, 0x9c9f3e4a, 0x121039a9, 0xdeba3937,
 	0xd47f302e, 0x18d530b0, 0x965a3753, 0x5af037cd,
 	0xff6b144a, 0x33c114d4, 0xbd4e1337, 0x71e413a9,
 	0x7b211ab0, 0xb78b1a2e, 0x39041dcd, 0xf5ae1d53,
 	0x2c8e0fff, 0xe0240f61, 0x6eab0882, 0xa201081c,
 	0xa8c40105, 0x646e019b, 0xeae10678, 0x264b06e6,
-#endif /* CRC32_SLICE8 */
 };
```

### Comparing `deflate-0.3.0/libdeflate/lib/deflate_compress.c` & `deflate-0.4.0/libdeflate/lib/deflate_compress.c`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * deflate_compress.c - a compressor for DEFLATE
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -25,133 +23,253 @@
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "deflate_compress.h"
 #include "deflate_constants.h"
-#include "unaligned.h"
 
-#include "libdeflate.h"
+/******************************************************************************/
 
 /*
- * By default, the near-optimal parsing algorithm is enabled at compression
- * level 8 and above.  The near-optimal parsing algorithm produces a compression
- * ratio significantly better than the greedy and lazy algorithms implemented
- * here, and also the algorithm used by zlib at level 9.  However, it is slow.
+ * The following parameters can be changed at build time to customize the
+ * compression algorithms slightly:
+ *
+ * (Note, not all customizable parameters are here.  Some others can be found in
+ * libdeflate_alloc_compressor() and in *_matchfinder.h.)
  */
-#define SUPPORT_NEAR_OPTIMAL_PARSING 1
 
 /*
- * Define to 1 to maintain the full map from match offsets to offset slots.
- * This slightly speeds up translations of match offsets to offset slots, but it
- * uses 32769 bytes of memory rather than the 512 bytes used by the condensed
- * map.  The speedup provided by the larger map is most helpful when the
- * near-optimal parsing algorithm is being used.
+ * If this parameter is defined to 1, then the near-optimal parsing algorithm
+ * will be included, and compression levels 10-12 will use it.  This algorithm
+ * usually produces a compression ratio significantly better than the other
+ * algorithms.  However, it is slow.  If this parameter is defined to 0, then
+ * levels 10-12 will be the same as level 9 and will use the lazy2 algorithm.
  */
-#define USE_FULL_OFFSET_SLOT_FAST	SUPPORT_NEAR_OPTIMAL_PARSING
+#define SUPPORT_NEAR_OPTIMAL_PARSING	1
 
 /*
- * DEFLATE uses a 32768 byte sliding window; set the matchfinder parameters
- * appropriately.
+ * This is the minimum block length that the compressor will use, in
+ * uncompressed bytes.  This should be a value below which using shorter blocks
+ * is unlikely to be worthwhile, due to the per-block overhead.  This value does
+ * not apply to the final block, which may be shorter than this (if the input is
+ * shorter, it will have to be), or to the final uncompressed block in a series
+ * of uncompressed blocks that cover more than UINT16_MAX bytes.
+ *
+ * This value is also approximately the amount by which what would otherwise be
+ * the second-to-last block is allowed to grow past the soft maximum length in
+ * order to avoid having to use a very short final block.
+ *
+ * Defining a fixed minimum block length is needed in order to guarantee a
+ * reasonable upper bound on the compressed size.  It's also needed because our
+ * block splitting algorithm doesn't work well on very short blocks.
  */
-#define MATCHFINDER_WINDOW_ORDER	15
+#define MIN_BLOCK_LENGTH	5000
 
-#include "hc_matchfinder.h"
-#if SUPPORT_NEAR_OPTIMAL_PARSING
-#  include "bt_matchfinder.h"
-#endif
+/*
+ * For the greedy, lazy, lazy2, and near-optimal compressors: This is the soft
+ * maximum block length, in uncompressed bytes.  The compressor will try to end
+ * blocks at this length, but it may go slightly past it if there is a match
+ * that straddles this limit or if the input data ends soon after this limit.
+ * This parameter doesn't apply to uncompressed blocks, which the DEFLATE format
+ * limits to 65535 bytes.
+ *
+ * This should be a value above which it is very likely that splitting the block
+ * would produce a better compression ratio.  For the near-optimal compressor,
+ * increasing/decreasing this parameter will increase/decrease per-compressor
+ * memory usage linearly.
+ */
+#define SOFT_MAX_BLOCK_LENGTH	300000
 
 /*
- * The compressor always chooses a block of at least MIN_BLOCK_LENGTH bytes,
- * except if the last block has to be shorter.
+ * For the greedy, lazy, and lazy2 compressors: this is the length of the
+ * sequence store, which is an array where the compressor temporarily stores
+ * matches that it's going to use in the current block.  This value is the
+ * maximum number of matches that can be used in a block.  If the sequence store
+ * fills up, then the compressor will be forced to end the block early.  This
+ * value should be large enough so that this rarely happens, due to the block
+ * being ended normally before then.  Increasing/decreasing this value will
+ * increase/decrease per-compressor memory usage linearly.
  */
-#define MIN_BLOCK_LENGTH	10000
+#define SEQ_STORE_LENGTH	50000
 
 /*
- * The compressor attempts to end blocks after SOFT_MAX_BLOCK_LENGTH bytes, but
- * the final length might be slightly longer due to matches extending beyond
- * this limit.
+ * For deflate_compress_fastest(): This is the soft maximum block length.
+ * deflate_compress_fastest() doesn't use the regular block splitting algorithm;
+ * it only ends blocks when they reach FAST_SOFT_MAX_BLOCK_LENGTH bytes or
+ * FAST_SEQ_STORE_LENGTH matches.  Therefore, this value should be lower than
+ * the regular SOFT_MAX_BLOCK_LENGTH.
  */
-#define SOFT_MAX_BLOCK_LENGTH	300000
+#define FAST_SOFT_MAX_BLOCK_LENGTH	65535
 
 /*
- * The number of observed matches or literals that represents sufficient data to
- * decide whether the current block should be terminated or not.
+ * For deflate_compress_fastest(): this is the length of the sequence store.
+ * This is like SEQ_STORE_LENGTH, but this should be a lower value.
  */
-#define NUM_OBSERVATIONS_PER_BLOCK_CHECK       512
+#define FAST_SEQ_STORE_LENGTH	8192
 
+/*
+ * These are the maximum codeword lengths, in bits, the compressor will use for
+ * each Huffman code.  The DEFLATE format defines limits for these.  However,
+ * further limiting litlen codewords to 14 bits is beneficial, since it has
+ * negligible effect on compression ratio but allows some optimizations when
+ * outputting bits.  (It allows 4 literals to be written at once rather than 3.)
+ */
+#define MAX_LITLEN_CODEWORD_LEN		14
+#define MAX_OFFSET_CODEWORD_LEN		DEFLATE_MAX_OFFSET_CODEWORD_LEN
+#define MAX_PRE_CODEWORD_LEN		DEFLATE_MAX_PRE_CODEWORD_LEN
 
 #if SUPPORT_NEAR_OPTIMAL_PARSING
-/* Constants specific to the near-optimal parsing algorithm */
+
+/* Parameters specific to the near-optimal parsing algorithm */
+
+/*
+ * BIT_COST is a scaling factor that allows the near-optimal compressor to
+ * consider fractional bit costs when deciding which literal/match sequence to
+ * use.  This is useful when the true symbol costs are unknown.  For example, if
+ * the compressor thinks that a symbol has 6.5 bits of entropy, it can set its
+ * cost to 6.5 bits rather than have to use 6 or 7 bits.  Although in the end
+ * each symbol will use a whole number of bits due to the Huffman coding,
+ * considering fractional bits can be helpful due to the limited information.
+ *
+ * BIT_COST should be a power of 2.  A value of 8 or 16 works well.  A higher
+ * value isn't very useful since the calculations are approximate anyway.
+ *
+ * BIT_COST doesn't apply to deflate_flush_block() and
+ * deflate_compute_true_cost(), which consider whole bits.
+ */
+#define BIT_COST	16
 
 /*
- * The maximum number of matches the matchfinder can find at a single position.
- * Since the matchfinder never finds more than one match for the same length,
- * presuming one of each possible length is sufficient for an upper bound.
- * (This says nothing about whether it is worthwhile to consider so many
- * matches; this is just defining the worst case.)
+ * The NOSTAT_BITS value for a given alphabet is the number of bits assumed to
+ * be needed to output a symbol that was unused in the previous optimization
+ * pass.  Assigning a default cost allows the symbol to be used in the next
+ * optimization pass.  However, the cost should be relatively high because the
+ * symbol probably won't be used very many times (if at all).
  */
-#  define MAX_MATCHES_PER_POS	(DEFLATE_MAX_MATCH_LEN - DEFLATE_MIN_MATCH_LEN + 1)
+#define LITERAL_NOSTAT_BITS	13
+#define LENGTH_NOSTAT_BITS	13
+#define OFFSET_NOSTAT_BITS	10
 
 /*
- * The number of lz_match structures in the match cache, excluding the extra
- * "overflow" entries.  This value should be high enough so that nearly the
- * time, all matches found in a given block can fit in the match cache.
- * However, fallback behavior (immediately terminating the block) on cache
- * overflow is still required.
+ * This is (slightly less than) the maximum number of matches that the
+ * near-optimal compressor will cache per block.  This behaves similarly to
+ * SEQ_STORE_LENGTH for the other compressors.
  */
-#  define CACHE_LENGTH      (SOFT_MAX_BLOCK_LENGTH * 5)
+#define MATCH_CACHE_LENGTH	(SOFT_MAX_BLOCK_LENGTH * 5)
 
 #endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
 
+/******************************************************************************/
+
+/* Include the needed matchfinders. */
+#define MATCHFINDER_WINDOW_ORDER	DEFLATE_WINDOW_ORDER
+#include "hc_matchfinder.h"
+#include "ht_matchfinder.h"
+#if SUPPORT_NEAR_OPTIMAL_PARSING
+#  include "bt_matchfinder.h"
 /*
- * These are the compressor-side limits on the codeword lengths for each Huffman
- * code.  To make outputting bits slightly faster, some of these limits are
- * lower than the limits defined by the DEFLATE format.  This does not
- * significantly affect the compression ratio, at least for the block lengths we
- * use.
+ * This is the maximum number of matches the binary trees matchfinder can find
+ * at a single position.  Since the matchfinder never finds more than one match
+ * for the same length, presuming one of each possible length is sufficient for
+ * an upper bound.  (This says nothing about whether it is worthwhile to
+ * consider so many matches; this is just defining the worst case.)
  */
-#define MAX_LITLEN_CODEWORD_LEN		14
-#define MAX_OFFSET_CODEWORD_LEN		DEFLATE_MAX_OFFSET_CODEWORD_LEN
-#define MAX_PRE_CODEWORD_LEN		DEFLATE_MAX_PRE_CODEWORD_LEN
+#define MAX_MATCHES_PER_POS	\
+	(DEFLATE_MAX_MATCH_LEN - DEFLATE_MIN_MATCH_LEN + 1)
+#endif
+
+/*
+ * The largest block length we will ever use is when the final block is of
+ * length SOFT_MAX_BLOCK_LENGTH + MIN_BLOCK_LENGTH - 1, or when any block is of
+ * length SOFT_MAX_BLOCK_LENGTH + 1 + DEFLATE_MAX_MATCH_LEN.  The latter case
+ * occurs when the lazy2 compressor chooses two literals and a maximum-length
+ * match, starting at SOFT_MAX_BLOCK_LENGTH - 1.
+ */
+#define MAX_BLOCK_LENGTH	\
+	MAX(SOFT_MAX_BLOCK_LENGTH + MIN_BLOCK_LENGTH - 1,	\
+	    SOFT_MAX_BLOCK_LENGTH + 1 + DEFLATE_MAX_MATCH_LEN)
+
+static forceinline void
+check_buildtime_parameters(void)
+{
+	/*
+	 * Verify that MIN_BLOCK_LENGTH is being honored, as
+	 * libdeflate_deflate_compress_bound() depends on it.
+	 */
+	STATIC_ASSERT(SOFT_MAX_BLOCK_LENGTH >= MIN_BLOCK_LENGTH);
+	STATIC_ASSERT(FAST_SOFT_MAX_BLOCK_LENGTH >= MIN_BLOCK_LENGTH);
+	STATIC_ASSERT(SEQ_STORE_LENGTH * DEFLATE_MIN_MATCH_LEN >=
+		      MIN_BLOCK_LENGTH);
+	STATIC_ASSERT(FAST_SEQ_STORE_LENGTH * HT_MATCHFINDER_MIN_MATCH_LEN >=
+		      MIN_BLOCK_LENGTH);
+#if SUPPORT_NEAR_OPTIMAL_PARSING
+	STATIC_ASSERT(MIN_BLOCK_LENGTH * MAX_MATCHES_PER_POS <=
+		      MATCH_CACHE_LENGTH);
+#endif
+
+	/* The definition of MAX_BLOCK_LENGTH assumes this. */
+	STATIC_ASSERT(FAST_SOFT_MAX_BLOCK_LENGTH <= SOFT_MAX_BLOCK_LENGTH);
+
+	/* Verify that the sequence stores aren't uselessly large. */
+	STATIC_ASSERT(SEQ_STORE_LENGTH * DEFLATE_MIN_MATCH_LEN <=
+		      SOFT_MAX_BLOCK_LENGTH + MIN_BLOCK_LENGTH);
+	STATIC_ASSERT(FAST_SEQ_STORE_LENGTH * HT_MATCHFINDER_MIN_MATCH_LEN <=
+		      FAST_SOFT_MAX_BLOCK_LENGTH + MIN_BLOCK_LENGTH);
+
+	/* Verify that the maximum codeword lengths are valid. */
+	STATIC_ASSERT(
+		MAX_LITLEN_CODEWORD_LEN <= DEFLATE_MAX_LITLEN_CODEWORD_LEN);
+	STATIC_ASSERT(
+		MAX_OFFSET_CODEWORD_LEN <= DEFLATE_MAX_OFFSET_CODEWORD_LEN);
+	STATIC_ASSERT(
+		MAX_PRE_CODEWORD_LEN <= DEFLATE_MAX_PRE_CODEWORD_LEN);
+	STATIC_ASSERT(
+		(1U << MAX_LITLEN_CODEWORD_LEN) >= DEFLATE_NUM_LITLEN_SYMS);
+	STATIC_ASSERT(
+		(1U << MAX_OFFSET_CODEWORD_LEN) >= DEFLATE_NUM_OFFSET_SYMS);
+	STATIC_ASSERT(
+		(1U << MAX_PRE_CODEWORD_LEN) >= DEFLATE_NUM_PRECODE_SYMS);
+}
+
+/******************************************************************************/
 
-/* Table: length slot => length slot base value  */
+/* Table: length slot => length slot base value */
 static const unsigned deflate_length_slot_base[] = {
-	3   , 4   , 5   , 6   , 7   , 8   , 9   , 10  ,
-	11  , 13  , 15  , 17  , 19  , 23  , 27  , 31  ,
-	35  , 43  , 51  , 59  , 67  , 83  , 99  , 115 ,
-	131 , 163 , 195 , 227 , 258 ,
+	3,    4,    5,    6,    7,    8,    9,    10,
+	11,   13,   15,   17,   19,   23,   27,   31,
+	35,   43,   51,   59,   67,   83,   99,   115,
+	131,  163,  195,  227,  258,
 };
 
-/* Table: length slot => number of extra length bits  */
+/* Table: length slot => number of extra length bits */
 static const u8 deflate_extra_length_bits[] = {
-	0   , 0   , 0   , 0   , 0   , 0   , 0   , 0 ,
-	1   , 1   , 1   , 1   , 2   , 2   , 2   , 2 ,
-	3   , 3   , 3   , 3   , 4   , 4   , 4   , 4 ,
-	5   , 5   , 5   , 5   , 0   ,
+	0,    0,    0,    0,    0,    0,    0,    0,
+	1,    1,    1,    1,    2,    2,    2,    2,
+	3,    3,    3,    3,    4,    4,    4,    4,
+	5,    5,    5,    5,    0,
 };
 
-/* Table: offset slot => offset slot base value  */
+/* Table: offset slot => offset slot base value */
 static const unsigned deflate_offset_slot_base[] = {
-	1    , 2    , 3    , 4     , 5     , 7     , 9     , 13    ,
-	17   , 25   , 33   , 49    , 65    , 97    , 129   , 193   ,
-	257  , 385  , 513  , 769   , 1025  , 1537  , 2049  , 3073  ,
-	4097 , 6145 , 8193 , 12289 , 16385 , 24577 ,
+	1,     2,     3,     4,     5,     7,     9,     13,
+	17,    25,    33,    49,    65,    97,    129,   193,
+	257,   385,   513,   769,   1025,  1537,  2049,  3073,
+	4097,  6145,  8193,  12289, 16385, 24577,
 };
 
-/* Table: offset slot => number of extra offset bits  */
+/* Table: offset slot => number of extra offset bits */
 static const u8 deflate_extra_offset_bits[] = {
-	0    , 0    , 0    , 0     , 1     , 1     , 2     , 2     ,
-	3    , 3    , 4    , 4     , 5     , 5     , 6     , 6     ,
-	7    , 7    , 8    , 8     , 9     , 9     , 10    , 10    ,
-	11   , 11   , 12   , 12    , 13    , 13    ,
+	0,     0,     0,     0,     1,     1,     2,     2,
+	3,     3,     4,     4,     5,     5,     6,     6,
+	7,     7,     8,     8,     9,     9,     10,    10,
+	11,    11,    12,    12,    13,    13,
 };
 
-/* Table: length => length slot  */
+/* Table: length => length slot */
 static const u8 deflate_length_slot[DEFLATE_MAX_MATCH_LEN + 1] = {
 	0, 0, 0, 0, 1, 2, 3, 4, 5, 6, 7, 8, 8, 9, 9, 10, 10, 11, 11, 12, 12, 12,
 	12, 13, 13, 13, 13, 14, 14, 14, 14, 15, 15, 15, 15, 16, 16, 16, 16, 16,
 	16, 16, 16, 17, 17, 17, 17, 17, 17, 17, 17, 18, 18, 18, 18, 18, 18, 18,
 	18, 19, 19, 19, 19, 19, 19, 19, 19, 20, 20, 20, 20, 20, 20, 20, 20, 20,
 	20, 20, 20, 20, 20, 20, 20, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21, 21,
 	21, 21, 21, 21, 21, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22, 22,
@@ -162,115 +280,144 @@
 	25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 26, 26, 26, 26, 26, 26, 26,
 	26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26,
 	26, 26, 26, 26, 26, 26, 26, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,
 	27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,
 	27, 27, 28,
 };
 
+/*
+ * A condensed table which maps offset => offset slot as follows:
+ *
+ *	offset <= 256: deflate_offset_slot[offset]
+ *	offset > 256: deflate_offset_slot[256 + ((offset - 1) >> 7)]
+ *
+ * This table was generated by scripts/gen_offset_slot_map.py.
+ */
+static const u8 deflate_offset_slot[512] = {
+	0, 0, 1, 2, 3, 4, 4, 5, 5, 6, 6, 6, 6, 7, 7, 7,
+	7, 8, 8, 8, 8, 8, 8, 8, 8, 9, 9, 9, 9, 9, 9, 9,
+	9, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10,
+	10, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11, 11,
+	11, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
+	12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12, 12,
+	12, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
+	13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13, 13,
+	13, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
+	14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
+	14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
+	14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14, 14,
+	14, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
+	15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
+	15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
+	15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15, 15,
+	15, 0, 16, 17, 18, 18, 19, 19, 20, 20, 20, 20, 21, 21, 21, 21,
+	22, 22, 22, 22, 22, 22, 22, 22, 23, 23, 23, 23, 23, 23, 23, 23,
+	24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24, 24,
+	25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25, 25,
+	26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26,
+	26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26, 26,
+	27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,
+	27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27, 27,
+	28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28,
+	28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28,
+	28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28,
+	28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28, 28,
+	29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+	29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+	29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+	29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29, 29,
+};
+
 /* The order in which precode codeword lengths are stored */
 static const u8 deflate_precode_lens_permutation[DEFLATE_NUM_PRECODE_SYMS] = {
 	16, 17, 18, 0, 8, 7, 9, 6, 10, 5, 11, 4, 12, 3, 13, 2, 14, 1, 15
 };
 
-/* Codewords for the DEFLATE Huffman codes.  */
+/* Table: precode symbol => number of extra bits */
+static const u8 deflate_extra_precode_bits[DEFLATE_NUM_PRECODE_SYMS] = {
+	0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 3, 7
+};
+
+/* Codewords for the DEFLATE Huffman codes */
 struct deflate_codewords {
 	u32 litlen[DEFLATE_NUM_LITLEN_SYMS];
 	u32 offset[DEFLATE_NUM_OFFSET_SYMS];
 };
 
-/* Codeword lengths (in bits) for the DEFLATE Huffman codes.
- * A zero length means the corresponding symbol had zero frequency.  */
+/*
+ * Codeword lengths (in bits) for the DEFLATE Huffman codes.
+ * A zero length means the corresponding symbol had zero frequency.
+ */
 struct deflate_lens {
 	u8 litlen[DEFLATE_NUM_LITLEN_SYMS];
 	u8 offset[DEFLATE_NUM_OFFSET_SYMS];
 };
 
-/* Codewords and lengths for the DEFLATE Huffman codes.  */
+/* Codewords and lengths for the DEFLATE Huffman codes */
 struct deflate_codes {
 	struct deflate_codewords codewords;
 	struct deflate_lens lens;
 };
 
-/* Symbol frequency counters for the DEFLATE Huffman codes.  */
+/* Symbol frequency counters for the DEFLATE Huffman codes */
 struct deflate_freqs {
 	u32 litlen[DEFLATE_NUM_LITLEN_SYMS];
 	u32 offset[DEFLATE_NUM_OFFSET_SYMS];
 };
 
-#if SUPPORT_NEAR_OPTIMAL_PARSING
-
-/* Costs for the near-optimal parsing algorithm.  */
-struct deflate_costs {
-
-	/* The cost to output each possible literal.  */
-	u32 literal[DEFLATE_NUM_LITERALS];
-
-	/* The cost to output each possible match length.  */
-	u32 length[DEFLATE_MAX_MATCH_LEN + 1];
-
-	/* The cost to output a match offset of each possible offset slot.  */
-	u32 offset_slot[DEFLATE_NUM_OFFSET_SYMS];
-};
-
-/*
- * COST_SHIFT is a scaling factor that makes it possible to consider fractional
- * bit costs.  A token requiring 'n' bits to represent has cost n << COST_SHIFT.
- *
- * Note: this is only useful as a statistical trick for when the true costs are
- * unknown.  In reality, each token in DEFLATE requires a whole number of bits
- * to output.
- */
-#define COST_SHIFT	3
-
-/*
- * The NOSTAT_BITS value for a given alphabet is the number of bits assumed to
- * be needed to output a symbol that was unused in the previous optimization
- * pass.  Assigning a default cost allows the symbol to be used in the next
- * optimization pass.  However, the cost should be relatively high because the
- * symbol probably won't be used very many times (if at all).
- */
-#define LITERAL_NOSTAT_BITS	13
-#define LENGTH_NOSTAT_BITS	13
-#define OFFSET_NOSTAT_BITS	10
-
-#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
-
 /*
  * Represents a run of literals followed by a match or end-of-block.  This
  * struct is needed to temporarily store items chosen by the parser, since items
  * cannot be written until all items for the block have been chosen and the
  * block's Huffman codes have been computed.
  */
 struct deflate_sequence {
 
-	/* Bits 0..22: the number of literals in this run.  This may be 0 and
-	 * can be at most about SOFT_MAX_BLOCK_LENGTH.  The literals are not
-	 * stored explicitly in this structure; instead, they are read directly
-	 * from the uncompressed data.
+	/*
+	 * Bits 0..22: the number of literals in this run.  This may be 0 and
+	 * can be at most MAX_BLOCK_LENGTH.  The literals are not stored
+	 * explicitly in this structure; instead, they are read directly from
+	 * the uncompressed data.
 	 *
 	 * Bits 23..31: the length of the match which follows the literals, or 0
 	 * if this literal run was the last in the block, so there is no match
-	 * which follows it.  */
+	 * which follows it.
+	 */
+#define SEQ_LENGTH_SHIFT 23
+#define SEQ_LITRUNLEN_MASK (((u32)1 << SEQ_LENGTH_SHIFT) - 1)
 	u32 litrunlen_and_length;
 
-	/* If 'length' doesn't indicate end-of-block, then this is the offset of
-	 * the match which follows the literals.  */
+	/*
+	 * If 'length' doesn't indicate end-of-block, then this is the offset of
+	 * the match which follows the literals.
+	 */
 	u16 offset;
 
-	/* If 'length' doesn't indicate end-of-block, then this is the offset
-	 * symbol of the match which follows the literals.  */
-	u8 offset_symbol;
-
-	/* If 'length' doesn't indicate end-of-block, then this is the length
-	 * slot of the match which follows the literals.  */
-	u8 length_slot;
+	/*
+	 * If 'length' doesn't indicate end-of-block, then this is the offset
+	 * slot of the match which follows the literals.
+	 */
+	u16 offset_slot;
 };
 
 #if SUPPORT_NEAR_OPTIMAL_PARSING
 
+/* Costs for the near-optimal parsing algorithm */
+struct deflate_costs {
+
+	/* The cost to output each possible literal */
+	u32 literal[DEFLATE_NUM_LITERALS];
+
+	/* The cost to output each possible match length */
+	u32 length[DEFLATE_MAX_MATCH_LEN + 1];
+
+	/* The cost to output a match offset of each possible offset slot */
+	u32 offset_slot[DEFLATE_NUM_OFFSET_SYMS];
+};
+
 /*
  * This structure represents a byte position in the input data and a node in the
  * graph of possible match/literal choices for the current block.
  *
  * Logically, each incoming edge to this node is labeled with a literal or a
  * match that can be taken to reach this position from an earlier position; and
  * each outgoing edge from this node is labeled with a literal or a match that
@@ -307,103 +454,114 @@
 };
 
 #endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
 
 /* Block split statistics.  See "Block splitting algorithm" below. */
 #define NUM_LITERAL_OBSERVATION_TYPES 8
 #define NUM_MATCH_OBSERVATION_TYPES 2
-#define NUM_OBSERVATION_TYPES (NUM_LITERAL_OBSERVATION_TYPES + NUM_MATCH_OBSERVATION_TYPES)
+#define NUM_OBSERVATION_TYPES (NUM_LITERAL_OBSERVATION_TYPES + \
+			       NUM_MATCH_OBSERVATION_TYPES)
+#define NUM_OBSERVATIONS_PER_BLOCK_CHECK 512
 struct block_split_stats {
 	u32 new_observations[NUM_OBSERVATION_TYPES];
 	u32 observations[NUM_OBSERVATION_TYPES];
 	u32 num_new_observations;
 	u32 num_observations;
 };
 
-/* The main DEFLATE compressor structure  */
+struct deflate_output_bitstream;
+
+/* The main DEFLATE compressor structure */
 struct libdeflate_compressor {
 
 	/* Pointer to the compress() implementation chosen at allocation time */
-	size_t (*impl)(struct libdeflate_compressor *,
-		       const u8 *, size_t, u8 *, size_t);
+	void (*impl)(struct libdeflate_compressor *restrict c, const u8 *in,
+		     size_t in_nbytes, struct deflate_output_bitstream *os);
 
-	/* Frequency counters for the current block  */
-	struct deflate_freqs freqs;
-
-	/* Dynamic Huffman codes for the current block  */
-	struct deflate_codes codes;
-
-	/* Static Huffman codes */
-	struct deflate_codes static_codes;
+	/* The compression level with which this compressor was created */
+	unsigned compression_level;
 
-	/* Block split statistics for the currently pending block */
-	struct block_split_stats split_stats;
+	/* Anything of this size or less we won't bother trying to compress. */
+	size_t max_passthrough_size;
 
-	/* A table for fast lookups of offset slot by match offset.
-	 *
-	 * If the full table is being used, it is a direct mapping from offset
-	 * to offset slot.
-	 *
-	 * If the condensed table is being used, the first 256 entries map
-	 * directly to the offset slots of offsets 1 through 256.  The next 256
-	 * entries map to the offset slots for the remaining offsets, stepping
-	 * through the offsets with a stride of 128.  This relies on the fact
-	 * that each of the remaining offset slots contains at least 128 offsets
-	 * and has an offset base that is a multiple of 128.  */
-#if USE_FULL_OFFSET_SLOT_FAST
-	u8 offset_slot_fast[DEFLATE_MAX_MATCH_OFFSET + 1];
-#else
-	u8 offset_slot_fast[512];
-#endif
+	/*
+	 * The maximum search depth: consider at most this many potential
+	 * matches at each position
+	 */
+	unsigned max_search_depth;
 
-	/* The "nice" match length: if a match of this length is found, choose
-	 * it immediately without further consideration.  */
+	/*
+	 * The "nice" match length: if a match of this length is found, choose
+	 * it immediately without further consideration
+	 */
 	unsigned nice_match_length;
 
-	/* The maximum search depth: consider at most this many potential
-	 * matches at each position.  */
-	unsigned max_search_depth;
+	/* Frequency counters for the current block */
+	struct deflate_freqs freqs;
 
-	/* The compression level with which this compressor was created.  */
-	unsigned compression_level;
+	/* Block split statistics for the current block */
+	struct block_split_stats split_stats;
+
+	/* Dynamic Huffman codes for the current block */
+	struct deflate_codes codes;
 
-	/* Anything smaller than this we won't bother trying to compress.  */
-	unsigned min_size_to_compress;
+	/* The static Huffman codes defined by the DEFLATE format */
+	struct deflate_codes static_codes;
 
-	/* Temporary space for Huffman code output  */
-	u32 precode_freqs[DEFLATE_NUM_PRECODE_SYMS];
-	u8 precode_lens[DEFLATE_NUM_PRECODE_SYMS];
-	u32 precode_codewords[DEFLATE_NUM_PRECODE_SYMS];
-	unsigned precode_items[DEFLATE_NUM_LITLEN_SYMS + DEFLATE_NUM_OFFSET_SYMS];
-	unsigned num_litlen_syms;
-	unsigned num_offset_syms;
-	unsigned num_explicit_lens;
-	unsigned num_precode_items;
+	/* Temporary space for block flushing */
+	union {
+		/* Information about the precode */
+		struct {
+			u32 freqs[DEFLATE_NUM_PRECODE_SYMS];
+			u32 codewords[DEFLATE_NUM_PRECODE_SYMS];
+			u8 lens[DEFLATE_NUM_PRECODE_SYMS];
+			unsigned items[DEFLATE_NUM_LITLEN_SYMS +
+				       DEFLATE_NUM_OFFSET_SYMS];
+			unsigned num_litlen_syms;
+			unsigned num_offset_syms;
+			unsigned num_explicit_lens;
+			unsigned num_items;
+		} precode;
+		/*
+		 * The "full" length codewords.  Used only after the information
+		 * in 'precode' is no longer needed.
+		 */
+		struct {
+			u32 codewords[DEFLATE_MAX_MATCH_LEN + 1];
+			u8 lens[DEFLATE_MAX_MATCH_LEN + 1];
+		} length;
+	} o;
 
 	union {
-		/* Data for greedy or lazy parsing  */
+		/* Data for greedy or lazy parsing */
 		struct {
-			/* Hash chain matchfinder  */
+			/* Hash chains matchfinder */
 			struct hc_matchfinder hc_mf;
 
-			/* The matches and literals that the parser has chosen
-			 * for the current block.  The required length of this
-			 * array is limited by the maximum number of matches
-			 * that can ever be chosen for a single block, plus one
-			 * for the special entry at the end.  */
-			struct deflate_sequence sequences[
-				DIV_ROUND_UP(SOFT_MAX_BLOCK_LENGTH,
-					     DEFLATE_MIN_MATCH_LEN) + 1];
+			/* Matches and literals chosen for the current block */
+			struct deflate_sequence sequences[SEQ_STORE_LENGTH + 1];
+
 		} g; /* (g)reedy */
 
+		/* Data for fastest parsing */
+		struct {
+			/* Hash table matchfinder */
+			struct ht_matchfinder ht_mf;
+
+			/* Matches and literals chosen for the current block */
+			struct deflate_sequence sequences[
+						FAST_SEQ_STORE_LENGTH + 1];
+
+		} f; /* (f)astest */
+
 	#if SUPPORT_NEAR_OPTIMAL_PARSING
-		/* Data for near-optimal parsing  */
+		/* Data for near-optimal parsing */
 		struct {
 
-			/* Binary tree matchfinder  */
+			/* Binary tree matchfinder */
 			struct bt_matchfinder bt_mf;
 
 			/*
 			 * Cached matches for the current block.  This array
 			 * contains the matches that were found at each position
 			 * in the block.  Specifically, for each position, there
 			 * is a list of matches found at that position, if any,
@@ -413,174 +571,198 @@
 			 * contains the number of matches found at that
 			 * position, and whose 'offset' member contains the
 			 * literal at that position.
 			 *
 			 * Note: in rare cases, there will be a very high number
 			 * of matches in the block and this array will overflow.
 			 * If this happens, we force the end of the current
-			 * block.  CACHE_LENGTH is the length at which we
+			 * block.  MATCH_CACHE_LENGTH is the length at which we
 			 * actually check for overflow.  The extra slots beyond
 			 * this are enough to absorb the worst case overflow,
-			 * which occurs if starting at &match_cache[CACHE_LENGTH
-			 * - 1], we write MAX_MATCHES_PER_POS matches and a
-			 * match count header, then skip searching for matches
-			 * at 'DEFLATE_MAX_MATCH_LEN - 1' positions and write
-			 * the match count header for each.
+			 * which occurs if starting at
+			 * &match_cache[MATCH_CACHE_LENGTH - 1], we write
+			 * MAX_MATCHES_PER_POS matches and a match count header,
+			 * then skip searching for matches at
+			 * 'DEFLATE_MAX_MATCH_LEN - 1' positions and write the
+			 * match count header for each.
 			 */
-			struct lz_match match_cache[CACHE_LENGTH +
+			struct lz_match match_cache[MATCH_CACHE_LENGTH +
 						    MAX_MATCHES_PER_POS +
 						    DEFLATE_MAX_MATCH_LEN - 1];
 
 			/*
 			 * Array of nodes, one per position, for running the
 			 * minimum-cost path algorithm.
 			 *
 			 * This array must be large enough to accommodate the
-			 * worst-case number of nodes, which occurs if we find a
-			 * match of length DEFLATE_MAX_MATCH_LEN at position
-			 * SOFT_MAX_BLOCK_LENGTH - 1, producing a block of
-			 * length SOFT_MAX_BLOCK_LENGTH - 1 +
-			 * DEFLATE_MAX_MATCH_LEN.  Add one for the end-of-block
-			 * node.
+			 * worst-case number of nodes, which is MAX_BLOCK_LENGTH
+			 * plus 1 for the end-of-block node.
 			 */
-			struct deflate_optimum_node optimum_nodes[SOFT_MAX_BLOCK_LENGTH - 1 +
-								  DEFLATE_MAX_MATCH_LEN + 1];
+			struct deflate_optimum_node optimum_nodes[
+				MAX_BLOCK_LENGTH + 1];
 
-			/* The current cost model being used.  */
+			/* The current cost model being used */
 			struct deflate_costs costs;
 
-			unsigned num_optim_passes;
+			struct deflate_costs costs_producing_best_true_cost;
+
+			/*
+			 * A table that maps match offset to offset slot.  This
+			 * differs from deflate_offset_slot[] in that this is a
+			 * full map, not a condensed one.  The full map is more
+			 * appropriate for the near-optimal parser, since the
+			 * near-optimal parser does more offset => offset_slot
+			 * translations, it doesn't intersperse them with
+			 * matchfinding (so cache evictions are less of a
+			 * concern), and it uses more memory anyway.
+			 */
+			u8 offset_slot_full[DEFLATE_MAX_MATCH_OFFSET + 1];
+
+			/* Literal/match statistics saved from previous block */
+			u32 prev_observations[NUM_OBSERVATION_TYPES];
+			u32 prev_num_observations;
+
+			/*
+			 * Approximate match length frequencies based on a
+			 * greedy parse, gathered during matchfinding.  This is
+			 * used for setting the initial symbol costs.
+			 */
+			u32 new_match_len_freqs[DEFLATE_MAX_MATCH_LEN + 1];
+			u32 match_len_freqs[DEFLATE_MAX_MATCH_LEN + 1];
+
+			/*
+			 * The maximum number of optimization passes
+			 * (min-cost path searches) per block.
+			 * Larger values = more compression.
+			 */
+			unsigned max_optim_passes;
+
+			/*
+			 * If an optimization pass improves the cost by fewer
+			 * than this number of bits, then optimization will stop
+			 * early, before max_optim_passes has been reached.
+			 * Smaller values = more compression.
+			 */
+			unsigned min_improvement_to_continue;
+
+			/*
+			 * The minimum number of bits that would need to be
+			 * saved for it to be considered worth the time to
+			 * regenerate and use the min-cost path from a previous
+			 * optimization pass, in the case where the final
+			 * optimization pass actually increased the cost.
+			 * Smaller values = more compression.
+			 */
+			unsigned min_bits_to_use_nonfinal_path;
+
 		} n; /* (n)ear-optimal */
 	#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
 
 	} p; /* (p)arser */
 };
 
 /*
  * The type for the bitbuffer variable, which temporarily holds bits that are
  * being packed into bytes and written to the output buffer.  For best
  * performance, this should have size equal to a machine word.
  */
 typedef machine_word_t bitbuf_t;
-#define BITBUF_NBITS	(8 * sizeof(bitbuf_t))
 
-/* Can the specified number of bits always be added to 'bitbuf' after any
- * pending bytes have been flushed?  */
-#define CAN_BUFFER(n)	((n) <= BITBUF_NBITS - 7)
+/*
+ * The capacity of the bitbuffer, in bits.  This is 1 less than the real size,
+ * in order to avoid undefined behavior when doing bitbuf >>= bitcount & ~7.
+ */
+#define BITBUF_NBITS	(8 * sizeof(bitbuf_t) - 1)
+
+/*
+ * Can the specified number of bits always be added to 'bitbuf' after any
+ * pending bytes have been flushed?  There can be up to 7 bits remaining after a
+ * flush, so the count must not exceed BITBUF_NBITS after adding 'n' more bits.
+ */
+#define CAN_BUFFER(n)	(7 + (n) <= BITBUF_NBITS)
 
 /*
  * Structure to keep track of the current state of sending bits to the
- * compressed output buffer.
+ * compressed output buffer
  */
 struct deflate_output_bitstream {
 
-	/* Bits that haven't yet been written to the output buffer.  */
+	/* Bits that haven't yet been written to the output buffer */
 	bitbuf_t bitbuf;
 
-	/* Number of bits currently held in @bitbuf.  */
+	/*
+	 * Number of bits currently held in @bitbuf.  This can be between 0 and
+	 * BITBUF_NBITS in general, or between 0 and 7 after a flush.
+	 */
 	unsigned bitcount;
 
-	/* Pointer to the beginning of the output buffer.  */
-	u8 *begin;
-
-	/* Pointer to the position in the output buffer at which the next byte
-	 * should be written.  */
+	/*
+	 * Pointer to the position in the output buffer at which the next byte
+	 * should be written
+	 */
 	u8 *next;
 
-	/* Pointer just past the end of the output buffer.  */
+	/*
+	 * Pointer to near the end of the output buffer.  'next' will never
+	 * exceed this.  There are OUTPUT_END_PADDING bytes reserved after this
+	 * to allow branchlessly writing a whole word at this location.
+	 */
 	u8 *end;
 };
 
 /*
  * OUTPUT_END_PADDING is the size, in bytes, of the extra space that must be
  * present following os->end, in order to not overrun the buffer when generating
  * output.  When UNALIGNED_ACCESS_IS_FAST, we need at least sizeof(bitbuf_t)
  * bytes for put_unaligned_leword().  Otherwise we need only 1 byte.  However,
  * to make the compression algorithm produce the same result on all CPU
  * architectures (which is sometimes desirable), we have to unconditionally use
  * the maximum for any CPU, which is sizeof(bitbuf_t) == 8.
  */
 #define OUTPUT_END_PADDING	8
 
-/* Initialize the output bitstream.  'size' is assumed to be at least
- * OUTPUT_END_PADDING.  */
-static void
-deflate_init_output(struct deflate_output_bitstream *os,
-		    void *buffer, size_t size)
-{
-	os->bitbuf = 0;
-	os->bitcount = 0;
-	os->begin = buffer;
-	os->next = os->begin;
-	os->end = os->begin + size - OUTPUT_END_PADDING;
-}
-
-/* Add some bits to the bitbuffer variable of the output bitstream.  The caller
- * must make sure there is enough room.  */
-static forceinline void
-deflate_add_bits(struct deflate_output_bitstream *os,
-		 const bitbuf_t bits, const unsigned num_bits)
-{
-	os->bitbuf |= bits << os->bitcount;
-	os->bitcount += num_bits;
-}
-
-/* Flush bits from the bitbuffer variable to the output buffer.  */
-static forceinline void
-deflate_flush_bits(struct deflate_output_bitstream *os)
-{
-	if (UNALIGNED_ACCESS_IS_FAST) {
-		/* Flush a whole word (branchlessly).  */
-		put_unaligned_leword(os->bitbuf, os->next);
-		os->bitbuf >>= os->bitcount & ~7;
-		os->next += MIN(os->end - os->next, os->bitcount >> 3);
-		os->bitcount &= 7;
-	} else {
-		/* Flush a byte at a time.  */
-		while (os->bitcount >= 8) {
-			*os->next = os->bitbuf;
-			if (os->next != os->end)
-				os->next++;
-			os->bitcount -= 8;
-			os->bitbuf >>= 8;
-		}
-	}
-}
-
-/* Align the bitstream on a byte boundary. */
-static forceinline void
-deflate_align_bitstream(struct deflate_output_bitstream *os)
-{
-	os->bitcount += -os->bitcount & 7;
-	deflate_flush_bits(os);
-}
-
 /*
- * Flush any remaining bits to the output buffer if needed.  Return the total
- * number of bytes written to the output buffer, or 0 if an overflow occurred.
+ * Add some bits to the bitbuffer variable of the output bitstream.  The caller
+ * must ensure that 'bitcount + n <= BITBUF_NBITS', by calling FLUSH_BITS()
+ * frequently enough.
+ */
+#define ADD_BITS(bits, n)			\
+do {						\
+	bitbuf |= (bitbuf_t)(bits) << bitcount;	\
+	bitcount += (n);			\
+	ASSERT(bitcount <= BITBUF_NBITS);	\
+} while (0)
+
+/* Flush bits from the bitbuffer variable to the output buffer. */
+#define FLUSH_BITS()							\
+do {									\
+	if (UNALIGNED_ACCESS_IS_FAST) {					\
+		/* Flush a whole word (branchlessly). */		\
+		put_unaligned_leword(bitbuf, out_next);			\
+		bitbuf >>= bitcount & ~7;				\
+		out_next += MIN(out_end - out_next, bitcount >> 3);	\
+		bitcount &= 7;						\
+	} else {							\
+		/* Flush a byte at a time. */				\
+		while (bitcount >= 8) {					\
+			*out_next = bitbuf;				\
+			if (out_next != out_end)			\
+				out_next++;				\
+			bitcount -= 8;					\
+			bitbuf >>= 8;					\
+		}							\
+	}								\
+} while (0)
+
+/*
+ * Given the binary tree node A[subtree_idx] whose children already satisfy the
+ * maxheap property, swap the node with its greater child until it is greater
+ * than or equal to both of its children, so that the maxheap property is
+ * satisfied in the subtree rooted at A[subtree_idx].  'A' uses 1-based indices.
  */
-static size_t
-deflate_flush_output(struct deflate_output_bitstream *os)
-{
-	if (os->next == os->end) /* overflow?  */
-		return 0;
-
-	while ((int)os->bitcount > 0) {
-		*os->next++ = os->bitbuf;
-		os->bitcount -= 8;
-		os->bitbuf >>= 8;
-	}
-
-	return os->next - os->begin;
-}
-
-/* Given the binary tree node A[subtree_idx] whose children already
- * satisfy the maxheap property, swap the node with its greater child
- * until it is greater than both its children, so that the maxheap
- * property is satisfied in the subtree rooted at A[subtree_idx].  */
 static void
 heapify_subtree(u32 A[], unsigned length, unsigned subtree_idx)
 {
 	unsigned parent_idx;
 	unsigned child_idx;
 	u32 v;
 
@@ -593,15 +775,16 @@
 			break;
 		A[parent_idx] = A[child_idx];
 		parent_idx = child_idx;
 	}
 	A[parent_idx] = v;
 }
 
-/* Rearrange the array 'A' so that it satisfies the maxheap property.
+/*
+ * Rearrange the array 'A' so that it satisfies the maxheap property.
  * 'A' uses 1-based indices, so the children of A[i] are A[i*2] and A[i*2 + 1].
  */
 static void
 heapify_array(u32 A[], unsigned length)
 {
 	unsigned subtree_idx;
 
@@ -609,319 +792,373 @@
 		heapify_subtree(A, length, subtree_idx);
 }
 
 /*
  * Sort the array 'A', which contains 'length' unsigned 32-bit integers.
  *
  * Note: name this function heap_sort() instead of heapsort() to avoid colliding
- * with heapsort() from stdlib.h on BSD-derived systems --- though this isn't
- * necessary when compiling with -D_ANSI_SOURCE, which is the better solution.
+ * with heapsort() from stdlib.h on BSD-derived systems.
  */
 static void
 heap_sort(u32 A[], unsigned length)
 {
 	A--; /* Use 1-based indices  */
 
 	heapify_array(A, length);
 
 	while (length >= 2) {
 		u32 tmp = A[length];
+
 		A[length] = A[1];
 		A[1] = tmp;
 		length--;
 		heapify_subtree(A, length, 1);
 	}
 }
 
 #define NUM_SYMBOL_BITS 10
-#define SYMBOL_MASK ((1 << NUM_SYMBOL_BITS) - 1)
+#define NUM_FREQ_BITS	(32 - NUM_SYMBOL_BITS)
+#define SYMBOL_MASK	((1 << NUM_SYMBOL_BITS) - 1)
+#define FREQ_MASK	(~SYMBOL_MASK)
+
+#define GET_NUM_COUNTERS(num_syms)	(num_syms)
 
-#define GET_NUM_COUNTERS(num_syms)	((((num_syms) + 3 / 4) + 3) & ~3)
 /*
- * Sort the symbols primarily by frequency and secondarily by symbol
- * value.  Discard symbols with zero frequency and fill in an array with
- * the remaining symbols, along with their frequencies.  The low
- * NUM_SYMBOL_BITS bits of each array entry will contain the symbol
- * value, and the remaining bits will contain the frequency.
+ * Sort the symbols primarily by frequency and secondarily by symbol value.
+ * Discard symbols with zero frequency and fill in an array with the remaining
+ * symbols, along with their frequencies.  The low NUM_SYMBOL_BITS bits of each
+ * array entry will contain the symbol value, and the remaining bits will
+ * contain the frequency.
  *
  * @num_syms
- *	Number of symbols in the alphabet.
- *	Can't be greater than (1 << NUM_SYMBOL_BITS).
+ *	Number of symbols in the alphabet, at most 1 << NUM_SYMBOL_BITS.
  *
  * @freqs[num_syms]
- *	The frequency of each symbol.
+ *	Frequency of each symbol, summing to at most (1 << NUM_FREQ_BITS) - 1.
  *
  * @lens[num_syms]
- *	An array that eventually will hold the length of each codeword.
- *	This function only fills in the codeword lengths for symbols that
- *	have zero frequency, which are not well defined per se but will
- *	be set to 0.
+ *	An array that eventually will hold the length of each codeword.  This
+ *	function only fills in the codeword lengths for symbols that have zero
+ *	frequency, which are not well defined per se but will be set to 0.
  *
  * @symout[num_syms]
  *	The output array, described above.
  *
- * Returns the number of entries in 'symout' that were filled.  This is
- * the number of symbols that have nonzero frequency.
+ * Returns the number of entries in 'symout' that were filled.  This is the
+ * number of symbols that have nonzero frequency.
  */
 static unsigned
-sort_symbols(unsigned num_syms, const u32 freqs[restrict],
-	     u8 lens[restrict], u32 symout[restrict])
+sort_symbols(unsigned num_syms, const u32 freqs[], u8 lens[], u32 symout[])
 {
 	unsigned sym;
 	unsigned i;
 	unsigned num_used_syms;
 	unsigned num_counters;
 	unsigned counters[GET_NUM_COUNTERS(DEFLATE_MAX_NUM_SYMS)];
 
-	/* We rely on heapsort, but with an added optimization.  Since
-	 * it's common for most symbol frequencies to be low, we first do
-	 * a count sort using a limited number of counters.  High
-	 * frequencies will be counted in the last counter, and only they
-	 * will be sorted with heapsort.
+	/*
+	 * We use heapsort, but with an added optimization.  Since often most
+	 * symbol frequencies are low, we first do a count sort using a limited
+	 * number of counters.  High frequencies are counted in the last
+	 * counter, and only they will be sorted with heapsort.
 	 *
 	 * Note: with more symbols, it is generally beneficial to have more
-	 * counters.  About 1 counter per 4 symbols seems fast.
-	 *
-	 * Note: I also tested radix sort, but even for large symbol
-	 * counts (> 255) and frequencies bounded at 16 bits (enabling
-	 * radix sort by just two base-256 digits), it didn't seem any
-	 * faster than the method implemented here.
-	 *
-	 * Note: I tested the optimized quicksort implementation from
-	 * glibc (with indirection overhead removed), but it was only
-	 * marginally faster than the simple heapsort implemented here.
-	 *
-	 * Tests were done with building the codes for LZX.  Results may
-	 * vary for different compression algorithms...!  */
+	 * counters.  About 1 counter per symbol seems fastest.
+	 */
 
 	num_counters = GET_NUM_COUNTERS(num_syms);
 
 	memset(counters, 0, num_counters * sizeof(counters[0]));
 
-	/* Count the frequencies.  */
+	/* Count the frequencies. */
 	for (sym = 0; sym < num_syms; sym++)
 		counters[MIN(freqs[sym], num_counters - 1)]++;
 
-	/* Make the counters cumulative, ignoring the zero-th, which
-	 * counted symbols with zero frequency.  As a side effect, this
-	 * calculates the number of symbols with nonzero frequency.  */
+	/*
+	 * Make the counters cumulative, ignoring the zero-th, which counted
+	 * symbols with zero frequency.  As a side effect, this calculates the
+	 * number of symbols with nonzero frequency.
+	 */
 	num_used_syms = 0;
 	for (i = 1; i < num_counters; i++) {
 		unsigned count = counters[i];
+
 		counters[i] = num_used_syms;
 		num_used_syms += count;
 	}
 
-	/* Sort nonzero-frequency symbols using the counters.  At the
-	 * same time, set the codeword lengths of zero-frequency symbols
-	 * to 0.  */
+	/*
+	 * Sort nonzero-frequency symbols using the counters.  At the same time,
+	 * set the codeword lengths of zero-frequency symbols to 0.
+	 */
 	for (sym = 0; sym < num_syms; sym++) {
 		u32 freq = freqs[sym];
+
 		if (freq != 0) {
 			symout[counters[MIN(freq, num_counters - 1)]++] =
 				sym | (freq << NUM_SYMBOL_BITS);
 		} else {
 			lens[sym] = 0;
 		}
 	}
 
-	/* Sort the symbols counted in the last counter.  */
+	/* Sort the symbols counted in the last counter. */
 	heap_sort(symout + counters[num_counters - 2],
 		  counters[num_counters - 1] - counters[num_counters - 2]);
 
 	return num_used_syms;
 }
 
 /*
- * Build the Huffman tree.
+ * Build a Huffman tree.
  *
  * This is an optimized implementation that
  *	(a) takes advantage of the frequencies being already sorted;
- *	(b) only generates non-leaf nodes, since the non-leaf nodes of a
- *	    Huffman tree are sufficient to generate a canonical code;
+ *	(b) only generates non-leaf nodes, since the non-leaf nodes of a Huffman
+ *	    tree are sufficient to generate a canonical code;
  *	(c) Only stores parent pointers, not child pointers;
- *	(d) Produces the nodes in the same memory used for input
- *	    frequency information.
+ *	(d) Produces the nodes in the same memory used for input frequency
+ *	    information.
  *
- * Array 'A', which contains 'sym_count' entries, is used for both input
- * and output.  For this function, 'sym_count' must be at least 2.
+ * Array 'A', which contains 'sym_count' entries, is used for both input and
+ * output.  For this function, 'sym_count' must be at least 2.
  *
- * For input, the array must contain the frequencies of the symbols,
- * sorted in increasing order.  Specifically, each entry must contain a
- * frequency left shifted by NUM_SYMBOL_BITS bits.  Any data in the low
- * NUM_SYMBOL_BITS bits of the entries will be ignored by this function.
- * Although these bits will, in fact, contain the symbols that correspond
- * to the frequencies, this function is concerned with frequencies only
- * and keeps the symbols as-is.
- *
- * For output, this function will produce the non-leaf nodes of the
- * Huffman tree.  These nodes will be stored in the first (sym_count - 1)
- * entries of the array.  Entry A[sym_count - 2] will represent the root
- * node.  Each other node will contain the zero-based index of its parent
- * node in 'A', left shifted by NUM_SYMBOL_BITS bits.  The low
- * NUM_SYMBOL_BITS bits of each entry in A will be kept as-is.  Again,
- * note that although these low bits will, in fact, contain a symbol
- * value, this symbol will have *no relationship* with the Huffman tree
- * node that happens to occupy the same slot.  This is because this
+ * For input, the array must contain the frequencies of the symbols, sorted in
+ * increasing order.  Specifically, each entry must contain a frequency left
+ * shifted by NUM_SYMBOL_BITS bits.  Any data in the low NUM_SYMBOL_BITS bits of
+ * the entries will be ignored by this function.  Although these bits will, in
+ * fact, contain the symbols that correspond to the frequencies, this function
+ * is concerned with frequencies only and keeps the symbols as-is.
+ *
+ * For output, this function will produce the non-leaf nodes of the Huffman
+ * tree.  These nodes will be stored in the first (sym_count - 1) entries of the
+ * array.  Entry A[sym_count - 2] will represent the root node.  Each other node
+ * will contain the zero-based index of its parent node in 'A', left shifted by
+ * NUM_SYMBOL_BITS bits.  The low NUM_SYMBOL_BITS bits of each entry in A will
+ * be kept as-is.  Again, note that although these low bits will, in fact,
+ * contain a symbol value, this symbol will have *no relationship* with the
+ * Huffman tree node that happens to occupy the same slot.  This is because this
  * implementation only generates the non-leaf nodes of the tree.
  */
 static void
 build_tree(u32 A[], unsigned sym_count)
 {
-	/* Index, in 'A', of next lowest frequency symbol that has not
-	 * yet been processed.  */
+	const unsigned last_idx = sym_count - 1;
+
+	/* Index of the next lowest frequency leaf that still needs a parent */
 	unsigned i = 0;
 
-	/* Index, in 'A', of next lowest frequency parentless non-leaf
-	 * node; or, if equal to 'e', then no such node exists yet.  */
+	/*
+	 * Index of the next lowest frequency non-leaf that still needs a
+	 * parent, or 'e' if there is currently no such node
+	 */
 	unsigned b = 0;
 
-	/* Index, in 'A', of next node to allocate as a non-leaf.  */
+	/* Index of the next spot for a non-leaf (will overwrite a leaf) */
 	unsigned e = 0;
 
 	do {
-		unsigned m, n;
-		u32 freq_shifted;
-
-		/* Choose the two next lowest frequency entries.  */
-
-		if (i != sym_count &&
-		    (b == e || (A[i] >> NUM_SYMBOL_BITS) <= (A[b] >> NUM_SYMBOL_BITS)))
-			m = i++;
-		else
-			m = b++;
-
-		if (i != sym_count &&
-		    (b == e || (A[i] >> NUM_SYMBOL_BITS) <= (A[b] >> NUM_SYMBOL_BITS)))
-			n = i++;
-		else
-			n = b++;
+		u32 new_freq;
 
-		/* Allocate a non-leaf node and link the entries to it.
-		 *
-		 * If we link an entry that we're visiting for the first
-		 * time (via index 'i'), then we're actually linking a
-		 * leaf node and it will have no effect, since the leaf
-		 * will be overwritten with a non-leaf when index 'e'
-		 * catches up to it.  But it's not any slower to
-		 * unconditionally set the parent index.
+		/*
+		 * Select the next two lowest frequency nodes among the leaves
+		 * A[i] and non-leaves A[b], and create a new node A[e] to be
+		 * their parent.  Set the new node's frequency to the sum of the
+		 * frequencies of its two children.
 		 *
-		 * We also compute the frequency of the non-leaf node as
-		 * the sum of its two children's frequencies.  */
-
-		freq_shifted = (A[m] & ~SYMBOL_MASK) + (A[n] & ~SYMBOL_MASK);
-
-		A[m] = (A[m] & SYMBOL_MASK) | (e << NUM_SYMBOL_BITS);
-		A[n] = (A[n] & SYMBOL_MASK) | (e << NUM_SYMBOL_BITS);
-		A[e] = (A[e] & SYMBOL_MASK) | freq_shifted;
-		e++;
-	} while (sym_count - e > 1);
-		/* When just one entry remains, it is a "leaf" that was
-		 * linked to some other node.  We ignore it, since the
-		 * rest of the array contains the non-leaves which we
-		 * need.  (Note that we're assuming the cases with 0 or 1
-		 * symbols were handled separately.) */
+		 * Usually the next two lowest frequency nodes are of the same
+		 * type (leaf or non-leaf), so check those cases first.
+		 */
+		if (i + 1 <= last_idx &&
+		    (b == e || (A[i + 1] & FREQ_MASK) <= (A[b] & FREQ_MASK))) {
+			/* Two leaves */
+			new_freq = (A[i] & FREQ_MASK) + (A[i + 1] & FREQ_MASK);
+			i += 2;
+		} else if (b + 2 <= e &&
+			   (i > last_idx ||
+			    (A[b + 1] & FREQ_MASK) < (A[i] & FREQ_MASK))) {
+			/* Two non-leaves */
+			new_freq = (A[b] & FREQ_MASK) + (A[b + 1] & FREQ_MASK);
+			A[b] = (e << NUM_SYMBOL_BITS) | (A[b] & SYMBOL_MASK);
+			A[b + 1] = (e << NUM_SYMBOL_BITS) |
+				   (A[b + 1] & SYMBOL_MASK);
+			b += 2;
+		} else {
+			/* One leaf and one non-leaf */
+			new_freq = (A[i] & FREQ_MASK) + (A[b] & FREQ_MASK);
+			A[b] = (e << NUM_SYMBOL_BITS) | (A[b] & SYMBOL_MASK);
+			i++;
+			b++;
+		}
+		A[e] = new_freq | (A[e] & SYMBOL_MASK);
+		/*
+		 * A binary tree with 'n' leaves has 'n - 1' non-leaves, so the
+		 * tree is complete once we've created 'n - 1' non-leaves.
+		 */
+	} while (++e < last_idx);
 }
 
 /*
- * Given the stripped-down Huffman tree constructed by build_tree(),
- * determine the number of codewords that should be assigned each
- * possible length, taking into account the length-limited constraint.
+ * Given the stripped-down Huffman tree constructed by build_tree(), determine
+ * the number of codewords that should be assigned each possible length, taking
+ * into account the length-limited constraint.
  *
  * @A
- *	The array produced by build_tree(), containing parent index
- *	information for the non-leaf nodes of the Huffman tree.  Each
- *	entry in this array is a node; a node's parent always has a
- *	greater index than that node itself.  This function will
- *	overwrite the parent index information in this array, so
- *	essentially it will destroy the tree.  However, the data in the
- *	low NUM_SYMBOL_BITS of each entry will be preserved.
+ *	The array produced by build_tree(), containing parent index information
+ *	for the non-leaf nodes of the Huffman tree.  Each entry in this array is
+ *	a node; a node's parent always has a greater index than that node
+ *	itself.  This function will overwrite the parent index information in
+ *	this array, so essentially it will destroy the tree.  However, the data
+ *	in the low NUM_SYMBOL_BITS of each entry will be preserved.
  *
  * @root_idx
- *	The 0-based index of the root node in 'A', and consequently one
- *	less than the number of tree node entries in 'A'.  (Or, really 2
- *	less than the actual length of 'A'.)
+ *	The 0-based index of the root node in 'A', and consequently one less
+ *	than the number of tree node entries in 'A'.  (Or, really 2 less than
+ *	the actual length of 'A'.)
  *
  * @len_counts
  *	An array of length ('max_codeword_len' + 1) in which the number of
- *	codewords having each length <= max_codeword_len will be
- *	returned.
+ *	codewords having each length <= max_codeword_len will be returned.
  *
  * @max_codeword_len
  *	The maximum permissible codeword length.
  */
 static void
-compute_length_counts(u32 A[restrict], unsigned root_idx,
-		      unsigned len_counts[restrict], unsigned max_codeword_len)
+compute_length_counts(u32 A[], unsigned root_idx, unsigned len_counts[],
+		      unsigned max_codeword_len)
 {
 	unsigned len;
 	int node;
 
-	/* The key observations are:
+	/*
+	 * The key observations are:
 	 *
-	 * (1) We can traverse the non-leaf nodes of the tree, always
-	 * visiting a parent before its children, by simply iterating
-	 * through the array in reverse order.  Consequently, we can
-	 * compute the depth of each node in one pass, overwriting the
-	 * parent indices with depths.
+	 * (1) We can traverse the non-leaf nodes of the tree, always visiting a
+	 *     parent before its children, by simply iterating through the array
+	 *     in reverse order.  Consequently, we can compute the depth of each
+	 *     node in one pass, overwriting the parent indices with depths.
 	 *
-	 * (2) We can initially assume that in the real Huffman tree,
-	 * both children of the root are leaves.  This corresponds to two
-	 * codewords of length 1.  Then, whenever we visit a (non-leaf)
-	 * node during the traversal, we modify this assumption to
-	 * account for the current node *not* being a leaf, but rather
-	 * its two children being leaves.  This causes the loss of one
-	 * codeword for the current depth and the addition of two
-	 * codewords for the current depth plus one.
+	 * (2) We can initially assume that in the real Huffman tree, both
+	 *     children of the root are leaves.  This corresponds to two
+	 *     codewords of length 1.  Then, whenever we visit a (non-leaf) node
+	 *     during the traversal, we modify this assumption to account for
+	 *     the current node *not* being a leaf, but rather its two children
+	 *     being leaves.  This causes the loss of one codeword for the
+	 *     current depth and the addition of two codewords for the current
+	 *     depth plus one.
 	 *
-	 * (3) We can handle the length-limited constraint fairly easily
-	 * by simply using the largest length available when a depth
-	 * exceeds max_codeword_len.
+	 * (3) We can handle the length-limited constraint fairly easily by
+	 *     simply using the largest length available when a depth exceeds
+	 *     max_codeword_len.
 	 */
 
 	for (len = 0; len <= max_codeword_len; len++)
 		len_counts[len] = 0;
 	len_counts[1] = 2;
 
-	/* Set the root node's depth to 0.  */
+	/* Set the root node's depth to 0. */
 	A[root_idx] &= SYMBOL_MASK;
 
 	for (node = root_idx - 1; node >= 0; node--) {
 
-		/* Calculate the depth of this node.  */
+		/* Calculate the depth of this node. */
 
 		unsigned parent = A[node] >> NUM_SYMBOL_BITS;
 		unsigned parent_depth = A[parent] >> NUM_SYMBOL_BITS;
 		unsigned depth = parent_depth + 1;
-		unsigned len = depth;
-
-		/* Set the depth of this node so that it is available
-		 * when its children (if any) are processed.  */
 
+		/*
+		 * Set the depth of this node so that it is available when its
+		 * children (if any) are processed.
+		 */
 		A[node] = (A[node] & SYMBOL_MASK) | (depth << NUM_SYMBOL_BITS);
 
-		/* If needed, decrease the length to meet the
-		 * length-limited constraint.  This is not the optimal
-		 * method for generating length-limited Huffman codes!
-		 * But it should be good enough.  */
-		if (len >= max_codeword_len) {
-			len = max_codeword_len;
+		/*
+		 * If needed, decrease the length to meet the length-limited
+		 * constraint.  This is not the optimal method for generating
+		 * length-limited Huffman codes!  But it should be good enough.
+		 */
+		if (depth >= max_codeword_len) {
+			depth = max_codeword_len;
 			do {
-				len--;
-			} while (len_counts[len] == 0);
+				depth--;
+			} while (len_counts[depth] == 0);
 		}
 
-		/* Account for the fact that we have a non-leaf node at
-		 * the current depth.  */
-		len_counts[len]--;
-		len_counts[len + 1] += 2;
+		/*
+		 * Account for the fact that we have a non-leaf node at the
+		 * current depth.
+		 */
+		len_counts[depth]--;
+		len_counts[depth + 1] += 2;
 	}
 }
 
 /*
+ * DEFLATE uses bit-reversed codewords, so we must bit-reverse the codewords
+ * after generating them.  All codewords have length <= 16 bits.  If the CPU has
+ * a bit-reversal instruction, then that is the fastest method.  Otherwise the
+ * fastest method is to reverse the bits in each of the two bytes using a table.
+ * The table method is slightly faster than using bitwise operations to flip
+ * adjacent 1, 2, 4, and then 8-bit fields, even if 2 to 4 codewords are packed
+ * into a machine word and processed together using that method.
+ */
+
+#ifdef rbit32
+static forceinline u32 reverse_codeword(u32 codeword, u8 len)
+{
+	return rbit32(codeword) >> ((32 - len) & 31);
+}
+#else
+/* Generated by scripts/gen_bitreverse_tab.py */
+static const u8 bitreverse_tab[256] = {
+	0x00, 0x80, 0x40, 0xc0, 0x20, 0xa0, 0x60, 0xe0,
+	0x10, 0x90, 0x50, 0xd0, 0x30, 0xb0, 0x70, 0xf0,
+	0x08, 0x88, 0x48, 0xc8, 0x28, 0xa8, 0x68, 0xe8,
+	0x18, 0x98, 0x58, 0xd8, 0x38, 0xb8, 0x78, 0xf8,
+	0x04, 0x84, 0x44, 0xc4, 0x24, 0xa4, 0x64, 0xe4,
+	0x14, 0x94, 0x54, 0xd4, 0x34, 0xb4, 0x74, 0xf4,
+	0x0c, 0x8c, 0x4c, 0xcc, 0x2c, 0xac, 0x6c, 0xec,
+	0x1c, 0x9c, 0x5c, 0xdc, 0x3c, 0xbc, 0x7c, 0xfc,
+	0x02, 0x82, 0x42, 0xc2, 0x22, 0xa2, 0x62, 0xe2,
+	0x12, 0x92, 0x52, 0xd2, 0x32, 0xb2, 0x72, 0xf2,
+	0x0a, 0x8a, 0x4a, 0xca, 0x2a, 0xaa, 0x6a, 0xea,
+	0x1a, 0x9a, 0x5a, 0xda, 0x3a, 0xba, 0x7a, 0xfa,
+	0x06, 0x86, 0x46, 0xc6, 0x26, 0xa6, 0x66, 0xe6,
+	0x16, 0x96, 0x56, 0xd6, 0x36, 0xb6, 0x76, 0xf6,
+	0x0e, 0x8e, 0x4e, 0xce, 0x2e, 0xae, 0x6e, 0xee,
+	0x1e, 0x9e, 0x5e, 0xde, 0x3e, 0xbe, 0x7e, 0xfe,
+	0x01, 0x81, 0x41, 0xc1, 0x21, 0xa1, 0x61, 0xe1,
+	0x11, 0x91, 0x51, 0xd1, 0x31, 0xb1, 0x71, 0xf1,
+	0x09, 0x89, 0x49, 0xc9, 0x29, 0xa9, 0x69, 0xe9,
+	0x19, 0x99, 0x59, 0xd9, 0x39, 0xb9, 0x79, 0xf9,
+	0x05, 0x85, 0x45, 0xc5, 0x25, 0xa5, 0x65, 0xe5,
+	0x15, 0x95, 0x55, 0xd5, 0x35, 0xb5, 0x75, 0xf5,
+	0x0d, 0x8d, 0x4d, 0xcd, 0x2d, 0xad, 0x6d, 0xed,
+	0x1d, 0x9d, 0x5d, 0xdd, 0x3d, 0xbd, 0x7d, 0xfd,
+	0x03, 0x83, 0x43, 0xc3, 0x23, 0xa3, 0x63, 0xe3,
+	0x13, 0x93, 0x53, 0xd3, 0x33, 0xb3, 0x73, 0xf3,
+	0x0b, 0x8b, 0x4b, 0xcb, 0x2b, 0xab, 0x6b, 0xeb,
+	0x1b, 0x9b, 0x5b, 0xdb, 0x3b, 0xbb, 0x7b, 0xfb,
+	0x07, 0x87, 0x47, 0xc7, 0x27, 0xa7, 0x67, 0xe7,
+	0x17, 0x97, 0x57, 0xd7, 0x37, 0xb7, 0x77, 0xf7,
+	0x0f, 0x8f, 0x4f, 0xcf, 0x2f, 0xaf, 0x6f, 0xef,
+	0x1f, 0x9f, 0x5f, 0xdf, 0x3f, 0xbf, 0x7f, 0xff,
+};
+
+static forceinline u32 reverse_codeword(u32 codeword, u8 len)
+{
+	STATIC_ASSERT(DEFLATE_MAX_CODEWORD_LEN <= 16);
+	codeword = ((u32)bitreverse_tab[codeword & 0xff] << 8) |
+		   bitreverse_tab[codeword >> 8];
+	return codeword >> (16 - len);
+}
+#endif /* !rbit32 */
+
+/*
  * Generate the codewords for a canonical Huffman code.
  *
  * @A
  *	The output array for codewords.  In addition, initially this
  *	array must contain the symbols, sorted primarily by frequency and
  *	secondarily by symbol value, in the low NUM_SYMBOL_BITS bits of
  *	each entry.
@@ -937,300 +1174,265 @@
  *	Maximum length, in bits, of each codeword.
  *
  * @num_syms
  *	Number of symbols in the alphabet, including symbols with zero
  *	frequency.  This is the length of the 'A' and 'len' arrays.
  */
 static void
-gen_codewords(u32 A[restrict], u8 lens[restrict],
-	      const unsigned len_counts[restrict],
+gen_codewords(u32 A[], u8 lens[], const unsigned len_counts[],
 	      unsigned max_codeword_len, unsigned num_syms)
 {
 	u32 next_codewords[DEFLATE_MAX_CODEWORD_LEN + 1];
 	unsigned i;
 	unsigned len;
 	unsigned sym;
 
-	/* Given the number of codewords that will have each length,
-	 * assign codeword lengths to symbols.  We do this by assigning
-	 * the lengths in decreasing order to the symbols sorted
-	 * primarily by increasing frequency and secondarily by
-	 * increasing symbol value.  */
+	/*
+	 * Given the number of codewords that will have each length, assign
+	 * codeword lengths to symbols.  We do this by assigning the lengths in
+	 * decreasing order to the symbols sorted primarily by increasing
+	 * frequency and secondarily by increasing symbol value.
+	 */
 	for (i = 0, len = max_codeword_len; len >= 1; len--) {
 		unsigned count = len_counts[len];
+
 		while (count--)
 			lens[A[i++] & SYMBOL_MASK] = len;
 	}
 
-	/* Generate the codewords themselves.  We initialize the
+	/*
+	 * Generate the codewords themselves.  We initialize the
 	 * 'next_codewords' array to provide the lexicographically first
-	 * codeword of each length, then assign codewords in symbol
-	 * order.  This produces a canonical code.  */
+	 * codeword of each length, then assign codewords in symbol order.  This
+	 * produces a canonical code.
+	 */
 	next_codewords[0] = 0;
 	next_codewords[1] = 0;
 	for (len = 2; len <= max_codeword_len; len++)
 		next_codewords[len] =
 			(next_codewords[len - 1] + len_counts[len - 1]) << 1;
 
-	for (sym = 0; sym < num_syms; sym++)
-		A[sym] = next_codewords[lens[sym]]++;
+	for (sym = 0; sym < num_syms; sym++) {
+		/* DEFLATE requires bit-reversed codewords. */
+		A[sym] = reverse_codeword(next_codewords[lens[sym]]++,
+					  lens[sym]);
+	}
 }
 
 /*
  * ---------------------------------------------------------------------
- *			make_canonical_huffman_code()
+ *			deflate_make_huffman_code()
  * ---------------------------------------------------------------------
  *
  * Given an alphabet and the frequency of each symbol in it, construct a
  * length-limited canonical Huffman code.
  *
  * @num_syms
- *	The number of symbols in the alphabet.  The symbols are the
- *	integers in the range [0, num_syms - 1].  This parameter must be
- *	at least 2 and can't be greater than (1 << NUM_SYMBOL_BITS).
+ *	The number of symbols in the alphabet.  The symbols are the integers in
+ *	the range [0, num_syms - 1].  This parameter must be at least 2 and
+ *	must not exceed (1 << NUM_SYMBOL_BITS).
  *
  * @max_codeword_len
  *	The maximum permissible codeword length.
  *
  * @freqs
- *	An array of @num_syms entries, each of which specifies the
- *	frequency of the corresponding symbol.  It is valid for some,
- *	none, or all of the frequencies to be 0.
+ *	An array of length @num_syms that gives the frequency of each symbol.
+ *	It is valid for some, none, or all of the frequencies to be 0.  The sum
+ *	of frequencies must not exceed (1 << NUM_FREQ_BITS) - 1.
  *
  * @lens
- *	An array of @num_syms entries in which this function will return
- *	the length, in bits, of the codeword assigned to each symbol.
- *	Symbols with 0 frequency will not have codewords per se, but
- *	their entries in this array will be set to 0.  No lengths greater
- *	than @max_codeword_len will be assigned.
+ *	An array of @num_syms entries in which this function will return the
+ *	length, in bits, of the codeword assigned to each symbol.  Symbols with
+ *	0 frequency will not have codewords per se, but their entries in this
+ *	array will be set to 0.  No lengths greater than @max_codeword_len will
+ *	be assigned.
  *
  * @codewords
- *	An array of @num_syms entries in which this function will return
- *	the codeword for each symbol, right-justified and padded on the
- *	left with zeroes.  Codewords for symbols with 0 frequency will be
- *	undefined.
+ *	An array of @num_syms entries in which this function will return the
+ *	codeword for each symbol, right-justified and padded on the left with
+ *	zeroes.  Codewords for symbols with 0 frequency will be undefined.
  *
  * ---------------------------------------------------------------------
  *
  * This function builds a length-limited canonical Huffman code.
  *
  * A length-limited Huffman code contains no codewords longer than some
- * specified length, and has exactly (with some algorithms) or
- * approximately (with the algorithm used here) the minimum weighted path
- * length from the root, given this constraint.
- *
- * A canonical Huffman code satisfies the properties that a longer
- * codeword never lexicographically precedes a shorter codeword, and the
- * lexicographic ordering of codewords of the same length is the same as
- * the lexicographic ordering of the corresponding symbols.  A canonical
- * Huffman code, or more generally a canonical prefix code, can be
- * reconstructed from only a list containing the codeword length of each
- * symbol.
- *
- * The classic algorithm to generate a Huffman code creates a node for
- * each symbol, then inserts these nodes into a min-heap keyed by symbol
- * frequency.  Then, repeatedly, the two lowest-frequency nodes are
- * removed from the min-heap and added as the children of a new node
- * having frequency equal to the sum of its two children, which is then
- * inserted into the min-heap.  When only a single node remains in the
- * min-heap, it is the root of the Huffman tree.  The codeword for each
- * symbol is determined by the path needed to reach the corresponding
- * node from the root.  Descending to the left child appends a 0 bit,
- * whereas descending to the right child appends a 1 bit.
- *
- * The classic algorithm is relatively easy to understand, but it is
- * subject to a number of inefficiencies.  In practice, it is fastest to
- * first sort the symbols by frequency.  (This itself can be subject to
- * an optimization based on the fact that most frequencies tend to be
- * low.)  At the same time, we sort secondarily by symbol value, which
- * aids the process of generating a canonical code.  Then, during tree
- * construction, no heap is necessary because both the leaf nodes and the
- * unparented non-leaf nodes can be easily maintained in sorted order.
- * Consequently, there can never be more than two possibilities for the
- * next-lowest-frequency node.
- *
- * In addition, because we're generating a canonical code, we actually
- * don't need the leaf nodes of the tree at all, only the non-leaf nodes.
- * This is because for canonical code generation we don't need to know
- * where the symbols are in the tree.  Rather, we only need to know how
- * many leaf nodes have each depth (codeword length).  And this
- * information can, in fact, be quickly generated from the tree of
- * non-leaves only.
- *
- * Furthermore, we can build this stripped-down Huffman tree directly in
- * the array in which the codewords are to be generated, provided that
- * these array slots are large enough to hold a symbol and frequency
- * value.
- *
- * Still furthermore, we don't even need to maintain explicit child
- * pointers.  We only need the parent pointers, and even those can be
- * overwritten in-place with depth information as part of the process of
- * extracting codeword lengths from the tree.  So in summary, we do NOT
- * need a big structure like:
+ * specified length, and has exactly (with some algorithms) or approximately
+ * (with the algorithm used here) the minimum weighted path length from the
+ * root, given this constraint.
+ *
+ * A canonical Huffman code satisfies the properties that a longer codeword
+ * never lexicographically precedes a shorter codeword, and the lexicographic
+ * ordering of codewords of the same length is the same as the lexicographic
+ * ordering of the corresponding symbols.  A canonical Huffman code, or more
+ * generally a canonical prefix code, can be reconstructed from only a list
+ * containing the codeword length of each symbol.
+ *
+ * The classic algorithm to generate a Huffman code creates a node for each
+ * symbol, then inserts these nodes into a min-heap keyed by symbol frequency.
+ * Then, repeatedly, the two lowest-frequency nodes are removed from the
+ * min-heap and added as the children of a new node having frequency equal to
+ * the sum of its two children, which is then inserted into the min-heap.  When
+ * only a single node remains in the min-heap, it is the root of the Huffman
+ * tree.  The codeword for each symbol is determined by the path needed to reach
+ * the corresponding node from the root.  Descending to the left child appends a
+ * 0 bit, whereas descending to the right child appends a 1 bit.
+ *
+ * The classic algorithm is relatively easy to understand, but it is subject to
+ * a number of inefficiencies.  In practice, it is fastest to first sort the
+ * symbols by frequency.  (This itself can be subject to an optimization based
+ * on the fact that most frequencies tend to be low.)  At the same time, we sort
+ * secondarily by symbol value, which aids the process of generating a canonical
+ * code.  Then, during tree construction, no heap is necessary because both the
+ * leaf nodes and the unparented non-leaf nodes can be easily maintained in
+ * sorted order.  Consequently, there can never be more than two possibilities
+ * for the next-lowest-frequency node.
+ *
+ * In addition, because we're generating a canonical code, we actually don't
+ * need the leaf nodes of the tree at all, only the non-leaf nodes.  This is
+ * because for canonical code generation we don't need to know where the symbols
+ * are in the tree.  Rather, we only need to know how many leaf nodes have each
+ * depth (codeword length).  And this information can, in fact, be quickly
+ * generated from the tree of non-leaves only.
+ *
+ * Furthermore, we can build this stripped-down Huffman tree directly in the
+ * array in which the codewords are to be generated, provided that these array
+ * slots are large enough to hold a symbol and frequency value.
+ *
+ * Still furthermore, we don't even need to maintain explicit child pointers.
+ * We only need the parent pointers, and even those can be overwritten in-place
+ * with depth information as part of the process of extracting codeword lengths
+ * from the tree.  So in summary, we do NOT need a big structure like:
  *
  *	struct huffman_tree_node {
  *		unsigned int symbol;
  *		unsigned int frequency;
  *		unsigned int depth;
  *		struct huffman_tree_node *left_child;
  *		struct huffman_tree_node *right_child;
  *	};
  *
  *
- *   ... which often gets used in "naive" implementations of Huffman code
- *   generation.
+ * ... which often gets used in "naive" implementations of Huffman code
+ * generation.
  *
- * Many of these optimizations are based on the implementation in 7-Zip
- * (source file: C/HuffEnc.c), which has been placed in the public domain
- * by Igor Pavlov.
+ * Many of these optimizations are based on the implementation in 7-Zip (source
+ * file: C/HuffEnc.c), which was placed in the public domain by Igor Pavlov.
  */
 static void
-make_canonical_huffman_code(unsigned num_syms, unsigned max_codeword_len,
-			    const u32 freqs[restrict],
-			    u8 lens[restrict], u32 codewords[restrict])
+deflate_make_huffman_code(unsigned num_syms, unsigned max_codeword_len,
+			  const u32 freqs[], u8 lens[], u32 codewords[])
 {
 	u32 *A = codewords;
 	unsigned num_used_syms;
 
 	STATIC_ASSERT(DEFLATE_MAX_NUM_SYMS <= 1 << NUM_SYMBOL_BITS);
+	STATIC_ASSERT(MAX_BLOCK_LENGTH <= ((u32)1 << NUM_FREQ_BITS) - 1);
 
-	/* We begin by sorting the symbols primarily by frequency and
-	 * secondarily by symbol value.  As an optimization, the array
-	 * used for this purpose ('A') shares storage with the space in
-	 * which we will eventually return the codewords.  */
-
+	/*
+	 * We begin by sorting the symbols primarily by frequency and
+	 * secondarily by symbol value.  As an optimization, the array used for
+	 * this purpose ('A') shares storage with the space in which we will
+	 * eventually return the codewords.
+	 */
 	num_used_syms = sort_symbols(num_syms, freqs, lens, A);
 
-	/* 'num_used_syms' is the number of symbols with nonzero
-	 * frequency.  This may be less than @num_syms.  'num_used_syms'
-	 * is also the number of entries in 'A' that are valid.  Each
-	 * entry consists of a distinct symbol and a nonzero frequency
-	 * packed into a 32-bit integer.  */
+	/*
+	 * 'num_used_syms' is the number of symbols with nonzero frequency.
+	 * This may be less than @num_syms.  'num_used_syms' is also the number
+	 * of entries in 'A' that are valid.  Each entry consists of a distinct
+	 * symbol and a nonzero frequency packed into a 32-bit integer.
+	 */
 
-	/* Handle special cases where only 0 or 1 symbols were used (had
-	 * nonzero frequency).  */
+	/*
+	 * Handle special cases where only 0 or 1 symbols were used (had nonzero
+	 * frequency).
+	 */
 
 	if (unlikely(num_used_syms == 0)) {
-		/* Code is empty.  sort_symbols() already set all lengths
-		 * to 0, so there is nothing more to do.  */
+		/*
+		 * Code is empty.  sort_symbols() already set all lengths to 0,
+		 * so there is nothing more to do.
+		 */
 		return;
 	}
 
 	if (unlikely(num_used_syms == 1)) {
-		/* Only one symbol was used, so we only need one
-		 * codeword.  But two codewords are needed to form the
-		 * smallest complete Huffman code, which uses codewords 0
-		 * and 1.  Therefore, we choose another symbol to which
-		 * to assign a codeword.  We use 0 (if the used symbol is
-		 * not 0) or 1 (if the used symbol is 0).  In either
-		 * case, the lesser-valued symbol must be assigned
-		 * codeword 0 so that the resulting code is canonical.  */
+		/*
+		 * Only one symbol was used, so we only need one codeword.  But
+		 * two codewords are needed to form the smallest complete
+		 * Huffman code, which uses codewords 0 and 1.  Therefore, we
+		 * choose another symbol to which to assign a codeword.  We use
+		 * 0 (if the used symbol is not 0) or 1 (if the used symbol is
+		 * 0).  In either case, the lesser-valued symbol must be
+		 * assigned codeword 0 so that the resulting code is canonical.
+		 */
 
 		unsigned sym = A[0] & SYMBOL_MASK;
 		unsigned nonzero_idx = sym ? sym : 1;
 
 		codewords[0] = 0;
 		lens[0] = 1;
 		codewords[nonzero_idx] = 1;
 		lens[nonzero_idx] = 1;
 		return;
 	}
 
-	/* Build a stripped-down version of the Huffman tree, sharing the
-	 * array 'A' with the symbol values.  Then extract length counts
-	 * from the tree and use them to generate the final codewords.  */
+	/*
+	 * Build a stripped-down version of the Huffman tree, sharing the array
+	 * 'A' with the symbol values.  Then extract length counts from the tree
+	 * and use them to generate the final codewords.
+	 */
 
 	build_tree(A, num_used_syms);
 
 	{
 		unsigned len_counts[DEFLATE_MAX_CODEWORD_LEN + 1];
 
 		compute_length_counts(A, num_used_syms - 2,
 				      len_counts, max_codeword_len);
 
 		gen_codewords(A, lens, len_counts, max_codeword_len, num_syms);
 	}
 }
 
 /*
- * Clear the Huffman symbol frequency counters.
- * This must be called when starting a new DEFLATE block.
+ * Clear the Huffman symbol frequency counters.  This must be called when
+ * starting a new DEFLATE block.
  */
 static void
 deflate_reset_symbol_frequencies(struct libdeflate_compressor *c)
 {
 	memset(&c->freqs, 0, sizeof(c->freqs));
 }
 
-/* Reverse the Huffman codeword 'codeword', which is 'len' bits in length.  */
-static u32
-deflate_reverse_codeword(u32 codeword, u8 len)
-{
-	/* The following branchless algorithm is faster than going bit by bit.
-	 * Note: since no codewords are longer than 16 bits, we only need to
-	 * reverse the low 16 bits of the 'u32'.  */
-	STATIC_ASSERT(DEFLATE_MAX_CODEWORD_LEN <= 16);
-
-	/* Flip adjacent 1-bit fields  */
-	codeword = ((codeword & 0x5555) << 1) | ((codeword & 0xAAAA) >> 1);
-
-	/* Flip adjacent 2-bit fields  */
-	codeword = ((codeword & 0x3333) << 2) | ((codeword & 0xCCCC) >> 2);
-
-	/* Flip adjacent 4-bit fields  */
-	codeword = ((codeword & 0x0F0F) << 4) | ((codeword & 0xF0F0) >> 4);
-
-	/* Flip adjacent 8-bit fields  */
-	codeword = ((codeword & 0x00FF) << 8) | ((codeword & 0xFF00) >> 8);
-
-	/* Return the high 'len' bits of the bit-reversed 16 bit value.  */
-	return codeword >> (16 - len);
-}
-
-/* Make a canonical Huffman code with bit-reversed codewords.  */
-static void
-deflate_make_huffman_code(unsigned num_syms, unsigned max_codeword_len,
-			  const u32 freqs[], u8 lens[], u32 codewords[])
-{
-	unsigned sym;
-
-	make_canonical_huffman_code(num_syms, max_codeword_len,
-				    freqs, lens, codewords);
-
-	for (sym = 0; sym < num_syms; sym++)
-		codewords[sym] = deflate_reverse_codeword(codewords[sym], lens[sym]);
-}
-
 /*
  * Build the literal/length and offset Huffman codes for a DEFLATE block.
  *
- * This takes as input the frequency tables for each code and produces as output
- * a set of tables that map symbols to codewords and codeword lengths.
+ * This takes as input the frequency tables for each alphabet and produces as
+ * output a set of tables that map symbols to codewords and codeword lengths.
  */
 static void
 deflate_make_huffman_codes(const struct deflate_freqs *freqs,
 			   struct deflate_codes *codes)
 {
-	STATIC_ASSERT(MAX_LITLEN_CODEWORD_LEN <= DEFLATE_MAX_LITLEN_CODEWORD_LEN);
-	STATIC_ASSERT(MAX_OFFSET_CODEWORD_LEN <= DEFLATE_MAX_OFFSET_CODEWORD_LEN);
-
 	deflate_make_huffman_code(DEFLATE_NUM_LITLEN_SYMS,
 				  MAX_LITLEN_CODEWORD_LEN,
 				  freqs->litlen,
 				  codes->lens.litlen,
 				  codes->codewords.litlen);
 
 	deflate_make_huffman_code(DEFLATE_NUM_OFFSET_SYMS,
 				  MAX_OFFSET_CODEWORD_LEN,
 				  freqs->offset,
 				  codes->lens.offset,
 				  codes->codewords.offset);
 }
 
-/* Initialize c->static_codes.  */
+/* Initialize c->static_codes. */
 static void
 deflate_init_static_codes(struct libdeflate_compressor *c)
 {
 	unsigned i;
 
 	for (i = 0; i < 144; i++)
 		c->freqs.litlen[i] = 1 << (9 - 8);
@@ -1243,104 +1445,99 @@
 
 	for (i = 0; i < 32; i++)
 		c->freqs.offset[i] = 1 << (5 - 5);
 
 	deflate_make_huffman_codes(&c->freqs, &c->static_codes);
 }
 
-/* Return the offset slot for the specified match offset.  */
+/* Return the offset slot for the given match offset, using the small map. */
 static forceinline unsigned
-deflate_get_offset_slot(struct libdeflate_compressor *c, unsigned offset)
+deflate_get_offset_slot(unsigned offset)
 {
-#if USE_FULL_OFFSET_SLOT_FAST
-	return c->offset_slot_fast[offset];
-#else
+#if 1
 	if (offset <= 256)
-		return c->offset_slot_fast[offset - 1];
+		return deflate_offset_slot[offset];
 	else
-		return c->offset_slot_fast[256 + ((offset - 1) >> 7)];
-#endif
-}
+		return deflate_offset_slot[256 + ((offset - 1) >> 7)];
+#else /* Branchless version */
+	u32 i1 = offset;
+	u32 i2 = 256 + ((offset - 1) >> 7);
+	u32 is_small = (s32)(offset - 257) >> 31;
 
-/* Write the header fields common to all DEFLATE block types.  */
-static void
-deflate_write_block_header(struct deflate_output_bitstream *os,
-			   bool is_final_block, unsigned block_type)
-{
-	deflate_add_bits(os, is_final_block, 1);
-	deflate_add_bits(os, block_type, 2);
-	deflate_flush_bits(os);
+	return deflate_offset_slot[(i1 & is_small) ^ (i2 & ~is_small)];
+#endif
 }
 
 static unsigned
-deflate_compute_precode_items(const u8 lens[restrict],
-			      const unsigned num_lens,
-			      u32 precode_freqs[restrict],
-			      unsigned precode_items[restrict])
+deflate_compute_precode_items(const u8 lens[], const unsigned num_lens,
+			      u32 precode_freqs[], unsigned precode_items[])
 {
 	unsigned *itemptr;
 	unsigned run_start;
 	unsigned run_end;
 	unsigned extra_bits;
 	u8 len;
 
 	memset(precode_freqs, 0,
 	       DEFLATE_NUM_PRECODE_SYMS * sizeof(precode_freqs[0]));
 
 	itemptr = precode_items;
 	run_start = 0;
 	do {
-		/* Find the next run of codeword lengths.  */
+		/* Find the next run of codeword lengths. */
 
-		/* len = the length being repeated  */
+		/* len = the length being repeated */
 		len = lens[run_start];
 
-		/* Extend the run.  */
+		/* Extend the run. */
 		run_end = run_start;
 		do {
 			run_end++;
 		} while (run_end != num_lens && len == lens[run_end]);
 
 		if (len == 0) {
-			/* Run of zeroes.  */
+			/* Run of zeroes. */
 
-			/* Symbol 18: RLE 11 to 138 zeroes at a time.  */
+			/* Symbol 18: RLE 11 to 138 zeroes at a time. */
 			while ((run_end - run_start) >= 11) {
-				extra_bits = MIN((run_end - run_start) - 11, 0x7F);
+				extra_bits = MIN((run_end - run_start) - 11,
+						 0x7F);
 				precode_freqs[18]++;
 				*itemptr++ = 18 | (extra_bits << 5);
 				run_start += 11 + extra_bits;
 			}
 
-			/* Symbol 17: RLE 3 to 10 zeroes at a time.  */
+			/* Symbol 17: RLE 3 to 10 zeroes at a time. */
 			if ((run_end - run_start) >= 3) {
-				extra_bits = MIN((run_end - run_start) - 3, 0x7);
+				extra_bits = MIN((run_end - run_start) - 3,
+						 0x7);
 				precode_freqs[17]++;
 				*itemptr++ = 17 | (extra_bits << 5);
 				run_start += 3 + extra_bits;
 			}
 		} else {
 
 			/* A run of nonzero lengths. */
 
-			/* Symbol 16: RLE 3 to 6 of the previous length.  */
+			/* Symbol 16: RLE 3 to 6 of the previous length. */
 			if ((run_end - run_start) >= 4) {
 				precode_freqs[len]++;
 				*itemptr++ = len;
 				run_start++;
 				do {
-					extra_bits = MIN((run_end - run_start) - 3, 0x3);
+					extra_bits = MIN((run_end - run_start) -
+							 3, 0x3);
 					precode_freqs[16]++;
 					*itemptr++ = 16 | (extra_bits << 5);
 					run_start += 3 + extra_bits;
 				} while ((run_end - run_start) >= 3);
 			}
 		}
 
-		/* Output any remaining lengths without RLE.  */
+		/* Output any remaining lengths without RLE. */
 		while (run_start != run_end) {
 			precode_freqs[len]++;
 			*itemptr++ = len;
 			run_start++;
 		}
 	} while (run_start != num_lens);
 
@@ -1353,495 +1550,478 @@
  * possible codeword length in the larger code as well as several special
  * symbols to represent repeated codeword lengths (a form of run-length
  * encoding).  The precode is itself constructed in canonical form, and its
  * codeword lengths are represented literally in 19 3-bit fields that
  * immediately precede the compressed codeword lengths of the larger code.
  */
 
-/* Precompute the information needed to output Huffman codes. */
+/* Precompute the information needed to output dynamic Huffman codes. */
 static void
 deflate_precompute_huffman_header(struct libdeflate_compressor *c)
 {
 	/* Compute how many litlen and offset symbols are needed. */
 
-	for (c->num_litlen_syms = DEFLATE_NUM_LITLEN_SYMS;
-	     c->num_litlen_syms > 257;
-	     c->num_litlen_syms--)
-		if (c->codes.lens.litlen[c->num_litlen_syms - 1] != 0)
+	for (c->o.precode.num_litlen_syms = DEFLATE_NUM_LITLEN_SYMS;
+	     c->o.precode.num_litlen_syms > 257;
+	     c->o.precode.num_litlen_syms--)
+		if (c->codes.lens.litlen[c->o.precode.num_litlen_syms - 1] != 0)
 			break;
 
-	for (c->num_offset_syms = DEFLATE_NUM_OFFSET_SYMS;
-	     c->num_offset_syms > 1;
-	     c->num_offset_syms--)
-		if (c->codes.lens.offset[c->num_offset_syms - 1] != 0)
+	for (c->o.precode.num_offset_syms = DEFLATE_NUM_OFFSET_SYMS;
+	     c->o.precode.num_offset_syms > 1;
+	     c->o.precode.num_offset_syms--)
+		if (c->codes.lens.offset[c->o.precode.num_offset_syms - 1] != 0)
 			break;
 
-	/* If we're not using the full set of literal/length codeword lengths,
+	/*
+	 * If we're not using the full set of literal/length codeword lengths,
 	 * then temporarily move the offset codeword lengths over so that the
-	 * literal/length and offset codeword lengths are contiguous. */
-
+	 * literal/length and offset codeword lengths are contiguous.
+	 */
 	STATIC_ASSERT(offsetof(struct deflate_lens, offset) ==
 		      DEFLATE_NUM_LITLEN_SYMS);
-
-	if (c->num_litlen_syms != DEFLATE_NUM_LITLEN_SYMS) {
-		memmove((u8 *)&c->codes.lens + c->num_litlen_syms,
+	if (c->o.precode.num_litlen_syms != DEFLATE_NUM_LITLEN_SYMS) {
+		memmove((u8 *)&c->codes.lens + c->o.precode.num_litlen_syms,
 			(u8 *)&c->codes.lens + DEFLATE_NUM_LITLEN_SYMS,
-			c->num_offset_syms);
+			c->o.precode.num_offset_syms);
 	}
 
-	/* Compute the "items" (RLE / literal tokens and extra bits) with which
-	 * the codeword lengths in the larger code will be output. */
-	c->num_precode_items =
+	/*
+	 * Compute the "items" (RLE / literal tokens and extra bits) with which
+	 * the codeword lengths in the larger code will be output.
+	 */
+	c->o.precode.num_items =
 		deflate_compute_precode_items((u8 *)&c->codes.lens,
-					      c->num_litlen_syms +
-							c->num_offset_syms,
-					      c->precode_freqs,
-					      c->precode_items);
+					      c->o.precode.num_litlen_syms +
+					      c->o.precode.num_offset_syms,
+					      c->o.precode.freqs,
+					      c->o.precode.items);
 
 	/* Build the precode. */
-	STATIC_ASSERT(MAX_PRE_CODEWORD_LEN <= DEFLATE_MAX_PRE_CODEWORD_LEN);
 	deflate_make_huffman_code(DEFLATE_NUM_PRECODE_SYMS,
 				  MAX_PRE_CODEWORD_LEN,
-				  c->precode_freqs, c->precode_lens,
-				  c->precode_codewords);
+				  c->o.precode.freqs, c->o.precode.lens,
+				  c->o.precode.codewords);
 
 	/* Count how many precode lengths we actually need to output. */
-	for (c->num_explicit_lens = DEFLATE_NUM_PRECODE_SYMS;
-	     c->num_explicit_lens > 4;
-	     c->num_explicit_lens--)
-		if (c->precode_lens[deflate_precode_lens_permutation[
-						c->num_explicit_lens - 1]] != 0)
+	for (c->o.precode.num_explicit_lens = DEFLATE_NUM_PRECODE_SYMS;
+	     c->o.precode.num_explicit_lens > 4;
+	     c->o.precode.num_explicit_lens--)
+		if (c->o.precode.lens[deflate_precode_lens_permutation[
+				c->o.precode.num_explicit_lens - 1]] != 0)
 			break;
 
 	/* Restore the offset codeword lengths if needed. */
-	if (c->num_litlen_syms != DEFLATE_NUM_LITLEN_SYMS) {
+	if (c->o.precode.num_litlen_syms != DEFLATE_NUM_LITLEN_SYMS) {
 		memmove((u8 *)&c->codes.lens + DEFLATE_NUM_LITLEN_SYMS,
-			(u8 *)&c->codes.lens + c->num_litlen_syms,
-			c->num_offset_syms);
-	}
-}
-
-/* Output the Huffman codes. */
-static void
-deflate_write_huffman_header(struct libdeflate_compressor *c,
-			     struct deflate_output_bitstream *os)
-{
-	unsigned i;
-
-	deflate_add_bits(os, c->num_litlen_syms - 257, 5);
-	deflate_add_bits(os, c->num_offset_syms - 1, 5);
-	deflate_add_bits(os, c->num_explicit_lens - 4, 4);
-	deflate_flush_bits(os);
-
-	/* Output the lengths of the codewords in the precode.  */
-	for (i = 0; i < c->num_explicit_lens; i++) {
-		deflate_add_bits(os, c->precode_lens[
-				       deflate_precode_lens_permutation[i]], 3);
-		deflate_flush_bits(os);
-	}
-
-	/* Output the encoded lengths of the codewords in the larger code.  */
-	for (i = 0; i < c->num_precode_items; i++) {
-		unsigned precode_item = c->precode_items[i];
-		unsigned precode_sym = precode_item & 0x1F;
-		deflate_add_bits(os, c->precode_codewords[precode_sym],
-				 c->precode_lens[precode_sym]);
-		if (precode_sym >= 16) {
-			if (precode_sym == 16)
-				deflate_add_bits(os, precode_item >> 5, 2);
-			else if (precode_sym == 17)
-				deflate_add_bits(os, precode_item >> 5, 3);
-			else
-				deflate_add_bits(os, precode_item >> 5, 7);
-		}
-		STATIC_ASSERT(CAN_BUFFER(DEFLATE_MAX_PRE_CODEWORD_LEN + 7));
-		deflate_flush_bits(os);
+			(u8 *)&c->codes.lens + c->o.precode.num_litlen_syms,
+			c->o.precode.num_offset_syms);
 	}
 }
 
-static void
-deflate_write_sequences(struct deflate_output_bitstream * restrict os,
-			const struct deflate_codes * restrict codes,
-			const struct deflate_sequence sequences[restrict],
-			const u8 * restrict in_next)
-{
-	const struct deflate_sequence *seq = sequences;
-
-	for (;;) {
-		u32 litrunlen = seq->litrunlen_and_length & 0x7FFFFF;
-		unsigned length = seq->litrunlen_and_length >> 23;
-		unsigned length_slot;
-		unsigned litlen_symbol;
-		unsigned offset_symbol;
-
-		if (litrunlen) {
-		#if 1
-			while (litrunlen >= 4) {
-				unsigned lit0 = in_next[0];
-				unsigned lit1 = in_next[1];
-				unsigned lit2 = in_next[2];
-				unsigned lit3 = in_next[3];
-
-				deflate_add_bits(os, codes->codewords.litlen[lit0],
-						 codes->lens.litlen[lit0]);
-				if (!CAN_BUFFER(2 * MAX_LITLEN_CODEWORD_LEN))
-					deflate_flush_bits(os);
-
-				deflate_add_bits(os, codes->codewords.litlen[lit1],
-						 codes->lens.litlen[lit1]);
-				if (!CAN_BUFFER(4 * MAX_LITLEN_CODEWORD_LEN))
-					deflate_flush_bits(os);
-
-				deflate_add_bits(os, codes->codewords.litlen[lit2],
-						 codes->lens.litlen[lit2]);
-				if (!CAN_BUFFER(2 * MAX_LITLEN_CODEWORD_LEN))
-					deflate_flush_bits(os);
-
-				deflate_add_bits(os, codes->codewords.litlen[lit3],
-						 codes->lens.litlen[lit3]);
-				deflate_flush_bits(os);
-				in_next += 4;
-				litrunlen -= 4;
-			}
-			if (litrunlen-- != 0) {
-				deflate_add_bits(os, codes->codewords.litlen[*in_next],
-						 codes->lens.litlen[*in_next]);
-				if (!CAN_BUFFER(3 * MAX_LITLEN_CODEWORD_LEN))
-					deflate_flush_bits(os);
-				in_next++;
-				if (litrunlen-- != 0) {
-					deflate_add_bits(os, codes->codewords.litlen[*in_next],
-							 codes->lens.litlen[*in_next]);
-					if (!CAN_BUFFER(3 * MAX_LITLEN_CODEWORD_LEN))
-						deflate_flush_bits(os);
-					in_next++;
-					if (litrunlen-- != 0) {
-						deflate_add_bits(os, codes->codewords.litlen[*in_next],
-								 codes->lens.litlen[*in_next]);
-						if (!CAN_BUFFER(3 * MAX_LITLEN_CODEWORD_LEN))
-							deflate_flush_bits(os);
-						in_next++;
-					}
-				}
-				if (CAN_BUFFER(3 * MAX_LITLEN_CODEWORD_LEN))
-					deflate_flush_bits(os);
-			}
-		#else
-			do {
-				unsigned lit = *in_next++;
-				deflate_add_bits(os, codes->codewords.litlen[lit],
-						 codes->lens.litlen[lit]);
-				deflate_flush_bits(os);
-			} while (--litrunlen);
-		#endif
-		}
-
-		if (length == 0)
-			return;
-
-		in_next += length;
-
-		length_slot = seq->length_slot;
-		litlen_symbol = 257 + length_slot;
-
-		/* Litlen symbol  */
-		deflate_add_bits(os, codes->codewords.litlen[litlen_symbol],
-				 codes->lens.litlen[litlen_symbol]);
-
-		/* Extra length bits  */
-		STATIC_ASSERT(CAN_BUFFER(MAX_LITLEN_CODEWORD_LEN +
-					 DEFLATE_MAX_EXTRA_LENGTH_BITS));
-		deflate_add_bits(os, length - deflate_length_slot_base[length_slot],
-				 deflate_extra_length_bits[length_slot]);
-
-		if (!CAN_BUFFER(MAX_LITLEN_CODEWORD_LEN +
-				DEFLATE_MAX_EXTRA_LENGTH_BITS +
-				MAX_OFFSET_CODEWORD_LEN +
-				DEFLATE_MAX_EXTRA_OFFSET_BITS))
-			deflate_flush_bits(os);
-
-		/* Offset symbol  */
-		offset_symbol = seq->offset_symbol;
-		deflate_add_bits(os, codes->codewords.offset[offset_symbol],
-				 codes->lens.offset[offset_symbol]);
-
-		if (!CAN_BUFFER(MAX_OFFSET_CODEWORD_LEN +
-				DEFLATE_MAX_EXTRA_OFFSET_BITS))
-			deflate_flush_bits(os);
-
-		/* Extra offset bits  */
-		deflate_add_bits(os, seq->offset - deflate_offset_slot_base[offset_symbol],
-				 deflate_extra_offset_bits[offset_symbol]);
-
-		deflate_flush_bits(os);
-
-		seq++;
-	}
-}
-
-#if SUPPORT_NEAR_OPTIMAL_PARSING
 /*
- * Follow the minimum-cost path in the graph of possible match/literal choices
- * for the current block and write out the matches/literals using the specified
- * Huffman codes.
- *
- * Note: this is slightly duplicated with deflate_write_sequences(), the reason
- * being that we don't want to waste time translating between intermediate
- * match/literal representations.
+ * To make it faster to output matches, compute the "full" match length
+ * codewords, i.e. the concatenation of the litlen codeword and the extra bits
+ * for each possible match length.
  */
 static void
-deflate_write_item_list(struct deflate_output_bitstream *os,
-			const struct deflate_codes *codes,
-			struct libdeflate_compressor *c,
-			u32 block_length)
-{
-	struct deflate_optimum_node *cur_node = &c->p.n.optimum_nodes[0];
-	struct deflate_optimum_node * const end_node = &c->p.n.optimum_nodes[block_length];
-	do {
-		unsigned length = cur_node->item & OPTIMUM_LEN_MASK;
-		unsigned offset = cur_node->item >> OPTIMUM_OFFSET_SHIFT;
-		unsigned litlen_symbol;
-		unsigned length_slot;
-		unsigned offset_slot;
-
-		if (length == 1) {
-			/* Literal  */
-			litlen_symbol = offset;
-			deflate_add_bits(os, codes->codewords.litlen[litlen_symbol],
-					 codes->lens.litlen[litlen_symbol]);
-			deflate_flush_bits(os);
-		} else {
-			/* Match length  */
-			length_slot = deflate_length_slot[length];
-			litlen_symbol = 257 + length_slot;
-			deflate_add_bits(os, codes->codewords.litlen[litlen_symbol],
-					 codes->lens.litlen[litlen_symbol]);
-
-			deflate_add_bits(os, length - deflate_length_slot_base[length_slot],
-					 deflate_extra_length_bits[length_slot]);
-
-			if (!CAN_BUFFER(MAX_LITLEN_CODEWORD_LEN +
-					DEFLATE_MAX_EXTRA_LENGTH_BITS +
-					MAX_OFFSET_CODEWORD_LEN +
-					DEFLATE_MAX_EXTRA_OFFSET_BITS))
-				deflate_flush_bits(os);
-
-
-			/* Match offset  */
-			offset_slot = deflate_get_offset_slot(c, offset);
-			deflate_add_bits(os, codes->codewords.offset[offset_slot],
-					 codes->lens.offset[offset_slot]);
-
-			if (!CAN_BUFFER(MAX_OFFSET_CODEWORD_LEN +
-					DEFLATE_MAX_EXTRA_OFFSET_BITS))
-				deflate_flush_bits(os);
-
-			deflate_add_bits(os, offset - deflate_offset_slot_base[offset_slot],
-					 deflate_extra_offset_bits[offset_slot]);
-
-			deflate_flush_bits(os);
-		}
-		cur_node += length;
-	} while (cur_node != end_node);
-}
-#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
-
-/* Output the end-of-block symbol.  */
-static void
-deflate_write_end_of_block(struct deflate_output_bitstream *os,
-			   const struct deflate_codes *codes)
+deflate_compute_full_len_codewords(struct libdeflate_compressor *c,
+				   const struct deflate_codes *codes)
 {
-	deflate_add_bits(os, codes->codewords.litlen[DEFLATE_END_OF_BLOCK],
-			 codes->lens.litlen[DEFLATE_END_OF_BLOCK]);
-	deflate_flush_bits(os);
-}
+	unsigned len;
 
-static void
-deflate_write_uncompressed_block(struct deflate_output_bitstream *os,
-				 const u8 *data, u16 len,
-				 bool is_final_block)
-{
-	deflate_write_block_header(os, is_final_block,
-				   DEFLATE_BLOCKTYPE_UNCOMPRESSED);
-	deflate_align_bitstream(os);
+	STATIC_ASSERT(MAX_LITLEN_CODEWORD_LEN +
+		      DEFLATE_MAX_EXTRA_LENGTH_BITS <= 32);
 
-	if (4 + (u32)len >= os->end - os->next) {
-		os->next = os->end;
-		return;
+	for (len = DEFLATE_MIN_MATCH_LEN; len <= DEFLATE_MAX_MATCH_LEN; len++) {
+		unsigned slot = deflate_length_slot[len];
+		unsigned litlen_sym = DEFLATE_FIRST_LEN_SYM + slot;
+		u32 extra_bits = len - deflate_length_slot_base[slot];
+
+		c->o.length.codewords[len] =
+			codes->codewords.litlen[litlen_sym] |
+			(extra_bits << codes->lens.litlen[litlen_sym]);
+		c->o.length.lens[len] = codes->lens.litlen[litlen_sym] +
+					deflate_extra_length_bits[slot];
 	}
-
-	put_unaligned_le16(len, os->next);
-	os->next += 2;
-	put_unaligned_le16(~len, os->next);
-	os->next += 2;
-	memcpy(os->next, data, len);
-	os->next += len;
 }
 
-static void
-deflate_write_uncompressed_blocks(struct deflate_output_bitstream *os,
-				  const u8 *data, size_t data_length,
-				  bool is_final_block)
-{
-	do {
-		u16 len = MIN(data_length, UINT16_MAX);
-
-		deflate_write_uncompressed_block(os, data, len,
-					is_final_block && len == data_length);
-		data += len;
-		data_length -= len;
-	} while (data_length != 0);
-}
+/* Write a match to the output buffer. */
+#define WRITE_MATCH(c_, codes_, length_, offset_, offset_slot_)		\
+do {									\
+	const struct libdeflate_compressor *c__ = (c_);			\
+	const struct deflate_codes *codes__ = (codes_);			\
+	unsigned length__ = (length_);					\
+	unsigned offset__ = (offset_);					\
+	unsigned offset_slot__ = (offset_slot_);			\
+									\
+	/* Litlen symbol and extra length bits */			\
+	STATIC_ASSERT(CAN_BUFFER(MAX_LITLEN_CODEWORD_LEN +		\
+				 DEFLATE_MAX_EXTRA_LENGTH_BITS));	\
+	ADD_BITS(c__->o.length.codewords[length__],			\
+		 c__->o.length.lens[length__]);				\
+									\
+	if (!CAN_BUFFER(MAX_LITLEN_CODEWORD_LEN +			\
+			DEFLATE_MAX_EXTRA_LENGTH_BITS +			\
+			MAX_OFFSET_CODEWORD_LEN +			\
+			DEFLATE_MAX_EXTRA_OFFSET_BITS))			\
+		FLUSH_BITS();						\
+									\
+	/* Offset symbol */						\
+	ADD_BITS(codes__->codewords.offset[offset_slot__],		\
+		 codes__->lens.offset[offset_slot__]);			\
+									\
+	if (!CAN_BUFFER(MAX_OFFSET_CODEWORD_LEN +			\
+			DEFLATE_MAX_EXTRA_OFFSET_BITS))			\
+		FLUSH_BITS();						\
+									\
+	/* Extra offset bits */						\
+	ADD_BITS(offset__ - deflate_offset_slot_base[offset_slot__],	\
+		 deflate_extra_offset_bits[offset_slot__]);		\
+									\
+	FLUSH_BITS();							\
+} while (0)
 
 /*
  * Choose the best type of block to use (dynamic Huffman, static Huffman, or
  * uncompressed), then output it.
+ *
+ * The uncompressed data of the block is @block_begin[0..@block_length-1].  The
+ * sequence of literals and matches that will be used to compress the block (if
+ * a compressed block is chosen) is given by @sequences if it's non-NULL, or
+ * else @c->p.n.optimum_nodes.  @c->freqs and @c->codes must be already set
+ * according to the literals, matches, and end-of-block symbol.
  */
 static void
-deflate_flush_block(struct libdeflate_compressor * restrict c,
-		    struct deflate_output_bitstream * restrict os,
-		    const u8 * restrict block_begin, u32 block_length,
-		    bool is_final_block, bool use_item_list)
+deflate_flush_block(struct libdeflate_compressor *c,
+		    struct deflate_output_bitstream *os,
+		    const u8 *block_begin, u32 block_length,
+		    const struct deflate_sequence *sequences,
+		    bool is_final_block)
 {
-	static const u8 deflate_extra_precode_bits[DEFLATE_NUM_PRECODE_SYMS] = {
-		0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 3, 7,
-	};
-
-	/* Costs are measured in bits */
+	/*
+	 * It is hard to get compilers to understand that writes to 'os->next'
+	 * don't alias 'os'.  That hurts performance significantly, as
+	 * everything in 'os' would keep getting re-loaded.  ('restrict'
+	 * *should* do the trick, but it's unreliable.)  Therefore, we keep all
+	 * the output bitstream state in local variables, and output bits using
+	 * macros.  This is similar to what the decompressor does.
+	 */
+	const u8 *in_next = block_begin;
+	const u8 * const in_end = block_begin + block_length;
+	bitbuf_t bitbuf = os->bitbuf;
+	unsigned bitcount = os->bitcount;
+	u8 *out_next = os->next;
+	u8 * const out_end = os->end;
+	/* The cost for each block type, in bits */
 	u32 dynamic_cost = 0;
 	u32 static_cost = 0;
 	u32 uncompressed_cost = 0;
+	u32 best_cost;
 	struct deflate_codes *codes;
-	int block_type;
 	unsigned sym;
 
-	/* Tally the end-of-block symbol. */
-	c->freqs.litlen[DEFLATE_END_OF_BLOCK]++;
+	ASSERT(block_length >= MIN_BLOCK_LENGTH || is_final_block);
+	ASSERT(block_length <= MAX_BLOCK_LENGTH);
+	ASSERT(bitcount <= 7);
+	ASSERT((bitbuf & ~(((bitbuf_t)1 << bitcount) - 1)) == 0);
+	ASSERT(out_next <= out_end);
 
-	/* Build dynamic Huffman codes. */
-	deflate_make_huffman_codes(&c->freqs, &c->codes);
-
-	/* Account for the cost of sending dynamic Huffman codes. */
+	/* Precompute the precode items and build the precode. */
 	deflate_precompute_huffman_header(c);
-	dynamic_cost += 5 + 5 + 4 + (3 * c->num_explicit_lens);
+
+	/* Account for the cost of encoding dynamic Huffman codes. */
+	dynamic_cost += 5 + 5 + 4 + (3 * c->o.precode.num_explicit_lens);
 	for (sym = 0; sym < DEFLATE_NUM_PRECODE_SYMS; sym++) {
 		u32 extra = deflate_extra_precode_bits[sym];
-		dynamic_cost += c->precode_freqs[sym] *
-				(extra + c->precode_lens[sym]);
+
+		dynamic_cost += c->o.precode.freqs[sym] *
+				(extra + c->o.precode.lens[sym]);
 	}
 
 	/* Account for the cost of encoding literals. */
-	for (sym = 0; sym < 256; sym++) {
+	for (sym = 0; sym < 144; sym++) {
 		dynamic_cost += c->freqs.litlen[sym] *
 				c->codes.lens.litlen[sym];
-	}
-	for (sym = 0; sym < 144; sym++)
 		static_cost += c->freqs.litlen[sym] * 8;
-	for (; sym < 256; sym++)
+	}
+	for (; sym < 256; sym++) {
+		dynamic_cost += c->freqs.litlen[sym] *
+				c->codes.lens.litlen[sym];
 		static_cost += c->freqs.litlen[sym] * 9;
+	}
 
 	/* Account for the cost of encoding the end-of-block symbol. */
-	dynamic_cost += c->codes.lens.litlen[256];
+	dynamic_cost += c->codes.lens.litlen[DEFLATE_END_OF_BLOCK];
 	static_cost += 7;
 
 	/* Account for the cost of encoding lengths. */
-	for (sym = 257; sym < 257 + ARRAY_LEN(deflate_extra_length_bits); sym++) {
-		u32 extra = deflate_extra_length_bits[sym - 257];
+	for (sym = DEFLATE_FIRST_LEN_SYM;
+	     sym < DEFLATE_FIRST_LEN_SYM + ARRAY_LEN(deflate_extra_length_bits);
+	     sym++) {
+		u32 extra = deflate_extra_length_bits[
+					sym - DEFLATE_FIRST_LEN_SYM];
+
 		dynamic_cost += c->freqs.litlen[sym] *
 				(extra + c->codes.lens.litlen[sym]);
 		static_cost += c->freqs.litlen[sym] *
 				(extra + c->static_codes.lens.litlen[sym]);
 	}
 
 	/* Account for the cost of encoding offsets. */
 	for (sym = 0; sym < ARRAY_LEN(deflate_extra_offset_bits); sym++) {
 		u32 extra = deflate_extra_offset_bits[sym];
+
 		dynamic_cost += c->freqs.offset[sym] *
 				(extra + c->codes.lens.offset[sym]);
 		static_cost += c->freqs.offset[sym] * (extra + 5);
 	}
 
 	/* Compute the cost of using uncompressed blocks. */
-	uncompressed_cost += (-(os->bitcount + 3) & 7) + 32 +
+	uncompressed_cost += (-(bitcount + 3) & 7) + 32 +
 			     (40 * (DIV_ROUND_UP(block_length,
 						 UINT16_MAX) - 1)) +
 			     (8 * block_length);
 
-	/* Choose the cheapest block type. */
-	if (dynamic_cost < MIN(static_cost, uncompressed_cost)) {
-		block_type = DEFLATE_BLOCKTYPE_DYNAMIC_HUFFMAN;
+	/* Choose and output the cheapest type of block. */
+	best_cost = MIN(static_cost, uncompressed_cost);
+	if (dynamic_cost < best_cost) {
+		const unsigned num_explicit_lens = c->o.precode.num_explicit_lens;
+		const unsigned num_precode_items = c->o.precode.num_items;
+		unsigned precode_sym, precode_item;
+		unsigned i;
+
+		/* Dynamic Huffman block */
+
+		best_cost = dynamic_cost;
 		codes = &c->codes;
+		STATIC_ASSERT(CAN_BUFFER(1 + 2 + 5 + 5 + 4 + 3));
+		ADD_BITS(is_final_block, 1);
+		ADD_BITS(DEFLATE_BLOCKTYPE_DYNAMIC_HUFFMAN, 2);
+		ADD_BITS(c->o.precode.num_litlen_syms - 257, 5);
+		ADD_BITS(c->o.precode.num_offset_syms - 1, 5);
+		ADD_BITS(num_explicit_lens - 4, 4);
+
+		/* Output the lengths of the codewords in the precode. */
+		if (CAN_BUFFER(3 * (DEFLATE_NUM_PRECODE_SYMS - 1))) {
+			/*
+			 * A 64-bit bitbuffer is just one bit too small to hold
+			 * the maximum number of precode lens, so to minimize
+			 * flushes we merge one len with the previous fields.
+			 */
+			precode_sym = deflate_precode_lens_permutation[0];
+			ADD_BITS(c->o.precode.lens[precode_sym], 3);
+			FLUSH_BITS();
+			i = 1; /* num_explicit_lens >= 4 */
+			do {
+				precode_sym =
+					deflate_precode_lens_permutation[i];
+				ADD_BITS(c->o.precode.lens[precode_sym], 3);
+			} while (++i < num_explicit_lens);
+			FLUSH_BITS();
+		} else {
+			FLUSH_BITS();
+			i = 0;
+			do {
+				precode_sym =
+					deflate_precode_lens_permutation[i];
+				ADD_BITS(c->o.precode.lens[precode_sym], 3);
+				FLUSH_BITS();
+			} while (++i < num_explicit_lens);
+		}
+
+		/*
+		 * Output the lengths of the codewords in the litlen and offset
+		 * codes, encoded by the precode.
+		 */
+		i = 0;
+		do {
+			precode_item = c->o.precode.items[i];
+			precode_sym = precode_item & 0x1F;
+			STATIC_ASSERT(CAN_BUFFER(MAX_PRE_CODEWORD_LEN + 7));
+			ADD_BITS(c->o.precode.codewords[precode_sym],
+				 c->o.precode.lens[precode_sym]);
+			ADD_BITS(precode_item >> 5,
+				 deflate_extra_precode_bits[precode_sym]);
+			FLUSH_BITS();
+		} while (++i < num_precode_items);
 	} else if (static_cost < uncompressed_cost) {
-		block_type = DEFLATE_BLOCKTYPE_STATIC_HUFFMAN;
+		/* Static Huffman block */
 		codes = &c->static_codes;
+		ADD_BITS(is_final_block, 1);
+		ADD_BITS(DEFLATE_BLOCKTYPE_STATIC_HUFFMAN, 2);
+		FLUSH_BITS();
 	} else {
-		block_type = DEFLATE_BLOCKTYPE_UNCOMPRESSED;
-	}
+		/*
+		 * Uncompressed block(s).  DEFLATE limits the length of
+		 * uncompressed blocks to UINT16_MAX bytes, so if the length of
+		 * the "block" we're flushing is over UINT16_MAX, we actually
+		 * output multiple blocks.
+		 */
+		do {
+			u8 bfinal = 0;
+			size_t len = UINT16_MAX;
 
-	/* Now actually output the block. */
+			if (in_end - in_next <= UINT16_MAX) {
+				bfinal = is_final_block;
+				len = in_end - in_next;
+			}
+			if (out_end - out_next <
+			    (bitcount + 3 + 7) / 8 + 4 + len) {
+				/* Not enough output space remaining. */
+				out_next = out_end;
+				goto out;
+			}
+			/*
+			 * Output BFINAL (1 bit) and BTYPE (2 bits), then align
+			 * to a byte boundary.
+			 */
+			STATIC_ASSERT(DEFLATE_BLOCKTYPE_UNCOMPRESSED == 0);
+			*out_next++ = (bfinal << bitcount) | bitbuf;
+			if (bitcount > 5)
+				*out_next++ = 0;
+			bitbuf = 0;
+			bitcount = 0;
+			/* Output LEN and NLEN, then the data itself. */
+			put_unaligned_le16(len, out_next);
+			out_next += 2;
+			put_unaligned_le16(~len, out_next);
+			out_next += 2;
+			memcpy(out_next, in_next, len);
+			out_next += len;
+			in_next += len;
+		} while (in_next != in_end);
+		/* Done outputting uncompressed block(s) */
+		goto out;
+	}
+
+	/* Output the literals and matches for a dynamic or static block. */
+	ASSERT(bitcount <= 7);
+	deflate_compute_full_len_codewords(c, codes);
+#if SUPPORT_NEAR_OPTIMAL_PARSING
+	if (sequences == NULL) {
+		/* Output the literals and matches from the minimum-cost path */
+		struct deflate_optimum_node *cur_node =
+			&c->p.n.optimum_nodes[0];
+		struct deflate_optimum_node * const end_node =
+			&c->p.n.optimum_nodes[block_length];
+		do {
+			unsigned length = cur_node->item & OPTIMUM_LEN_MASK;
+			unsigned offset = cur_node->item >>
+					  OPTIMUM_OFFSET_SHIFT;
+			if (length == 1) {
+				/* Literal */
+				ADD_BITS(codes->codewords.litlen[offset],
+					 codes->lens.litlen[offset]);
+				FLUSH_BITS();
+			} else {
+				/* Match */
+				WRITE_MATCH(c, codes, length, offset,
+					    c->p.n.offset_slot_full[offset]);
+			}
+			cur_node += length;
+		} while (cur_node != end_node);
+	} else
+#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
+	{
+		/* Output the literals and matches from the sequences list. */
+		const struct deflate_sequence *seq;
 
-	if (block_type == DEFLATE_BLOCKTYPE_UNCOMPRESSED) {
-		/* Note: the length being flushed may exceed the maximum length
-		 * of an uncompressed block (65535 bytes).  Therefore, more than
-		 * one uncompressed block might be needed. */
-		deflate_write_uncompressed_blocks(os, block_begin, block_length,
-						  is_final_block);
-	} else {
-		/* Output the block header. */
-		deflate_write_block_header(os, is_final_block, block_type);
+		for (seq = sequences; ; seq++) {
+			u32 litrunlen = seq->litrunlen_and_length &
+					SEQ_LITRUNLEN_MASK;
+			unsigned length = seq->litrunlen_and_length >>
+					  SEQ_LENGTH_SHIFT;
+			unsigned lit;
+
+			/* Output a run of literals. */
+			if (CAN_BUFFER(4 * MAX_LITLEN_CODEWORD_LEN)) {
+				for (; litrunlen >= 4; litrunlen -= 4) {
+					lit = *in_next++;
+					ADD_BITS(codes->codewords.litlen[lit],
+						 codes->lens.litlen[lit]);
+					lit = *in_next++;
+					ADD_BITS(codes->codewords.litlen[lit],
+						 codes->lens.litlen[lit]);
+					lit = *in_next++;
+					ADD_BITS(codes->codewords.litlen[lit],
+						 codes->lens.litlen[lit]);
+					lit = *in_next++;
+					ADD_BITS(codes->codewords.litlen[lit],
+						 codes->lens.litlen[lit]);
+					FLUSH_BITS();
+				}
+				if (litrunlen-- != 0) {
+					lit = *in_next++;
+					ADD_BITS(codes->codewords.litlen[lit],
+						 codes->lens.litlen[lit]);
+					if (litrunlen-- != 0) {
+						lit = *in_next++;
+						ADD_BITS(codes->codewords.litlen[lit],
+							 codes->lens.litlen[lit]);
+						if (litrunlen-- != 0) {
+							lit = *in_next++;
+							ADD_BITS(codes->codewords.litlen[lit],
+								 codes->lens.litlen[lit]);
+						}
+					}
+					FLUSH_BITS();
+				}
+			} else {
+				while (litrunlen--) {
+					lit = *in_next++;
+					ADD_BITS(codes->codewords.litlen[lit],
+						 codes->lens.litlen[lit]);
+					FLUSH_BITS();
+				}
+			}
 
-		/* Output the Huffman codes (dynamic Huffman blocks only). */
-		if (block_type == DEFLATE_BLOCKTYPE_DYNAMIC_HUFFMAN)
-			deflate_write_huffman_header(c, os);
+			if (length == 0) { /* Last sequence? */
+				ASSERT(in_next == in_end);
+				break;
+			}
 
-		/* Output the literals, matches, and end-of-block symbol. */
-	#if SUPPORT_NEAR_OPTIMAL_PARSING
-		if (use_item_list)
-			deflate_write_item_list(os, codes, c, block_length);
-		else
-	#endif
-			deflate_write_sequences(os, codes, c->p.g.sequences,
-						block_begin);
-		deflate_write_end_of_block(os, codes);
+			/* Output a match. */
+			WRITE_MATCH(c, codes, length, seq->offset,
+				    seq->offset_slot);
+			in_next += length;
+		}
 	}
-}
 
-static forceinline void
-deflate_choose_literal(struct libdeflate_compressor *c, unsigned literal,
-		       u32 *litrunlen_p)
-{
-	c->freqs.litlen[literal]++;
-	++*litrunlen_p;
-}
-
-static forceinline void
-deflate_choose_match(struct libdeflate_compressor *c,
-		     unsigned length, unsigned offset,
-		     u32 *litrunlen_p, struct deflate_sequence **next_seq_p)
-{
-	struct deflate_sequence *seq = *next_seq_p;
-	unsigned length_slot = deflate_length_slot[length];
-	unsigned offset_slot = deflate_get_offset_slot(c, offset);
-
-	c->freqs.litlen[257 + length_slot]++;
-	c->freqs.offset[offset_slot]++;
-
-	seq->litrunlen_and_length = ((u32)length << 23) | *litrunlen_p;
-	seq->offset = offset;
-	seq->length_slot = length_slot;
-	seq->offset_symbol = offset_slot;
+	/* Output the end-of-block symbol. */
+	ASSERT(bitcount <= 7);
+	ADD_BITS(codes->codewords.litlen[DEFLATE_END_OF_BLOCK],
+		 codes->lens.litlen[DEFLATE_END_OF_BLOCK]);
+	FLUSH_BITS();
+out:
+	ASSERT(bitcount <= 7);
+	/*
+	 * Assert that the block cost was computed correctly, as
+	 * libdeflate_deflate_compress_bound() relies on this via the assumption
+	 * that uncompressed blocks will always be used when cheaper.
+	 */
+	ASSERT(8 * (out_next - os->next) + bitcount - os->bitcount ==
+	       3 + best_cost || out_next == out_end);
 
-	*litrunlen_p = 0;
-	*next_seq_p = seq + 1;
+	os->bitbuf = bitbuf;
+	os->bitcount = bitcount;
+	os->next = out_next;
 }
 
-static forceinline void
-deflate_finish_sequence(struct deflate_sequence *seq, u32 litrunlen)
+static void
+deflate_finish_block(struct libdeflate_compressor *c,
+		     struct deflate_output_bitstream *os,
+		     const u8 *block_begin, u32 block_length,
+		     const struct deflate_sequence *sequences,
+		     bool is_final_block)
 {
-	seq->litrunlen_and_length = litrunlen; /* length = 0 */
+	c->freqs.litlen[DEFLATE_END_OF_BLOCK]++;
+	deflate_make_huffman_codes(&c->freqs, &c->codes);
+	deflate_flush_block(c, os, block_begin, block_length, sequences,
+			    is_final_block);
 }
 
 /******************************************************************************/
 
 /*
  * Block splitting algorithm.  The problem is to decide when it is worthwhile to
  * start a new block with new Huffman codes.  There is a theoretically optimal
@@ -1853,27 +2033,27 @@
  * start a new block.
  *
  * As an optimization and heuristic, we don't distinguish between every symbol
  * but rather we combine many symbols into a single "observation type".  For
  * literals we only look at the high bits and low bits, and for matches we only
  * look at whether the match is long or not.  The assumption is that for typical
  * "real" data, places that are good block boundaries will tend to be noticeable
- * based only on changes in these aggregate frequencies, without looking for
+ * based only on changes in these aggregate probabilities, without looking for
  * subtle differences in individual symbols.  For example, a change from ASCII
  * bytes to non-ASCII bytes, or from few matches (generally less compressible)
  * to many matches (generally more compressible), would be easily noticed based
  * on the aggregates.
  *
- * For determining whether the frequency distributions are "different enough" to
- * start a new block, the simply heuristic of splitting when the sum of absolute
- * differences exceeds a constant seems to be good enough.  We also add a number
- * proportional to the block length so that the algorithm is more likely to end
- * long blocks than short blocks.  This reflects the general expectation that it
- * will become increasingly beneficial to start a new block as the current
- * block grows longer.
+ * For determining whether the probability distributions are "different enough"
+ * to start a new block, the simple heuristic of splitting when the sum of
+ * absolute differences exceeds a constant seems to be good enough.  We also add
+ * a number proportional to the block length so that the algorithm is more
+ * likely to end long blocks than short blocks.  This reflects the general
+ * expectation that it will become increasingly beneficial to start a new block
+ * as the current block grows longer.
  *
  * Finally, for an approximation, it is not strictly necessary that the exact
  * symbols being used are considered.  With "near-optimal parsing", for example,
  * the actual symbols that will be used are unknown until after the block
  * boundary is chosen and the block has been optimized.  Since the final choices
  * cannot be used, we can use preliminary "greedy" choices instead.
  */
@@ -1888,474 +2068,1214 @@
 		stats->new_observations[i] = 0;
 		stats->observations[i] = 0;
 	}
 	stats->num_new_observations = 0;
 	stats->num_observations = 0;
 }
 
-/* Literal observation.  Heuristic: use the top 2 bits and low 1 bits of the
- * literal, for 8 possible literal observation types.  */
+/*
+ * Literal observation.  Heuristic: use the top 2 bits and low 1 bits of the
+ * literal, for 8 possible literal observation types.
+ */
 static forceinline void
 observe_literal(struct block_split_stats *stats, u8 lit)
 {
 	stats->new_observations[((lit >> 5) & 0x6) | (lit & 1)]++;
 	stats->num_new_observations++;
 }
 
-/* Match observation.  Heuristic: use one observation type for "short match" and
- * one observation type for "long match".  */
+/*
+ * Match observation.  Heuristic: use one observation type for "short match" and
+ * one observation type for "long match".
+ */
 static forceinline void
 observe_match(struct block_split_stats *stats, unsigned length)
 {
-	stats->new_observations[NUM_LITERAL_OBSERVATION_TYPES + (length >= 9)]++;
+	stats->new_observations[NUM_LITERAL_OBSERVATION_TYPES +
+				(length >= 9)]++;
 	stats->num_new_observations++;
 }
 
-static bool
-do_end_block_check(struct block_split_stats *stats, u32 block_length)
+static void
+merge_new_observations(struct block_split_stats *stats)
 {
 	int i;
 
-	if (stats->num_observations > 0) {
+	for (i = 0; i < NUM_OBSERVATION_TYPES; i++) {
+		stats->observations[i] += stats->new_observations[i];
+		stats->new_observations[i] = 0;
+	}
+	stats->num_observations += stats->num_new_observations;
+	stats->num_new_observations = 0;
+}
 
-		/* Note: to avoid slow divisions, we do not divide by
-		 * 'num_observations', but rather do all math with the numbers
-		 * multiplied by 'num_observations'.  */
+static bool
+do_end_block_check(struct block_split_stats *stats, u32 block_length)
+{
+	if (stats->num_observations > 0) {
+		/*
+		 * Compute the sum of absolute differences of probabilities.  To
+		 * avoid needing to use floating point arithmetic or do slow
+		 * divisions, we do all arithmetic with the probabilities
+		 * multiplied by num_observations * num_new_observations.  E.g.,
+		 * for the "old" observations the probabilities would be
+		 * (double)observations[i] / num_observations, but since we
+		 * multiply by both num_observations and num_new_observations we
+		 * really do observations[i] * num_new_observations.
+		 */
 		u32 total_delta = 0;
+		u32 num_items;
+		u32 cutoff;
+		int i;
+
 		for (i = 0; i < NUM_OBSERVATION_TYPES; i++) {
-			u32 expected = stats->observations[i] * stats->num_new_observations;
-			u32 actual = stats->new_observations[i] * stats->num_observations;
+			u32 expected = stats->observations[i] *
+				       stats->num_new_observations;
+			u32 actual = stats->new_observations[i] *
+				     stats->num_observations;
 			u32 delta = (actual > expected) ? actual - expected :
 							  expected - actual;
+
 			total_delta += delta;
 		}
 
+		num_items = stats->num_observations +
+			    stats->num_new_observations;
+		/*
+		 * Heuristic: the cutoff is when the sum of absolute differences
+		 * of probabilities becomes at least 200/512.  As above, the
+		 * probability is multiplied by both num_new_observations and
+		 * num_observations.  Be careful to avoid integer overflow.
+		 */
+		cutoff = stats->num_new_observations * 200 / 512 *
+			 stats->num_observations;
+		/*
+		 * Very short blocks have a lot of overhead for the Huffman
+		 * codes, so only use them if it clearly seems worthwhile.
+		 * (This is an additional penalty, which adds to the smaller
+		 * penalty below which scales more slowly.)
+		 */
+		if (block_length < 10000 && num_items < 8192)
+			cutoff += (u64)cutoff * (8192 - num_items) / 8192;
+
 		/* Ready to end the block? */
-		if (total_delta + (block_length / 4096) * stats->num_observations >=
-		    NUM_OBSERVATIONS_PER_BLOCK_CHECK * 200 / 512 * stats->num_observations)
+		if (total_delta +
+		    (block_length / 4096) * stats->num_observations >= cutoff)
 			return true;
 	}
-
-	for (i = 0; i < NUM_OBSERVATION_TYPES; i++) {
-		stats->num_observations += stats->new_observations[i];
-		stats->observations[i] += stats->new_observations[i];
-		stats->new_observations[i] = 0;
-	}
-	stats->num_new_observations = 0;
+	merge_new_observations(stats);
 	return false;
 }
 
 static forceinline bool
+ready_to_check_block(const struct block_split_stats *stats,
+		     const u8 *in_block_begin, const u8 *in_next,
+		     const u8 *in_end)
+{
+	return stats->num_new_observations >= NUM_OBSERVATIONS_PER_BLOCK_CHECK
+		&& in_next - in_block_begin >= MIN_BLOCK_LENGTH
+		&& in_end - in_next >= MIN_BLOCK_LENGTH;
+}
+
+static forceinline bool
 should_end_block(struct block_split_stats *stats,
 		 const u8 *in_block_begin, const u8 *in_next, const u8 *in_end)
 {
-	/* Ready to check block split statistics? */
-	if (stats->num_new_observations < NUM_OBSERVATIONS_PER_BLOCK_CHECK ||
-	    in_next - in_block_begin < MIN_BLOCK_LENGTH ||
-	    in_end - in_next < MIN_BLOCK_LENGTH)
+	/* Ready to try to end the block (again)? */
+	if (!ready_to_check_block(stats, in_block_begin, in_next, in_end))
 		return false;
 
 	return do_end_block_check(stats, in_next - in_block_begin);
 }
 
 /******************************************************************************/
 
+static void
+deflate_begin_sequences(struct libdeflate_compressor *c,
+			struct deflate_sequence *first_seq)
+{
+	deflate_reset_symbol_frequencies(c);
+	first_seq->litrunlen_and_length = 0;
+}
+
+static forceinline void
+deflate_choose_literal(struct libdeflate_compressor *c, unsigned literal,
+		       bool gather_split_stats, struct deflate_sequence *seq)
+{
+	c->freqs.litlen[literal]++;
+
+	if (gather_split_stats)
+		observe_literal(&c->split_stats, literal);
+
+	STATIC_ASSERT(MAX_BLOCK_LENGTH <= SEQ_LITRUNLEN_MASK);
+	seq->litrunlen_and_length++;
+}
+
+static forceinline void
+deflate_choose_match(struct libdeflate_compressor *c,
+		     unsigned length, unsigned offset, bool gather_split_stats,
+		     struct deflate_sequence **seq_p)
+{
+	struct deflate_sequence *seq = *seq_p;
+	unsigned length_slot = deflate_length_slot[length];
+	unsigned offset_slot = deflate_get_offset_slot(offset);
+
+	c->freqs.litlen[DEFLATE_FIRST_LEN_SYM + length_slot]++;
+	c->freqs.offset[offset_slot]++;
+	if (gather_split_stats)
+		observe_match(&c->split_stats, length);
+
+	seq->litrunlen_and_length |= (u32)length << SEQ_LENGTH_SHIFT;
+	seq->offset = offset;
+	seq->offset_slot = offset_slot;
+
+	seq++;
+	seq->litrunlen_and_length = 0;
+	*seq_p = seq;
+}
+
+/*
+ * Decrease the maximum and nice match lengths if we're approaching the end of
+ * the input buffer.
+ */
+static forceinline void
+adjust_max_and_nice_len(unsigned *max_len, unsigned *nice_len, size_t remaining)
+{
+	if (unlikely(remaining < DEFLATE_MAX_MATCH_LEN)) {
+		*max_len = remaining;
+		*nice_len = MIN(*nice_len, *max_len);
+	}
+}
+
+/*
+ * Choose the minimum match length for the greedy and lazy parsers.
+ *
+ * By default the minimum match length is 3, which is the smallest length the
+ * DEFLATE format allows.  However, with greedy and lazy parsing, some data
+ * (e.g. DNA sequencing data) benefits greatly from a longer minimum length.
+ * Typically, this is because literals are very cheap.  In general, the
+ * near-optimal parser handles this case naturally, but the greedy and lazy
+ * parsers need a heuristic to decide when to use short matches.
+ *
+ * The heuristic we use is to make the minimum match length depend on the number
+ * of different literals that exist in the data.  If there are many different
+ * literals, then literals will probably be expensive, so short matches will
+ * probably be worthwhile.  Conversely, if not many literals are used, then
+ * probably literals will be cheap and short matches won't be worthwhile.
+ */
+static unsigned
+choose_min_match_len(unsigned num_used_literals, unsigned max_search_depth)
+{
+	/* map from num_used_literals to min_len */
+	static const u8 min_lens[] = {
+		9, 9, 9, 9, 9, 9, 8, 8, 7, 7, 6, 6, 6, 6, 6, 6,
+		5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5,
+		5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 4, 4, 4,
+		4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
+		4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4,
+		/* The rest is implicitly 3. */
+	};
+	unsigned min_len;
+
+	STATIC_ASSERT(DEFLATE_MIN_MATCH_LEN <= 3);
+	STATIC_ASSERT(ARRAY_LEN(min_lens) <= DEFLATE_NUM_LITERALS + 1);
+
+	if (num_used_literals >= ARRAY_LEN(min_lens))
+		return 3;
+	min_len = min_lens[num_used_literals];
+	/*
+	 * With a low max_search_depth, it may be too hard to find long matches.
+	 */
+	if (max_search_depth < 16) {
+		if (max_search_depth < 5)
+			min_len = MIN(min_len, 4);
+		else if (max_search_depth < 10)
+			min_len = MIN(min_len, 5);
+		else
+			min_len = MIN(min_len, 7);
+	}
+	return min_len;
+}
+
+static unsigned
+calculate_min_match_len(const u8 *data, size_t data_len,
+			unsigned max_search_depth)
+{
+	u8 used[256] = { 0 };
+	unsigned num_used_literals = 0;
+	size_t i;
+
+	/*
+	 * For an initial approximation, scan the first 4 KiB of data.  The
+	 * caller may use recalculate_min_match_len() to update min_len later.
+	 */
+	data_len = MIN(data_len, 4096);
+	for (i = 0; i < data_len; i++)
+		used[data[i]] = 1;
+	for (i = 0; i < 256; i++)
+		num_used_literals += used[i];
+	return choose_min_match_len(num_used_literals, max_search_depth);
+}
+
+/*
+ * Recalculate the minimum match length for a block, now that we know the
+ * distribution of literals that are actually being used (freqs->litlen).
+ */
+static unsigned
+recalculate_min_match_len(const struct deflate_freqs *freqs,
+			  unsigned max_search_depth)
+{
+	u32 literal_freq = 0;
+	u32 cutoff;
+	unsigned num_used_literals = 0;
+	int i;
+
+	for (i = 0; i < DEFLATE_NUM_LITERALS; i++)
+		literal_freq += freqs->litlen[i];
+
+	cutoff = literal_freq >> 10; /* Ignore literals used very rarely. */
+
+	for (i = 0; i < DEFLATE_NUM_LITERALS; i++) {
+		if (freqs->litlen[i] > cutoff)
+			num_used_literals++;
+	}
+	return choose_min_match_len(num_used_literals, max_search_depth);
+}
+
+static forceinline const u8 *
+choose_max_block_end(const u8 *in_block_begin, const u8 *in_end,
+		     size_t soft_max_len)
+{
+	if (in_end - in_block_begin < soft_max_len + MIN_BLOCK_LENGTH)
+		return in_end;
+	return in_block_begin + soft_max_len;
+}
+
 /*
  * This is the level 0 "compressor".  It always outputs uncompressed blocks.
  */
 static size_t
-deflate_compress_none(struct libdeflate_compressor * restrict c,
-		      const u8 * restrict in, size_t in_nbytes,
-		      u8 * restrict out, size_t out_nbytes_avail)
+deflate_compress_none(const u8 *in, size_t in_nbytes,
+		      u8 *out, size_t out_nbytes_avail)
 {
-	struct deflate_output_bitstream os;
+	const u8 *in_next = in;
+	const u8 * const in_end = in + in_nbytes;
+	u8 *out_next = out;
+	u8 * const out_end = out + out_nbytes_avail;
+
+	/*
+	 * If the input is zero-length, we still must output a block in order
+	 * for the output to be a valid DEFLATE stream.  Handle this case
+	 * specially to avoid potentially passing NULL to memcpy() below.
+	 */
+	if (unlikely(in_nbytes == 0)) {
+		if (out_nbytes_avail < 5)
+			return 0;
+		/* BFINAL and BTYPE */
+		*out_next++ = 1 | (DEFLATE_BLOCKTYPE_UNCOMPRESSED << 1);
+		/* LEN and NLEN */
+		put_unaligned_le32(0xFFFF0000, out_next);
+		return 5;
+	}
+
+	do {
+		u8 bfinal = 0;
+		size_t len = UINT16_MAX;
 
-	deflate_init_output(&os, out, out_nbytes_avail);
+		if (in_end - in_next <= UINT16_MAX) {
+			bfinal = 1;
+			len = in_end - in_next;
+		}
+		if (out_end - out_next < 5 + len)
+			return 0;
+		/*
+		 * Output BFINAL and BTYPE.  The stream is already byte-aligned
+		 * here, so this step always requires outputting exactly 1 byte.
+		 */
+		*out_next++ = bfinal | (DEFLATE_BLOCKTYPE_UNCOMPRESSED << 1);
 
-	deflate_write_uncompressed_blocks(&os, in, in_nbytes, true);
+		/* Output LEN and NLEN, then the data itself. */
+		put_unaligned_le16(len, out_next);
+		out_next += 2;
+		put_unaligned_le16(~len, out_next);
+		out_next += 2;
+		memcpy(out_next, in_next, len);
+		out_next += len;
+		in_next += len;
+	} while (in_next != in_end);
 
-	return deflate_flush_output(&os);
+	return out_next - out;
 }
 
 /*
- * This is the "greedy" DEFLATE compressor. It always chooses the longest match.
+ * This is a faster variant of deflate_compress_greedy().  It uses the
+ * ht_matchfinder rather than the hc_matchfinder.  It also skips the block
+ * splitting algorithm and just uses fixed length blocks.  c->max_search_depth
+ * has no effect with this algorithm, as it is hardcoded in ht_matchfinder.h.
  */
-static size_t
-deflate_compress_greedy(struct libdeflate_compressor * restrict c,
-			const u8 * restrict in, size_t in_nbytes,
-			u8 * restrict out, size_t out_nbytes_avail)
+static void
+deflate_compress_fastest(struct libdeflate_compressor * restrict c,
+			 const u8 *in, size_t in_nbytes,
+			 struct deflate_output_bitstream *os)
 {
 	const u8 *in_next = in;
 	const u8 *in_end = in_next + in_nbytes;
-	struct deflate_output_bitstream os;
 	const u8 *in_cur_base = in_next;
 	unsigned max_len = DEFLATE_MAX_MATCH_LEN;
 	unsigned nice_len = MIN(c->nice_match_length, max_len);
-	u32 next_hashes[2] = {0, 0};
+	u32 next_hash = 0;
 
-	deflate_init_output(&os, out, out_nbytes_avail);
-	hc_matchfinder_init(&c->p.g.hc_mf);
+	ht_matchfinder_init(&c->p.f.ht_mf);
 
 	do {
-		/* Starting a new DEFLATE block.  */
+		/* Starting a new DEFLATE block */
 
 		const u8 * const in_block_begin = in_next;
-		const u8 * const in_max_block_end =
-			in_next + MIN(in_end - in_next, SOFT_MAX_BLOCK_LENGTH);
-		u32 litrunlen = 0;
-		struct deflate_sequence *next_seq = c->p.g.sequences;
+		const u8 * const in_max_block_end = choose_max_block_end(
+				in_next, in_end, FAST_SOFT_MAX_BLOCK_LENGTH);
+		struct deflate_sequence *seq = c->p.f.sequences;
 
-		init_block_split_stats(&c->split_stats);
-		deflate_reset_symbol_frequencies(c);
+		deflate_begin_sequences(c, seq);
 
 		do {
 			u32 length;
 			u32 offset;
+			size_t remaining = in_end - in_next;
 
-			/* Decrease the maximum and nice match lengths if we're
-			 * approaching the end of the input buffer.  */
-			if (unlikely(max_len > in_end - in_next)) {
-				max_len = in_end - in_next;
+			if (unlikely(remaining < DEFLATE_MAX_MATCH_LEN)) {
+				max_len = remaining;
+				if (max_len < HT_MATCHFINDER_REQUIRED_NBYTES) {
+					do {
+						deflate_choose_literal(c,
+							*in_next++, false, seq);
+					} while (--max_len);
+					break;
+				}
 				nice_len = MIN(nice_len, max_len);
 			}
-
-			length = hc_matchfinder_longest_match(&c->p.g.hc_mf,
+			length = ht_matchfinder_longest_match(&c->p.f.ht_mf,
 							      &in_cur_base,
 							      in_next,
-							      DEFLATE_MIN_MATCH_LEN - 1,
 							      max_len,
 							      nice_len,
-							      c->max_search_depth,
-							      next_hashes,
+							      &next_hash,
 							      &offset);
-
-			if (length >= DEFLATE_MIN_MATCH_LEN) {
-				/* Match found.  */
-				deflate_choose_match(c, length, offset,
-						     &litrunlen, &next_seq);
-				observe_match(&c->split_stats, length);
-				in_next = hc_matchfinder_skip_positions(&c->p.g.hc_mf,
-									&in_cur_base,
-									in_next + 1,
-									in_end,
-									length - 1,
-									next_hashes);
+			if (length) {
+				/* Match found */
+				deflate_choose_match(c, length, offset, false,
+						     &seq);
+				ht_matchfinder_skip_bytes(&c->p.f.ht_mf,
+							  &in_cur_base,
+							  in_next + 1,
+							  in_end,
+							  length - 1,
+							  &next_hash);
+				in_next += length;
 			} else {
-				/* No match found.  */
-				deflate_choose_literal(c, *in_next, &litrunlen);
-				observe_literal(&c->split_stats, *in_next);
-				in_next++;
+				/* No match found */
+				deflate_choose_literal(c, *in_next++, false,
+						       seq);
 			}
 
-			/* Check if it's time to output another block.  */
+			/* Check if it's time to output another block. */
 		} while (in_next < in_max_block_end &&
-			 !should_end_block(&c->split_stats, in_block_begin, in_next, in_end));
+			 seq < &c->p.f.sequences[FAST_SEQ_STORE_LENGTH]);
 
-		deflate_finish_sequence(next_seq, litrunlen);
-		deflate_flush_block(c, &os, in_block_begin,
-				    in_next - in_block_begin,
-				    in_next == in_end, false);
+		deflate_finish_block(c, os, in_block_begin,
+				     in_next - in_block_begin,
+				     c->p.f.sequences, in_next == in_end);
 	} while (in_next != in_end);
-
-	return deflate_flush_output(&os);
 }
 
 /*
- * This is the "lazy" DEFLATE compressor.  Before choosing a match, it checks to
- * see if there's a longer match at the next position.  If yes, it outputs a
- * literal and continues to the next position.  If no, it outputs the match.
+ * This is the "greedy" DEFLATE compressor. It always chooses the longest match.
  */
-static size_t
-deflate_compress_lazy(struct libdeflate_compressor * restrict c,
-		      const u8 * restrict in, size_t in_nbytes,
-		      u8 * restrict out, size_t out_nbytes_avail)
+static void
+deflate_compress_greedy(struct libdeflate_compressor * restrict c,
+			const u8 *in, size_t in_nbytes,
+			struct deflate_output_bitstream *os)
 {
 	const u8 *in_next = in;
 	const u8 *in_end = in_next + in_nbytes;
-	struct deflate_output_bitstream os;
 	const u8 *in_cur_base = in_next;
 	unsigned max_len = DEFLATE_MAX_MATCH_LEN;
 	unsigned nice_len = MIN(c->nice_match_length, max_len);
 	u32 next_hashes[2] = {0, 0};
 
-	deflate_init_output(&os, out, out_nbytes_avail);
 	hc_matchfinder_init(&c->p.g.hc_mf);
 
 	do {
-		/* Starting a new DEFLATE block.  */
+		/* Starting a new DEFLATE block */
 
 		const u8 * const in_block_begin = in_next;
-		const u8 * const in_max_block_end =
-			in_next + MIN(in_end - in_next, SOFT_MAX_BLOCK_LENGTH);
-		u32 litrunlen = 0;
-		struct deflate_sequence *next_seq = c->p.g.sequences;
+		const u8 * const in_max_block_end = choose_max_block_end(
+				in_next, in_end, SOFT_MAX_BLOCK_LENGTH);
+		struct deflate_sequence *seq = c->p.g.sequences;
+		unsigned min_len;
 
 		init_block_split_stats(&c->split_stats);
-		deflate_reset_symbol_frequencies(c);
+		deflate_begin_sequences(c, seq);
+		min_len = calculate_min_match_len(in_next,
+						  in_max_block_end - in_next,
+						  c->max_search_depth);
+		do {
+			u32 length;
+			u32 offset;
+
+			adjust_max_and_nice_len(&max_len, &nice_len,
+						in_end - in_next);
+			length = hc_matchfinder_longest_match(
+						&c->p.g.hc_mf,
+						&in_cur_base,
+						in_next,
+						min_len - 1,
+						max_len,
+						nice_len,
+						c->max_search_depth,
+						next_hashes,
+						&offset);
+
+			if (length >= min_len &&
+			    (length > DEFLATE_MIN_MATCH_LEN ||
+			     offset <= 4096)) {
+				/* Match found */
+				deflate_choose_match(c, length, offset, true,
+						     &seq);
+				hc_matchfinder_skip_bytes(&c->p.g.hc_mf,
+							  &in_cur_base,
+							  in_next + 1,
+							  in_end,
+							  length - 1,
+							  next_hashes);
+				in_next += length;
+			} else {
+				/* No match found */
+				deflate_choose_literal(c, *in_next++, true,
+						       seq);
+			}
+
+			/* Check if it's time to output another block. */
+		} while (in_next < in_max_block_end &&
+			 seq < &c->p.g.sequences[SEQ_STORE_LENGTH] &&
+			 !should_end_block(&c->split_stats,
+					   in_block_begin, in_next, in_end));
+
+		deflate_finish_block(c, os, in_block_begin,
+				     in_next - in_block_begin,
+				     c->p.g.sequences, in_next == in_end);
+	} while (in_next != in_end);
+}
+
+static forceinline void
+deflate_compress_lazy_generic(struct libdeflate_compressor * restrict c,
+			      const u8 *in, size_t in_nbytes,
+			      struct deflate_output_bitstream *os, bool lazy2)
+{
+	const u8 *in_next = in;
+	const u8 *in_end = in_next + in_nbytes;
+	const u8 *in_cur_base = in_next;
+	unsigned max_len = DEFLATE_MAX_MATCH_LEN;
+	unsigned nice_len = MIN(c->nice_match_length, max_len);
+	u32 next_hashes[2] = {0, 0};
+
+	hc_matchfinder_init(&c->p.g.hc_mf);
+
+	do {
+		/* Starting a new DEFLATE block */
 
+		const u8 * const in_block_begin = in_next;
+		const u8 * const in_max_block_end = choose_max_block_end(
+				in_next, in_end, SOFT_MAX_BLOCK_LENGTH);
+		const u8 *next_recalc_min_len =
+			in_next + MIN(in_end - in_next, 10000);
+		struct deflate_sequence *seq = c->p.g.sequences;
+		unsigned min_len;
+
+		init_block_split_stats(&c->split_stats);
+		deflate_begin_sequences(c, seq);
+		min_len = calculate_min_match_len(in_next,
+						  in_max_block_end - in_next,
+						  c->max_search_depth);
 		do {
 			unsigned cur_len;
 			unsigned cur_offset;
 			unsigned next_len;
 			unsigned next_offset;
 
-			if (unlikely(in_end - in_next < DEFLATE_MAX_MATCH_LEN)) {
-				max_len = in_end - in_next;
-				nice_len = MIN(nice_len, max_len);
+			/*
+			 * Recalculate the minimum match length if it hasn't
+			 * been done recently.
+			 */
+			if (in_next >= next_recalc_min_len) {
+				min_len = recalculate_min_match_len(
+						&c->freqs,
+						c->max_search_depth);
+				next_recalc_min_len +=
+					MIN(in_end - next_recalc_min_len,
+					    in_next - in_block_begin);
 			}
 
-			/* Find the longest match at the current position.  */
-			cur_len = hc_matchfinder_longest_match(&c->p.g.hc_mf,
-							       &in_cur_base,
-							       in_next,
-							       DEFLATE_MIN_MATCH_LEN - 1,
-							       max_len,
-							       nice_len,
-							       c->max_search_depth,
-							       next_hashes,
-							       &cur_offset);
-			in_next += 1;
-
-			if (cur_len < DEFLATE_MIN_MATCH_LEN) {
-				/* No match found.  Choose a literal.  */
-				deflate_choose_literal(c, *(in_next - 1), &litrunlen);
-				observe_literal(&c->split_stats, *(in_next - 1));
+			/* Find the longest match at the current position. */
+			adjust_max_and_nice_len(&max_len, &nice_len,
+						in_end - in_next);
+			cur_len = hc_matchfinder_longest_match(
+						&c->p.g.hc_mf,
+						&in_cur_base,
+						in_next,
+						min_len - 1,
+						max_len,
+						nice_len,
+						c->max_search_depth,
+						next_hashes,
+						&cur_offset);
+			if (cur_len < min_len ||
+			    (cur_len == DEFLATE_MIN_MATCH_LEN &&
+			     cur_offset > 8192)) {
+				/* No match found.  Choose a literal. */
+				deflate_choose_literal(c, *in_next++, true,
+						       seq);
 				continue;
 			}
+			in_next++;
 
-		have_cur_match:
-			observe_match(&c->split_stats, cur_len);
-
-			/* We have a match at the current position.  */
-
-			/* If the current match is very long, choose it
-			 * immediately.  */
+have_cur_match:
+			/*
+			 * We have a match at the current position.
+			 * If it's very long, choose it immediately.
+			 */
 			if (cur_len >= nice_len) {
 				deflate_choose_match(c, cur_len, cur_offset,
-						     &litrunlen, &next_seq);
-				in_next = hc_matchfinder_skip_positions(&c->p.g.hc_mf,
-									&in_cur_base,
-									in_next,
-									in_end,
-									cur_len - 1,
-									next_hashes);
+						     true, &seq);
+				hc_matchfinder_skip_bytes(&c->p.g.hc_mf,
+							  &in_cur_base,
+							  in_next,
+							  in_end,
+							  cur_len - 1,
+							  next_hashes);
+				in_next += cur_len - 1;
 				continue;
 			}
 
 			/*
-			 * Try to find a match at the next position.
+			 * Try to find a better match at the next position.
 			 *
 			 * Note: since we already have a match at the *current*
 			 * position, we use only half the 'max_search_depth'
 			 * when checking the *next* position.  This is a useful
 			 * trade-off because it's more worthwhile to use a
 			 * greater search depth on the initial match.
 			 *
 			 * Note: it's possible to structure the code such that
 			 * there's only one call to longest_match(), which
 			 * handles both the "find the initial match" and "try to
-			 * find a longer match" cases.  However, it is faster to
+			 * find a better match" cases.  However, it is faster to
 			 * have two call sites, with longest_match() inlined at
 			 * each.
 			 */
-			if (unlikely(in_end - in_next < DEFLATE_MAX_MATCH_LEN)) {
-				max_len = in_end - in_next;
-				nice_len = MIN(nice_len, max_len);
-			}
-			next_len = hc_matchfinder_longest_match(&c->p.g.hc_mf,
-								&in_cur_base,
-								in_next,
-								cur_len,
-								max_len,
-								nice_len,
-								c->max_search_depth / 2,
-								next_hashes,
-								&next_offset);
-			in_next += 1;
-
-			if (next_len > cur_len) {
-				/* Found a longer match at the next position.
+			adjust_max_and_nice_len(&max_len, &nice_len,
+						in_end - in_next);
+			next_len = hc_matchfinder_longest_match(
+						&c->p.g.hc_mf,
+						&in_cur_base,
+						in_next++,
+						cur_len - 1,
+						max_len,
+						nice_len,
+						c->max_search_depth >> 1,
+						next_hashes,
+						&next_offset);
+			if (next_len >= cur_len &&
+			    4 * (int)(next_len - cur_len) +
+			    ((int)bsr32(cur_offset) -
+			     (int)bsr32(next_offset)) > 2) {
+				/*
+				 * Found a better match at the next position.
 				 * Output a literal.  Then the next match
-				 * becomes the current match.  */
-				deflate_choose_literal(c, *(in_next - 2), &litrunlen);
+				 * becomes the current match.
+				 */
+				deflate_choose_literal(c, *(in_next - 2), true,
+						       seq);
 				cur_len = next_len;
 				cur_offset = next_offset;
 				goto have_cur_match;
 			}
 
-			/* No longer match at the next position.
-			 * Output the current match.  */
-			deflate_choose_match(c, cur_len, cur_offset,
-					     &litrunlen, &next_seq);
-			in_next = hc_matchfinder_skip_positions(&c->p.g.hc_mf,
-								&in_cur_base,
-								in_next,
-								in_end,
-								cur_len - 2,
-								next_hashes);
-
-			/* Check if it's time to output another block.  */
+			if (lazy2) {
+				/* In lazy2 mode, look ahead another position */
+				adjust_max_and_nice_len(&max_len, &nice_len,
+							in_end - in_next);
+				next_len = hc_matchfinder_longest_match(
+						&c->p.g.hc_mf,
+						&in_cur_base,
+						in_next++,
+						cur_len - 1,
+						max_len,
+						nice_len,
+						c->max_search_depth >> 2,
+						next_hashes,
+						&next_offset);
+				if (next_len >= cur_len &&
+				    4 * (int)(next_len - cur_len) +
+				    ((int)bsr32(cur_offset) -
+				     (int)bsr32(next_offset)) > 6) {
+					/*
+					 * There's a much better match two
+					 * positions ahead, so use two literals.
+					 */
+					deflate_choose_literal(
+						c, *(in_next - 3), true, seq);
+					deflate_choose_literal(
+						c, *(in_next - 2), true, seq);
+					cur_len = next_len;
+					cur_offset = next_offset;
+					goto have_cur_match;
+				}
+				/*
+				 * No better match at either of the next 2
+				 * positions.  Output the current match.
+				 */
+				deflate_choose_match(c, cur_len, cur_offset,
+						     true, &seq);
+				if (cur_len > 3) {
+					hc_matchfinder_skip_bytes(&c->p.g.hc_mf,
+								  &in_cur_base,
+								  in_next,
+								  in_end,
+								  cur_len - 3,
+								  next_hashes);
+					in_next += cur_len - 3;
+				}
+			} else { /* !lazy2 */
+				/*
+				 * No better match at the next position.  Output
+				 * the current match.
+				 */
+				deflate_choose_match(c, cur_len, cur_offset,
+						     true, &seq);
+				hc_matchfinder_skip_bytes(&c->p.g.hc_mf,
+							  &in_cur_base,
+							  in_next,
+							  in_end,
+							  cur_len - 2,
+							  next_hashes);
+				in_next += cur_len - 2;
+			}
+			/* Check if it's time to output another block. */
 		} while (in_next < in_max_block_end &&
-			 !should_end_block(&c->split_stats, in_block_begin, in_next, in_end));
-
-		deflate_finish_sequence(next_seq, litrunlen);
-		deflate_flush_block(c, &os, in_block_begin,
-				    in_next - in_block_begin,
-				    in_next == in_end, false);
+			 seq < &c->p.g.sequences[SEQ_STORE_LENGTH] &&
+			 !should_end_block(&c->split_stats,
+					   in_block_begin, in_next, in_end));
+
+		deflate_finish_block(c, os, in_block_begin,
+				     in_next - in_block_begin,
+				     c->p.g.sequences, in_next == in_end);
 	} while (in_next != in_end);
+}
 
-	return deflate_flush_output(&os);
+/*
+ * This is the "lazy" DEFLATE compressor.  Before choosing a match, it checks to
+ * see if there's a better match at the next position.  If yes, it outputs a
+ * literal and continues to the next position.  If no, it outputs the match.
+ */
+static void
+deflate_compress_lazy(struct libdeflate_compressor * restrict c,
+		      const u8 *in, size_t in_nbytes,
+		      struct deflate_output_bitstream *os)
+{
+	deflate_compress_lazy_generic(c, in, in_nbytes, os, false);
+}
+
+/*
+ * The lazy2 compressor.  This is similar to the regular lazy one, but it looks
+ * for a better match at the next 2 positions rather than the next 1.  This
+ * makes it take slightly more time, but compress some inputs slightly more.
+ */
+static void
+deflate_compress_lazy2(struct libdeflate_compressor * restrict c,
+		       const u8 *in, size_t in_nbytes,
+		       struct deflate_output_bitstream *os)
+{
+	deflate_compress_lazy_generic(c, in, in_nbytes, os, true);
 }
 
 #if SUPPORT_NEAR_OPTIMAL_PARSING
 
 /*
  * Follow the minimum-cost path in the graph of possible match/literal choices
  * for the current block and compute the frequencies of the Huffman symbols that
  * would be needed to output those matches and literals.
  */
 static void
 deflate_tally_item_list(struct libdeflate_compressor *c, u32 block_length)
 {
 	struct deflate_optimum_node *cur_node = &c->p.n.optimum_nodes[0];
-	struct deflate_optimum_node *end_node = &c->p.n.optimum_nodes[block_length];
+	struct deflate_optimum_node *end_node =
+		&c->p.n.optimum_nodes[block_length];
+
 	do {
 		unsigned length = cur_node->item & OPTIMUM_LEN_MASK;
 		unsigned offset = cur_node->item >> OPTIMUM_OFFSET_SHIFT;
 
 		if (length == 1) {
-			/* Literal  */
+			/* Literal */
 			c->freqs.litlen[offset]++;
 		} else {
-			/* Match  */
-			c->freqs.litlen[257 + deflate_length_slot[length]]++;
-			c->freqs.offset[deflate_get_offset_slot(c, offset)]++;
+			/* Match */
+			c->freqs.litlen[DEFLATE_FIRST_LEN_SYM +
+					deflate_length_slot[length]]++;
+			c->freqs.offset[c->p.n.offset_slot_full[offset]]++;
 		}
 		cur_node += length;
 	} while (cur_node != end_node);
+
+	/* Tally the end-of-block symbol. */
+	c->freqs.litlen[DEFLATE_END_OF_BLOCK]++;
 }
 
-/* Set the current cost model from the codeword lengths specified in @lens.  */
+static void
+deflate_choose_all_literals(struct libdeflate_compressor *c,
+			    const u8 *block, u32 block_length)
+{
+	u32 i;
+
+	deflate_reset_symbol_frequencies(c);
+	for (i = 0; i < block_length; i++)
+		c->freqs.litlen[block[i]]++;
+	c->freqs.litlen[DEFLATE_END_OF_BLOCK]++;
+
+	deflate_make_huffman_codes(&c->freqs, &c->codes);
+}
+
+/*
+ * Compute the exact cost, in bits, that would be required to output the matches
+ * and literals described by @c->freqs as a dynamic Huffman block.  The litlen
+ * and offset codes are assumed to have already been built in @c->codes.
+ */
+static u32
+deflate_compute_true_cost(struct libdeflate_compressor *c)
+{
+	u32 cost = 0;
+	unsigned sym;
+
+	deflate_precompute_huffman_header(c);
+
+	memset(&c->codes.lens.litlen[c->o.precode.num_litlen_syms], 0,
+	       DEFLATE_NUM_LITLEN_SYMS - c->o.precode.num_litlen_syms);
+
+	cost += 5 + 5 + 4 + (3 * c->o.precode.num_explicit_lens);
+	for (sym = 0; sym < DEFLATE_NUM_PRECODE_SYMS; sym++) {
+		cost += c->o.precode.freqs[sym] *
+			(c->o.precode.lens[sym] +
+			 deflate_extra_precode_bits[sym]);
+	}
+
+	for (sym = 0; sym < DEFLATE_FIRST_LEN_SYM; sym++)
+		cost += c->freqs.litlen[sym] * c->codes.lens.litlen[sym];
+
+	for (; sym < DEFLATE_FIRST_LEN_SYM +
+	       ARRAY_LEN(deflate_extra_length_bits); sym++)
+		cost += c->freqs.litlen[sym] *
+			(c->codes.lens.litlen[sym] +
+			 deflate_extra_length_bits[sym - DEFLATE_FIRST_LEN_SYM]);
+
+	for (sym = 0; sym < ARRAY_LEN(deflate_extra_offset_bits); sym++)
+		cost += c->freqs.offset[sym] *
+			(c->codes.lens.offset[sym] +
+			 deflate_extra_offset_bits[sym]);
+	return cost;
+}
+
+/* Set the current cost model from the codeword lengths specified in @lens. */
 static void
 deflate_set_costs_from_codes(struct libdeflate_compressor *c,
 			     const struct deflate_lens *lens)
 {
 	unsigned i;
 
-	/* Literals  */
+	/* Literals */
 	for (i = 0; i < DEFLATE_NUM_LITERALS; i++) {
-		u32 bits = (lens->litlen[i] ? lens->litlen[i] : LITERAL_NOSTAT_BITS);
-		c->p.n.costs.literal[i] = bits << COST_SHIFT;
+		u32 bits = (lens->litlen[i] ?
+			    lens->litlen[i] : LITERAL_NOSTAT_BITS);
+
+		c->p.n.costs.literal[i] = bits * BIT_COST;
 	}
 
-	/* Lengths  */
+	/* Lengths */
 	for (i = DEFLATE_MIN_MATCH_LEN; i <= DEFLATE_MAX_MATCH_LEN; i++) {
 		unsigned length_slot = deflate_length_slot[i];
-		unsigned litlen_sym = 257 + length_slot;
-		u32 bits = (lens->litlen[litlen_sym] ? lens->litlen[litlen_sym] : LENGTH_NOSTAT_BITS);
+		unsigned litlen_sym = DEFLATE_FIRST_LEN_SYM + length_slot;
+		u32 bits = (lens->litlen[litlen_sym] ?
+			    lens->litlen[litlen_sym] : LENGTH_NOSTAT_BITS);
+
 		bits += deflate_extra_length_bits[length_slot];
-		c->p.n.costs.length[i] = bits << COST_SHIFT;
+		c->p.n.costs.length[i] = bits * BIT_COST;
 	}
 
-	/* Offset slots  */
+	/* Offset slots */
 	for (i = 0; i < ARRAY_LEN(deflate_offset_slot_base); i++) {
-		u32 bits = (lens->offset[i] ? lens->offset[i] : OFFSET_NOSTAT_BITS);
+		u32 bits = (lens->offset[i] ?
+			    lens->offset[i] : OFFSET_NOSTAT_BITS);
+
 		bits += deflate_extra_offset_bits[i];
-		c->p.n.costs.offset_slot[i] = bits << COST_SHIFT;
+		c->p.n.costs.offset_slot[i] = bits * BIT_COST;
 	}
 }
 
-static forceinline u32
-deflate_default_literal_cost(unsigned literal)
-{
-	STATIC_ASSERT(COST_SHIFT == 3);
-	/* 66 is 8.25 bits/symbol  */
-	return 66;
+/*
+ * This lookup table gives the default cost of a literal symbol and of a length
+ * symbol, depending on the characteristics of the input data.  It was generated
+ * by scripts/gen_default_litlen_costs.py.
+ *
+ * This table is indexed first by the estimated match probability:
+ *
+ *	i=0: data doesn't contain many matches	[match_prob=0.25]
+ *	i=1: neutral				[match_prob=0.50]
+ *	i=2: data contains lots of matches	[match_prob=0.75]
+ *
+ * This lookup produces a subtable which maps the number of distinct used
+ * literals to the default cost of a literal symbol, i.e.:
+ *
+ *	int(-log2((1 - match_prob) / num_used_literals) * BIT_COST)
+ *
+ * ... for num_used_literals in [1, 256] (and 0, which is copied from 1).  This
+ * accounts for literals usually getting cheaper as the number of distinct
+ * literals decreases, and as the proportion of literals to matches increases.
+ *
+ * The lookup also produces the cost of a length symbol, which is:
+ *
+ *	int(-log2(match_prob/NUM_LEN_SLOTS) * BIT_COST)
+ *
+ * Note: we don't currently assign different costs to different literal symbols,
+ * or to different length symbols, as this is hard to do in a useful way.
+ */
+static const struct {
+	u8 used_lits_to_lit_cost[257];
+	u8 len_sym_cost;
+} default_litlen_costs[] = {
+	{ /* match_prob = 0.25 */
+		.used_lits_to_lit_cost = {
+			6, 6, 22, 32, 38, 43, 48, 51,
+			54, 57, 59, 61, 64, 65, 67, 69,
+			70, 72, 73, 74, 75, 76, 77, 79,
+			80, 80, 81, 82, 83, 84, 85, 85,
+			86, 87, 88, 88, 89, 89, 90, 91,
+			91, 92, 92, 93, 93, 94, 95, 95,
+			96, 96, 96, 97, 97, 98, 98, 99,
+			99, 99, 100, 100, 101, 101, 101, 102,
+			102, 102, 103, 103, 104, 104, 104, 105,
+			105, 105, 105, 106, 106, 106, 107, 107,
+			107, 108, 108, 108, 108, 109, 109, 109,
+			109, 110, 110, 110, 111, 111, 111, 111,
+			112, 112, 112, 112, 112, 113, 113, 113,
+			113, 114, 114, 114, 114, 114, 115, 115,
+			115, 115, 115, 116, 116, 116, 116, 116,
+			117, 117, 117, 117, 117, 118, 118, 118,
+			118, 118, 118, 119, 119, 119, 119, 119,
+			120, 120, 120, 120, 120, 120, 121, 121,
+			121, 121, 121, 121, 121, 122, 122, 122,
+			122, 122, 122, 123, 123, 123, 123, 123,
+			123, 123, 124, 124, 124, 124, 124, 124,
+			124, 125, 125, 125, 125, 125, 125, 125,
+			125, 126, 126, 126, 126, 126, 126, 126,
+			127, 127, 127, 127, 127, 127, 127, 127,
+			128, 128, 128, 128, 128, 128, 128, 128,
+			128, 129, 129, 129, 129, 129, 129, 129,
+			129, 129, 130, 130, 130, 130, 130, 130,
+			130, 130, 130, 131, 131, 131, 131, 131,
+			131, 131, 131, 131, 131, 132, 132, 132,
+			132, 132, 132, 132, 132, 132, 132, 133,
+			133, 133, 133, 133, 133, 133, 133, 133,
+			133, 134, 134, 134, 134, 134, 134, 134,
+			134,
+		},
+		.len_sym_cost = 109,
+	}, { /* match_prob = 0.5 */
+		.used_lits_to_lit_cost = {
+			16, 16, 32, 41, 48, 53, 57, 60,
+			64, 66, 69, 71, 73, 75, 76, 78,
+			80, 81, 82, 83, 85, 86, 87, 88,
+			89, 90, 91, 92, 92, 93, 94, 95,
+			96, 96, 97, 98, 98, 99, 99, 100,
+			101, 101, 102, 102, 103, 103, 104, 104,
+			105, 105, 106, 106, 107, 107, 108, 108,
+			108, 109, 109, 110, 110, 110, 111, 111,
+			112, 112, 112, 113, 113, 113, 114, 114,
+			114, 115, 115, 115, 115, 116, 116, 116,
+			117, 117, 117, 118, 118, 118, 118, 119,
+			119, 119, 119, 120, 120, 120, 120, 121,
+			121, 121, 121, 122, 122, 122, 122, 122,
+			123, 123, 123, 123, 124, 124, 124, 124,
+			124, 125, 125, 125, 125, 125, 126, 126,
+			126, 126, 126, 127, 127, 127, 127, 127,
+			128, 128, 128, 128, 128, 128, 129, 129,
+			129, 129, 129, 129, 130, 130, 130, 130,
+			130, 130, 131, 131, 131, 131, 131, 131,
+			131, 132, 132, 132, 132, 132, 132, 133,
+			133, 133, 133, 133, 133, 133, 134, 134,
+			134, 134, 134, 134, 134, 134, 135, 135,
+			135, 135, 135, 135, 135, 135, 136, 136,
+			136, 136, 136, 136, 136, 136, 137, 137,
+			137, 137, 137, 137, 137, 137, 138, 138,
+			138, 138, 138, 138, 138, 138, 138, 139,
+			139, 139, 139, 139, 139, 139, 139, 139,
+			140, 140, 140, 140, 140, 140, 140, 140,
+			140, 141, 141, 141, 141, 141, 141, 141,
+			141, 141, 141, 142, 142, 142, 142, 142,
+			142, 142, 142, 142, 142, 142, 143, 143,
+			143, 143, 143, 143, 143, 143, 143, 143,
+			144,
+		},
+		.len_sym_cost = 93,
+	}, { /* match_prob = 0.75 */
+		.used_lits_to_lit_cost = {
+			32, 32, 48, 57, 64, 69, 73, 76,
+			80, 82, 85, 87, 89, 91, 92, 94,
+			96, 97, 98, 99, 101, 102, 103, 104,
+			105, 106, 107, 108, 108, 109, 110, 111,
+			112, 112, 113, 114, 114, 115, 115, 116,
+			117, 117, 118, 118, 119, 119, 120, 120,
+			121, 121, 122, 122, 123, 123, 124, 124,
+			124, 125, 125, 126, 126, 126, 127, 127,
+			128, 128, 128, 129, 129, 129, 130, 130,
+			130, 131, 131, 131, 131, 132, 132, 132,
+			133, 133, 133, 134, 134, 134, 134, 135,
+			135, 135, 135, 136, 136, 136, 136, 137,
+			137, 137, 137, 138, 138, 138, 138, 138,
+			139, 139, 139, 139, 140, 140, 140, 140,
+			140, 141, 141, 141, 141, 141, 142, 142,
+			142, 142, 142, 143, 143, 143, 143, 143,
+			144, 144, 144, 144, 144, 144, 145, 145,
+			145, 145, 145, 145, 146, 146, 146, 146,
+			146, 146, 147, 147, 147, 147, 147, 147,
+			147, 148, 148, 148, 148, 148, 148, 149,
+			149, 149, 149, 149, 149, 149, 150, 150,
+			150, 150, 150, 150, 150, 150, 151, 151,
+			151, 151, 151, 151, 151, 151, 152, 152,
+			152, 152, 152, 152, 152, 152, 153, 153,
+			153, 153, 153, 153, 153, 153, 154, 154,
+			154, 154, 154, 154, 154, 154, 154, 155,
+			155, 155, 155, 155, 155, 155, 155, 155,
+			156, 156, 156, 156, 156, 156, 156, 156,
+			156, 157, 157, 157, 157, 157, 157, 157,
+			157, 157, 157, 158, 158, 158, 158, 158,
+			158, 158, 158, 158, 158, 158, 159, 159,
+			159, 159, 159, 159, 159, 159, 159, 159,
+			160,
+		},
+		.len_sym_cost = 84,
+	},
+};
+
+/*
+ * Choose the default costs for literal and length symbols.  These symbols are
+ * both part of the litlen alphabet.
+ */
+static void
+deflate_choose_default_litlen_costs(struct libdeflate_compressor *c,
+				    const u8 *block_begin, u32 block_length,
+				    u32 *lit_cost, u32 *len_sym_cost)
+{
+	unsigned num_used_literals = 0;
+	u32 literal_freq = block_length;
+	u32 match_freq = 0;
+	u32 cutoff;
+	u32 i;
+
+	/* Calculate the number of distinct literals that exist in the data. */
+	memset(c->freqs.litlen, 0,
+	       DEFLATE_NUM_LITERALS * sizeof(c->freqs.litlen[0]));
+	cutoff = literal_freq >> 11; /* Ignore literals used very rarely. */
+	for (i = 0; i < block_length; i++)
+		c->freqs.litlen[block_begin[i]]++;
+	for (i = 0; i < DEFLATE_NUM_LITERALS; i++) {
+		if (c->freqs.litlen[i] > cutoff)
+			num_used_literals++;
+	}
+	if (num_used_literals == 0)
+		num_used_literals = 1;
+
+	/*
+	 * Estimate the relative frequency of literals and matches in the
+	 * optimal parsing solution.  We don't know the optimal solution, so
+	 * this can only be a very rough estimate.  Therefore, we basically use
+	 * the match frequency from a greedy parse.  We also apply the min_len
+	 * heuristic used by the greedy and lazy parsers, to avoid counting too
+	 * many matches when literals are cheaper than short matches.
+	 */
+	match_freq = 0;
+	i = choose_min_match_len(num_used_literals, c->max_search_depth);
+	for (; i < ARRAY_LEN(c->p.n.match_len_freqs); i++) {
+		match_freq += c->p.n.match_len_freqs[i];
+		literal_freq -= i * c->p.n.match_len_freqs[i];
+	}
+	if ((s32)literal_freq < 0) /* shouldn't happen */
+		literal_freq = 0;
+
+	if (match_freq > literal_freq)
+		i = 2; /* many matches */
+	else if (match_freq * 4 > literal_freq)
+		i = 1; /* neutral */
+	else
+		i = 0; /* few matches */
+
+	STATIC_ASSERT(BIT_COST == 16);
+	*lit_cost = default_litlen_costs[i].used_lits_to_lit_cost[
+							num_used_literals];
+	*len_sym_cost = default_litlen_costs[i].len_sym_cost;
 }
 
 static forceinline u32
-deflate_default_length_slot_cost(unsigned length_slot)
+deflate_default_length_cost(unsigned len, u32 len_sym_cost)
 {
-	STATIC_ASSERT(COST_SHIFT == 3);
-	/* 60 is 7.5 bits/symbol  */
-	return 60 + ((u32)deflate_extra_length_bits[length_slot] << COST_SHIFT);
+	unsigned slot = deflate_length_slot[len];
+	u32 num_extra_bits = deflate_extra_length_bits[slot];
+
+	return len_sym_cost + (num_extra_bits * BIT_COST);
 }
 
 static forceinline u32
-deflate_default_offset_slot_cost(unsigned offset_slot)
+deflate_default_offset_slot_cost(unsigned slot)
 {
-	STATIC_ASSERT(COST_SHIFT == 3);
-	/* 39 is 4.875 bits/symbol  */
-	return 39 + ((u32)deflate_extra_offset_bits[offset_slot] << COST_SHIFT);
+	u32 num_extra_bits = deflate_extra_offset_bits[slot];
+	/*
+	 * Assume that all offset symbols are equally probable.
+	 * The resulting cost is 'int(-log2(1/30) * BIT_COST)',
+	 * where 30 is the number of potentially-used offset symbols.
+	 */
+	u32 offset_sym_cost = 4*BIT_COST + (907*BIT_COST)/1000;
+
+	return offset_sym_cost + (num_extra_bits * BIT_COST);
 }
 
-/*
- * Set default symbol costs for the first block's first optimization pass.
- *
- * It works well to assume that each symbol is equally probable.  This results
- * in each symbol being assigned a cost of (-log2(1.0/num_syms) * (1 <<
- * COST_SHIFT)) where 'num_syms' is the number of symbols in the corresponding
- * alphabet.  However, we intentionally bias the parse towards matches rather
- * than literals by using a slightly lower default cost for length symbols than
- * for literals.  This often improves the compression ratio slightly.
- */
+/* Set default symbol costs for the first block's first optimization pass. */
 static void
-deflate_set_default_costs(struct libdeflate_compressor *c)
+deflate_set_default_costs(struct libdeflate_compressor *c,
+			  u32 lit_cost, u32 len_sym_cost)
 {
 	unsigned i;
 
-	/* Literals  */
+	/* Literals */
 	for (i = 0; i < DEFLATE_NUM_LITERALS; i++)
-		c->p.n.costs.literal[i] = deflate_default_literal_cost(i);
+		c->p.n.costs.literal[i] = lit_cost;
 
-	/* Lengths  */
+	/* Lengths */
 	for (i = DEFLATE_MIN_MATCH_LEN; i <= DEFLATE_MAX_MATCH_LEN; i++)
-		c->p.n.costs.length[i] = deflate_default_length_slot_cost(
-						deflate_length_slot[i]);
+		c->p.n.costs.length[i] =
+			deflate_default_length_cost(i, len_sym_cost);
 
-	/* Offset slots  */
+	/* Offset slots */
 	for (i = 0; i < ARRAY_LEN(deflate_offset_slot_base); i++)
-		c->p.n.costs.offset_slot[i] = deflate_default_offset_slot_cost(i);
+		c->p.n.costs.offset_slot[i] =
+			deflate_default_offset_slot_cost(i);
 }
 
 static forceinline void
-deflate_adjust_cost(u32 *cost_p, u32 default_cost)
+deflate_adjust_cost(u32 *cost_p, u32 default_cost, int change_amount)
 {
-	*cost_p += ((s32)default_cost - (s32)*cost_p) >> 1;
+	if (change_amount == 0)
+		/* Block is very similar to previous; prefer previous costs. */
+		*cost_p = (default_cost + 3 * *cost_p) / 4;
+	else if (change_amount == 1)
+		*cost_p = (default_cost + *cost_p) / 2;
+	else if (change_amount == 2)
+		*cost_p = (5 * default_cost + 3 * *cost_p) / 8;
+	else
+		/* Block differs greatly from previous; prefer default costs. */
+		*cost_p = (3 * default_cost + *cost_p) / 4;
 }
 
-/*
- * Adjust the costs when beginning a new block.
- *
- * Since the current costs have been optimized for the data, it's undesirable to
- * throw them away and start over with the default costs.  At the same time, we
- * don't want to bias the parse by assuming that the next block will be similar
- * to the current block.  As a compromise, make the costs closer to the
- * defaults, but don't simply set them to the defaults.
- */
-static void
-deflate_adjust_costs(struct libdeflate_compressor *c)
+static forceinline void
+deflate_adjust_costs_impl(struct libdeflate_compressor *c,
+			  u32 lit_cost, u32 len_sym_cost, int change_amount)
 {
 	unsigned i;
 
-	/* Literals  */
+	/* Literals */
 	for (i = 0; i < DEFLATE_NUM_LITERALS; i++)
-		deflate_adjust_cost(&c->p.n.costs.literal[i],
-				    deflate_default_literal_cost(i));
+		deflate_adjust_cost(&c->p.n.costs.literal[i], lit_cost,
+				    change_amount);
 
-	/* Lengths  */
+	/* Lengths */
 	for (i = DEFLATE_MIN_MATCH_LEN; i <= DEFLATE_MAX_MATCH_LEN; i++)
 		deflate_adjust_cost(&c->p.n.costs.length[i],
-				    deflate_default_length_slot_cost(
-						deflate_length_slot[i]));
+				    deflate_default_length_cost(i,
+								len_sym_cost),
+				    change_amount);
 
-	/* Offset slots  */
+	/* Offset slots */
 	for (i = 0; i < ARRAY_LEN(deflate_offset_slot_base); i++)
 		deflate_adjust_cost(&c->p.n.costs.offset_slot[i],
-				    deflate_default_offset_slot_cost(i));
+				    deflate_default_offset_slot_cost(i),
+				    change_amount);
+}
+
+/*
+ * Adjust the costs when beginning a new block.
+ *
+ * Since the current costs are optimized for the data already, it can be helpful
+ * to reuse them instead of starting over with the default costs.  However, this
+ * depends on how similar the new block is to the previous block.  Therefore,
+ * use a heuristic to decide how similar the blocks are, and mix together the
+ * current costs and the default costs accordingly.
+ */
+static void
+deflate_adjust_costs(struct libdeflate_compressor *c,
+		     u32 lit_cost, u32 len_sym_cost)
+{
+	u64 total_delta = 0;
+	u64 cutoff;
+	int i;
+
+	/*
+	 * Decide how different the current block is from the previous block,
+	 * using the block splitting statistics from the current and previous
+	 * blocks.  The more different the current block is, the more we prefer
+	 * the default costs rather than the previous block's costs.
+	 *
+	 * The algorithm here is similar to the end-of-block check one, but here
+	 * we compare two entire blocks rather than a partial block with a small
+	 * extra part, and therefore we need 64-bit numbers in some places.
+	 */
+	for (i = 0; i < NUM_OBSERVATION_TYPES; i++) {
+		u64 prev = (u64)c->p.n.prev_observations[i] *
+			    c->split_stats.num_observations;
+		u64 cur = (u64)c->split_stats.observations[i] *
+			  c->p.n.prev_num_observations;
+
+		total_delta += prev > cur ? prev - cur : cur - prev;
+	}
+	cutoff = ((u64)c->p.n.prev_num_observations *
+		  c->split_stats.num_observations * 200) / 512;
+
+	if (total_delta > 3 * cutoff)
+		/* Big change in the data; just use the default costs. */
+		deflate_set_default_costs(c, lit_cost, len_sym_cost);
+	else if (4 * total_delta > 9 * cutoff)
+		deflate_adjust_costs_impl(c, lit_cost, len_sym_cost, 3);
+	else if (2 * total_delta > 3 * cutoff)
+		deflate_adjust_costs_impl(c, lit_cost, len_sym_cost, 2);
+	else if (2 * total_delta > cutoff)
+		deflate_adjust_costs_impl(c, lit_cost, len_sym_cost, 1);
+	else
+		deflate_adjust_costs_impl(c, lit_cost, len_sym_cost, 0);
+}
+
+static void
+deflate_set_initial_costs(struct libdeflate_compressor *c,
+			  const u8 *block_begin, u32 block_length,
+			  bool is_first_block)
+{
+	u32 lit_cost, len_sym_cost;
+
+	deflate_choose_default_litlen_costs(c, block_begin, block_length,
+					    &lit_cost, &len_sym_cost);
+	if (is_first_block)
+		deflate_set_default_costs(c, lit_cost, len_sym_cost);
+	else
+		deflate_adjust_costs(c, lit_cost, len_sym_cost);
 }
 
 /*
  * Find the minimum-cost path through the graph of possible match/literal
  * choices for this block.
  *
  * We find the minimum cost path from 'c->p.n.optimum_nodes[0]', which
@@ -2369,35 +3289,36 @@
  * saved.
  */
 static void
 deflate_find_min_cost_path(struct libdeflate_compressor *c,
 			   const u32 block_length,
 			   const struct lz_match *cache_ptr)
 {
-	struct deflate_optimum_node *end_node = &c->p.n.optimum_nodes[block_length];
+	struct deflate_optimum_node *end_node =
+		&c->p.n.optimum_nodes[block_length];
 	struct deflate_optimum_node *cur_node = end_node;
 
 	cur_node->cost_to_end = 0;
 	do {
 		unsigned num_matches;
 		unsigned literal;
 		u32 best_cost_to_end;
 
 		cur_node--;
 		cache_ptr--;
 
 		num_matches = cache_ptr->length;
 		literal = cache_ptr->offset;
 
-		/* It's always possible to choose a literal.  */
+		/* It's always possible to choose a literal. */
 		best_cost_to_end = c->p.n.costs.literal[literal] +
 				   (cur_node + 1)->cost_to_end;
 		cur_node->item = ((u32)literal << OPTIMUM_OFFSET_SHIFT) | 1;
 
-		/* Also consider matches if there are any.  */
+		/* Also consider matches if there are any. */
 		if (num_matches) {
 			const struct lz_match *match;
 			unsigned len;
 			unsigned offset;
 			unsigned offset_slot;
 			u32 offset_cost;
 			u32 cost_to_end;
@@ -2412,77 +3333,188 @@
 			 * offset costing less than a smaller offset to code,
 			 * this is a very useful heuristic.
 			 */
 			match = cache_ptr - num_matches;
 			len = DEFLATE_MIN_MATCH_LEN;
 			do {
 				offset = match->offset;
-				offset_slot = deflate_get_offset_slot(c, offset);
-				offset_cost = c->p.n.costs.offset_slot[offset_slot];
+				offset_slot = c->p.n.offset_slot_full[offset];
+				offset_cost =
+					c->p.n.costs.offset_slot[offset_slot];
 				do {
 					cost_to_end = offset_cost +
-						      c->p.n.costs.length[len] +
-						      (cur_node + len)->cost_to_end;
+						c->p.n.costs.length[len] +
+						(cur_node + len)->cost_to_end;
 					if (cost_to_end < best_cost_to_end) {
 						best_cost_to_end = cost_to_end;
-						cur_node->item = ((u32)offset << OPTIMUM_OFFSET_SHIFT) | len;
+						cur_node->item = len |
+							((u32)offset <<
+							 OPTIMUM_OFFSET_SHIFT);
 					}
 				} while (++len <= match->length);
 			} while (++match != cache_ptr);
 			cache_ptr -= num_matches;
 		}
 		cur_node->cost_to_end = best_cost_to_end;
 	} while (cur_node != &c->p.n.optimum_nodes[0]);
+
+	deflate_reset_symbol_frequencies(c);
+	deflate_tally_item_list(c, block_length);
+	deflate_make_huffman_codes(&c->freqs, &c->codes);
 }
 
 /*
- * Choose the literal/match sequence to use for the current block.  The basic
- * algorithm finds a minimum-cost path through the block's graph of
- * literal/match choices, given a cost model.  However, the cost of each symbol
- * is unknown until the Huffman codes have been built, but at the same time the
- * Huffman codes depend on the frequencies of chosen symbols.  Consequently,
- * multiple passes must be used to try to approximate an optimal solution.  The
- * first pass uses default costs, mixed with the costs from the previous block
- * if any.  Later passes use the Huffman codeword lengths from the previous pass
- * as the costs.
- */
-static void
-deflate_optimize_block(struct libdeflate_compressor *c, u32 block_length,
-		       const struct lz_match *cache_ptr, bool is_first_block)
-{
-	unsigned num_passes_remaining = c->p.n.num_optim_passes;
+ * Choose the literals and matches for the current block, then output the block.
+ *
+ * To choose the literal/match sequence, we find the minimum-cost path through
+ * the block's graph of literal/match choices, given a cost model.  However, the
+ * true cost of each symbol is unknown until the Huffman codes have been built,
+ * but at the same time the Huffman codes depend on the frequencies of chosen
+ * symbols.  Consequently, multiple passes must be used to try to approximate an
+ * optimal solution.  The first pass uses default costs, mixed with the costs
+ * from the previous block when it seems appropriate.  Later passes use the
+ * Huffman codeword lengths from the previous pass as the costs.
+ *
+ * As an alternate strategy, also consider using only literals.  The boolean
+ * returned in *used_only_literals indicates whether that strategy was best.
+ */
+static void
+deflate_optimize_and_flush_block(struct libdeflate_compressor *c,
+				 struct deflate_output_bitstream *os,
+				 const u8 *block_begin, u32 block_length,
+				 const struct lz_match *cache_ptr,
+				 bool is_first_block, bool is_final_block,
+				 bool *used_only_literals)
+{
+	unsigned num_passes_remaining = c->p.n.max_optim_passes;
+	u32 best_true_cost = UINT32_MAX;
+	u32 true_cost;
+	u32 only_lits_cost;
+	struct deflate_sequence seq_;
+	struct deflate_sequence *seq = NULL;
 	u32 i;
 
-	/* Force the block to really end at the desired length, even if some
-	 * matches extend beyond it. */
-	for (i = block_length; i <= MIN(block_length - 1 + DEFLATE_MAX_MATCH_LEN,
-					ARRAY_LEN(c->p.n.optimum_nodes) - 1); i++)
+	/*
+	 * On some data, using only literals (no matches) ends up being better
+	 * than what the iterative optimization algorithm produces.  Therefore,
+	 * consider using only literals.
+	 */
+	deflate_choose_all_literals(c, block_begin, block_length);
+	only_lits_cost = deflate_compute_true_cost(c);
+
+	/*
+	 * Force the block to really end at the desired length, even if some
+	 * matches extend beyond it.
+	 */
+	for (i = block_length;
+	     i <= MIN(block_length - 1 + DEFLATE_MAX_MATCH_LEN,
+		      ARRAY_LEN(c->p.n.optimum_nodes) - 1); i++)
 		c->p.n.optimum_nodes[i].cost_to_end = 0x80000000;
 
-	/* Set the initial costs. */
-	if (is_first_block)
-		deflate_set_default_costs(c);
-	else
-		deflate_adjust_costs(c);
+	/* Initialize c->p.n.costs with default costs. */
+	deflate_set_initial_costs(c, block_begin, block_length, is_first_block);
 
-	for (;;) {
-		/* Find the minimum cost path for this pass. */
+	do {
+		/*
+		 * Find the minimum-cost path for this pass.
+		 * Also set c->freqs and c->codes to match the path.
+		 */
 		deflate_find_min_cost_path(c, block_length, cache_ptr);
 
-		/* Compute frequencies of the chosen symbols. */
-		deflate_reset_symbol_frequencies(c);
-		deflate_tally_item_list(c, block_length);
+		/*
+		 * Compute the exact cost of the block if the path were to be
+		 * used.  Note that this differs from
+		 * c->p.n.optimum_nodes[0].cost_to_end in that true_cost uses
+		 * the actual Huffman codes instead of c->p.n.costs.
+		 */
+		true_cost = deflate_compute_true_cost(c);
 
-		if (--num_passes_remaining == 0)
+		/*
+		 * If the cost didn't improve much from the previous pass, then
+		 * doing more passes probably won't be helpful, so stop early.
+		 */
+		if (true_cost + c->p.n.min_improvement_to_continue >
+		    best_true_cost)
 			break;
 
-		/* At least one optimization pass remains; update the costs. */
-		deflate_make_huffman_codes(&c->freqs, &c->codes);
+		best_true_cost = true_cost;
+		c->p.n.costs_producing_best_true_cost = c->p.n.costs;
+
+		/* Update the cost model from the Huffman codes. */
+		deflate_set_costs_from_codes(c, &c->codes.lens);
+
+	} while (--num_passes_remaining);
+
+	*used_only_literals = false;
+	if (only_lits_cost < best_true_cost) {
+		/* Using only literals ended up being best! */
+		deflate_choose_all_literals(c, block_begin, block_length);
+		deflate_set_costs_from_codes(c, &c->codes.lens);
+		seq_.litrunlen_and_length = block_length;
+		seq = &seq_;
+		*used_only_literals = true;
+	} else if (true_cost >=
+		   best_true_cost + c->p.n.min_bits_to_use_nonfinal_path) {
+		/*
+		 * The best solution was actually from a non-final optimization
+		 * pass, so recover and use the min-cost path from that pass.
+		 */
+		c->p.n.costs = c->p.n.costs_producing_best_true_cost;
+		deflate_find_min_cost_path(c, block_length, cache_ptr);
 		deflate_set_costs_from_codes(c, &c->codes.lens);
 	}
+	deflate_flush_block(c, os, block_begin, block_length, seq,
+			    is_final_block);
+}
+
+static void
+deflate_near_optimal_init_stats(struct libdeflate_compressor *c)
+{
+	init_block_split_stats(&c->split_stats);
+	memset(c->p.n.new_match_len_freqs, 0,
+	       sizeof(c->p.n.new_match_len_freqs));
+	memset(c->p.n.match_len_freqs, 0, sizeof(c->p.n.match_len_freqs));
+}
+
+static void
+deflate_near_optimal_merge_stats(struct libdeflate_compressor *c)
+{
+	unsigned i;
+
+	merge_new_observations(&c->split_stats);
+	for (i = 0; i < ARRAY_LEN(c->p.n.match_len_freqs); i++) {
+		c->p.n.match_len_freqs[i] += c->p.n.new_match_len_freqs[i];
+		c->p.n.new_match_len_freqs[i] = 0;
+	}
+}
+
+/*
+ * Save some literal/match statistics from the previous block so that
+ * deflate_adjust_costs() will be able to decide how much the current block
+ * differs from the previous one.
+ */
+static void
+deflate_near_optimal_save_stats(struct libdeflate_compressor *c)
+{
+	int i;
+
+	for (i = 0; i < NUM_OBSERVATION_TYPES; i++)
+		c->p.n.prev_observations[i] = c->split_stats.observations[i];
+	c->p.n.prev_num_observations = c->split_stats.num_observations;
+}
+
+static void
+deflate_near_optimal_clear_old_stats(struct libdeflate_compressor *c)
+{
+	int i;
+
+	for (i = 0; i < NUM_OBSERVATION_TYPES; i++)
+		c->split_stats.observations[i] = 0;
+	c->split_stats.num_observations = 0;
+	memset(c->p.n.match_len_freqs, 0, sizeof(c->p.n.match_len_freqs));
 }
 
 /*
  * This is the "near-optimal" DEFLATE compressor.  It computes the optimal
  * representation of each DEFLATE block using a minimum-cost path search over
  * the graph of possible match/literal choices for that block, assuming a
  * certain cost for each Huffman symbol.
@@ -2490,73 +3522,86 @@
  * For several reasons, the end result is not guaranteed to be optimal:
  *
  * - Nonoptimal choice of blocks
  * - Heuristic limitations on which matches are actually considered
  * - Symbol costs are unknown until the symbols have already been chosen
  *   (so iterative optimization must be used)
  */
-static size_t
+static void
 deflate_compress_near_optimal(struct libdeflate_compressor * restrict c,
-			      const u8 * restrict in, size_t in_nbytes,
-			      u8 * restrict out, size_t out_nbytes_avail)
+			      const u8 *in, size_t in_nbytes,
+			      struct deflate_output_bitstream *os)
 {
 	const u8 *in_next = in;
+	const u8 *in_block_begin = in_next;
 	const u8 *in_end = in_next + in_nbytes;
-	struct deflate_output_bitstream os;
 	const u8 *in_cur_base = in_next;
-	const u8 *in_next_slide = in_next + MIN(in_end - in_next, MATCHFINDER_WINDOW_SIZE);
+	const u8 *in_next_slide =
+		in_next + MIN(in_end - in_next, MATCHFINDER_WINDOW_SIZE);
 	unsigned max_len = DEFLATE_MAX_MATCH_LEN;
 	unsigned nice_len = MIN(c->nice_match_length, max_len);
+	struct lz_match *cache_ptr = c->p.n.match_cache;
 	u32 next_hashes[2] = {0, 0};
+	bool prev_block_used_only_literals = false;
 
-	deflate_init_output(&os, out, out_nbytes_avail);
 	bt_matchfinder_init(&c->p.n.bt_mf);
+	deflate_near_optimal_init_stats(c);
 
 	do {
-		/* Starting a new DEFLATE block.  */
-
-		struct lz_match *cache_ptr = c->p.n.match_cache;
-		const u8 * const in_block_begin = in_next;
-		const u8 * const in_max_block_end =
-			in_next + MIN(in_end - in_next, SOFT_MAX_BLOCK_LENGTH);
+		/* Starting a new DEFLATE block */
+		const u8 * const in_max_block_end = choose_max_block_end(
+				in_block_begin, in_end, SOFT_MAX_BLOCK_LENGTH);
+		const u8 *prev_end_block_check = NULL;
+		bool change_detected = false;
 		const u8 *next_observation = in_next;
+		unsigned min_len;
 
-		init_block_split_stats(&c->split_stats);
+		/*
+		 * Use the minimum match length heuristic to improve the
+		 * literal/match statistics gathered during matchfinding.
+		 * However, the actual near-optimal parse won't respect min_len,
+		 * as it can accurately assess the costs of different matches.
+		 *
+		 * If the "use only literals" strategy happened to be the best
+		 * strategy on the previous block, then probably the
+		 * min_match_len heuristic is still not aggressive enough for
+		 * the data, so force gathering literal stats only.
+		 */
+		if (prev_block_used_only_literals)
+			min_len = DEFLATE_MAX_MATCH_LEN + 1;
+		else
+			min_len = calculate_min_match_len(
+					in_block_begin,
+					in_max_block_end - in_block_begin,
+					c->max_search_depth);
 
 		/*
 		 * Find matches until we decide to end the block.  We end the
 		 * block if any of the following is true:
 		 *
 		 * (1) Maximum block length has been reached
 		 * (2) Match catch may overflow.
 		 * (3) Block split heuristic says to split now.
 		 */
-		do {
+		for (;;) {
 			struct lz_match *matches;
 			unsigned best_len;
+			size_t remaining = in_end - in_next;
 
-			/* Slide the window forward if needed.  */
+			/* Slide the window forward if needed. */
 			if (in_next == in_next_slide) {
 				bt_matchfinder_slide_window(&c->p.n.bt_mf);
 				in_cur_base = in_next;
-				in_next_slide = in_next + MIN(in_end - in_next,
-							      MATCHFINDER_WINDOW_SIZE);
-			}
-
-			/* Decrease the maximum and nice match lengths if we're
-			 * approaching the end of the input buffer.  */
-			if (unlikely(max_len > in_end - in_next)) {
-				max_len = in_end - in_next;
-				nice_len = MIN(nice_len, max_len);
+				in_next_slide = in_next +
+					MIN(remaining, MATCHFINDER_WINDOW_SIZE);
 			}
 
 			/*
 			 * Find matches with the current position using the
-			 * binary tree matchfinder and save them in
-			 * 'match_cache'.
+			 * binary tree matchfinder and save them in match_cache.
 			 *
 			 * Note: the binary tree matchfinder is more suited for
 			 * optimal parsing than the hash chain matchfinder.  The
 			 * reasons for this include:
 			 *
 			 * - The binary tree matchfinder can find more matches
 			 *   in the same number of steps.
@@ -2564,32 +3609,37 @@
 			 *   skipping positions (not searching for matches at
 			 *   them) is faster; however, with optimal parsing we
 			 *   search for matches at almost all positions, so this
 			 *   advantage of hash chains is negated.
 			 */
 			matches = cache_ptr;
 			best_len = 0;
+			adjust_max_and_nice_len(&max_len, &nice_len, remaining);
 			if (likely(max_len >= BT_MATCHFINDER_REQUIRED_NBYTES)) {
-				cache_ptr = bt_matchfinder_get_matches(&c->p.n.bt_mf,
-								       in_cur_base,
-								       in_next - in_cur_base,
-								       max_len,
-								       nice_len,
-								       c->max_search_depth,
-								       next_hashes,
-								       &best_len,
-								       matches);
+				cache_ptr = bt_matchfinder_get_matches(
+						&c->p.n.bt_mf,
+						in_cur_base,
+						in_next - in_cur_base,
+						max_len,
+						nice_len,
+						c->max_search_depth,
+						next_hashes,
+						matches);
+				if (cache_ptr > matches)
+					best_len = cache_ptr[-1].length;
 			}
-
 			if (in_next >= next_observation) {
-				if (best_len >= 4) {
-					observe_match(&c->split_stats, best_len);
+				if (best_len >= min_len) {
+					observe_match(&c->split_stats,
+						      best_len);
 					next_observation = in_next + best_len;
+					c->p.n.new_match_len_freqs[best_len]++;
 				} else {
-					observe_literal(&c->split_stats, *in_next);
+					observe_literal(&c->split_stats,
+							*in_next);
 					next_observation = in_next + 1;
 				}
 			}
 
 			cache_ptr->length = cache_ptr - matches;
 			cache_ptr->offset = *in_next;
 			in_next++;
@@ -2603,252 +3653,396 @@
 			 * very large.
 			 *
 			 * This heuristic doesn't actually hurt the compression
 			 * ratio very much.  If there's a long match, then the
 			 * data must be highly compressible, so it doesn't
 			 * matter much what we do.
 			 */
-			if (best_len >= DEFLATE_MIN_MATCH_LEN && best_len >= nice_len) {
+			if (best_len >= DEFLATE_MIN_MATCH_LEN &&
+			    best_len >= nice_len) {
 				--best_len;
 				do {
+					remaining = in_end - in_next;
 					if (in_next == in_next_slide) {
-						bt_matchfinder_slide_window(&c->p.n.bt_mf);
+						bt_matchfinder_slide_window(
+							&c->p.n.bt_mf);
 						in_cur_base = in_next;
-						in_next_slide = in_next + MIN(in_end - in_next,
-									      MATCHFINDER_WINDOW_SIZE);
-					}
-					if (unlikely(max_len > in_end - in_next)) {
-						max_len = in_end - in_next;
-						nice_len = MIN(nice_len, max_len);
+						in_next_slide = in_next +
+							MIN(remaining,
+							    MATCHFINDER_WINDOW_SIZE);
 					}
-					if (max_len >= BT_MATCHFINDER_REQUIRED_NBYTES) {
-						bt_matchfinder_skip_position(&c->p.n.bt_mf,
-									     in_cur_base,
-									     in_next - in_cur_base,
-									     nice_len,
-									     c->max_search_depth,
-									     next_hashes);
+					adjust_max_and_nice_len(&max_len,
+								&nice_len,
+								remaining);
+					if (max_len >=
+					    BT_MATCHFINDER_REQUIRED_NBYTES) {
+						bt_matchfinder_skip_byte(
+							&c->p.n.bt_mf,
+							in_cur_base,
+							in_next - in_cur_base,
+							nice_len,
+							c->max_search_depth,
+							next_hashes);
 					}
 					cache_ptr->length = 0;
 					cache_ptr->offset = *in_next;
 					in_next++;
 					cache_ptr++;
 				} while (--best_len);
 			}
-		} while (in_next < in_max_block_end &&
-			 cache_ptr < &c->p.n.match_cache[CACHE_LENGTH] &&
-			 !should_end_block(&c->split_stats, in_block_begin, in_next, in_end));
+			/* Maximum block length or end of input reached? */
+			if (in_next >= in_max_block_end)
+				break;
+			/* Match cache overflowed? */
+			if (cache_ptr >=
+			    &c->p.n.match_cache[MATCH_CACHE_LENGTH])
+				break;
+			/* Not ready to try to end the block (again)? */
+			if (!ready_to_check_block(&c->split_stats,
+						  in_block_begin, in_next,
+						  in_end))
+				continue;
+			/* Check if it would be worthwhile to end the block. */
+			if (do_end_block_check(&c->split_stats,
+					       in_next - in_block_begin)) {
+				change_detected = true;
+				break;
+			}
+			/* Ending the block doesn't seem worthwhile here. */
+			deflate_near_optimal_merge_stats(c);
+			prev_end_block_check = in_next;
+		}
+		/*
+		 * All the matches for this block have been cached.  Now choose
+		 * the precise end of the block and the sequence of items to
+		 * output to represent it, then flush the block.
+		 */
+		if (change_detected && prev_end_block_check != NULL) {
+			/*
+			 * The block is being ended because a recent chunk of
+			 * data differs from the rest of the block.  We could
+			 * end the block at 'in_next' like the greedy and lazy
+			 * compressors do, but that's not ideal since it would
+			 * include the differing chunk in the block.  The
+			 * near-optimal compressor has time to do a better job.
+			 * Therefore, we rewind to just before the chunk, and
+			 * output a block that only goes up to there.
+			 *
+			 * We then set things up to correctly start the next
+			 * block, considering that some work has already been
+			 * done on it (some matches found and stats gathered).
+			 */
+			struct lz_match *orig_cache_ptr = cache_ptr;
+			const u8 *in_block_end = prev_end_block_check;
+			u32 block_length = in_block_end - in_block_begin;
+			bool is_first = (in_block_begin == in);
+			bool is_final = false;
+			u32 num_bytes_to_rewind = in_next - in_block_end;
+			size_t cache_len_rewound;
 
-		/* All the matches for this block have been cached.  Now choose
-		 * the sequence of items to output and flush the block.  */
-		deflate_optimize_block(c, in_next - in_block_begin, cache_ptr,
-				       in_block_begin == in);
-		deflate_flush_block(c, &os, in_block_begin, in_next - in_block_begin,
-				    in_next == in_end, true);
+			/* Rewind the match cache. */
+			do {
+				cache_ptr--;
+				cache_ptr -= cache_ptr->length;
+			} while (--num_bytes_to_rewind);
+			cache_len_rewound = orig_cache_ptr - cache_ptr;
+
+			deflate_optimize_and_flush_block(
+						c, os, in_block_begin,
+						block_length, cache_ptr,
+						is_first, is_final,
+						&prev_block_used_only_literals);
+			memmove(c->p.n.match_cache, cache_ptr,
+				cache_len_rewound * sizeof(*cache_ptr));
+			cache_ptr = &c->p.n.match_cache[cache_len_rewound];
+			deflate_near_optimal_save_stats(c);
+			/*
+			 * Clear the stats for the just-flushed block, leaving
+			 * just the stats for the beginning of the next block.
+			 */
+			deflate_near_optimal_clear_old_stats(c);
+			in_block_begin = in_block_end;
+		} else {
+			/*
+			 * The block is being ended for a reason other than a
+			 * differing data chunk being detected.  Don't rewind at
+			 * all; just end the block at the current position.
+			 */
+			u32 block_length = in_next - in_block_begin;
+			bool is_first = (in_block_begin == in);
+			bool is_final = (in_next == in_end);
+
+			deflate_near_optimal_merge_stats(c);
+			deflate_optimize_and_flush_block(
+						c, os, in_block_begin,
+						block_length, cache_ptr,
+						is_first, is_final,
+						&prev_block_used_only_literals);
+			cache_ptr = &c->p.n.match_cache[0];
+			deflate_near_optimal_save_stats(c);
+			deflate_near_optimal_init_stats(c);
+			in_block_begin = in_next;
+		}
 	} while (in_next != in_end);
-
-	return deflate_flush_output(&os);
 }
 
-#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
-
-/* Initialize c->offset_slot_fast.  */
+/* Initialize c->p.n.offset_slot_full. */
 static void
-deflate_init_offset_slot_fast(struct libdeflate_compressor *c)
+deflate_init_offset_slot_full(struct libdeflate_compressor *c)
 {
 	unsigned offset_slot;
 	unsigned offset;
 	unsigned offset_end;
 
-	for (offset_slot = 0;
-	     offset_slot < ARRAY_LEN(deflate_offset_slot_base);
-	     offset_slot++)
-	{
+	for (offset_slot = 0; offset_slot < ARRAY_LEN(deflate_offset_slot_base);
+	     offset_slot++) {
 		offset = deflate_offset_slot_base[offset_slot];
-	#if USE_FULL_OFFSET_SLOT_FAST
-		offset_end = offset + (1 << deflate_extra_offset_bits[offset_slot]);
+		offset_end = offset +
+			     (1 << deflate_extra_offset_bits[offset_slot]);
 		do {
-			c->offset_slot_fast[offset] = offset_slot;
+			c->p.n.offset_slot_full[offset] = offset_slot;
 		} while (++offset != offset_end);
-	#else
-		if (offset <= 256) {
-			offset_end = offset + (1 << deflate_extra_offset_bits[offset_slot]);
-			do {
-				c->offset_slot_fast[offset - 1] = offset_slot;
-			} while (++offset != offset_end);
-		} else {
-			offset_end = offset + (1 << deflate_extra_offset_bits[offset_slot]);
-			do {
-				c->offset_slot_fast[256 + ((offset - 1) >> 7)] = offset_slot;
-			} while ((offset += (1 << 7)) != offset_end);
-		}
-	#endif
 	}
 }
 
-LIBDEFLATEEXPORT struct libdeflate_compressor * LIBDEFLATEAPI
+#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
+
+LIBDEFLATEAPI struct libdeflate_compressor *
 libdeflate_alloc_compressor(int compression_level)
 {
 	struct libdeflate_compressor *c;
 	size_t size = offsetof(struct libdeflate_compressor, p);
 
+	check_buildtime_parameters();
+
 	if (compression_level < 0 || compression_level > 12)
 		return NULL;
 
 #if SUPPORT_NEAR_OPTIMAL_PARSING
-	if (compression_level >= 8)
+	if (compression_level >= 10)
 		size += sizeof(c->p.n);
-	else if (compression_level >= 1)
-		size += sizeof(c->p.g);
-#else
-	if (compression_level >= 1)
-		size += sizeof(c->p.g);
+	else
 #endif
+	{
+		if (compression_level >= 2)
+			size += sizeof(c->p.g);
+		else if (compression_level == 1)
+			size += sizeof(c->p.f);
+	}
 
 	c = libdeflate_aligned_malloc(MATCHFINDER_MEM_ALIGNMENT, size);
 	if (!c)
 		return NULL;
 
 	c->compression_level = compression_level;
 
 	/*
 	 * The higher the compression level, the more we should bother trying to
 	 * compress very small inputs.
 	 */
-	c->min_size_to_compress = 56 - (compression_level * 4);
+	c->max_passthrough_size = 55 - (compression_level * 4);
 
 	switch (compression_level) {
 	case 0:
-		c->impl = deflate_compress_none;
+		c->max_passthrough_size = SIZE_MAX;
+		c->impl = NULL; /* not used */
 		break;
 	case 1:
-		c->impl = deflate_compress_greedy;
-		c->max_search_depth = 2;
-		c->nice_match_length = 8;
+		c->impl = deflate_compress_fastest;
+		/* max_search_depth is unused. */
+		c->nice_match_length = 32;
 		break;
 	case 2:
 		c->impl = deflate_compress_greedy;
 		c->max_search_depth = 6;
 		c->nice_match_length = 10;
 		break;
 	case 3:
 		c->impl = deflate_compress_greedy;
 		c->max_search_depth = 12;
 		c->nice_match_length = 14;
 		break;
 	case 4:
 		c->impl = deflate_compress_greedy;
-		c->max_search_depth = 24;
-		c->nice_match_length = 24;
+		c->max_search_depth = 16;
+		c->nice_match_length = 30;
 		break;
 	case 5:
 		c->impl = deflate_compress_lazy;
-		c->max_search_depth = 20;
+		c->max_search_depth = 16;
 		c->nice_match_length = 30;
 		break;
 	case 6:
 		c->impl = deflate_compress_lazy;
-		c->max_search_depth = 40;
+		c->max_search_depth = 35;
 		c->nice_match_length = 65;
 		break;
 	case 7:
 		c->impl = deflate_compress_lazy;
 		c->max_search_depth = 100;
 		c->nice_match_length = 130;
 		break;
-#if SUPPORT_NEAR_OPTIMAL_PARSING
 	case 8:
-		c->impl = deflate_compress_near_optimal;
-		c->max_search_depth = 12;
-		c->nice_match_length = 20;
-		c->p.n.num_optim_passes = 1;
+		c->impl = deflate_compress_lazy2;
+		c->max_search_depth = 300;
+		c->nice_match_length = DEFLATE_MAX_MATCH_LEN;
 		break;
 	case 9:
-		c->impl = deflate_compress_near_optimal;
-		c->max_search_depth = 16;
-		c->nice_match_length = 26;
-		c->p.n.num_optim_passes = 2;
+#if !SUPPORT_NEAR_OPTIMAL_PARSING
+	default:
+#endif
+		c->impl = deflate_compress_lazy2;
+		c->max_search_depth = 600;
+		c->nice_match_length = DEFLATE_MAX_MATCH_LEN;
 		break;
+#if SUPPORT_NEAR_OPTIMAL_PARSING
 	case 10:
 		c->impl = deflate_compress_near_optimal;
-		c->max_search_depth = 30;
-		c->nice_match_length = 50;
-		c->p.n.num_optim_passes = 2;
+		c->max_search_depth = 35;
+		c->nice_match_length = 75;
+		c->p.n.max_optim_passes = 2;
+		c->p.n.min_improvement_to_continue = 32;
+		c->p.n.min_bits_to_use_nonfinal_path = 32;
+		deflate_init_offset_slot_full(c);
 		break;
 	case 11:
 		c->impl = deflate_compress_near_optimal;
-		c->max_search_depth = 60;
-		c->nice_match_length = 80;
-		c->p.n.num_optim_passes = 3;
-		break;
-	default:
-		c->impl = deflate_compress_near_optimal;
 		c->max_search_depth = 100;
-		c->nice_match_length = 133;
-		c->p.n.num_optim_passes = 4;
-		break;
-#else
-	case 8:
-		c->impl = deflate_compress_lazy;
-		c->max_search_depth = 150;
-		c->nice_match_length = 200;
+		c->nice_match_length = 150;
+		c->p.n.max_optim_passes = 4;
+		c->p.n.min_improvement_to_continue = 16;
+		c->p.n.min_bits_to_use_nonfinal_path = 16;
+		deflate_init_offset_slot_full(c);
 		break;
+	case 12:
 	default:
-		c->impl = deflate_compress_lazy;
-		c->max_search_depth = 200;
+		c->impl = deflate_compress_near_optimal;
+		c->max_search_depth = 300;
 		c->nice_match_length = DEFLATE_MAX_MATCH_LEN;
+		c->p.n.max_optim_passes = 10;
+		c->p.n.min_improvement_to_continue = 1;
+		c->p.n.min_bits_to_use_nonfinal_path = 1;
+		deflate_init_offset_slot_full(c);
 		break;
-#endif
+#endif /* SUPPORT_NEAR_OPTIMAL_PARSING */
 	}
 
-	deflate_init_offset_slot_fast(c);
 	deflate_init_static_codes(c);
 
 	return c;
 }
 
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_deflate_compress(struct libdeflate_compressor *c,
 			    const void *in, size_t in_nbytes,
 			    void *out, size_t out_nbytes_avail)
 {
-	if (unlikely(out_nbytes_avail < OUTPUT_END_PADDING))
-		return 0;
+	struct deflate_output_bitstream os;
 
-	/* For extremely small inputs just use a single uncompressed block. */
-	if (unlikely(in_nbytes < c->min_size_to_compress)) {
-		struct deflate_output_bitstream os;
-		deflate_init_output(&os, out, out_nbytes_avail);
-		if (in_nbytes == 0)
-			in = &os; /* Avoid passing NULL to memcpy() */
-		deflate_write_uncompressed_block(&os, in, in_nbytes, true);
-		return deflate_flush_output(&os);
-	}
+	/*
+	 * For extremely short inputs, or for compression level 0, just output
+	 * uncompressed blocks.
+	 */
+	if (unlikely(in_nbytes <= c->max_passthrough_size))
+		return deflate_compress_none(in, in_nbytes,
+					     out, out_nbytes_avail);
 
-	return (*c->impl)(c, in, in_nbytes, out, out_nbytes_avail);
+	/*
+	 * Initialize the output bitstream structure.
+	 *
+	 * The end is set to OUTPUT_END_PADDING below the true end, so that
+	 * FLUSH_BITS() can be more efficient.
+	 */
+	if (unlikely(out_nbytes_avail <= OUTPUT_END_PADDING))
+		return 0;
+	os.bitbuf = 0;
+	os.bitcount = 0;
+	os.next = out;
+	os.end = os.next + out_nbytes_avail - OUTPUT_END_PADDING;
+	(*c->impl)(c, in, in_nbytes, &os);
+	/*
+	 * If 'os.next' reached 'os.end', then either there was not enough space
+	 * in the output buffer, or the compressed size would have been within
+	 * OUTPUT_END_PADDING of the true end.  For performance reasons we don't
+	 * distinguish between these cases; we just make sure to return some
+	 * extra space from libdeflate_deflate_compress_bound().
+	 */
+	if (os.next >= os.end)
+		return 0;
+	ASSERT(os.bitcount <= 7);
+	if (os.bitcount)
+		*os.next++ = os.bitbuf;
+	return os.next - (u8 *)out;
 }
 
-LIBDEFLATEEXPORT void LIBDEFLATEAPI
+LIBDEFLATEAPI void
 libdeflate_free_compressor(struct libdeflate_compressor *c)
 {
 	libdeflate_aligned_free(c);
 }
 
 unsigned int
-deflate_get_compression_level(struct libdeflate_compressor *c)
+libdeflate_get_compression_level(struct libdeflate_compressor *c)
 {
 	return c->compression_level;
 }
 
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_deflate_compress_bound(struct libdeflate_compressor *c,
 				  size_t in_nbytes)
 {
+	size_t bound = 0;
+	size_t max_blocks;
+
 	/*
-	 * The worst case is all uncompressed blocks where one block has length
-	 * <= MIN_BLOCK_LENGTH and the others have length MIN_BLOCK_LENGTH.
-	 * Each uncompressed block has 5 bytes of overhead: 1 for BFINAL, BTYPE,
-	 * and alignment to a byte boundary; 2 for LEN; and 2 for NLEN.
+	 * Since the compressor never uses a compressed block when an
+	 * uncompressed block is cheaper, the worst case can be no worse than
+	 * the case where only uncompressed blocks are used.
+	 *
+	 * This is true even though up to 7 bits are "wasted" to byte-align the
+	 * bitstream when a compressed block is followed by an uncompressed
+	 * block.  This is because a compressed block wouldn't have been used if
+	 * it wasn't cheaper than an uncompressed block, and uncompressed blocks
+	 * always end on a byte boundary.  So the alignment bits will, at worst,
+	 * go up to the place where the uncompressed block would have ended.
 	 */
-	size_t max_num_blocks = MAX(DIV_ROUND_UP(in_nbytes, MIN_BLOCK_LENGTH), 1);
-	return (5 * max_num_blocks) + in_nbytes + 1 + OUTPUT_END_PADDING;
+
+	/*
+	 * The minimum length that is passed to deflate_flush_block() is
+	 * MIN_BLOCK_LENGTH bytes, except for the final block if needed.
+	 *
+	 * If deflate_flush_block() decides to use an uncompressed block, it
+	 * actually will (in general) output a series of uncompressed blocks in
+	 * order to stay within the UINT16_MAX limit of DEFLATE.  But this can
+	 * be disregarded here as long as '2 * MIN_BLOCK_LENGTH <= UINT16_MAX',
+	 * as in that case this behavior can't result in more blocks than the
+	 * case where deflate_flush_block() is called with min-length inputs.
+	 *
+	 * So the number of uncompressed blocks needed would be bounded by
+	 * DIV_ROUND_UP(in_nbytes, MIN_BLOCK_LENGTH).  However, empty inputs
+	 * need 1 (empty) block, which gives the final expression below.
+	 */
+	STATIC_ASSERT(2 * MIN_BLOCK_LENGTH <= UINT16_MAX);
+	max_blocks = MAX(DIV_ROUND_UP(in_nbytes, MIN_BLOCK_LENGTH), 1);
+
+	/*
+	 * Each uncompressed block has 5 bytes of overhead, for the BFINAL,
+	 * BTYPE, LEN, and NLEN fields.  (For the reason explained earlier, the
+	 * alignment bits at the very start of the block can be disregarded;
+	 * they would otherwise increase the overhead to 6 bytes per block.)
+	 */
+	bound += 5 * max_blocks;
+
+	/* Account for the data itself, stored uncompressed. */
+	bound += in_nbytes;
+
+	/*
+	 * Add 1 + OUTPUT_END_PADDING because for performance reasons, the
+	 * compressor doesn't distinguish between cases where there wasn't
+	 * enough space and cases where the compressed size would have been
+	 * 'out_nbytes_avail - OUTPUT_END_PADDING' or greater.  Adding
+	 * 1 + OUTPUT_END_PADDING to the bound ensures the needed wiggle room.
+	 */
+	bound += 1 + OUTPUT_END_PADDING;
+
+	return bound;
 }
```

### Comparing `deflate-0.3.0/libdeflate/lib/deflate_constants.h` & `deflate-0.4.0/libdeflate/lib/deflate_constants.h`

 * *Files 18% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 #define DEFLATE_BLOCKTYPE_STATIC_HUFFMAN	1
 #define DEFLATE_BLOCKTYPE_DYNAMIC_HUFFMAN	2
 
 /* Minimum and maximum supported match lengths (in bytes)  */
 #define DEFLATE_MIN_MATCH_LEN			3
 #define DEFLATE_MAX_MATCH_LEN			258
 
-/* Minimum and maximum supported match offsets (in bytes)  */
-#define DEFLATE_MIN_MATCH_OFFSET		1
+/* Maximum supported match offset (in bytes) */
 #define DEFLATE_MAX_MATCH_OFFSET		32768
 
-#define DEFLATE_MAX_WINDOW_SIZE			32768
+/* log2 of DEFLATE_MAX_MATCH_OFFSET */
+#define DEFLATE_WINDOW_ORDER			15
 
 /* Number of symbols in each Huffman code.  Note: for the literal/length
  * and offset codes, these are actually the maximum values; a given block
  * might use fewer symbols.  */
 #define DEFLATE_NUM_PRECODE_SYMS		19
 #define DEFLATE_NUM_LITLEN_SYMS			288
 #define DEFLATE_NUM_OFFSET_SYMS			32
 
 /* The maximum number of symbols across all codes  */
 #define DEFLATE_MAX_NUM_SYMS			288
 
 /* Division of symbols in the literal/length code  */
 #define DEFLATE_NUM_LITERALS			256
 #define DEFLATE_END_OF_BLOCK			256
-#define DEFLATE_NUM_LEN_SYMS			31
+#define DEFLATE_FIRST_LEN_SYM			257
 
 /* Maximum codeword length, in bits, within each Huffman code  */
 #define DEFLATE_MAX_PRE_CODEWORD_LEN		7
 #define DEFLATE_MAX_LITLEN_CODEWORD_LEN		15
 #define DEFLATE_MAX_OFFSET_CODEWORD_LEN		15
 
 /* The maximum codeword length across all codes  */
@@ -45,22 +45,12 @@
 
 /* Maximum possible overrun when decoding codeword lengths  */
 #define DEFLATE_MAX_LENS_OVERRUN		137
 
 /*
  * Maximum number of extra bits that may be required to represent a match
  * length or offset.
- *
- * TODO: are we going to have full DEFLATE64 support?  If so, up to 16
- * length bits must be supported.
  */
 #define DEFLATE_MAX_EXTRA_LENGTH_BITS		5
-#define DEFLATE_MAX_EXTRA_OFFSET_BITS		14
-
-/* The maximum number of bits in which a match can be represented.  This
- * is the absolute worst case, which assumes the longest possible Huffman
- * codewords and the maximum numbers of extra bits.  */
-#define DEFLATE_MAX_MATCH_BITS	\
-	(DEFLATE_MAX_LITLEN_CODEWORD_LEN + DEFLATE_MAX_EXTRA_LENGTH_BITS + \
-	DEFLATE_MAX_OFFSET_CODEWORD_LEN + DEFLATE_MAX_EXTRA_OFFSET_BITS)
+#define DEFLATE_MAX_EXTRA_OFFSET_BITS		13
 
 #endif /* LIB_DEFLATE_CONSTANTS_H */
```

### Comparing `deflate-0.3.0/libdeflate/lib/deflate_decompress.c` & `deflate-0.4.0/libdeflate/lib/deflate_decompress.c`

 * *Files 19% similar despite different names*

```diff
@@ -22,38 +22,32 @@
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  *
  * ---------------------------------------------------------------------------
  *
- * This is a highly optimized DEFLATE decompressor.  When compiled with gcc on
- * x86_64, it decompresses data in about 52% of the time of zlib (48% if BMI2
- * instructions are available).  On other architectures it should still be
- * significantly faster than zlib, but the difference may be smaller.
+ * This is a highly optimized DEFLATE decompressor.  It is much faster than
+ * vanilla zlib, typically well over twice as fast, though results vary by CPU.
  *
- * Why this is faster than zlib's implementation:
+ * Why this is faster than vanilla zlib:
  *
  * - Word accesses rather than byte accesses when reading input
  * - Word accesses rather than byte accesses when copying matches
  * - Faster Huffman decoding combined with various DEFLATE-specific tricks
- * - Larger bitbuffer variable that doesn't need to be filled as often
+ * - Larger bitbuffer variable that doesn't need to be refilled as often
  * - Other optimizations to remove unnecessary branches
  * - Only full-buffer decompression is supported, so the code doesn't need to
  *   support stopping and resuming decompression.
- * - On x86_64, compile a version of the decompression routine using BMI2
- *   instructions and use it automatically at runtime when supported.
+ * - On x86_64, a version of the decompression routine is compiled with BMI2
+ *   instructions enabled and is used automatically at runtime when supported.
  */
 
-#include <limits.h>
-
+#include "lib_common.h"
 #include "deflate_constants.h"
-#include "unaligned.h"
-
-#include "libdeflate.h"
 
 /*
  * If the expression passed to SAFETY_CHECK() evaluates to false, then the
  * decompression routine immediately returns LIBDEFLATE_BAD_DATA, indicating the
  * compressed data is invalid.
  *
  * Theoretically, these checks could be disabled for specialized applications
@@ -62,353 +56,459 @@
 #if 0
 #  pragma message("UNSAFE DECOMPRESSION IS ENABLED. THIS MUST ONLY BE USED IF THE DECOMPRESSOR INPUT WILL ALWAYS BE TRUSTED!")
 #  define SAFETY_CHECK(expr)	(void)(expr)
 #else
 #  define SAFETY_CHECK(expr)	if (unlikely(!(expr))) return LIBDEFLATE_BAD_DATA
 #endif
 
-/*
- * Each TABLEBITS number is the base-2 logarithm of the number of entries in the
- * main portion of the corresponding decode table.  Each number should be large
- * enough to ensure that for typical data, the vast majority of symbols can be
- * decoded by a direct lookup of the next TABLEBITS bits of compressed data.
- * However, this must be balanced against the fact that a larger table requires
- * more memory and requires more time to fill.
- *
- * Note: you cannot change a TABLEBITS number without also changing the
- * corresponding ENOUGH number!
- */
-#define PRECODE_TABLEBITS	7
-#define LITLEN_TABLEBITS	10
-#define OFFSET_TABLEBITS	8
-
-/*
- * Each ENOUGH number is the maximum number of decode table entries that may be
- * required for the corresponding Huffman code, including the main table and all
- * subtables.  Each number depends on three parameters:
- *
- *	(1) the maximum number of symbols in the code (DEFLATE_NUM_*_SYMS)
- *	(2) the number of main table bits (the TABLEBITS numbers defined above)
- *	(3) the maximum allowed codeword length (DEFLATE_MAX_*_CODEWORD_LEN)
- *
- * The ENOUGH numbers were computed using the utility program 'enough' from
- * zlib.  This program enumerates all possible relevant Huffman codes to find
- * the worst-case usage of decode table entries.
- */
-#define PRECODE_ENOUGH		128	/* enough 19 7 7	*/
-#define LITLEN_ENOUGH		1334	/* enough 288 10 15	*/
-#define OFFSET_ENOUGH		402	/* enough 32 8 15	*/
-
-/*
- * Type for codeword lengths.
- */
-typedef u8 len_t;
-
-/*
- * The main DEFLATE decompressor structure.  Since this implementation only
- * supports full buffer decompression, this structure does not store the entire
- * decompression state, but rather only some arrays that are too large to
- * comfortably allocate on the stack.
- */
-struct libdeflate_decompressor {
-
-	/*
-	 * The arrays aren't all needed at the same time.  'precode_lens' and
-	 * 'precode_decode_table' are unneeded after 'lens' has been filled.
-	 * Furthermore, 'lens' need not be retained after building the litlen
-	 * and offset decode tables.  In fact, 'lens' can be in union with
-	 * 'litlen_decode_table' provided that 'offset_decode_table' is separate
-	 * and is built first.
-	 */
-
-	union {
-		len_t precode_lens[DEFLATE_NUM_PRECODE_SYMS];
-
-		struct {
-			len_t lens[DEFLATE_NUM_LITLEN_SYMS +
-				   DEFLATE_NUM_OFFSET_SYMS +
-				   DEFLATE_MAX_LENS_OVERRUN];
-
-			u32 precode_decode_table[PRECODE_ENOUGH];
-		} l;
-
-		u32 litlen_decode_table[LITLEN_ENOUGH];
-	} u;
-
-	u32 offset_decode_table[OFFSET_ENOUGH];
-
-	/* used only during build_decode_table() */
-	u16 sorted_syms[DEFLATE_MAX_NUM_SYMS];
-
-	bool static_codes_loaded;
-};
-
 /*****************************************************************************
  *				Input bitstream                              *
  *****************************************************************************/
 
 /*
  * The state of the "input bitstream" consists of the following variables:
  *
- *	- in_next: pointer to the next unread byte in the input buffer
+ *	- in_next: a pointer to the next unread byte in the input buffer
  *
- *	- in_end: pointer just past the end of the input buffer
+ *	- in_end: a pointer to just past the end of the input buffer
  *
  *	- bitbuf: a word-sized variable containing bits that have been read from
- *		  the input buffer.  The buffered bits are right-aligned
- *		  (they're the low-order bits).
- *
- *	- bitsleft: number of bits in 'bitbuf' that are valid.
+ *		  the input buffer or from the implicit appended zero bytes
  *
- * To make it easier for the compiler to optimize the code by keeping variables
- * in registers, these are declared as normal variables and manipulated using
- * macros.
+ *	- bitsleft: the number of bits in 'bitbuf' available to be consumed.
+ *		    After REFILL_BITS_BRANCHLESS(), 'bitbuf' can actually
+ *		    contain more bits than this.  However, only the bits counted
+ *		    by 'bitsleft' can actually be consumed; the rest can only be
+ *		    used for preloading.
+ *
+ *		    As a micro-optimization, we allow bits 8 and higher of
+ *		    'bitsleft' to contain garbage.  When consuming the bits
+ *		    associated with a decode table entry, this allows us to do
+ *		    'bitsleft -= entry' instead of 'bitsleft -= (u8)entry'.
+ *		    On some CPUs, this helps reduce instruction dependencies.
+ *		    This does have the disadvantage that 'bitsleft' sometimes
+ *		    needs to be cast to 'u8', such as when it's used as a shift
+ *		    amount in REFILL_BITS_BRANCHLESS().  But that one happens
+ *		    for free since most CPUs ignore high bits in shift amounts.
+ *
+ *	- overread_count: the total number of implicit appended zero bytes that
+ *			  have been loaded into the bitbuffer, including any
+ *			  counted by 'bitsleft' and any already consumed
  */
 
 /*
  * The type for the bitbuffer variable ('bitbuf' described above).  For best
  * performance, this should have size equal to a machine word.
  *
  * 64-bit platforms have a significant advantage: they get a bigger bitbuffer
- * which they have to fill less often.
+ * which they don't have to refill as often.
  */
 typedef machine_word_t bitbuf_t;
+#define BITBUF_NBITS	(8 * (int)sizeof(bitbuf_t))
 
-/*
- * Number of bits the bitbuffer variable can hold.
- *
- * This is one less than the obvious value because of the optimized arithmetic
- * in FILL_BITS_WORDWISE() that leaves 'bitsleft' in the range
- * [WORDBITS - 8, WORDBITS - 1] rather than [WORDBITS - 7, WORDBITS].
- */
-#define BITBUF_NBITS	(8 * sizeof(bitbuf_t) - 1)
+/* BITMASK(n) returns a bitmask of length 'n'. */
+#define BITMASK(n)	(((bitbuf_t)1 << (n)) - 1)
 
 /*
- * The maximum number of bits that can be ensured in the bitbuffer variable,
- * i.e. the maximum value of 'n' that can be passed ENSURE_BITS(n).  The decoder
- * only reads whole bytes from memory, so this is the lowest value of 'bitsleft'
- * at which another byte cannot be read without first consuming some bits.
+ * MAX_BITSLEFT is the maximum number of consumable bits, i.e. the maximum value
+ * of '(u8)bitsleft'.  This is the size of the bitbuffer variable, minus 1 if
+ * the branchless refill method is being used (see REFILL_BITS_BRANCHLESS()).
  */
-#define MAX_ENSURE	(BITBUF_NBITS - 7)
+#define MAX_BITSLEFT	\
+	(UNALIGNED_ACCESS_IS_FAST ? BITBUF_NBITS - 1 : BITBUF_NBITS)
 
 /*
- * Evaluates to true if 'n' is a valid argument to ENSURE_BITS(n), or false if
- * 'n' is too large to be passed to ENSURE_BITS(n).  Note: if 'n' is a compile
- * time constant, then this expression will be a compile-type constant.
- * Therefore, CAN_ENSURE() can be used choose between alternative
- * implementations at compile time.
+ * CONSUMABLE_NBITS is the minimum number of bits that are guaranteed to be
+ * consumable (counted in 'bitsleft') immediately after refilling the bitbuffer.
+ * Since only whole bytes can be added to 'bitsleft', the worst case is
+ * 'MAX_BITSLEFT - 7': the smallest amount where another byte doesn't fit.
  */
-#define CAN_ENSURE(n)	((n) <= MAX_ENSURE)
+#define CONSUMABLE_NBITS	(MAX_BITSLEFT - 7)
 
 /*
- * Fill the bitbuffer variable, reading one byte at a time.
- *
- * If we would overread the input buffer, we just don't read anything, leaving
- * the bits zeroed but marking them filled.  This simplifies the decompressor
- * because it removes the need to distinguish between real overreads and
- * overreads that occur only because of the decompressor's own lookahead.
- *
- * The disadvantage is that real overreads are not detected immediately.
- * However, this is safe because the decompressor is still guaranteed to make
- * forward progress when presented never-ending 0 bits.  In an existing block
- * output will be getting generated, whereas new blocks can only be uncompressed
- * (since the type code for uncompressed blocks is 0), for which we check for
- * previous overread.  But even if we didn't check, uncompressed blocks would
- * fail to validate because LEN would not equal ~NLEN.  So the decompressor will
- * eventually either detect that the output buffer is full, or detect invalid
- * input, or finish the final block.
- */
-#define FILL_BITS_BYTEWISE()					\
-do {								\
-	if (likely(in_next != in_end))				\
-		bitbuf |= (bitbuf_t)*in_next++ << bitsleft;	\
-	else							\
-		overrun_count++;				\
-	bitsleft += 8;						\
-} while (bitsleft <= BITBUF_NBITS - 8)
-
-/*
- * Fill the bitbuffer variable by reading the next word from the input buffer
- * and branchlessly updating 'in_next' and 'bitsleft' based on how many bits
- * were filled.  This can be significantly faster than FILL_BITS_BYTEWISE().
- * However, for this to work correctly, the word must be interpreted in
- * little-endian format.  In addition, the memory access may be unaligned.
- * Therefore, this method is most efficient on little-endian architectures that
- * support fast unaligned access, such as x86 and x86_64.
- *
- * For faster updating of 'bitsleft', we consider the bitbuffer size in bits to
- * be 1 less than the word size and therefore be all 1 bits.  Then the number of
- * bits filled is the value of the 0 bits in position >= 3 when changed to 1.
- * E.g. if words are 64 bits and bitsleft = 16 = b010000 then we refill b101000
- * = 40 bits = 5 bytes.  This uses only 4 operations to update 'in_next' and
- * 'bitsleft': one each of +, ^, >>, and |.  (Not counting operations the
- * compiler optimizes out.)  In contrast, the alternative of:
- *
- *	in_next += (BITBUF_NBITS - bitsleft) >> 3;
- *	bitsleft += (BITBUF_NBITS - bitsleft) & ~7;
- *
- * (where BITBUF_NBITS would be WORDBITS rather than WORDBITS - 1) would on
- * average refill an extra bit, but uses 5 operations: two +, and one each of
- * -, >>, and &.  Also the - and & must be completed before 'bitsleft' can be
- * updated, while the current solution updates 'bitsleft' with no dependencies.
- */
-#define FILL_BITS_WORDWISE()					\
-do {								\
-	/* BITBUF_NBITS must be all 1's in binary, see above */	\
-	STATIC_ASSERT((BITBUF_NBITS & (BITBUF_NBITS + 1)) == 0);\
-								\
-	bitbuf |= get_unaligned_leword(in_next) << bitsleft;	\
-	in_next += (bitsleft ^ BITBUF_NBITS) >> 3;		\
-	bitsleft |= BITBUF_NBITS & ~7;				\
-} while (0)
-
-/*
- * Does the bitbuffer variable currently contain at least 'n' bits?
+ * FASTLOOP_PRELOADABLE_NBITS is the minimum number of bits that are guaranteed
+ * to be preloadable immediately after REFILL_BITS_IN_FASTLOOP().  (It is *not*
+ * guaranteed after REFILL_BITS(), since REFILL_BITS() falls back to a
+ * byte-at-a-time refill method near the end of input.)  This may exceed the
+ * number of consumable bits (counted by 'bitsleft').  Any bits not counted in
+ * 'bitsleft' can only be used for precomputation and cannot be consumed.
  */
-#define HAVE_BITS(n) (bitsleft >= (n))
+#define FASTLOOP_PRELOADABLE_NBITS	\
+	(UNALIGNED_ACCESS_IS_FAST ? BITBUF_NBITS : CONSUMABLE_NBITS)
 
 /*
- * Load more bits from the input buffer until the specified number of bits is
- * present in the bitbuffer variable.  'n' cannot be too large; see MAX_ENSURE
- * and CAN_ENSURE().
- */
-#define ENSURE_BITS(n)						\
-if (!HAVE_BITS(n)) {						\
-	if (CPU_IS_LITTLE_ENDIAN() &&				\
-	    UNALIGNED_ACCESS_IS_FAST &&				\
-	    likely(in_end - in_next >= sizeof(bitbuf_t)))	\
-		FILL_BITS_WORDWISE();				\
-	else							\
-		FILL_BITS_BYTEWISE();				\
-}
+ * PRELOAD_SLACK is the minimum number of bits that are guaranteed to be
+ * preloadable but not consumable, following REFILL_BITS_IN_FASTLOOP() and any
+ * subsequent consumptions.  This is 1 bit if the branchless refill method is
+ * being used, and 0 bits otherwise.
+ */
+#define PRELOAD_SLACK	MAX(0, FASTLOOP_PRELOADABLE_NBITS - MAX_BITSLEFT)
 
 /*
- * Return the next 'n' bits from the bitbuffer variable without removing them.
+ * CAN_CONSUME(n) is true if it's guaranteed that if the bitbuffer has just been
+ * refilled, then it's always possible to consume 'n' bits from it.  'n' should
+ * be a compile-time constant, to enable compile-time evaluation.
  */
-#define BITS(n) ((u32)bitbuf & (((u32)1 << (n)) - 1))
+#define CAN_CONSUME(n)	(CONSUMABLE_NBITS >= (n))
 
 /*
- * Remove the next 'n' bits from the bitbuffer variable.
+ * CAN_CONSUME_AND_THEN_PRELOAD(consume_nbits, preload_nbits) is true if it's
+ * guaranteed that after REFILL_BITS_IN_FASTLOOP(), it's always possible to
+ * consume 'consume_nbits' bits, then preload 'preload_nbits' bits.  The
+ * arguments should be compile-time constants to enable compile-time evaluation.
  */
-#define REMOVE_BITS(n) (bitbuf >>= (n), bitsleft -= (n))
+#define CAN_CONSUME_AND_THEN_PRELOAD(consume_nbits, preload_nbits)	\
+	(CONSUMABLE_NBITS >= (consume_nbits) &&				\
+	 FASTLOOP_PRELOADABLE_NBITS >= (consume_nbits) + (preload_nbits))
 
 /*
- * Remove and return the next 'n' bits from the bitbuffer variable.
+ * REFILL_BITS_BRANCHLESS() branchlessly refills the bitbuffer variable by
+ * reading the next word from the input buffer and updating 'in_next' and
+ * 'bitsleft' based on how many bits were refilled -- counting whole bytes only.
+ * This is much faster than reading a byte at a time, at least if the CPU is
+ * little endian and supports fast unaligned memory accesses.
+ *
+ * The simplest way of branchlessly updating 'bitsleft' would be:
+ *
+ *	bitsleft += (MAX_BITSLEFT - bitsleft) & ~7;
+ *
+ * To make it faster, we define MAX_BITSLEFT to be 'WORDBITS - 1' rather than
+ * WORDBITS, so that in binary it looks like 111111 or 11111.  Then, we update
+ * 'bitsleft' by just setting the bits above the low 3 bits:
+ *
+ *	bitsleft |= MAX_BITSLEFT & ~7;
+ *
+ * That compiles down to a single instruction like 'or $0x38, %rbp'.  Using
+ * 'MAX_BITSLEFT == WORDBITS - 1' also has the advantage that refills can be
+ * done when 'bitsleft == MAX_BITSLEFT' without invoking undefined behavior.
+ *
+ * The simplest way of branchlessly updating 'in_next' would be:
+ *
+ *	in_next += (MAX_BITSLEFT - bitsleft) >> 3;
+ *
+ * With 'MAX_BITSLEFT == WORDBITS - 1' we could use an XOR instead, though this
+ * isn't really better:
+ *
+ *	in_next += (MAX_BITSLEFT ^ bitsleft) >> 3;
+ *
+ * An alternative which can be marginally better is the following:
+ *
+ *	in_next += sizeof(bitbuf_t) - 1;
+ *	in_next -= (bitsleft >> 3) & 0x7;
+ *
+ * It seems this would increase the number of CPU instructions from 3 (sub, shr,
+ * add) to 4 (add, shr, and, sub).  However, if the CPU has a bitfield
+ * extraction instruction (e.g. arm's ubfx), it stays at 3, and is potentially
+ * more efficient because the length of the longest dependency chain decreases
+ * from 3 to 2.  This alternative also has the advantage that it ignores the
+ * high bits in 'bitsleft', so it is compatible with the micro-optimization we
+ * use where we let the high bits of 'bitsleft' contain garbage.
  */
-#define POP_BITS(n) (tmp32 = BITS(n), REMOVE_BITS(n), tmp32)
+#define REFILL_BITS_BRANCHLESS()					\
+do {									\
+	bitbuf |= get_unaligned_leword(in_next) << (u8)bitsleft;	\
+	in_next += sizeof(bitbuf_t) - 1;				\
+	in_next -= (bitsleft >> 3) & 0x7;				\
+	bitsleft |= MAX_BITSLEFT & ~7;					\
+} while (0)
 
 /*
- * Verify that the input buffer hasn't been overread, then align the input to
- * the next byte boundary, discarding any remaining bits in the current byte.
+ * REFILL_BITS() loads bits from the input buffer until the bitbuffer variable
+ * contains at least CONSUMABLE_NBITS consumable bits.
+ *
+ * This checks for the end of input, and it doesn't guarantee
+ * FASTLOOP_PRELOADABLE_NBITS, so it can't be used in the fastloop.
+ *
+ * If we would overread the input buffer, we just don't read anything, leaving
+ * the bits zeroed but marking them filled.  This simplifies the decompressor
+ * because it removes the need to always be able to distinguish between real
+ * overreads and overreads caused only by the decompressor's own lookahead.
  *
- * Note that if the bitbuffer variable currently contains more than 7 bits, then
- * we must rewind 'in_next', effectively putting those bits back.  Only the bits
- * in what would be the "current" byte if we were reading one byte at a time can
- * be actually discarded.
+ * We do still keep track of the number of bytes that have been overread, for
+ * two reasons.  First, it allows us to determine the exact number of bytes that
+ * were consumed once the stream ends or an uncompressed block is reached.
+ * Second, it allows us to stop early if the overread amount gets so large (more
+ * than sizeof bitbuf) that it can only be caused by a real overread.  (The
+ * second part is arguably unneeded, since libdeflate is buffer-based; given
+ * infinite zeroes, it will eventually either completely fill the output buffer
+ * or return an error.  However, we do it to be slightly more friendly to the
+ * not-recommended use case of decompressing with an unknown output size.)
  */
-#define ALIGN_INPUT()							\
+#define REFILL_BITS()							\
 do {									\
-	SAFETY_CHECK(overrun_count <= (bitsleft >> 3));			\
-	in_next -= (bitsleft >> 3) - overrun_count;			\
-	overrun_count = 0;						\
-	bitbuf = 0;							\
-	bitsleft = 0;							\
-} while(0)
+	if (UNALIGNED_ACCESS_IS_FAST &&					\
+	    likely(in_end - in_next >= sizeof(bitbuf_t))) {		\
+		REFILL_BITS_BRANCHLESS();				\
+	} else {							\
+		while ((u8)bitsleft < CONSUMABLE_NBITS) {		\
+			if (likely(in_next != in_end)) {		\
+				bitbuf |= (bitbuf_t)*in_next++ <<	\
+					  (u8)bitsleft;			\
+			} else {					\
+				overread_count++;			\
+				SAFETY_CHECK(overread_count <=		\
+					     sizeof(bitbuf_t));		\
+			}						\
+			bitsleft += 8;					\
+		}							\
+	}								\
+} while (0)
 
 /*
- * Read a 16-bit value from the input.  This must have been preceded by a call
- * to ALIGN_INPUT(), and the caller must have already checked for overrun.
+ * REFILL_BITS_IN_FASTLOOP() is like REFILL_BITS(), but it doesn't check for the
+ * end of the input.  It can only be used in the fastloop.
  */
-#define READ_U16() (tmp16 = get_unaligned_le16(in_next), in_next += 2, tmp16)
+#define REFILL_BITS_IN_FASTLOOP()					\
+do {									\
+	STATIC_ASSERT(UNALIGNED_ACCESS_IS_FAST ||			\
+		      FASTLOOP_PRELOADABLE_NBITS == CONSUMABLE_NBITS);	\
+	if (UNALIGNED_ACCESS_IS_FAST) {					\
+		REFILL_BITS_BRANCHLESS();				\
+	} else {							\
+		while ((u8)bitsleft < CONSUMABLE_NBITS) {		\
+			bitbuf |= (bitbuf_t)*in_next++ << (u8)bitsleft;	\
+			bitsleft += 8;					\
+		}							\
+	}								\
+} while (0)
+
+/*
+ * This is the worst-case maximum number of output bytes that are written to
+ * during each iteration of the fastloop.  The worst case is 2 literals, then a
+ * match of length DEFLATE_MAX_MATCH_LEN.  Additionally, some slack space must
+ * be included for the intentional overrun in the match copy implementation.
+ */
+#define FASTLOOP_MAX_BYTES_WRITTEN	\
+	(2 + DEFLATE_MAX_MATCH_LEN + (5 * WORDBYTES) - 1)
+
+/*
+ * This is the worst-case maximum number of input bytes that are read during
+ * each iteration of the fastloop.  To get this value, we first compute the
+ * greatest number of bits that can be refilled during a loop iteration.  The
+ * refill at the beginning can add at most MAX_BITSLEFT, and the amount that can
+ * be refilled later is no more than the maximum amount that can be consumed by
+ * 2 literals that don't need a subtable, then a match.  We convert this value
+ * to bytes, rounding up; this gives the maximum number of bytes that 'in_next'
+ * can be advanced.  Finally, we add sizeof(bitbuf_t) to account for
+ * REFILL_BITS_BRANCHLESS() reading a word past 'in_next'.
+ */
+#define FASTLOOP_MAX_BYTES_READ					\
+	(DIV_ROUND_UP(MAX_BITSLEFT + (2 * LITLEN_TABLEBITS) +	\
+		      LENGTH_MAXBITS + OFFSET_MAXBITS, 8) +	\
+	 sizeof(bitbuf_t))
 
 /*****************************************************************************
  *                              Huffman decoding                             *
  *****************************************************************************/
 
 /*
- * A decode table for order TABLEBITS consists of a main table of (1 <<
- * TABLEBITS) entries followed by a variable number of subtables.
- *
- * The decoding algorithm takes the next TABLEBITS bits of compressed data and
- * uses them as an index into the decode table.  The resulting entry is either a
- * "direct entry", meaning that it contains the value desired, or a "subtable
- * pointer", meaning that the entry references a subtable that must be indexed
- * using more bits of the compressed data to decode the symbol.
- *
- * Each decode table (a main table along with its subtables, if any) is
- * associated with a Huffman code.  Logically, the result of a decode table
- * lookup is a symbol from the alphabet from which the corresponding Huffman
- * code was constructed.  A symbol with codeword length n <= TABLEBITS is
- * associated with 2**(TABLEBITS - n) direct entries in the table, whereas a
- * symbol with codeword length n > TABLEBITS is associated with one or more
- * subtable entries.
- *
- * On top of this basic design, we implement several optimizations:
- *
- * - We store the length of each codeword directly in each of its decode table
- *   entries.  This allows the codeword length to be produced without indexing
- *   an additional table.
- *
- * - When beneficial, we don't store the Huffman symbol itself, but instead data
- *   generated from it.  For example, when decoding an offset symbol in DEFLATE,
- *   it's more efficient if we can decode the offset base and number of extra
- *   offset bits directly rather than decoding the offset symbol and then
- *   looking up both of those values in an additional table or tables.
+ * The fastest way to decode Huffman-encoded data is basically to use a decode
+ * table that maps the next TABLEBITS bits of data to their symbol.  Each entry
+ * decode_table[i] maps to the symbol whose codeword is a prefix of 'i'.  A
+ * symbol with codeword length 'n' has '2**(TABLEBITS-n)' entries in the table.
+ *
+ * Ideally, TABLEBITS and the maximum codeword length would be the same; some
+ * compression formats are designed with this goal in mind.  Unfortunately, in
+ * DEFLATE, the maximum litlen and offset codeword lengths are 15 bits, which is
+ * too large for a practical TABLEBITS.  It's not *that* much larger, though, so
+ * the workaround is to use a single level of subtables.  In the main table,
+ * entries for prefixes of codewords longer than TABLEBITS contain a "pointer"
+ * to the appropriate subtable along with the number of bits it is indexed with.
+ *
+ * The most efficient way to allocate subtables is to allocate them dynamically
+ * after the main table.  The worst-case number of table entries needed,
+ * including subtables, is precomputable; see the ENOUGH constants below.
+ *
+ * A useful optimization is to store the codeword lengths in the decode table so
+ * that they don't have to be looked up by indexing a separate table that maps
+ * symbols to their codeword lengths.  We basically do this; however, for the
+ * litlen and offset codes we also implement some DEFLATE-specific optimizations
+ * that build in the consideration of the "extra bits" and the
+ * literal/length/end-of-block division.  For the exact decode table entry
+ * format we use, see the definitions of the *_decode_results[] arrays below.
+ */
+
+
+/*
+ * These are the TABLEBITS values we use for each of the DEFLATE Huffman codes,
+ * along with their corresponding ENOUGH values.
+ *
+ * For the precode, we use PRECODE_TABLEBITS == 7 since this is the maximum
+ * precode codeword length.  This avoids ever needing subtables.
+ *
+ * For the litlen and offset codes, we cannot realistically avoid ever needing
+ * subtables, since litlen and offset codewords can be up to 15 bits.  A higher
+ * TABLEBITS reduces the number of lookups that need a subtable, which increases
+ * performance; however, it increases memory usage and makes building the table
+ * take longer, which decreases performance.  We choose values that work well in
+ * practice, making subtables rarely needed without making the tables too large.
+ *
+ * Our choice of OFFSET_TABLEBITS == 8 is a bit low; without any special
+ * considerations, 9 would fit the trade-off curve better.  However, there is a
+ * performance benefit to using exactly 8 bits when it is a compile-time
+ * constant, as many CPUs can take the low byte more easily than the low 9 bits.
+ *
+ * zlib treats its equivalents of TABLEBITS as maximum values; whenever it
+ * builds a table, it caps the actual table_bits to the longest codeword.  This
+ * makes sense in theory, as there's no need for the table to be any larger than
+ * needed to support the longest codeword.  However, having the table bits be a
+ * compile-time constant is beneficial to the performance of the decode loop, so
+ * there is a trade-off.  libdeflate currently uses the dynamic table_bits
+ * strategy for the litlen table only, due to its larger maximum size.
+ * PRECODE_TABLEBITS and OFFSET_TABLEBITS are smaller, so going dynamic there
+ * isn't as useful, and OFFSET_TABLEBITS=8 is useful as mentioned above.
+ *
+ * Each TABLEBITS value has a corresponding ENOUGH value that gives the
+ * worst-case maximum number of decode table entries, including the main table
+ * and all subtables.  The ENOUGH value depends on three parameters:
  *
- * The size of each decode table entry is 32 bits, which provides slightly
- * better performance than 16-bit entries on 32 and 64 bit processers, provided
- * that the table doesn't get so large that it takes up too much memory and
- * starts generating cache misses.  The bits of each decode table entry are
- * defined as follows:
+ *	(1) the maximum number of symbols in the code (DEFLATE_NUM_*_SYMS)
+ *	(2) the maximum number of main table bits (*_TABLEBITS)
+ *	(3) the maximum allowed codeword length (DEFLATE_MAX_*_CODEWORD_LEN)
  *
- * - Bits 30 -- 31: flags (see below)
- * - Bits 8 -- 29: decode result: a Huffman symbol or related data
- * - Bits 0 -- 7: codeword length
+ * The ENOUGH values were computed using the utility program 'enough' from zlib.
  */
+#define PRECODE_TABLEBITS	7
+#define PRECODE_ENOUGH		128	/* enough 19 7 7	*/
+#define LITLEN_TABLEBITS	11
+#define LITLEN_ENOUGH		2342	/* enough 288 11 15	*/
+#define OFFSET_TABLEBITS	8
+#define OFFSET_ENOUGH		402	/* enough 32 8 15	*/
 
 /*
- * This flag is set in all main decode table entries that represent subtable
- * pointers.
+ * make_decode_table_entry() creates a decode table entry for the given symbol
+ * by combining the static part 'decode_results[sym]' with the dynamic part
+ * 'len', which is the remaining codeword length (the codeword length for main
+ * table entries, or the codeword length minus TABLEBITS for subtable entries).
+ *
+ * In all cases, we add 'len' to each of the two low-order bytes to create the
+ * appropriately-formatted decode table entry.  See the definitions of the
+ * *_decode_results[] arrays below, where the entry format is described.
  */
-#define HUFFDEC_SUBTABLE_POINTER	0x80000000
+static forceinline u32
+make_decode_table_entry(const u32 decode_results[], u32 sym, u32 len)
+{
+	return decode_results[sym] + (len << 8) + len;
+}
 
 /*
- * This flag is set in all entries in the litlen decode table that represent
- * literals.
+ * Here is the format of our precode decode table entries.  Bits not explicitly
+ * described contain zeroes:
+ *
+ *	Bit 20-16:  presym
+ *	Bit 10-8:   codeword length [not used]
+ *	Bit 2-0:    codeword length
+ *
+ * The precode decode table never has subtables, since we use
+ * PRECODE_TABLEBITS == DEFLATE_MAX_PRE_CODEWORD_LEN.
+ *
+ * precode_decode_results[] contains the static part of the entry for each
+ * symbol.  make_decode_table_entry() produces the final entries.
  */
-#define HUFFDEC_LITERAL			0x40000000
-
-/* Mask for extracting the codeword length from a decode table entry.  */
-#define HUFFDEC_LENGTH_MASK		0xFF
-
-/* Shift to extract the decode result from a decode table entry.  */
-#define HUFFDEC_RESULT_SHIFT		8
-
-/* Shift a decode result into its position in the decode table entry.  */
-#define HUFFDEC_RESULT_ENTRY(result)	((u32)(result) << HUFFDEC_RESULT_SHIFT)
-
-/* The decode result for each precode symbol.  There is no special optimization
- * for the precode; the decode result is simply the symbol value.  */
-static const u32 precode_decode_results[DEFLATE_NUM_PRECODE_SYMS] = {
-#define ENTRY(presym)	HUFFDEC_RESULT_ENTRY(presym)
+static const u32 precode_decode_results[] = {
+#define ENTRY(presym)	((u32)presym << 16)
 	ENTRY(0)   , ENTRY(1)   , ENTRY(2)   , ENTRY(3)   ,
 	ENTRY(4)   , ENTRY(5)   , ENTRY(6)   , ENTRY(7)   ,
 	ENTRY(8)   , ENTRY(9)   , ENTRY(10)  , ENTRY(11)  ,
 	ENTRY(12)  , ENTRY(13)  , ENTRY(14)  , ENTRY(15)  ,
 	ENTRY(16)  , ENTRY(17)  , ENTRY(18)  ,
 #undef ENTRY
 };
 
-/* The decode result for each litlen symbol.  For literals, this is the literal
- * value itself and the HUFFDEC_LITERAL flag.  For lengths, this is the length
- * base and the number of extra length bits.  */
-static const u32 litlen_decode_results[DEFLATE_NUM_LITLEN_SYMS] = {
+/* Litlen and offset decode table entry flags */
 
-	/* Literals  */
-#define ENTRY(literal)	(HUFFDEC_LITERAL | HUFFDEC_RESULT_ENTRY(literal))
+/* Indicates a literal entry in the litlen decode table */
+#define HUFFDEC_LITERAL			0x80000000
+
+/* Indicates that HUFFDEC_SUBTABLE_POINTER or HUFFDEC_END_OF_BLOCK is set */
+#define HUFFDEC_EXCEPTIONAL		0x00008000
+
+/* Indicates a subtable pointer entry in the litlen or offset decode table */
+#define HUFFDEC_SUBTABLE_POINTER	0x00004000
+
+/* Indicates an end-of-block entry in the litlen decode table */
+#define HUFFDEC_END_OF_BLOCK		0x00002000
+
+/* Maximum number of bits that can be consumed by decoding a match length */
+#define LENGTH_MAXBITS		(DEFLATE_MAX_LITLEN_CODEWORD_LEN + \
+				 DEFLATE_MAX_EXTRA_LENGTH_BITS)
+#define LENGTH_MAXFASTBITS	(LITLEN_TABLEBITS /* no subtable needed */ + \
+				 DEFLATE_MAX_EXTRA_LENGTH_BITS)
+
+/*
+ * Here is the format of our litlen decode table entries.  Bits not explicitly
+ * described contain zeroes:
+ *
+ *	Literals:
+ *		Bit 31:     1 (HUFFDEC_LITERAL)
+ *		Bit 23-16:  literal value
+ *		Bit 15:     0 (!HUFFDEC_EXCEPTIONAL)
+ *		Bit 14:     0 (!HUFFDEC_SUBTABLE_POINTER)
+ *		Bit 13:     0 (!HUFFDEC_END_OF_BLOCK)
+ *		Bit 11-8:   remaining codeword length [not used]
+ *		Bit 3-0:    remaining codeword length
+ *	Lengths:
+ *		Bit 31:     0 (!HUFFDEC_LITERAL)
+ *		Bit 24-16:  length base value
+ *		Bit 15:     0 (!HUFFDEC_EXCEPTIONAL)
+ *		Bit 14:     0 (!HUFFDEC_SUBTABLE_POINTER)
+ *		Bit 13:     0 (!HUFFDEC_END_OF_BLOCK)
+ *		Bit 11-8:   remaining codeword length
+ *		Bit 4-0:    remaining codeword length + number of extra bits
+ *	End of block:
+ *		Bit 31:     0 (!HUFFDEC_LITERAL)
+ *		Bit 15:     1 (HUFFDEC_EXCEPTIONAL)
+ *		Bit 14:     0 (!HUFFDEC_SUBTABLE_POINTER)
+ *		Bit 13:     1 (HUFFDEC_END_OF_BLOCK)
+ *		Bit 11-8:   remaining codeword length [not used]
+ *		Bit 3-0:    remaining codeword length
+ *	Subtable pointer:
+ *		Bit 31:     0 (!HUFFDEC_LITERAL)
+ *		Bit 30-16:  index of start of subtable
+ *		Bit 15:     1 (HUFFDEC_EXCEPTIONAL)
+ *		Bit 14:     1 (HUFFDEC_SUBTABLE_POINTER)
+ *		Bit 13:     0 (!HUFFDEC_END_OF_BLOCK)
+ *		Bit 11-8:   number of subtable bits
+ *		Bit 3-0:    number of main table bits
+ *
+ * This format has several desirable properties:
+ *
+ *	- The codeword length, length slot base, and number of extra length bits
+ *	  are all built in.  This eliminates the need to separately look up this
+ *	  information by indexing separate arrays by symbol or length slot.
+ *
+ *	- The HUFFDEC_* flags enable easily distinguishing between the different
+ *	  types of entries.  The HUFFDEC_LITERAL flag enables a fast path for
+ *	  literals; the high bit is used for this, as some CPUs can test the
+ *	  high bit more easily than other bits.  The HUFFDEC_EXCEPTIONAL flag
+ *	  makes it possible to detect the two unlikely cases (subtable pointer
+ *	  and end of block) in a single bit flag test.
+ *
+ *	- The low byte is the number of bits that need to be removed from the
+ *	  bitstream; this makes this value easily accessible, and it enables the
+ *	  micro-optimization of doing 'bitsleft -= entry' instead of
+ *	  'bitsleft -= (u8)entry'.  It also includes the number of extra bits,
+ *	  so they don't need to be removed separately.
+ *
+ *	- The flags in bits 15-13 are arranged to be 0 when the
+ *	  "remaining codeword length" in bits 11-8 is needed, making this value
+ *	  fairly easily accessible as well via a shift and downcast.
+ *
+ *	- Similarly, bits 13-12 are 0 when the "subtable bits" in bits 11-8 are
+ *	  needed, making it possible to extract this value with '& 0x3F' rather
+ *	  than '& 0xF'.  This value is only used as a shift amount, so this can
+ *	  save an 'and' instruction as the masking by 0x3F happens implicitly.
+ *
+ * litlen_decode_results[] contains the static part of the entry for each
+ * symbol.  make_decode_table_entry() produces the final entries.
+ */
+static const u32 litlen_decode_results[] = {
+
+	/* Literals */
+#define ENTRY(literal)	(HUFFDEC_LITERAL | ((u32)literal << 16))
 	ENTRY(0)   , ENTRY(1)   , ENTRY(2)   , ENTRY(3)   ,
 	ENTRY(4)   , ENTRY(5)   , ENTRY(6)   , ENTRY(7)   ,
 	ENTRY(8)   , ENTRY(9)   , ENTRY(10)  , ENTRY(11)  ,
 	ENTRY(12)  , ENTRY(13)  , ENTRY(14)  , ENTRY(15)  ,
 	ENTRY(16)  , ENTRY(17)  , ENTRY(18)  , ENTRY(19)  ,
 	ENTRY(20)  , ENTRY(21)  , ENTRY(22)  , ENTRY(23)  ,
 	ENTRY(24)  , ENTRY(25)  , ENTRY(26)  , ENTRY(27)  ,
@@ -467,58 +567,117 @@
 	ENTRY(236) , ENTRY(237) , ENTRY(238) , ENTRY(239) ,
 	ENTRY(240) , ENTRY(241) , ENTRY(242) , ENTRY(243) ,
 	ENTRY(244) , ENTRY(245) , ENTRY(246) , ENTRY(247) ,
 	ENTRY(248) , ENTRY(249) , ENTRY(250) , ENTRY(251) ,
 	ENTRY(252) , ENTRY(253) , ENTRY(254) , ENTRY(255) ,
 #undef ENTRY
 
-#define HUFFDEC_EXTRA_LENGTH_BITS_MASK	0xFF
-#define HUFFDEC_LENGTH_BASE_SHIFT	8
-#define HUFFDEC_END_OF_BLOCK_LENGTH	0
-
-#define ENTRY(length_base, num_extra_bits)	HUFFDEC_RESULT_ENTRY(	\
-	((u32)(length_base) << HUFFDEC_LENGTH_BASE_SHIFT) | (num_extra_bits))
+	/* End of block */
+	HUFFDEC_EXCEPTIONAL | HUFFDEC_END_OF_BLOCK,
 
-	/* End of block  */
-	ENTRY(HUFFDEC_END_OF_BLOCK_LENGTH, 0),
-
-	/* Lengths  */
+	/* Lengths */
+#define ENTRY(length_base, num_extra_bits)	\
+	(((u32)(length_base) << 16) | (num_extra_bits))
 	ENTRY(3  , 0) , ENTRY(4  , 0) , ENTRY(5  , 0) , ENTRY(6  , 0),
 	ENTRY(7  , 0) , ENTRY(8  , 0) , ENTRY(9  , 0) , ENTRY(10 , 0),
 	ENTRY(11 , 1) , ENTRY(13 , 1) , ENTRY(15 , 1) , ENTRY(17 , 1),
 	ENTRY(19 , 2) , ENTRY(23 , 2) , ENTRY(27 , 2) , ENTRY(31 , 2),
 	ENTRY(35 , 3) , ENTRY(43 , 3) , ENTRY(51 , 3) , ENTRY(59 , 3),
 	ENTRY(67 , 4) , ENTRY(83 , 4) , ENTRY(99 , 4) , ENTRY(115, 4),
 	ENTRY(131, 5) , ENTRY(163, 5) , ENTRY(195, 5) , ENTRY(227, 5),
 	ENTRY(258, 0) , ENTRY(258, 0) , ENTRY(258, 0) ,
 #undef ENTRY
 };
 
-/* The decode result for each offset symbol.  This is the offset base and the
- * number of extra offset bits.  */
-static const u32 offset_decode_results[DEFLATE_NUM_OFFSET_SYMS] = {
-
-#define HUFFDEC_EXTRA_OFFSET_BITS_SHIFT 16
-#define HUFFDEC_OFFSET_BASE_MASK (((u32)1 << HUFFDEC_EXTRA_OFFSET_BITS_SHIFT) - 1)
-
-#define ENTRY(offset_base, num_extra_bits)	HUFFDEC_RESULT_ENTRY(	\
-		((u32)(num_extra_bits) << HUFFDEC_EXTRA_OFFSET_BITS_SHIFT) | \
-		(offset_base))
+/* Maximum number of bits that can be consumed by decoding a match offset */
+#define OFFSET_MAXBITS		(DEFLATE_MAX_OFFSET_CODEWORD_LEN + \
+				 DEFLATE_MAX_EXTRA_OFFSET_BITS)
+#define OFFSET_MAXFASTBITS	(OFFSET_TABLEBITS /* no subtable needed */ + \
+				 DEFLATE_MAX_EXTRA_OFFSET_BITS)
+
+/*
+ * Here is the format of our offset decode table entries.  Bits not explicitly
+ * described contain zeroes:
+ *
+ *	Offsets:
+ *		Bit 31-16:  offset base value
+ *		Bit 15:     0 (!HUFFDEC_EXCEPTIONAL)
+ *		Bit 14:     0 (!HUFFDEC_SUBTABLE_POINTER)
+ *		Bit 11-8:   remaining codeword length
+ *		Bit 4-0:    remaining codeword length + number of extra bits
+ *	Subtable pointer:
+ *		Bit 31-16:  index of start of subtable
+ *		Bit 15:     1 (HUFFDEC_EXCEPTIONAL)
+ *		Bit 14:     1 (HUFFDEC_SUBTABLE_POINTER)
+ *		Bit 11-8:   number of subtable bits
+ *		Bit 3-0:    number of main table bits
+ *
+ * These work the same way as the length entries and subtable pointer entries in
+ * the litlen decode table; see litlen_decode_results[] above.
+ */
+static const u32 offset_decode_results[] = {
+#define ENTRY(offset_base, num_extra_bits)	\
+	(((u32)(offset_base) << 16) | (num_extra_bits))
 	ENTRY(1     , 0)  , ENTRY(2     , 0)  , ENTRY(3     , 0)  , ENTRY(4     , 0)  ,
 	ENTRY(5     , 1)  , ENTRY(7     , 1)  , ENTRY(9     , 2)  , ENTRY(13    , 2) ,
 	ENTRY(17    , 3)  , ENTRY(25    , 3)  , ENTRY(33    , 4)  , ENTRY(49    , 4)  ,
 	ENTRY(65    , 5)  , ENTRY(97    , 5)  , ENTRY(129   , 6)  , ENTRY(193   , 6)  ,
 	ENTRY(257   , 7)  , ENTRY(385   , 7)  , ENTRY(513   , 8)  , ENTRY(769   , 8)  ,
 	ENTRY(1025  , 9)  , ENTRY(1537  , 9)  , ENTRY(2049  , 10) , ENTRY(3073  , 10) ,
 	ENTRY(4097  , 11) , ENTRY(6145  , 11) , ENTRY(8193  , 12) , ENTRY(12289 , 12) ,
-	ENTRY(16385 , 13) , ENTRY(24577 , 13) , ENTRY(32769 , 14) , ENTRY(49153 , 14) ,
+	ENTRY(16385 , 13) , ENTRY(24577 , 13) , ENTRY(24577 , 13) , ENTRY(24577 , 13) ,
 #undef ENTRY
 };
 
 /*
+ * The main DEFLATE decompressor structure.  Since libdeflate only supports
+ * full-buffer decompression, this structure doesn't store the entire
+ * decompression state, most of which is in stack variables.  Instead, this
+ * struct just contains the decode tables and some temporary arrays used for
+ * building them, as these are too large to comfortably allocate on the stack.
+ *
+ * Storing the decode tables in the decompressor struct also allows the decode
+ * tables for the static codes to be reused whenever two static Huffman blocks
+ * are decoded without an intervening dynamic block, even across streams.
+ */
+struct libdeflate_decompressor {
+
+	/*
+	 * The arrays aren't all needed at the same time.  'precode_lens' and
+	 * 'precode_decode_table' are unneeded after 'lens' has been filled.
+	 * Furthermore, 'lens' need not be retained after building the litlen
+	 * and offset decode tables.  In fact, 'lens' can be in union with
+	 * 'litlen_decode_table' provided that 'offset_decode_table' is separate
+	 * and is built first.
+	 */
+
+	union {
+		u8 precode_lens[DEFLATE_NUM_PRECODE_SYMS];
+
+		struct {
+			u8 lens[DEFLATE_NUM_LITLEN_SYMS +
+				DEFLATE_NUM_OFFSET_SYMS +
+				DEFLATE_MAX_LENS_OVERRUN];
+
+			u32 precode_decode_table[PRECODE_ENOUGH];
+		} l;
+
+		u32 litlen_decode_table[LITLEN_ENOUGH];
+	} u;
+
+	u32 offset_decode_table[OFFSET_ENOUGH];
+
+	/* used only during build_decode_table() */
+	u16 sorted_syms[DEFLATE_MAX_NUM_SYMS];
+
+	bool static_codes_loaded;
+	unsigned litlen_tablebits;
+};
+
+/*
  * Build a table for fast decoding of symbols from a Huffman code.  As input,
  * this function takes the codeword length of each symbol which may be used in
  * the code.  As output, it produces a decode table for the canonical Huffman
  * code described by the codeword lengths.  The decode table is built with the
  * assumption that it will be indexed with "bit-reversed" codewords, where the
  * low-order bit is the first bit of the codeword.  This format is used for all
  * Huffman codes in DEFLATE.
@@ -533,37 +692,42 @@
  *	@lens have been consumed.  All codeword lengths are assumed to be <=
  *	@max_codeword_len but are otherwise considered untrusted.  If they do
  *	not form a valid Huffman code, then the decode table is not built and
  *	%false is returned.
  * @num_syms
  *	The number of symbols in the code, including all unused symbols.
  * @decode_results
- *	An array which provides, for each symbol, the actual value to store into
- *	the decode table.  This value will be directly produced as the result of
- *	decoding that symbol, thereby moving the indirection out of the decode
- *	loop and into the table initialization.
+ *	An array which gives the incomplete decode result for each symbol.  The
+ *	needed values in this array will be combined with codeword lengths to
+ *	make the final decode table entries using make_decode_table_entry().
  * @table_bits
  *	The log base-2 of the number of main table entries to use.
+ *	If @table_bits_ret != NULL, then @table_bits is treated as a maximum
+ *	value and it will be decreased if a smaller table would be sufficient.
  * @max_codeword_len
  *	The maximum allowed codeword length for this Huffman code.
  *	Must be <= DEFLATE_MAX_CODEWORD_LEN.
  * @sorted_syms
  *	A temporary array of length @num_syms.
+ * @table_bits_ret
+ *	If non-NULL, then the dynamic table_bits is enabled, and the actual
+ *	table_bits value will be returned here.
  *
  * Returns %true if successful; %false if the codeword lengths do not form a
  * valid Huffman code.
  */
 static bool
 build_decode_table(u32 decode_table[],
-		   const len_t lens[],
+		   const u8 lens[],
 		   const unsigned num_syms,
 		   const u32 decode_results[],
-		   const unsigned table_bits,
-		   const unsigned max_codeword_len,
-		   u16 *sorted_syms)
+		   unsigned table_bits,
+		   unsigned max_codeword_len,
+		   u16 *sorted_syms,
+		   unsigned *table_bits_ret)
 {
 	unsigned len_counts[DEFLATE_MAX_CODEWORD_LEN + 1];
 	unsigned offsets[DEFLATE_MAX_CODEWORD_LEN + 1];
 	unsigned sym;		/* current symbol */
 	unsigned codeword;	/* current codeword, bit-reversed */
 	unsigned len;		/* current codeword length in bits */
 	unsigned count;		/* num codewords remaining with this length */
@@ -576,14 +740,25 @@
 	/* Count how many codewords have each length, including 0. */
 	for (len = 0; len <= max_codeword_len; len++)
 		len_counts[len] = 0;
 	for (sym = 0; sym < num_syms; sym++)
 		len_counts[lens[sym]]++;
 
 	/*
+	 * Determine the actual maximum codeword length that was used, and
+	 * decrease table_bits to it if allowed.
+	 */
+	while (max_codeword_len > 1 && len_counts[max_codeword_len] == 0)
+		max_codeword_len--;
+	if (table_bits_ret != NULL) {
+		table_bits = MIN(table_bits, max_codeword_len);
+		*table_bits_ret = table_bits;
+	}
+
+	/*
 	 * Sort the symbols primarily by increasing codeword length and
 	 * secondarily by increasing symbol value; or equivalently by their
 	 * codewords in lexicographic order, since a canonical code is assumed.
 	 *
 	 * For efficiency, also compute 'codespace_used' in the same pass over
 	 * 'len_counts[]' used to build 'offsets[]' for sorting.
 	 */
@@ -631,15 +806,15 @@
 			/*
 			 * An empty code is allowed.  This can happen for the
 			 * offset code in DEFLATE, since a dynamic Huffman block
 			 * need not contain any matches.
 			 */
 
 			/* sym=0, len=1 (arbitrary) */
-			entry = decode_results[0] | 1;
+			entry = make_decode_table_entry(decode_results, 0, 1);
 		} else {
 			/*
 			 * Allow codes with a single used symbol, with codeword
 			 * length 1.  The DEFLATE RFC is unclear regarding this
 			 * case.  What zlib's decompressor does is permit this
 			 * for the litlen and offset codes and assume the
 			 * codeword is '0' rather than '1'.  We do the same
@@ -647,15 +822,16 @@
 			 * no convincing reason to treat the codes differently.
 			 * We also assign both codewords '0' and '1' to the
 			 * symbol to avoid having to handle '1' specially.
 			 */
 			if (codespace_used != (1U << (max_codeword_len - 1)) ||
 			    len_counts[1] != 1)
 				return false;
-			entry = decode_results[*sorted_syms] | 1;
+			entry = make_decode_table_entry(decode_results,
+							*sorted_syms, 1);
 		}
 		/*
 		 * Note: the decode table still must be fully initialized, in
 		 * case the stream is malformed and contains bits from the part
 		 * of the codespace the incomplete code doesn't use.
 		 */
 		for (i = 0; i < (1U << table_bits); i++)
@@ -695,15 +871,16 @@
 	while (len <= table_bits) {
 		/* Process all 'count' codewords with length 'len' bits. */
 		do {
 			unsigned bit;
 
 			/* Fill the first entry for the current codeword. */
 			decode_table[codeword] =
-				decode_results[*sorted_syms++] | len;
+				make_decode_table_entry(decode_results,
+							*sorted_syms++, len);
 
 			if (codeword == cur_table_end - 1) {
 				/* Last codeword (all 1's) */
 				for (; len < table_bits; len++) {
 					memcpy(&decode_table[cur_table_end],
 					       decode_table,
 					       cur_table_end *
@@ -778,27 +955,26 @@
 				codespace_used = (codespace_used << 1) +
 					len_counts[table_bits + subtable_bits];
 			}
 			cur_table_end = subtable_start + (1U << subtable_bits);
 
 			/*
 			 * Create the entry that points from the main table to
-			 * the subtable.  This entry contains the index of the
-			 * start of the subtable and the number of bits with
-			 * which the subtable is indexed (the log base 2 of the
-			 * number of entries it contains).
+			 * the subtable.
 			 */
 			decode_table[subtable_prefix] =
+				((u32)subtable_start << 16) |
+				HUFFDEC_EXCEPTIONAL |
 				HUFFDEC_SUBTABLE_POINTER |
-				HUFFDEC_RESULT_ENTRY(subtable_start) |
-				subtable_bits;
+				(subtable_bits << 8) | table_bits;
 		}
 
 		/* Fill the subtable entries for the current codeword. */
-		entry = decode_results[*sorted_syms++] | (len - table_bits);
+		entry = make_decode_table_entry(decode_results, *sorted_syms++,
+						len - table_bits);
 		i = subtable_start + (codeword >> table_bits);
 		stride = 1U << (len - table_bits);
 		do {
 			decode_table[i] = entry;
 			i += stride;
 		} while (i < cur_table_end);
 
@@ -817,161 +993,157 @@
 /* Build the decode table for the precode.  */
 static bool
 build_precode_decode_table(struct libdeflate_decompressor *d)
 {
 	/* When you change TABLEBITS, you must change ENOUGH, and vice versa! */
 	STATIC_ASSERT(PRECODE_TABLEBITS == 7 && PRECODE_ENOUGH == 128);
 
+	STATIC_ASSERT(ARRAY_LEN(precode_decode_results) ==
+		      DEFLATE_NUM_PRECODE_SYMS);
+
 	return build_decode_table(d->u.l.precode_decode_table,
 				  d->u.precode_lens,
 				  DEFLATE_NUM_PRECODE_SYMS,
 				  precode_decode_results,
 				  PRECODE_TABLEBITS,
 				  DEFLATE_MAX_PRE_CODEWORD_LEN,
-				  d->sorted_syms);
+				  d->sorted_syms,
+				  NULL);
 }
 
 /* Build the decode table for the literal/length code.  */
 static bool
 build_litlen_decode_table(struct libdeflate_decompressor *d,
 			  unsigned num_litlen_syms, unsigned num_offset_syms)
 {
 	/* When you change TABLEBITS, you must change ENOUGH, and vice versa! */
-	STATIC_ASSERT(LITLEN_TABLEBITS == 10 && LITLEN_ENOUGH == 1334);
+	STATIC_ASSERT(LITLEN_TABLEBITS == 11 && LITLEN_ENOUGH == 2342);
+
+	STATIC_ASSERT(ARRAY_LEN(litlen_decode_results) ==
+		      DEFLATE_NUM_LITLEN_SYMS);
 
 	return build_decode_table(d->u.litlen_decode_table,
 				  d->u.l.lens,
 				  num_litlen_syms,
 				  litlen_decode_results,
 				  LITLEN_TABLEBITS,
 				  DEFLATE_MAX_LITLEN_CODEWORD_LEN,
-				  d->sorted_syms);
+				  d->sorted_syms,
+				  &d->litlen_tablebits);
 }
 
 /* Build the decode table for the offset code.  */
 static bool
 build_offset_decode_table(struct libdeflate_decompressor *d,
 			  unsigned num_litlen_syms, unsigned num_offset_syms)
 {
 	/* When you change TABLEBITS, you must change ENOUGH, and vice versa! */
 	STATIC_ASSERT(OFFSET_TABLEBITS == 8 && OFFSET_ENOUGH == 402);
 
+	STATIC_ASSERT(ARRAY_LEN(offset_decode_results) ==
+		      DEFLATE_NUM_OFFSET_SYMS);
+
 	return build_decode_table(d->offset_decode_table,
 				  d->u.l.lens + num_litlen_syms,
 				  num_offset_syms,
 				  offset_decode_results,
 				  OFFSET_TABLEBITS,
 				  DEFLATE_MAX_OFFSET_CODEWORD_LEN,
-				  d->sorted_syms);
-}
-
-static forceinline machine_word_t
-repeat_byte(u8 b)
-{
-	machine_word_t v;
-
-	STATIC_ASSERT(WORDBITS == 32 || WORDBITS == 64);
-
-	v = b;
-	v |= v << 8;
-	v |= v << 16;
-	v |= v << ((WORDBITS == 64) ? 32 : 0);
-	return v;
-}
-
-static forceinline void
-copy_word_unaligned(const void *src, void *dst)
-{
-	store_word_unaligned(load_word_unaligned(src), dst);
+				  d->sorted_syms,
+				  NULL);
 }
 
 /*****************************************************************************
  *                         Main decompression routine
  *****************************************************************************/
 
 typedef enum libdeflate_result (*decompress_func_t)
 	(struct libdeflate_decompressor * restrict d,
 	 const void * restrict in, size_t in_nbytes,
 	 void * restrict out, size_t out_nbytes_avail,
 	 size_t *actual_in_nbytes_ret, size_t *actual_out_nbytes_ret);
 
+#define FUNCNAME deflate_decompress_default
+#undef ATTRIBUTES
+#undef EXTRACT_VARBITS
+#undef EXTRACT_VARBITS8
+#include "decompress_template.h"
+
+/* Include architecture-specific implementation(s) if available. */
 #undef DEFAULT_IMPL
-#undef DISPATCH
-#if defined(__i386__) || defined(__x86_64__)
+#undef arch_select_decompress_func
+#if defined(ARCH_X86_32) || defined(ARCH_X86_64)
 #  include "x86/decompress_impl.h"
 #endif
 
 #ifndef DEFAULT_IMPL
-#  define FUNCNAME deflate_decompress_default
-#  define ATTRIBUTES
-#  include "decompress_template.h"
 #  define DEFAULT_IMPL deflate_decompress_default
 #endif
 
-#ifdef DISPATCH
+#ifdef arch_select_decompress_func
 static enum libdeflate_result
-dispatch(struct libdeflate_decompressor * restrict d,
-	 const void * restrict in, size_t in_nbytes,
-	 void * restrict out, size_t out_nbytes_avail,
-	 size_t *actual_in_nbytes_ret, size_t *actual_out_nbytes_ret);
+dispatch_decomp(struct libdeflate_decompressor *d,
+		const void *in, size_t in_nbytes,
+		void *out, size_t out_nbytes_avail,
+		size_t *actual_in_nbytes_ret, size_t *actual_out_nbytes_ret);
 
-static volatile decompress_func_t decompress_impl = dispatch;
+static volatile decompress_func_t decompress_impl = dispatch_decomp;
 
-/* Choose the fastest implementation at runtime */
+/* Choose the best implementation at runtime. */
 static enum libdeflate_result
-dispatch(struct libdeflate_decompressor * restrict d,
-	 const void * restrict in, size_t in_nbytes,
-	 void * restrict out, size_t out_nbytes_avail,
-	 size_t *actual_in_nbytes_ret, size_t *actual_out_nbytes_ret)
+dispatch_decomp(struct libdeflate_decompressor *d,
+		const void *in, size_t in_nbytes,
+		void *out, size_t out_nbytes_avail,
+		size_t *actual_in_nbytes_ret, size_t *actual_out_nbytes_ret)
 {
 	decompress_func_t f = arch_select_decompress_func();
 
 	if (f == NULL)
 		f = DEFAULT_IMPL;
 
 	decompress_impl = f;
-	return (*f)(d, in, in_nbytes, out, out_nbytes_avail,
-		    actual_in_nbytes_ret, actual_out_nbytes_ret);
+	return f(d, in, in_nbytes, out, out_nbytes_avail,
+		 actual_in_nbytes_ret, actual_out_nbytes_ret);
 }
 #else
-#  define decompress_impl DEFAULT_IMPL /* only one implementation, use it */
+/* The best implementation is statically known, so call it directly. */
+#  define decompress_impl DEFAULT_IMPL
 #endif
 
-
 /*
  * This is the main DEFLATE decompression routine.  See libdeflate.h for the
  * documentation.
  *
  * Note that the real code is in decompress_template.h.  The part here just
  * handles calling the appropriate implementation depending on the CPU features
  * at runtime.
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
-libdeflate_deflate_decompress_ex(struct libdeflate_decompressor * restrict d,
-				 const void * restrict in, size_t in_nbytes,
-				 void * restrict out, size_t out_nbytes_avail,
+LIBDEFLATEAPI enum libdeflate_result
+libdeflate_deflate_decompress_ex(struct libdeflate_decompressor *d,
+				 const void *in, size_t in_nbytes,
+				 void *out, size_t out_nbytes_avail,
 				 size_t *actual_in_nbytes_ret,
 				 size_t *actual_out_nbytes_ret)
 {
 	return decompress_impl(d, in, in_nbytes, out, out_nbytes_avail,
 			       actual_in_nbytes_ret, actual_out_nbytes_ret);
 }
 
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
-libdeflate_deflate_decompress(struct libdeflate_decompressor * restrict d,
-			      const void * restrict in, size_t in_nbytes,
-			      void * restrict out, size_t out_nbytes_avail,
+LIBDEFLATEAPI enum libdeflate_result
+libdeflate_deflate_decompress(struct libdeflate_decompressor *d,
+			      const void *in, size_t in_nbytes,
+			      void *out, size_t out_nbytes_avail,
 			      size_t *actual_out_nbytes_ret)
 {
 	return libdeflate_deflate_decompress_ex(d, in, in_nbytes,
 						out, out_nbytes_avail,
 						NULL, actual_out_nbytes_ret);
 }
 
-LIBDEFLATEEXPORT struct libdeflate_decompressor * LIBDEFLATEAPI
+LIBDEFLATEAPI struct libdeflate_decompressor *
 libdeflate_alloc_decompressor(void)
 {
 	/*
 	 * Note that only certain parts of the decompressor actually must be
 	 * initialized here:
 	 *
 	 * - 'static_codes_loaded' must be initialized to false.
@@ -989,12 +1161,12 @@
 
 	if (d == NULL)
 		return NULL;
 	memset(d, 0, sizeof(*d));
 	return d;
 }
 
-LIBDEFLATEEXPORT void LIBDEFLATEAPI
+LIBDEFLATEAPI void
 libdeflate_free_decompressor(struct libdeflate_decompressor *d)
 {
 	libdeflate_free(d);
 }
```

### Comparing `deflate-0.3.0/libdeflate/lib/gzip_compress.c` & `deflate-0.4.0/libdeflate/lib/gzip_compress.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * gzip_compress.c - compress with a gzip wrapper
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -25,19 +23,16 @@
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "deflate_compress.h"
 #include "gzip_constants.h"
-#include "unaligned.h"
-
-#include "libdeflate.h"
 
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_gzip_compress(struct libdeflate_compressor *c,
 			 const void *in, size_t in_nbytes,
 			 void *out, size_t out_nbytes_avail)
 {
 	u8 *out_next = out;
 	unsigned compression_level;
 	u8 xfl;
@@ -55,15 +50,15 @@
 	/* FLG */
 	*out_next++ = 0;
 	/* MTIME */
 	put_unaligned_le32(GZIP_MTIME_UNAVAILABLE, out_next);
 	out_next += 4;
 	/* XFL */
 	xfl = 0;
-	compression_level = deflate_get_compression_level(c);
+	compression_level = libdeflate_get_compression_level(c);
 	if (compression_level < 2)
 		xfl |= GZIP_XFL_FASTEST_COMPRESSION;
 	else if (compression_level >= 8)
 		xfl |= GZIP_XFL_SLOWEST_COMPRESSION;
 	*out_next++ = xfl;
 	/* OS */
 	*out_next++ = GZIP_OS_UNKNOWN;	/* OS  */
@@ -82,14 +77,14 @@
 	/* ISIZE */
 	put_unaligned_le32((u32)in_nbytes, out_next);
 	out_next += 4;
 
 	return out_next - (u8 *)out;
 }
 
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_gzip_compress_bound(struct libdeflate_compressor *c,
 			       size_t in_nbytes)
 {
 	return GZIP_MIN_OVERHEAD +
 	       libdeflate_deflate_compress_bound(c, in_nbytes);
 }
```

### Comparing `deflate-0.3.0/libdeflate/lib/gzip_constants.h` & `deflate-0.4.0/libdeflate/lib/gzip_constants.h`

 * *Files identical despite different names*

### Comparing `deflate-0.3.0/libdeflate/lib/gzip_decompress.c` & `deflate-0.4.0/libdeflate/lib/gzip_decompress.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * gzip_decompress.c - decompress with a gzip wrapper
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -23,20 +21,18 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
+#include "lib_common.h"
 #include "gzip_constants.h"
-#include "unaligned.h"
-
-#include "libdeflate.h"
 
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_gzip_decompress_ex(struct libdeflate_decompressor *d,
 			      const void *in, size_t in_nbytes,
 			      void *out, size_t out_nbytes_avail,
 			      size_t *actual_in_nbytes_ret,
 			      size_t *actual_out_nbytes_ret)
 {
 	const u8 *in_next = in;
@@ -132,15 +128,15 @@
 
 	if (actual_in_nbytes_ret)
 		*actual_in_nbytes_ret = in_next - (u8 *)in;
 
 	return LIBDEFLATE_SUCCESS;
 }
 
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_gzip_decompress(struct libdeflate_decompressor *d,
 			   const void *in, size_t in_nbytes,
 			   void *out, size_t out_nbytes_avail,
 			   size_t *actual_out_nbytes_ret)
 {
 	return libdeflate_gzip_decompress_ex(d, in, in_nbytes,
 					     out, out_nbytes_avail,
```

### Comparing `deflate-0.3.0/libdeflate/lib/hc_matchfinder.h` & `deflate-0.4.0/libdeflate/lib/hc_matchfinder.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * hc_matchfinder.h - Lempel-Ziv matchfinding with a hash table of linked lists
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -71,15 +69,15 @@
  * The main hash table and chains handle length 4+ matches.  Length 3 matches
  * are handled by a separate hash table with no chains.  This works well for
  * typical "greedy" or "lazy"-style compressors, where length 3 matches are
  * often only helpful if they have small offsets.  Instead of searching a full
  * chain for length 3+ matches, the algorithm just checks for one close length 3
  * match, then focuses on finding length 4+ matches.
  *
- * The longest_match() and skip_positions() functions are inlined into the
+ * The longest_match() and skip_bytes() functions are inlined into the
  * compressors that use them.  This isn't just about saving the overhead of a
  * function call.  These functions are intended to be called from the inner
  * loops of compressors, where giving the compiler more control over register
  * allocation is very helpful.  There is also significant benefit to be gained
  * from allowing the CPU to predict branches independently at each call site.
  * For example, "lazy"-style compressors can be written with two calls to
  * longest_match(), each of which starts with a different 'best_len' and
@@ -102,41 +100,39 @@
  * The code also uses a tight inner loop that only compares the last and first
  * bytes of a potential match.  It is only when these bytes match that a full
  * match extension is attempted.
  *
  * ----------------------------------------------------------------------------
  */
 
+#ifndef LIB_HC_MATCHFINDER_H
+#define LIB_HC_MATCHFINDER_H
+
 #include "matchfinder_common.h"
 
 #define HC_MATCHFINDER_HASH3_ORDER	15
 #define HC_MATCHFINDER_HASH4_ORDER	16
 
 #define HC_MATCHFINDER_TOTAL_HASH_SIZE			\
 	(((1UL << HC_MATCHFINDER_HASH3_ORDER) +		\
 	  (1UL << HC_MATCHFINDER_HASH4_ORDER)) * sizeof(mf_pos_t))
 
-struct hc_matchfinder {
+struct MATCHFINDER_ALIGNED hc_matchfinder  {
 
 	/* The hash table for finding length 3 matches  */
 	mf_pos_t hash3_tab[1UL << HC_MATCHFINDER_HASH3_ORDER];
 
 	/* The hash table which contains the first nodes of the linked lists for
 	 * finding length 4+ matches  */
 	mf_pos_t hash4_tab[1UL << HC_MATCHFINDER_HASH4_ORDER];
 
 	/* The "next node" references for the linked lists.  The "next node" of
 	 * the node for the sequence with position 'pos' is 'next_tab[pos]'.  */
 	mf_pos_t next_tab[MATCHFINDER_WINDOW_SIZE];
-
-}
-#ifdef _aligned_attribute
-  _aligned_attribute(MATCHFINDER_MEM_ALIGNMENT)
-#endif
-;
+};
 
 /* Prepare the matchfinder for a new input buffer.  */
 static forceinline void
 hc_matchfinder_init(struct hc_matchfinder *mf)
 {
 	STATIC_ASSERT(HC_MATCHFINDER_TOTAL_HASH_SIZE %
 		      MATCHFINDER_SIZE_ALIGNMENT == 0);
@@ -157,17 +153,17 @@
  *
  * @mf
  *	The matchfinder structure.
  * @in_base_p
  *	Location of a pointer which points to the place in the input data the
  *	matchfinder currently stores positions relative to.  This may be updated
  *	by this function.
- * @cur_pos
- *	The current position in the input buffer relative to @in_base (the
- *	position of the sequence being matched against).
+ * @in_next
+ *	Pointer to the next position in the input buffer, i.e. the sequence
+ *	being matched against.
  * @best_len
  *	Require a match longer than this length.
  * @max_len
  *	The maximum permissible match length at this position.
  * @nice_len
  *	Stop searching if a match of at least this length is found.
  *	Must be <= @max_len.
@@ -180,23 +176,23 @@
  * @offset_ret
  *	If a match is found, its offset is returned in this location.
  *
  * Return the length of the match found, or 'best_len' if no match longer than
  * 'best_len' was found.
  */
 static forceinline u32
-hc_matchfinder_longest_match(struct hc_matchfinder * const restrict mf,
-			     const u8 ** const restrict in_base_p,
-			     const u8 * const restrict in_next,
+hc_matchfinder_longest_match(struct hc_matchfinder * const mf,
+			     const u8 ** const in_base_p,
+			     const u8 * const in_next,
 			     u32 best_len,
 			     const u32 max_len,
 			     const u32 nice_len,
 			     const u32 max_search_depth,
-			     u32 * const restrict next_hashes,
-			     u32 * const restrict offset_ret)
+			     u32 * const next_hashes,
+			     u32 * const offset_ret)
 {
 	u32 depth_remaining = max_search_depth;
 	const u8 *best_matchptr = in_next;
 	mf_pos_t cur_node3, cur_node4;
 	u32 hash3, hash4;
 	u32 next_hashseq;
 	u32 seq4;
@@ -346,42 +342,40 @@
  *
  * @mf
  *	The matchfinder structure.
  * @in_base_p
  *	Location of a pointer which points to the place in the input data the
  *	matchfinder currently stores positions relative to.  This may be updated
  *	by this function.
- * @cur_pos
- *	The current position in the input buffer relative to @in_base.
- * @end_pos
- *	The end position of the input buffer, relative to @in_base.
+ * @in_next
+ *	Pointer to the next position in the input buffer.
+ * @in_end
+ *	Pointer to the end of the input buffer.
+ * @count
+ *	The number of bytes to advance.  Must be > 0.
  * @next_hashes
  *	The precomputed hash codes for the sequence beginning at @in_next.
  *	These will be used and then updated with the precomputed hashcodes for
  *	the sequence beginning at @in_next + @count.
- * @count
- *	The number of bytes to advance.  Must be > 0.
- *
- * Returns @in_next + @count.
  */
-static forceinline const u8 *
-hc_matchfinder_skip_positions(struct hc_matchfinder * const restrict mf,
-			      const u8 ** const restrict in_base_p,
-			      const u8 *in_next,
-			      const u8 * const in_end,
-			      const u32 count,
-			      u32 * const restrict next_hashes)
+static forceinline void
+hc_matchfinder_skip_bytes(struct hc_matchfinder * const mf,
+			  const u8 ** const in_base_p,
+			  const u8 *in_next,
+			  const u8 * const in_end,
+			  const u32 count,
+			  u32 * const next_hashes)
 {
 	u32 cur_pos;
 	u32 hash3, hash4;
 	u32 next_hashseq;
 	u32 remaining = count;
 
 	if (unlikely(count + 5 > in_end - in_next))
-		return &in_next[count];
+		return;
 
 	cur_pos = in_next - *in_base_p;
 	hash3 = next_hashes[0];
 	hash4 = next_hashes[1];
 	do {
 		if (cur_pos == MATCHFINDER_WINDOW_SIZE) {
 			hc_matchfinder_slide_window(mf);
@@ -398,10 +392,10 @@
 		cur_pos++;
 	} while (--remaining);
 
 	prefetchw(&mf->hash3_tab[hash3]);
 	prefetchw(&mf->hash4_tab[hash4]);
 	next_hashes[0] = hash3;
 	next_hashes[1] = hash4;
-
-	return in_next;
 }
+
+#endif /* LIB_HC_MATCHFINDER_H */
```

### Comparing `deflate-0.3.0/libdeflate/lib/matchfinder_common.h` & `deflate-0.4.0/libdeflate/lib/matchfinder_common.h`

 * *Files 25% similar despite different names*

```diff
@@ -2,20 +2,52 @@
  * matchfinder_common.h - common code for Lempel-Ziv matchfinding
  */
 
 #ifndef LIB_MATCHFINDER_COMMON_H
 #define LIB_MATCHFINDER_COMMON_H
 
 #include "lib_common.h"
-#include "unaligned.h"
 
 #ifndef MATCHFINDER_WINDOW_ORDER
 #  error "MATCHFINDER_WINDOW_ORDER must be defined!"
 #endif
 
+/*
+ * Given a 32-bit value that was loaded with the platform's native endianness,
+ * return a 32-bit value whose high-order 8 bits are 0 and whose low-order 24
+ * bits contain the first 3 bytes, arranged in octets in a platform-dependent
+ * order, at the memory location from which the input 32-bit value was loaded.
+ */
+static forceinline u32
+loaded_u32_to_u24(u32 v)
+{
+	if (CPU_IS_LITTLE_ENDIAN())
+		return v & 0xFFFFFF;
+	else
+		return v >> 8;
+}
+
+/*
+ * Load the next 3 bytes from @p into the 24 low-order bits of a 32-bit value.
+ * The order in which the 3 bytes will be arranged as octets in the 24 bits is
+ * platform-dependent.  At least 4 bytes (not 3) must be available at @p.
+ */
+static forceinline u32
+load_u24_unaligned(const u8 *p)
+{
+#if UNALIGNED_ACCESS_IS_FAST
+	return loaded_u32_to_u24(load_u32_unaligned(p));
+#else
+	if (CPU_IS_LITTLE_ENDIAN())
+		return ((u32)p[0] << 0) | ((u32)p[1] << 8) | ((u32)p[2] << 16);
+	else
+		return ((u32)p[2] << 0) | ((u32)p[1] << 8) | ((u32)p[0] << 16);
+#endif
+}
+
 #define MATCHFINDER_WINDOW_SIZE (1UL << MATCHFINDER_WINDOW_ORDER)
 
 typedef s16 mf_pos_t;
 
 #define MATCHFINDER_INITVAL ((mf_pos_t)-MATCHFINDER_WINDOW_SIZE)
 
 /*
@@ -24,19 +56,22 @@
  */
 #define MATCHFINDER_MEM_ALIGNMENT	32
 #define MATCHFINDER_SIZE_ALIGNMENT	128
 
 #undef matchfinder_init
 #undef matchfinder_rebase
 #ifdef _aligned_attribute
-#  if defined(__arm__) || defined(__aarch64__)
+#  define MATCHFINDER_ALIGNED _aligned_attribute(MATCHFINDER_MEM_ALIGNMENT)
+#  if defined(ARCH_ARM32) || defined(ARCH_ARM64)
 #    include "arm/matchfinder_impl.h"
-#  elif defined(__i386__) || defined(__x86_64__)
+#  elif defined(ARCH_X86_32) || defined(ARCH_X86_64)
 #    include "x86/matchfinder_impl.h"
 #  endif
+#else
+#  define MATCHFINDER_ALIGNED
 #endif
 
 /*
  * Initialize the hash table portion of the matchfinder.
  *
  * Essentially, this is an optimized memset().
  *
@@ -52,64 +87,52 @@
 
 	for (i = 0; i < num_entries; i++)
 		data[i] = MATCHFINDER_INITVAL;
 }
 #endif
 
 /*
- * Slide the matchfinder by WINDOW_SIZE bytes.
- *
- * This must be called just after each WINDOW_SIZE bytes have been run through
- * the matchfinder.
- *
- * This will subtract WINDOW_SIZE bytes from each entry in the array specified.
- * The effect is that all entries are updated to be relative to the current
- * position, rather than the position WINDOW_SIZE bytes prior.
- *
- * Underflow is detected and replaced with signed saturation.  This ensures that
- * once the sliding window has passed over a position, that position forever
- * remains out of bounds.
+ * Slide the matchfinder by MATCHFINDER_WINDOW_SIZE bytes.
  *
- * The array passed in must contain all matchfinder data that is
- * position-relative.  Concretely, this will include the hash table as well as
- * the table of positions that is used to link together the sequences in each
- * hash bucket.  Note that in the latter table, the links are 1-ary in the case
- * of "hash chains", and 2-ary in the case of "binary trees".  In either case,
- * the links need to be rebased in the same way.
+ * This must be called just after each MATCHFINDER_WINDOW_SIZE bytes have been
+ * run through the matchfinder.
  *
- * 'data' must be aligned to a MATCHFINDER_MEM_ALIGNMENT boundary, and
- * 'size' must be a multiple of MATCHFINDER_SIZE_ALIGNMENT.
+ * This subtracts MATCHFINDER_WINDOW_SIZE bytes from each entry in the given
+ * array, making the entries be relative to the current position rather than the
+ * position MATCHFINDER_WINDOW_SIZE bytes prior.  To avoid integer underflows,
+ * entries that would become less than -MATCHFINDER_WINDOW_SIZE stay at
+ * -MATCHFINDER_WINDOW_SIZE, keeping them permanently out of bounds.
+ *
+ * The given array must contain all matchfinder data that is position-relative:
+ * the hash table(s) as well as any hash chain or binary tree links.  Its
+ * address must be aligned to a MATCHFINDER_MEM_ALIGNMENT boundary, and its size
+ * must be a multiple of MATCHFINDER_SIZE_ALIGNMENT.
  */
 #ifndef matchfinder_rebase
 static forceinline void
 matchfinder_rebase(mf_pos_t *data, size_t size)
 {
 	size_t num_entries = size / sizeof(*data);
 	size_t i;
 
 	if (MATCHFINDER_WINDOW_SIZE == 32768) {
-		/* Branchless version for 32768 byte windows.  If the value was
-		 * already negative, clear all bits except the sign bit; this
-		 * changes the value to -32768.  Otherwise, set the sign bit;
-		 * this is equivalent to subtracting 32768.  */
+		/*
+		 * Branchless version for 32768-byte windows.  Clear all bits if
+		 * the value was already negative, then set the sign bit.  This
+		 * is equivalent to subtracting 32768 with signed saturation.
+		 */
+		for (i = 0; i < num_entries; i++)
+			data[i] = 0x8000 | (data[i] & ~(data[i] >> 15));
+	} else {
 		for (i = 0; i < num_entries; i++) {
-			u16 v = data[i];
-			u16 sign_bit = v & 0x8000;
-			v &= sign_bit - ((sign_bit >> 15) ^ 1);
-			v |= 0x8000;
-			data[i] = v;
+			if (data[i] >= 0)
+				data[i] -= (mf_pos_t)-MATCHFINDER_WINDOW_SIZE;
+			else
+				data[i] = (mf_pos_t)-MATCHFINDER_WINDOW_SIZE;
 		}
-		return;
-	}
-
-	for (i = 0; i < num_entries; i++) {
-		if (data[i] >= 0)
-			data[i] -= (mf_pos_t)-MATCHFINDER_WINDOW_SIZE;
-		else
-			data[i] = (mf_pos_t)-MATCHFINDER_WINDOW_SIZE;
 	}
 }
 #endif
 
 /*
  * The hash function: given a sequence prefix held in the low-order bits of a
  * 32-bit value, multiply by a carefully-chosen large constant.  Discard any
```

### Comparing `deflate-0.3.0/libdeflate/lib/utils.c` & `deflate-0.4.0/libdeflate/lib/utils.c`

 * *Files 23% similar despite different names*

```diff
@@ -23,16 +23,14 @@
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "lib_common.h"
 
-#include "libdeflate.h"
-
 #ifdef FREESTANDING
 #  define malloc NULL
 #  define free NULL
 #else
 #  include <stdlib.h>
 #endif
 
@@ -66,73 +64,88 @@
 void
 libdeflate_aligned_free(void *ptr)
 {
 	if (ptr)
 		libdeflate_free(((void **)ptr)[-1]);
 }
 
-LIBDEFLATEEXPORT void LIBDEFLATEAPI
+LIBDEFLATEAPI void
 libdeflate_set_memory_allocator(void *(*malloc_func)(size_t),
 				void (*free_func)(void *))
 {
 	libdeflate_malloc_func = malloc_func;
 	libdeflate_free_func = free_func;
 }
 
 /*
  * Implementations of libc functions for freestanding library builds.
  * Normal library builds don't use these.  Not optimized yet; usually the
  * compiler expands these functions and doesn't actually call them anyway.
  */
 #ifdef FREESTANDING
 #undef memset
-void *memset(void *s, int c, size_t n)
+void * __attribute__((weak))
+memset(void *s, int c, size_t n)
 {
 	u8 *p = s;
 	size_t i;
 
 	for (i = 0; i < n; i++)
 		p[i] = c;
 	return s;
 }
 
 #undef memcpy
-void *memcpy(void *dest, const void *src, size_t n)
+void * __attribute__((weak))
+memcpy(void *dest, const void *src, size_t n)
 {
 	u8 *d = dest;
 	const u8 *s = src;
 	size_t i;
 
 	for (i = 0; i < n; i++)
 		d[i] = s[i];
 	return dest;
 }
 
 #undef memmove
-void *memmove(void *dest, const void *src, size_t n)
+void * __attribute__((weak))
+memmove(void *dest, const void *src, size_t n)
 {
 	u8 *d = dest;
 	const u8 *s = src;
 	size_t i;
 
 	if (d <= s)
 		return memcpy(d, s, n);
 
 	for (i = n; i > 0; i--)
 		d[i - 1] = s[i - 1];
 	return dest;
 }
 
 #undef memcmp
-int memcmp(const void *s1, const void *s2, size_t n)
+int __attribute__((weak))
+memcmp(const void *s1, const void *s2, size_t n)
 {
 	const u8 *p1 = s1;
 	const u8 *p2 = s2;
 	size_t i;
 
 	for (i = 0; i < n; i++) {
 		if (p1[i] != p2[i])
 			return (int)p1[i] - (int)p2[i];
 	}
 	return 0;
 }
 #endif /* FREESTANDING */
+
+#ifdef LIBDEFLATE_ENABLE_ASSERTIONS
+#include <stdio.h>
+#include <stdlib.h>
+void
+libdeflate_assertion_failed(const char *expr, const char *file, int line)
+{
+	fprintf(stderr, "Assertion failed: %s at %s:%d\n", expr, file, line);
+	abort();
+}
+#endif /* LIBDEFLATE_ENABLE_ASSERTIONS */
```

### Comparing `deflate-0.3.0/libdeflate/lib/x86/cpu_features.c` & `deflate-0.4.0/libdeflate/lib/x86/cpu_features.c`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * x86/cpu_features.c - feature detection for x86 processors
+ * x86/cpu_features.c - feature detection for x86 CPUs
  *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
@@ -24,80 +24,89 @@
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "../cpu_features_common.h" /* must be included first */
 #include "cpu_features.h"
 
-#if X86_CPU_FEATURES_ENABLED
-
-volatile u32 _cpu_features = 0;
+#if HAVE_DYNAMIC_X86_CPU_FEATURES
 
 /* With old GCC versions we have to manually save and restore the x86_32 PIC
  * register (ebx).  See: https://gcc.gnu.org/bugzilla/show_bug.cgi?id=47602  */
-#if defined(__i386__) && defined(__PIC__)
+#if defined(ARCH_X86_32) && defined(__PIC__)
 #  define EBX_CONSTRAINT "=&r"
 #else
 #  define EBX_CONSTRAINT "=b"
 #endif
 
 /* Execute the CPUID instruction.  */
 static inline void
 cpuid(u32 leaf, u32 subleaf, u32 *a, u32 *b, u32 *c, u32 *d)
 {
+#ifdef _MSC_VER
+	int result[4];
+
+	__cpuidex(result, leaf, subleaf);
+	*a = result[0];
+	*b = result[1];
+	*c = result[2];
+	*d = result[3];
+#else
 	__asm__(".ifnc %%ebx, %1; mov  %%ebx, %1; .endif\n"
 		"cpuid                                  \n"
 		".ifnc %%ebx, %1; xchg %%ebx, %1; .endif\n"
 		: "=a" (*a), EBX_CONSTRAINT (*b), "=c" (*c), "=d" (*d)
 		: "a" (leaf), "c" (subleaf));
+#endif
 }
 
 /* Read an extended control register.  */
 static inline u64
 read_xcr(u32 index)
 {
+#ifdef _MSC_VER
+	return _xgetbv(index);
+#else
 	u32 edx, eax;
 
 	/* Execute the "xgetbv" instruction.  Old versions of binutils do not
 	 * recognize this instruction, so list the raw bytes instead.  */
 	__asm__ (".byte 0x0f, 0x01, 0xd0" : "=d" (edx), "=a" (eax) : "c" (index));
 
 	return ((u64)edx << 32) | eax;
+#endif
 }
 
 #undef BIT
 #define BIT(nr)			(1UL << (nr))
 
 #define XCR0_BIT_SSE		BIT(1)
 #define XCR0_BIT_AVX		BIT(2)
-#define XCR0_BIT_OPMASK		BIT(5)
-#define XCR0_BIT_ZMM_HI256	BIT(6)
-#define XCR0_BIT_HI16_ZMM	BIT(7)
 
 #define IS_SET(reg, nr)		((reg) & BIT(nr))
 #define IS_ALL_SET(reg, mask)	(((reg) & (mask)) == (mask))
 
 static const struct cpu_feature x86_cpu_feature_table[] = {
 	{X86_CPU_FEATURE_SSE2,		"sse2"},
 	{X86_CPU_FEATURE_PCLMUL,	"pclmul"},
 	{X86_CPU_FEATURE_AVX,		"avx"},
 	{X86_CPU_FEATURE_AVX2,		"avx2"},
 	{X86_CPU_FEATURE_BMI2,		"bmi2"},
-	{X86_CPU_FEATURE_AVX512BW,	"avx512bw"},
 };
 
-/* Initialize _cpu_features with bits for interesting processor features. */
-void setup_cpu_features(void)
+volatile u32 libdeflate_x86_cpu_features = 0;
+
+/* Initialize libdeflate_x86_cpu_features. */
+void libdeflate_init_x86_cpu_features(void)
 {
 	u32 features = 0;
 	u32 dummy1, dummy2, dummy3, dummy4;
 	u32 max_function;
 	u32 features_1, features_2, features_3, features_4;
 	bool os_avx_support = false;
-	bool os_avx512_support = false;
 
 	/* Get maximum supported function  */
 	cpuid(0, 0, &max_function, &dummy2, &dummy3, &dummy4);
 	if (max_function < 1)
 		goto out;
 
 	/* Standard feature flags  */
@@ -111,21 +120,14 @@
 
 	if (IS_SET(features_2, 27)) { /* OSXSAVE set? */
 		u64 xcr0 = read_xcr(0);
 
 		os_avx_support = IS_ALL_SET(xcr0,
 					    XCR0_BIT_SSE |
 					    XCR0_BIT_AVX);
-
-		os_avx512_support = IS_ALL_SET(xcr0,
-					       XCR0_BIT_SSE |
-					       XCR0_BIT_AVX |
-					       XCR0_BIT_OPMASK |
-					       XCR0_BIT_ZMM_HI256 |
-					       XCR0_BIT_HI16_ZMM);
 	}
 
 	if (os_avx_support && IS_SET(features_2, 28))
 		features |= X86_CPU_FEATURE_AVX;
 
 	if (max_function < 7)
 		goto out;
@@ -135,18 +137,15 @@
 
 	if (os_avx_support && IS_SET(features_3, 5))
 		features |= X86_CPU_FEATURE_AVX2;
 
 	if (IS_SET(features_3, 8))
 		features |= X86_CPU_FEATURE_BMI2;
 
-	if (os_avx512_support && IS_SET(features_3, 30))
-		features |= X86_CPU_FEATURE_AVX512BW;
-
 out:
 	disable_cpu_features_for_testing(&features, x86_cpu_feature_table,
 					 ARRAY_LEN(x86_cpu_feature_table));
 
-	_cpu_features = features | X86_CPU_FEATURES_KNOWN;
+	libdeflate_x86_cpu_features = features | X86_CPU_FEATURES_KNOWN;
 }
 
-#endif /* X86_CPU_FEATURES_ENABLED */
+#endif /* HAVE_DYNAMIC_X86_CPU_FEATURES */
```

### Comparing `deflate-0.3.0/libdeflate/lib/x86/crc32_impl.h` & `deflate-0.4.0/libdeflate/lib/x86/crc32_impl.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * x86/crc32_impl.h - x86 implementations of CRC-32 checksum algorithm
+ * x86/crc32_impl.h - x86 implementations of the gzip CRC-32 algorithm
  *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
@@ -21,67 +21,76 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
+#ifndef LIB_X86_CRC32_IMPL_H
+#define LIB_X86_CRC32_IMPL_H
+
 #include "cpu_features.h"
 
-/*
- * Include the PCLMUL/AVX implementation?  Although our PCLMUL-optimized CRC-32
- * function doesn't use any AVX intrinsics specifically, it can benefit a lot
- * from being compiled for an AVX target: on Skylake, ~16700 MB/s vs. ~10100
- * MB/s.  I expect this is related to the PCLMULQDQ instructions being assembled
- * in the newer three-operand form rather than the older two-operand form.
- *
- * Note: this is only needed if __AVX__ is *not* defined, since otherwise the
- * "regular" PCLMUL implementation would already be AVX enabled.
- */
-#undef DISPATCH_PCLMUL_AVX
-#if !defined(DEFAULT_IMPL) && !defined(__AVX__) &&	\
-	X86_CPU_FEATURES_ENABLED && COMPILER_SUPPORTS_AVX_TARGET &&	\
-	(defined(__PCLMUL__) || COMPILER_SUPPORTS_PCLMUL_TARGET_INTRINSICS)
-#  define FUNCNAME		crc32_pclmul_avx
-#  define FUNCNAME_ALIGNED	crc32_pclmul_avx_aligned
-#  define ATTRIBUTES		__attribute__((target("pclmul,avx")))
-#  define DISPATCH		1
-#  define DISPATCH_PCLMUL_AVX	1
+/* PCLMUL implementation */
+#if HAVE_PCLMUL_INTRIN
+#  define crc32_x86_pclmul	crc32_x86_pclmul
+#  define SUFFIX			 _pclmul
+#  if HAVE_PCLMUL_NATIVE
+#    define ATTRIBUTES
+#  else
+#    define ATTRIBUTES		_target_attribute("pclmul")
+#  endif
+#  define FOLD_PARTIAL_VECS	0
 #  include "crc32_pclmul_template.h"
 #endif
 
-/* PCLMUL implementation */
-#undef DISPATCH_PCLMUL
-#if !defined(DEFAULT_IMPL) &&	\
-	(defined(__PCLMUL__) || (X86_CPU_FEATURES_ENABLED &&	\
-				 COMPILER_SUPPORTS_PCLMUL_TARGET_INTRINSICS))
-#  define FUNCNAME		crc32_pclmul
-#  define FUNCNAME_ALIGNED	crc32_pclmul_aligned
-#  ifdef __PCLMUL__
+/*
+ * PCLMUL/AVX implementation.  This implementation has two benefits over the
+ * regular PCLMUL one.  First, simply compiling against the AVX target can
+ * improve performance significantly (e.g. 10100 MB/s to 16700 MB/s on Skylake)
+ * without actually using any AVX intrinsics, probably due to the availability
+ * of non-destructive VEX-encoded instructions.  Second, AVX support implies
+ * SSSE3 and SSE4.1 support, and we can use SSSE3 and SSE4.1 intrinsics for
+ * efficient handling of partial blocks.  (We *could* compile a variant with
+ * PCLMUL+SSSE3+SSE4.1 w/o AVX, but for simplicity we don't currently bother.)
+ *
+ * FIXME: with MSVC, this isn't actually compiled with AVX code generation
+ * enabled yet.  That would require that this be moved to its own .c file.
+ */
+#if HAVE_PCLMUL_INTRIN && HAVE_AVX_INTRIN
+#  define crc32_x86_pclmul_avx	crc32_x86_pclmul_avx
+#  define SUFFIX			 _pclmul_avx
+#  if HAVE_PCLMUL_NATIVE && HAVE_AVX_NATIVE
 #    define ATTRIBUTES
-#    define DEFAULT_IMPL	crc32_pclmul
 #  else
-#    define ATTRIBUTES		__attribute__((target("pclmul")))
-#    define DISPATCH		1
-#    define DISPATCH_PCLMUL	1
+#    define ATTRIBUTES		_target_attribute("pclmul,avx")
 #  endif
+#  define FOLD_PARTIAL_VECS	1
 #  include "crc32_pclmul_template.h"
 #endif
 
-#ifdef DISPATCH
+/*
+ * If the best implementation is statically available, use it unconditionally.
+ * Otherwise choose the best implementation at runtime.
+ */
+#if defined(crc32_x86_pclmul_avx) && HAVE_PCLMUL_NATIVE && HAVE_AVX_NATIVE
+#define DEFAULT_IMPL	crc32_x86_pclmul_avx
+#else
 static inline crc32_func_t
 arch_select_crc32_func(void)
 {
-	u32 features = get_cpu_features();
+	const u32 features MAYBE_UNUSED = get_x86_cpu_features();
 
-#ifdef DISPATCH_PCLMUL_AVX
-	if ((features & X86_CPU_FEATURE_PCLMUL) &&
-	    (features & X86_CPU_FEATURE_AVX))
-		return crc32_pclmul_avx;
+#ifdef crc32_x86_pclmul_avx
+	if (HAVE_PCLMUL(features) && HAVE_AVX(features))
+		return crc32_x86_pclmul_avx;
 #endif
-#ifdef DISPATCH_PCLMUL
-	if (features & X86_CPU_FEATURE_PCLMUL)
-		return crc32_pclmul;
+#ifdef crc32_x86_pclmul
+	if (HAVE_PCLMUL(features))
+		return crc32_x86_pclmul;
 #endif
 	return NULL;
 }
-#endif /* DISPATCH */
+#define arch_select_crc32_func	arch_select_crc32_func
+#endif
+
+#endif /* LIB_X86_CRC32_IMPL_H */
```

### Comparing `deflate-0.3.0/libdeflate/lib/x86/matchfinder_impl.h` & `deflate-0.4.0/libdeflate/lib/x86/matchfinder_impl.h`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,20 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
-#ifdef __AVX2__
+#ifndef LIB_X86_MATCHFINDER_IMPL_H
+#define LIB_X86_MATCHFINDER_IMPL_H
+
+#include "cpu_features.h"
+
+#if HAVE_AVX2_NATIVE
 #  include <immintrin.h>
 static forceinline void
 matchfinder_init_avx2(mf_pos_t *data, size_t size)
 {
 	__m256i *p = (__m256i *)data;
 	__m256i v = _mm256_set1_epi16(MATCHFINDER_INITVAL);
 
@@ -66,15 +71,15 @@
 		p[3] = _mm256_adds_epi16(p[3], v);
 		p += 4;
 		size -= 4 * sizeof(*p);
 	} while (size != 0);
 }
 #define matchfinder_rebase matchfinder_rebase_avx2
 
-#elif defined(__SSE2__)
+#elif HAVE_SSE2_NATIVE
 #  include <emmintrin.h>
 static forceinline void
 matchfinder_init_sse2(mf_pos_t *data, size_t size)
 {
 	__m128i *p = (__m128i *)data;
 	__m128i v = _mm_set1_epi16(MATCHFINDER_INITVAL);
 
@@ -110,8 +115,10 @@
 		p[2] = _mm_adds_epi16(p[2], v);
 		p[3] = _mm_adds_epi16(p[3], v);
 		p += 4;
 		size -= 4 * sizeof(*p);
 	} while (size != 0);
 }
 #define matchfinder_rebase matchfinder_rebase_sse2
-#endif /* __SSE2__ */
+#endif /* HAVE_SSE2_NATIVE */
+
+#endif /* LIB_X86_MATCHFINDER_IMPL_H */
```

### Comparing `deflate-0.3.0/libdeflate/lib/zlib_compress.c` & `deflate-0.4.0/libdeflate/lib/zlib_compress.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * zlib_compress.c - compress with a zlib wrapper
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,20 +22,17 @@
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "deflate_compress.h"
-#include "unaligned.h"
 #include "zlib_constants.h"
 
-#include "libdeflate.h"
-
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_zlib_compress(struct libdeflate_compressor *c,
 			 const void *in, size_t in_nbytes,
 			 void *out, size_t out_nbytes_avail)
 {
 	u8 *out_next = out;
 	u16 hdr;
 	unsigned compression_level;
@@ -45,15 +40,15 @@
 	size_t deflate_size;
 
 	if (out_nbytes_avail <= ZLIB_MIN_OVERHEAD)
 		return 0;
 
 	/* 2 byte header: CMF and FLG  */
 	hdr = (ZLIB_CM_DEFLATE << 8) | (ZLIB_CINFO_32K_WINDOW << 12);
-	compression_level = deflate_get_compression_level(c);
+	compression_level = libdeflate_get_compression_level(c);
 	if (compression_level < 2)
 		level_hint = ZLIB_FASTEST_COMPRESSION;
 	else if (compression_level < 6)
 		level_hint = ZLIB_FAST_COMPRESSION;
 	else if (compression_level < 8)
 		level_hint = ZLIB_DEFAULT_COMPRESSION;
 	else
@@ -74,14 +69,14 @@
 	/* ADLER32  */
 	put_unaligned_be32(libdeflate_adler32(1, in, in_nbytes), out_next);
 	out_next += 4;
 
 	return out_next - (u8 *)out;
 }
 
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_zlib_compress_bound(struct libdeflate_compressor *c,
 			       size_t in_nbytes)
 {
 	return ZLIB_MIN_OVERHEAD +
 	       libdeflate_deflate_compress_bound(c, in_nbytes);
 }
```

### Comparing `deflate-0.3.0/libdeflate/lib/zlib_decompress.c` & `deflate-0.4.0/libdeflate/lib/zlib_decompress.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /*
  * zlib_decompress.c - decompress with a zlib wrapper
  *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
- *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
  * copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -23,20 +21,18 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
-#include "unaligned.h"
+#include "lib_common.h"
 #include "zlib_constants.h"
 
-#include "libdeflate.h"
-
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_zlib_decompress_ex(struct libdeflate_decompressor *d,
 			      const void *in, size_t in_nbytes,
 			      void *out, size_t out_nbytes_avail,
 			      size_t *actual_in_nbytes_ret,
 			      size_t *actual_out_nbytes_ret)
 {
 	const u8 *in_next = in;
@@ -92,15 +88,15 @@
 
 	if (actual_in_nbytes_ret)
 		*actual_in_nbytes_ret = in_next - (u8 *)in;
 
 	return LIBDEFLATE_SUCCESS;
 }
 
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_zlib_decompress(struct libdeflate_decompressor *d,
 			   const void *in, size_t in_nbytes,
 			   void *out, size_t out_nbytes_avail,
 			   size_t *actual_out_nbytes_ret)
 {
 	return libdeflate_zlib_decompress_ex(d, in, in_nbytes,
 					     out, out_nbytes_avail,
```

### Comparing `deflate-0.3.0/libdeflate/libdeflate.h` & `deflate-0.4.0/libdeflate/libdeflate.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,38 @@
 /*
  * libdeflate.h - public header for libdeflate
  */
 
 #ifndef LIBDEFLATE_H
 #define LIBDEFLATE_H
 
+#include <stddef.h>
+#include <stdint.h>
+
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #define LIBDEFLATE_VERSION_MAJOR	1
-#define LIBDEFLATE_VERSION_MINOR	7
-#define LIBDEFLATE_VERSION_STRING	"1.7"
-
-#include <stddef.h>
-#include <stdint.h>
+#define LIBDEFLATE_VERSION_MINOR	18
+#define LIBDEFLATE_VERSION_STRING	"1.18"
 
 /*
- * On Windows, if you want to link to the DLL version of libdeflate, then
- * #define LIBDEFLATE_DLL.  Note that the calling convention is "stdcall".
- */
-#ifdef LIBDEFLATE_DLL
-#  ifdef BUILDING_LIBDEFLATE
-#    define LIBDEFLATEEXPORT	LIBEXPORT
-#  elif defined(_WIN32) || defined(__CYGWIN__)
-#    define LIBDEFLATEEXPORT	__declspec(dllimport)
+ * Users of libdeflate.dll on Windows can define LIBDEFLATE_DLL to cause
+ * __declspec(dllimport) to be used.  This should be done when it's easy to do.
+ * Otherwise it's fine to skip it, since it is a very minor performance
+ * optimization that is irrelevant for most use cases of libdeflate.
+ */
+#ifndef LIBDEFLATEAPI
+#  if defined(LIBDEFLATE_DLL) && (defined(_WIN32) || defined(__CYGWIN__))
+#    define LIBDEFLATEAPI	__declspec(dllimport)
+#  else
+#    define LIBDEFLATEAPI
 #  endif
 #endif
-#ifndef LIBDEFLATEEXPORT
-#  define LIBDEFLATEEXPORT
-#endif
-
-#if defined(_WIN32) && !defined(_WIN64)
-#  define LIBDEFLATEAPI_ABI	__stdcall
-#else
-#  define LIBDEFLATEAPI_ABI
-#endif
-
-#if defined(BUILDING_LIBDEFLATE) && defined(__GNUC__) && \
-	defined(_WIN32) && !defined(_WIN64)
-    /*
-     * On 32-bit Windows, gcc assumes 16-byte stack alignment but MSVC only 4.
-     * Realign the stack when entering libdeflate to avoid crashing in SSE/AVX
-     * code when called from an MSVC-compiled application.
-     */
-#  define LIBDEFLATEAPI_STACKALIGN	__attribute__((force_align_arg_pointer))
-#else
-#  define LIBDEFLATEAPI_STACKALIGN
-#endif
-
-#define LIBDEFLATEAPI	LIBDEFLATEAPI_ABI LIBDEFLATEAPI_STACKALIGN
 
 /* ========================================================================== */
 /*                             Compression                                    */
 /* ========================================================================== */
 
 struct libdeflate_compressor;
 
@@ -71,38 +50,62 @@
  * Note: for compression, the sliding window size is defined at compilation time
  * to 32768, the largest size permissible in the DEFLATE format.  It cannot be
  * changed at runtime.
  *
  * A single compressor is not safe to use by multiple threads concurrently.
  * However, different threads may use different compressors concurrently.
  */
-LIBDEFLATEEXPORT struct libdeflate_compressor * LIBDEFLATEAPI
+LIBDEFLATEAPI struct libdeflate_compressor *
 libdeflate_alloc_compressor(int compression_level);
 
 /*
  * libdeflate_deflate_compress() performs raw DEFLATE compression on a buffer of
- * data.  The function attempts to compress 'in_nbytes' bytes of data located at
- * 'in' and write the results to 'out', which has space for 'out_nbytes_avail'
- * bytes.  The return value is the compressed size in bytes, or 0 if the data
- * could not be compressed to 'out_nbytes_avail' bytes or fewer.
+ * data.  It attempts to compress 'in_nbytes' bytes of data located at 'in' and
+ * write the result to 'out', which has space for 'out_nbytes_avail' bytes.  The
+ * return value is the compressed size in bytes, or 0 if the data could not be
+ * compressed to 'out_nbytes_avail' bytes or fewer (but see note below).
+ *
+ * If compression is successful, then the output data is guaranteed to be a
+ * valid DEFLATE stream that decompresses to the input data.  No other
+ * guarantees are made about the output data.  Notably, different versions of
+ * libdeflate can produce different compressed data for the same uncompressed
+ * data, even at the same compression level.  Do ***NOT*** do things like
+ * writing tests that compare compressed data to a golden output, as this can
+ * break when libdeflate is updated.  (This property isn't specific to
+ * libdeflate; the same is true for zlib and other compression libraries too.)
+ *
+ * Note: due to a performance optimization, libdeflate_deflate_compress()
+ * currently needs a small amount of slack space at the end of the output
+ * buffer.  As a result, it can't actually report compressed sizes very close to
+ * 'out_nbytes_avail'.  This doesn't matter in real-world use cases, and
+ * libdeflate_deflate_compress_bound() already includes the slack space.
+ * However, it does mean that testing code that redundantly compresses data
+ * using an exact-sized output buffer won't work as might be expected:
+ *
+ *	out_nbytes = libdeflate_deflate_compress(c, in, in_nbytes, out,
+ *						 libdeflate_deflate_compress_bound(in_nbytes));
+ *	// The following assertion will fail.
+ *	assert(libdeflate_deflate_compress(c, in, in_nbytes, out, out_nbytes) != 0);
+ *
+ * To avoid this, either don't write tests like the above, or make sure to
+ * include at least 9 bytes of slack space in 'out_nbytes_avail'.
  */
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_deflate_compress(struct libdeflate_compressor *compressor,
 			    const void *in, size_t in_nbytes,
 			    void *out, size_t out_nbytes_avail);
 
 /*
  * libdeflate_deflate_compress_bound() returns a worst-case upper bound on the
  * number of bytes of compressed data that may be produced by compressing any
  * buffer of length less than or equal to 'in_nbytes' using
- * libdeflate_deflate_compress() with the specified compressor.  Mathematically,
- * this bound will necessarily be a number greater than or equal to 'in_nbytes'.
- * It may be an overestimate of the true upper bound.  The return value is
- * guaranteed to be the same for all invocations with the same compressor and
- * same 'in_nbytes'.
+ * libdeflate_deflate_compress() with the specified compressor.  This bound will
+ * necessarily be a number greater than or equal to 'in_nbytes'.  It may be an
+ * overestimate of the true upper bound.  The return value is guaranteed to be
+ * the same for all invocations with the same compressor and same 'in_nbytes'.
  *
  * As a special case, 'compressor' may be NULL.  This causes the bound to be
  * taken across *any* libdeflate_compressor that could ever be allocated with
  * this build of the library, with any options.
  *
  * Note that this function is not necessary in many applications.  With
  * block-based compression, it is usually preferable to separately store the
@@ -111,60 +114,60 @@
  * need to know the worst-case compressed size, since the maximum number of
  * bytes of compressed data that may be used would always be one less than the
  * input length.  You can just pass a buffer of that size to
  * libdeflate_deflate_compress() and store the data uncompressed if
  * libdeflate_deflate_compress() returns 0, indicating that the compressed data
  * did not fit into the provided output buffer.
  */
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_deflate_compress_bound(struct libdeflate_compressor *compressor,
 				  size_t in_nbytes);
 
 /*
- * Like libdeflate_deflate_compress(), but stores the data in the zlib wrapper
- * format.
+ * Like libdeflate_deflate_compress(), but uses the zlib wrapper format instead
+ * of raw DEFLATE.
  */
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_zlib_compress(struct libdeflate_compressor *compressor,
 			 const void *in, size_t in_nbytes,
 			 void *out, size_t out_nbytes_avail);
 
 /*
  * Like libdeflate_deflate_compress_bound(), but assumes the data will be
  * compressed with libdeflate_zlib_compress() rather than with
  * libdeflate_deflate_compress().
  */
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_zlib_compress_bound(struct libdeflate_compressor *compressor,
 			       size_t in_nbytes);
 
 /*
- * Like libdeflate_deflate_compress(), but stores the data in the gzip wrapper
- * format.
+ * Like libdeflate_deflate_compress(), but uses the gzip wrapper format instead
+ * of raw DEFLATE.
  */
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_gzip_compress(struct libdeflate_compressor *compressor,
 			 const void *in, size_t in_nbytes,
 			 void *out, size_t out_nbytes_avail);
 
 /*
  * Like libdeflate_deflate_compress_bound(), but assumes the data will be
  * compressed with libdeflate_gzip_compress() rather than with
  * libdeflate_deflate_compress().
  */
-LIBDEFLATEEXPORT size_t LIBDEFLATEAPI
+LIBDEFLATEAPI size_t
 libdeflate_gzip_compress_bound(struct libdeflate_compressor *compressor,
 			       size_t in_nbytes);
 
 /*
  * libdeflate_free_compressor() frees a compressor that was allocated with
  * libdeflate_alloc_compressor().  If a NULL pointer is passed in, no action is
  * taken.
  */
-LIBDEFLATEEXPORT void LIBDEFLATEAPI
+LIBDEFLATEAPI void
 libdeflate_free_compressor(struct libdeflate_compressor *compressor);
 
 /* ========================================================================== */
 /*                             Decompression                                  */
 /* ========================================================================== */
 
 struct libdeflate_decompressor;
@@ -177,46 +180,45 @@
  * This function takes no parameters, and the returned decompressor is valid for
  * decompressing data that was compressed at any compression level and with any
  * sliding window size.
  *
  * A single decompressor is not safe to use by multiple threads concurrently.
  * However, different threads may use different decompressors concurrently.
  */
-LIBDEFLATEEXPORT struct libdeflate_decompressor * LIBDEFLATEAPI
+LIBDEFLATEAPI struct libdeflate_decompressor *
 libdeflate_alloc_decompressor(void);
 
 /*
  * Result of a call to libdeflate_deflate_decompress(),
  * libdeflate_zlib_decompress(), or libdeflate_gzip_decompress().
  */
 enum libdeflate_result {
 	/* Decompression was successful.  */
 	LIBDEFLATE_SUCCESS = 0,
 
-	/* Decompressed failed because the compressed data was invalid, corrupt,
-	 * or otherwise unsupported.  */
+	/* Decompression failed because the compressed data was invalid,
+	 * corrupt, or otherwise unsupported.  */
 	LIBDEFLATE_BAD_DATA = 1,
 
 	/* A NULL 'actual_out_nbytes_ret' was provided, but the data would have
 	 * decompressed to fewer than 'out_nbytes_avail' bytes.  */
 	LIBDEFLATE_SHORT_OUTPUT = 2,
 
 	/* The data would have decompressed to more than 'out_nbytes_avail'
 	 * bytes.  */
 	LIBDEFLATE_INSUFFICIENT_SPACE = 3,
 };
 
 /*
- * libdeflate_deflate_decompress() decompresses the DEFLATE-compressed stream
- * from the buffer 'in' with compressed size up to 'in_nbytes' bytes.  The
- * uncompressed data is written to 'out', a buffer with size 'out_nbytes_avail'
- * bytes.  If decompression succeeds, then 0 (LIBDEFLATE_SUCCESS) is returned.
- * Otherwise, a nonzero result code such as LIBDEFLATE_BAD_DATA is returned.  If
- * a nonzero result code is returned, then the contents of the output buffer are
- * undefined.
+ * libdeflate_deflate_decompress() decompresses a DEFLATE stream from the buffer
+ * 'in' with compressed size up to 'in_nbytes' bytes.  The uncompressed data is
+ * written to 'out', a buffer with size 'out_nbytes_avail' bytes.  If
+ * decompression succeeds, then 0 (LIBDEFLATE_SUCCESS) is returned.  Otherwise,
+ * a nonzero result code such as LIBDEFLATE_BAD_DATA is returned, and the
+ * contents of the output buffer are undefined.
  *
  * Decompression stops at the end of the DEFLATE stream (as indicated by the
  * BFINAL flag), even if it is actually shorter than 'in_nbytes' bytes.
  *
  * libdeflate_deflate_decompress() can be used in cases where the actual
  * uncompressed size is known (recommended) or unknown (not recommended):
  *
@@ -233,133 +235,133 @@
  *     or equal to 'out_nbytes_avail' bytes, then
  *     libdeflate_deflate_decompress() will write the actual uncompressed size
  *     to *actual_out_nbytes_ret and return 0 (LIBDEFLATE_SUCCESS).  Otherwise,
  *     it will return LIBDEFLATE_INSUFFICIENT_SPACE if the provided buffer was
  *     not large enough but no other problems were encountered, or another
  *     nonzero result code if decompression failed for another reason.
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_deflate_decompress(struct libdeflate_decompressor *decompressor,
 			      const void *in, size_t in_nbytes,
 			      void *out, size_t out_nbytes_avail,
 			      size_t *actual_out_nbytes_ret);
 
 /*
  * Like libdeflate_deflate_decompress(), but adds the 'actual_in_nbytes_ret'
  * argument.  If decompression succeeds and 'actual_in_nbytes_ret' is not NULL,
  * then the actual compressed size of the DEFLATE stream (aligned to the next
  * byte boundary) is written to *actual_in_nbytes_ret.
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_deflate_decompress_ex(struct libdeflate_decompressor *decompressor,
 				 const void *in, size_t in_nbytes,
 				 void *out, size_t out_nbytes_avail,
 				 size_t *actual_in_nbytes_ret,
 				 size_t *actual_out_nbytes_ret);
 
 /*
  * Like libdeflate_deflate_decompress(), but assumes the zlib wrapper format
  * instead of raw DEFLATE.
  *
  * Decompression will stop at the end of the zlib stream, even if it is shorter
  * than 'in_nbytes'.  If you need to know exactly where the zlib stream ended,
  * use libdeflate_zlib_decompress_ex().
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_zlib_decompress(struct libdeflate_decompressor *decompressor,
 			   const void *in, size_t in_nbytes,
 			   void *out, size_t out_nbytes_avail,
 			   size_t *actual_out_nbytes_ret);
 
 /*
  * Like libdeflate_zlib_decompress(), but adds the 'actual_in_nbytes_ret'
  * argument.  If 'actual_in_nbytes_ret' is not NULL and the decompression
  * succeeds (indicating that the first zlib-compressed stream in the input
  * buffer was decompressed), then the actual number of input bytes consumed is
  * written to *actual_in_nbytes_ret.
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_zlib_decompress_ex(struct libdeflate_decompressor *decompressor,
 			      const void *in, size_t in_nbytes,
 			      void *out, size_t out_nbytes_avail,
 			      size_t *actual_in_nbytes_ret,
 			      size_t *actual_out_nbytes_ret);
 
 /*
  * Like libdeflate_deflate_decompress(), but assumes the gzip wrapper format
  * instead of raw DEFLATE.
  *
  * If multiple gzip-compressed members are concatenated, then only the first
  * will be decompressed.  Use libdeflate_gzip_decompress_ex() if you need
  * multi-member support.
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_gzip_decompress(struct libdeflate_decompressor *decompressor,
 			   const void *in, size_t in_nbytes,
 			   void *out, size_t out_nbytes_avail,
 			   size_t *actual_out_nbytes_ret);
 
 /*
  * Like libdeflate_gzip_decompress(), but adds the 'actual_in_nbytes_ret'
  * argument.  If 'actual_in_nbytes_ret' is not NULL and the decompression
  * succeeds (indicating that the first gzip-compressed member in the input
  * buffer was decompressed), then the actual number of input bytes consumed is
  * written to *actual_in_nbytes_ret.
  */
-LIBDEFLATEEXPORT enum libdeflate_result LIBDEFLATEAPI
+LIBDEFLATEAPI enum libdeflate_result
 libdeflate_gzip_decompress_ex(struct libdeflate_decompressor *decompressor,
 			      const void *in, size_t in_nbytes,
 			      void *out, size_t out_nbytes_avail,
 			      size_t *actual_in_nbytes_ret,
 			      size_t *actual_out_nbytes_ret);
 
 /*
  * libdeflate_free_decompressor() frees a decompressor that was allocated with
  * libdeflate_alloc_decompressor().  If a NULL pointer is passed in, no action
  * is taken.
  */
-LIBDEFLATEEXPORT void LIBDEFLATEAPI
+LIBDEFLATEAPI void
 libdeflate_free_decompressor(struct libdeflate_decompressor *decompressor);
 
 /* ========================================================================== */
 /*                                Checksums                                   */
 /* ========================================================================== */
 
 /*
  * libdeflate_adler32() updates a running Adler-32 checksum with 'len' bytes of
  * data and returns the updated checksum.  When starting a new checksum, the
  * required initial value for 'adler' is 1.  This value is also returned when
  * 'buffer' is specified as NULL.
  */
-LIBDEFLATEEXPORT uint32_t LIBDEFLATEAPI
+LIBDEFLATEAPI uint32_t
 libdeflate_adler32(uint32_t adler, const void *buffer, size_t len);
 
 
 /*
  * libdeflate_crc32() updates a running CRC-32 checksum with 'len' bytes of data
  * and returns the updated checksum.  When starting a new checksum, the required
  * initial value for 'crc' is 0.  This value is also returned when 'buffer' is
  * specified as NULL.
  */
-LIBDEFLATEEXPORT uint32_t LIBDEFLATEAPI
+LIBDEFLATEAPI uint32_t
 libdeflate_crc32(uint32_t crc, const void *buffer, size_t len);
 
 /* ========================================================================== */
 /*                           Custom memory allocator                          */
 /* ========================================================================== */
 
 /*
  * Install a custom memory allocator which libdeflate will use for all memory
  * allocations.  'malloc_func' is a function that must behave like malloc(), and
  * 'free_func' is a function that must behave like free().
  *
  * There must not be any libdeflate_compressor or libdeflate_decompressor
  * structures in existence when calling this function.
  */
-LIBDEFLATEEXPORT void LIBDEFLATEAPI
+LIBDEFLATEAPI void
 libdeflate_set_memory_allocator(void *(*malloc_func)(size_t),
 				void (*free_func)(void *));
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `deflate-0.3.0/libdeflate/programs/benchmark.c` & `deflate-0.4.0/libdeflate/programs/benchmark.c`

 * *Files 4% similar despite different names*

```diff
@@ -25,29 +25,29 @@
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "test_util.h"
 
 static const tchar *const optstring = T("0::1::2::3::4::5::6::7::8::9::C:D:eghs:VYZz");
 
-enum wrapper {
-	NO_WRAPPER,
-	ZLIB_WRAPPER,
-	GZIP_WRAPPER,
+enum format {
+	DEFLATE_FORMAT,
+	ZLIB_FORMAT,
+	GZIP_FORMAT,
 };
 
 struct compressor {
 	int level;
-	enum wrapper wrapper;
+	enum format format;
 	const struct engine *engine;
 	void *private;
 };
 
 struct decompressor {
-	enum wrapper wrapper;
+	enum format format;
 	const struct engine *engine;
 	void *private;
 };
 
 struct engine {
 	const tchar *name;
 
@@ -71,33 +71,33 @@
 	c->private = alloc_compressor(c->level);
 	return c->private != NULL;
 }
 
 static size_t
 libdeflate_engine_compress_bound(struct compressor *c, size_t in_nbytes)
 {
-	switch (c->wrapper) {
-	case ZLIB_WRAPPER:
+	switch (c->format) {
+	case ZLIB_FORMAT:
 		return libdeflate_zlib_compress_bound(c->private, in_nbytes);
-	case GZIP_WRAPPER:
+	case GZIP_FORMAT:
 		return libdeflate_gzip_compress_bound(c->private, in_nbytes);
 	default:
 		return libdeflate_deflate_compress_bound(c->private, in_nbytes);
 	}
 }
 
 static size_t
 libdeflate_engine_compress(struct compressor *c, const void *in,
 			   size_t in_nbytes, void *out, size_t out_nbytes_avail)
 {
-	switch (c->wrapper) {
-	case ZLIB_WRAPPER:
+	switch (c->format) {
+	case ZLIB_FORMAT:
 		return libdeflate_zlib_compress(c->private, in, in_nbytes,
 						out, out_nbytes_avail);
-	case GZIP_WRAPPER:
+	case GZIP_FORMAT:
 		return libdeflate_gzip_compress(c->private, in, in_nbytes,
 						out, out_nbytes_avail);
 	default:
 		return libdeflate_deflate_compress(c->private, in, in_nbytes,
 						   out, out_nbytes_avail);
 	}
 }
@@ -115,19 +115,19 @@
 	return d->private != NULL;
 }
 
 static bool
 libdeflate_engine_decompress(struct decompressor *d, const void *in,
 			     size_t in_nbytes, void *out, size_t out_nbytes)
 {
-	switch (d->wrapper) {
-	case ZLIB_WRAPPER:
+	switch (d->format) {
+	case ZLIB_FORMAT:
 		return !libdeflate_zlib_decompress(d->private, in, in_nbytes,
 						   out, out_nbytes, NULL);
-	case GZIP_WRAPPER:
+	case GZIP_FORMAT:
 		return !libdeflate_gzip_decompress(d->private, in, in_nbytes,
 						   out, out_nbytes, NULL);
 	default:
 		return !libdeflate_deflate_decompress(d->private, in, in_nbytes,
 						      out, out_nbytes, NULL);
 	}
 }
@@ -150,21 +150,21 @@
 	.decompress		= libdeflate_engine_decompress,
 	.destroy_decompressor	= libdeflate_engine_destroy_decompressor,
 };
 
 /******************************************************************************/
 
 static int
-get_libz_window_bits(enum wrapper wrapper)
+get_libz_window_bits(enum format format)
 {
 	const int windowBits = 15;
-	switch (wrapper) {
-	case ZLIB_WRAPPER:
+	switch (format) {
+	case ZLIB_FORMAT:
 		return windowBits;
-	case GZIP_WRAPPER:
+	case GZIP_FORMAT:
 		return windowBits + 16;
 	default:
 		return -windowBits;
 	}
 }
 
 static bool
@@ -183,15 +183,15 @@
 
 	z->next_in = NULL;
 	z->avail_in = 0;
 	z->zalloc = NULL;
 	z->zfree = NULL;
 	z->opaque = NULL;
 	if (deflateInit2(z, c->level, Z_DEFLATED,
-			 get_libz_window_bits(c->wrapper),
+			 get_libz_window_bits(c->format),
 			 8, Z_DEFAULT_STRATEGY) != Z_OK)
 	{
 		msg("unable to initialize deflater");
 		free(z);
 		return false;
 	}
 
@@ -243,15 +243,15 @@
 		return false;
 
 	z->next_in = NULL;
 	z->avail_in = 0;
 	z->zalloc = NULL;
 	z->zfree = NULL;
 	z->opaque = NULL;
-	if (inflateInit2(z, get_libz_window_bits(d->wrapper)) != Z_OK) {
+	if (inflateInit2(z, get_libz_window_bits(d->format)) != Z_OK) {
 		msg("unable to initialize inflater");
 		free(z);
 		return false;
 	}
 
 	d->private = z;
 	return true;
@@ -314,19 +314,19 @@
 			return all_engines[i];
 	return NULL;
 }
 
 /******************************************************************************/
 
 static bool
-compressor_init(struct compressor *c, int level, enum wrapper wrapper,
+compressor_init(struct compressor *c, int level, enum format format,
 		const struct engine *engine)
 {
 	c->level = level;
-	c->wrapper = wrapper;
+	c->format = format;
 	c->engine = engine;
 	return engine->init_compressor(c);
 }
 
 static size_t
 compress_bound(struct compressor *c, size_t in_nbytes)
 {
@@ -344,18 +344,18 @@
 compressor_destroy(struct compressor *c)
 {
 	if (c->engine != NULL)
 		c->engine->destroy_compressor(c);
 }
 
 static bool
-decompressor_init(struct decompressor *d, enum wrapper wrapper,
+decompressor_init(struct decompressor *d, enum format format,
 		  const struct engine *engine)
 {
-	d->wrapper = wrapper;
+	d->format = format;
 	d->engine = engine;
 	return engine->init_decompressor(d);
 }
 
 static bool
 do_decompress(struct decompressor *d, const void *in, size_t in_nbytes,
 	      void *out, size_t out_nbytes)
@@ -397,19 +397,19 @@
 "  -0        no compression\n"
 "  -1        fastest (worst) compression\n"
 "  -6        medium compression (default)\n"
 "  -12       slowest (best) compression\n"
 "  -C ENGINE compression engine\n"
 "  -D ENGINE decompression engine\n"
 "  -e        allow chunks to be expanded (implied by -0)\n"
-"  -g        use gzip wrapper\n"
+"  -g        use gzip format instead of raw DEFLATE\n"
 "  -h        print this help\n"
 "  -s SIZE   chunk size\n"
 "  -V        show version and legal information\n"
-"  -z        use zlib wrapper\n"
+"  -z        use zlib format instead of raw DEFLATE\n"
 "\n", prog_invocation_name);
 
 	show_available_engines(fp);
 }
 
 static void
 show_version(void)
@@ -538,15 +538,15 @@
 }
 
 int
 tmain(int argc, tchar *argv[])
 {
 	u32 chunk_size = 1048576;
 	int level = 6;
-	enum wrapper wrapper = NO_WRAPPER;
+	enum format format = DEFLATE_FORMAT;
 	const struct engine *compress_engine = &DEFAULT_ENGINE;
 	const struct engine *decompress_engine = &DEFAULT_ENGINE;
 	bool allow_expansion = false;
 	struct compressor compressor = { 0 };
 	struct decompressor decompressor = { 0 };
 	size_t compressed_buf_size;
 	void *original_buf = NULL;
@@ -591,15 +591,15 @@
 				return 1;
 			}
 			break;
 		case 'e':
 			allow_expansion = true;
 			break;
 		case 'g':
-			wrapper = GZIP_WRAPPER;
+			format = GZIP_FORMAT;
 			break;
 		case 'h':
 			show_usage(stdout);
 			return 0;
 		case 's':
 			chunk_size = tstrtoul(toptarg, NULL, 10);
 			if (chunk_size == 0) {
@@ -613,32 +613,32 @@
 		case 'Y': /* deprecated, use '-C libz' instead */
 			compress_engine = &libz_engine;
 			break;
 		case 'Z': /* deprecated, use '-D libz' instead */
 			decompress_engine = &libz_engine;
 			break;
 		case 'z':
-			wrapper = ZLIB_WRAPPER;
+			format = ZLIB_FORMAT;
 			break;
 		default:
 			show_usage(stderr);
 			return 1;
 		}
 	}
 
 	argc -= toptind;
 	argv += toptind;
 
 	if (level == 0)
 		allow_expansion = true;
 
 	ret = -1;
-	if (!compressor_init(&compressor, level, wrapper, compress_engine))
+	if (!compressor_init(&compressor, level, format, compress_engine))
 		goto out;
-	if (!decompressor_init(&decompressor, wrapper, decompress_engine))
+	if (!decompressor_init(&decompressor, format, decompress_engine))
 		goto out;
 
 	if (allow_expansion)
 		compressed_buf_size = compress_bound(&compressor, chunk_size);
 	else
 		compressed_buf_size = chunk_size - 1;
 
@@ -656,20 +656,19 @@
 		argc = ARRAY_LEN(default_file_list);
 	} else {
 		for (i = 0; i < argc; i++)
 			if (argv[i][0] == '-' && argv[i][1] == '\0')
 				argv[i] = NULL;
 	}
 
-	printf("Benchmarking DEFLATE compression:\n");
+	printf("Benchmarking %s compression:\n",
+	       format == DEFLATE_FORMAT ? "DEFLATE" :
+	       format == ZLIB_FORMAT ? "zlib" : "gzip");
 	printf("\tCompression level: %d\n", level);
 	printf("\tChunk size: %"PRIu32"\n", chunk_size);
-	printf("\tWrapper: %s\n",
-	       wrapper == NO_WRAPPER ? "None" :
-	       wrapper == ZLIB_WRAPPER ? "zlib" : "gzip");
 	printf("\tCompression engine: %"TS"\n", compress_engine->name);
 	printf("\tDecompression engine: %"TS"\n", decompress_engine->name);
 
 	for (i = 0; i < argc; i++) {
 		struct file_stream in;
 
 		ret = xopen_for_read(argv[i], true, &in);
```

### Comparing `deflate-0.3.0/libdeflate/programs/checksum.c` & `deflate-0.4.0/libdeflate/programs/checksum.c`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,28 @@
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "test_util.h"
 
-static const tchar *const optstring = T("Ahs:tZ");
+static const tchar *const optstring = T("Ahm:s:tZ");
 
 static void
 show_usage(FILE *fp)
 {
 	fprintf(fp,
-"Usage: %"TS" [-A] [-h] [-s SIZE] [-t] [-Z] [FILE]...\n"
+"Usage: %"TS" [-A] [-h] [-m ALIGN] [-s SIZE] [-t] [-Z] [FILE]...\n"
 "Calculate Adler-32 or CRC-32 checksums of the specified FILEs.\n"
 "\n"
 "Options:\n"
 "  -A        use Adler-32 (default is CRC-32)\n"
 "  -h        print this help\n"
-"  -s SIZE   chunk size\n"
+"  -m ALIGN  misalign the buffer by ALIGN bytes\n"
+"  -s SIZE   chunk size in bytes\n"
 "  -t        show checksum speed, excluding I/O\n"
 "  -Z        use zlib implementation instead of libdeflate\n",
 	prog_invocation_name);
 }
 
 typedef u32 (*cksum_fn_t)(u32, const void *, size_t);
 
@@ -103,15 +104,17 @@
 
 int
 tmain(int argc, tchar *argv[])
 {
 	bool use_adler32 = false;
 	bool use_zlib_impl = false;
 	bool do_timing = false;
+	void *orig_buf = NULL;
 	void *buf;
+	size_t misalignment = 0;
 	size_t bufsize = 131072;
 	tchar *default_file_list[] = { NULL };
 	cksum_fn_t cksum;
 	int opt_char;
 	int i;
 	int ret;
 
@@ -121,17 +124,24 @@
 		switch (opt_char) {
 		case 'A':
 			use_adler32 = true;
 			break;
 		case 'h':
 			show_usage(stdout);
 			return 0;
+		case 'm':
+			misalignment = tstrtoul(toptarg, NULL, 10);
+			if (misalignment >= 4096) {
+				msg("invalid misalignment: \"%"TS"\"", toptarg);
+				return 1;
+			}
+			break;
 		case 's':
 			bufsize = tstrtoul(toptarg, NULL, 10);
-			if (bufsize == 0) {
+			if (bufsize == 0 || bufsize > SIZE_MAX / 2) {
 				msg("invalid chunk size: \"%"TS"\"", toptarg);
 				return 1;
 			}
 			break;
 		case 't':
 			do_timing = true;
 			break;
@@ -155,17 +165,18 @@
 	} else {
 		if (use_zlib_impl)
 			cksum = crc32_zlib;
 		else
 			cksum = crc32_libdeflate;
 	}
 
-	buf = xmalloc(bufsize);
-	if (buf == NULL)
+	orig_buf = xmalloc(bufsize + 4096 + misalignment);
+	if (orig_buf == NULL)
 		return 1;
+	buf = (u8 *)orig_buf + (-(uintptr_t)orig_buf % 4096) + misalignment;
 
 	if (argc == 0) {
 		argv = default_file_list;
 		argc = ARRAY_LEN(default_file_list);
 	} else {
 		for (i = 0; i < argc; i++)
 			if (argv[i][0] == '-' && argv[i][1] == '\0')
@@ -198,10 +209,10 @@
 		xclose(&in);
 
 		if (ret != 0)
 			goto out;
 	}
 	ret = 0;
 out:
-	free(buf);
+	free(orig_buf);
 	return -ret;
 }
```

### Comparing `deflate-0.3.0/libdeflate/programs/gzip.c` & `deflate-0.4.0/libdeflate/programs/gzip.c`

 * *Files 4% similar despite different names*

```diff
@@ -24,52 +24,62 @@
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #include "prog_util.h"
 
 #include <errno.h>
-#include <sys/types.h>
 #include <sys/stat.h>
 #ifdef _WIN32
 #  include <sys/utime.h>
 #else
 #  include <sys/time.h>
 #  include <unistd.h>
 #  include <utime.h>
 #endif
 
+#define GZIP_MIN_HEADER_SIZE	10
+#define GZIP_FOOTER_SIZE	8
+#define GZIP_MIN_OVERHEAD	(GZIP_MIN_HEADER_SIZE + GZIP_FOOTER_SIZE)
+#define GZIP_ID1		0x1F
+#define GZIP_ID2		0x8B
+
 struct options {
 	bool to_stdout;
 	bool decompress;
 	bool force;
 	bool keep;
+	bool test;
 	int compression_level;
 	const tchar *suffix;
 };
 
-static const tchar *const optstring = T("1::2::3::4::5::6::7::8::9::cdfhknS:V");
+static const tchar *const optstring = T("1::2::3::4::5::6::7::8::9::cdfhknqS:tV");
 
 static void
 show_usage(FILE *fp)
 {
 	fprintf(fp,
-"Usage: %"TS" [-LEVEL] [-cdfhkV] [-S SUF] FILE...\n"
+"Usage: %"TS" [-LEVEL] [-cdfhkqtV] [-S SUF] FILE...\n"
 "Compress or decompress the specified FILEs.\n"
 "\n"
 "Options:\n"
 "  -1        fastest (worst) compression\n"
 "  -6        medium compression (default)\n"
 "  -12       slowest (best) compression\n"
 "  -c        write to standard output\n"
 "  -d        decompress\n"
-"  -f        overwrite existing output files\n"
+"  -f        overwrite existing output files; (de)compress hard-linked files;\n"
+"            allow reading/writing compressed data from/to terminal;\n"
+"            with gunzip -c, pass through non-gzipped data\n"
 "  -h        print this help\n"
 "  -k        don't delete input files\n"
+"  -q        suppress warnings\n"
 "  -S SUF    use suffix SUF instead of .gz\n"
+"  -t        test file integrity\n"
 "  -V        show version and legal information\n",
 	prog_invocation_name);
 }
 
 static void
 show_version(void)
 {
@@ -170,53 +180,67 @@
 
 	ret = full_write(out, compressed_data, actual_compressed_size);
 out:
 	free(compressed_data);
 	return ret;
 }
 
-static u32
-load_u32_gzip(const u8 *p)
-{
-	return ((u32)p[0] << 0) | ((u32)p[1] << 8) |
-		((u32)p[2] << 16) | ((u32)p[3] << 24);
-}
-
 static int
 do_decompress(struct libdeflate_decompressor *decompressor,
-	      struct file_stream *in, struct file_stream *out)
+	      struct file_stream *in, struct file_stream *out,
+	      const struct options *options)
 {
 	const u8 *compressed_data = in->mmap_mem;
 	size_t compressed_size = in->mmap_size;
 	void *uncompressed_data = NULL;
 	size_t uncompressed_size;
+	size_t max_uncompressed_size;
 	size_t actual_in_nbytes;
 	size_t actual_out_nbytes;
 	enum libdeflate_result result;
 	int ret = 0;
 
-	if (compressed_size < sizeof(u32)) {
-	       msg("%"TS": not in gzip format", in->name);
-	       ret = -1;
-	       goto out;
+	if (compressed_size < GZIP_MIN_OVERHEAD ||
+	    compressed_data[0] != GZIP_ID1 ||
+	    compressed_data[1] != GZIP_ID2) {
+		if (options->force && options->to_stdout)
+			return full_write(out, compressed_data, compressed_size);
+		msg("%"TS": not in gzip format", in->name);
+		return -1;
 	}
 
 	/*
 	 * Use the ISIZE field as a hint for the decompressed data size.  It may
 	 * need to be increased later, however, because the file may contain
 	 * multiple gzip members and the particular ISIZE we happen to use may
 	 * not be the largest; or the real size may be >= 4 GiB, causing ISIZE
 	 * to overflow.  In any case, make sure to allocate at least one byte.
 	 */
-	uncompressed_size = load_u32_gzip(&compressed_data[compressed_size - 4]);
+	uncompressed_size =
+		get_unaligned_le32(&compressed_data[compressed_size - 4]);
 	if (uncompressed_size == 0)
 		uncompressed_size = 1;
 
+	/*
+	 * DEFLATE cannot expand data more than 1032x, so there's no need to
+	 * ever allocate a buffer more than 1032 times larger than the
+	 * compressed data.  This is a fail-safe, albeit not a very good one, if
+	 * ISIZE becomes corrupted on a small file.  (The 1032x number comes
+	 * from each 2 bits generating a 258-byte match.  This is a hard upper
+	 * bound; the real upper bound is slightly smaller due to overhead.)
+	 */
+	if (compressed_size <= SIZE_MAX / 1032)
+		max_uncompressed_size = compressed_size * 1032;
+	else
+		max_uncompressed_size = SIZE_MAX;
+
 	do {
 		if (uncompressed_data == NULL) {
+			uncompressed_size = MIN(uncompressed_size,
+						max_uncompressed_size);
 			uncompressed_data = xmalloc(uncompressed_size);
 			if (uncompressed_data == NULL) {
 				msg("%"TS": file is probably too large to be "
 				    "processed by this program", in->name);
 				ret = -1;
 				goto out;
 			}
@@ -227,14 +251,19 @@
 						       compressed_size,
 						       uncompressed_data,
 						       uncompressed_size,
 						       &actual_in_nbytes,
 						       &actual_out_nbytes);
 
 		if (result == LIBDEFLATE_INSUFFICIENT_SPACE) {
+			if (uncompressed_size >= max_uncompressed_size) {
+				msg("Bug in libdeflate_gzip_decompress_ex(): data expanded too much!");
+				ret = -1;
+				goto out;
+			}
 			if (uncompressed_size * 2 <= uncompressed_size) {
 				msg("%"TS": file corrupt or too large to be "
 				    "processed by this program", in->name);
 				ret = -1;
 				goto out;
 			}
 			uncompressed_size *= 2;
@@ -249,22 +278,24 @@
 			ret = -1;
 			goto out;
 		}
 
 		if (actual_in_nbytes == 0 ||
 		    actual_in_nbytes > compressed_size ||
 		    actual_out_nbytes > uncompressed_size) {
-			msg("Bug in libdeflate_gzip_decompress_ex()!");
+			msg("Bug in libdeflate_gzip_decompress_ex(): impossible actual_nbytes value!");
 			ret = -1;
 			goto out;
 		}
 
-		ret = full_write(out, uncompressed_data, actual_out_nbytes);
-		if (ret != 0)
-			goto out;
+		if (!options->test) {
+			ret = full_write(out, uncompressed_data, actual_out_nbytes);
+			if (ret != 0)
+				goto out;
+		}
 
 		compressed_data += actual_in_nbytes;
 		compressed_size -= actual_in_nbytes;
 
 	} while (compressed_size != 0);
 out:
 	free(uncompressed_data);
@@ -276,23 +307,23 @@
 {
 	if (tfstat(in->fd, stbuf) != 0) {
 		msg("%"TS": unable to stat file", in->name);
 		return -1;
 	}
 
 	if (!S_ISREG(stbuf->st_mode) && !in->is_standard_stream) {
-		msg("%"TS" is %s -- skipping",
-		    in->name, S_ISDIR(stbuf->st_mode) ? "a directory" :
-							"not a regular file");
+		warn("%"TS" is %s -- skipping",
+		     in->name, S_ISDIR(stbuf->st_mode) ? "a directory" :
+							 "not a regular file");
 		return -2;
 	}
 
 	if (stbuf->st_nlink > 1 && !allow_hard_links) {
-		msg("%"TS" has multiple hard links -- skipping "
-		    "(use -f to process anyway)", in->name);
+		warn("%"TS" has multiple hard links -- skipping (use -f to process anyway)",
+		     in->name);
 		return -2;
 	}
 
 	return 0;
 }
 
 static void
@@ -316,29 +347,27 @@
 }
 
 static void
 restore_timestamps(struct file_stream *out, const tchar *newpath,
 		   const stat_t *stbuf)
 {
 	int ret;
-#if defined(HAVE_FUTIMENS) && defined(HAVE_STAT_NANOSECOND_PRECISION)
-	struct timespec times[2] = {
-		stbuf->st_atim, stbuf->st_mtim,
-	};
+#ifdef __APPLE__
+	struct timespec times[2] = { stbuf->st_atimespec, stbuf->st_mtimespec };
+
+	ret = futimens(out->fd, times);
+#elif (defined(HAVE_FUTIMENS) && defined(HAVE_STAT_NANOSECOND_PRECISION)) || \
+	/* fallback detection method for direct compilation */ \
+	(!defined(HAVE_CONFIG_H) && defined(UTIME_NOW))
+	struct timespec times[2] = { stbuf->st_atim, stbuf->st_mtim };
+
 	ret = futimens(out->fd, times);
-#elif defined(HAVE_FUTIMES) && defined(HAVE_STAT_NANOSECOND_PRECISION)
-	struct timeval times[2] = {
-		{ stbuf->st_atim.tv_sec, stbuf->st_atim.tv_nsec / 1000, },
-		{ stbuf->st_mtim.tv_sec, stbuf->st_mtim.tv_nsec / 1000, },
-	};
-	ret = futimes(out->fd, times);
 #else
-	struct tutimbuf times = {
-		stbuf->st_atime, stbuf->st_mtime,
-	};
+	struct tutimbuf times = { stbuf->st_atime, stbuf->st_mtime };
+
 	ret = tutime(newpath, &times);
 #endif
 	if (ret != 0)
 		msg_errno("%"TS": unable to preserve timestamps", out->name);
 }
 
 static void
@@ -375,17 +404,16 @@
 			if (tstat(path, &stbuf) != 0 && errno == ENOENT) {
 				oldpath = append_suffix(path, options->suffix);
 				if (oldpath == NULL)
 					return -1;
 				if (!options->to_stdout)
 					newpath = (tchar *)path;
 			} else if (!options->to_stdout) {
-				msg("\"%"TS"\" does not end with the %"TS" "
-				    "suffix -- skipping",
-				    path, options->suffix);
+				warn("\"%"TS"\" does not end with the %"TS" suffix -- skipping",
+				     path, options->suffix);
 				return -2;
 			}
 		} else if (!options->to_stdout) {
 			/*
 			 * Input file is suffixed, and we're not writing to
 			 * stdout.  Strip the suffix to get the path to the
 			 * output file.
@@ -421,15 +449,15 @@
 		goto out_close_in;
 
 	/* TODO: need a streaming-friendly solution */
 	ret = map_file_contents(&in, stbuf.st_size);
 	if (ret != 0)
 		goto out_close_out;
 
-	ret = do_decompress(decompressor, &in, &out);
+	ret = do_decompress(decompressor, &in, &out, options);
 	if (ret != 0)
 		goto out_close_out;
 
 	if (oldpath != NULL && newpath != NULL)
 		restore_metadata(&out, newpath, &stbuf);
 	ret = 0;
 out_close_out:
@@ -530,14 +558,15 @@
 
 	begin_program(argv);
 
 	options.to_stdout = false;
 	options.decompress = is_gunzip();
 	options.force = false;
 	options.keep = false;
+	options.test = false;
 	options.compression_level = 6;
 	options.suffix = T(".gz");
 
 	while ((opt_char = tgetopt(argc, argv, optstring)) != -1) {
 		switch (opt_char) {
 		case '1':
 		case '2':
@@ -572,21 +601,35 @@
 			/*
 			 * -n means don't save or restore the original filename
 			 *  in the gzip header.  Currently this implementation
 			 *  already behaves this way by default, so accept the
 			 *  option as a no-op.
 			 */
 			break;
+		case 'q':
+			suppress_warnings = true;
+			break;
 		case 'S':
 			options.suffix = toptarg;
 			if (options.suffix[0] == T('\0')) {
 				msg("invalid suffix");
 				return 1;
 			}
 			break;
+		case 't':
+			options.test = true;
+			options.decompress = true;
+			options.to_stdout = true;
+			/*
+			 * -t behaves just like the more commonly used -c
+			 * option, except that -t doesn't actually write
+			 * anything.  For ease of implementation, just pretend
+			 * that -c was specified too.
+			 */
+			break;
 		case 'V':
 			show_version();
 			return 0;
 		default:
 			show_usage(stderr);
 			return 1;
 		}
@@ -625,17 +668,21 @@
 
 		for (i = 0; i < argc; i++)
 			ret |= -compress_file(c, argv[i], &options);
 
 		libdeflate_free_compressor(c);
 	}
 
-	/*
-	 * If ret=0, there were no warnings or errors.  Exit with status 0.
-	 * If ret=2, there was at least one warning.  Exit with status 2.
-	 * Else, there was at least one error.  Exit with status 1.
-	 */
-	if (ret != 0 && ret != 2)
-		ret = 1;
-
-	return ret;
+	switch (ret) {
+	case 0:
+		/* No warnings or errors */
+		return 0;
+	case 2:
+		/* At least one warning, but no errors */
+		if (suppress_warnings)
+			return 0;
+		return 2;
+	default:
+		/* At least one error */
+		return 1;
+	}
 }
```

### Comparing `deflate-0.3.0/libdeflate/programs/prog_util.c` & `deflate-0.4.0/libdeflate/programs/prog_util.c`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 #ifndef O_NOCTTY
 #  define O_NOCTTY 0
 #endif
 
 /* The invocation name of the program (filename component only) */
 const tchar *prog_invocation_name;
 
+/* Whether to suppress warning messages or not */
+bool suppress_warnings;
+
 static void
 do_msg(const char *format, bool with_errno, va_list va)
 {
 	int saved_errno = errno;
 
 	fprintf(stderr, "%"TS": ", prog_invocation_name);
 	vfprintf(stderr, format, va);
@@ -89,14 +92,28 @@
 	va_list va;
 
 	va_start(va, format);
 	do_msg(format, true, va);
 	va_end(va);
 }
 
+
+/* Same as msg(), but do nothing if 'suppress_warnings' has been set. */
+void
+warn(const char *format, ...)
+{
+	if (!suppress_warnings) {
+		va_list va;
+
+		va_start(va, format);
+		do_msg(format, false, va);
+		va_end(va);
+	}
+}
+
 /* malloc() wrapper */
 void *
 xmalloc(size_t size)
 {
 	void *p = malloc(size);
 	if (p == NULL && size == 0)
 		p = malloc(1);
@@ -181,16 +198,19 @@
 			 (symlink_ok ? 0 : O_NOFOLLOW) | O_SEQUENTIAL);
 	if (strm->fd < 0) {
 		msg_errno("Can't open %"TS" for reading", strm->name);
 		free(strm->name);
 		return -1;
 	}
 
-#if defined(HAVE_POSIX_FADVISE) && (O_SEQUENTIAL == 0)
-	posix_fadvise(strm->fd, 0, 0, POSIX_FADV_SEQUENTIAL);
+#if O_SEQUENTIAL == 0 && \
+	(defined(HAVE_POSIX_FADVISE) || \
+	 /* fallback detection method for direct compilation */ \
+	 (!defined(HAVE_CONFIG_H) && defined(POSIX_FADV_SEQUENTIAL)))
+	(void)posix_fadvise(strm->fd, 0, 0, POSIX_FADV_SEQUENTIAL);
 #endif
 
 	return 0;
 }
 
 /* Open a file for writing, or set up standard output for writing */
 int
@@ -222,16 +242,16 @@
 	if (strm->fd < 0) {
 		if (errno != EEXIST) {
 			msg_errno("Can't open %"TS" for writing", strm->name);
 			goto err;
 		}
 		if (!overwrite) {
 			if (!isatty(STDERR_FILENO) || !isatty(STDIN_FILENO)) {
-				msg("%"TS" already exists; use -f to overwrite",
-				    strm->name);
+				warn("%"TS" already exists; use -f to overwrite",
+				     strm->name);
 				ret = -2; /* warning only */
 				goto err;
 			}
 			fprintf(stderr, "%"TS": %"TS" already exists; "
 				"overwrite? (y/n) ",
 				prog_invocation_name, strm->name);
 			if (getchar() != 'y') {
@@ -330,28 +350,33 @@
 		CloseHandle((HANDLE)strm->mmap_token);
 		return -1;
 	}
 #else /* _WIN32 */
 	strm->mmap_mem = mmap(NULL, size, PROT_READ, MAP_SHARED, strm->fd, 0);
 	if (strm->mmap_mem == MAP_FAILED) {
 		strm->mmap_mem = NULL;
-		if (errno == ENODEV) /* mmap isn't supported on this file */
+		if (errno == ENODEV /* standard */ ||
+		    errno == EINVAL /* macOS */) {
+			/* mmap isn't supported on this file */
 			return read_full_contents(strm);
+		}
 		if (errno == ENOMEM) {
 			msg("%"TS" is too large to be processed by this "
 			    "program", strm->name);
 		} else {
 			msg_errno("Unable to map %"TS" into memory",
 				  strm->name);
 		}
 		return -1;
 	}
 
-#ifdef HAVE_POSIX_MADVISE
-	posix_madvise(strm->mmap_mem, size, POSIX_MADV_SEQUENTIAL);
+#if defined(HAVE_POSIX_MADVISE) || \
+	/* fallback detection method for direct compilation */ \
+	(!defined(HAVE_CONFIG_H) && defined(POSIX_MADV_SEQUENTIAL))
+	(void)posix_madvise(strm->mmap_mem, size, POSIX_MADV_SEQUENTIAL);
 #endif
 	strm->mmap_token = strm; /* anything that's not NULL */
 
 #endif /* !_WIN32 */
 	strm->mmap_size = size;
 	return 0;
 }
```

### Comparing `deflate-0.3.0/libdeflate/programs/prog_util.h` & `deflate-0.4.0/libdeflate/programs/prog_util.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * prog_util.h - utility functions for programs
+ * prog_util.h - common header for the programs; must be included first
  *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
@@ -24,63 +24,110 @@
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #ifndef PROGRAMS_PROG_UTIL_H
 #define PROGRAMS_PROG_UTIL_H
 
+/*
+ * This header provides some utility functions and macros for the programs.  It
+ * also defines some macros that control the behavior of system headers, and for
+ * that reason it must be included before any system header.
+ *
+ * The latter part could be handled in this directory's CMakeLists.txt instead.
+ * We put as much as possible here, directly in the source, to make it easier to
+ * build the programs using other build systems (or "no build system").
+ *
+ * Note: CMakeLists.txt does do some dynamic feature detection, which can't be
+ * done in the source code.  For that reason, it duplicates some of the logic
+ * that defines macros like _GNU_SOURCE.  Keep this logic in sync.
+ */
+
+#ifdef _WIN32
+
+  /*
+   * To keep the code similar on all platforms, sometimes we intentionally use
+   * the "deprecated" non-underscore-prefixed variants of functions in msvcrt.
+   */
+#  undef _CRT_NONSTDC_NO_DEPRECATE
+#  define _CRT_NONSTDC_NO_DEPRECATE	1
+
+  /*
+   * Similarly, to match other platforms we intentionally use the "non-secure"
+   * variants, which aren't actually any less secure when used properly.
+   */
+#  undef _CRT_SECURE_NO_WARNINGS
+#  define _CRT_SECURE_NO_WARNINGS	1
+
+#else
+
+   /* Needed to work with files >= 2 GiB on 32-bit systems */
+#  undef _FILE_OFFSET_BITS
+#  define _FILE_OFFSET_BITS	64
+
+   /* Note: when making changes here, update programs/CMakeLists.txt too. */
+#  if defined(__linux__)
+     /*
+      * May be needed for clock_gettime(), posix_fadvise(), posix_madvise(),
+      * futimens(), and MAP_ANONYMOUS, depending on the C library version.
+      */
+#    undef _GNU_SOURCE
+#    define _GNU_SOURCE
+#    undef _POSIX_C_SOURCE
+#    define _POSIX_C_SOURCE	200809L
+#  elif defined(__APPLE__)
+     /* Needed for O_NOFOLLOW and MAP_ANON */
+#    undef _DARWIN_C_SOURCE
+#    define _DARWIN_C_SOURCE
+#    undef _POSIX_C_SOURCE
+#  elif defined(__sun)
+     /* Needed for futimens() */
+#    undef __EXTENSIONS__
+#    define __EXTENSIONS__
+#    undef _POSIX_C_SOURCE
+#  else
+     /*
+      * Else assume that nothing else is needed.  Don't use _POSIX_C_SOURCE on
+      * BSD, since it causes anything non-POSIX, such as MAP_ANON, to be hidden.
+      */
+#    undef _POSIX_C_SOURCE
+#  endif
+#endif
+
 #ifdef HAVE_CONFIG_H
 #  include "config.h"
 #endif
 
-#include "libdeflate.h"
+#include "../common_defs.h"
 
+#include <inttypes.h>
 #include <limits.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
+#ifndef _WIN32
+#  include <sys/types.h>
+#endif
 
-#include "../common/common_defs.h"
-
-#ifdef __GNUC__
+#if defined(__GNUC__) || __has_attribute(format)
 # define _printf(str_idx, args_idx)	\
 		__attribute__((format(printf, str_idx, args_idx)))
 #else
 # define _printf(str_idx, args_idx)
 #endif
 
-#ifdef _MSC_VER
-/*
- * Old versions (e.g. VS2010) of MSC have stdint.h but not the C99 header
- * inttypes.h.  Work around this by defining the PRI* macros ourselves.
- */
-# define PRIu8  "hhu"
-# define PRIu16 "hu"
-# define PRIu32 "u"
-# define PRIu64 "llu"
-# define PRIi8  "hhi"
-# define PRIi16 "hi"
-# define PRIi32 "i"
-# define PRIi64 "lli"
-# define PRIx8  "hhx"
-# define PRIx16 "hx"
-# define PRIx32 "x"
-# define PRIx64 "llx"
-#else
-# include <inttypes.h>
-#endif
-
 #ifdef _WIN32
 
 /*
  * Definitions for Windows builds.  Mainly, 'tchar' is defined to be the 2-byte
  * 'wchar_t' type instead of 'char'.  This is the only "easy" way I know of to
  * get full Unicode support on Windows...
  */
 
+#include <io.h>
 #include <wchar.h>
 int wmain(int argc, wchar_t **argv);
 #  define	tmain		wmain
 #  define	tchar		wchar_t
 #  define	_T(text)	L##text
 #  define	T(text)		_T(text)
 #  define	TS		"ls"
@@ -130,17 +177,19 @@
 #  define	tstat		stat
 #  define	tfstat		fstat
 #  define	stat_t		struct stat
 
 #endif /* !_WIN32 */
 
 extern const tchar *prog_invocation_name;
+extern bool suppress_warnings;
 
 void _printf(1, 2) msg(const char *fmt, ...);
 void _printf(1, 2) msg_errno(const char *fmt, ...);
+void _printf(1, 2) warn(const char *fmt, ...);
 
 void *xmalloc(size_t size);
 
 void begin_program(tchar *argv[]);
 
 struct file_stream {
 	int fd;
```

### Comparing `deflate-0.3.0/libdeflate/programs/test_checksums.c` & `deflate-0.4.0/libdeflate/programs/test_checksums.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*
  * test_checksums.c
  *
  * Verify that libdeflate's Adler-32 and CRC-32 functions produce the same
  * results as their zlib equivalents.
  */
 
+#include "test_util.h"
+
 #include <stdlib.h>
 #include <time.h>
 
-#include "test_util.h"
-
 static unsigned int rng_seed;
 
 typedef u32 (*cksum_fn_t)(u32, const void *, size_t);
 
 static u32
 adler32_libdeflate(u32 adler, const void *buf, size_t len)
 {
@@ -118,79 +118,83 @@
 static void
 test_adler32(const void *buffer, size_t size, u32 initial_value)
 {
 	test_checksums(buffer, size, "Adler-32",
 		       adler32_libdeflate, adler32_zlib, initial_value);
 }
 
-static void test_random_buffers(u8 *buffer, u8 *guarded_buf_end,
-				size_t limit, u32 num_iter)
+static void test_random_buffers(u8 *buf_start, u8 *buf_end, size_t limit,
+				u32 num_iter)
 {
 	for (u32 i = 0; i < num_iter; i++) {
 		size_t start = rand() % limit;
 		size_t len = rand() % (limit - start);
 		u32 a0 = select_initial_adler();
 		u32 c0 = select_initial_crc();
 
 		for (size_t j = start; j < start + len; j++)
-			buffer[j] = rand();
+			buf_start[j] = rand();
 
 		/* Test with chosen size and alignment */
-		test_adler32(&buffer[start], len, a0);
-		test_crc32(&buffer[start], len, c0);
+		test_adler32(&buf_start[start], len, a0);
+		test_crc32(&buf_start[start], len, c0);
+
+		/* Test with chosen size, with guard page before input buffer */
+		memmove(buf_start, &buf_start[start], len);
+		test_adler32(buf_start, len, a0);
+		test_crc32(buf_start, len, c0);
 
 		/* Test with chosen size, with guard page after input buffer */
-		memcpy(guarded_buf_end - len, &buffer[start], len);
-		test_adler32(guarded_buf_end - len, len, a0);
-		test_crc32(guarded_buf_end - len, len, c0);
+		memmove(buf_end - len, buf_start, len);
+		test_adler32(buf_end - len, len, a0);
+		test_crc32(buf_end - len, len, c0);
 	}
 }
 
 int
 tmain(int argc, tchar *argv[])
 {
-	u8 *buffer = xmalloc(32768);
-	u8 *guarded_buf_start, *guarded_buf_end;
+	u8 *buf_start, *buf_end;
 
 	begin_program(argv);
 
-	alloc_guarded_buffer(32768, &guarded_buf_start, &guarded_buf_end);
+	alloc_guarded_buffer(262144, &buf_start, &buf_end);
 
 	rng_seed = time(NULL);
 	srand(rng_seed);
 
 	test_initial_values(adler32_libdeflate, 1);
 	test_initial_values(adler32_zlib, 1);
 	test_initial_values(crc32_libdeflate, 0);
 	test_initial_values(crc32_zlib, 0);
 
 	/* Test different buffer sizes and alignments */
-	test_random_buffers(buffer, guarded_buf_end, 256, 5000);
-	test_random_buffers(buffer, guarded_buf_end, 1024, 500);
-	test_random_buffers(buffer, guarded_buf_end, 32768, 50);
+	test_random_buffers(buf_start, buf_end, 256,  5000);
+	test_random_buffers(buf_start, buf_end, 1024,  500);
+	test_random_buffers(buf_start, buf_end, 32768,  50);
+	test_random_buffers(buf_start, buf_end, 262144, 25);
 
 	/*
 	 * Test Adler-32 overflow cases.  For example, given all 0xFF bytes and
 	 * the highest possible initial (s1, s2) of (65520, 65520), then s2 if
 	 * stored as a 32-bit unsigned integer will overflow if > 5552 bytes are
 	 * processed.  Implementations must make sure to reduce s2 modulo 65521
 	 * before that point.  Also, some implementations make use of 16-bit
 	 * counters which can overflow earlier.
 	 */
-	memset(buffer, 0xFF, 32768);
+	memset(buf_start, 0xFF, 32768);
 	for (u32 i = 0; i < 20; i++) {
 		u32 initial_value;
 
 		if (i == 0)
 			initial_value = ((u32)65520 << 16) | 65520;
 		else
 			initial_value = select_initial_adler();
 
-		test_adler32(buffer, 5553, initial_value);
-		test_adler32(buffer, rand() % 32769, initial_value);
-		buffer[rand() % 32768] = 0xFE;
+		test_adler32(buf_start, 5553, initial_value);
+		test_adler32(buf_start, rand() % 32769, initial_value);
+		buf_start[rand() % 32768] = 0xFE;
 	}
 
-	free(buffer);
-	free_guarded_buffer(guarded_buf_start, guarded_buf_end);
+	free_guarded_buffer(buf_start, buf_end);
 	return 0;
 }
```

### Comparing `deflate-0.3.0/libdeflate/programs/test_custom_malloc.c` & `deflate-0.4.0/libdeflate/programs/test_custom_malloc.c`

 * *Files identical despite different names*

### Comparing `deflate-0.3.0/libdeflate/programs/test_incomplete_codes.c` & `deflate-0.4.0/libdeflate/programs/test_incomplete_codes.c`

 * *Files identical despite different names*

### Comparing `deflate-0.3.0/libdeflate/programs/test_litrunlen_overflow.c` & `deflate-0.4.0/libdeflate/programs/test_litrunlen_overflow.c`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  */
 
 #include "test_util.h"
 
 int
 tmain(int argc, tchar *argv[])
 {
-	const size_t data_size = 2 * 250 * 251;
+	const int data_size = 2 * 250 * 251;
 	u8 *orig_data, *compressed_data, *decompressed_data;
 	int i, stride, multiple, j = 0;
 	struct libdeflate_decompressor *d;
 	static const int levels[] = { 3, 6, 12 };
 
 	begin_program(argv);
```

### Comparing `deflate-0.3.0/libdeflate/programs/test_slow_decompression.c` & `deflate-0.4.0/libdeflate/programs/test_slow_decompression.c`

 * *Files identical despite different names*

### Comparing `deflate-0.3.0/libdeflate/programs/test_trailing_bytes.c` & `deflate-0.4.0/libdeflate/programs/test_trailing_bytes.c`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,23 @@
  * Test that decompression correctly stops at the end of the first DEFLATE,
  * zlib, or gzip stream, and doesn't process any additional trailing bytes.
  */
 
 #include "test_util.h"
 
 static const struct {
-	size_t (LIBDEFLATEAPI *compress)(
-			struct libdeflate_compressor *compressor,
-			const void *in, size_t in_nbytes,
-			void *out, size_t out_nbytes_avail);
-	enum libdeflate_result (LIBDEFLATEAPI *decompress)(
+	size_t (*compress)(struct libdeflate_compressor *compressor,
+			   const void *in, size_t in_nbytes,
+			   void *out, size_t out_nbytes_avail);
+	enum libdeflate_result (*decompress)(
 			struct libdeflate_decompressor *decompressor,
 			const void *in, size_t in_nbytes,
 			void *out, size_t out_nbytes_avail,
 			size_t *actual_out_nbytes_ret);
-	enum libdeflate_result (LIBDEFLATEAPI *decompress_ex)(
+	enum libdeflate_result (*decompress_ex)(
 			struct libdeflate_decompressor *decompressor,
 			const void *in, size_t in_nbytes,
 			void *out, size_t out_nbytes_avail,
 			size_t *actual_in_nbytes_ret,
 			size_t *actual_out_nbytes_ret);
 } codecs[] = {
 	{
```

### Comparing `deflate-0.3.0/libdeflate/programs/test_util.c` & `deflate-0.4.0/libdeflate/programs/test_util.c`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,14 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
-#ifndef _WIN32
-/* for MAP_ANONYMOUS or MAP_ANON, which unfortunately aren't part of POSIX... */
-#  undef _POSIX_C_SOURCE
-#  ifdef __APPLE__
-#    define _DARWIN_C_SOURCE
-#  elif defined(__linux__)
-#    define _GNU_SOURCE
-#  endif
-#endif
-
 #include "test_util.h"
 
 #include <fcntl.h>
 #include <time.h>
 #ifdef _WIN32
 #  include <windows.h>
 #else
@@ -154,15 +144,17 @@
 timer_ticks(void)
 {
 #ifdef _WIN32
 	LARGE_INTEGER count;
 
 	QueryPerformanceCounter(&count);
 	return count.QuadPart;
-#elif defined(HAVE_CLOCK_GETTIME)
+#elif defined(HAVE_CLOCK_GETTIME) || \
+	/* fallback detection method for direct compilation */ \
+	(!defined(HAVE_CONFIG_H) && defined(CLOCK_MONOTONIC))
 	struct timespec ts;
 
 	clock_gettime(CLOCK_MONOTONIC, &ts);
 	return (1000000000 * (u64)ts.tv_sec) + ts.tv_nsec;
 #else
 	struct timeval tv;
```

### Comparing `deflate-0.3.0/libdeflate/programs/test_util.h` & `deflate-0.4.0/libdeflate/programs/test_util.h`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,19 @@
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
 #ifndef PROGRAMS_TEST_UTIL_H
 #define PROGRAMS_TEST_UTIL_H
 
-#include "prog_util.h"
+#include "prog_util.h" /* must be included first */
 
 #include <zlib.h> /* for comparison purposes */
 
-#ifdef __GNUC__
+#if defined(__GNUC__) || __has_attribute(noreturn)
 # define _noreturn __attribute__((noreturn))
 #else
 # define _noreturn
 #endif
 
 void _noreturn
 assertion_failed(const char *expr, const char *file, int line);
```

### Comparing `deflate-0.3.0/libdeflate/programs/tgetopt.c` & `deflate-0.4.0/libdeflate/programs/tgetopt.c`

 * *Files identical despite different names*

### Comparing `deflate-0.3.0/libdeflate/scripts/android_build.sh` & `deflate-0.4.0/libdeflate/scripts/android_build.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/bin/bash
 
 set -eu -o pipefail
 
+SCRIPTDIR="$(dirname "$0")"
+BUILDDIR="$SCRIPTDIR/../build"
 API_LEVEL=28
 ARCH=arm64
-CFLAGS=
+export CFLAGS=${CFLAGS:-}
 ENABLE_CRC=false
 ENABLE_CRYPTO=false
-NDKDIR=$HOME/android-ndk-r21d
+NDKDIR=$HOME/android-ndk-r23b
 
 usage() {
 	cat << EOF
-Usage: $0 [OPTION]... -- [MAKE_TARGET]...
+Usage: $0 [OPTION]...
 Build libdeflate for Android.
 
   --api-level=LEVEL    Android API level to target (default: $API_LEVEL)
-  --arch=ARCH          Architecture: arm32|arm64 (default: $ARCH)
+  --arch=ARCH          Architecture: arm32|arm64|x86|x86_64 (default: $ARCH)
   --enable-crc         Enable crc instructions
   --enable-crypto      Enable crypto instructions
   --ndkdir=NDKDIR      Android NDK directory (default: $NDKDIR)
 EOF
 }
 if ! options=$(getopt -o '' \
 	-l 'api-level:,arch:,enable-crc,enable-crypto,help,ndkdir:' -- "$@"); then
@@ -61,48 +63,55 @@
 		echo 1>&2 "Unknown option \"$1\""
 		usage 1>&2
 		exit 1
 	esac
 	shift
 done
 
-BINDIR=$NDKDIR/toolchains/llvm/prebuilt/linux-x86_64/bin/
-
 case "$ARCH" in
-arm|arm32|aarch32)
-	CC=$BINDIR/armv7a-linux-androideabi$API_LEVEL-clang
+arm|arm32|aarch32|armeabi-v7a)
+	ANDROID_ABI=armeabi-v7a
 	if $ENABLE_CRC || $ENABLE_CRYPTO; then
-		CFLAGS="-march=armv8-a"
+		CFLAGS+=" -march=armv8-a"
 		if $ENABLE_CRC; then
 			CFLAGS+=" -mcrc"
 		else
 			CFLAGS+=" -mnocrc"
 		fi
 		if $ENABLE_CRYPTO; then
 			CFLAGS+=" -mfpu=crypto-neon-fp-armv8"
 		else
 			CFLAGS+=" -mfpu=neon"
 		fi
 	fi
 	;;
-arm64|aarch64)
-	CC=$BINDIR/aarch64-linux-android$API_LEVEL-clang
+arm64|aarch64|arm64-v8a)
+	ANDROID_ABI=arm64-v8a
 	features=""
 	if $ENABLE_CRC; then
 		features+="+crc"
 	fi
 	if $ENABLE_CRYPTO; then
 		features+="+crypto"
 	fi
 	if [ -n "$features" ]; then
-		CFLAGS="-march=armv8-a$features"
+		CFLAGS+=" -march=armv8-a$features"
 	fi
 	;;
+x86)
+	ANDROID_ABI=x86
+	;;
+x86_64)
+	ANDROID_ABI=x86_64
+	;;
 *)
 	echo 1>&2 "Unknown architecture: \"$ARCH\""
 	usage 1>&2
 	exit 1
 esac
 
-cmd=(make "-j$(grep -c processor /proc/cpuinfo)" "CC=$CC" "CFLAGS=$CFLAGS" "$@")
-echo "${cmd[*]}"
-"${cmd[@]}"
+"$SCRIPTDIR"/cmake-helper.sh -G Ninja \
+	-DCMAKE_TOOLCHAIN_FILE="$NDKDIR"/build/cmake/android.toolchain.cmake \
+	-DANDROID_ABI="$ANDROID_ABI" \
+	-DANDROID_PLATFORM="$API_LEVEL" \
+	-DLIBDEFLATE_BUILD_TESTS=1
+cmake --build "$BUILDDIR"
```

### Comparing `deflate-0.3.0/libdeflate/scripts/android_tests.sh` & `deflate-0.4.0/libdeflate/scripts/android_tests.sh`

 * *Files 20% similar despite different names*

```diff
@@ -8,55 +8,62 @@
 
 if [ $# -ne 0 ]; then
 	echo 1>&2 "Usage: $0"
 	exit 2
 fi
 
 # Use NDKDIR if specified in environment, else use default value.
-: "${NDKDIR:=$HOME/android-ndk-r21d}"
+: "${NDKDIR:=$HOME/android-ndk-r23b}"
 if [ ! -e "$NDKDIR" ]; then
 	cat 1>&2 << EOF
 Android NDK was not found in NDKDIR=$NDKDIR!  Set the
 environmental variable NDKDIR to the location of your Android NDK installation.
 EOF
 	exit 1
 fi
 
+CLEANUP_CMDS=()
+cleanup() {
+	for cmd in "${CLEANUP_CMDS[@]}"; do
+		eval "$cmd"
+	done
+}
+trap cleanup EXIT
+
 # Use TESTDATA if specified in environment, else generate it.
 if [ -z "${TESTDATA:-}" ]; then
 	# Generate default TESTDATA file.
-	TESTDATA=$(mktemp -t libdeflate_testdata.XXXXXXX)
+	TESTDATA=$(mktemp -t libdeflate_testdata.XXXXXXXXXX)
 	export TESTDATA
-	trap 'rm -f "$TESTDATA"' EXIT
+	CLEANUP_CMDS+=("rm -f '$TESTDATA'")
 	find . '(' -name '*.c' -o -name '*.h' -o -name '*.sh' ')' \
 		-exec cat '{}' ';' | head -c 1000000 > "$TESTDATA"
 fi
 
-# Create a temporary file.
-TMPFILE=$(mktemp -t libdeflate_tmpfile.XXXXXX)
-trap 'rm -f "$TMPFILE"' EXIT
+TMPDIR=$(mktemp -d -t libdeflate_test.XXXXXXXXX)
+CLEANUP_CMDS+=("rm -r '$TMPDIR'")
 
 android_build_and_test() {
 	echo "Running Android tests with $*"
 
-	./scripts/android_build.sh --ndkdir="$NDKDIR" "$@" \
-		all test_programs > /dev/null
-	adb push "$TESTDATA" ./scripts/exec_tests.sh benchmark test_* \
-		/data/local/tmp/ > /dev/null
+	./scripts/android_build.sh --ndkdir="$NDKDIR" "$@" > /dev/null
+	adb push "$TESTDATA" ./scripts/exec_tests.sh \
+		./build/programs/{benchmark,test_*} /data/local/tmp/ > /dev/null
 
 	# Note: adb shell always returns 0, even if the shell command fails...
 	adb shell "cd /data/local/tmp && WRAPPER= TESTDATA=$(basename "$TESTDATA") sh exec_tests.sh" \
-		> "$TMPFILE"
-	if ! grep -q "exec_tests finished successfully" "$TMPFILE"; then
+		> "$TMPDIR/adb.out"
+	if ! grep -q "exec_tests finished successfully" "$TMPDIR/adb.out"; then
 		echo 1>&2 "Android test failure!  adb shell output:"
-		cat "$TMPFILE"
+		cat "$TMPDIR/adb.out"
 		exit 1
 	fi
 }
 
-for arch in arm32 arm64; do
-	android_build_and_test --arch=$arch
-	android_build_and_test --arch=$arch --enable-crc
-	android_build_and_test --arch=$arch --enable-crypto
-	android_build_and_test --arch=$arch --enable-crc --enable-crypto
-done
+android_build_and_test --arch=arm32
+android_build_and_test --arch=arm32 --enable-crc
+android_build_and_test --arch=arm64
+android_build_and_test --arch=arm64 --enable-crc
+android_build_and_test --arch=arm64 --enable-crypto
+android_build_and_test --arch=arm64 --enable-crc --enable-crypto
+
 echo "Android tests passed"
```

### Comparing `deflate-0.3.0/libdeflate/scripts/checksum_benchmarks.sh` & `deflate-0.4.0/libdeflate/scripts/checksum_benchmarks.sh`

 * *Files 12% similar despite different names*

```diff
@@ -15,41 +15,45 @@
 	esac
 	grep -q "^$tag"$'[ \t]'"*:.*\<$feature\>" /proc/cpuinfo
 }
 
 make_and_test() {
 	# Build the checksum program and tests.  Set the special test support
 	# flag to get support for LIBDEFLATE_DISABLE_CPU_FEATURES.
-	make "$@" TEST_SUPPORT__DO_NOT_USE=1 checksum test_checksums > /dev/null
+	rm -rf build
+	CFLAGS="$CFLAGS -DTEST_SUPPORT__DO_NOT_USE=1" \
+		cmake -B build -G Ninja -DLIBDEFLATE_BUILD_TESTS=1 > /dev/null
+	cmake --build build > /dev/null
 
 	# Run the checksum tests, for good measure.  (This isn't actually part
 	# of the benchmarking.)
-	./test_checksums > /dev/null
+	./build/programs/test_checksums > /dev/null
 }
 
 __do_benchmark() {
 	local impl="$1" speed
 	shift
 	local flags=("$@")
 
-	speed=$(./checksum "${CKSUM_FLAGS[@]}" "${flags[@]}" -t "$FILE" | \
+	speed=$(./build/programs/checksum "${CKSUM_FLAGS[@]}" \
+		"${flags[@]}" -t "$FILE" | \
 		grep -o '[0-9]\+ MB/s' | grep -o '[0-9]\+')
 	printf "%-45s%-10s\n" "$CKSUM_NAME ($impl)" "$speed"
 }
 
 do_benchmark() {
 	local impl="$1"
 
 	if [ "$impl" = zlib ]; then
 		__do_benchmark "$impl" "-Z"
 	else
-		make_and_test CFLAGS="${EXTRA_CFLAGS[*]}"
+		CFLAGS="${EXTRA_CFLAGS[*]}" make_and_test
 		__do_benchmark "libdeflate, $impl"
 		if [ "$ARCH" = x86_64 ]; then
-			make_and_test CFLAGS="-m32 ${EXTRA_CFLAGS[*]}"
+			CFLAGS="-m32 ${EXTRA_CFLAGS[*]}" make_and_test
 			__do_benchmark "libdeflate, $impl, 32-bit"
 		fi
 	fi
 }
 
 sort_by_speed() {
 	awk '{print $NF, $0}' | sort -nr | cut -f2- -d' '
@@ -132,18 +136,14 @@
 CKSUM_FLAGS=(-A)
 EXTRA_CFLAGS=()
 export LIBDEFLATE_DISABLE_CPU_FEATURES=""
 echo
 {
 case $ARCH in
 i386|x86_64)
-	if have_cpu_feature avx512bw; then
-		do_benchmark "AVX-512BW"
-		disable_cpu_feature "avx512bw" "-mno-avx512bw"
-	fi
 	if have_cpu_feature avx2; then
 		do_benchmark "AVX2"
 		disable_cpu_feature "avx2" "-mno-avx2"
 	fi
 	if have_cpu_feature sse2; then
 		do_benchmark "SSE2"
 		disable_cpu_feature "sse2" "-mno-sse2"
```

### Comparing `deflate-0.3.0/libdeflate/scripts/exec_tests.sh` & `deflate-0.4.0/libdeflate/scripts/exec_tests.sh`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 #
 # Helper script used by run_tests.sh and android_tests.sh,
 # not intended to be run directly
 #
 
 set -eu
 
+DIR=${1:-.}
+
+cd "$DIR"
+
 run_cmd() {
 	echo "$WRAPPER $*"
 	$WRAPPER "$@" > /dev/null
 }
 
 for prog in ./test_*; do
 	run_cmd "$prog"
```

### Comparing `deflate-0.3.0/libdeflate/scripts/gen_crc32_table.c` & `deflate-0.4.0/libdeflate/scripts/gen_crc32_tables.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 /*
- * gen_crc32_table.c - a program for CRC-32 table generation
- *
- * Originally public domain; changes after 2016-09-07 are copyrighted.
+ * gen_crc32_tables.c - a program for CRC-32 table generation
  *
  * Copyright 2016 Eric Biggers
  *
  * Permission is hereby granted, free of charge, to any person
  * obtaining a copy of this software and associated documentation
  * files (the "Software"), to deal in the Software without
  * restriction, including without limitation the rights to use,
@@ -23,36 +21,36 @@
  * NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  * HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  * WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  * FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  * OTHER DEALINGS IN THE SOFTWARE.
  */
 
-#include <stdint.h>
 #include <stdio.h>
 
-static uint32_t crc32_table[0x800];
+#include "../common_defs.h"
+
+#define CRCPOLY	0xEDB88320 /* G(x) without x^32 term */
 
-static uint32_t
-crc32_update_bit(uint32_t remainder, uint8_t next_bit)
+static u32
+crc32_update_bit(u32 remainder, u8 next_bit)
 {
-	return (remainder >> 1) ^
-		(((remainder ^ next_bit) & 1) ? 0xEDB88320 : 0);
+	return (remainder >> 1) ^ (((remainder ^ next_bit) & 1) ? CRCPOLY : 0);
 }
 
-static uint32_t
-crc32_update_byte(uint32_t remainder, uint8_t next_byte)
+static u32
+crc32_update_byte(u32 remainder, u8 next_byte)
 {
 	for (int j = 0; j < 8; j++, next_byte >>= 1)
 		remainder = crc32_update_bit(remainder, next_byte & 1);
 	return remainder;
 }
 
 static void
-print_256_entries(const uint32_t *entries)
+print_256_entries(const u32 *entries)
 {
 	for (size_t i = 0; i < 256 / 4; i++) {
 		printf("\t");
 		for (size_t j = 0; j < 4; j++) {
 			printf("0x%08x,", entries[i * 4 + j]);
 			if (j != 3)
 				printf(" ");
@@ -60,41 +58,48 @@
 		printf("\n");
 	}
 }
 
 int
 main(void)
 {
-	/* crc32_table[i] for 0 <= i < 0x100 is the CRC-32 of byte i.  */
+	u32 crc32_table[0x800];
+
+	/* crc32_table[i] for 0 <= i < 0x100 is the CRC-32 of byte i. */
 	for (int i = 0; i < 0x100; i++)
 		crc32_table[i] = crc32_update_byte(0, i);
 
-	/* crc32_table[i] for 0x100 <= i < 0x800 is the CRC-32 of byte i % 0x100
-	 * followed by i / 0x100 zero bytes.  */
+	/*
+	 * crc32_table[i] for 0x100 <= i < 0x800 is the CRC-32 of byte i % 0x100
+	 * followed by i / 0x100 zero bytes.
+	 */
 	for (int i = 0x100; i < 0x800; i++)
 		crc32_table[i] = crc32_update_byte(crc32_table[i - 0x100], 0);
 
 	printf("/*\n");
-	printf(" * crc32_table.h - data table to accelerate CRC-32 computation\n");
+	printf(" * crc32_tables.h - data tables for CRC-32 computation\n");
 	printf(" *\n");
-	printf(" * THIS FILE WAS AUTOMATICALLY GENERATED "
-	       "BY gen_crc32_table.c.  DO NOT EDIT.\n");
+	printf(" * THIS FILE WAS GENERATED BY gen_crc32_tables.c.  DO NOT EDIT.\n");
 	printf(" */\n");
 	printf("\n");
-	printf("#include <stdint.h>\n");
+	/*
+	 * Although crc32_slice1_table is the same as the first 256 entries of
+	 * crc32_slice8_table, we output these tables separately because any
+	 * combo of (slice1, slice8, slice1 && slice8, nothing) might be needed,
+	 * and it's simplest to let the compiler optimize out any unused tables.
+	 */
+	printf("static const u32 crc32_slice1_table[] MAYBE_UNUSED = {\n");
+	print_256_entries(&crc32_table[0x000]);
+	printf("};\n");
 	printf("\n");
-	printf("static const uint32_t crc32_table[] = {\n");
+	printf("static const u32 crc32_slice8_table[] MAYBE_UNUSED = {\n");
 	print_256_entries(&crc32_table[0x000]);
-	printf("#if defined(CRC32_SLICE4) || defined(CRC32_SLICE8)\n");
 	print_256_entries(&crc32_table[0x100]);
 	print_256_entries(&crc32_table[0x200]);
 	print_256_entries(&crc32_table[0x300]);
-	printf("#endif /* CRC32_SLICE4 || CRC32_SLICE8 */\n");
-	printf("#if defined(CRC32_SLICE8)\n");
 	print_256_entries(&crc32_table[0x400]);
 	print_256_entries(&crc32_table[0x500]);
 	print_256_entries(&crc32_table[0x600]);
 	print_256_entries(&crc32_table[0x700]);
-	printf("#endif /* CRC32_SLICE8 */\n");
 	printf("};\n");
 	return 0;
 }
```

### Comparing `deflate-0.3.0/libdeflate/scripts/gzip_tests.sh` & `deflate-0.4.0/libdeflate/scripts/gzip_tests.sh`

 * *Files 9% similar despite different names*

```diff
@@ -11,43 +11,83 @@
 # test data.
 #
 
 set -eu -o pipefail
 
 export -n GZIP GUNZIP TESTDATA
 
+ORIG_PWD=$PWD
 TMPDIR="$(mktemp -d)"
 CURRENT_TEST=
 
+BSD_STAT=false
+if ! stat --version 2>&1 | grep -q coreutils; then
+	BSD_STAT=true
+fi
+
 cleanup() {
 	if [ -n "$CURRENT_TEST" ]; then
 		echo "TEST FAILED: \"$CURRENT_TEST\""
 	fi
 	rm -rf -- "$TMPDIR"
 }
 
 trap cleanup EXIT
 
-TESTDATA="$(readlink -f "$TESTDATA")"
-cd "$TMPDIR"
-
 begin_test() {
 	CURRENT_TEST="$1"
 	rm -rf -- "${TMPDIR:?}"/*
-	cp "$TESTDATA" file
+	cd "$ORIG_PWD"
+	cp "$TESTDATA" "$TMPDIR/file"
+	chmod +w "$TMPDIR/file"
+	cd "$TMPDIR"
 }
 
 gzip() {
 	$GZIP "$@"
 }
 
 gunzip() {
 	$GUNZIP "$@"
 }
 
+get_filesize() {
+	local file=$1
+
+	if $BSD_STAT; then
+		stat -f %z "$file"
+	else
+		stat -c %s "$file"
+	fi
+}
+
+get_linkcount() {
+	local file=$1
+
+	if $BSD_STAT; then
+		stat -f %l "$file"
+	else
+		stat -c %h "$file"
+	fi
+}
+
+get_modeandtimestamps() {
+	local file=$1
+
+	if $BSD_STAT; then
+		stat -f "%p;%a;%m" "$file"
+	elif [ "$(uname -m)" = s390x ]; then
+		# Use seconds precision instead of nanoseconds.
+		# TODO: why is this needed?  QEMU user mode emulation bug?
+		stat -c "%a;%X;%Y" "$file"
+	else
+		stat -c "%a;%x;%y" "$file"
+	fi
+}
+
 assert_status() {
 	local expected_status="$1"
 	local expected_msg="$2"
 	shift 2
 	(
 		set +e
 		{ eval "$*" > /dev/null; } 2>&1
@@ -89,34 +129,14 @@
 
 	if [ "$expected" != "$actual" ]; then
 		echo 1>&2 "Expected '$expected', but got '$actual'"
 		return 1
 	fi
 }
 
-# Get the filesystem type.
-FSTYPE=$(df -T . | tail -1 | awk '{print $2}')
-
-# If gzip or gunzip is the GNU version, require that it supports the '-k'
-# option.  This option was added in v1.6, released in 2013.
-check_version_prereq() {
-	local prog=$1
-
-	if ! echo | { $prog -k || true; } |& grep -q 'invalid option'; then
-		return 0
-	fi
-	if ! $prog -V |& grep -q 'Free Software Foundation'; then
-		echo 1>&2 "Unexpected case: not GNU $prog, but -k option is invalid"
-		exit 1
-	fi
-	echo "GNU $prog is too old; skipping gzip/gunzip tests"
-	exit 0
-}
-check_version_prereq gzip
-check_version_prereq gunzip
 
 begin_test 'Basic compression and decompression works'
 cp file orig
 gzip file
 [ ! -e file ] && [ -e file.gz ]
 gunzip file.gz
 [ -e file ] && [ ! -e file.gz ]
@@ -174,15 +194,15 @@
 begin_test 'can specify multiple options'
 gzip -fk1 file
 cmp <(gzip -c -1 file) file.gz
 gunzip -kfd file.gz
 
 
 begin_test 'Compression levels'
-if [ "$GZIP" = /bin/gzip ]; then
+if [ "$GZIP" = /bin/gzip ] || [ "$GZIP" = /usr/bin/gzip ]; then
 	assert_error '\<invalid option\>' gzip -10
 	max_level=9
 else
 	for level in 13 99999 1a; do
 		assert_error '\<Invalid compression level\>' gzip -$level
 	done
 	max_level=12
@@ -220,14 +240,29 @@
 gzip file.gz 2>&1 >/dev/null | grep -q 'already has .gz suffix'
 [ -e file.gz ] && [ ! -e file.gz.gz ]
 gzip -f file.gz
 [ ! -e file.gz ] && [ -e file.gz.gz ]
 cmp file.gz.gz c.gz
 
 
+begin_test 'gunzip -f -c passes through non-gzip data'
+echo hello > file
+cp file orig
+gunzip -f -c file > foo
+cmp file foo
+gzip file
+gunzip -f -c file.gz > foo
+cmp foo orig
+
+
+begin_test 'gunzip -f (without -c) does *not* pass through non-gzip data'
+echo hello > file.gz
+assert_error '\<not in gzip format\>' gunzip -f file.gz
+
+
 begin_test 'Decompressing unsuffixed file only works with -c'
 gzip file && mv file.gz file
 assert_skipped gunzip file
 assert_skipped gunzip -f file
 gunzip -c file > orig
 mv file file.gz && gunzip file.gz && cmp file orig
 
@@ -313,36 +348,36 @@
 cmp <(echo a) a
 cmp <(echo b) b
 
 
 begin_test '(gzip) hard linked file skipped without -f or -c'
 cp file orig
 ln file link
-assert_equals 2 "$(stat -c %h file)"
+assert_equals 2 "$(get_linkcount file)"
 assert_skipped gzip file
 gzip -c file > /dev/null
-assert_equals 2 "$(stat -c %h file)"
+assert_equals 2 "$(get_linkcount file)"
 gzip -f file
-assert_equals 1 "$(stat -c %h link)"
-assert_equals 1 "$(stat -c %h file.gz)"
+assert_equals 1 "$(get_linkcount link)"
+assert_equals 1 "$(get_linkcount file.gz)"
 cmp link orig
 # XXX: GNU gzip skips hard linked files with -k, libdeflate's doesn't
 
 
 begin_test '(gunzip) hard linked file skipped without -f or -c'
 gzip file
 ln file.gz link.gz
 cp file.gz orig.gz
-assert_equals 2 "$(stat -c %h file.gz)"
+assert_equals 2 "$(get_linkcount file.gz)"
 assert_skipped gunzip file.gz
 gunzip -c file.gz > /dev/null
-assert_equals 2 "$(stat -c %h file.gz)"
+assert_equals 2 "$(get_linkcount file.gz)"
 gunzip -f file
-assert_equals 1 "$(stat -c %h link.gz)"
-assert_equals 1 "$(stat -c %h file)"
+assert_equals 1 "$(get_linkcount link.gz)"
+assert_equals 1 "$(get_linkcount file)"
 cmp link.gz orig.gz
 
 
 begin_test 'Multiple files'
 cp file file2
 gzip file file2
 [ ! -e file ] && [ ! -e file2 ] && [ -e file.gz ] && [ -e file2.gz ]
@@ -359,27 +394,29 @@
 rmdir 1
 mkdir 1.gz
 assert_skipped gunzip 1.gz 2.gz
 [ ! -e 1 ]
 cmp 2 file
 
 
-begin_test 'Multiple files, continue on error'
-cp file 1
-cp file 2
-chmod a-r 1
-assert_error 'Permission denied' gzip 1 2
-[ ! -e 1.gz ]
-cmp file <(gunzip -c 2.gz)
-rm -f 1
-cp 2.gz 1.gz
-chmod a-r 1.gz
-assert_error 'Permission denied' gunzip 1.gz 2.gz
-[ ! -e 1 ]
-cmp 2 file
+if (( $(id -u) != 0 )); then
+	begin_test 'Multiple files, continue on error'
+	cp file 1
+	cp file 2
+	chmod a-r 1
+	assert_error 'Permission denied' gzip 1 2
+	[ ! -e 1.gz ]
+	cmp file <(gunzip -c 2.gz)
+	rm -f 1
+	cp 2.gz 1.gz
+	chmod a-r 1.gz
+	assert_error 'Permission denied' gunzip 1.gz 2.gz
+	[ ! -e 1 ]
+	cmp 2 file
+fi
 
 
 begin_test 'Compressing empty file'
 echo -n > empty
 gzip empty
 gunzip empty.gz
 cmp /dev/null empty
@@ -389,18 +426,16 @@
 echo -n > foo.gz
 assert_error '\<(not in gzip format|unexpected end of file)\>' \
 	gunzip foo.gz
 echo 1 > foo.gz
 assert_error '\<not in gzip format\>' gunzip foo.gz
 echo abcdefgh > foo.gz
 assert_error '\<not in gzip format\>' gunzip foo.gz
-xxd -r > foo.gz <<-EOF
-00000000: 1f8b 0800 0000 0000 00ff 4b4c 4a4e 4924  ..........KLJNI$
-00000010: 1673 0100 6c5b a262 2e00 0000            .s..l[.b....
-EOF
+echo -ne '\x1f\x8b\x08\x00\x00\x00\x00\x00\x00\xff\x4b\x4c\x4a\x4e\x49\x24\x16\x73\x01\x00\x6c\x5b\xa2\x62\x2e\x00\x00\x00' \
+	> foo.gz
 assert_error '\<(not in gzip format|crc error)\>' gunzip foo.gz
 
 
 for suf in .foo foo .blaaaaaaaaaaaaaaaargh; do
 	begin_test "Custom suffix: $suf"
 	gzip -S $suf file
 	[ ! -e file ] && [ ! -e file.gz ] && [ -e file$suf ]
@@ -413,28 +448,20 @@
 
 begin_test 'Empty suffix is rejected'
 assert_error '\<invalid suffix\>' gzip -S '""' file
 assert_error '\<invalid suffix\>' gunzip -S '""' file
 
 
 begin_test 'Timestamps and mode are preserved'
-if [ "$FSTYPE" = shiftfs ]; then
-	# In Travis CI, the filesystem (shiftfs) only supports seconds precision
-	# timestamps.  Nanosecond precision still sometimes seems to work,
-	# probably due to caching, but it is unreliable.
-	format='%a;%X;%Y'
-else
-	format='%a;%x;%y'
-fi
 chmod 777 file
-orig_stat="$(stat -c "$format" file)"
+orig_stat=$(get_modeandtimestamps file)
 gzip file
 sleep 1
 gunzip file.gz
-assert_equals "$orig_stat" "$(stat -c "$format" file)"
+assert_equals "$orig_stat" "$(get_modeandtimestamps file)"
 
 
 begin_test 'Decompressing multi-member gzip file'
 cat file file > orig
 gzip -c file > file.gz
 gzip -c file >> file.gz
 gunzip -f file.gz
@@ -459,12 +486,38 @@
 for prog in gzip gunzip; do
 	for opt in '--invalid-option' '-0'; do
 		assert_error '\<(unrecognized|invalid) option\>' $prog $opt
 	done
 done
 
 
+begin_test '-t (test) option works'
+good_files=(
+'H4sIAAAAAAAAA3PMSVTITVTIzi9JVABTIJ5jzpGZelwAX+86ehsAAAA='
+'H4sIAAAAAAAAAwvJSFUoLM1MzlZIKsovz1NIy69QyCrNLShWyC9LLVIoAUrnJFZVKqTkp+txAQBqzFDrLQAAAA==')
+bad_files=(
+'H4sIAO1YYmAAA3PMSVTITVTIzi9JVABTIJ5jzpGZelwAX+46ehsAAAA='
+'H4sIAO1YYmAAA3PMSVTITVTIzi85VABTIJ5jzpGZelwAX+86ehsAAAA='
+'H4sIAAAAAAAAA3PMSVTITVTIzi9JVABTIJ5jzpGZelwAX+86ehsBAAA='
+'H4sIAAAAAAAAAwvJSFUoLM1MzlZIKsovz1NIy69QyCrNLShWyC9LLVIogUrnJFZVKqTkp+txAQBqzFDrLQAAAA=='
+'H4sIAAAAAAAAAwvJSFUoLM1MzlZIKsovz1NIy69QyCrNLShWyC9L')
+for contents in "${good_files[@]}"; do
+	echo "$contents" | base64 -d | gzip -t
+done
+for contents in "${bad_files[@]}"; do
+	echo "$contents" | base64 -d > file
+	assert_error '\<invalid compressed data|file corrupt|unexpected end of file|Out of memory\>' \
+		gzip -t file
+done
+
+
+begin_test '-q (quiet) option works'
+mkdir dir
+gunzip -q dir &> output || true
+[ ! -s output ]
+
+
 begin_test 'Version information'
 gzip -V | grep -q Copyright
 gunzip -V | grep -q Copyright
 
 CURRENT_TEST=
```

