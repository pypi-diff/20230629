# Comparing `tmp/naluconfigs-11.1.1.tar.gz` & `tmp/naluconfigs-11.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-11.1.1.tar", last modified: Mon Jun 12 23:28:59 2023, max compression
+gzip compressed data, was "naluconfigs-11.2.1.tar", last modified: Thu Jun 29 20:55:41 2023, max compression
```

## Comparing `naluconfigs-11.1.1.tar` & `naluconfigs-11.2.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.554154 naluconfigs-11.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.558154 naluconfigs-11.1.1/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.554154 naluconfigs-11.1.1/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.558154 naluconfigs-11.1.1/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.562154 naluconfigs-11.1.1/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.558154 naluconfigs-11.1.1/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 23:28:59.000000 naluconfigs-11.1.1/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:28:59.566154 naluconfigs-11.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-12 23:28:38.000000 naluconfigs-11.1.1/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.411994 naluconfigs-11.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.415994 naluconfigs-11.2.1/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.411994 naluconfigs-11.2.1/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.415994 naluconfigs-11.2.1/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.423994 naluconfigs-11.2.1/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13720 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.415994 naluconfigs-11.2.1/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 20:55:41.000000 naluconfigs-11.2.1/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:55:41.427994 naluconfigs-11.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-29 20:55:25.000000 naluconfigs-11.2.1/tests/test_range_keys.py
```

### Comparing `naluconfigs-11.1.1/PKG-INFO` & `naluconfigs-11.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.1.1
+Version: 11.2.1
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.1.1/README.md` & `naluconfigs-11.2.1/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/pyproject.toml` & `naluconfigs-11.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/setup.py` & `naluconfigs-11.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/__init__.py` & `naluconfigs-11.2.1/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/_constructors.py` & `naluconfigs-11.2.1/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/aardvarcv4.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       value: 2048
     mont_on:
       address: 0x17
       bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
+      value: false
     mont_select:
       address: 0x17
       bitposition: 0
       bitwidth: 3
       description: ''
       readwrite: w
       value: 0
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       value: 2048
     mont_on:
       address: 0x17
       bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: w
-      value: 0
+      value: false
     mont_select:
       address: 0x17
       bitposition: 0
       bitwidth: 3
       description: ''
       readwrite: w
       value: 0
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/asocv3.yml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       value: 2048
     mont_on:
       address: 0x17
       bitposition: 3
       bitwidth: 1
       description: ''
       readwrite: rw
-      value: true
+      value: false
     mont_select:
       address: 0x17
       bitposition: 0
       bitwidth: 3
       description: ''
       readwrite: rw
       value: 0
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-11.2.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     - d2xx
   si5341_address: 0xE8
   default_baud:
     115200: 53
   default_baudrate: 115200
   default_clock: 100000000.0
   default_divider: 53
-  expected_scalmon: 2500
   ext_dac:
     chip: ad5675
     max_mv: 1200
     max_counts: 65535
     channels:
       0..3: 30000
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: dac7578
     max_mv: 1200
     max_counts: 4095
     channels:
       0..3: 2048
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv3_gbe.yml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: dac7578
     max_mv: 1200
     max_counts: 4095
     channels:
       0..3: 2048
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: dac7578
     max_mv: 1200
     max_counts: 4095
     channels:
       0..7: 2048
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: dac7578
     max_mv: 2500
     max_counts: 4095
     channels:
       0..7: 2048
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: dac7578
     max_mv: 2500
     max_counts: 4095
     channels:
       0..7: 2048
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: ad5671
     max_mv: 2500
     max_counts: 4095
     channels:
       0: 2048
       1: 2175
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files 1% similar despite different names*

