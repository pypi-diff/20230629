# Comparing `tmp/ppafm-0.2.0a3.tar.gz` & `tmp/ppafm-0.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppafm-0.2.0a3.tar", last modified: Tue Jun 13 17:03:49 2023, max compression
+gzip compressed data, was "ppafm-0.2.1a2.tar", last modified: Thu Jun 29 17:18:54 2023, max compression
```

## Comparing `ppafm-0.2.0a3.tar` & `ppafm-0.2.1a2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.810512 ppafm-0.2.0a3/ppafm/
--rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/GUIWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/GridUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16312 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/HighLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/PPPlot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/atomicUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/chemistry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.814513 ppafm-0.2.0a3/ppafm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/conv_rho.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateDFTD3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9054 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateElFF.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1536 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateElFF_point_charges.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1777 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateLJFF.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateTraining_PVE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.814513 ppafm-0.2.0a3/ppafm/cli/gui/
--rwxr-xr-x   0 runner    (1001) docker     (123)    25999 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter.py
--rw-r--r--   0 runner    (1001) docker     (123)    36464 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter_2tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/Viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45544 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/ppafm_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15238 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/plot_results.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9261 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/relaxed_scan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9983 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/relaxed_scan_PVE.py
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12070 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.818513 ppafm-0.2.0a3/ppafm/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/CG.h
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Forces.h
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Grid.h
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/GridUtils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Mat3.h
--rw-r--r--   0 runner    (1001) docker     (123)    31964 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/ProbeParticle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Vec2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Vec3.h
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/VecN.h
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fastmath.h
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fastmath_light.h
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fitSpline.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fitting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/gonioApprox.h
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/integerOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/macroUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/spline_hermite.h
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.822512 ppafm-0.2.0a3/ppafm/defaults/
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/atomtypes.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)    13678 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/d3.py
--rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/d3_R0.npy
--rw-r--r--   0 runner    (1001) docker     (123)   883728 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/d3_c6.npy
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/params.ini
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/valelec_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/fieldFFT.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/file_dat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10694 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/fitSpline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4986 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.822512 ppafm-0.2.0a3/ppafm/ml/
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/AuxMap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/CorrectionLoop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/Corrector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19109 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/Generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.822512 ppafm-0.2.0a3/ppafm/ocl/
--rw-r--r--   0 runner    (1001) docker     (123)    33867 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/AFMulator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/ppafm/ocl/cl/
--rw-r--r--   0 runner    (1001) docker     (123)    69639 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/FF.cl
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/relax.cl
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/splines.cl
--rw-r--r--   0 runner    (1001) docker     (123)    88476 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/oclUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/relax.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.810512 ppafm-0.2.0a3/ppafm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2318 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_afmulator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_atomicUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2437 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_datagrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_vdw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.247415 ppafm-0.2.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-29 17:18:54.247415 ppafm-0.2.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.235415 ppafm-0.2.1a2/ppafm/
+-rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/GUIWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/GridUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16312 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/HighLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/PPPlot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/atomicUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/chemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.239415 ppafm-0.2.1a2/ppafm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/conv_rho.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/generateDFTD3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9054 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/generateElFF.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1536 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/generateElFF_point_charges.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1777 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/generateLJFF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/generateTraining_PVE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.239415 ppafm-0.2.1a2/ppafm/cli/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25999 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/gui/ExpShifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36464 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/gui/ExpShifter_2tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/gui/Viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45544 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/gui/ppafm_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15238 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/plot_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9261 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/relaxed_scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9983 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cli/relaxed_scan_PVE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12070 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.243415 ppafm-0.2.1a2/ppafm/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/CG.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/Forces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/Grid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/GridUtils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/Mat3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31964 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/ProbeParticle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/Vec2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/Vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/VecN.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/fastmath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/fastmath_light.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/fitSpline.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/fitting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/gonioApprox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/integerOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/macroUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp/spline_hermite.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/cpp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.243415 ppafm-0.2.1a2/ppafm/defaults/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/atomtypes.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13678 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/d3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/d3_R0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)   883728 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/d3_c6.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/params.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/defaults/valelec_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/fieldFFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/file_dat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10694 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/fitSpline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4986 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.243415 ppafm-0.2.1a2/ppafm/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ml/AuxMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ml/CorrectionLoop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ml/Corrector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19109 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ml/Generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.247415 ppafm-0.2.1a2/ppafm/ocl/
+-rw-r--r--   0 runner    (1001) docker     (123)    33867 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/AFMulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.247415 ppafm-0.2.1a2/ppafm/ocl/cl/
+-rw-r--r--   0 runner    (1001) docker     (123)    69639 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/cl/FF.cl
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/cl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/cl/relax.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/cl/splines.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    88476 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/oclUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/ocl/relax.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/ppafm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.235415 ppafm-0.2.1a2/ppafm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-29 17:18:54.000000 ppafm-0.2.1a2/ppafm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-29 17:18:54.000000 ppafm-0.2.1a2/ppafm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:18:54.000000 ppafm-0.2.1a2/ppafm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-29 17:18:54.000000 ppafm-0.2.1a2/ppafm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:18:53.000000 ppafm-0.2.1a2/ppafm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 17:18:54.000000 ppafm-0.2.1a2/ppafm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 17:18:54.000000 ppafm-0.2.1a2/ppafm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:18:54.247415 ppafm-0.2.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:18:54.247415 ppafm-0.2.1a2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2318 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/tests/test_afmulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/tests/test_atomicUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/tests/test_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2437 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/tests/test_datagrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/tests/test_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-06-29 17:18:44.000000 ppafm-0.2.1a2/tests/test_vdw.py
```

### Comparing `ppafm-0.2.0a3/PKG-INFO` & `ppafm-0.2.1a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ppafm
-Version: 0.2.0a3
+Version: 0.2.1a2
 Summary: Classical force field model for simulating atomic force microscopy images.
 Project-URL: Homepage, https://github.com/Probe-Particle/ProbeParticleModel
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: opencl
 Provides-Extra: dev
 
 
 # Probe Particle Model (PPM)
 
