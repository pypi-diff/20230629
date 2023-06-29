# Comparing `tmp/sim-ldpc-0.3.4.tar.gz` & `tmp/sim-ldpc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim-ldpc-0.3.4.tar", last modified: Sat Feb 11 18:38:12 2023, max compression
+gzip compressed data, was "sim-ldpc-0.3.5.tar", last modified: Thu Jun 29 16:29:02 2023, max compression
```

## Comparing `sim-ldpc-0.3.4.tar` & `sim-ldpc-0.3.5.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.076413 sim-ldpc-0.3.4/
--rw-r--r--   0 yairmazal   (501) staff       (20)     1063 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/LICENSE
--rw-r--r--   0 yairmazal   (501) staff       (20)       47 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/MANIFEST.in
--rw-r--r--   0 yairmazal   (501) staff       (20)     5050 2023-02-11 18:38:12.076545 sim-ldpc-0.3.4/PKG-INFO
--rw-r--r--   0 yairmazal   (501) staff       (20)     4366 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/README.md
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.034937 sim-ldpc-0.3.4/ldpc/
--rw-r--r--   0 yairmazal   (501) staff       (20)      142 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/__init__.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      666 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/base_code.py
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.041359 sim-ldpc-0.3.4/ldpc/code_specs/
--rw-r--r--   0 yairmazal   (501) staff       (20)   150794 2022-03-10 18:23:20.000000 sim-ldpc-0.3.4/ldpc/code_specs/4098_3095_non_sys_h.alist
--rw-r--r--   0 yairmazal   (501) staff       (20)     1947 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/Mackay_96.3.963.alist
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.067558 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/
--rw-r--r--   0 yairmazal   (501) staff       (20)      836 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1296_R12.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      553 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1296_R23.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      411 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1296_R34.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      270 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1296_R56.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      838 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1944_R12.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      557 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1944_R23.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      418 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1944_R34.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      279 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1944_R56.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      817 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N648_R12.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      548 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N648_R23.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      395 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N648_R34.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)      257 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N648_R56.qc
--rw-r--r--   0 yairmazal   (501) staff       (20)  1263745 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/code_specs/ieee802.3_G.alist
--rw-r--r--   0 yairmazal   (501) staff       (20)  8696104 2022-03-10 16:09:49.000000 sim-ldpc-0.3.4/ldpc/code_specs/systematic_4098_3095.alist
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.069495 sim-ldpc-0.3.4/ldpc/decoder/
--rw-r--r--   0 yairmazal   (501) staff       (20)      271 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/decoder/__init__.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      701 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/decoder/channel_models.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     5908 2023-02-11 16:38:06.000000 sim-ldpc-0.3.4/ldpc/decoder/graph.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     1363 2022-04-05 12:34:54.000000 sim-ldpc-0.3.4/ldpc/decoder/ieee802_11_decoder.py
--rwxr-xr-x   0 yairmazal   (501) staff       (20)     5606 2023-02-11 16:14:17.000000 sim-ldpc-0.3.4/ldpc/decoder/log_spa_decoder.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     6504 2022-11-06 11:56:46.000000 sim-ldpc-0.3.4/ldpc/decoder/node.py
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.071004 sim-ldpc-0.3.4/ldpc/encoder/
--rw-r--r--   0 yairmazal   (501) staff       (20)      302 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/encoder/__init__.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      635 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/encoder/base_encoder.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      986 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/encoder/generator_based_encoder.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     1575 2022-11-06 11:56:46.000000 sim-ldpc-0.3.4/ldpc/encoder/h_based_encoder.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     3565 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/encoder/ieee802_11_encoder.py
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.072537 sim-ldpc-0.3.4/ldpc/utils/
--rw-r--r--   0 yairmazal   (501) staff       (20)      376 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/utils/__init__.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     6516 2023-02-11 14:06:45.000000 sim-ldpc-0.3.4/ldpc/utils/a_list_format.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      241 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/utils/custom_exceptions.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     1981 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/utils/frame.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     3979 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/utils/qc_format.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      354 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/ldpc/wifi_spec_codes.py
--rw-r--r--   0 yairmazal   (501) staff       (20)       79 2023-02-11 18:38:12.077010 sim-ldpc-0.3.4/setup.cfg
--rw-r--r--   0 yairmazal   (501) staff       (20)     1187 2023-02-11 16:48:54.000000 sim-ldpc-0.3.4/setup.py
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.074276 sim-ldpc-0.3.4/sim_ldpc.egg-info/
--rw-r--r--   0 yairmazal   (501) staff       (20)     5050 2023-02-11 18:38:12.000000 sim-ldpc-0.3.4/sim_ldpc.egg-info/PKG-INFO
--rw-r--r--   0 yairmazal   (501) staff       (20)     1464 2023-02-11 18:38:12.000000 sim-ldpc-0.3.4/sim_ldpc.egg-info/SOURCES.txt
--rw-r--r--   0 yairmazal   (501) staff       (20)        1 2023-02-11 18:38:12.000000 sim-ldpc-0.3.4/sim_ldpc.egg-info/dependency_links.txt
--rw-r--r--   0 yairmazal   (501) staff       (20)       31 2023-02-11 18:38:12.000000 sim-ldpc-0.3.4/sim_ldpc.egg-info/requires.txt
--rw-r--r--   0 yairmazal   (501) staff       (20)        5 2023-02-11 18:38:12.000000 sim-ldpc-0.3.4/sim_ldpc.egg-info/top_level.txt
-drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-02-11 18:38:12.076139 sim-ldpc-0.3.4/tests/
--rw-r--r--   0 yairmazal   (501) staff       (20)     3002 2022-11-06 11:56:46.000000 sim-ldpc-0.3.4/tests/test_a_list.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     2445 2022-11-06 11:56:46.000000 sim-ldpc-0.3.4/tests/test_encoders.py
--rw-r--r--   0 yairmazal   (501) staff       (20)      875 2022-03-28 15:49:58.000000 sim-ldpc-0.3.4/tests/test_frames.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     7009 2022-11-06 11:56:46.000000 sim-ldpc-0.3.4/tests/test_ieee802_11.py
--rw-r--r--   0 yairmazal   (501) staff       (20)     2576 2022-11-06 11:56:46.000000 sim-ldpc-0.3.4/tests/test_qcfile.py
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.151043 sim-ldpc-0.3.5/
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1063 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/LICENSE
+-rw-r--r--   0 yairmazal   (501) staff       (20)       47 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/MANIFEST.in
+-rw-r--r--   0 yairmazal   (501) staff       (20)     5267 2023-06-29 16:29:02.151243 sim-ldpc-0.3.5/PKG-INFO
+-rw-r--r--   0 yairmazal   (501) staff       (20)     4583 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/README.md
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.098924 sim-ldpc-0.3.5/ldpc/
+-rw-r--r--   0 yairmazal   (501) staff       (20)      142 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/__init__.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)      666 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/base_code.py
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.106031 sim-ldpc-0.3.5/ldpc/code_specs/
+-rw-r--r--   0 yairmazal   (501) staff       (20)   150794 2022-03-10 18:23:20.000000 sim-ldpc-0.3.5/ldpc/code_specs/4098_3095_non_sys_h.alist
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1947 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/Mackay_96.3.963.alist
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.128020 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/
+-rw-r--r--   0 yairmazal   (501) staff       (20)      836 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1296_R12.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      553 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1296_R23.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      411 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1296_R34.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      270 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1296_R56.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      838 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1944_R12.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      557 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1944_R23.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      418 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1944_R34.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      279 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1944_R56.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      817 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N648_R12.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      548 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N648_R23.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      395 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N648_R34.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)      257 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N648_R56.qc
+-rw-r--r--   0 yairmazal   (501) staff       (20)  1263745 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/code_specs/ieee802.3_G.alist
+-rw-r--r--   0 yairmazal   (501) staff       (20)  8696104 2022-03-10 16:09:49.000000 sim-ldpc-0.3.5/ldpc/code_specs/systematic_4098_3095.alist
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.134896 sim-ldpc-0.3.5/ldpc/decoder/
+-rw-r--r--   0 yairmazal   (501) staff       (20)      565 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/ldpc/decoder/__init__.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1350 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/decoder/common.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     3277 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/decoder/gal_bf.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     5896 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/decoder/graph.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1355 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/decoder/ieee802_11_decoder.py
+-rwxr-xr-x   0 yairmazal   (501) staff       (20)     5441 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/decoder/log_spa_decoder.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     6506 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/decoder/node.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     8592 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/ldpc/decoder/pbf_decoder.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     9770 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/ldpc/decoder/wbf.py
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.138625 sim-ldpc-0.3.5/ldpc/encoder/
+-rw-r--r--   0 yairmazal   (501) staff       (20)      302 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/encoder/__init__.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)      684 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/encoder/base_encoder.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)      971 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/encoder/generator_based_encoder.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1489 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/encoder/h_based_encoder.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     3513 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/encoder/ieee802_11_encoder.py
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.142169 sim-ldpc-0.3.5/ldpc/utils/
+-rw-r--r--   0 yairmazal   (501) staff       (20)      376 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/utils/__init__.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     6516 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/utils/a_list_format.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)      241 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/utils/custom_exceptions.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1965 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/ldpc/utils/frame.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     3979 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/utils/qc_format.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)      354 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/ldpc/wifi_spec_codes.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)       79 2023-06-29 16:29:02.151971 sim-ldpc-0.3.5/setup.cfg
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1187 2023-06-29 16:27:45.000000 sim-ldpc-0.3.5/setup.py
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.144975 sim-ldpc-0.3.5/sim_ldpc.egg-info/
+-rw-r--r--   0 yairmazal   (501) staff       (20)     5267 2023-06-29 16:29:02.000000 sim-ldpc-0.3.5/sim_ldpc.egg-info/PKG-INFO
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1600 2023-06-29 16:29:02.000000 sim-ldpc-0.3.5/sim_ldpc.egg-info/SOURCES.txt
+-rw-r--r--   0 yairmazal   (501) staff       (20)        1 2023-06-29 16:29:02.000000 sim-ldpc-0.3.5/sim_ldpc.egg-info/dependency_links.txt
+-rw-r--r--   0 yairmazal   (501) staff       (20)       31 2023-06-29 16:29:02.000000 sim-ldpc-0.3.5/sim_ldpc.egg-info/requires.txt
+-rw-r--r--   0 yairmazal   (501) staff       (20)        5 2023-06-29 16:29:02.000000 sim-ldpc-0.3.5/sim_ldpc.egg-info/top_level.txt
+drwxr-xr-x   0 yairmazal   (501) staff       (20)        0 2023-06-29 16:29:02.150531 sim-ldpc-0.3.5/tests/
+-rw-r--r--   0 yairmazal   (501) staff       (20)     2988 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/tests/test_a_list.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     2399 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/tests/test_encoders.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)      875 2023-06-15 16:47:47.000000 sim-ldpc-0.3.5/tests/test_frames.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     1939 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/tests/test_gal_bf.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     7029 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/tests/test_ieee802_11.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     3453 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/tests/test_pbf_decoder.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     2578 2023-06-27 14:58:24.000000 sim-ldpc-0.3.5/tests/test_qcfile.py
+-rw-r--r--   0 yairmazal   (501) staff       (20)     5295 2023-06-19 20:10:18.000000 sim-ldpc-0.3.5/tests/test_wbf_decoder.py
```

### Comparing `sim-ldpc-0.3.4/LICENSE` & `sim-ldpc-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/PKG-INFO` & `sim-ldpc-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sim-ldpc
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simulate LDPC codes, both encoding and decoding
 Home-page: https://github.com/YairMZ/LDPC
 Author: Yair Mazal
 Author-email: yairmazal@gmail.com
 License: MIT
 Keywords: LDPC,Belief Propagation,SPA,Tanner Graph,IEEE 802.11
 Classifier: License :: OSI Approved :: MIT License