```diff
@@ -19,27 +19,26 @@
   clock_file: AODS_300GCC.txt  #  AODS_debugpulse_240MGCC_10Mref.txt
   connections:
     - serial
     - d2xx
     - udp
   si5341_address: 0xE8
   default_baud:
-    111111: 53
-  default_baudrate: 111111
-  default_clock: 200000000.0
-  default_divider: 53
+    115200: 868
+  default_baudrate: 115200
+  default_clock: 96000000.0
+  default_divider: 868
   default_trigger_value: 2000
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: ad5671
     max_mv: 2500
     max_counts: 4096
     channels:
       0: 2048
       1: 2175
@@ -82,16 +81,16 @@
         digital_registers:
           begin: 300
           length: 330
         control_registers:
           begin: 630
           length: 70
   possible_bauds:
-    111111: 53
-    1500000: 3
+    115200: 868
+    2000000: 50
   resolution: 12
   samples: 64
   samplingrate: 1.0
   stop_word: !!binary |
     +s4=
   wait: AE000001
   wbias: 848
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/asoc.yml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     - d2xx
   si5341_address: 0xE8
   default_baud:
     115200: 53
   default_baudrate: 115200
   default_clock: 100000000.0
   default_divider: 53
-  expected_scalmon: 2500
   ext_dac:
     max_mv: 2500
     max_counts: 4095
     channels:
       0: 2000
       1: 2000
       2: 2000
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv2.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     - d2xx
   si5341_address: 0xE8
   default_baud:
     111111: 53
   default_baudrate: 111111
   default_clock: 96000000.0
   default_divider: 53
-  expected_scalmon: 2500
   ext_dac:
     chip: ad5675
     max_mv: 2500
     max_counts: 65535
     channels:
       0..3: 30000
     address_mapping:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/asocv3.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,18 @@
   clock_file: Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
   connections:
     - serial
     - d2xx
     - udp
   si5341_address: 0xE8
   default_baud:
-    115200: 826
-  default_baudrate: 111111
+    115200: 868
+  default_baudrate: 115200
   default_clock: 96000000.0
-  default_divider: 53
-  expected_scalmon: 2500
+  default_divider: 868
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   si5341_address: 0xEE
   default_baud:
     3000000: 33
   default_baudrate: 3000000
   default_clock: 100000000.0
   default_divider: 33
   default_trigger_value: 1500
-  expected_scalmon: 2500
   ext_dac:
     max_mv: 1200
     max_counts: 4095
     channels:
       0..13: 0
   headers: 3
   numregs: 64
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   si5341_address: 0xE8
   default_baud:
     3000000: 33
   default_baudrate: 3000000
   default_clock: 100000000.0
   default_divider: 33
   default_trigger_value: 1500
-  expected_scalmon: 2500
   ext_dac:
     max_mv: 1200
     max_counts: 4095
     channels:
       0: 2048
       1: 2048
       2: 2048
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     max_mv: 2500
     max_counts: 65535
     channels:
       0: 32768
       1: 34800
       2: 31500
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/siread.yml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     - serial
     - d2xx
   default_baud:
     230400: 53
   default_baudrate: 230400
   default_clock: 200000000.0
   default_divider: 53
-  expected_scalmon: 2500
   headers: 3
   last_window_fix_amount: 47
   numregs: 32
   pedestals_blocks: 8
   possible_bauds:
     230400: 53
     625000: 19
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/trbhm.yml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
   threshold_scan:
     min_vref: 0
     max_vref: 2500
     start: 500
     stop: 3500
     stepsize: 5
     units: counts
-  expected_scalmon: 2500
   ext_dac:
     chip: ltc2620
     max_mv: 1200
     max_counts: 4095
     channels:
       0..7: 2048
     chip_mapping: # asic channel: dac chip number
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/udc16.yml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
       6, 14: 6
       7, 15: 7
   trigger:
     max_val: 2047
     min_val: 0
     default: false
   num_trigger_channels: 8
-  expected_scalmon: 2500
   headers: 0
   last_window_fix_amount: 47
   lastbits: 0
   numregs: 32
   pedestals_blocks: 8
   peripherals:
     current:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/upac32.yml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
       24: dac_vbias24_31_out
   trigger:
     triggers_available: 8
     max_val: 2047
     min_val: 0
     default: false
   num_trigger_channels: 8
-  expected_scalmon: 2500
   headers: 0
   last_window_fix_amount: 47
   lastbits: 0
   numregs: 32
   pedestals_blocks: 8
   peripherals:
     current:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/upac96.yml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
       64: 4
       80: 6
   trigger:
     max_val: 4095
     min_val: 0
     default: false
   num_trigger_channels: 8
-  expected_scalmon: 2500
   headers: 0
   last_window_fix_amount: 47
   lastbits: 0
   numregs: 32
   pedestals_blocks: 64
   peripherals:
     readout_pcb_temp:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/upaci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
       24: 30000
   trigger:
     triggers_available: 8
     max_val: 2047
     min_val: 0
     default: false
   num_trigger_channels: 8
-  expected_scalmon: 2500
   headers: 0
   last_window_fix_amount: 47
   lastbits: 0
   numregs: 32
   pedestals_blocks: 8
   peripherals:
     current:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-11.2.1/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
       24: 30000
   trigger:
     triggers_available: 8
     max_val: 2047
     min_val: 0
     default: false
   num_trigger_channels: 8
-  expected_scalmon: 2500
   headers: 0
   last_window_fix_amount: 47
   lastbits: 0
   numregs: 32
   pedestals_blocks: 8
   peripherals:
     current:
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs/exceptions.py` & `naluconfigs-11.2.1/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/helpers.py` & `naluconfigs-11.2.1/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs/postprocess.py` & `naluconfigs-11.2.1/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-11.2.1/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.1.1
+Version: 11.2.1
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.1.1/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-11.2.1/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/tests/test_hex_addr_converter.py` & `naluconfigs-11.2.1/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/tests/test_i2c_registers.py` & `naluconfigs-11.2.1/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/tests/test_multichip.py` & `naluconfigs-11.2.1/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/tests/test_post_processing.py` & `naluconfigs-11.2.1/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.1.1/tests/test_range_keys.py` & `naluconfigs-11.2.1/tests/test_range_keys.py`

 * *Files identical despite different names*

