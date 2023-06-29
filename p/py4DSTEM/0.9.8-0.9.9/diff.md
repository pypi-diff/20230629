# Comparing `tmp/py4DSTEM-0.9.8.tar.gz` & `tmp/py4DSTEM-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py4DSTEM-0.9.8.tar", last modified: Thu Jul  2 19:09:53 2020, max compression
+gzip compressed data, was "dist/py4DSTEM-0.9.9.tar", last modified: Wed Jul  8 19:44:15 2020, max compression
```

## Comparing `py4DSTEM-0.9.8.tar` & `py4DSTEM-0.9.9.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.974819 py4DSTEM-0.9.8/
--rw-r--r--   0 Ben        (501) staff       (20)     6545 2020-07-02 19:09:53.974373 py4DSTEM-0.9.8/PKG-INFO
--rw-r--r--   0 Ben        (501) staff       (20)     4853 2020-07-02 19:09:20.000000 py4DSTEM-0.9.8/README.md
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.904626 py4DSTEM-0.9.8/py4DSTEM/
--rw-r--r--   0 Ben        (501) staff       (20)      148 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.908845 py4DSTEM-0.9.8/py4DSTEM/file/
--rw-r--r--   0 Ben        (501) staff       (20)       45 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.915017 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/
--rw-r--r--   0 Ben        (501) staff       (20)      171 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    18474 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/_metadata.py
--rw-r--r--   0 Ben        (501) staff       (20)    16450 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/datacube.py
--rw-r--r--   0 Ben        (501) staff       (20)     6324 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/dataobject.py
--rw-r--r--   0 Ben        (501) staff       (20)     2275 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/dataslice.py
--rw-r--r--   0 Ben        (501) staff       (20)     1706 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/diffraction.py
--rw-r--r--   0 Ben        (501) staff       (20)      252 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/metadata.py
--rw-r--r--   0 Ben        (501) staff       (20)    11618 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/pointlist.py
--rw-r--r--   0 Ben        (501) staff       (20)     1671 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/file/datastructure/real.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.916160 py4DSTEM-0.9.8/py4DSTEM/file/io/
--rw-r--r--   0 Ben        (501) staff       (20)       20 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.922621 py4DSTEM-0.9.8/py4DSTEM/file/io/native/
--rw-r--r--   0 Ben        (501) staff       (20)      135 2020-06-12 06:26:26.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     7667 2020-06-12 19:38:50.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/append.py
--rw-r--r--   0 Ben        (501) staff       (20)     2481 2020-06-12 20:16:07.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/copy.py
--rw-r--r--   0 Ben        (501) staff       (20)    20185 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/h5rw.py
--rw-r--r--   0 Ben        (501) staff       (20)    14731 2020-06-17 00:24:29.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/read_py4DSTEM.py
--rw-r--r--   0 Ben        (501) staff       (20)    14776 2020-06-12 20:16:07.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/read_py4DSTEM_legacy.py
--rw-r--r--   0 Ben        (501) staff       (20)     5445 2020-06-15 07:35:17.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/read_utils.py
--rw-r--r--   0 Ben        (501) staff       (20)     2482 2020-06-15 06:33:06.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/remove.py
--rw-r--r--   0 Ben        (501) staff       (20)    23917 2020-06-12 05:59:19.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/native/write.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.926545 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/
--rw-r--r--   0 Ben        (501) staff       (20)      154 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     2356 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_dm.py
--rw-r--r--   0 Ben        (501) staff       (20)     1399 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_empad.py
--rw-r--r--   0 Ben        (501) staff       (20)     1415 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_gatan_K2_bin.py
--rw-r--r--   0 Ben        (501) staff       (20)     1448 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_kitware_counted.py
--rw-r--r--   0 Ben        (501) staff       (20)     1512 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_mrc_relativity.py
--rw-r--r--   0 Ben        (501) staff       (20)     6875 2020-06-12 19:18:42.000000 py4DSTEM-0.9.8/py4DSTEM/file/io/read.py
--rw-r--r--   0 Ben        (501) staff       (20)     3954 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/file/log.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.930487 py4DSTEM-0.9.8/py4DSTEM/gui/
--rw-r--r--   0 Ben        (501) staff       (20)       66 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    30303 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/dialogs.py
--rw-r--r--   0 Ben        (501) staff       (20)     8946 2020-06-15 07:35:17.000000 py4DSTEM-0.9.8/py4DSTEM/gui/gui_utils.py
--rw-r--r--   0 Ben        (501) staff       (20)      270 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/runGUI.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.935522 py4DSTEM-0.9.8/py4DSTEM/gui/strain/
--rw-r--r--   0 Ben        (501) staff       (20)     3144 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/strain/ImageViewMasked.py
--rw-r--r--   0 Ben        (501) staff       (20)       81 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/strain/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     5459 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/strain/cmaptopg.py
--rw-r--r--   0 Ben        (501) staff       (20)    56022 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/gui/strain/panels.py
--rw-r--r--   0 Ben        (501) staff       (20)     2517 2020-04-01 19:37:32.000000 py4DSTEM-0.9.8/py4DSTEM/gui/strain/strain_window.py
--rw-r--r--   0 Ben        (501) staff       (20)    40894 2020-06-15 07:35:17.000000 py4DSTEM-0.9.8/py4DSTEM/gui/viewer.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.936263 py4DSTEM-0.9.8/py4DSTEM/process/
--rw-r--r--   0 Ben        (501) staff       (20)      211 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/__init__.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.940739 py4DSTEM-0.9.8/py4DSTEM/process/calibration/
--rw-r--r--   0 Ben        (501) staff       (20)      121 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/calibration/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     8164 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/calibration/diffractionshifts.py
--rw-r--r--   0 Ben        (501) staff       (20)     7588 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/calibration/ellipticaldistortion.py
--rw-r--r--   0 Ben        (501) staff       (20)     4240 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/calibration/qpixelsize.py
--rw-r--r--   0 Ben        (501) staff       (20)     4573 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/calibration/rotation.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.942898 py4DSTEM-0.9.8/py4DSTEM/process/classification/
--rw-r--r--   0 Ben        (501) staff       (20)       67 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/classification/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    38194 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/classification/braggvectorclassification.py
--rw-r--r--   0 Ben        (501) staff       (20)     7472 2020-07-02 19:09:20.000000 py4DSTEM-0.9.8/py4DSTEM/process/classification/classutils.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.946545 py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/
--rw-r--r--   0 Ben        (501) staff       (20)       81 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     4248 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/braggvectormap.py
--rw-r--r--   0 Ben        (501) staff       (20)    31502 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/diskdetection.py
--rw-r--r--   0 Ben        (501) staff       (20)    20337 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/diskdetection_parallel.py
--rw-r--r--   0 Ben        (501) staff       (20)    12552 2020-07-02 06:35:14.000000 py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/probe.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.947661 py4DSTEM-0.9.8/py4DSTEM/process/dpc/
--rw-r--r--   0 Ben        (501) staff       (20)       19 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/dpc/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    25047 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/process/dpc/dpc.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.949630 py4DSTEM-0.9.8/py4DSTEM/process/fit/
--rw-r--r--   0 Ben        (501) staff       (20)       44 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/fit/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     2471 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/fit/fit.py
--rw-r--r--   0 Ben        (501) staff       (20)      215 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/fit/functions.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.952985 py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/
--rw-r--r--   0 Ben        (501) staff       (20)       91 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    10127 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/fit.py
--rw-r--r--   0 Ben        (501) staff       (20)    10470 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/index.py
--rw-r--r--   0 Ben        (501) staff       (20)     8845 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/initialguess.py
--rw-r--r--   0 Ben        (501) staff       (20)     8976 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/strain.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.956030 py4DSTEM-0.9.8/py4DSTEM/process/preprocess/
--rw-r--r--   0 Ben        (501) staff       (20)      111 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/preprocess/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     7688 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/process/preprocess/darkreference.py
--rw-r--r--   0 Ben        (501) staff       (20)    18808 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/preprocess/electroncount.py
--rw-r--r--   0 Ben        (501) staff       (20)     5615 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/process/preprocess/preprocess.py
--rw-r--r--   0 Ben        (501) staff       (20)     6887 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/preprocess/relativity.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.958690 py4DSTEM-0.9.8/py4DSTEM/process/ptychography/
--rw-r--r--   0 Ben        (501) staff       (20)       38 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/ptychography/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    10726 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/ptychography/ssb.py
--rw-r--r--   0 Ben        (501) staff       (20)     7644 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/ptychography/utils.py
--rw-r--r--   0 Ben        (501) staff       (20)        0 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/ptychography/wdd.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.960422 py4DSTEM-0.9.8/py4DSTEM/process/rdf/
--rw-r--r--   0 Ben        (501) staff       (20)       18 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/rdf/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     6971 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/process/rdf/amorph.py
--rw-r--r--   0 Ben        (501) staff       (20)     2377 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/rdf/rdf.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.968405 py4DSTEM-0.9.8/py4DSTEM/process/utils/
--rw-r--r--   0 Ben        (501) staff       (20)      242 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     1093 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/aberrations.py
--rw-r--r--   0 Ben        (501) staff       (20)    25892 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/cartesian_to_polarelliptical_transform.py
--rw-r--r--   0 Ben        (501) staff       (20)    16792 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/ellipticalCoords.py
--rw-r--r--   0 Ben        (501) staff       (20)     7125 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/multicorr.py
--rw-r--r--   0 Ben        (501) staff       (20)     8596 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/parameters.py
--rw-r--r--   0 Ben        (501) staff       (20)    27558 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/scatteringFactors.txt
--rw-r--r--   0 Ben        (501) staff       (20)     3379 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/single_atom_scatter.py
--rw-r--r--   0 Ben        (501) staff       (20)     1014 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/tqdmnd.py
--rw-r--r--   0 Ben        (501) staff       (20)    22761 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/process/utils/utils.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.969701 py4DSTEM-0.9.8/py4DSTEM/process/virtualimage/
--rw-r--r--   0 Ben        (501) staff       (20)       28 2020-04-01 19:37:33.000000 py4DSTEM-0.9.8/py4DSTEM/process/virtualimage/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     2886 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/process/virtualimage/virtualimage.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.970702 py4DSTEM-0.9.8/py4DSTEM/process/virtualimage_viewer/
--rw-r--r--   0 Ben        (501) staff       (20)       35 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/process/virtualimage_viewer/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)    11938 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/process/virtualimage_viewer/virtualimage_viewer.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.971858 py4DSTEM-0.9.8/py4DSTEM/simulate/
--rw-r--r--   0 Ben        (501) staff       (20)       24 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/simulate/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     9925 2020-06-10 08:33:52.000000 py4DSTEM-0.9.8/py4DSTEM/simulate/kinematic.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.973578 py4DSTEM-0.9.8/py4DSTEM/test/
--rw-r--r--   0 Ben        (501) staff       (20)        0 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/test/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)      237 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/test/test.py
--rw-r--r--   0 Ben        (501) staff       (20)     1771 2020-04-02 05:41:22.000000 py4DSTEM-0.9.8/py4DSTEM/test/test_virtualimage.py
--rw-r--r--   0 Ben        (501) staff       (20)       20 2020-07-02 19:09:20.000000 py4DSTEM-0.9.8/py4DSTEM/version.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-02 19:09:53.907609 py4DSTEM-0.9.8/py4DSTEM.egg-info/
--rw-r--r--   0 Ben        (501) staff       (20)     6545 2020-07-02 19:09:53.000000 py4DSTEM-0.9.8/py4DSTEM.egg-info/PKG-INFO
--rw-r--r--   0 Ben        (501) staff       (20)     3831 2020-07-02 19:09:53.000000 py4DSTEM-0.9.8/py4DSTEM.egg-info/SOURCES.txt
--rw-r--r--   0 Ben        (501) staff       (20)        1 2020-07-02 19:09:53.000000 py4DSTEM-0.9.8/py4DSTEM.egg-info/dependency_links.txt
--rw-r--r--   0 Ben        (501) staff       (20)       57 2020-07-02 19:09:53.000000 py4DSTEM-0.9.8/py4DSTEM.egg-info/entry_points.txt
--rw-r--r--   0 Ben        (501) staff       (20)      246 2020-07-02 19:09:53.000000 py4DSTEM-0.9.8/py4DSTEM.egg-info/requires.txt
--rw-r--r--   0 Ben        (501) staff       (20)        9 2020-07-02 19:09:53.000000 py4DSTEM-0.9.8/py4DSTEM.egg-info/top_level.txt
--rw-r--r--   0 Ben        (501) staff       (20)       38 2020-07-02 19:09:53.974926 py4DSTEM-0.9.8/setup.cfg
--rw-r--r--   0 Ben        (501) staff       (20)     1272 2020-07-02 19:09:20.000000 py4DSTEM-0.9.8/setup.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.291355 py4DSTEM-0.9.9/
+-rw-r--r--   0 Ben        (501) staff       (20)     6545 2020-07-08 19:44:15.291012 py4DSTEM-0.9.9/PKG-INFO
+-rw-r--r--   0 Ben        (501) staff       (20)     4853 2020-07-08 19:43:50.000000 py4DSTEM-0.9.9/README.md
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.218109 py4DSTEM-0.9.9/py4DSTEM/
+-rw-r--r--   0 Ben        (501) staff       (20)      148 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/__init__.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.222371 py4DSTEM-0.9.9/py4DSTEM/file/
+-rw-r--r--   0 Ben        (501) staff       (20)       45 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/__init__.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.228012 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/
+-rw-r--r--   0 Ben        (501) staff       (20)      171 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    18474 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/_metadata.py
+-rw-r--r--   0 Ben        (501) staff       (20)    16450 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/datacube.py
+-rw-r--r--   0 Ben        (501) staff       (20)     6324 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/dataobject.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2275 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/dataslice.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1706 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/diffraction.py
+-rw-r--r--   0 Ben        (501) staff       (20)      252 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/metadata.py
+-rw-r--r--   0 Ben        (501) staff       (20)    11618 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/pointlist.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1671 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/file/datastructure/real.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.229157 py4DSTEM-0.9.9/py4DSTEM/file/io/
+-rw-r--r--   0 Ben        (501) staff       (20)       20 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/__init__.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.235646 py4DSTEM-0.9.9/py4DSTEM/file/io/native/
+-rw-r--r--   0 Ben        (501) staff       (20)      135 2020-06-12 06:26:26.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     7667 2020-06-12 19:38:50.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/append.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2481 2020-06-12 20:16:07.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/copy.py
+-rw-r--r--   0 Ben        (501) staff       (20)    20185 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/h5rw.py
+-rw-r--r--   0 Ben        (501) staff       (20)    14731 2020-06-17 00:24:29.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/read_py4DSTEM.py
+-rw-r--r--   0 Ben        (501) staff       (20)    14776 2020-06-12 20:16:07.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/read_py4DSTEM_legacy.py
+-rw-r--r--   0 Ben        (501) staff       (20)     5445 2020-06-15 07:35:17.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/read_utils.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2482 2020-06-15 06:33:06.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/remove.py
+-rw-r--r--   0 Ben        (501) staff       (20)    23917 2020-06-12 05:59:19.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/native/write.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.239608 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/
+-rw-r--r--   0 Ben        (501) staff       (20)      154 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2356 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_dm.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1399 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_empad.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1415 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_gatan_K2_bin.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1448 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_kitware_counted.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1512 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_mrc_relativity.py
+-rw-r--r--   0 Ben        (501) staff       (20)     6875 2020-06-12 19:18:42.000000 py4DSTEM-0.9.9/py4DSTEM/file/io/read.py
+-rw-r--r--   0 Ben        (501) staff       (20)     3954 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/file/log.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.244096 py4DSTEM-0.9.9/py4DSTEM/gui/
+-rw-r--r--   0 Ben        (501) staff       (20)       66 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    30303 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/dialogs.py
+-rw-r--r--   0 Ben        (501) staff       (20)     8946 2020-06-15 07:35:17.000000 py4DSTEM-0.9.9/py4DSTEM/gui/gui_utils.py
+-rw-r--r--   0 Ben        (501) staff       (20)      270 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/runGUI.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.247788 py4DSTEM-0.9.9/py4DSTEM/gui/strain/
+-rw-r--r--   0 Ben        (501) staff       (20)     3144 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/strain/ImageViewMasked.py
+-rw-r--r--   0 Ben        (501) staff       (20)       81 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/strain/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     5459 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/strain/cmaptopg.py
+-rw-r--r--   0 Ben        (501) staff       (20)    56022 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/gui/strain/panels.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2517 2020-04-01 19:37:32.000000 py4DSTEM-0.9.9/py4DSTEM/gui/strain/strain_window.py
+-rw-r--r--   0 Ben        (501) staff       (20)    40894 2020-06-15 07:35:17.000000 py4DSTEM-0.9.9/py4DSTEM/gui/viewer.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.248599 py4DSTEM-0.9.9/py4DSTEM/process/
+-rw-r--r--   0 Ben        (501) staff       (20)      211 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/__init__.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.251652 py4DSTEM-0.9.9/py4DSTEM/process/calibration/
+-rw-r--r--   0 Ben        (501) staff       (20)      121 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/calibration/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     8164 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/calibration/diffractionshifts.py
+-rw-r--r--   0 Ben        (501) staff       (20)     7588 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/calibration/ellipticaldistortion.py
+-rw-r--r--   0 Ben        (501) staff       (20)     4240 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/calibration/qpixelsize.py
+-rw-r--r--   0 Ben        (501) staff       (20)     4573 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/calibration/rotation.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.253780 py4DSTEM-0.9.9/py4DSTEM/process/classification/
+-rw-r--r--   0 Ben        (501) staff       (20)       67 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/classification/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    38801 2020-07-08 19:43:50.000000 py4DSTEM-0.9.9/py4DSTEM/process/classification/braggvectorclassification.py
+-rw-r--r--   0 Ben        (501) staff       (20)     7472 2020-07-02 19:09:20.000000 py4DSTEM-0.9.9/py4DSTEM/process/classification/classutils.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.257454 py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/
+-rw-r--r--   0 Ben        (501) staff       (20)       81 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     4248 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/braggvectormap.py
+-rw-r--r--   0 Ben        (501) staff       (20)    31502 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/diskdetection.py
+-rw-r--r--   0 Ben        (501) staff       (20)    20337 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/diskdetection_parallel.py
+-rw-r--r--   0 Ben        (501) staff       (20)    12552 2020-07-02 06:35:14.000000 py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/probe.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.258776 py4DSTEM-0.9.9/py4DSTEM/process/dpc/
+-rw-r--r--   0 Ben        (501) staff       (20)       19 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/dpc/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    25047 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/process/dpc/dpc.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.260799 py4DSTEM-0.9.9/py4DSTEM/process/fit/
+-rw-r--r--   0 Ben        (501) staff       (20)       44 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/fit/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2471 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/fit/fit.py
+-rw-r--r--   0 Ben        (501) staff       (20)      215 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/fit/functions.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.264411 py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/
+-rw-r--r--   0 Ben        (501) staff       (20)       91 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    10127 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/fit.py
+-rw-r--r--   0 Ben        (501) staff       (20)    10470 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/index.py
+-rw-r--r--   0 Ben        (501) staff       (20)     8845 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/initialguess.py
+-rw-r--r--   0 Ben        (501) staff       (20)     8976 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/strain.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.268684 py4DSTEM-0.9.9/py4DSTEM/process/preprocess/
+-rw-r--r--   0 Ben        (501) staff       (20)      111 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/preprocess/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     7688 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/process/preprocess/darkreference.py
+-rw-r--r--   0 Ben        (501) staff       (20)    18808 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/preprocess/electroncount.py
+-rw-r--r--   0 Ben        (501) staff       (20)     5615 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/process/preprocess/preprocess.py
+-rw-r--r--   0 Ben        (501) staff       (20)     6887 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/preprocess/relativity.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.272775 py4DSTEM-0.9.9/py4DSTEM/process/ptychography/
+-rw-r--r--   0 Ben        (501) staff       (20)       38 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/ptychography/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    10726 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/ptychography/ssb.py
+-rw-r--r--   0 Ben        (501) staff       (20)     7644 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/ptychography/utils.py
+-rw-r--r--   0 Ben        (501) staff       (20)        0 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/ptychography/wdd.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.274959 py4DSTEM-0.9.9/py4DSTEM/process/rdf/
+-rw-r--r--   0 Ben        (501) staff       (20)       18 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/rdf/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     6971 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/process/rdf/amorph.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2377 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/rdf/rdf.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.283619 py4DSTEM-0.9.9/py4DSTEM/process/utils/
+-rw-r--r--   0 Ben        (501) staff       (20)      242 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1093 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/aberrations.py
+-rw-r--r--   0 Ben        (501) staff       (20)    25892 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/cartesian_to_polarelliptical_transform.py
+-rw-r--r--   0 Ben        (501) staff       (20)    16792 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/ellipticalCoords.py
+-rw-r--r--   0 Ben        (501) staff       (20)     7125 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/multicorr.py
+-rw-r--r--   0 Ben        (501) staff       (20)     8596 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/parameters.py
+-rw-r--r--   0 Ben        (501) staff       (20)    27558 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/scatteringFactors.txt
+-rw-r--r--   0 Ben        (501) staff       (20)     3379 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/single_atom_scatter.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1014 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/tqdmnd.py
+-rw-r--r--   0 Ben        (501) staff       (20)    22761 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/process/utils/utils.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.285202 py4DSTEM-0.9.9/py4DSTEM/process/virtualimage/
+-rw-r--r--   0 Ben        (501) staff       (20)       28 2020-04-01 19:37:33.000000 py4DSTEM-0.9.9/py4DSTEM/process/virtualimage/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     2886 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/process/virtualimage/virtualimage.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.286372 py4DSTEM-0.9.9/py4DSTEM/process/virtualimage_viewer/
+-rw-r--r--   0 Ben        (501) staff       (20)       35 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/process/virtualimage_viewer/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    11938 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/process/virtualimage_viewer/virtualimage_viewer.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.287572 py4DSTEM-0.9.9/py4DSTEM/simulate/
+-rw-r--r--   0 Ben        (501) staff       (20)       24 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/simulate/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)     9925 2020-06-10 08:33:52.000000 py4DSTEM-0.9.9/py4DSTEM/simulate/kinematic.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.289307 py4DSTEM-0.9.9/py4DSTEM/test/
+-rw-r--r--   0 Ben        (501) staff       (20)        0 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/test/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)      237 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/test/test.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1771 2020-04-02 05:41:22.000000 py4DSTEM-0.9.9/py4DSTEM/test/test_virtualimage.py
+-rw-r--r--   0 Ben        (501) staff       (20)       20 2020-07-08 19:43:50.000000 py4DSTEM-0.9.9/py4DSTEM/version.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2020-07-08 19:44:15.221146 py4DSTEM-0.9.9/py4DSTEM.egg-info/
+-rw-r--r--   0 Ben        (501) staff       (20)     6545 2020-07-08 19:44:14.000000 py4DSTEM-0.9.9/py4DSTEM.egg-info/PKG-INFO
+-rw-r--r--   0 Ben        (501) staff       (20)     3831 2020-07-08 19:44:15.000000 py4DSTEM-0.9.9/py4DSTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 Ben        (501) staff       (20)        1 2020-07-08 19:44:14.000000 py4DSTEM-0.9.9/py4DSTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 Ben        (501) staff       (20)       57 2020-07-08 19:44:14.000000 py4DSTEM-0.9.9/py4DSTEM.egg-info/entry_points.txt
+-rw-r--r--   0 Ben        (501) staff       (20)      246 2020-07-08 19:44:14.000000 py4DSTEM-0.9.9/py4DSTEM.egg-info/requires.txt
+-rw-r--r--   0 Ben        (501) staff       (20)        9 2020-07-08 19:44:14.000000 py4DSTEM-0.9.9/py4DSTEM.egg-info/top_level.txt
+-rw-r--r--   0 Ben        (501) staff       (20)       38 2020-07-08 19:44:15.291472 py4DSTEM-0.9.9/setup.cfg
+-rw-r--r--   0 Ben        (501) staff       (20)     1272 2020-07-08 19:43:50.000000 py4DSTEM-0.9.9/setup.py
```

### Comparing `py4DSTEM-0.9.8/PKG-INFO` & `py4DSTEM-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4DSTEM
-Version: 0.9.8
+Version: 0.9.9
 Summary: An open source python package for processing and analysis of 4D STEM data.
 Home-page: https://github.com/py4dstem/py4DSTEM/
 Author: Benjamin H. Savitzky
 Author-email: ben.savitzky@gmail.com
 License: GNU GPLv3
 Description: # py4DSTEM: open source processing and analysis of 4D-STEM data
         [![DOI](https://zenodo.org/badge/148587083.svg)](https://zenodo.org/badge/latestdoi/148587083)
@@ -145,15 +145,15 @@
         
         * ipyparallel
         * dask
         
         
         ### Versioning
         
-        v. 0.9.8
+        v. 0.9.9
         
         
         
         ### License
         
         GNU GPLv3
```

### Comparing `py4DSTEM-0.9.8/README.md` & `py4DSTEM-0.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 * ipyparallel
 * dask
 
 
 ### Versioning
 
-v. 0.9.8
+v. 0.9.9
 
 
 
 ### License
 
 GNU GPLv3
```

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/_metadata.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/_metadata.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/datacube.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/datacube.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/dataobject.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/dataobject.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/dataslice.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/dataslice.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/diffraction.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/diffraction.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/pointlist.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/pointlist.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/datastructure/real.py` & `py4DSTEM-0.9.9/py4DSTEM/file/datastructure/real.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/append.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/append.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/copy.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/copy.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/h5rw.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/h5rw.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/read_py4DSTEM.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/read_py4DSTEM.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/read_py4DSTEM_legacy.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/read_py4DSTEM_legacy.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/read_utils.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/read_utils.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/remove.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/remove.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/native/write.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/native/write.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_dm.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_dm.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_empad.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_empad.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_gatan_K2_bin.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_gatan_K2_bin.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_kitware_counted.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_kitware_counted.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/nonnative/read_mrc_relativity.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/nonnative/read_mrc_relativity.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/io/read.py` & `py4DSTEM-0.9.9/py4DSTEM/file/io/read.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/file/log.py` & `py4DSTEM-0.9.9/py4DSTEM/file/log.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/dialogs.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/gui_utils.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/strain/ImageViewMasked.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/strain/ImageViewMasked.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/strain/cmaptopg.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/strain/cmaptopg.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/strain/panels.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/strain/panels.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/strain/strain_window.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/strain/strain_window.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/gui/viewer.py` & `py4DSTEM-0.9.9/py4DSTEM/gui/viewer.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/calibration/diffractionshifts.py` & `py4DSTEM-0.9.9/py4DSTEM/process/calibration/diffractionshifts.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/calibration/ellipticaldistortion.py` & `py4DSTEM-0.9.9/py4DSTEM/process/calibration/ellipticaldistortion.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/calibration/qpixelsize.py` & `py4DSTEM-0.9.9/py4DSTEM/process/calibration/qpixelsize.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/calibration/rotation.py` & `py4DSTEM-0.9.9/py4DSTEM/process/calibration/rotation.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/classification/braggvectorclassification.py` & `py4DSTEM-0.9.9/py4DSTEM/process/classification/braggvectorclassification.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         get_candidate_class_BPs:
             as above, for the current candidate class
         get_candidate_class_image:
             as above, for the current candidate class
 
     """
 
-    def __init__(self, braggpeaks, Qx, Qy, X_is_boolean=True):
+    def __init__(self, braggpeaks, Qx, Qy, X_is_boolean=True, max_dist=None):
         """
         Initializes a BraggVectorClassification instance.
 
         This method:
         1.  Gets integer labels for all of the detected Bragg peaks, according to which
             (Qx,Qy) is closest, then generating a corresponding set of integers for each scan
             position.  See get_braggpeak_labels_by_scan_position() docstring for more info.
@@ -90,26 +90,28 @@
 
         Accepts:
             braggpeaks          (PointListArray) Bragg peaks; must have coords 'qx' and 'qy'
             Qx                  (ndarray of floats) x-coords of the voronoi points
             Qy                  (ndarray of floats) y-coords of the voronoi points
             X_is_boolean        (bool) if True, populate X with bools (BP is or is not present)
                                 if False, populate X with floats (BP c.c. intensities)
+            max_dist            (None or number) maximum distance from a given voronoi point a peak
+                                can be and still be associated with this label
         """
         assert isinstance(braggpeaks,PointListArray), "braggpeaks must be a PointListArray"
         assert np.all([name in braggpeaks.dtype.names for name in ('qx','qy')]), "braggpeaks must contain coords 'qx' and 'qy'"
         assert len(Qx)==len(Qy), "Qx and Qy must have same length"
         self.braggpeaks = braggpeaks
         self.R_Nx = braggpeaks.shape[0]
         self.R_Ny = braggpeaks.shape[1]
         self.Qx = Qx
         self.Qy = Qy
 
         # Get the sets of Bragg peaks present at each scan position
-        self.braggpeak_labels = get_braggpeak_labels_by_scan_position(braggpeaks, Qx, Qy)
+        self.braggpeak_labels = get_braggpeak_labels_by_scan_position(braggpeaks, Qx, Qy, max_dist)
 
         # Construct X matrix
         self.N_feat = len(self.Qx)
         self.N_meas = self.R_Nx*self.R_Ny
 
         self.X = np.zeros((self.N_feat,self.N_meas))
         for Rx in range(self.R_Nx):
@@ -656,15 +658,15 @@
         assert self.H_next is not None, "H_next is not assigned."
 
         return self.H_next[i,:].reshape((self.R_Nx,self.R_Ny))
 
 
 ### Functions for initial class determination ###
 
-def get_braggpeak_labels_by_scan_position(braggpeaks, Qx, Qy):
+def get_braggpeak_labels_by_scan_position(braggpeaks, Qx, Qy, max_dist=None):
     """
     For each scan position, gets a set of integers, specifying the bragg peaks at this scan
     position.
 
     From a set of positions in diffraction space (Qx,Qy), assign each detected bragg peak in the
     PointListArray braggpeaks a label corresponding to the index of the closest position; thus
     for a bragg peak at (qx,qy), if the closest position in (Qx,Qy) is (Qx[i],Qy[i]), assign
@@ -675,14 +677,16 @@
     For each scan position, get the set of all indices i for all bragg peaks found at this scan
     position.
 
     Accepts:
         braggpeaks          (PointListArray) Bragg peaks; must have coords 'qx' and 'qy'
         Qx                  (ndarray of floats) x-coords of the voronoi points
         Qy                  (ndarray of floats) y-coords of the voronoi points
+        max_dist            (None or number) maximum distance from a given voronoi point a peak
+                            can be and still be associated with this label
 
     Returns:
         braggpeak_labels    (list of lists of sets) the labels found at each scan position.
                             Scan position (Rx,Ry) is accessed via braggpeak_labels[Rx][Ry]
     """
     assert isinstance(braggpeaks,PointListArray), "braggpeaks must be a PointListArray"
     assert np.all([name in braggpeaks.dtype.names for name in ('qx','qy')]), "braggpeaks must contain coords 'qx' and 'qy'"
@@ -690,15 +694,19 @@
     braggpeak_labels = [[set() for i in range(braggpeaks.shape[1])] for j in range(braggpeaks.shape[0])]
     for Rx in range(braggpeaks.shape[0]):
         for Ry in range(braggpeaks.shape[1]):
             s = braggpeak_labels[Rx][Ry]
             pointlist = braggpeaks.get_pointlist(Rx,Ry)
             for i in range(pointlist.length):
                 label = np.argmin(np.hypot(Qx-pointlist.data['qx'][i],Qy-pointlist.data['qy'][i]))
-                s.add(label)
+                if max_dist is not None:
+                    if np.hypot(Qx[label]-pointlist.data['qx'][i],Qy[label]-pointlist.data['qy'][i]) < max_dist:
+                        s.add(label)
+                else:
+                    s.add(label)
 
     return braggpeak_labels
 
 
 def get_initial_classes(braggpeak_labels, N, thresh=0.3, BP_fraction_thresh=0.1, max_iterations=200,
                         n_corr_init=2):
     """
```

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/classification/classutils.py` & `py4DSTEM-0.9.9/py4DSTEM/process/classification/classutils.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/braggvectormap.py` & `py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/braggvectormap.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/diskdetection.py` & `py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/diskdetection.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/diskdetection_parallel.py` & `py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/diskdetection_parallel.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/diskdetection/probe.py` & `py4DSTEM-0.9.9/py4DSTEM/process/diskdetection/probe.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/dpc/dpc.py` & `py4DSTEM-0.9.9/py4DSTEM/process/dpc/dpc.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/fit/fit.py` & `py4DSTEM-0.9.9/py4DSTEM/process/fit/fit.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/fit.py` & `py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/fit.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/index.py` & `py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/index.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/initialguess.py` & `py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/initialguess.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/latticevectors/strain.py` & `py4DSTEM-0.9.9/py4DSTEM/process/latticevectors/strain.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/preprocess/darkreference.py` & `py4DSTEM-0.9.9/py4DSTEM/process/preprocess/darkreference.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/preprocess/electroncount.py` & `py4DSTEM-0.9.9/py4DSTEM/process/preprocess/electroncount.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/preprocess/preprocess.py` & `py4DSTEM-0.9.9/py4DSTEM/process/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/preprocess/relativity.py` & `py4DSTEM-0.9.9/py4DSTEM/process/preprocess/relativity.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/ptychography/ssb.py` & `py4DSTEM-0.9.9/py4DSTEM/process/ptychography/ssb.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/ptychography/utils.py` & `py4DSTEM-0.9.9/py4DSTEM/process/ptychography/utils.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/rdf/amorph.py` & `py4DSTEM-0.9.9/py4DSTEM/process/rdf/amorph.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/rdf/rdf.py` & `py4DSTEM-0.9.9/py4DSTEM/process/rdf/rdf.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/aberrations.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/aberrations.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/cartesian_to_polarelliptical_transform.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/cartesian_to_polarelliptical_transform.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/ellipticalCoords.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/ellipticalCoords.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/multicorr.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/multicorr.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/parameters.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/scatteringFactors.txt` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/scatteringFactors.txt`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/single_atom_scatter.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/single_atom_scatter.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/tqdmnd.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/utils/utils.py` & `py4DSTEM-0.9.9/py4DSTEM/process/utils/utils.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/virtualimage/virtualimage.py` & `py4DSTEM-0.9.9/py4DSTEM/process/virtualimage/virtualimage.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/process/virtualimage_viewer/virtualimage_viewer.py` & `py4DSTEM-0.9.9/py4DSTEM/process/virtualimage_viewer/virtualimage_viewer.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/simulate/kinematic.py` & `py4DSTEM-0.9.9/py4DSTEM/simulate/kinematic.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM/test/test_virtualimage.py` & `py4DSTEM-0.9.9/py4DSTEM/test/test_virtualimage.py`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/py4DSTEM.egg-info/PKG-INFO` & `py4DSTEM-0.9.9/py4DSTEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4DSTEM
-Version: 0.9.8
+Version: 0.9.9
 Summary: An open source python package for processing and analysis of 4D STEM data.
 Home-page: https://github.com/py4dstem/py4DSTEM/
 Author: Benjamin H. Savitzky
 Author-email: ben.savitzky@gmail.com
 License: GNU GPLv3
 Description: # py4DSTEM: open source processing and analysis of 4D-STEM data
         [![DOI](https://zenodo.org/badge/148587083.svg)](https://zenodo.org/badge/latestdoi/148587083)
@@ -145,15 +145,15 @@
         
         * ipyparallel
         * dask
         
         
         ### Versioning
         
-        v. 0.9.8
+        v. 0.9.9
         
         
         
         ### License
         
         GNU GPLv3
```

### Comparing `py4DSTEM-0.9.8/py4DSTEM.egg-info/SOURCES.txt` & `py4DSTEM-0.9.9/py4DSTEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4DSTEM-0.9.8/setup.py` & `py4DSTEM-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     long_description = f.read()
 
 setup(
     name='py4DSTEM',
-    version='0.9.8',
+    version='0.9.9',
     packages=find_packages(),
     description='An open source python package for processing and analysis of 4D STEM data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/py4dstem/py4DSTEM/',
     author='Benjamin H. Savitzky',
     author_email='ben.savitzky@gmail.com',
```