@@ -48,30 +48,34 @@
 ```
 
 -----
 ## Included modules
  - [Utilities](ldpc/utils/README.md): implementing various utility operations to assist with encoding, decoding and 
 simulations.
  - [Encoder](ldpc/encoder/README.md): implementing a generator based encoder, and encoders for IEEE802.11 (WiFi) LDPC codes.
- - [Decoder](ldpc/decoder/README.md): implementing a Log-SPA based BP decoder.
-
+ - [Decoder](ldpc/decoder/README.md): implementing several decoders
+   - Log-SPA based BP decoder
+   - MS decodcer
+   - Gallager bit filpping decoder
+   - Weighted bit flipping decoders, several variants
+   - Parallel probabilistic bit flipping decoder (PPBF)
 -----
 
 ## Basic Example
 ```python
 import numpy as np
 from bitstring import BitArray, Bits
 from ldpc.decoder import DecoderWiFi, bsc_llr
 from ldpc.encoder import EncoderWiFi
 from ldpc.wifi_spec_codes import WiFiSpecCode
 from ldpc.utils import QCFile
 
 # create information bearing bits
 rng = np.random.default_rng()
-info_bits = Bits(bytes=rng.bytes(41))[:648//2]
+info_bits = np.array(Bits(bytes=rng.bytes(41))[:648//2], dtype=np.int_)
 # create encoder with frame of 648 bits, and rate 1/2. Possible rates and frame sizes are per the ieee802.11n spec.
 enc = EncoderWiFi(WiFiSpecCode.N648_R12)
 # encode bits
 encoded = enc.encode(info_bits)
 
 # verify validity of codeword
 h = enc.h
@@ -86,24 +90,24 @@
 corrupted = BitArray(encoded)
 no_errors = int(len(corrupted)*p)
 error_idx = rng.choice(len(corrupted), size=no_errors, replace=False)
 for idx in error_idx:
     corrupted[idx] = not corrupted[idx]
 decoded, llr, decode_success, num_of_iterations, syndrome, vnode_validity  = decoder.decode(corrupted)
 # Verify correct decoding
-print(Bits(decoded) == encoded)  # true
+print(Bits(decoded) == Bits(encoded))  # true
 info = decoder.info_bits(decoded)
 
 # a decoder can also be instantiated without a channel model, in which case llr is expected to be sent for decoding instead of
 # hard channel outputs.
 channel = bsc_llr(p=p)
 channel_llr = channel(np.array(corrupted, dtype=np.int_))
 decoder = DecoderWiFi(spec=WiFiSpecCode.N648_R12, max_iter=20)
 decoded, llr2, decode_success, num_of_iterations, syndrome, vnode_validity  = decoder.decode(channel_llr)
-print(Bits(decoded) == encoded)  # true
+print(Bits(decoded) == Bits(encoded))  # true
 info = decoder.info_bits(decoded)
 ```
 The example is also included as a jupyter notebook. Note however, that you need to launch the notebook from the correct 
 path for it to be able to access installed packages. To run the notebook:
 1. create a new virtualenv
 ```shell
 python3 -m venv ~/.virtualenv/LDPC_env
```

### Comparing `sim-ldpc-0.3.4/README.md` & `sim-ldpc-0.3.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -29,30 +29,34 @@
 ```
 
 -----
 ## Included modules
  - [Utilities](ldpc/utils/README.md): implementing various utility operations to assist with encoding, decoding and 
 simulations.
  - [Encoder](ldpc/encoder/README.md): implementing a generator based encoder, and encoders for IEEE802.11 (WiFi) LDPC codes.
- - [Decoder](ldpc/decoder/README.md): implementing a Log-SPA based BP decoder.
-
+ - [Decoder](ldpc/decoder/README.md): implementing several decoders
+   - Log-SPA based BP decoder
+   - MS decodcer
+   - Gallager bit filpping decoder
+   - Weighted bit flipping decoders, several variants
+   - Parallel probabilistic bit flipping decoder (PPBF)
 -----
 
 ## Basic Example
 ```python
 import numpy as np
 from bitstring import BitArray, Bits
 from ldpc.decoder import DecoderWiFi, bsc_llr
 from ldpc.encoder import EncoderWiFi
 from ldpc.wifi_spec_codes import WiFiSpecCode
 from ldpc.utils import QCFile
 
 # create information bearing bits
 rng = np.random.default_rng()
-info_bits = Bits(bytes=rng.bytes(41))[:648//2]
+info_bits = np.array(Bits(bytes=rng.bytes(41))[:648//2], dtype=np.int_)
 # create encoder with frame of 648 bits, and rate 1/2. Possible rates and frame sizes are per the ieee802.11n spec.
 enc = EncoderWiFi(WiFiSpecCode.N648_R12)
 # encode bits
 encoded = enc.encode(info_bits)
 
 # verify validity of codeword
 h = enc.h
@@ -67,24 +71,24 @@
 corrupted = BitArray(encoded)
 no_errors = int(len(corrupted)*p)
 error_idx = rng.choice(len(corrupted), size=no_errors, replace=False)
 for idx in error_idx:
     corrupted[idx] = not corrupted[idx]
 decoded, llr, decode_success, num_of_iterations, syndrome, vnode_validity  = decoder.decode(corrupted)
 # Verify correct decoding
-print(Bits(decoded) == encoded)  # true
+print(Bits(decoded) == Bits(encoded))  # true
 info = decoder.info_bits(decoded)
 
 # a decoder can also be instantiated without a channel model, in which case llr is expected to be sent for decoding instead of
 # hard channel outputs.
 channel = bsc_llr(p=p)
 channel_llr = channel(np.array(corrupted, dtype=np.int_))
 decoder = DecoderWiFi(spec=WiFiSpecCode.N648_R12, max_iter=20)
 decoded, llr2, decode_success, num_of_iterations, syndrome, vnode_validity  = decoder.decode(channel_llr)
-print(Bits(decoded) == encoded)  # true
+print(Bits(decoded) == Bits(encoded))  # true
 info = decoder.info_bits(decoded)
 ```
 The example is also included as a jupyter notebook. Note however, that you need to launch the notebook from the correct 
 path for it to be able to access installed packages. To run the notebook:
 1. create a new virtualenv
 ```shell
 python3 -m venv ~/.virtualenv/LDPC_env
```

### Comparing `sim-ldpc-0.3.4/ldpc/base_code.py` & `sim-ldpc-0.3.5/ldpc/base_code.py`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/4098_3095_non_sys_h.alist` & `sim-ldpc-0.3.5/ldpc/code_specs/4098_3095_non_sys_h.alist`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/Mackay_96.3.963.alist` & `sim-ldpc-0.3.5/ldpc/code_specs/Mackay_96.3.963.alist`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1296_R12.qc` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1296_R12.qc`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1296_R23.qc` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1296_R23.qc`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1944_R12.qc` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1944_R12.qc`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N1944_R23.qc` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N1944_R23.qc`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N648_R12.qc` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N648_R12.qc`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.11/N648_R23.qc` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.11/N648_R23.qc`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/ieee802.3_G.alist` & `sim-ldpc-0.3.5/ldpc/code_specs/ieee802.3_G.alist`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/code_specs/systematic_4098_3095.alist` & `sim-ldpc-0.3.5/ldpc/code_specs/systematic_4098_3095.alist`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/decoder/graph.py` & `sim-ldpc-0.3.5/ldpc/decoder/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import networkx as nx
 from ldpc.decoder.node import VNode, CNode
 import numpy as np
 import numpy.typing as npt
 from typing import Optional, Union
-from ldpc.decoder.channel_models import ChannelModel
+from ldpc.decoder.common import ChannelModel
 import scipy as sp
 
 
 __all__ = ["TannerGraph"]
 
 Edge = tuple[int, int]
 EdgesSet = set[tuple[int, int]]
@@ -114,15 +114,15 @@
             ordered_vnode_uid[i] = v_uid
         if isinstance(h, np.ndarray):
             for j in range(m):
                 c_uid = g.add_c_node(name=f"c{j}", ordering_key=j, decoder=decoder).uid
                 for i in range(n):
                     if h[j, i] == 1:
                         g.add_edge(ordered_vnode_uid[i], c_uid)
-        if isinstance(h, sp.sparse.lil.lil_matrix):
+        if isinstance(h, sp.sparse.lil_matrix):
             for j in range(m):
                 c_uid = g.add_c_node(name=f"c{j}", ordering_key=j, decoder=decoder).uid
                 for col in h.rows[j]:
                     g.add_edge(ordered_vnode_uid[col], c_uid)
         return g
 
     def __str__(self) -> str:
```

### Comparing `sim-ldpc-0.3.4/ldpc/decoder/ieee802_11_decoder.py` & `sim-ldpc-0.3.5/ldpc/decoder/ieee802_11_decoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ldpc.decoder.log_spa_decoder import LogSpaDecoder
 import numpy as np
-from ldpc.decoder.channel_models import ChannelModel
+from ldpc.decoder.common import ChannelModel
 from ldpc.wifi_spec_codes import WiFiSpecCode
 import os
 from ldpc.utils.qc_format import QCFile
 from typing import Optional
 
 
 class DecoderWiFi(LogSpaDecoder):
```

### Comparing `sim-ldpc-0.3.4/ldpc/decoder/log_spa_decoder.py` & `sim-ldpc-0.3.5/ldpc/decoder/log_spa_decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from ldpc.decoder.graph import TannerGraph
 from numpy.typing import ArrayLike, NDArray
 import numpy as np
 from collections.abc import Sequence
-from ldpc.decoder.channel_models import ChannelModel
+from ldpc.decoder.common import ChannelModel, InfoBitsNotSpecified
 from typing import Optional
-from bitstring import Bits
 from ldpc.utils import IncorrectLength
 from ldpc.decoder.node import VNode
 import numpy.typing as npt
 
-__all__ = ["LogSpaDecoder", "InfoBitsNotSpecified"]
-
-
-class InfoBitsNotSpecified(Exception):
-    """Raised when a non-binary matrix is used while a binary one expected"""
-    pass
+__all__ = ["LogSpaDecoder"]
 
 
 class LogSpaDecoder:
     """Decode codewords according to Log-SPA version of the belief propagation algorithm"""
     def __init__(self, h: ArrayLike, max_iter: int, info_idx: Optional[NDArray[np.bool_]] = None,
                  channel_model: Optional[ChannelModel] = None, decoder_type: Optional[str] = "BP"):
         """
@@ -50,15 +44,15 @@
         :return: return a tuple (estimated_bits, llr, decode_success, no_iterations)
         where:
             - estimated_bits is a 1-d np array of hard bit estimates
             - llr is a 1-d np array of soft bit estimates
             - decode_success is a boolean flag stating of the estimated_bits form a valid  code word
             - no_iterations is the number of iterations of belief propagation before exiting the loop
             - syndrome
-            - a measure of validity of each vnode, higher is better
+            - a measure of validity of each vnode, lower is better
         """
         if len(channel_word) != self.n:
             raise IncorrectLength("incorrect block size")
 
         # initial step
         for idx, vnode in enumerate(self._ordered_vnodes):
             vnode.initialize(channel_word[idx])
@@ -90,18 +84,18 @@
         #
         # for idx, vnode in enumerate(self._ordered_vnodes):
         #     neighbors = vnode.get_neighbors()
         #     for neighbor in neighbors:
         #         vnode_validity[idx] += 2*syndrome_compliance[neighbor] - 1
         return estimate, llr, not syndrome.any(), iteration+1, syndrome, vnode_validity
 
-    def info_bits(self, estimate: NDArray[np.int_]) -> Bits:
+    def info_bits(self, estimate: NDArray[np.int_]) -> NDArray[np.int_]:
         """extract information bearing bits from decoded estimate, assuming info bits indices were specified"""
         if self.info_idx is not None:
-            return Bits(auto=estimate[self.info_idx])
+            return estimate[self.info_idx]
         else:
             raise InfoBitsNotSpecified("decoder cannot tell info bits")
 
     def ordered_vnodes(self) -> list[VNode]:
         """getter for ordered graph v-nodes"""
         return self._ordered_vnodes
```

### Comparing `sim-ldpc-0.3.4/ldpc/decoder/node.py` & `sim-ldpc-0.3.5/ldpc/decoder/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import numpy as np
 import itertools
 from typing import Any, Optional, Tuple
 from functools import total_ordering
 from abc import ABC, abstractmethod
 import numpy.typing as npt
-from ldpc.decoder.channel_models import ChannelModel
+from ldpc.decoder.common import ChannelModel
 from numba import jit
 
 
 __all__ = ["Node", "CNode", "VNode"]
 
 
 @jit(nopython=True, cache=True)  # type: ignore
@@ -18,15 +18,15 @@
     return -np.prod(np.sign(q)) * np.log(  # type: ignore
         np.maximum(np.tanh(
             sum(
                 -np.log(np.maximum(np.tanh(np.absolute(q) / 2), 1e3 * np.finfo(np.float_).eps))
             ) / 2), 1e3 * np.finfo(np.float_).eps))
 
 
-@total_ordering  # type: ignore
+@total_ordering
 class Node(ABC):
     """Base class VNodes anc CNodes.
     Derived classes are expected to implement an "initialize" and  method a "message" which should return the message to
     be passed on the graph.
     Nodes are ordered and deemed equal according to their ordering_key.
     """
     _uid_generator = itertools.count()
@@ -106,15 +106,16 @@
         :param requester_uid: uid of requesting v-node
         """
         if self.decoder_type == "MS":
             q: npt.NDArray[np.float_] = np.array([msg for uid, msg in self.received_messages.items() if uid != requester_uid])
             return np.prod(np.sign(q)) * np.absolute(q).min()   # type: ignore
 
         # full BP
-        return c_message(requester_uid, tuple(self.received_messages.keys()), tuple(self.received_messages.values()))  # type: ignore
+        return c_message(requester_uid, tuple(self.received_messages.keys()), tuple(self.received_messages.values())
+                         )  # type: ignore
 
         # def phi(x: npt.NDArray[np.float_]) -> npt.NDArray[np.float_]:
         #     """see sources for definition and reasons for use of this function"""
         #     return -np.log(np.maximum(np.tanh(x / 2), 1e3 * np.finfo(np.float_).eps))
         # return np.prod(np.sign(q))*phi(sum(phi(np.absolute(q))))  # type: ignore
 
         # return -np.prod(np.sign(q)) * np.log(
```

### Comparing `sim-ldpc-0.3.4/ldpc/encoder/generator_based_encoder.py` & `sim-ldpc-0.3.5/ldpc/encoder/generator_based_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import bitstring
-
 from ldpc.encoder.base_encoder import Encoder
 import numpy as np
-import numpy.typing as npt
-from bitstring import Bits
+from numpy.typing import NDArray
 from ldpc.utils.custom_exceptions import NonBinaryMatrix, IncorrectLength
 
 
 class EncoderG(Encoder):
     """Encoder which is based on multiplying the generator matrix by message bits"""
-    def __init__(self, generator: npt.NDArray[np.int_]) -> None:
+    def __init__(self, generator: NDArray[np.int_]) -> None:
         """
         :param generator: generator matrix, should be a binary matrix
         :raises: NonBinaryMatrix if matrix elements are non-binary
         """
         self.generator = generator
         if generator.max(initial=0) > 1 or generator.min(initial=1) < 0:
             raise NonBinaryMatrix
         k, n = generator.shape
         super().__init__(k, n)
 
-    def encode(self, information_bits: Bits) -> Bits:
+    def encode(self, information_bits: NDArray[np.int_]) -> NDArray[np.int_]:
         if len(information_bits) != self.k:
             raise IncorrectLength
-        return bitstring.Bits(np.matmul(np.array(information_bits, dtype=np.int_), self.generator))
+        return np.matmul(np.array(information_bits, dtype=np.int_), self.generator) % 2  # type: ignore
```

### Comparing `sim-ldpc-0.3.4/ldpc/encoder/h_based_encoder.py` & `sim-ldpc-0.3.5/ldpc/encoder/h_based_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from ldpc.encoder.base_encoder import Encoder
-import numpy.typing as npt
+from numpy.typing import NDArray
 import numpy as np
-from bitstring import Bits
 from ldpc.utils.custom_exceptions import IncorrectLength, NonBinaryMatrix
 
 
 class EncoderTriangularH(Encoder):
     """Encoder which encodes using back-substitution, given a parity check matrix in lower triangular form
     based on: "Efficient Encoding of Low-Density Parity-Check Codes"
     """
-    def __init__(self, h: npt.NDArray[np.int_]) -> None:
+    def __init__(self, h: NDArray[np.int_]) -> None:
         """
         :param h: parity check matrix, should be a lower triangular binary matrix
         :raises: NonBinaryMatrix if matrix elements are non-binary
         """
         self.h = h
         if h.max(initial=0) > 1 or h.min(initial=1) < 0:
             raise NonBinaryMatrix
@@ -21,19 +20,18 @@
         k = n - m
         self.m = m
         # check if parity part is identity
         self.identity_p = np.array_equal(h[:, k:], np.identity(m))
 
         super().__init__(k, n)
 
-    def encode(self, information_bits: Bits) -> Bits:
+    def encode(self, information_bits: NDArray[np.int_]) -> NDArray[np.int_]:
         if len(information_bits) != self.k:
             raise IncorrectLength
-        info: npt.NDArray[np.int_] = np.array(information_bits, dtype=np.int_)
-        encoded: npt.NDArray[np.int_] = np.zeros(self.n, dtype=np.int_)
-        encoded[:self.k] = info
-        p: npt.NDArray[np.int_] = np.mod(np.matmul(self.h[:, :self.k], info), 2)
+        encoded: NDArray[np.int_] = np.zeros(self.n, dtype=np.int_)
+        encoded[:self.k] = information_bits
+        p: NDArray[np.int_] = np.mod(np.matmul(self.h[:, :self.k], information_bits), 2)
         if not self.identity_p:
             for l in range(1, self.m):
-                p[l] += np.mod(np.dot(self.h[l, self.k:self.k+l], p[:l]), 2)  # type: ignore
+                p[l] += np.mod(np.dot(self.h[l, self.k:self.k+l], p[:l]), 2)
         encoded[self.k:] = p
-        return Bits(encoded)
+        return encoded
```

### Comparing `sim-ldpc-0.3.4/ldpc/encoder/ieee802_11_encoder.py` & `sim-ldpc-0.3.5/ldpc/encoder/ieee802_11_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from ldpc.encoder.base_encoder import Encoder
-import numpy.typing as npt
+from numpy.typing import NDArray
 import numpy as np
-from bitstring import Bits
 from ldpc.utils.custom_exceptions import IncorrectLength
 from ldpc.utils.qc_format import QCFile
 import os
-from numpy.typing import NDArray
 from ldpc.wifi_spec_codes import WiFiSpecCode
 from typing import Any
 
 
 class EncoderWiFi(Encoder):
     """Encode messages according to the codes in the IEEE802.11n standard"""
     _spec_base_path: str = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'code_specs', 'ieee802.11')
@@ -23,45 +21,45 @@
         self.h = qc_file.to_array()
         self.m, n = self.h.shape
         k = n - self.m
         self.z = qc_file.z
         self.block_structure = qc_file.block_structure
         super().__init__(k, n)
 
-    def encode(self, information_bits: Bits) -> Bits:
+    def encode(self, information_bits: NDArray[np.int_]) -> NDArray[np.int_]:
         """Based on: Efficient encoding of IEEE 802.11n LDPC codes,
         https://www.researchgate.net/publication/3389450_Efficient_encoding_of_IEEE_80211n_LDPC_codes
         """
         if len(information_bits) != self.k:
             raise IncorrectLength
 
         shifted_messages = self._shifted_messages(information_bits)
-        parities: npt.NDArray[np.int_] = np.zeros((self.m//self.z, self.z), dtype=np.int_)
+        parities: NDArray[np.int_] = np.zeros((self.m//self.z, self.z), dtype=np.int_)
         # special parts see article
         parities[0, :] = np.sum(shifted_messages, axis=0) % 2  # find first batch of z parity bits
         parities[1, :] = (shifted_messages[0, :] + np.roll(parities[0, :], -1)) % 2  # find second set of z parity bits
         parities[-1, :] = (shifted_messages[-1, :] + np.roll(parities[0, :], -1)) % 2  # find last set of z parity bits
         for idx in range(1, (self.m//self.z)-2):  # -1 needed to avoid exceeding memory limits due to idx+1 below.
             # -2 needed as bottom row is a special case.
             if self.block_structure[idx][self.k // self.z] >= 0:
                 # special treatment of x-th row, see article
                 parities[idx+1, :] = (parities[idx, :] + shifted_messages[idx, :] + parities[0, :]) % 2
             else:
                 parities[idx+1, :] = (parities[idx, :] + shifted_messages[idx, :]) % 2
 
-        return information_bits + Bits(np.ravel(parities))
+        return np.concatenate((information_bits, np.ravel(parities)))
 
-    def _shifted_messages(self, information_bits: Bits) -> NDArray[np.int_]:
+    def _shifted_messages(self, information_bits: NDArray[np.int_]) -> NDArray[np.int_]:
         # break message bits into groups (rows) of Z bits. Each row is a subset of z bits, overall k message bits
-        bit_blocks: npt.NDArray[np.int_] = np.array(information_bits, dtype=np.int_).reshape((self.k // self.z, self.z))
+        bit_blocks: NDArray[np.int_] = information_bits.reshape((self.k // self.z, self.z))
 
         # find shifted messages (termed lambda_i in article)
-        shifted_messages: npt.NDArray[np.int_] = np.zeros((self.m // self.z, self.z),
-                                                          dtype=np.int_)  # each row is a sum of circular shifts of
+        shifted_messages: NDArray[np.int_] = np.zeros((self.m // self.z, self.z),
+                                                      dtype=np.int_)  # each row is a sum of circular shifts of
         # message bits (some lambda_i in article). One row per block of h.
         for i in range(self.m // self.z):
             for j in range(self.k // self.z):
                 if self.block_structure[i][j] >= 0:  # zero blocks don't contribute to parity bits
                     # multiply by translation reduces to shift.
-                    vec: npt.NDArray[Any] = np.roll(bit_blocks[j, :], -self.block_structure[i][j])
+                    vec: NDArray[Any] = np.roll(bit_blocks[j, :], -self.block_structure[i][j])
                     shifted_messages[i, :] = np.logical_xor(shifted_messages[i, :], vec)  # xor as sum mod 2
         return shifted_messages
```

### Comparing `sim-ldpc-0.3.4/ldpc/utils/a_list_format.py` & `sim-ldpc-0.3.5/ldpc/utils/a_list_format.py`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/ldpc/utils/frame.py` & `sim-ldpc-0.3.5/ldpc/utils/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __str__(self) -> str:
         return "id: " + str(self.uid)
 
     def __eq__(self, other: object) -> bool:
         """Only bits are compared not uid"""
         if not isinstance(other, Frame):
             raise NotImplementedError
-        return self.bits == other.bits  # type: ignore
+        return self.bits == other.bits
 
 
 class FramesManager:
     """The class holds all frames in a dictionary with uid as key.
     It also holds a list of tuples, where each tuple contains a TX frame and a corresponding RX frame."""
     def __init__(self) -> None:
         self.frames_dict: dict[int, Frame] = {}
```

### Comparing `sim-ldpc-0.3.4/ldpc/utils/qc_format.py` & `sim-ldpc-0.3.5/ldpc/utils/qc_format.py`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/setup.py` & `sim-ldpc-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import pathlib
 
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).resolve().parent
 
 # The text of the README file is used as a description
 README = HERE.joinpath("README.md").read_text()
```

### Comparing `sim-ldpc-0.3.4/sim_ldpc.egg-info/PKG-INFO` & `sim-ldpc-0.3.5/sim_ldpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sim-ldpc
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simulate LDPC codes, both encoding and decoding
 Home-page: https://github.com/YairMZ/LDPC
 Author: Yair Mazal
 Author-email: yairmazal@gmail.com
 License: MIT
 Keywords: LDPC,Belief Propagation,SPA,Tanner Graph,IEEE 802.11
 Classifier: License :: OSI Approved :: MIT License
@@ -48,30 +48,34 @@
 ```
 
 -----
 ## Included modules
  - [Utilities](ldpc/utils/README.md): implementing various utility operations to assist with encoding, decoding and 
 simulations.
  - [Encoder](ldpc/encoder/README.md): implementing a generator based encoder, and encoders for IEEE802.11 (WiFi) LDPC codes.
- - [Decoder](ldpc/decoder/README.md): implementing a Log-SPA based BP decoder.
-
+ - [Decoder](ldpc/decoder/README.md): implementing several decoders
+   - Log-SPA based BP decoder
+   - MS decodcer
+   - Gallager bit filpping decoder
+   - Weighted bit flipping decoders, several variants
+   - Parallel probabilistic bit flipping decoder (PPBF)
 -----
 
 ## Basic Example
 ```python
 import numpy as np
 from bitstring import BitArray, Bits
 from ldpc.decoder import DecoderWiFi, bsc_llr
 from ldpc.encoder import EncoderWiFi
 from ldpc.wifi_spec_codes import WiFiSpecCode
 from ldpc.utils import QCFile
 
 # create information bearing bits
 rng = np.random.default_rng()
-info_bits = Bits(bytes=rng.bytes(41))[:648//2]
+info_bits = np.array(Bits(bytes=rng.bytes(41))[:648//2], dtype=np.int_)
 # create encoder with frame of 648 bits, and rate 1/2. Possible rates and frame sizes are per the ieee802.11n spec.
 enc = EncoderWiFi(WiFiSpecCode.N648_R12)
 # encode bits
 encoded = enc.encode(info_bits)
 
 # verify validity of codeword
 h = enc.h
@@ -86,24 +90,24 @@
 corrupted = BitArray(encoded)
 no_errors = int(len(corrupted)*p)
 error_idx = rng.choice(len(corrupted), size=no_errors, replace=False)
 for idx in error_idx:
     corrupted[idx] = not corrupted[idx]
 decoded, llr, decode_success, num_of_iterations, syndrome, vnode_validity  = decoder.decode(corrupted)
 # Verify correct decoding
-print(Bits(decoded) == encoded)  # true
+print(Bits(decoded) == Bits(encoded))  # true
 info = decoder.info_bits(decoded)
 
 # a decoder can also be instantiated without a channel model, in which case llr is expected to be sent for decoding instead of
 # hard channel outputs.
 channel = bsc_llr(p=p)
 channel_llr = channel(np.array(corrupted, dtype=np.int_))
 decoder = DecoderWiFi(spec=WiFiSpecCode.N648_R12, max_iter=20)
 decoded, llr2, decode_success, num_of_iterations, syndrome, vnode_validity  = decoder.decode(channel_llr)
-print(Bits(decoded) == encoded)  # true
+print(Bits(decoded) == Bits(encoded))  # true
 info = decoder.info_bits(decoded)
 ```
 The example is also included as a jupyter notebook. Note however, that you need to launch the notebook from the correct 
 path for it to be able to access installed packages. To run the notebook:
 1. create a new virtualenv
 ```shell
 python3 -m venv ~/.virtualenv/LDPC_env
```

### Comparing `sim-ldpc-0.3.4/sim_ldpc.egg-info/SOURCES.txt` & `sim-ldpc-0.3.5/sim_ldpc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 ldpc/code_specs/ieee802.11/N1944_R34.qc
 ldpc/code_specs/ieee802.11/N1944_R56.qc
 ldpc/code_specs/ieee802.11/N648_R12.qc
 ldpc/code_specs/ieee802.11/N648_R23.qc
 ldpc/code_specs/ieee802.11/N648_R34.qc
 ldpc/code_specs/ieee802.11/N648_R56.qc
 ldpc/decoder/__init__.py
-ldpc/decoder/channel_models.py
+ldpc/decoder/common.py
+ldpc/decoder/gal_bf.py
 ldpc/decoder/graph.py
 ldpc/decoder/ieee802_11_decoder.py
 ldpc/decoder/log_spa_decoder.py
 ldpc/decoder/node.py
+ldpc/decoder/pbf_decoder.py
+ldpc/decoder/wbf.py
 ldpc/encoder/__init__.py
 ldpc/encoder/base_encoder.py
 ldpc/encoder/generator_based_encoder.py
 ldpc/encoder/h_based_encoder.py
 ldpc/encoder/ieee802_11_encoder.py
 ldpc/utils/__init__.py
 ldpc/utils/a_list_format.py
@@ -42,9 +45,12 @@
 sim_ldpc.egg-info/SOURCES.txt
 sim_ldpc.egg-info/dependency_links.txt
 sim_ldpc.egg-info/requires.txt
 sim_ldpc.egg-info/top_level.txt
 tests/test_a_list.py
 tests/test_encoders.py
 tests/test_frames.py
+tests/test_gal_bf.py
 tests/test_ieee802_11.py
-tests/test_qcfile.py
+tests/test_pbf_decoder.py
+tests/test_qcfile.py
+tests/test_wbf_decoder.py
```

### Comparing `sim-ldpc-0.3.4/tests/test_a_list.py` & `sim-ldpc-0.3.5/tests/test_a_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                                               [0, 1],
                                               [2],
                                               [1, 2]]
         assert a.non_zero_elements_in_column == [[0, 1],
                                                  [0, 1, 3],
                                                  [0, 2, 3]]
         b = a.to_array()
-        np.testing.assert_array_equal(arr, b)  # type: ignore
+        np.testing.assert_array_equal(arr, b)
 
     def test_verify_alist(self) -> None:
         original_file = "ldpc/code_specs/Mackay_96.3.963.alist"
         a = AList.from_file(original_file)
         assert a.verify_elements() is True
 
     def test_sparse_arrays(self) -> None:
@@ -69,8 +69,8 @@
                                               [0, 1],
                                               [2],
                                               [1, 2]]
         assert a.non_zero_elements_in_column == [[0, 1],
                                                  [0, 1, 3],
                                                  [0, 2, 3]]
         b = a.to_sparse()
-        assert sp.spmatrix.sum(arr != b) == 0
+        assert sp.lil_matrix.sum(arr != b) == 0
```

### Comparing `sim-ldpc-0.3.4/tests/test_encoders.py` & `sim-ldpc-0.3.5/tests/test_encoders.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,54 +13,54 @@
             EncoderG(mat)
 
     def test_params(self) -> None:
         g = AList.from_file("tests/test_data/Hamming_7_4_g.alist").to_array()
         enc = EncoderG(g)
         assert enc.n == 7
         assert enc.k == 4
-        np.testing.assert_array_equal(g, enc.generator)  # type: ignore
+        np.testing.assert_array_equal(g, enc.generator)
 
     def test_encoding(self) -> None:
         g = AList.from_file("tests/test_data/Hamming_7_4_g.alist").to_array()
         enc = EncoderG(g)
         bits: npt.NDArray[np.int_] = np.array([1, 1, 0, 1])
-        encoded = np.matmul(bits, g)
-        res = enc.encode(Bits(bits))
-        assert res == Bits(encoded)
+        encoded = np.matmul(bits, g) % 2
+        res = enc.encode(bits)
+        assert Bits(res) == Bits(encoded)
 
     def test_incorrect_length(self) -> None:
         g = AList.from_file("tests/test_data/Hamming_7_4_g.alist").to_array()
         enc = EncoderG(g)
         bits: npt.NDArray[np.int_] = np.array([1, 1, 0])
         with pytest.raises(IncorrectLength):
-            enc.encode(Bits(bits))
+            enc.encode(bits)
 
 
 class TestEncoderTriangularH:
     def test_non_binary_matrix(self) -> None:
         mat = np.arange(1, 5).reshape((2, 2))
         with pytest.raises(NonBinaryMatrix):
             EncoderTriangularH(mat)
 
     def test_params(self) -> None:
         h = AList.from_file("tests/test_data/systematic_4098_3095.alist").to_array()
         enc = EncoderTriangularH(h)
         assert enc.n == 4098
         assert enc.m == 3095
         assert enc.k == 4098-3095
-        np.testing.assert_array_equal(h, enc.h)  # type: ignore
+        np.testing.assert_array_equal(h, enc.h)
 
     def test_encoding(self) -> None:
         h = AList.from_file("tests/test_data/systematic_4098_3095.alist").to_array()
         enc = EncoderTriangularH(h)
         bits: npt.NDArray[np.int_] = np.random.randint(2, size=enc.k)
-        encoded = enc.encode(Bits(bits))
+        encoded = enc.encode(bits)
         s = np.mod(np.matmul(h, encoded), 2)
         assert s.max() == 0
         assert s.min() == 0
 
     def test_incorrect_length(self) -> None:
         h = AList.from_file("tests/test_data/systematic_4098_3095.alist").to_array()
         enc = EncoderTriangularH(h)
         bits: npt.NDArray[np.int_] = np.array([1, 1, 0])
         with pytest.raises(IncorrectLength):
-            enc.encode(Bits(bits))
+            enc.encode(bits)
```

### Comparing `sim-ldpc-0.3.4/tests/test_frames.py` & `sim-ldpc-0.3.5/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `sim-ldpc-0.3.4/tests/test_ieee802_11.py` & `sim-ldpc-0.3.5/tests/test_ieee802_11.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,66 +9,66 @@
 
 
 class TestEncoder802_11:
     def test_incorrect_length(self) -> None:
         enc = EncoderWiFi(WiFiSpecCode.N648_R12)
         bits: npt.NDArray[np.int_] = np.array([1, 1, 0])
         with pytest.raises(IncorrectLength):
-            enc.encode(Bits(bits))
+            enc.encode(bits)
 
     def test_encoding_648_r12(self) -> None:
         # comparing encodings with reference implementation by: https://github.com/tavildar/LDPC
-        info_bits = Bits(auto=np.genfromtxt(
-            'tests/test_data/ieee_802_11/info_bits_N648_R12.csv', delimiter=',', dtype=np.int_))  # type: ignore
+        info_bits = np.genfromtxt(
+            'tests/test_data/ieee_802_11/info_bits_N648_R12.csv', delimiter=',', dtype=np.int_)  # type: ignore
         encoded_ref = Bits(auto=np.genfromtxt(
             'tests/test_data/ieee_802_11/encoded_N648_R12.csv', delimiter=',', dtype=np.int_))  # type: ignore
         enc = EncoderWiFi(WiFiSpecCode.N648_R12)
 
         encoded = Bits()
         for frame_idx in range(len(info_bits)//enc.k):
-            encoded += enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k])
+            encoded += Bits(auto=enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k]))
         assert sum(encoded_ref ^ encoded) == 0  # assert Hamming distance of my implementation with reference
 
     def test_encoding_648_r56(self) -> None:
         # comparing encodings with reference implementation by: https://github.com/tavildar/LDPC
-        info_bits = Bits(auto=np.genfromtxt(
-            'tests/test_data/ieee_802_11/info_bits_N648_R56.csv', delimiter=',', dtype=np.int_))  # type: ignore
+        info_bits = np.genfromtxt(
+            'tests/test_data/ieee_802_11/info_bits_N648_R56.csv', delimiter=',', dtype=np.int_)  # type: ignore
         encoded_ref = Bits(auto=np.genfromtxt(
             'tests/test_data/ieee_802_11/encoded_N648_R56.csv', delimiter=',', dtype=np.int_))  # type: ignore
         enc = EncoderWiFi(WiFiSpecCode.N648_R56)
 
         encoded = Bits()
         for frame_idx in range(len(info_bits)//enc.k):
-            encoded += enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k])
+            encoded += Bits(auto=enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k]))
         assert sum(encoded_ref ^ encoded) == 0  # assert Hamming distance of my implementation with reference
 
     def test_encoding_1296_r23(self) -> None:
         # comparing encodings with reference implementation by: https://github.com/tavildar/LDPC
-        info_bits = Bits(auto=np.genfromtxt(
-            'tests/test_data/ieee_802_11/info_bits_N1296_R23.csv', delimiter=',', dtype=np.int_))  # type: ignore
+        info_bits = np.genfromtxt(
+            'tests/test_data/ieee_802_11/info_bits_N1296_R23.csv', delimiter=',', dtype=np.int_)  # type: ignore
         encoded_ref = Bits(auto=np.genfromtxt(
             'tests/test_data/ieee_802_11/encoded_N1296_R23.csv', delimiter=',', dtype=np.int_))  # type: ignore
         enc = EncoderWiFi(WiFiSpecCode.N1296_R23)
 
         encoded = Bits()
         for frame_idx in range(len(info_bits)//enc.k):
-            encoded += enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k])
+            encoded += Bits(auto=enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k]))
         assert sum(encoded_ref ^ encoded) == 0  # assert Hamming distance of my implementation with reference
 
     def test_encoding_1944_r34(self) -> None:
         # comparing encodings with reference implementation by: https://github.com/tavildar/LDPC
-        info_bits = Bits(auto=np.genfromtxt(
-            'tests/test_data/ieee_802_11/info_bits_N1944_R34.csv', delimiter=',', dtype=np.int_))  # type: ignore
+        info_bits = np.genfromtxt(
+            'tests/test_data/ieee_802_11/info_bits_N1944_R34.csv', delimiter=',', dtype=np.int_)  # type: ignore
         encoded_ref = Bits(auto=np.genfromtxt(
             'tests/test_data/ieee_802_11/encoded_N1944_R34.csv', delimiter=',', dtype=np.int_))  # type: ignore
         enc = EncoderWiFi(WiFiSpecCode.N1944_R34)
 
         encoded = Bits()
         for frame_idx in range(len(info_bits)//enc.k):
-            encoded += enc.encode(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k])
+            encoded += Bits(auto=enc.encode(np.array(info_bits[frame_idx*enc.k: (frame_idx+1)*enc.k], dtype=np.int_)))
         assert sum(encoded_ref ^ encoded) == 0  # assert Hamming distance of my implementation with reference
 
 
 class TestDecoder802_11:
     def test_incorrect_length(self) -> None:
         p = 0.1
         h = QCFile.from_file("ldpc/code_specs/ieee802.11/N648_R12.qc").to_array()
@@ -112,15 +112,15 @@
         corrupted = BitArray(encoded_ref)
         no_errors = int(len(corrupted) * p)
         rng = np.random.default_rng()
         error_idx = rng.choice(len(corrupted), size=no_errors, replace=False)
         for idx in error_idx:
             corrupted[idx] = not corrupted[idx]
 
-        decoder = DecoderWiFi(spec=WiFiSpecCode.N1296_R23, max_iter=20, channel_model=bsc_llr(p=p),decoder_type="MS")
+        decoder = DecoderWiFi(spec=WiFiSpecCode.N1296_R23, max_iter=20, channel_model=bsc_llr(p=p), decoder_type="MS")
         decoded = Bits()
         decoded_info = Bits()
         for frame_idx in range(len(corrupted) // decoder.n):
             decoder_output = decoder.decode(corrupted[frame_idx * decoder.n: (frame_idx + 1) * decoder.n])
             decoded += decoder_output[0]
             decoded_info += decoder.info_bits(decoder_output[0])
             assert decoder_output[2] is True
```

### Comparing `sim-ldpc-0.3.4/tests/test_qcfile.py` & `sim-ldpc-0.3.5/tests/test_qcfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,11 +61,11 @@
         """
         z = 10
         arr: Any = np.block([[np.eye(z), np.eye(z, k=1) + np.eye(z, k=-z+1)],
                              [np.eye(z, k=2) + np.eye(z, k=-z+2), np.zeros((z, z))]])
         a = QCFile.from_array(arr, z)
         arr = sp.lil_matrix(arr)
         b = a.to_sparse()
-        assert sp.spmatrix.sum(arr != b) == 0
+        assert sp.lil_matrix.sum(arr != b) == 0
         a.block_structure[0][0] = a.z
         with pytest.raises(InconsistentQCFile):
             a.to_sparse()
```