@@ -25,93 +25,62 @@
 ```bash
 $ pip install ppafm
 ```
 
 This should install the package and all its dependencies.
 Once the installation is completed, the following commands should be available:
 
-- `ppafm-generate-elff` - command-line interface to gelerate electrostatic force field.
-- `ppafm-generate-elff-point-charges` - command-line interface to gelerate electrostatic force field using point charges.
-- `ppafm-generate-ljff` - command-line interface to gelerate Lennard-Jones force field.
-- `ppafm-relaxed-scan` - command-line interface to run scan the sample with the probe particle.
+- `ppafm-generate-elff` - command-line interface to generate electrostatic force field.
+- `ppafm-generate-elff-point-charges` - command-line interface to generate electrostatic force field using point charges.
+- `ppafm-generate-ljff` - command-line interface to generate Lennard-Jones force field.
+- `ppafm-relaxed-scan` - command-line interface to run a scan of the sample with the probe particle.
 - `ppafm-plot-results` - command-line interface to plot the results of the simulation.
-- `ppafm-gui` - GUI application for interactive simulation of AFM images.
+- `ppafm-gui` - GUI application for interactive simulation of AFM images. Requires some additional dependencies, see below.
 
+Alternatives (Docker, Anaconda) and some notes on different platforms (Linux, MacOS, Windows) can be found on the wiki: [Additional installation instructions](https://github.com/Probe-Particle/ppafm/wiki/Additional-installation-instructions)
 
 ### Install GPU GUI
-
-To make sure the `ppafm-gui` command works without problems, you need to install QT5 library on your system.
-On Ubuntu, you can do this by running:
+The `ppafm-gui` application requires some additional dependencies. These dependencies should be installed automatically when you install the `ppafm` package with the `opencl` option:
 
 ```bash
-$ sudo apt install python3-pyqt5
+$ pip install ppafm[opencl]
 ```
 
-The other dependencies should be installed automatically when you install the `ppafm` package with `opencl` option:
+On Linux systems (tested on Ubuntu) you need to additionally install PyQt5 on your system
 
 ```bash
-$ pip install ppafm[opencl]
+$ sudo apt install python3-pyqt5
 ```
 
-Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
+Additionally, an OpenCL Installable Client Driver (ICD) for your compute device is required. On Ubuntu:
 * Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
-* AMD GPU: `sudo apt install mesa-opencl-icd`
+* AMD GPU: `sudo apt install mesa-opencl-icd` (May not work on all AMD devices, see the [Pro drivers](https://www.amd.com/en/support/kb/faq/amdgpu-installation))
 * Intel HD Graphics: `sudo apt install intel-opencl-icd`
 * CPU: `sudo apt install pocl-opencl-icd`
 
-### Use ppafm Docker container
-
-We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
-
-Here are the steps to build and run the ppafm Docker container:
-
-1. Build the image.
-
-```bash
-$ docker build -t ppafm:latest .
-```
-2. Execute the container.
-
-```bash
-$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
-```
-
+See additional instructions on the wiki: [PPAFM GUI](https://github.com/Probe-Particle/ppafm/wiki/PPAFM-GUI)
 
 ## Usage examples
 
 We provide a set of examples in the `examples` directory.
 To run them, navigate to the directory and run the `run.sh` script.
 For example:
 
 ```bash
 $ cd examples/PTCDA_single
 $ ./run.sh
 ```
 
 You can study the script to see how to run the simulation.
-Also, have a look at the `params.ini` file to see how to set up the simulation parameters.
-
+Also, have a look at the `params.ini` file and [the wiki](https://github.com/Probe-Particle/ppafm/wiki/Params) to see how to set up the simulation parameters.
 
 Once the simulation is finished, a number of files and folders will be created.
 
-### GUI usage
-
-* Open a file by clicking `Open File...` at the bottom or provide an input file as a command line argument. The input file can be a .xyz geometry file (possibly with point charges*), a VASP POSCAR or CONTCAR file, an FHI-aims .in file, or a .xsf or .cube Hartree potential file. Loading large files may take some time.
-* Changing any number in any input box will automatically update the image. There are also presets for some commonly used tip configurations.
-Hover the mouse cursor over any parameter for a tooltip explaining the meaning of the parameter.
-* Click anywhere on the image to bring up a plot of the df approach curve for that point in the image.
-* Scroll anywhere on the image to zoom the scan window in/out of that spot.
-* Click on the `View Geometry` button to show the system geometry in ASE GUI.
-* Click on the `Edit Geometry` button to edit the positions, types, and charges of the atoms in the system. Note that for Hartree potential inputs editing charges is disabled and editing the geometry only affects the Lennard-Jones force field.
-* Click on the `View Forcefield` button to view different components of the force field. Note that the forcefield box size is inferred automatically from the scan size and is bigger than the scan size. Take into account the probe particle equilibrium distance when comparing the reported z-coordinates between the forcefield and the df image.
-* Click on the `Edit Forcefield` button to edit the per-species parameters of the Lennard-Jones forcefield.
-* Save the current image or df data by clicking the `Save Image...` or `Save df...` buttons at the bottom.
-* In case there are multiple OpenCL devices installed on the system, use the `-l` or `--list-devices` option to list available devices and choose the device using the `-d` or `--device` option with the device platform number as the argument.
-
-*Note that while input files without charges work, depending on the system, the resulting image may be significantly different from an image with electrostatics, and therefore may not be representative of reality. If no electrostatics are included, this is indicated in the title of the image.
+### GUI
+See the wiki: [PPAFM GUI](https://github.com/Probe-Particle/ppafm/wiki/PPAFM-GUI)
 
 ### Run GPU generator for machine learning
 
 * `examples/CorrectionLoopGraphene` use GPU accelerated PPM to iteratively improve the estimate of molecular geometry by comparing simulated AFM images with reference. This is work-in-progress. Currently, modification of estimate geometry is random (Monte-Carlo), while later we plan to develop a more clever (e.g. Machine-Learned) heuristic for more efficient improvment.
 * `examples/Generator` quickly generates a batch of simulated AFM images (resp. 3D data stacks) which can be further used for machine learning. Especially in connection with (https://github.com/SINGROUP/ASD-AFM).
 
 ## Flavors of PPM
@@ -131,22 +100,19 @@
 * **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
 * **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
 * **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
 
 
 ## For developers
 
-If you would like to contribute to the development of ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
+If you would like to contribute to the development of the ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
 
-
-### Further information
-- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
+## Further information
 - Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
-- API documentation: https://ppafm.readthedocs.io/en/latest/
-
+- Python API documentation: https://ppafm.readthedocs.io/en/latest/
 
 ### Notable publications using Probe Particle Model
 
 * [Prokop Hapala, Georgy Kichin, Christian Wagner, F. Stefan Tautz, Ruslan Temirov, and Pavel Jelínek, Mechanism of high-resolution STM/AFM imaging with functionalized tips, Phys. Rev. B 90, 085421 – Published 19 August 2014](http://journals.aps.org/prb/abstract/10.1103/PhysRevB.90.085421)
 * [Prokop Hapala, Ruslan Temirov, F. Stefan Tautz, and Pavel Jelínek, Origin of High-Resolution IETS-STM Images of Organic Molecules with Functionalized Tips, Phys. Rev. Lett. 113, 226101 – Published 25 November 2014,](http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.226101)
 
 ### License
```

### Comparing `ppafm-0.2.0a3/README.md` & `ppafm-0.2.1a2/ppafm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ppafm
+Version: 0.2.1a2
+Summary: Classical force field model for simulating atomic force microscopy images.
+Project-URL: Homepage, https://github.com/Probe-Particle/ProbeParticleModel
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: opencl
+Provides-Extra: dev
+
 
 # Probe Particle Model (PPM)
 
 Simple and efficient **simulation software for high-resolution atomic force microscopy** (**HR-AFM**) and other scanning probe microscopy (SPM) techniques with sub-molecular resolution (STM, IETS, TERS). It simulates deflection of the particle attached to the tip (typically CO molecule, but also e.g. Xe, Cl-, H2O and others).
 
 ## Installation
 
@@ -10,93 +25,62 @@
 ```bash
 $ pip install ppafm
 ```
 
 This should install the package and all its dependencies.
 Once the installation is completed, the following commands should be available:
 
-- `ppafm-generate-elff` - command-line interface to gelerate electrostatic force field.
-- `ppafm-generate-elff-point-charges` - command-line interface to gelerate electrostatic force field using point charges.
-- `ppafm-generate-ljff` - command-line interface to gelerate Lennard-Jones force field.
-- `ppafm-relaxed-scan` - command-line interface to run scan the sample with the probe particle.
+- `ppafm-generate-elff` - command-line interface to generate electrostatic force field.
+- `ppafm-generate-elff-point-charges` - command-line interface to generate electrostatic force field using point charges.
+- `ppafm-generate-ljff` - command-line interface to generate Lennard-Jones force field.
+- `ppafm-relaxed-scan` - command-line interface to run a scan of the sample with the probe particle.
 - `ppafm-plot-results` - command-line interface to plot the results of the simulation.
-- `ppafm-gui` - GUI application for interactive simulation of AFM images.
+- `ppafm-gui` - GUI application for interactive simulation of AFM images. Requires some additional dependencies, see below.
 
+Alternatives (Docker, Anaconda) and some notes on different platforms (Linux, MacOS, Windows) can be found on the wiki: [Additional installation instructions](https://github.com/Probe-Particle/ppafm/wiki/Additional-installation-instructions)
 
 ### Install GPU GUI
-
-To make sure the `ppafm-gui` command works without problems, you need to install QT5 library on your system.
-On Ubuntu, you can do this by running:
+The `ppafm-gui` application requires some additional dependencies. These dependencies should be installed automatically when you install the `ppafm` package with the `opencl` option:
 
 ```bash
-$ sudo apt install python3-pyqt5
+$ pip install ppafm[opencl]
 ```
 
-The other dependencies should be installed automatically when you install the `ppafm` package with `opencl` option:
+On Linux systems (tested on Ubuntu) you need to additionally install PyQt5 on your system
 
 ```bash
-$ pip install ppafm[opencl]
+$ sudo apt install python3-pyqt5
 ```
 
-Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
+Additionally, an OpenCL Installable Client Driver (ICD) for your compute device is required. On Ubuntu:
 * Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
-* AMD GPU: `sudo apt install mesa-opencl-icd`
+* AMD GPU: `sudo apt install mesa-opencl-icd` (May not work on all AMD devices, see the [Pro drivers](https://www.amd.com/en/support/kb/faq/amdgpu-installation))
 * Intel HD Graphics: `sudo apt install intel-opencl-icd`
 * CPU: `sudo apt install pocl-opencl-icd`
 
-### Use ppafm Docker container
-
-We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
-
-Here are the steps to build and run the ppafm Docker container:
-
-1. Build the image.
-
-```bash
-$ docker build -t ppafm:latest .
-```
-2. Execute the container.
-
-```bash
-$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
-```
-
+See additional instructions on the wiki: [PPAFM GUI](https://github.com/Probe-Particle/ppafm/wiki/PPAFM-GUI)
 
 ## Usage examples
 
 We provide a set of examples in the `examples` directory.
 To run them, navigate to the directory and run the `run.sh` script.
 For example:
 
 ```bash
 $ cd examples/PTCDA_single
 $ ./run.sh
 ```
 
 You can study the script to see how to run the simulation.
-Also, have a look at the `params.ini` file to see how to set up the simulation parameters.
-
+Also, have a look at the `params.ini` file and [the wiki](https://github.com/Probe-Particle/ppafm/wiki/Params) to see how to set up the simulation parameters.
 
 Once the simulation is finished, a number of files and folders will be created.
 
-### GUI usage
-
-* Open a file by clicking `Open File...` at the bottom or provide an input file as a command line argument. The input file can be a .xyz geometry file (possibly with point charges*), a VASP POSCAR or CONTCAR file, an FHI-aims .in file, or a .xsf or .cube Hartree potential file. Loading large files may take some time.
-* Changing any number in any input box will automatically update the image. There are also presets for some commonly used tip configurations.
-Hover the mouse cursor over any parameter for a tooltip explaining the meaning of the parameter.
-* Click anywhere on the image to bring up a plot of the df approach curve for that point in the image.
-* Scroll anywhere on the image to zoom the scan window in/out of that spot.
-* Click on the `View Geometry` button to show the system geometry in ASE GUI.
-* Click on the `Edit Geometry` button to edit the positions, types, and charges of the atoms in the system. Note that for Hartree potential inputs editing charges is disabled and editing the geometry only affects the Lennard-Jones force field.
-* Click on the `View Forcefield` button to view different components of the force field. Note that the forcefield box size is inferred automatically from the scan size and is bigger than the scan size. Take into account the probe particle equilibrium distance when comparing the reported z-coordinates between the forcefield and the df image.
-* Click on the `Edit Forcefield` button to edit the per-species parameters of the Lennard-Jones forcefield.
-* Save the current image or df data by clicking the `Save Image...` or `Save df...` buttons at the bottom.
-* In case there are multiple OpenCL devices installed on the system, use the `-l` or `--list-devices` option to list available devices and choose the device using the `-d` or `--device` option with the device platform number as the argument.
-
-*Note that while input files without charges work, depending on the system, the resulting image may be significantly different from an image with electrostatics, and therefore may not be representative of reality. If no electrostatics are included, this is indicated in the title of the image.
+### GUI
+See the wiki: [PPAFM GUI](https://github.com/Probe-Particle/ppafm/wiki/PPAFM-GUI)
 
 ### Run GPU generator for machine learning
 
 * `examples/CorrectionLoopGraphene` use GPU accelerated PPM to iteratively improve the estimate of molecular geometry by comparing simulated AFM images with reference. This is work-in-progress. Currently, modification of estimate geometry is random (Monte-Carlo), while later we plan to develop a more clever (e.g. Machine-Learned) heuristic for more efficient improvment.
 * `examples/Generator` quickly generates a batch of simulated AFM images (resp. 3D data stacks) which can be further used for machine learning. Especially in connection with (https://github.com/SINGROUP/ASD-AFM).
 
 ## Flavors of PPM
@@ -116,22 +100,19 @@
 * **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
 * **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
 * **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
 
 
 ## For developers
 
-If you would like to contribute to the development of ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
+If you would like to contribute to the development of the ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
 
-
-### Further information
-- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
+## Further information
 - Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
-- API documentation: https://ppafm.readthedocs.io/en/latest/
-
+- Python API documentation: https://ppafm.readthedocs.io/en/latest/
 
 ### Notable publications using Probe Particle Model
 
 * [Prokop Hapala, Georgy Kichin, Christian Wagner, F. Stefan Tautz, Ruslan Temirov, and Pavel Jelínek, Mechanism of high-resolution STM/AFM imaging with functionalized tips, Phys. Rev. B 90, 085421 – Published 19 August 2014](http://journals.aps.org/prb/abstract/10.1103/PhysRevB.90.085421)
 * [Prokop Hapala, Ruslan Temirov, F. Stefan Tautz, and Pavel Jelínek, Origin of High-Resolution IETS-STM Images of Organic Molecules with Functionalized Tips, Phys. Rev. Lett. 113, 226101 – Published 25 November 2014,](http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.226101)
 
 ### License
```

### Comparing `ppafm-0.2.0a3/ppafm/GUIWidgets.py` & `ppafm-0.2.1a2/ppafm/GUIWidgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         F = F_stack
         print("plotSlice F.shape, F.min(), F.max() ", F.shape, F.min(), F.max())
 
 
         print('self.margins', margins)
         if alpha>0 and big_len_image is not None:
             F = F*(1-alpha) + big_len_image*alpha
-        self.img = self.axes.imshow( F, origin='image', cmap='viridis', interpolation='bicubic' )
+        self.img = self.axes.imshow( F, origin='lower', cmap='viridis', interpolation='bicubic' )
 
         j_min,i_min = np.unravel_index(F.argmin(), F.shape)
         j_max,i_max = np.unravel_index(F.argmax(), F.shape)
 
         if margins:
             self.axes.add_patch(matplotlib.patches.Rectangle((margins[0], margins[1]),margins[2], margins[3], linewidth=2,edgecolor='r',facecolor='none'))
             textRes = 'output size: '+str(margins[2])+ 'x'+ str(margins[3])
```

### Comparing `ppafm-0.2.0a3/ppafm/GridUtils.py` & `ppafm-0.2.1a2/ppafm/GridUtils.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/HighLevel.py` & `ppafm-0.2.1a2/ppafm/HighLevel.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/PPPlot.py` & `ppafm-0.2.1a2/ppafm/PPPlot.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     interpolation=default_interpolation,
     atoms=None, bonds=None, atomSize=default_atom_size
     ):
     for ii,i in enumerate(slices):
         print(" plotting ", i)
         plt.figure( figsize=( 10,10 ) )
         HSBs,vmax = colorize_XY2RG(dXs[i],dYs[i])
-        plt.imshow( HSBs, extent=extent, origin='image', interpolation=interpolation )
+        plt.imshow( HSBs, extent=extent, origin='lower', interpolation=interpolation )
         plotGeom( atoms, bonds, atomSize=atomSize )
         plt.xlabel(r' Tip_x $\AA$')
         plt.ylabel(r' Tip_y $\AA$')
         if zs is None:
             plt.title( r"iz = %i" %i  )
         else:
             plt.title( r"Tip_z = %2.2f $\AA$" %zs[i]  )
@@ -107,15 +107,15 @@
     atoms=None, bonds=None, atomSize=default_atom_size
     ):
     for ii,i in enumerate(slices):
         print(" plotting ", i)
         plt.figure( figsize=figsize )
         plt.plot  ( X[i,::by,::by].flat, Y[i,::by,::by].flat, 'r.', markersize=markersize )
         if BG is not None:
-            plt.imshow( BG[i,:,:], origin='image', interpolation=interpolation, cmap=cmap, extent=extent, vmin=vmin, vmax=vmax )
+            plt.imshow( BG[i,:,:], origin='lower', interpolation=interpolation, cmap=cmap, extent=extent, vmin=vmin, vmax=vmax )
             if cbar:
                 plt.colorbar()
         plotGeom( atoms, bonds, atomSize=atomSize )
         plt.xlabel(r' Tip_x $\AA$')
         plt.ylabel(r' Tip_y $\AA$')
         if zs is None:
             plt.title( r"iz = %i" %i  )
@@ -132,15 +132,15 @@
     atoms=None, bonds=None, atomSize=default_atom_size
     ):
     for ii,i in enumerate(slices):
         print(" plotting ", i)
         plt.figure( figsize=figsize )
         plt.quiver(  Xs[::by,::by], Ys[::by,::by],  dX[::by,::by], dY[::by,::by], color = 'k', headlength=10, headwidth=10, scale=15 )
         if BG is not None:
-            plt.imshow    ( BG[i,:,:], origin='image',  interpolation=interpolation, cmap=cmap, extent=extent, vmin=vmin, vmax=vmax  )
+            plt.imshow    ( BG[i,:,:], origin='lower',  interpolation=interpolation, cmap=cmap, extent=extent, vmin=vmin, vmax=vmax  )
             if cbar:
                 plt.colorbar()
         plotGeom( atoms, bonds, atomSize=atomSize )
         plt.xlabel(r' Tip_x $\AA$')
         plt.ylabel(r' Tip_y $\AA$')
         if zs is None:
             plt.title( r"iz = %i" %i  )
```

### Comparing `ppafm-0.2.0a3/ppafm/atomicUtils.py` & `ppafm-0.2.1a2/ppafm/atomicUtils.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/chemistry.py` & `ppafm-0.2.1a2/ppafm/chemistry.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/conv_rho.py` & `ppafm-0.2.1a2/ppafm/cli/conv_rho.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/generateDFTD3.py` & `ppafm-0.2.1a2/ppafm/cli/generateDFTD3.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/generateElFF.py` & `ppafm-0.2.1a2/ppafm/cli/generateElFF.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/generateElFF_point_charges.py` & `ppafm-0.2.1a2/ppafm/cli/generateElFF_point_charges.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/generateLJFF.py` & `ppafm-0.2.1a2/ppafm/cli/generateLJFF.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/generateTraining_PVE.py` & `ppafm-0.2.1a2/ppafm/cli/generateTraining_PVE.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter.py` & `ppafm-0.2.1a2/ppafm/cli/gui/ExpShifter.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,15 +464,15 @@
 
     def saveImg(self):
         n = len(self.data)
         plt.figure( figsize=(n*5,5) )
         for i in range(n):
             print (i)
             plt.subplot(1,n,i+1)
-            plt.imshow(self.data[i], origin='image') #,cmap='gray')
+            plt.imshow(self.data[i], origin='lower') #,cmap='gray')
             print ('image path = ' , self.path+'data.png')
         plt.savefig(self.path+"data.png", bbox_inches='tight')
 
     def shiftData(self):
         print ("shiftData")
         iz = int(self.bxZ.value())
         ix = int(self.bxX.value()); dix = ix - self.shifts[iz][0]; self.shifts[iz][0] = ix
```

### Comparing `ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter_2tips.py` & `ppafm-0.2.1a2/ppafm/cli/gui/ExpShifter_2tips.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,15 @@
 
     def saveImg(self):
         n = len(self.data)
         plt.figure( figsize=(n*5,5) )
         for i in range(n):
             print (i)
             plt.subplot(1,n,i+1)
-            plt.imshow(self.data[i], origin='image') #,cmap='gray')
+            plt.imshow(self.data[i], origin='lower') #,cmap='gray')
             print ('image path = ' , self.path+'data.png')
         plt.savefig(self.path+"data.png", bbox_inches='tight')
 
     def shiftData(self):
         print ("shiftData")
         iz = int(self.bxZ.value())
         ix = int(self.bxX.value()); dix = ix - self.shifts[self.tip][iz][0]; self.shifts[self.tip][iz][0] = ix
```

### Comparing `ppafm-0.2.0a3/ppafm/cli/gui/Viewer.py` & `ppafm-0.2.1a2/ppafm/cli/gui/Viewer.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/gui/ppafm_gui.py` & `ppafm-0.2.1a2/ppafm/cli/gui/ppafm_gui.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/plot_results.py` & `ppafm-0.2.1a2/ppafm/cli/plot_results.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/relaxed_scan.py` & `ppafm-0.2.1a2/ppafm/cli/relaxed_scan.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cli/relaxed_scan_PVE.py` & `ppafm-0.2.1a2/ppafm/cli/relaxed_scan_PVE.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/common.py` & `ppafm-0.2.1a2/ppafm/common.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/core.py` & `ppafm-0.2.1a2/ppafm/core.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/CG.h` & `ppafm-0.2.1a2/ppafm/cpp/CG.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/Forces.h` & `ppafm-0.2.1a2/ppafm/cpp/Forces.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/Grid.h` & `ppafm-0.2.1a2/ppafm/cpp/Grid.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/GridUtils.cpp` & `ppafm-0.2.1a2/ppafm/cpp/GridUtils.cpp`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/Mat3.h` & `ppafm-0.2.1a2/ppafm/cpp/Mat3.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/ProbeParticle.cpp` & `ppafm-0.2.1a2/ppafm/cpp/ProbeParticle.cpp`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/Vec2.h` & `ppafm-0.2.1a2/ppafm/cpp/Vec2.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/Vec3.h` & `ppafm-0.2.1a2/ppafm/cpp/Vec3.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/VecN.h` & `ppafm-0.2.1a2/ppafm/cpp/VecN.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/fastmath.h` & `ppafm-0.2.1a2/ppafm/cpp/fastmath.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/fastmath_light.h` & `ppafm-0.2.1a2/ppafm/cpp/fastmath_light.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/fitSpline.cpp` & `ppafm-0.2.1a2/ppafm/cpp/fitSpline.cpp`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/fitting.cpp` & `ppafm-0.2.1a2/ppafm/cpp/fitting.cpp`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/gonioApprox.h` & `ppafm-0.2.1a2/ppafm/cpp/gonioApprox.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/integerOps.h` & `ppafm-0.2.1a2/ppafm/cpp/integerOps.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/macroUtils.h` & `ppafm-0.2.1a2/ppafm/cpp/macroUtils.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/quaternion.h` & `ppafm-0.2.1a2/ppafm/cpp/quaternion.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp/spline_hermite.h` & `ppafm-0.2.1a2/ppafm/cpp/spline_hermite.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/cpp_utils.py` & `ppafm-0.2.1a2/ppafm/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/defaults/atomtypes.ini` & `ppafm-0.2.1a2/ppafm/defaults/atomtypes.ini`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/defaults/d3.py` & `ppafm-0.2.1a2/ppafm/defaults/d3.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/defaults/d3_R0.npy` & `ppafm-0.2.1a2/ppafm/defaults/d3_R0.npy`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/defaults/d3_c6.npy` & `ppafm-0.2.1a2/ppafm/defaults/d3_c6.npy`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/defaults/params.ini` & `ppafm-0.2.1a2/ppafm/defaults/params.ini`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/elements.py` & `ppafm-0.2.1a2/ppafm/elements.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/fieldFFT.py` & `ppafm-0.2.1a2/ppafm/fieldFFT.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/file_dat.py` & `ppafm-0.2.1a2/ppafm/file_dat.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/fitSpline.py` & `ppafm-0.2.1a2/ppafm/fitSpline.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/fitting.py` & `ppafm-0.2.1a2/ppafm/fitting.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/io.py` & `ppafm-0.2.1a2/ppafm/io.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ml/AuxMap.py` & `ppafm-0.2.1a2/ppafm/ml/AuxMap.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ml/CorrectionLoop.py` & `ppafm-0.2.1a2/ppafm/ml/CorrectionLoop.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ml/Corrector.py` & `ppafm-0.2.1a2/ppafm/ml/Corrector.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ml/Generator.py` & `ppafm-0.2.1a2/ppafm/ml/Generator.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/AFMulator.py` & `ppafm-0.2.1a2/ppafm/ocl/AFMulator.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/cl/FF.cl` & `ppafm-0.2.1a2/ppafm/ocl/cl/FF.cl`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/cl/relax.cl` & `ppafm-0.2.1a2/ppafm/ocl/cl/relax.cl`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/cl/splines.cl` & `ppafm-0.2.1a2/ppafm/ocl/cl/splines.cl`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/field.py` & `ppafm-0.2.1a2/ppafm/ocl/field.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/oclUtils.py` & `ppafm-0.2.1a2/ppafm/ocl/oclUtils.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm/ocl/relax.py` & `ppafm-0.2.1a2/ppafm/ocl/relax.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/ppafm.egg-info/PKG-INFO` & `ppafm-0.2.1a2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ppafm
-Version: 0.2.0a3
-Summary: Classical force field model for simulating atomic force microscopy images.
-Project-URL: Homepage, https://github.com/Probe-Particle/ProbeParticleModel
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: opencl
-Provides-Extra: dev
-
 
 # Probe Particle Model (PPM)
 
 Simple and efficient **simulation software for high-resolution atomic force microscopy** (**HR-AFM**) and other scanning probe microscopy (SPM) techniques with sub-molecular resolution (STM, IETS, TERS). It simulates deflection of the particle attached to the tip (typically CO molecule, but also e.g. Xe, Cl-, H2O and others).
 
 ## Installation
 
@@ -25,93 +10,62 @@
 ```bash
 $ pip install ppafm
 ```
 
 This should install the package and all its dependencies.
 Once the installation is completed, the following commands should be available:
 
-- `ppafm-generate-elff` - command-line interface to gelerate electrostatic force field.
-- `ppafm-generate-elff-point-charges` - command-line interface to gelerate electrostatic force field using point charges.
-- `ppafm-generate-ljff` - command-line interface to gelerate Lennard-Jones force field.
-- `ppafm-relaxed-scan` - command-line interface to run scan the sample with the probe particle.
+- `ppafm-generate-elff` - command-line interface to generate electrostatic force field.
+- `ppafm-generate-elff-point-charges` - command-line interface to generate electrostatic force field using point charges.
+- `ppafm-generate-ljff` - command-line interface to generate Lennard-Jones force field.
+- `ppafm-relaxed-scan` - command-line interface to run a scan of the sample with the probe particle.
 - `ppafm-plot-results` - command-line interface to plot the results of the simulation.
-- `ppafm-gui` - GUI application for interactive simulation of AFM images.
+- `ppafm-gui` - GUI application for interactive simulation of AFM images. Requires some additional dependencies, see below.
 
+Alternatives (Docker, Anaconda) and some notes on different platforms (Linux, MacOS, Windows) can be found on the wiki: [Additional installation instructions](https://github.com/Probe-Particle/ppafm/wiki/Additional-installation-instructions)
 
 ### Install GPU GUI
-
-To make sure the `ppafm-gui` command works without problems, you need to install QT5 library on your system.
-On Ubuntu, you can do this by running:
+The `ppafm-gui` application requires some additional dependencies. These dependencies should be installed automatically when you install the `ppafm` package with the `opencl` option:
 
 ```bash
-$ sudo apt install python3-pyqt5
+$ pip install ppafm[opencl]
 ```
 
-The other dependencies should be installed automatically when you install the `ppafm` package with `opencl` option:
+On Linux systems (tested on Ubuntu) you need to additionally install PyQt5 on your system
 
 ```bash
-$ pip install ppafm[opencl]
+$ sudo apt install python3-pyqt5
 ```
 
-Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
+Additionally, an OpenCL Installable Client Driver (ICD) for your compute device is required. On Ubuntu:
 * Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
-* AMD GPU: `sudo apt install mesa-opencl-icd`
+* AMD GPU: `sudo apt install mesa-opencl-icd` (May not work on all AMD devices, see the [Pro drivers](https://www.amd.com/en/support/kb/faq/amdgpu-installation))
 * Intel HD Graphics: `sudo apt install intel-opencl-icd`
 * CPU: `sudo apt install pocl-opencl-icd`
 
-### Use ppafm Docker container
-
-We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
-
-Here are the steps to build and run the ppafm Docker container:
-
-1. Build the image.
-
-```bash
-$ docker build -t ppafm:latest .
-```
-2. Execute the container.
-
-```bash
-$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
-```
-
+See additional instructions on the wiki: [PPAFM GUI](https://github.com/Probe-Particle/ppafm/wiki/PPAFM-GUI)
 
 ## Usage examples
 
 We provide a set of examples in the `examples` directory.
 To run them, navigate to the directory and run the `run.sh` script.
 For example:
 
 ```bash
 $ cd examples/PTCDA_single
 $ ./run.sh
 ```
 
 You can study the script to see how to run the simulation.
-Also, have a look at the `params.ini` file to see how to set up the simulation parameters.
-
+Also, have a look at the `params.ini` file and [the wiki](https://github.com/Probe-Particle/ppafm/wiki/Params) to see how to set up the simulation parameters.
 
 Once the simulation is finished, a number of files and folders will be created.
 
-### GUI usage
-
-* Open a file by clicking `Open File...` at the bottom or provide an input file as a command line argument. The input file can be a .xyz geometry file (possibly with point charges*), a VASP POSCAR or CONTCAR file, an FHI-aims .in file, or a .xsf or .cube Hartree potential file. Loading large files may take some time.
-* Changing any number in any input box will automatically update the image. There are also presets for some commonly used tip configurations.
-Hover the mouse cursor over any parameter for a tooltip explaining the meaning of the parameter.
-* Click anywhere on the image to bring up a plot of the df approach curve for that point in the image.
-* Scroll anywhere on the image to zoom the scan window in/out of that spot.
-* Click on the `View Geometry` button to show the system geometry in ASE GUI.
-* Click on the `Edit Geometry` button to edit the positions, types, and charges of the atoms in the system. Note that for Hartree potential inputs editing charges is disabled and editing the geometry only affects the Lennard-Jones force field.
-* Click on the `View Forcefield` button to view different components of the force field. Note that the forcefield box size is inferred automatically from the scan size and is bigger than the scan size. Take into account the probe particle equilibrium distance when comparing the reported z-coordinates between the forcefield and the df image.
-* Click on the `Edit Forcefield` button to edit the per-species parameters of the Lennard-Jones forcefield.
-* Save the current image or df data by clicking the `Save Image...` or `Save df...` buttons at the bottom.
-* In case there are multiple OpenCL devices installed on the system, use the `-l` or `--list-devices` option to list available devices and choose the device using the `-d` or `--device` option with the device platform number as the argument.
-
-*Note that while input files without charges work, depending on the system, the resulting image may be significantly different from an image with electrostatics, and therefore may not be representative of reality. If no electrostatics are included, this is indicated in the title of the image.
+### GUI
+See the wiki: [PPAFM GUI](https://github.com/Probe-Particle/ppafm/wiki/PPAFM-GUI)
 
 ### Run GPU generator for machine learning
 
 * `examples/CorrectionLoopGraphene` use GPU accelerated PPM to iteratively improve the estimate of molecular geometry by comparing simulated AFM images with reference. This is work-in-progress. Currently, modification of estimate geometry is random (Monte-Carlo), while later we plan to develop a more clever (e.g. Machine-Learned) heuristic for more efficient improvment.
 * `examples/Generator` quickly generates a batch of simulated AFM images (resp. 3D data stacks) which can be further used for machine learning. Especially in connection with (https://github.com/SINGROUP/ASD-AFM).
 
 ## Flavors of PPM
@@ -131,22 +85,19 @@
 * **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
 * **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
 * **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
 
 
 ## For developers
 
-If you would like to contribute to the development of ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
+If you would like to contribute to the development of the ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
 
-
-### Further information
-- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
+## Further information
 - Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
-- API documentation: https://ppafm.readthedocs.io/en/latest/
-
+- Python API documentation: https://ppafm.readthedocs.io/en/latest/
 
 ### Notable publications using Probe Particle Model
 
 * [Prokop Hapala, Georgy Kichin, Christian Wagner, F. Stefan Tautz, Ruslan Temirov, and Pavel Jelínek, Mechanism of high-resolution STM/AFM imaging with functionalized tips, Phys. Rev. B 90, 085421 – Published 19 August 2014](http://journals.aps.org/prb/abstract/10.1103/PhysRevB.90.085421)
 * [Prokop Hapala, Ruslan Temirov, F. Stefan Tautz, and Pavel Jelínek, Origin of High-Resolution IETS-STM Images of Organic Molecules with Functionalized Tips, Phys. Rev. Lett. 113, 226101 – Published 25 November 2014,](http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.226101)
 
 ### License
```

### Comparing `ppafm-0.2.0a3/ppafm.egg-info/SOURCES.txt` & `ppafm-0.2.1a2/ppafm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/pyproject.toml` & `ppafm-0.2.1a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 dependencies = [
     "matplotlib",
     "numpy",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Probe-Particle/ProbeParticleModel"
@@ -55,18 +55,21 @@
 [tool.setuptools.packages]
 find = {namespaces = false}
 
 [tool.setuptools.dynamic]
 version = {attr = "ppafm.version.__version__"}
 
 [tool.bumpver]
-current_version = "v0.2.0a3"
+current_version = "v0.2.1a2"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "ppafm/version.py" = [
     '__version__ = "{pep440_version}"',
 ]
+
+[tool.cibuildwheel]
+skip = ["pp*", "*-manylinux_i686", "*-musllinux*", '*-win32']
```

### Comparing `ppafm-0.2.0a3/tests/test_afmulator.py` & `ppafm-0.2.1a2/tests/test_afmulator.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/tests/test_common.py` & `ppafm-0.2.1a2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/tests/test_datagrid.py` & `ppafm-0.2.1a2/tests/test_datagrid.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/tests/test_io.py` & `ppafm-0.2.1a2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a3/tests/test_vdw.py` & `ppafm-0.2.1a2/tests/test_vdw.py`

 * *Files identical despite different names*

