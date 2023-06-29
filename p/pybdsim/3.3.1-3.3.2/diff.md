# Comparing `tmp/pybdsim-3.3.1.tar.gz` & `tmp/pybdsim-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdsim-3.3.1.tar", last modified: Mon May 15 09:10:48 2023, max compression
+gzip compressed data, was "pybdsim-3.3.2.tar", last modified: Thu Jun 29 15:37:39 2023, max compression
```

## Comparing `pybdsim-3.3.1.tar` & `pybdsim-3.3.2.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.574314 pybdsim-3.3.1/
--rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.3.1/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.3.1/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.3.1/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.3.1/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-05-15 09:10:48.574416 pybdsim-3.3.1/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      936 2023-05-08 16:07:40.000000 pybdsim-3.3.1/README.md
--rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.3.1/bitbucket-pipelines.yml
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.537600 pybdsim-3.3.1/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)  1199563 2023-05-08 16:10:24.000000 pybdsim-3.3.1/docs/pybdsim.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.543129 pybdsim-3.3.1/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      307 2023-05-08 16:07:51.000000 pybdsim-3.3.1/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.3.1/docs/source/builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.3.1/docs/source/classes.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.3.1/docs/source/compare.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.3.1/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.3.1/docs/source/convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.3.1/docs/source/data.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.3.1/docs/source/data_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.3.1/docs/source/developer.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12893 2023-05-11 15:00:20.000000 pybdsim-3.3.1/docs/source/fieldmaps.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.545772 pybdsim-3.3.1/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/source/figures/rebdsimFileHistograms.png
--rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/source/figures/rebdsimFileHistogramsWrapped.png
--rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/source/figures/rebdsimFileMembers.png
--rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/source/figures/simpleHistogramPlot.png
--rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.3.1/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2198 2023-05-08 16:05:46.000000 pybdsim-3.3.1/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.3.1/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.3.1/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.3.1/docs/source/plotting.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.3.1/docs/source/support.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12360 2023-05-15 09:08:38.000000 pybdsim-3.3.1/docs/source/version_history.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.546423 pybdsim-3.3.1/examples/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.547592 pybdsim-3.3.1/examples/1_builder/
--rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/1_builder/1_builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/1_builder/1_testmachine.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/1_builder/1_testmachine.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.549940 pybdsim-3.3.1/examples/2_convert/
--rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/1_madxtfs2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/1_madxtfs2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/2_convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/2_transport2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/2_transport2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/transport_example.dat
--rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/transport_example.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/twiss35tevb1_short.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.3.1/examples/2_convert/twiss35tevb1_short.tar.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.550121 pybdsim-3.3.1/examples/3_optics/
--rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.3.1/examples/3_optics/optics_validation.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.550336 pybdsim-3.3.1/examples/4_uproot/
--rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.3.1/examples/4_uproot/4_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.3.1/examples/examples.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1846 2023-05-15 09:07:01.000000 pybdsim-3.3.1/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      258 2023-05-15 09:10:48.574682 pybdsim-3.3.1/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.3.1/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.533836 pybdsim-3.3.1/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.557885 pybdsim-3.3.1/src/pybdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.3.1/src/pybdsim/Beam.py
--rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.3.1/src/pybdsim/Builder.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.560891 pybdsim-3.3.1/src/pybdsim/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.3.1/src/pybdsim/Compare/_BdsimBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.3.1/src/pybdsim/Compare/_ElegantBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Compare/_Mad8BdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23115 2023-04-26 11:54:49.000000 pybdsim-3.3.1/src/pybdsim/Compare/_MadxBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Compare/_MadxMadxComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48470 2023-04-26 11:55:02.000000 pybdsim-3.3.1/src/pybdsim/Compare/_MultipleCodeComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Compare/_SadComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6438 2023-05-08 16:03:57.000000 pybdsim-3.3.1/src/pybdsim/Compare/_TransportBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      827 2023-05-08 16:04:54.000000 pybdsim-3.3.1/src/pybdsim/Compare/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.3.1/src/pybdsim/Constants.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.563869 pybdsim-3.3.1/src/pybdsim/Convert/
--rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.3.1/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.3.1/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
--rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.3.1/src/pybdsim/Convert/_CPyMad2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Convert/_ElegantParamToStrength.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Convert/_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Convert/_Rebdsim2Numpy.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Convert/_SadFlat2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     4483 2023-05-08 16:02:45.000000 pybdsim-3.3.1/src/pybdsim/Convert/_Transport2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-05-08 15:59:37.000000 pybdsim-3.3.1/src/pybdsim/Convert/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Convert/collimator_analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)    79780 2023-05-03 14:03:26.000000 pybdsim-3.3.1/src/pybdsim/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.3.1/src/pybdsim/DataUproot.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.564733 pybdsim-3.3.1/src/pybdsim/Field/
--rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Field/FieldPlotter.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Field/FieldPlotterVtk.py
--rw-r--r--   0 lnevay     (501) staff       (20)    16881 2023-04-17 18:48:37.000000 pybdsim-3.3.1/src/pybdsim/Field/_Field.py
--rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.3.1/src/pybdsim/Field/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.3.1/src/pybdsim/Geant4.py
--rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.3.1/src/pybdsim/Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Joinhistograms.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.3.1/src/pybdsim/ModelProcessing.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.534119 pybdsim-3.3.1/src/pybdsim/Obsolete/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.567121 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
--rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Event.py
--rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Model.py
--rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Plots.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Processed.py
--rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Root.py
--rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Run.py
--rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.3.1/src/pybdsim/Optics.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.3.1/src/pybdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)    76884 2023-04-26 21:11:06.000000 pybdsim-3.3.1/src/pybdsim/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.3.1/src/pybdsim/Run.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.567950 pybdsim-3.3.1/src/pybdsim/Testing/
--rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Testing/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.3.1/src/pybdsim/Testing/bdsimMadx.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.3.1/src/pybdsim/Testing/trackingTester.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.3.1/src/pybdsim/Visualisation.py
--rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.3.1/src/pybdsim/Writer.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.3.1/src/pybdsim/XSecBias.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3358 2023-04-26 09:53:42.000000 pybdsim-3.3.1/src/pybdsim/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.3.1/src/pybdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-05-15 09:10:48.000000 pybdsim-3.3.1/src/pybdsim/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.558661 pybdsim-3.3.1/src/pybdsim.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-05-15 09:10:48.000000 pybdsim-3.3.1/src/pybdsim.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-05-15 09:10:48.000000 pybdsim-3.3.1/src/pybdsim.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-05-15 09:10:48.000000 pybdsim-3.3.1/src/pybdsim.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.3.1/src/pybdsim.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)      335 2023-05-15 09:10:48.000000 pybdsim-3.3.1/src/pybdsim.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-05-15 09:10:48.000000 pybdsim-3.3.1/src/pybdsim.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.568175 pybdsim-3.3.1/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.3.1/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.569559 pybdsim-3.3.1/tests/test_input/
--rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.3.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
--rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.3.1/tests/test_input/model-model-aper.tfs.gz
--rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.3.1/tests/test_input/model-model-collsettings.dat
--rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.3.1/tests/test_input/model-model.tfs.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.569902 pybdsim-3.3.1/tests/test_output/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.3.1/tests/test_output/.gitkeep
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.570855 pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.571717 pybdsim-3.3.1/tests/test_output/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.534625 pybdsim-3.3.1/tests/test_output2/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.572468 pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.573321 pybdsim-3.3.1/tests/test_output2/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/test_output2/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.574064 pybdsim-3.3.1/tests/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.3.1/tests/tests/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/tests/pybdsim_test_utils.py
--rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.3.1/tests/tests/test_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.3.1/tests/tests/testratio.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.3.1/tests/tests/write_test_outputs.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-15 09:10:48.574198 pybdsim-3.3.1/tests/unit/
--rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.3.1/tests/unit/test_Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.277667 pybdsim-3.3.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.3.2/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.3.2/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.3.2/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.3.2/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-06-29 15:37:39.277772 pybdsim-3.3.2/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      936 2023-05-08 16:07:40.000000 pybdsim-3.3.2/README.md
+-rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.3.2/bitbucket-pipelines.yml
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.258870 pybdsim-3.3.2/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)  1200819 2023-06-29 15:29:59.000000 pybdsim-3.3.2/docs/pybdsim.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.261270 pybdsim-3.3.2/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      307 2023-05-08 16:07:51.000000 pybdsim-3.3.2/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.3.2/docs/source/builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.3.2/docs/source/classes.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.3.2/docs/source/compare.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-06-29 15:36:52.000000 pybdsim-3.3.2/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.3.2/docs/source/convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.3.2/docs/source/data.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.3.2/docs/source/data_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.3.2/docs/source/developer.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12893 2023-05-11 15:00:20.000000 pybdsim-3.3.2/docs/source/fieldmaps.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.262375 pybdsim-3.3.2/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/rebdsimFileHistograms.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/rebdsimFileHistogramsWrapped.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/rebdsimFileMembers.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/figures/simpleHistogramPlot.png
+-rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.3.2/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2198 2023-05-08 16:05:46.000000 pybdsim-3.3.2/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.3.2/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.3.2/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.3.2/docs/source/plotting.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.3.2/docs/source/support.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12803 2023-06-29 15:06:32.000000 pybdsim-3.3.2/docs/source/version_history.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.262586 pybdsim-3.3.2/examples/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.263111 pybdsim-3.3.2/examples/1_builder/
+-rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/1_builder/1_builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/1_builder/1_testmachine.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/1_builder/1_testmachine.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.265472 pybdsim-3.3.2/examples/2_convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/1_madxtfs2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/1_madxtfs2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/2_convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/2_transport2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/2_transport2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/transport_example.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/transport_example.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.tar.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.265608 pybdsim-3.3.2/examples/3_optics/
+-rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.3.2/examples/3_optics/optics_validation.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.265717 pybdsim-3.3.2/examples/4_uproot/
+-rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.3.2/examples/4_uproot/4_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.3.2/examples/examples.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1846 2023-05-15 09:07:01.000000 pybdsim-3.3.2/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      258 2023-06-29 15:37:39.278075 pybdsim-3.3.2/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.3.2/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.256625 pybdsim-3.3.2/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.267899 pybdsim-3.3.2/src/pybdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.3.2/src/pybdsim/Beam.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.3.2/src/pybdsim/Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.269635 pybdsim-3.3.2/src/pybdsim/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.3.2/src/pybdsim/Compare/_BdsimBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    10613 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_ElegantBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    14712 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    23099 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_MadxBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Compare/_MadxMadxComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48466 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Compare/_MultipleCodeComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Compare/_SadComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6438 2023-05-08 16:03:57.000000 pybdsim-3.3.2/src/pybdsim/Compare/_TransportBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      827 2023-05-08 16:04:54.000000 pybdsim-3.3.2/src/pybdsim/Compare/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.3.2/src/pybdsim/Constants.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.271161 pybdsim-3.3.2/src/pybdsim/Convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.3.2/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.3.2/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    24017 2023-06-29 15:27:24.000000 pybdsim-3.3.2/src/pybdsim/Convert/_CPyMad2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_ElegantParamToStrength.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Rebdsim2Numpy.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Convert/_SadFlat2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     4483 2023-05-08 16:02:45.000000 pybdsim-3.3.2/src/pybdsim/Convert/_Transport2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-05-08 15:59:37.000000 pybdsim-3.3.2/src/pybdsim/Convert/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Convert/collimator_analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    83880 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.3.2/src/pybdsim/DataUproot.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.271594 pybdsim-3.3.2/src/pybdsim/Field/
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Field/FieldPlotter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Field/FieldPlotterVtk.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    17734 2023-06-29 15:07:38.000000 pybdsim-3.3.2/src/pybdsim/Field/_Field.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.3.2/src/pybdsim/Field/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.3.2/src/pybdsim/Geant4.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.3.2/src/pybdsim/Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Joinhistograms.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.3.2/src/pybdsim/ModelProcessing.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.256898 pybdsim-3.3.2/src/pybdsim/Obsolete/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.272736 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Event.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Model.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Plots.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Processed.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Root.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Run.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.3.2/src/pybdsim/Optics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.3.2/src/pybdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    76876 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.3.2/src/pybdsim/Run.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.273072 pybdsim-3.3.2/src/pybdsim/Testing/
+-rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Testing/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.3.2/src/pybdsim/Testing/bdsimMadx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.3.2/src/pybdsim/Testing/trackingTester.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.3.2/src/pybdsim/Visualisation.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.3.2/src/pybdsim/Writer.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.3.2/src/pybdsim/XSecBias.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1586 2023-06-29 15:06:32.000000 pybdsim-3.3.2/src/pybdsim/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.3.2/src/pybdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.268517 pybdsim-3.3.2/src/pybdsim.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.3.2/src/pybdsim.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      335 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-06-29 15:37:39.000000 pybdsim-3.3.2/src/pybdsim.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.273175 pybdsim-3.3.2/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.3.2/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.274071 pybdsim-3.3.2/tests/test_input/
+-rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/model-model-aper.tfs.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/model-model-collsettings.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_input/model-model.tfs.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.274334 pybdsim-3.3.2/tests/test_output/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/test_output/.gitkeep
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.275157 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.275751 pybdsim-3.3.2/tests/test_output/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.257395 pybdsim-3.3.2/tests/test_output2/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.276328 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.276882 pybdsim-3.3.2/tests/test_output2/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/test_output2/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.277442 pybdsim-3.3.2/tests/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.3.2/tests/tests/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/tests/pybdsim_test_utils.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.3.2/tests/tests/test_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.3.2/tests/tests/testratio.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.3.2/tests/tests/write_test_outputs.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-06-29 15:37:39.277562 pybdsim-3.3.2/tests/unit/
+-rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.3.2/tests/unit/test_Builder.py
```

### Comparing `pybdsim-3.3.1/COPYING.txt` & `pybdsim-3.3.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/LICENSE.txt` & `pybdsim-3.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/Makefile` & `pybdsim-3.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/PKG-INFO` & `pybdsim-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.3.1
+Version: 3.3.2
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.3.1/README.md` & `pybdsim-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/bitbucket-pipelines.yml` & `pybdsim-3.3.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/Makefile` & `pybdsim-3.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/make.bat` & `pybdsim-3.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/pybdsim.pdf` & `pybdsim-3.3.2/docs/pybdsim.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 pybdsim Documentation
 Release 3.3.0
 
 Royal Holloway
 
-May 08, 2023
+Jun 29, 2023
 
 CONTENTS
 
 1
 
 Licence & Disclaimer
 
@@ -158,51 +158,55 @@
 12 Support
 12.1 Feature Request . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 47
 47
 
 13 Version History
-13.1 V3.3.0 - 2023 / 05 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.2 V3.2.0 - 2023 / 04 / 26 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.3 V3.1.1 - 2023 / 04 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.4 V3.1.0 - 2023 / 04 / 02 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.5 V3.0.1 - 2023 / 03 / 22 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.6 V3.0.0 - 2023 / 03 / 19 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.7 v2.4.0 - 2021 / 06 / 16 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.8 v2.3.0 - 2020 / 12 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.9 v2.2.0 - 2020 / 06 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.10 v2.1 - 2019 / 04 / 20 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.11 v2.0 - 2019 / 02 / 27 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.12 v1.9 - 2018 / 08 / 24 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.13 v1.8 - 2018 / 06 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.14 v1.7 - 2018 / 06 / 30 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.15 v1.6 - 2018 / 05 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.16 v1.5 - 2018 / 05 / 17 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.17 v1.4 - 2018 / 10 / 04 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.18 v1.3 - 2017 / 12 / 05 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.1 V3.3.2 - 2023 / 06 / 29 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.2 V3.3.1 - 2023 / 05 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.3 V3.3.0 - 2023 / 05 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.4 V3.2.0 - 2023 / 04 / 26 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.5 V3.1.1 - 2023 / 04 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.6 V3.1.0 - 2023 / 04 / 02 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.7 V3.0.1 - 2023 / 03 / 22 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.8 V3.0.0 - 2023 / 03 / 19 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.9 v2.4.0 - 2021 / 06 / 16 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.10 v2.3.0 - 2020 / 12 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.11 v2.2.0 - 2020 / 06 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.12 v2.1 - 2019 / 04 / 20 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.13 v2.0 - 2019 / 02 / 27 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.14 v1.9 - 2018 / 08 / 24 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.15 v1.8 - 2018 / 06 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.16 v1.7 - 2018 / 06 / 30 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.17 v1.6 - 2018 / 05 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.18 v1.5 - 2018 / 05 / 17 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.19 v1.4 - 2018 / 10 / 04 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.20 v1.3 - 2017 / 12 / 05 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 49
 49
 49
 49
+49
+50
 50
 50
 50
 51
 52
 52
 52
-52
 53
 53
 54
 54
 54
 55
+55
 56
 
 14 Module Contents
 14.1 pybdsim.Beam module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.2 pybdsim.Builder module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.3 pybdsim.Compare . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.4 pybdsim.Constants module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -212,36 +216,35 @@
 14.8 pybdsim.Gmad module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.9 pybdsim.ModelProcessing module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.10 pybdsim.Options module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.11 pybdsim.Plot module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.12 pybdsim.Run module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.13 pybdsim.Visualisation module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.14 pybdsim.Writer module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-14.15 pybdsim.XSecBias module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 57
 57
 58
 67
 68
 68
 73
 80
-85
-87
+86
 88
-90
-95
+88
+91
 96
 97
-99
+97
 
 ii
 
-15 Developer Documentation
+14.15 pybdsim.XSecBias module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 100
+15 Developer Documentation
 101
 15.1 Release Checklist . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
 16 Indices and tables
 
 103
 
 Python Module Index
@@ -1376,15 +1379,15 @@
 • pybdsim.Field.Field4D
 These all have member variables such as:
 • data - the numpy array of the field map data
 • columns - a list of column names
 • header - a dictionary of all information in the header
 
 10.2 Writing
-Al of the pybdsim classes described in Loading (e.g. Field3D) have a method called Write. This will write out
+All of the pybdsim classes described in Loading (e.g. Field3D) have a method called Write. This will write out
 the instance of that class (i.e. that particular field map data) to a BDSIM-format field map file.
 Therefore, these classes represent a a very good route for creation and conversion of field maps. The recommended
 strategy is to get the information into one of those classes then it can be written out to file, loaded, plotted with
 ease.
 
 39
 
@@ -1477,15 +1480,15 @@
 data.append(v)
 # convert to numpy array
 data = np.array(data)
 # construct a BDSIM format field object and write it out
 # this will be written out in the BDSIM conventional looping order
 f = pybdsim.Field.Field2D(data, flip=True)
 f.Write("box-field-map.dat')
-Below is a script included with bdsim (bdsim/examples/features/maps_bdsim/Generate2DLoopOrder.
+Below is a script included with BDSIM (bdsim/examples/features/maps_bdsim/Generate2DLoopOrder.
 py) that shows 4 ways to write a field map with the same information. Ultimately, they convey the exact same field
 map to BDSIM although the file contents differ (2 sets of possible contents).
 
 10.3. Creation
 
 41
 
@@ -1541,15 +1544,15 @@
 
 10.4 Visualisation and Plotting
 To visualise a field map, it is possible to do so in BDSIM / Geant4. See the BDSIM manual for this information.
 This draws a selection of arrows in the 3D model and gives a rough indication that the field map is as intended.
 An alternative way is to load the data in pybdsim in Python and plot it, either fully or in slices (for 3D or 4D maps).
 Any library desired can be used in Python and the classes described above in Loading provide an excellent way to
 get a numpy array, that is ubiquitous in Python programming and libraries.
-pybdsim provides a variety of small plotting functions mostly for 1D and 2D field maps using Matplotlib. These
+pybdsim provides a variety of small plotting functions mostly for 1D and 2D field maps using matplotlib. These
 functions are inside the pybdsim.Field module and all start with Plot. A list is:
 • pybdsim.Field.Plot1DFxFyFz
 • pybdsim.Field.Plot2D
 • pybdsim.Field.Plot2DXY
 • pybdsim.Field.Plot2DXYMagnitude
 • pybdsim.Field.Plot2DXYConnectionOrder
 • pybdsim.Field.Plot2DXYStream
@@ -1716,281 +1719,290 @@
 
 CHAPTER
 
 THIRTEEN
 
 VERSION HISTORY
 
-13.1 V3.3.0 - 2023 / 05 / 08
+13.1 V3.3.2 - 2023 / 06 / 29
+• Fix loading of new header variables with backwards compatibility.
+• Fix extra new lines and white space being written out in comments at the top of field maps.
+• New function to write a 3D scoring mesh out as ASCII for transfer to other programs.
+• Explicit exception when the ROOT libraries can’t be loaded for reading BDSIM data.
+• Fix circular import from Data.py and _General.py.
+
+13.2 V3.3.1 - 2023 / 05 / 15
+• Reduce Python version requirement to >3.6 instead of 3.7.
+
+13.3 V3.3.0 - 2023 / 05 / 08
 • Fix installation where there was a missing dependency of pandas with pymad8. pymad8 is now no longer a
 formal dependency but all the conversion and comparison code still exists.
 • Fix setup.cfg having pymadx in the name although it makes no difference.
 • Add new pybdsim.Data.GetHistoryPDGTuple() function to aid trajectory analysis.
 
-13.2 V3.2.0 - 2023 / 04 / 26
+13.4 V3.2.0 - 2023 / 04 / 26
 • Remove the function pybdsim.Plot.AddMachineLatticeToFigure(). This was just a forward to
 pymadx.Plot.AddMachineLatticeToFigure() and this should be used explicitly for machine diagram
 plotting for TFS files. Otherwise, pybdsim.Plot.AddMachineLatticeFromSurveyToFigure should be
 used.
 • Better documentation about plotting.
 • Increase the visibility of light grey elements in the machine diagram from alpha 0.1 to 0.4.
 
-13.3 V3.1.1 - 2023 / 04 / 23
+49
+
+pybdsim Documentation, Release 3.3.0
+
+13.5 V3.1.1 - 2023 / 04 / 23
 • Fixed spectra loading and plotting for when the ‘p’ and ‘s’ prefixes are used in the rebdsim Spectra command
 to denote primary and secondary particles.
 • Fixed error with default log scale in Plot.Histogram2D when no vmin was specified.
 • Fix pybdsim._version_tuple which should be pybdsim.__version_tuple__.
 • Fix import without awkward array which is only required for the [uproot] feature of pybdsim.
 • pybdsim.Plot.Spectra() now makes more than one plot if more than 8 particles are specified.
 • Recognised PDG ID 0 as “total” from BDSIM.
 
-49
-
-pybdsim Documentation, Release 3.3.0
-
-13.4 V3.1.0 - 2023 / 04 / 02
+13.6 V3.1.0 - 2023 / 04 / 02
 • Add the writing and reading of comment lines in field maps.
 • Reduce print out when loading a field map.
 • Clean imports in cpymad interface as well as in Convert functions.
 
-13.5 V3.0.1 - 2023 / 03 / 22
+13.7 V3.0.1 - 2023 / 03 / 22
 • Fix import for pybdsim when ROOT is present but librebdsim etc. are not available through environmental
 variables, or findable. Would cause induce a classic ROOT segfault when importing pybdsim.
 • Fix wrong exception being raised.
 • Always write a comment string at the start of a BDSIM field map file to specify the units of the file.
 
-13.6 V3.0.0 - 2023 / 03 / 19
+13.8 V3.0.0 - 2023 / 03 / 19
 • Restructure package into a declarative Python package where all source files are now in src/pybdsim/.
 • The package now has a feature called uproot for the optional dependencies of uproot, pandas, and pint
 packages.
 • Field classes no longer have flip=True as the default - it is now False. Please check any field maps created
 by scripts using these classes.
 
-13.6.1 New Features
+13.8.1 New Features
 • Add a module to load BDSIM output file, included rebdsim files with uproot.
 • Create a nice Python copy of the header information from any (re)bdsim file when loading with pybdsim
 using only Python types.
 • New integration for 2D histograms along each axis to 1D histograms.
 • New slices for 3D histograms as well as integrating along a dimension (‘projection’). See 3D Scoring Histograms.
 • New ratio plot for 2x 1D histograms. See pybdsim.Plot.Histogram1DRatio.
 • New loading and handling of 4D histograms (from BDSIM with Boost). They can now be loaded and handled
 similarly to 1,2,3D histograms. They are loaded automatically when loading a rebdsim file.
+
+50
+
+Chapter 13. Version History
+
+pybdsim Documentation, Release 3.3.0
+
 • pybdsim.Data.TH1,2,3 now have xrange, yrange, and zrange members where appropriate with a convenient tuple of the range in each dimension. They also have the member integral and integralError
 taken from their ROOT objects.
 • Field plotting functions now tolerate Field class objects as well as filenames to make it easier to check field
 objects as you’re making them.
 • New field plotting for 2D field maps showing each component.
 • New field reflection utility function pybdsim.Field.MirrorDipoleQuadrant1 for 2D fields.
 • New field plotting function pybdsim.Field.Plot2DXYConnectionOrder to see the order an array is written in.
 This can be used to validate any field manipulations.
 • New field plotting function pybdsim.Field.Plot1DFxFyFz to see field components in 1D.
 • Field loading automatically works for dimensions such as X, Z for 2D instead of X, Y now.
-
-50
-
-Chapter 13. Version History
-
-pybdsim Documentation, Release 3.3.0
-
 • Ability to load a rebdsim output file and only load the ROOT histograms without loading the BDSIM and
 rebdsim shared libraries, so it can be used on a separate computer with just ROOT.
 • Added classes to Builder for all GMAD objects. New ones include aperture, atom, blm, cavitymodel, crystal,
 field, material, newcolour, query, region, samplerplacement, scorer, tunnel, xsecbias.
 
-13.6.2 Bug Fixes
+13.8.2 Bug Fixes
 • pybdsim would throw an exception that librebdsim and libbdsimRootEvent could not be loaded and stop if the
 libraries had been already loaded separately outside pybdsim. This has been fixed by fixing the interpretation
 of the error codes from ROOT.
 • Fix warning about “nonposy” in matplotlib version for log scales.
 • Fix check in Run of if it’s a ROOT file or not. Simplify it to use file extension.
 • Tolerate no pytransport installation.
 • Fix loading of aperture data from a BDSIM output file.
 • Fix loading of model data.
 • Fix aperture plots from a BDSIM output file.
 
-13.6.3 General
+13.8.3 General
 • The Beam class now takes distrType and not distrtype so as to match BDSIM syntax and be less confusing.
 • Updated out of date documentation.
 • Better automatic ranges for Histogram1DMultiple plots by default.
 • Better field loading in pybdsim.Field.Load. Returns the same Field object from pybdsim as you would write.
 
-13.7 v2.4.0 - 2021 / 06 / 16
-13.7.1 New Features
+13.9 v2.4.0 - 2021 / 06 / 16
+13.9.1 New Features
 • Transform3D function in a Machine.
 • Crystal, ScorerMesh and Placement also can be added to a Machine.
 • Ability to insert and replace an element in a machine.
 
-13.7.2 Bug Fixes
-• Python 3.8+ warnings fixed.
-• Add ROOT_INCLUDE_PATH to ROOT as newer versions don’t do this automatically.
-• Fixed vmin for 2D histogram plot.
-
-13.7. v2.4.0 - 2021 / 06 / 16
+13.9. v2.4.0 - 2021 / 06 / 16
 
 51
 
 pybdsim Documentation, Release 3.3.0
 
-13.8 v2.3.0 - 2020 / 12 / 15
-13.8.1 New Features
+13.9.2 Bug Fixes
+• Python 3.8+ warnings fixed.
+• Add ROOT_INCLUDE_PATH to ROOT as newer versions don’t do this automatically.
+• Fixed vmin for 2D histogram plot.
+
+13.10 v2.3.0 - 2020 / 12 / 15
+13.10.1 New Features
 • Convenience functions for pickling and un-pickling data in the Data module with optional compression.
 • Generic loss map plot.
 
-13.9 v2.2.0 - 2020 / 06 / 08
-13.9.1 New Features
+13.11 v2.2.0 - 2020 / 06 / 08
+13.11.1 New Features
 • Support for Python3.
 
-13.10 v2.1 - 2019 / 04 / 20
-13.10.1 New Featuers
+13.12 v2.1 - 2019 / 04 / 20
+13.12.1 New Featuers
 • Optional flag of whether to write out the converted model with pybdsim.Convert.MadxTfs2Gmad.
 • Machine builder now supports new bdsim jcol element.
 • Machine diagram drawing can now start from any arbitrary S location.
 • For loaded histograms (using pybdsim.Data.TH1, TH2, TH3 classes, there are now functions ErrorsToSTD()
 and ErrorsToErrorOnMean() to easily convert between the different types of error - the default is error on
 the mean.
 • New plotting function pybdsim.Plot.Histogram2DErrors to visualise 2D histogram errors.
 
-13.10.2 General
+13.12.2 General
 • Return arguments of pybdsim.Convert.MadxTfs2Gmad is now just 2 items - machine and omitted items.
 Previously 3.
 
-13.10.3 Bug Fixes
+13.12.3 Bug Fixes
 • Fix loading of Model tree from ROOT output given some recent collimation variables may have a different
 structure or type from the existing ones.
 • In pybdsim.Plot.Histogram2D, the y log scale argument was “ylocscale” and is fixed to “yLogScale”.
 
-13.11 v2.0 - 2019 / 02 / 27
-13.11.1 New Features
-• Machine diagram plotting automatically from BDSIM output. Compatible with newer BDSIM output format.
-• Support for thin R matrix, parallel transporter and thick R matrix in builder.
-• Generate transfer matrix from tracking data from BDSIM for a single element.
-• Control over legend location in standard energy deposition and loss plots.
 52
 
 Chapter 13. Version History
 
 pybdsim Documentation, Release 3.3.0
 
+13.13 v2.0 - 2019 / 02 / 27
+13.13.1 New Features
+• Machine diagram plotting automatically from BDSIM output. Compatible with newer BDSIM output format.
+• Support for thin R matrix, parallel transporter and thick R matrix in builder.
+• Generate transfer matrix from tracking data from BDSIM for a single element.
+• Control over legend location in standard energy deposition and loss plots.
 • Utility function to write sampler data from BDSIM output to a user input file.
 • Support for energy variation in the beam line in MAD8 conversion.
 
-13.11.2 General
+13.13.2 General
 • Remove dependency of root_numpy. pybdsim now uses only standard ROOT interfaces.
 • Update physics lists.
 
-13.11.3 Bug Fixes
+13.13.3 Bug Fixes
 • Fix bug where calling pybdsim.Plot.PrimaryPhaseSpace with an output file name would result in an error as
 this argument was wrongly supplied to the number of bins argument.
 • Fix for hidden scientific notation when using machine diagram.
 • Fix TH1 TH2 TH3 histogram x,y,z highedge variables in histogram loading. These were the lowedge duplicated, which was wrong.
 • Add missing variables from sampler data given changes in BDSIM.
 
-13.12 v1.9 - 2018 / 08 / 24
-13.12.1 General
+13.14 v1.9 - 2018 / 08 / 24
+13.14.1 General
 • Significant new tests.
 • Trajectory loading from BDSIM ROOT output.
 • Plot trajectories.
 • New padding function for 1D histogram to ensure lines in plots.
 • New value replacement function for histograms to ensure continuous line in log plots.
 • Control over aspect ration in default 2D histogram plots.
 • New classes for each element in the Builder.
 • Refactor of MadxTfs2Gmad to use new classes in Builder.
 
-13.12.2 Bug Fixes
+13.13. v2.0 - 2019 / 02 / 27
+
+53
+
+pybdsim Documentation, Release 3.3.0
+
+13.14.2 Bug Fixes
 • Fix orientation of 2D histograms in plotting.
 • Fix header information labels when writing field maps with reversed order.
 
-13.13 v1.8 - 2018 / 06 / 23
-13.13.1 General
+13.15 v1.8 - 2018 / 06 / 23
+13.15.1 General
 • Setup requires pytest-runner.
 • Introduction of testing.
 • Removed line wrapping written to GMAD files in Builder.
 • “PlotBdsimOptics” is now “BDSIMOptics” in the Plot module.
-
-13.12. v1.9 - 2018 / 08 / 24
-
-53
-
-pybdsim Documentation, Release 3.3.0
-
 • New comparison plots for arbitrary inputs from different tracking codes.
 • Prepare PTC coordinates from any BDSIM sampler.
 
-13.13.2 Bug Fixes
+13.15.2 Bug Fixes
 • Fixes for “Optics” vs “optics” naming change in ROOT files.
 
-13.14 v1.7 - 2018 / 06 / 30
-13.14.1 General
+13.16 v1.7 - 2018 / 06 / 30
+13.16.1 General
 • Can specify which dimension in Field class construction (i.e. ‘x’:’z’ instead of default ‘x’:’y’).
 
-13.14.2 Bug Fixes
+13.16.2 Bug Fixes
 • ‘nx’ and ‘ny’ were written the wrong way around from a 2D field map in pybdsim.
 
-13.15 v1.6 - 2018 / 05 / 23
-13.15.1 Bug Fixes
+13.17 v1.6 - 2018 / 05 / 23
+13.17.1 Bug Fixes
 • Fix machine diagram plotting from BDSIM survey.
 • Fix machine diagram searching with right-click in plots.
 
-13.16 v1.5 - 2018 / 05 / 17
-13.16.1 New Features
+54
+
+Chapter 13. Version History
+
+pybdsim Documentation, Release 3.3.0
+
+13.18 v1.5 - 2018 / 05 / 17
+13.18.1 New Features
 • Function now public to create beam from Madx TFS file.
 • Improved searching for BDSAsciiData class.
 • Ability to easily write out beam class.
 • Plot phase space from any sampler in a BDSIM output file.
 • __version__ information in package.
 • Get a column from data irrespective of case.
 • Coded energy deposition plot. Use for example for labelling cyrogenic, warm and collimator losses.
 • Improved Transport BDSIM comparison.
 • Function to convert a line from a TFS file into a beam definition file.
 
-54
-
-Chapter 13. Version History
-
-pybdsim Documentation, Release 3.3.0
-
-13.16.2 Bug Fixes
+13.18.2 Bug Fixes
 • Fix library loading given changes to capitalisation in BDSIM.
 • Beam class now supports all BDSIM beam definitions.
 • Support all aperture shapes in Builder.
 • Fixes for loading optics given changes to capitalisation and BDSAsciiData class usage.
 • Fixes for collimator conversion from MADX.
 
-13.17 v1.4 - 2018 / 10 / 04
-13.17.1 New Features
+13.19 v1.4 - 2018 / 10 / 04
+13.19.1 New Features
 • Full support for loading BDSIM output formats through ROOT.
 • Extraction of data from ROOT histograms to numpy arrays.
 • Simple histogram plotting from ROOT files.
 • Loading of sampler data and simple extraction of phase space data.
 • Line wrapping for elements with very long definitions.
 • Comparison plots standardised.
 • New BDSIM BDSIM comparison.
 • New BDSIM Mad8 comparison.
 • Support for changes to BDSIM data format variable renaming in V1.0
 
-13.17.2 Bug Fixes
+13.18. v1.5 - 2018 / 05 / 17
+
+55
+
+pybdsim Documentation, Release 3.3.0
+
+13.19.2 Bug Fixes
 • Correct conversion of all dispersion component for Beam.
 • Don’t write all multipole components if not needed.
 • Fixed histogram plotting.
 • Fixed conversion of coordinates in BDSIM2PtcInrays for subrelativistic particles.
 • Fixed behaviour of fringe field fint and fintx behaviour from MADX.
 • Fixed pole face angles given MADX writes out wrong angles.
 • Fixed conversion of multipoles and other components for ‘linear’ flag in MadxTfs2Gmad.
 • Fixed axis labels in field map plotting utilities.
 • MADX BDSIM testing suite now works with subrelativistic particles.
 • Many small fixes to conversion.
 
-13.17. v1.4 - 2018 / 10 / 04
-
-55
-
-pybdsim Documentation, Release 3.3.0
-
-13.18 v1.3 - 2017 / 12 / 05
-13.18.1 New Features
+13.20 v1.3 - 2017 / 12 / 05
+13.20.1 New Features
 • GPL3 licence introduced.
 • Compatibility with PIP install system.
 • Manual.
 • Testing suite.
 
 56
 
@@ -2869,42 +2881,45 @@
 standard deviation. Will automatically only apply itself once even if repeatedly called.
 class pybdsim.Data.BeamData(data)
 Bases: object
 classmethod FromROOTFile(path)
 class pybdsim.Data.CavityInfo(rootInstance=None)
 Bases: object
 Simple class to represent a cavity info instance. Construct from a root instance of the class.
+pybdsim.Data.CheckBdsimDataHasSurveyModel(bfile)
+pybdsim.Data.CheckItsBDSAsciiData(bfile, requireOptics=False)
 class pybdsim.Data.CollimatorInfo(rootInstance=None)
 Bases: object
 Simple class to represent a collimator info instance. Construct from a root instance of the class.
 pybdsim.Data.CreateEmptyRebdsimFile(outputfilename, nOriginalEvents=1)
 Create an empty rebdsim format file with the layout of folders. Returns the ROOT.TFile object.
 class pybdsim.Data.EventInfoData(data)
 Bases: object
 Extract data from the Info branch of the Event tree.
 classmethod FromROOTFile(path)
 class pybdsim.Data.EventSummaryData(data)
 Bases: EventInfoData
 Extract data from the Summary branch of the Event tree.
 pybdsim.Data.GetApertureExtent(apertureType, aper1=0, aper2=0, aper3=0, aper4=0)
+pybdsim.Data.GetFileName(ob)
 pybdsim.Data.GetHistoryPDGTuple(trajectories, startingTrajectoryStorageIndex, reduceDuplicates=False)
 Return a tuple of PDG IDs for the history of a particle given by trajectories in an event.
 Parameters
 • trajectories (event.Trajectory) – event.Trajectory instance from loaded ROOT
 data
 • startingTrajectoryStorageIndex (int) – storage index of which trajectory to start
 from
-• reduceDuplicates (bool) – whether to remove sequential duplicates from the history
 
 74
 
 Chapter 14. Module Contents
 
 pybdsim Documentation, Release 3.3.0
 
+• reduceDuplicates (bool) – whether to remove sequential duplicates from the history
 >>> d = pybdsim.Data.Load("somdbdsimoutputfile.root")
 >>> et = d.GetEventTree()
 >>> for event in et:
 tid = event.sampler1.trackID[0]
 history = pybdsim.Data.GetHistoryPDGTuple(event.Trajectory, tid)
 print(history)
 An example might be (13,211,211,2212) or with reducedDuplicates (31,211,2212)
@@ -2944,14 +2959,16 @@
 
 14.6. pybdsim.Data module
 
 75
 
 pybdsim Documentation, Release 3.3.0
 
+pybdsim.Data.IsSurvey(file)
+Checks if input is a BDSIM generated survey
 pybdsim.Data.Load(filepath)
 Load the data with the appropriate loader.
 ASCII file - returns BDSAsciiData instance. BDSIM file - uses ROOT, returns BDSIM DataLoader instance.
 REBDSIM file - uses ROOT, returns RebdsimFile instance.
 pybdsim.Data.LoadPickledObject(filename)
 Unpickle an object. If the name contains .pbz2 the bz2 library will be used as well to load the compressed
 pickled object.
@@ -2982,25 +2999,25 @@
 pybdsim.Data.ParseSpectraName(hname)
 class pybdsim.Data.PhaseSpaceData(data, samplerIndexOrName=0)
 Bases: _SamplerData
 Pull phase space data from a loaded DataLoader instance of raw data for all events.
 Extracts only: ‘x’,’xp’,’y’,’yp’,’z’,’zp’,’energy’,’T’
 Can either supply the sampler name or index as the optional second argument. The index is 0 counting
 including the primaries (ie +1 on the index in data.GetSamplerNames()). Examples:
->>> f = pybdsim.Data.Load("file.root")
->>> primaries = pybdsim.Data.PhaseSpaceData(f)
->>> samplerfd45 = pybdsim.Data.PhaseSpaceData(f, "samplerfd45")
->>> thirdAfterPrimaries = pybdsim.Data.PhaseSpaceData(f, 3)
 
 76
 
 Chapter 14. Module Contents
 
 pybdsim Documentation, Release 3.3.0
 
+>>> f = pybdsim.Data.Load("file.root")
+>>> primaries = pybdsim.Data.PhaseSpaceData(f)
+>>> samplerfd45 = pybdsim.Data.PhaseSpaceData(f, "samplerfd45")
+>>> thirdAfterPrimaries = pybdsim.Data.PhaseSpaceData(f, 3)
 pybdsim.Data.PickleObject(ob, filename, compress=True)
 Write an object to a pickled file using Python pickle.
 If compress is True, the bz2 package will be imported and used to compress the file.
 class pybdsim.Data.ROOTHist(hist)
 Bases: object
 Base class for histogram wrappers.
 ErrorsToErrorOnMean()
@@ -3029,27 +3046,27 @@
 GetModelTree()
 ListOfDirectories()
 List all directories inside the root file.
 ListOfLeavesInTree(tree)
 List all leaves in a tree.
 ListOfTrees()
 List all trees inside the root file.
-pybdsim.Data.ReplaceZeroWithMinimum(hist, value=1e-20)
-Replace zero values with given value. Useful for log plots.
-For log plots we want a small but +ve number instead of 0 so the line is continuous on the plot. This is also
-required for padding to work for the edge of the lines.
-Works for TH1, TH2, TH3.
-returns a new instance of the pybdsim.Data.TH1, TH2 or TH3.
 
 14.6. pybdsim.Data module
 
 77
 
 pybdsim Documentation, Release 3.3.0
 
+pybdsim.Data.ReplaceZeroWithMinimum(hist, value=1e-20)
+Replace zero values with given value. Useful for log plots.
+For log plots we want a small but +ve number instead of 0 so the line is continuous on the plot. This is also
+required for padding to work for the edge of the lines.
+Works for TH1, TH2, TH3.
+returns a new instance of the pybdsim.Data.TH1, TH2 or TH3.
 pybdsim.Data.SDDSBuildParameterDicts(sddsColumnDict)
 Use first the LoadSDDSColumnsToDict on a parameters file. Then call this function to sort it into ElementName : {ParameterName:ParameterValue}. An extra key will be added that is KEYWORD for the
 ElementType in the inner dictionary.
 class pybdsim.Data.SamplerData(data, samplerIndexOrName=0)
 Bases: _SamplerData
 Pull sampler data from a loaded DataLoader instance of raw data for all events.
 Loads all data in a given sampler.
@@ -3076,26 +3093,26 @@
 IntegrateAlongX()
 Integrate along the x axis returning a TH1 in y.
 IntegrateAlongY()
 Integrate along the y axis returning a TH1 in x.
 Rebin(nBinsX, nBinsY=None)
 SwapAxes()
 Swap X and Y for all members. Returns a new copy of the histogram.
-class pybdsim.Data.TH3(hist, extractData=True)
-Bases: TH2
-Wrapper for a ROOT TH3 instance. Converts to numpy data.
->>> h = file.Get("histogramName")
->>> hpy = TH3(h)
 
 78
 
 Chapter 14. Module Contents
 
 pybdsim Documentation, Release 3.3.0
 
+class pybdsim.Data.TH3(hist, extractData=True)
+Bases: TH2
+Wrapper for a ROOT TH3 instance. Converts to numpy data.
+>>> h = file.Get("histogramName")
+>>> hpy = TH3(h)
 IntegateAlong1Dimension(dimension)
 Integrate along a dimension returning a new 2D histogram.
 Parameters
 dimension (str) – ‘x’, ‘y’ or ‘z’ dimension to integrate along
 returns pybdsim.Data.TH2 instance.
 If the projection is done in z, a 2D histogram of x,y is returned that is the sum of the bins along z. The
 errors are also calculated.
@@ -3113,35 +3130,44 @@
 Extract a single 2D histogram from an index along the Y dimension.
 Parameters
 index (int) – index in y array of bins to extract, e.g. 0 -> nbinsy-1
 Slice2DZY(index)
 Extract a single 2D histogram from an index along the X dimension.
 Parameters
 index (int) – index in x array of bins to extract, e.g. 0 -> nbinsx-1
+WriteASCII(filename, scalingFactor=1.0, comments=None)
+Write the contents to a text file. Optionally multiply contents by a numerical factor.
+Parameters
+• filename (str) – output name to write to - can optionally include .dat suffix.
+• scalingFactor (float) – numerical factor to multiply all contents by on writing out
+only.
+• comments (list(str)) – list of comments to be written at the top of the file.
 pybdsim.Data.TRotationToAxisAngle(trot)
 This will return a list of [Ax,Ay,Az,angle] from a ROOT.TRotation.
 If not imported, it will return [0,0,0,0]
+
+14.6. pybdsim.Data module
+
+79
+
+pybdsim Documentation, Release 3.3.0
+
 class pybdsim.Data.TrajectoryData(dataLoader, eventNumber=0)
 Bases: object
 Pull trajectory data from a loaded Dataloader instance of raw data
 Loads all trajectory data in a event event
 >>> f = pybdsim.Data.Load("file.root")
 >>> trajectories = pybdsim.Data.TrajectoryData(f,0)
 next()
 pybdsim.Data.WriteROOTHistogramsToDirectory(tfile, directoryName, histograms)
 Parameters
 • tfile (ROOT.TFile.) – TFile object to write to.
 • directoryName (str (e.g. "Event/PerEntryHistograms" )) – Full path of directory you wish to write the histograms to.
 • histograms ([ROOT.TH1,..]) – List of ROOT histograms to write.
 Write a list of histograms (ROOT.TH*) to a directory (str) in a ROOT.TFile instance.
-14.6. pybdsim.Data module
-
-79
-
-pybdsim Documentation, Release 3.3.0
 
 14.7 pybdsim.Field module
 Utilities to convert and prepare field maps.
 Most of the plots assume magnetic fields for the labels, but they work equally well for electric fields.
 class pybdsim.Field._Field.Field(array=array([], dtype=float64), columns=[], flip=False,
 doublePrecision=False)
 Bases: object
@@ -3156,14 +3182,21 @@
 order.
 gzip - if the file ends with “.gz” the file will be compressed automatically.
 For overrideLoopOrder it should be only ‘xyzt’ or ‘tzyx’. This option is provided in case a field is
 prepared in the other order somehow and you want to control the writing of this header variable independently.
 WriteFLUKA2DFormat1(fileName)
 Write one of the FLUKA formats (x,y,Bx,by) in cm,T with no header.
 Very simple and only works for Field2D - can be improved.
+
+80
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 class pybdsim.Field._Field.Field1D(data, doublePrecision=False, column='X')
 Bases: Field
 Utility class to write a 1D field map array to BDSIM field format.
 The array supplied should be 2 dimensional. Dimensions are: (x,value) where value has 4 elements
 [x,fx,fy,fz]. So a 120 long array would have np.shape of (120,4).
 This can be used for both electric and magnetic fields.
 Example:
@@ -3174,21 +3207,14 @@
 Bases: Field
 Utility class to write a 2D field map array to BDSIM field format.
 The array supplied should be 3 dimensional. Dimensions are: (x,y,value) where value has 5 elements
 [x,y,fx,fy,fz]. So a 100x50 (x,y) grid would have np.shape of (100,50,5).
 Example:
 >>> a = Field2D(data) # data is a prepared array
 >>> a.Write('outputFileName.dat')
-
-80
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 The ‘flip’ boolean allows an array with (y,x,value) dimension order to be written as (x,y,value). Values must
 still be (x,y,fx,fy,fz).
 The ‘doublePrecision’ boolean controls whether the field and spatial values are written to 16 s.f. (True) or 8
 s.f. (False - default).
 class pybdsim.Field._Field.Field3D(data, flip=False, doublePrecision=False, firstColumn='X',
 secondColumn='Y', thirdColumn='Z')
 Bases: Field
@@ -3204,14 +3230,21 @@
 s.f. (False - default).
 class pybdsim.Field._Field.Field4D(data, flip=False, doublePrecision=False)
 Bases: Field
 Utility class to write a 4D field map array to BDSIM field format.
 The array supplied should be 5 dimensional. Dimensions are: (t,y,z,x,value) where value has 7 elements
 [x,y,z,t,fx,fy,fz]. So a 100x50x30x10 (x,y,z,t) grid would have np.shape of (10,30,50,100,7).
 Example:
+
+14.7. pybdsim.Field module
+
+81
+
+pybdsim Documentation, Release 3.3.0
+
 >>> a = Field4D(data) # data is a prepared array
 >>> a.Write('outputFileName.dat')
 The ‘flip’ boolean allows an array with (t,z,y,x,value) dimension order to be written as (x,y,z,t,value). Values
 must still be (x,y,fx,fy,fz).
 The ‘doublePrecision’ boolean controls whether the field and spatial values are written to 16 s.f. (True) or 8
 s.f. (False - default).
 pybdsim.Field._Field.Load(filename, debug=False)
@@ -3226,21 +3259,14 @@
 3
 
 1
 4
 
 Parameters
 field2D (pybdsim.Field._Field.Field2D instance) – field object
-
-14.7. pybdsim.Field module
-
-81
-
-pybdsim Documentation, Release 3.3.0
-
 returns an instance of the same type.
 For a 2D field (i.e. function of x,y but can include Bx,By,Bz), for the quadrant number 1, mirror it and
 generate a bigger field for all four quadrants.
 1. original data
 2. data mirrored in x, (x,Bx) *= -1
 3. data mirrored in x,y, (x,y,By) *= -1
 4. data mirrored in y, (y,Bx) *= -1
@@ -3256,14 +3282,21 @@
 class pybdsim.Field.FieldPlotter.OneDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 pybdsim.Field.FieldPlotter.Plot1DFxFyFz(filename)
 Plot a bdsim 1D field map file.
 Parameters
 filename (str, pybdsim.Field._Field.Field1D instance) – name of the field map
 file or object
+
+82
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Field.FieldPlotter.Plot2D(filename, scale=None, title=None, flipX=False, flipY=False,
 firstDimension='X', secondDimension='Y', aspect='equal')
 Plot a bdsim field map file using any two planes. The corresponding field components are plotted (e.g. X:Z
 -> Fx:Fz).
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
@@ -3277,20 +3310,14 @@
 pybdsim.Field.FieldPlotter.Plot2DXY(filename, scale=None, title=None, flipX=False,
 firstDimension='X', secondDimension='Y', aspect='equal',
 figsize=(6, 5))
 Plot a bdsim field map file using the X,Y plane.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
-82
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 • scale (float) – numerical scaling for quiver plot arrow lengths.
 • title (str) – title for plot
 • flipX (bool) – whether to plot x backwards to match the right hand coordinate system
 of Geant4.
 • firstDimension (str) – Label of first dimension, e.g. “X”
 • secondDimension (str) – Label of second dimension, e.g. “Z”
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
@@ -3305,14 +3332,21 @@
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYBy(filename, scale=None, title=None, flipX=False,
 aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
+
+14.7. pybdsim.Field module
+
+83
+
+pybdsim Documentation, Release 3.3.0
+
 • scale (float) – numerical scaling for quiver plot arrow lengths.
 • title (str) – title for plot
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYBz(filename, scale=None, title=None, flipX=False,
 aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
@@ -3325,28 +3359,21 @@
 title=None, flipX=False, aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
 • componentIndex (int) – index of field component (0,1,2) for Fx, Fy, Fz
 • scale (float) – numerical scaling for quiver plot arrow lengths.
-
-14.7. pybdsim.Field module
-
-83
-
-pybdsim Documentation, Release 3.3.0
-
 • title (str) – title for plot
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYConnectionOrder(filename)
-Plot a point in orange and a line in blue (default matplotlib colours) for each locationin the field map. If the
+Plot a point in orange and a line in blue (default matplotlib colours) for each location in the field map. If the
 field map is constructed correctly, this should show a set of lines with diagonals between them. The other
 plots with the arrows are independent of order unlike when BDSIM loads the fields. So you might see an
-OK field map, but it could be wrong if hand written.
+OK field map, but it could be wrong if handwritten.
 pybdsim.Field.FieldPlotter.Plot2DXYFxFyFz(filename, title=None, aspect='auto', extent=None,
 **imshowKwargs)
 Plot Fx,Fy,Fz components of a field separately as a function of X,Y.
 Parameters
 • filename (str, pybdsim.Field._Field.Field1D instance) – name of field
 map file or object
 • title (None, str) – optional title for plot
@@ -3356,14 +3383,20 @@
 firstDimension='X', secondDimension='Y',
 aspect='equal', zlabel='|$B_{x,y}$| (T)', figsize=(6,
 5))
 Plot a the magnitude of a 2D bdsim field map file using any two planes.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
+84
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 • title (str, None) – title for plot
 • flipX (bool) – whether to plot x backwards to match the right hand coordinate system
 of Geant4.
 • firstDimension (str) – Name of first dimension, e.g. “X”
 • secondDimension (str) – Name of second dimension, e.g. “Z”
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 • zlabel (str) – Label for colour bar
@@ -3374,21 +3407,14 @@
 • filename (str, pybdsim.Field._Field.Field2D or Field3D instance) –
 name of field map file or object
 • density (float) – arrow density (default=1) for matplotlib streamplot
 • zIndexIf3D (int) – index in Z if using 3D field map (default=0)
 • useColour (bool :param aspect: Matplotlib axes aspect (e.g. 'auto'
 or 'equal')) – use magnitude of field as colour.
 Note, matplotlibs streamplot may raise an exception if the field is entriely 0 valued.
-
-84
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 pybdsim.Field.FieldPlotter.Plot2DXZStream(filename, density=1, yIndexIf3D=0, useColour=True,
 aspect='equal')
 Plot a bdsim field map file using the X,Z plane as a stream plot and plotting Fx, Fz.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D or Field3D instance) –
 name of field map file or object
 • density (float) – arrow density (default=1) for matplotlib streamplot
@@ -3401,14 +3427,20 @@
 pybdsim.Field.FieldPlotter.Plot3DXZ(filename, scale=None)
 Plots (B_x,B_z) as a function of x and z.
 class pybdsim.Field.FieldPlotter.ThreeDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 class pybdsim.Field.FieldPlotter.TwoDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 
+14.7. pybdsim.Field module
+
+85
+
+pybdsim Documentation, Release 3.3.0
+
 14.8 pybdsim.Gmad module
 Survey() - survey a gmad lattice, plot element coords
 Loader() - load a gmad file using the compiled bdsim parser
 GmadFile() - modify a text based gmad file
 
 class pybdsim.Gmad.GmadFile(fileName)
 Bases: object
@@ -3421,21 +3453,14 @@
 Class to load a gmad components file to a buffer and modify the contents
 Example : python> g = pybdsim.Gmad.GmadFileComponents(“./atf2_components.gmad”) python>
 g.change(“KEX1A”,”l”,”10”) python> g.write(“./atf2_components.gmad”)
 change(element, parameter, value)
 Edit element dictionary
 elementNames()
 Make a list of element names, stored in self.elementNameList
-
-14.8. pybdsim.Gmad module
-
-85
-
-pybdsim Documentation, Release 3.3.0
-
 findElement(elementName)
 Returns the start and end (inclusive location of the element lines as a tuble (start,end)
 getParameter(element, parameter)
 Edit element dictionary
 getType(element)
 parseElement(elementString)
 Create element dictionary from element
@@ -3446,14 +3471,21 @@
 class pybdsim.Gmad.Lattice(filename=None)
 Bases: object
 BDSIM Gmad parser lattice.
 Use this class to load a bdsim input file using the BDSIM parser (GMAD) and then interrogate it. You can
 use this to regenerate a lattice with less information for example
 >>> a = Lattice("filename.gmad")
 or
+
+86
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 >>> a = Lattice()
 >>> a.Load("filename.gmad")
 >>> a # this will tell you some basic details
 >>> print(a) # this will print out the full lattice
 GetAllNames()
 GetAngle(index)
 GetAper1(index)
@@ -3465,21 +3497,14 @@
 GetColumn(column)
 GetElement(i)
 GetIndexOfElementNamed(elementname)
 GetKs(index)
 GetLength(index)
 GetName(index)
 GetType(index)
-
-86
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 IndexFromNearestS(S)
 return the index of the beamline element clostest to S
 Load(filename)
 Load the BDSIM input file and parse it using the BDSIM parser (GMAD).
 ParseLattice()
 Put lattice data into python data structure
 Print(includeheaderlines=True)
@@ -3490,14 +3515,21 @@
 Bases: object
 Survey - load a gmad lattice and have a look
 Example:
 >>> a = Survey()
 >>> a.Load('mylattice.gmad')
 >>> a.Plot()
 CompareMadX(fileName)
+
+14.8. pybdsim.Gmad module
+
+87
+
+pybdsim Documentation, Release 3.3.0
+
 FinalDiff()
 FindClosestElement(coord)
 Load(filename)
 Plot()
 Step(angle, length)
 
 14.9 pybdsim.ModelProcessing module
@@ -3512,20 +3544,14 @@
 Inspect pybdsim.Data.ModelData assuming collimator info was stored to give an axis aligned bounding box
 set of ranges in global coordinates.
 pybdsim.ModelProcessing.GetMaterialIDOfCollimator(modelData, collimatorName)
 Inspect pybdsim.Data.ModelData assuming collimator info was stored to give an axis aligned bounding box
 set of ranges in global coordinates.
 pybdsim.ModelProcessing.WrapLatticeAboutItem(maingmadfile, itemname, outputfilename)
 
-14.9. pybdsim.ModelProcessing module
-
-87
-
-pybdsim Documentation, Release 3.3.0
-
 14.10 pybdsim.Options module
 See Options class inside this module.
 pybdsim.Options.ElectronColliderOptions()
 class pybdsim.Options.Options(*args, **kwargs)
 Bases: dict
 Inherits a dict. Converting to a string or using ReturnOptionsString() will give a suitable GMAD string to
 write out to a file.
@@ -3533,14 +3559,21 @@
 aper1=5*m;’
 There is no checking on the option if using []. A tuple of (value, unitsString) can be used too resulting in
 value*unitsString.
 ReturnOptionsString()
 SetBLMLength(length=50.0, unitsstring='cm')
 SetBLMRadius(radius=5.0, unitsstring='cm')
 SetBeamPipeRadius(beampiperadius=5.0, unitsstring='cm')
+
+88
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 SetBeamPipeThickness(bpt, unitsstring='mm')
 SetBeamlineS(beamlineS=0, unitsstring='m')
 SetBuildTunnel(tunnel=False)
 SetBuildTunnelFloor(tunnelfloor=False)
 SetCherenkovOn(on=True)
 SetChordStepMinimum(csm=1.0, unitsstring='nm')
 SetDefaultBiasMaterial(biases='')
@@ -3552,35 +3585,35 @@
 SetDontSplitSBends(dontsplitsbends=False)
 SetELossHistBinWidth(width)
 SetEMLeadParticleBiasing(on=True)
 SetEPAnnihilation2HadronEnhancementFactor(ef=1.0)
 SetEPAnnihilation2MuonEnhancementFactor(ef=1.0)
 SetGamma2MuonEnahncementFactor(ef=1.0)
 SetGeneralOption(option, value)
-
-88
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 SetIncludeFringeFields(on=True)
 SetIncludeIronMagField(iron=True)
 SetIntegratorSet(integratorSet='"bdsim"')
 SetLPBFraction(fraction=0.5)
 SetLengthSafety(ls=10.0, unitsstring='um')
 SetMagnetGeometryType(magnetGeometryType='"none"')
 SetMaximumEpsilonStep(mes=1.0, unitsstring='m')
 SetMaximumStepLength(msl=20.0, unitsstring='m')
 SetMaximumTrackingTime(mtt=-1.0, unitsstring='s')
 SetMinimumEpsilonStep(mes=10.0, unitsstring='nm')
 SetNGenerate(nparticles=10)
 SetNLinesIgnore(nlines=0)
 SetNPerFile(nperfile=100)
 SetOuterDiameter(outerdiameter=2.0, unitsstring='m')
+
+14.10. pybdsim.Options module
+
+89
+
+pybdsim Documentation, Release 3.3.0
+
 SetPhysicsList(physicslist='')
 SetPipeMaterial(bpm)
 SetPrintModuloFraction(pmf=0.01)
 SetProductionCutElectrons(pc=100.0, unitsstring='keV')
 SetProductionCutPhotons(pc=100.0, unitsstring='keV')
 SetProductionCutPositrons(pc=100.0, unitsstring='keV')
 SetRandomSeed(rs=0)
@@ -3592,21 +3625,14 @@
 SetSenssitiveBLMs(on=True)
 SetSoilMaterial(sm)
 SetSoilThickness(st=4.0, unitsstring='m')
 SetStopSecondaries(stop=True)
 SetStoreTrajectory(on=True)
 SetStoreTrajectoryParticle(particle='muon')
 SetSynchRadiationOn(on=True)
-
-14.10. pybdsim.Options module
-
-89
-
-pybdsim Documentation, Release 3.3.0
-
 SetThresholdCutCharged(tcc=100.0, unitsstring='MeV')
 SetThresholdCutPhotons(tcp=1.0, unitsstring='MeV')
 SetTrackSRPhotons(track=True)
 SetTrajectoryCutGTZ(gtz=0.0, unitsstring='m')
 SetTrajectoryCutLTR(ltr=10.0, unitsstring='m')
 SetTunnelFloorOffset(offset=1.0, unitsstring='m')
 SetTunnelMaterial(tm)
@@ -3616,14 +3642,20 @@
 SetTunnelThickness(tt=1.0, unitsstring='m')
 SetVacuumMaterial(vm)
 SetVacuumPressure(vp)
 Vacuum pressure in bar
 SetWritePrimaries(on=True)
 pybdsim.Options.ProtonColliderOptions()
 
+90
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 14.11 pybdsim.Plot module
 Useful plots for bdsim output
 pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(figure, surveyfile, tightLayout=True,
 sOffset=0.0, fraction=0.9)
 Add a machine diagram to the top of the plot in a current figure.
 Parameters
 • figure (matplotlib.figure.Figure) – the matplotlib figure to add the plot to.
@@ -3639,21 +3671,14 @@
 pybdsim.Plot.AddMachineLatticeFromSurveyToFigureMultiple(figure, machines, tightLayout=True)
 Similar to AddMachineLatticeFromSurveyToFigure() but accepts multiple machines.
 pybdsim.Plot.Aperture(rootFileName, filterThin=False, surveyFileName=None)
 pybdsim.Plot.BDSIMAperture(data, machineDiagram=True, plot='xy', plotApertureType=True,
 removeZeroLength=False, removeZeroApertures=True)
 Plot the aperture from a BDSIM DataLoader instance. By default it’s colour coded and excludes any 0
 aperture elements. Zero length elements are included.
-
-90
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 pybdsim.Plot.BDSIMApertureFromFile(filename, machineDiagram=True, plot='xy',
 plotApertureType=True, removeZeroLength=False,
 removeZeroApertures=True)
 Plot the aperture from a BDSIM output file. By default it’s colour coded and excludes any 0s.
 pybdsim.Plot.BDSIMOptics(rebdsimOpticsOutput, outputfilename=None, saveall=True, survey=None,
 **kwargs)
 Display all the optical function plots for a rebdsim optics root file. By default, this saves all optical functions
@@ -3665,14 +3690,21 @@
 Parameters
 • axesinstance (matplotlib.axes.Axes) – the plotting axis to draw the machine diagram into.
 • sOffset (float) – add this value to the S of all machine elements in the diagram.
 Param
 bdsasciidataobject The model data.
 The main interface is AddMachineLatticeFromSurveyToFigure, but this function may be useful for more
 granular plotting, e.g. with custom subfigures / axes.
+
+14.11. pybdsim.Plot module
+
+91
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Plot.EnergyDeposition(filename, outputfilename=None, tfssurvey=None, bdsimsurvey=None)
 Plot the energy deposition from a REBDSIM output file - uses premade merged histograms.
 Optional either Twiss table for MADX or BDSIM Survey to add machine diagram to plot. If both are provided, the machine diagram is plotted from the MADX survey.
 pybdsim.Plot.EnergyDepositionCoded(filename, outputfilename=None, tfssurvey=None,
 bdsimsurvey=None, warmaperinfo=None, **kwargs)
 Plot the energy deposition from a REBDSIM output file - uses premade merged histograms.
 Optional either Twiss table for MADX or BDSIM Survey to add machine diagram to plot. If both are provided, the machine diagram is plotted from the MADX survey.
@@ -3689,21 +3721,14 @@
 file with the plot. Default is None.
 tfssurvey (str, optional): Path to MADX survey used to plot machine diagram on top of figure. Default
 is None.
 tfssurvey (str, optional): Path to BDSIM survey used to classify losses into collimator/warm/cold and/or
 plot machine diagram on top of figure. Default is None.
 warmaperinfo (int|list|str, optional): Information about warm aperture in the machine. Default is None.
 **kwargs: Arbitrary keyword arguments.
-
-14.11. pybdsim.Plot module
-
-91
-
-pybdsim Documentation, Release 3.3.0
-
 Kwargs:
 skipMachineLattice (bool): If enabled, use the BDSIM survey to classify losses, but do not plot the
 lattice on top.
 Returns:
 matplotlib.pyplot.Figure object
 pybdsim.Plot.Histogram1D(histogram, xlabel=None, ylabel=None, title=None, scalingFactor=1.0,
 xScalingFactor=1.0, figsize=(6.4, 4.8), log=False, **errorbarKwargs)
@@ -3716,14 +3741,21 @@
 • xScalingFactor – multiplier for x axis coordinates
 • log – whether to automatically plot on a vertical log scale
 return figure instance
 pybdsim.Plot.Histogram1DMultiple(histograms, labels, log=False, xlog=False, xlabel=None,
 ylabel=None, title=None, scalingFactors=None,
 xScalingFactors=None, figsize=(10, 5), legendKwargs={},
 **errorbarKwargs)
+
+92
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 Plot multiple 1D histograms on the same plot. Histograms and labels should be lists of the same length with
 pybdsim.Data.TH1 objects and strings.
 return figure instance
 xScalingFactors may be a float, int or list
 Example:
 Histogram1DMultiple([h1,h2,h3],
 ['Photons', 'Electrons', 'Positrons'],
@@ -3741,20 +3773,14 @@
 Parameters
 • histogram1 – a pybdsim.Data.TH1 instance
 • histogram2 – a pybdsim.Data.TH1 instance
 • label1 – legend label for histogram1 (str or “” or None)
 • label2 – legend label for histogram2
 • ratio – integer ratio of main plot height to ratio plot height (recommend 1 - 5)
 • ratioYAxisLimit (tuple(float, float)) – ylim upper for ratio subplot y axis
-92
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 If the labels are “” then the histogram.title string will be used. If None, then no label will be added.
 pybdsim.Plot.Histogram2D(histogram, logNorm=False, xLogScale=False, yLogScale=False, xlabel='',
 ylabel='', zlabel='', title='', aspect='auto', scalingFactor=1.0,
 xScalingFactor=1.0, yScalingFactor=1.0, figsize=(6, 5), vmin=None,
 autovmin=False, vmax=None, colourbar=True, **imshowKwargs)
 Plot a pybdsim.Data.TH2 instance. logNorm - logarithmic colour scale xlogscale - x axis logarithmic scale
 ylogscale - y axis logarithmic scale zlabel - label for color bar scale aspect - “auto”, “equal”, “none” - see
@@ -3766,14 +3792,21 @@
 pybdsim.Plot.Histogram2DErrors(histogram, logNorm=False, xLogScale=False, yLogScale=False,
 xlabel='', ylabel='', zlabel='', title='', aspect='auto', scalingFactor=1.0,
 xScalingFactor=1.0, yScalingFactor=1.0, figsize=(6, 5), vmin=None,
 autovmin=False, vmax=None, **imshowKwargs)
 Similar to Histogram2D() but plot the errors from the histogram instead of the contents. See pybdsim.Plot.Histogram2D for documentation of arguments.
 pybdsim.Plot.Histogram3D(th3)
 Plot a pybdsim.Data.TH3 instance - TBC
+
+14.11. pybdsim.Plot module
+
+93
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Plot.LossAndEnergyDeposition(filename, outputfilename=None, tfssurvey=None,
 bdsimsurvey=None, hitslegendloc='upper left',
 elosslegendloc='upper right', perelement=False,
 elossylim=None, phitsylim=None)
 Load a REBDSIM output file and plot the merged histograms automatically generated by BDSIM.
 Optional either Twiss table for MADX or BDSIM Survey to add machine diagram to plot.
 pybdsim.Plot.LossMap(ax, xcentres, y, ylow=None, **kwargs)
@@ -3793,21 +3826,14 @@
 end positions of each element in the sequence.
 pybdsim.Plot.ModelBDSIMYZ(model, ax=None)
 The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey done in BDSIM.
 The results can be found in the BDSIM output file in the Model tree. The functions can plot the start and
 end positions of each element in the sequence.
 pybdsim.Plot.ModelElegantXZ(model, ax=None, transpose=False)
 Plot a model madx from elegant. In development.
-
-14.11. pybdsim.Plot module
-
-93
-
-pybdsim Documentation, Release 3.3.0
-
 pybdsim.Plot.ModelElegantYZ(model, ax=None, transpose=False)
 Plot a model madx from elegant. In development.
 pybdsim.Plot.PhaseSpace(data, nbins=None, outputfilename=None, extension='.pdf')
 Make two figures for coordinates and correlations.
 Number of bins chosen depending on number of samples.
 ‘outputfilename’ should be without an extension - any extension will be stripped off.
 Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g.
@@ -3819,14 +3845,20 @@
 Number of bins chosen depending on number of samples.
 ‘outputfilename’ should be without an extension - any extension will be stripped off. Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g. extension=’.png’.
 pybdsim.Plot.PhaseSpaceSeparateAxes(filename, samplerIndexOrName=0, outputfilename=None,
 extension='.pdf', nbins=None, energy='total', offsetTime=True,
 includeSecondaries=False, coordsTitle=None,
 correlationTitle=None, scalefactors={}, labels={},
 log1daxes=False, log2daxes=False, includeColorbar=True)
+94
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 Plot the coordinates and correlations of both the transverse and longitudinal phase space in separate plots
 (four total) recorded in a sampler. Default sampler is the primary distribution.
 ‘outputfilename’ is name without extension, extension can be supplied as a string separately. Default = pdf.
 The number of bins chosen depending on number of samples. Can be overridden with nbins.
 Energy can be binned as either kinetic or total (default), supply either energy=’total’ or energy=’kinetic’.
 offSetTime centers the time distribution about the nominal time for the specified sampler rather than the
 absolute time. Default = True.
@@ -3840,35 +3872,35 @@
 includeColorbar adds a colorbar to the correlation plots. The colorbar is normalised for all plot subfigures.
 Default = True.
 pybdsim.Plot.PlotAlpha(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotBeta(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotDisp(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotDispP(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotMean(bds, outputfilename=None, survey=None, **kwargs)
-
-94
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 pybdsim.Plot.PlotNPart(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotSigma(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotSigmaP(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PrimaryPhaseSpace(filename, outputfilename=None, extension='.pdf')
 Load a BDSIM output file and plot primary phase space. Only accepts raw BDSIM output.
 ‘outputfilename’ should be without an extension - any extension will be stripped off. Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g. extension=’.png’.
 pybdsim.Plot.PrimarySurvival(filename, outputfilename=None, tfssurvey=None, bdsimsurvey=None)
 pybdsim.Plot.PrimaryTrajectoryAndProcess(rootData, eventNumber)
 pybdsim.Plot.ProvideWrappedS(sArray, index)
 pybdsim.Plot.Spectra(spectra, log=False, xlog=False, xlabel=None, ylabel=None, title=None,
 scalingFactors=None, xScalingFactors=None, figsize=(10, 5), legendKwargs={},
 vmin=None, vmax=None, **errorbarKwargs)
 Plot a Spectra object loaded from data that represents a set of histograms.
 returns a list of figure objects.
+
+14.11. pybdsim.Plot module
+
+95
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Plot.SubplotsWithDrawnMachineLattice(survey, nrows=2, machine_plot_gap=0.01,
 gridspec_kw=None, subplots_kw=None, **fig_kw)
 Create a figure with a single column of axes, sharing the x-axis by default, with the machine drawn from the
 provided survey on the top row axes. nrows gives the number of axes, the first is always the machine lattice.
 by default 2 are drawn, the first for the machine, and the second for any data to be plotted to afterwards.
 Parameters
 survey (str, pybdsim.Data.BDSAsciiData) – BDSIM survey which is used to draw
@@ -3888,21 +3920,14 @@
 options=None, bdsimExecutable=None)
 Runs bdsim with gmadpath as inputfile and outfile as outfile. Runs in batch mode by default, with 10,000
 particles. Any extra options should be provided as a string or iterable of strings of the form “–vis_debug” or
 “–vis_mac=vis.mac”, etc.
 class pybdsim.Run.ExecOptions(*args, **kwargs)
 Bases: dict
 GetExecArgs()
-
-14.12. pybdsim.Run module
-
-95
-
-pybdsim Documentation, Release 3.3.0
-
 GetExecFlags()
 pybdsim.Run.GetOpticsFromGMAD(gmad, keep_optics=False)
 Get the optical functions as a BDSAsciiData instance from this GMAD file. If keep_optics is false then all
 intermediate files are discarded, otherwise the final optics ROOT file is written to ./
 class pybdsim.Run.GmadModifier(rootgmadfilename)
 Bases: object
 CheckExtensions()
@@ -3910,14 +3935,21 @@
 ReplaceTokens(tokenDict)
 pybdsim.Run.Rebdsim(rootpath, inpath, outpath, silent=False, rebdsimExecutable=None)
 Run rebdsim with rootpath as analysisConfig file, inpath as bdsim file, and outpath as output analysis file.
 pybdsim.Run.RebdsimCombine(rootpath, outpath, silent=False, rebdsimHistoExecutable=None)
 Run rebdsimCombine
 pybdsim.Run.RebdsimHistoMerge(rootpath, outpath, silent=False, rebdsimHistoExecutable=None)
 Run rebdsimHistoMerge
+
+96
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Run.RebdsimOptics(rootpath, outpath, silent=False)
 Run rebdsimOptics
 pybdsim.Run.RebdsimOrbit(rootpath, outpath, index='1', silent=False, rebdsimHistoExecutable=None)
 Run rebdsimOrbit
 class pybdsim.Run.Study
 Bases: object
 A holder for multiple runs.
@@ -3935,33 +3967,33 @@
 draw()
 Quick survey drawing for diagnostic reasons.
 findComponentCoords(componentName)
 Returns the XYZ coordinates of a component relative to the centre
 getWorldCentre(type='linear')
 Returns the center in world coordinates of the centre of the visualisation space
 
-96
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 14.14 pybdsim.Writer module
 Writer
 Write files for a pybdsim.Builder.Machine instance. Each section of the written output (e.g. components, sequence,
 beam etc.) can be written in the main gmad file, written in its own separate file, or called from an external, preexisting file.
 Classes: File - A class that represents each section of the written output - contains booleans and strings. Writer A class that writes the data to disk.
 class pybdsim.Writer.FileSection(willContain='')
 Bases: object
 A class that represents a section of a gmad file. The sections that this class can represent are:
 • Components
 • Sequence
 • Samplers
 • Beam
 • Options
+14.13. pybdsim.Visualisation module
+
+97
+
+pybdsim Documentation, Release 3.3.0
+
 • Bias
 • Material
 The class contains booleans and strings relating to the location of that sections data. The section can set to
 be:
 • Written in its own separate file (default)
 • Written in the main gmad file
 • Called from an external file
@@ -3978,21 +4010,14 @@
 WriteInMain()
 WriteSeparately()
 class pybdsim.Writer.Writer
 Bases: object
 A class for writing a pybdsim.Builder.Machine instance to file.
 This class allows the user to write individual sections of a BDSIM input file (e.g. components, sequence,
 beam etc.) or write the machine as a whole.
-
-14.14. pybdsim.Writer module
-
-97
-
-pybdsim Documentation, Release 3.3.0
-
 There are 6 attributes in this class which are FileSection instances representing each section of the data. The
 location where these sections will be written/read is stored in these instances. See the FileSection class for
 further details.
 The optional boolean ‘singlefile’ in the WriteMachine function for writing the sections to a single file overrides any sections locations set in their respective FileSection instances.
 This class also has individual functions (e.g. WriteBeam) to write each file section and the main file
 (WriteMain) separately. These section functions must be called BEFORE the WriteMain function is called
 otherwise the main file will have no reference to these sections.
@@ -4004,14 +4029,20 @@
 lattice_components.gmad
 lattice_sequence.gmad
 lattice_beam.gmad
 lattice.gmad
 All included in main file:
 lattice.gmad
 Writing the Builder.Machine instance myMachine into a single file:
+98
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 >>> a = Writer()
 >>> a.WriteMachine(myMachine,'lattice.gmad',singlefile=True)
 Lattice written to:
 lattice.gmad
 All included in main file:
 lattice.gmad
 WriteBeam(machine, filename='')
@@ -4040,20 +4071,14 @@
 machine biases (if defined)
 machine materials (if defined)
 suitable main file with all sub files in correct order
 
 These are prefixed with the specified filename / path
 The optional bool singlefile = True will write all the above sections into a single file:
 filename.gmad
-98
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.3.0
-
 kwargs: overwrite : Do not append an integer to the basefilename if already exists, instead overwrite
 existing files.
 WriteMain(machine(machine), filename(string))
 Write the main gmad file: filename.gmad
 The
 functions
 for
@@ -4072,14 +4097,19 @@
 WriteOptions(machine, filename='')
 Write a machines options to disk: filename.gmad
 Machine can be either a pybdsim.Builder.Machine instance or a pybdsim.Options.Options instance.
 WriteSamplers(machine, filename='')
 Write the machines samplers to disk: filename.gmad
 WriteSequence(machine, filename='')
 Write the machines sequence to disk: filename.gmad
+14.14. pybdsim.Writer module
+
+99
+
+pybdsim Documentation, Release 3.3.0
 
 14.15 pybdsim.XSecBias module
 class pybdsim.XSecBias.XSecBias(name, particle, processes, xsecfactors, flags)
 Bases: object
 A class for containing all information regarding cross section definitions.
 CheckBiasedProcesses()
 SetFlags(flags)
@@ -4089,20 +4119,14 @@
 SetParticle(particle)
 Set the particle for bias to be associated with.
 SetProcesses(processes)
 Set the list of processes to be biased. processes hould be a space-delimited string of processes.
 SetXSecFactors(xsecs)
 Set cross section factors. xsecs should be a space-delimited string of floats, e.g. “1.0 1e13 1234.9”
 
-14.15. pybdsim.XSecBias module
-
-99
-
-pybdsim Documentation, Release 3.3.0
-
 100
 
 Chapter 14. Module Contents
 
 CHAPTER
 
 FIFTEEN
@@ -4166,22 +4190,22 @@
 pybdsim.Constants, 68
 pybdsim.Convert, 68
 pybdsim.Convert._MadxTfs2Gmad, 71
 pybdsim.Data, 73
 pybdsim.Field, 80
 pybdsim.Field._Field, 80
 pybdsim.Field.FieldPlotter, 82
-pybdsim.Gmad, 85
-pybdsim.ModelProcessing, 87
+pybdsim.Gmad, 86
+pybdsim.ModelProcessing, 88
 pybdsim.Options, 88
-pybdsim.Plot, 90
-pybdsim.Run, 95
-pybdsim.Visualisation, 96
+pybdsim.Plot, 91
+pybdsim.Run, 96
+pybdsim.Visualisation, 97
 pybdsim.Writer, 97
-pybdsim.XSecBias, 99
+pybdsim.XSecBias, 100
 
 105
 
 pybdsim Documentation, Release 3.3.0
 
 106
 
@@ -4276,19 +4300,19 @@
 AddWireScanner()
 (pybdsim.Builder.Machine
 AddKicker() (pybdsim.Builder.Machine method), 63
 method), 64
 AddLaser() (pybdsim.Builder.Machine method), 63
 AddMachineLatticeFromSurveyToFigure()
 (in Aperture (class in pybdsim.Builder), 58
-Aperture() (in module pybdsim.Plot), 90
-module pybdsim.Plot), 90
+Aperture() (in module pybdsim.Plot), 91
+module pybdsim.Plot), 91
 AddMachineLatticeFromSurveyToFigureMultiple()ApertureInfo (class in pybdsim.Data), 73
 ApertureModel (class in pybdsim.Builder), 58
-(in module pybdsim.Plot), 90
+(in module pybdsim.Plot), 91
 Append() (pybdsim.Builder.Machine method), 64
 AddMarker() (pybdsim.Builder.Machine method), 63
 AddMaterial() (pybdsim.Builder.Machine method), append() (pybdsim.Data.Spectra method), 78
 Atom (class in pybdsim.Builder), 58
 63
 AddMultipole() (pybdsim.Builder.Machine method),
 63
@@ -4298,17 +4322,17 @@
 BDSAsciiData (class in pybdsim.Data), 73
 
 107
 
 pybdsim Documentation, Release 3.3.0
 
 BDSBH4D (class in pybdsim.Data), 74
-Bdsim() (in module pybdsim.Run), 95
-BDSIMAperture() (in module pybdsim.Plot), 90
-BDSIMApertureFromFile() (in module pybdsim.Plot), 90
+Bdsim() (in module pybdsim.Run), 96
+BDSIMAperture() (in module pybdsim.Plot), 91
+BDSIMApertureFromFile() (in module pybdsim.Plot), 91
 BDSIMOptics() (in module pybdsim.Plot), 91
 BdsimPrimaries2Mad8()
 (in
 module
 pybdsim.Convert), 68
 BdsimPrimaries2Madx()
 (in
@@ -4319,333 +4343,307 @@
 module
 pybdsim.Convert), 69
 BDSIMVsBDSIM() (in module pybdsim.Compare), 68
 Beam (class in pybdsim.Beam), 57
 BeamData (class in pybdsim.Data), 74
 BLM (class in pybdsim.Builder), 58
 
+DrawMachineLattice() (in module pybdsim.Plot), 91
+Drift (class in pybdsim.Builder), 59
+Dump (class in pybdsim.Builder), 59
+
 E
 
 ECol (class in pybdsim.Builder), 59
 ElectronColliderOptions() (in module pybdsim.Options), 88
 Element (class in pybdsim.Builder), 59
 ElementBase (class in pybdsim.Builder), 60
 ElementModifier (class in pybdsim.Builder), 60
 elementNames()
 (pybdsim.Gmad.GmadFileComponents method),
-85
+86
 EnergyDeposition() (in module pybdsim.Plot), 91
-EnergyDepositionCoded() (in module pybdsim.Plot), 91
+EnergyDepositionCoded() (in module pybdsim.Plot), 92
+C
 ErrorsToErrorOnMean() (pybdsim.Data.BDSBH4D
+CallExternalFile()
+(pybdsim.Writer.FileSection
 method), 74
+method), 98
 ErrorsToErrorOnMean() (pybdsim.Data.ROOTHist
+CavityInfo (class in pybdsim.Data), 74
 method), 77
-C
+CavityModel (class in pybdsim.Builder), 58
 ErrorsToSTD() (pybdsim.Data.BDSBH4D method),
-CallExternalFile()
-(pybdsim.Writer.FileSection
+change()
+(pybdsim.Gmad.GmadFileComponents
 74
-method), 97
+method), 86
 ErrorsToSTD() (pybdsim.Data.ROOTHist method),
-CavityInfo (class in pybdsim.Data), 74
+CheckBdsimDataHasSurveyModel() (in module
 77
-CavityModel (class in pybdsim.Builder), 58
+pybdsim.Data), 74
 EventInfoData (class in pybdsim.Data), 74
-change()
-(pybdsim.Gmad.GmadFileComponents EventSummaryData (class in pybdsim.Data), 74
-method), 85
-ExecOptions (class in pybdsim.Run), 95
 CheckBiasedProcesses()
-(pybd- ExternalGeometry (class in pybdsim.Builder), 60
-sim.XSecBias.XSecBias method), 99
+(pybd- EventSummaryData (class in pybdsim.Data), 74
+sim.XSecBias.XSecBias method), 100
+ExecOptions (class in pybdsim.Run), 96
 CheckExtensions()
-(pybdsim.Run.GmadModifier F
+(pybdsim.Run.GmadModifier ExternalGeometry (class in pybdsim.Builder), 60
 method), 96
+CheckItsBDSAsciiData() (in module pybd- F
+sim.Data), 74
 Field (class in pybdsim.Builder), 60
 CollimatorInfo (class in pybdsim.Data), 74
 Field (class in pybdsim.Field._Field), 80
 CompareMadX() (pybdsim.Gmad.Survey method), 87
 Field1D (class in pybdsim.Field._Field), 80
 ConcatenateMachine()
-(pybd- Field2D (class in pybdsim.Field._Field), 80
+(pybd- Field2D (class in pybdsim.Field._Field), 81
 sim.Data.BDSAsciiData method), 73
 Field3D (class in pybdsim.Field._Field), 81
 ConvertToPybdsimHistograms()
 (pybd- Field4D (class in pybdsim.Field._Field), 81
 sim.Data.RebdsimFile method), 77
 FileSection (class in pybdsim.Writer), 97
 CreateDipoleDriftRing() (in module pybd- Fill() (pybdsim.Data.Histogram1DSet method), 75
 sim.Builder), 58
 Filter() (pybdsim.Data.BDSAsciiData method), 73
 CreateDipoleFodoRing() (in module pybd- FinalDiff() (pybdsim.Gmad.Survey method), 87
 sim.Builder), 59
 FindClosestElement()
 (pybdsim.Gmad.Survey
 CreateDipoleRing() (in module pybdsim.Builder),
-method), 87
+method), 88
 59
 findComponentCoords()
-(pybdCreateEmptyRebdsimFile() (in module pybdsim.Visualisation.Helper method), 96
+(pybdCreateEmptyRebdsimFile() (in module pybdsim.Visualisation.Helper method), 97
 sim.Data), 74
 findElement()
 (pybdCreateFodoLine() (in module pybdsim.Builder), 59
 sim.Gmad.GmadFileComponents method),
 Crystal (class in pybdsim.Builder), 59
-85
+86
 CrystalCol (class in pybdsim.Builder), 59
 Flush() (pybdsim.Data.Histogram1DSet method), 75
-
 FourDData (class in pybdsim.Field.FieldPlotter), 82
+D
 from_element() (pybdsim.Builder.Element class
 Decapole (class in pybdsim.Builder), 59
 method), 60
 DefineConstituentElements()
 (pybd- FromROOTFile() (pybdsim.Data.BeamData class
 sim.Builder.Line method), 61
 method), 74
 Degrader (class in pybdsim.Builder), 59
 FromROOTFile() (pybdsim.Data.EventInfoData class
 DetermineIncludes() (pybdsim.Run.GmadModifier
 method), 74
 method), 96
 FromROOTFile() (pybdsim.Data.ModelData class
-draw() (pybdsim.Visualisation.Helper method), 96
-method), 76
-DrawMachineLattice() (in module pybdsim.Plot), 91 FromROOTFile() (pybdsim.Data.OptionsData class
-Drift (class in pybdsim.Builder), 59
+draw() (pybdsim.Visualisation.Helper method), 97
 method), 76
-Dump (class in pybdsim.Builder), 59
-
-D
 
 108
 
 Index
 
 pybdsim Documentation, Release 3.3.0
 
-G
+FromROOTFile() (pybdsim.Data.OptionsData class
+method), 76
 
-GetPDGInd() (in module pybdsim.Constants), 68
-GetPDGName() (in module pybdsim.Constants), 68
+GetOpticsFromGMAD() (in module pybdsim.Run), 96
+getParameter()
+(pybdsim.Gmad.GmadFileComponents method),
+G
+86
+GetPDGInd()
+(in module pybdsim.Constants), 68
 Gap (class in pybdsim.Builder), 60
+GetPDGName()
+(in module pybdsim.Constants), 68
+GenerateFullListOfSamplers() (in module pybdgetType()
 (pybdsim.Gmad.GmadFileComponents
-GenerateFullListOfSamplers() (in module pybd- getType()
-method),
-86
-sim.ModelProcessing), 87
-GetType()
-(pybdsim.Gmad.Lattice
+sim.ModelProcessing), 88
 method), 86
 GenerateSamplersFromBDSIMSurvey() (in module
+GetType() (pybdsim.Gmad.Lattice method), 87
+pybdsim.Builder), 61
 getWorldCentre()
 (pybdsim.Visualisation.Helper
-pybdsim.Builder), 61
-method), 96
-GetAllNames() (pybdsim.Gmad.Lattice method), 86
-GmadFile
-(class in pybdsim.Gmad), 85
-GetAngle() (pybdsim.Gmad.Lattice method), 86
-GmadFileBeam
-(class in pybdsim.Gmad), 85
-GetAper1() (pybdsim.Gmad.Lattice method), 86
-GmadFileComponents
-(class in pybdsim.Gmad), 85
-GetAper2() (pybdsim.Gmad.Lattice method), 86
-GmadFileOptions
-(class
-in pybdsim.Gmad), 86
-GetAper3() (pybdsim.Gmad.Lattice method), 86
-GmadModifier
-(class
-in
-pybdsim.Run),
-96
-GetAper4() (pybdsim.Gmad.Lattice method), 86
-GmadObject
-(class
-in
-pybdsim.Builder),
-61
+GetAllNames() (pybdsim.Gmad.Lattice method), 87
+method), 97
+GetAngle() (pybdsim.Gmad.Lattice method), 87
+GmadFile (class in pybdsim.Gmad), 86
+GetAper1() (pybdsim.Gmad.Lattice method), 87
+GmadFileBeam (class in pybdsim.Gmad), 86
+GetAper2() (pybdsim.Gmad.Lattice method), 87
+GmadFileComponents (class in pybdsim.Gmad), 86
+GetAper3() (pybdsim.Gmad.Lattice method), 87
+GmadFileOptions (class in pybdsim.Gmad), 86
+GetAper4() (pybdsim.Gmad.Lattice method), 87
 GetApertureData()
-(pybdsim.Data.ModelData
+(pybdsim.Data.ModelData GmadModifier (class in pybdsim.Run), 96
+GmadObject (class in pybdsim.Builder), 61
 method), 76
-GetApertureExtent() (in module pybdsim.Data), 74 H
+GetApertureExtent() (in module pybdsim.Data), 74
 GetApertureExtents()
-(pybdsim.Gmad.Lattice Header (class in pybdsim.Data), 75
-Helper (class in pybdsim.Visualisation), 96
-method), 86
+(pybdsim.Gmad.Lattice H
+Header (class in pybdsim.Data), 75
+method), 87
 GetApertureType()
-(pybdsim.Gmad.Lattice Histogram1D() (in module pybdsim.Plot), 92
-Histogram1DMultiple() (in module pybdsim.Plot),
-method), 86
+(pybdsim.Gmad.Lattice Helper (class in pybdsim.Visualisation), 97
+Histogram1D() (in module pybdsim.Plot), 92
+method), 87
+GetAxisAlignedBoundingBoxOfCollimator() (in Histogram1DMultiple() (in module pybdsim.Plot),
 92
-GetAxisAlignedBoundingBoxOfCollimator() (in
-Histogram1DRatio()
-(in module pybdsim.Plot), 92
-module pybdsim.ModelProcessing), 87
-Histogram1DSet
-(class
-in pybdsim.Data), 75
-GetColumn() (pybdsim.Data.BDSAsciiData method),
-Histogram2D()
-(in
-module
-pybdsim.Plot), 93
+module pybdsim.ModelProcessing), 88
+GetColumn() (pybdsim.Data.BDSAsciiData method), Histogram1DRatio() (in module pybdsim.Plot), 93
+Histogram1DSet (class in pybdsim.Data), 75
 73
-Histogram2DErrors()
-(in
-module
-pybdsim.Plot), 93
-GetColumn() (pybdsim.Gmad.Lattice method), 86
-Histogram3D()
-(in
-module
-pybdsim.Plot),
-93
-GetElement() (pybdsim.Gmad.Lattice method), 86
-HKicker
-(class
-in
-pybdsim.Builder),
-61
-GetExecArgs() (pybdsim.Run.ExecOptions method),
-95
-GetExecFlags() (pybdsim.Run.ExecOptions method), I
-95
+Histogram2D() (in module pybdsim.Plot), 93
+GetColumn() (pybdsim.Gmad.Lattice method), 87
+Histogram2DErrors() (in module pybdsim.Plot), 93
+GetElement() (pybdsim.Gmad.Lattice method), 87
+GetExecArgs() (pybdsim.Run.ExecOptions method), Histogram3D() (in module pybdsim.Plot), 93
+HKicker (class in pybdsim.Builder), 61
+96
+GetExecFlags() (pybdsim.Run.ExecOptions method),
+I
+96
+GetFileName() (in module pybdsim.Data), 74
 IndexFromNearestS() (pybdsim.Data.BDSAsciiData
 GetHistoryPDGTuple() (in module pybdsim.Data),
 method), 73
 74
 IndexFromNearestS()
 (pybdsim.Gmad.Lattice
 GetIndexOfElementNamed()
-(pybdmethod), 86
-sim.Gmad.Lattice method), 86
+(pybdmethod), 87
+sim.Gmad.Lattice method), 87
 InsertAndReplace()
 (pybdsim.Builder.Machine
-GetInfo() (pybdsim.Run.Study method), 96
+GetInfo() (pybdsim.Run.Study method), 97
 method), 64
 GetIntegratedAngle() (pybdsim.Builder.Machine IntegateAlong1Dimension() (pybdsim.Data.TH3
 method), 64
-method), 78
+method), 79
 GetIntegratedLength() (pybdsim.Builder.Machine IntegateAlong2Dimensions() (pybdsim.Data.TH3
 method), 64
 method), 79
 GetItemTuple()
 (pybdsim.Data.BDSAsciiData IntegrateAlongX() (pybdsim.Data.TH2 method), 78
 method), 73
 IntegrateAlongY() (pybdsim.Data.TH2 method), 78
-GetKs() (pybdsim.Gmad.Lattice method), 86
-GetLength() (pybdsim.Gmad.Lattice method), 86
-J
-GetMaterialIDOfCollimator() (in module pybd- JCol (class in pybdsim.Builder), 61
-sim.ModelProcessing), 87
-GetModel() (pybdsim.Data.RebdsimFile method), 77 K
-GetModelForPlotting() (in module pybdsim.Data),
-keysextra() (pybdsim.Builder.ElementBase method),
+GetKs() (pybdsim.Gmad.Lattice method), 87
+IsSurvey() (in module pybdsim.Data), 75
+GetLength() (pybdsim.Gmad.Lattice method), 87
+GetMaterialIDOfCollimator() (in module pybd- J
+sim.ModelProcessing), 88
+JCol (class in pybdsim.Builder), 61
+GetModel() (pybdsim.Data.RebdsimFile method), 77
+GetModelForPlotting() (in module pybdsim.Data), K
 75
-60
+keysextra() (pybdsim.Builder.ElementBase method),
 GetModelTree()
 (pybdsim.Data.RebdsimFile
-keysextra() (pybdsim.Builder.GmadObject method),
+60
 method), 77
+keysextra() (pybdsim.Builder.GmadObject method),
+GetName() (pybdsim.Gmad.Lattice method), 87
 61
-GetName() (pybdsim.Gmad.Lattice method), 86
-Kicker (class in pybdsim.Builder), 61
 GetNamesOfType()
-(pybdsim.Builder.Machine
+(pybdsim.Builder.Machine Kicker (class in pybdsim.Builder), 61
 method), 64
-L
-GetNEventsInBDSIMFile() (in module pybdLaser (class in pybdsim.Builder), 61
+GetNEventsInBDSIMFile() (in module pybd- L
 sim.Data), 75
-GetOpticsFromGMAD() (in module pybdsim.Run), 96 Lattice (class in pybdsim.Gmad), 86
-getParameter()
-(pybd- Line (class in pybdsim.Builder), 61
-sim.Gmad.GmadFileComponents method), ListOfDirectories() (pybdsim.Data.RebdsimFile
-method), 77
-86
+Laser (class in pybdsim.Builder), 61
 Index
 
 109
 
 pybdsim Documentation, Release 3.3.0
 
+Lattice (class in pybdsim.Gmad), 86
+Line (class in pybdsim.Builder), 61
+ListOfDirectories() (pybdsim.Data.RebdsimFile
+method), 77
 ListOfLeavesInTree() (pybdsim.Data.RebdsimFile
 method), 77
 ListOfTrees() (pybdsim.Data.RebdsimFile method),
 77
-Load() (in module pybdsim.Data), 75
-Load() (in module pybdsim.Field._Field), 81
+Load() (in module pybdsim.Data), 76
+Load() (in module pybdsim.Field._Field), 82
 Load() (pybdsim.Gmad.Lattice method), 87
-Load() (pybdsim.Gmad.Survey method), 87
+Load() (pybdsim.Gmad.Survey method), 88
 LoadPickledObject() (in module pybdsim.Data), 76
 LoadROOTLibraries() (in module pybdsim.Data), 76
 LoadSDDSColumnsToDict() (in module pybdsim.Data), 76
 LossAndEnergyDeposition() (in module pybdsim.Plot), 93
-LossMap() (in module pybdsim.Plot), 93
+LossMap() (in module pybdsim.Plot), 94
 
 M
 Machine (class in pybdsim.Builder), 61
 MadxTfs2Gmad() (in module pybdsim.Convert), 69
 MadxTfs2Gmad()
 (in
 module
 pybdsim.Convert._MadxTfs2Gmad), 71
 MadxTfs2GmadBeam()
 (in
 module
 pybdsim.Convert._MadxTfs2Gmad), 73
 MadxTfs2GmadStrength() (in module pybdsim.Convert), 71
-MadxTfsBeta() (in module pybdsim.Plot), 93
+MadxTfsBeta() (in module pybdsim.Plot), 94
 MadxVsBDSIM() (in module pybdsim.Compare), 67
 MadxVsBDSIMOrbit() (in module pybdsim.Compare),
 68
 Marker (class in pybdsim.Builder), 65
 MatchValue()
 (pybdsim.Data.BDSAsciiData
 method), 73
 Material (class in pybdsim.Builder), 65
-MirrorDipoleQuadrant1() (in module pybdsim.Field._Field), 81
-ModelBDSIMXZ() (in module pybdsim.Plot), 93
-ModelBDSIMYZ() (in module pybdsim.Plot), 93
+MirrorDipoleQuadrant1() (in module pybdsim.Field._Field), 82
+ModelBDSIMXZ() (in module pybdsim.Plot), 94
+ModelBDSIMYZ() (in module pybdsim.Plot), 94
 ModelData (class in pybdsim.Data), 76
-ModelElegantXZ() (in module pybdsim.Plot), 93
-ModelElegantYZ() (in module pybdsim.Plot), 93
+ModelElegantXZ() (in module pybdsim.Plot), 94
+ModelElegantYZ() (in module pybdsim.Plot), 94
 module
 pybdsim, 57
 pybdsim.Beam, 57
 pybdsim.Builder, 58
 pybdsim.Compare, 67
 pybdsim.Constants, 68
 pybdsim.Convert, 68
 pybdsim.Convert._MadxTfs2Gmad, 71
 pybdsim.Data, 73
 pybdsim.Field, 80
 pybdsim.Field._Field, 80
 pybdsim.Field.FieldPlotter, 82
-pybdsim.Gmad, 85
-pybdsim.ModelProcessing, 87
-pybdsim.Options, 88
-pybdsim.Plot, 90
-pybdsim.Run, 95
-pybdsim.Visualisation, 96
+pybdsim.Gmad, 86
+pybdsim.ModelProcessing, 88
 110
 
+pybdsim.Options, 88
+pybdsim.Plot, 91
+pybdsim.Run, 96
+pybdsim.Visualisation, 97
 pybdsim.Writer, 97
-pybdsim.XSecBias, 99
+pybdsim.XSecBias, 100
 Multipole (class in pybdsim.Builder), 65
 MuSpoiler (class in pybdsim.Builder), 65
 
 N
 NameFromNearestS() (pybdsim.Data.BDSAsciiData
 method), 73
 NewColour (class in pybdsim.Builder), 65
 next() (pybdsim.Builder.Machine method), 65
-next() (pybdsim.Data.TrajectoryData method), 79
+next() (pybdsim.Data.TrajectoryData method), 80
 next() (pybdsim.Gmad.Lattice method), 87
 
 O
 Octupole (class in pybdsim.Builder), 65
 OneDData (class in pybdsim.Field.FieldPlotter), 82
 Options (class in pybdsim.Options), 88
 OptionsData (class in pybdsim.Data), 76
@@ -4657,72 +4655,72 @@
 86
 ParseLattice() (pybdsim.Gmad.Lattice method), 87
 ParseSpectraName() (in module pybdsim.Data), 76
 PhaseSpace() (in module pybdsim.Plot), 94
 PhaseSpaceData (class in pybdsim.Data), 76
 PhaseSpaceFromFile() (in module pybdsim.Plot), 94
 PhaseSpaceSeparateAxes() (in module pybdsim.Plot), 94
-PickleObject() (in module pybdsim.Data), 76
+PickleObject() (in module pybdsim.Data), 77
 Placement (class in pybdsim.Builder), 65
-Plot() (pybdsim.Gmad.Survey method), 87
+Plot() (pybdsim.Gmad.Survey method), 88
 Plot1DFxFyFz()
 (in
 module
 pybdsim.Field.FieldPlotter), 82
 Plot2D() (in module pybdsim.Field.FieldPlotter), 82
 Plot2DXY() (in module pybdsim.Field.FieldPlotter),
-82
+83
 Plot2DXYBx()
 (in
 module
 pybdsim.Field.FieldPlotter), 83
 Plot2DXYBy()
 (in
 module
 pybdsim.Field.FieldPlotter), 83
 Plot2DXYBz()
 (in
 module
-pybdsim.Field.FieldPlotter), 83
+pybdsim.Field.FieldPlotter), 84
 Plot2DXYComponent()
 (in
 module
-pybdsim.Field.FieldPlotter), 83
+pybdsim.Field.FieldPlotter), 84
 Plot2DXYConnectionOrder() (in module pybdsim.Field.FieldPlotter), 84
 Plot2DXYFxFyFz()
 (in
 module
 pybdsim.Field.FieldPlotter), 84
 Plot2DXYMagnitude()
 (in
 module
 pybdsim.Field.FieldPlotter), 84
+
+Index
+
+pybdsim Documentation, Release 3.3.0
+
 Plot2DXYStream()
 (in
 module
-pybdsim.Field.FieldPlotter), 84
+pybdsim.Field.FieldPlotter), 85
 Plot2DXZStream()
 (in
 module
-pybdsim.Field.FieldPlotter), 84
-
-Index
-
-pybdsim Documentation, Release 3.3.0
-
+pybdsim.Field.FieldPlotter), 85
 Plot3DXY() (in module pybdsim.Field.FieldPlotter),
 85
 Plot3DXZ() (in module pybdsim.Field.FieldPlotter),
 85
-PlotAlpha() (in module pybdsim.Plot), 94
-PlotBeta() (in module pybdsim.Plot), 94
-PlotDisp() (in module pybdsim.Plot), 94
-PlotDispP() (in module pybdsim.Plot), 94
-PlotMean() (in module pybdsim.Plot), 94
-PlotNPart() (in module pybdsim.Plot), 94
+PlotAlpha() (in module pybdsim.Plot), 95
+PlotBeta() (in module pybdsim.Plot), 95
+PlotDisp() (in module pybdsim.Plot), 95
+PlotDispP() (in module pybdsim.Plot), 95
+PlotMean() (in module pybdsim.Plot), 95
+PlotNPart() (in module pybdsim.Plot), 95
 PlotSigma() (in module pybdsim.Plot), 95
 PlotSigmaP() (in module pybdsim.Plot), 95
 PrepareApertureModel() (in module pybdsim.Builder), 65
 PrepareAxisAngleRotations()
 (pybdsim.Data.ModelData method), 76
 PrimaryPhaseSpace() (in module pybdsim.Plot), 95
 PrimarySurvival() (in module pybdsim.Plot), 95
@@ -4752,46 +4750,46 @@
 pybdsim.Field
 module, 80
 pybdsim.Field._Field
 module, 80
 pybdsim.Field.FieldPlotter
 module, 82
 pybdsim.Gmad
-module, 85
+module, 86
 pybdsim.ModelProcessing
-module, 87
+module, 88
 pybdsim.Options
 module, 88
-pybdsim.Plot
-module, 90
-pybdsim.Run
-module, 95
 
 Index
 
-pybdsim.Visualisation
+pybdsim.Plot
+module, 91
+pybdsim.Run
 module, 96
+pybdsim.Visualisation
+module, 97
 pybdsim.Writer
 module, 97
 pybdsim.XSecBias
-module, 99
+module, 100
 
 Q
 Quadrupole (class in pybdsim.Builder), 65
 Query (class in pybdsim.Builder), 65
 
 R
 RBend (class in pybdsim.Builder), 66
 RCol (class in pybdsim.Builder), 66
 Rebdsim() (in module pybdsim.Run), 96
 RebdsimCombine() (in module pybdsim.Run), 96
 RebdsimFile (class in pybdsim.Data), 77
 RebdsimHistoMerge() (in module pybdsim.Run), 96
 RebdsimOptics() (in module pybdsim.Run), 96
-RebdsimOrbit() (in module pybdsim.Run), 96
+RebdsimOrbit() (in module pybdsim.Run), 97
 Rebin() (pybdsim.Data.TH1 method), 78
 Rebin() (pybdsim.Data.TH2 method), 78
 RegenerateLenInt()
 (pybdsim.Builder.Machine
 method), 64
 Region (class in pybdsim.Builder), 66
 ReplaceElementCategory()
@@ -4809,172 +4807,175 @@
 ReturnBeamString() (pybdsim.Beam.Beam method),
 57
 ReturnOptionsString() (pybdsim.Options.Options
 method), 88
 RFCavity (class in pybdsim.Builder), 66
 Rmat (class in pybdsim.Builder), 66
 ROOTHist (class in pybdsim.Data), 77
-Run() (pybdsim.Run.Study method), 96
-RunExecOptions() (pybdsim.Run.Study method), 96
+Run() (pybdsim.Run.Study method), 97
+RunExecOptions() (pybdsim.Run.Study method), 97
 
 S
 Sampler (class in pybdsim.Builder), 66
 SamplerData (class in pybdsim.Data), 78
 SamplerPlacement (class in pybdsim.Builder), 66
 SBend (class in pybdsim.Builder), 66
 Scorer (class in pybdsim.Builder), 66
 ScorerMesh (class in pybdsim.Builder), 66
-SDDSBuildParameterDicts() (in module pybdsim.Data), 77
-SetBeamlineS() (pybdsim.Options.Options method),
-88
 
 111
 
 pybdsim Documentation, Release 3.3.0
 
-SetBeamPipeRadius()
+SDDSBuildParameterDicts() (in module pybd- SetLengthSafety()
 (pybdsim.Options.Options
+sim.Data), 78
+method), 89
+SetBeamlineS() (pybdsim.Options.Options method), SetLPBFraction()
+(pybdsim.Options.Options
+89
+method), 89
+SetBeamPipeRadius()
+(pybdsim.Options.Options SetMagnetGeometryType()
+(pybdmethod), 88
 sim.Options.Options method), 89
-method), 88
-SetMaximumEpsilonStep()
-(pybdSetBeamPipeThickness()
-(pybdsim.Options.Options method), 89
-sim.Options.Options method), 88
-SetMaximumStepLength()
-(pybdSetBLMLength() (pybdsim.Options.Options method),
+SetBeamPipeThickness()
+(pybd- SetMaximumEpsilonStep()
+(pybdsim.Options.Options method), 88
 sim.Options.Options method), 89
-88
-SetMaximumTrackingTime()
-(pybdSetBLMRadius() (pybdsim.Options.Options method),
+SetBLMLength() (pybdsim.Options.Options method), SetMaximumStepLength()
+(pybd88
 sim.Options.Options method), 89
-88
-SetMinimumEpsilonStep()
-(pybdSetBuildTunnel()
-(pybdsim.Options.Options
+SetBLMRadius() (pybdsim.Options.Options method), SetMaximumTrackingTime()
+(pybd88
 sim.Options.Options method), 89
-method), 88
-SetName() (pybdsim.XSecBias.XSecBias method), 99
-SetBuildTunnelFloor() (pybdsim.Options.Options SetNGenerate() (pybdsim.Options.Options method),
-method), 88
-89
+SetBuildTunnel()
+(pybdsim.Options.Options SetMinimumEpsilonStep()
+(pybdmethod), 89
+sim.Options.Options method), 89
+SetBuildTunnelFloor() (pybdsim.Options.Options SetName() (pybdsim.XSecBias.XSecBias method), 100
+method), 89
+SetNGenerate() (pybdsim.Options.Options method),
 SetCherenkovOn()
-(pybdsim.Options.Options SetNLinesIgnore()
 (pybdsim.Options.Options
-method), 88
-method), 89
-SetChordStepMinimum() (pybdsim.Options.Options SetNPerFile() (pybdsim.Options.Options method),
-method), 88
 89
-SetDefaultBiasMaterial()
-(pybd- SetOuterDiameter()
+method), 89
+SetNLinesIgnore()
 (pybdsim.Options.Options
-sim.Options.Options method), 88
+SetChordStepMinimum() (pybdsim.Options.Options
 method), 89
+method), 89
+SetNPerFile() (pybdsim.Options.Options method),
+SetDefaultBiasMaterial()
+(pybd89
+sim.Options.Options method), 89
+SetOuterDiameter()
+(pybdsim.Options.Options
 SetDefaultBiasVaccum()
-(pybd- SetParticle()
+(pybdmethod), 89
+sim.Options.Options method), 89
+SetParticle()
 (pybdsim.XSecBias.XSecBias
-sim.Options.Options method), 88
-method), 99
-SetDefaultRangeCut() (pybdsim.Options.Options SetParticleType() (pybdsim.Beam.Beam method),
-method), 88
-57
+SetDefaultRangeCut() (pybdsim.Options.Options
+method), 100
+method), 89
+SetParticleType() (pybdsim.Beam.Beam method),
 SetDeltaChord()
-(pybdsim.Options.Options SetPhysicsList()
 (pybdsim.Options.Options
-method), 88
+57
 method), 89
+SetPhysicsList()
+(pybdsim.Options.Options
 SetDeltaIntersection()
-(pybd- SetPipeMaterial()
+(pybdmethod), 89
+sim.Options.Options method), 89
+SetPipeMaterial()
 (pybdsim.Options.Options
-sim.Options.Options method), 88
-method), 89
 SetDeltaOneStep()
-(pybdsim.Options.Options SetPrintModuloFraction()
-(pybdmethod), 88
-sim.Options.Options method), 89
-SetDistributionType()
-(pybdsim.Beam.Beam SetProcesses()
-(pybdsim.XSecBias.XSecBias
+(pybdsim.Options.Options
+method), 90
+method), 89
+SetPrintModuloFraction()
+(pybdSetDistributionType()
+(pybdsim.Beam.Beam
+sim.Options.Options method), 90
 method), 57
-method), 99
-SetDontSplitSBends() (pybdsim.Options.Options SetProductionCutElectrons()
-(pybdmethod), 88
-sim.Options.Options method), 89
-SetE0() (pybdsim.Beam.Beam method), 57
-SetProductionCutPhotons()
-(pybdSetELossHistBinWidth()
+SetProcesses()
+(pybdsim.XSecBias.XSecBias
+SetDontSplitSBends() (pybdsim.Options.Options
+method), 100
+method), 89
+SetProductionCutElectrons()
+(pybdSetE0() (pybdsim.Beam.Beam method), 57
+sim.Options.Options method), 90
+SetELossHistBinWidth()
+(pybd- SetProductionCutPhotons()
 (pybdsim.Options.Options method), 89
-sim.Options.Options method), 88
-SetProductionCutPositrons()
-(pybdSetEMLeadParticleBiasing()
+sim.Options.Options method), 90
+SetEMLeadParticleBiasing()
+(pybd- SetProductionCutPositrons()
 (pybdsim.Options.Options method), 89
-sim.Options.Options method), 88
+sim.Options.Options method), 90
+SetEnergy() (pybdsim.Beam.Beam method), 57
 SetRandomSeed()
 (pybdsim.Options.Options
-SetEnergy() (pybdsim.Beam.Beam method), 57
-method), 89
-SetEPAnnihilation2HadronEnhancementFactor() SetS0() (pybdsim.Beam.Beam method), 58
-(pybdsim.Options.Options method), 88
-SetSamplerDiameter() (pybdsim.Options.Options
+SetEPAnnihilation2HadronEnhancementFactor()
+method), 90
+(pybdsim.Options.Options method), 89
+SetS0() (pybdsim.Beam.Beam method), 58
 SetEPAnnihilation2MuonEnhancementFactor()
-method), 89
-(pybdsim.Options.Options method), 88
-SetSensitiveBeamlineComponents()
-(pybdSetFlags() (pybdsim.XSecBias.XSecBias method), 99
-sim.Options.Options method), 89
+SetSamplerDiameter() (pybdsim.Options.Options
+(pybdsim.Options.Options method), 89
+method), 90
+SetFlags() (pybdsim.XSecBias.XSecBias method), SetSensitiveBeamlineComponents()
+(pybd100
+sim.Options.Options method), 90
 SetGamma2MuonEnahncementFactor()
 (pybd- SetSensitiveBeamPipe()
-(pybdsim.Options.Options method), 88
-sim.Options.Options method), 89
+(pybdsim.Options.Options method), 89
+sim.Options.Options method), 90
 SetGeneralOption()
 (pybdsim.Options.Options SetSenssitiveBLMs()
 (pybdsim.Options.Options
-method), 88
 method), 89
+method), 90
 SetIncludeFringeFields()
 (pybd- SetSoilMaterial()
 (pybdsim.Options.Options
-sim.Options.Options method), 88
-method), 89
+sim.Options.Options method), 89
+method), 90
 SetIncludeIronMagField()
 (pybd- SetSoilThickness()
 (pybdsim.Options.Options
 sim.Options.Options method), 89
-method), 89
+method), 90
 SetIntegratorSet()
-(pybdsim.Options.Options SetSRLowX() (pybdsim.Options.Options method), 89
+(pybdsim.Options.Options SetSRLowX() (pybdsim.Options.Options method), 90
 method), 89
 SetSRMultiplicity()
 (pybdsim.Options.Options
-SetLengthSafety()
-(pybdsim.Options.Options
-method), 89
-method), 89
-SetStopSecondaries() (pybdsim.Options.Options
-SetLPBFraction()
-(pybdsim.Options.Options
-method), 89
-method), 89
-SetStoreTrajectory() (pybdsim.Options.Options
-SetMagnetGeometryType()
-(pybdmethod), 89
 
 112
 
 Index
 
 pybdsim Documentation, Release 3.3.0
 
+method), 90
+SetStopSecondaries() (pybdsim.Options.Options
+method), 90
+SetStoreTrajectory() (pybdsim.Options.Options
+method), 90
 SetStoreTrajectoryParticle()
-(pybdsim.Options.Options method), 89
+(pybdsim.Options.Options method), 90
 SetSynchRadiationOn() (pybdsim.Options.Options
-method), 89
+method), 90
 SetT0() (pybdsim.Beam.Beam method), 58
 SetThresholdCutCharged()
-(pybdsim.Options.Options method), 89
+(pybdsim.Options.Options method), 90
 SetThresholdCutPhotons()
 (pybdsim.Options.Options method), 90
 SetTrackSRPhotons()
 (pybdsim.Options.Options
 method), 90
 SetTrajectoryCutGTZ() (pybdsim.Options.Options
 method), 90
@@ -5005,15 +5006,15 @@
 SetWritePrimaries()
 (pybdsim.Options.Options
 method), 90
 SetX0() (pybdsim.Beam.Beam method), 58
 SetXP0() (pybdsim.Beam.Beam method), 58
 SetXSecFactors()
 (pybdsim.XSecBias.XSecBias
-method), 99
+method), 100
 SetY0() (pybdsim.Beam.Beam method), 58
 SetYP0() (pybdsim.Beam.Beam method), 58
 SetZ0() (pybdsim.Beam.Beam method), 58
 SetZP0() (pybdsim.Beam.Beam method), 58
 Sextupole (class in pybdsim.Builder), 66
 Shield (class in pybdsim.Builder), 66
 Slice2DXY() (pybdsim.Data.TH3 method), 79
@@ -5022,25 +5023,25 @@
 Solenoid (class in pybdsim.Builder), 66
 SortByBin()
 (pybdsim.Data.Histogram1DSet
 method), 75
 SortUnorderedFieldMap2D() (in module pybdsim.Field._Field), 82
 Spectra (class in pybdsim.Data), 78
 Spectra() (in module pybdsim.Plot), 95
+
+Index
+
 split() (pybdsim.Builder.Element method), 60
 split() (pybdsim.Builder.HKicker method), 61
 split() (pybdsim.Builder.Kicker method), 61
 split() (pybdsim.Builder.Multipole method), 65
 split() (pybdsim.Builder.TKicker method), 67
-
-Index
-
 split() (pybdsim.Builder.VKicker method), 67
-Step() (pybdsim.Gmad.Survey method), 87
-Study (class in pybdsim.Run), 96
+Step() (pybdsim.Gmad.Survey method), 88
+Study (class in pybdsim.Run), 97
 SubplotsWithDrawnMachineLattice() (in module
 pybdsim.Plot), 95
 SuggestFodoK() (in module pybdsim.Builder), 66
 Survey (class in pybdsim.Gmad), 87
 SwapAxes() (pybdsim.Data.TH2 method), 78
 SynchrotronRadiationRescale()
 (pybdsim.Builder.Machine method), 64
@@ -5049,15 +5050,15 @@
 TH1 (class in pybdsim.Data), 78
 TH2 (class in pybdsim.Data), 78
 TH3 (class in pybdsim.Data), 78
 ThinMultipole (class in pybdsim.Builder), 67
 ThreeDData (class in pybdsim.Field.FieldPlotter), 85
 TKicker (class in pybdsim.Builder), 67
 ToDF() (pybdsim.Data.BDSAsciiData method), 74
-Trajectory3D() (in module pybdsim.Plot), 95
+Trajectory3D() (in module pybdsim.Plot), 96
 TrajectoryData (class in pybdsim.Data), 79
 Transform3D (class in pybdsim.Builder), 67
 TransportVsBDSIM() (in module pybdsim.Compare),
 68
 TRotationToAxisAngle() (in module pybdsim.Data), 79
 Tunnel (class in pybdsim.Builder), 67
 TwoDData (class in pybdsim.Field.FieldPlotter), 85
@@ -5076,54 +5077,54 @@
 (pybdsim.Builder.Machine method), 65
 
 V
 VKicker (class in pybdsim.Builder), 67
 
 W
 WireScanner (class in pybdsim.Builder), 67
-WrapLatticeAboutItem() (in module pybdsim.ModelProcessing), 87
+WrapLatticeAboutItem() (in module pybdsim.ModelProcessing), 88
 Write() (pybdsim.Builder.Machine method), 65
 Write() (pybdsim.Field._Field.Field method), 80
 write()
 (pybdsim.Gmad.GmadFileComponents
 method), 86
-WriteBeam() (pybdsim.Writer.Writer method), 98
-WriteBias() (pybdsim.Writer.Writer method), 98
-WriteComponents() (pybdsim.Writer.Writer method),
-98
-WriteFLUKA2DFormat1()
-(pybdsim.Field._Field.Field method), 80
-
+WriteASCII() (pybdsim.Data.TH3 method), 79
+WriteBeam() (pybdsim.Writer.Writer method), 99
 113
 
 pybdsim Documentation, Release 3.3.0
 
+WriteBias() (pybdsim.Writer.Writer method), 99
+WriteComponents() (pybdsim.Writer.Writer method),
+99
+WriteFLUKA2DFormat1()
+(pybdsim.Field._Field.Field method), 80
 WriteInMain() (pybdsim.Writer.FileSection method),
-97
-WriteMachine() (pybdsim.Writer.Writer method), 98
+98
+WriteMachine() (pybdsim.Writer.Writer method), 99
 WriteMain() (pybdsim.Writer.Writer method), 99
 WriteMaterial() (pybdsim.Writer.Writer method),
 99
 WriteObjects() (pybdsim.Writer.Writer method), 99
 WriteOptions() (pybdsim.Writer.Writer method), 99
-Writer (class in pybdsim.Writer), 97
+Writer (class in pybdsim.Writer), 98
 WriteROOTHistogramsToDirectory() (in module
-pybdsim.Data), 79
+pybdsim.Data), 80
 WriteSamplers() (pybdsim.Writer.Writer method),
 99
 WriteSeparately()
 (pybdsim.Writer.FileSection
-method), 97
+method), 98
 WriteSequence() (pybdsim.Writer.Writer method),
 99
 WriteToFile() (pybdsim.Beam.Beam method), 58
 
 X
 XSecBias (class in pybdsim.Builder), 67
-XSecBias (class in pybdsim.XSecBias), 99
+XSecBias (class in pybdsim.XSecBias), 100
 
 Z
 ZeroMissingRequiredColumns() (in module pybdsim.Convert._MadxTfs2Gmad), 73
 
 114
 
 Index
```

### Comparing `pybdsim-3.3.1/docs/source/builder.rst` & `pybdsim-3.3.2/docs/source/builder.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/classes.rst` & `pybdsim-3.3.2/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/compare.rst` & `pybdsim-3.3.2/docs/source/compare.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/conf.py` & `pybdsim-3.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/convert.rst` & `pybdsim-3.3.2/docs/source/convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/data.rst` & `pybdsim-3.3.2/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/data_uproot.rst` & `pybdsim-3.3.2/docs/source/data_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/developer.rst` & `pybdsim-3.3.2/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/fieldmaps.rst` & `pybdsim-3.3.2/docs/source/fieldmaps.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/figures/rebdsimFileHistograms.png` & `pybdsim-3.3.2/docs/source/figures/rebdsimFileHistograms.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/figures/rebdsimFileHistogramsWrapped.png` & `pybdsim-3.3.2/docs/source/figures/rebdsimFileHistogramsWrapped.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/figures/rebdsimFileMembers.png` & `pybdsim-3.3.2/docs/source/figures/rebdsimFileMembers.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/figures/simpleHistogramPlot.png` & `pybdsim-3.3.2/docs/source/figures/simpleHistogramPlot.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/installation.rst` & `pybdsim-3.3.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/licence.rst` & `pybdsim-3.3.2/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/moduledocs.rst` & `pybdsim-3.3.2/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/plotting.rst` & `pybdsim-3.3.2/docs/source/plotting.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/support.rst` & `pybdsim-3.3.2/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/docs/source/version_history.rst` & `pybdsim-3.3.2/docs/source/version_history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 ===============
 Version History
 ===============
 
+V3.3.2 - 2023 / 06 / 29
+=======================
+
+* Fix loading of new header variables with backwards compatibility.
+* Fix extra new lines and white space being written out in comments at the top
+  of field maps.
+* New function to write a 3D scoring mesh out as ASCII for transfer to
+  other programs.
+* Explicit exception when the ROOT libraries can't be loaded for reading
+  BDSIM data.
+* Fix circular import from Data.py and _General.py.
+
+
 V3.3.1 - 2023 / 05 / 15
 =======================
 
 * Reduce Python version requirement to >3.6 instead of 3.7.
 
 V3.3.0 - 2023 / 05 / 08
 =======================
```

### Comparing `pybdsim-3.3.1/examples/1_builder/1_testmachine.png` & `pybdsim-3.3.2/examples/1_builder/1_testmachine.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/1_madxtfs2gmad.png` & `pybdsim-3.3.2/examples/2_convert/1_madxtfs2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/2_convert.rst` & `pybdsim-3.3.2/examples/2_convert/2_convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/2_transport2gmad.png` & `pybdsim-3.3.2/examples/2_convert/2_transport2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/transport_example.dat` & `pybdsim-3.3.2/examples/2_convert/transport_example.dat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/transport_example.pdf` & `pybdsim-3.3.2/examples/2_convert/transport_example.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/twiss35tevb1_short.pdf` & `pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/2_convert/twiss35tevb1_short.tar.gz` & `pybdsim-3.3.2/examples/2_convert/twiss35tevb1_short.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/3_optics/optics_validation.py` & `pybdsim-3.3.2/examples/3_optics/optics_validation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/examples/4_uproot/4_uproot.rst` & `pybdsim-3.3.2/examples/4_uproot/4_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/pyproject.toml` & `pybdsim-3.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Beam.py` & `pybdsim-3.3.2/src/pybdsim/Beam.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Builder.py` & `pybdsim-3.3.2/src/pybdsim/Builder.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_BdsimBdsimComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_BdsimBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_ElegantBdsimComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_ElegantBdsimComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     fname = _pybdsim._General.GetFileName(bdsim) # cache file name
     if fname == "":
         fname = "optics_report"
 
     bdsData = _pybdsim.Data.Load(bdsim)
 
-    bdsinst = _pybdsim._General.CheckItsBDSAsciiData(bdsData, True)
+    bdsinst = _pybdsim.Data.CheckItsBDSAsciiData(bdsData, True)
     bdsopt  = _GetBDSIMOptics(bdsinst)
     survey  = bdsData.model if hasattr(bdsData, "model") else None
 
     eTwi = _LoadSDDSColumnsToDict(elegantTwiss)
     eSig = _LoadSDDSColumnsToDict(elegantSigma)
     eCen = _LoadSDDSColumnsToDict(elegantCentroid)
     eleopt  = _GetElegantOptics(eTwi,eSig,eCen,particleType)
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_Mad8BdsimComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle as _pkl
 import pylab as _pl
 import pymad8 as _m8
-import pybdsim as _bd
+import pybdsim as _pybdsim
 import matplotlib.pyplot as _plt
 import numpy as _np
 from os.path import isfile as _isfile
 from matplotlib.backends.backend_pdf import PdfPages as _PdfPages
 import datetime as _datetime
 
 # Predefined dicts for making the standard plots,
@@ -234,21 +234,21 @@
     """
 
     if not _isfile(twiss):
         raise IOError("File not found: ", twiss)
     if isinstance(bdsim, str) and not _isfile(bdsim):
         raise IOError("File not found: ", bdsim)
 
-    fname = _bd._General.GetFileName(bdsim)  # cache file name
+    fname = _pybdsim._General.GetFileName(bdsim)  # cache file name
     if fname == "":
         fname = "optics_report"
 
     # load mad8 optics and bdsim optics
     mad8opt = _m8.Output(twiss)
-    bdsinst = _bd._General.CheckItsBDSAsciiData(bdsim)
+    bdsinst = _pybdsim.Data.CheckItsBDSAsciiData(bdsim)
     bdsopt = _GetBDSIMOptics(bdsinst)
 
     # parameters required for calculating beam sizes, not written in mad8 output so have to supply manually.
     beamParams = {'esprd': energySpread, 'particle': particle, 'ex': ex, 'ey': ey}
 
     # make plots
     # energy and npart plotted with individual methods
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_MadxBdsimComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_MadxBdsimComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     _CheckFilesExist(tfs, bdsim, survey)
 
     fname = _pybdsim._General.GetFileName(bdsim) # cache file name
     if fname == "":
         fname = "optics_report"
 
     tfsinst = _pymadx.Data.CheckItsTfs(tfs)
-    bdsinst = _pybdsim._General.CheckItsBDSAsciiData(bdsim, True)
+    bdsinst = _pybdsim.Data.CheckItsBDSAsciiData(bdsim, True)
 
     tfsheader = tfsinst.header
     tfsopt  = _GetTfsOptics(tfsinst)
     bdsopt  = _GetBDSIMOptics(bdsinst)
 
     if survey is None:
         survey = tfsinst
@@ -108,15 +108,15 @@
 def PrepareResiduals(tfs, bds, survey=None, verbose=False):
     """
     Filter the tfs and bds to provide data that will match the 
     BDSIM data in element name. 
     """
     _CheckFilesExist(tfs, bds, survey)
     tfsinst   = _pymadx.Data.CheckItsTfs(tfs)
-    bdsinst   = _pybdsim._General.CheckItsBDSAsciiData(bds) # works for root files too
+    bdsinst   = _pybdsim.Data.CheckItsBDSAsciiData(bds) # works for root files too
 
     bdel    = bdsinst.orbit.elementName()
     bdslist = _np.array(bdel)
     tfsa  = tfsinst.GetColumn("NAME")
 
     keys = ['S', 'X', 'PX', 'Y', 'PY']
 
@@ -495,15 +495,15 @@
     Plot both the BDSIM orbit and MADX orbit (mean x,y).
 
     tfs - either file name or pymadx.Data.Tfs instance
     bds - filename or BDSAsciiData instance - rebdsimOrbit, rebdsimOptics output files
     """
     _CheckFilesExist(tfs, bds, survey)
     tfsopt = _pymadx.Data.CheckItsTfs(tfs)
-    bdsopt = _pybdsim._General.CheckItsBDSAsciiData(bds)
+    bdsopt = _pybdsim.Data.CheckItsBDSAsciiData(bds)
 
     if survey is None:
         survey = tfsopt
 
     orbitPlot = _plt.figure('Orbit', figsize=figsize)
     
     #tfs
@@ -542,15 +542,15 @@
 
     _plt.show(block=False)
     return orbitPlot
 
 def MadxVsBDSIMOrbitResiduals(tfs, bds, survey=None, functions=None, postfunctions=None, verbose=False, figsize=(12,5)):
     _CheckFilesExist(tfs, bds, survey)
     tfsinst   = _pymadx.Data.CheckItsTfs(tfs)
-    bdsinst   = _pybdsim._General.CheckItsBDSAsciiData(bds)
+    bdsinst   = _pybdsim.Data.CheckItsBDSAsciiData(bds)
     tfsd = PrepareResiduals(tfs, bds)
     tdata = tfsd[0]
     bdata = tfsd[1]
 
     if survey is None:
         survey = tfs
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_MultipleCodeComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_MultipleCodeComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pymadx as _pymadx
 import pybdsim as _pybdsim
 import matplotlib.pyplot as _plt
 import numpy as _np
 import os.path as _ospath
 from matplotlib.backends.backend_pdf import PdfPages as _PdfPages
 import datetime as _datetime
-from pybdsim._General import CheckItsBDSAsciiData, CheckBdsimDataHasSurveyModel
+from pybdsim.Data import CheckItsBDSAsciiData, CheckBdsimDataHasSurveyModel
 
 # Predefined dicts of variables for making the standard plots,
 # ptctwiss variables are the same as madx, ptc variables are the same as bdsim
 
 _BETA =    {"bdsimdata"  : ("Beta_x", "Beta_y"),
             "bdsimerror" : ("Sigma_Beta_x","Sigma_Beta_y"),
             "madx"       : ("BETX", "BETY"),
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_SadComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_SadComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/_TransportBdsimComparison.py` & `pybdsim-3.3.2/src/pybdsim/Compare/_TransportBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Compare/__init__.py` & `pybdsim-3.3.2/src/pybdsim/Compare/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Constants.py` & `pybdsim-3.3.2/src/pybdsim/Constants.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_CPyMad2Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_CPyMad2Gmad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations as _annotations
 from typing import Optional as _Optional
 from typing import Dict as _Dict
 from typing import Tuple as _Tuple
 from typing import MutableMapping as _MutableMapping
 from typing import Callable as _Callable
 from typing import TYPE_CHECKING as _TYPE_CHECKING
 import os as _os
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_ElegantParamToStrength.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_ElegantParamToStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_Mad8Saveline2Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Saveline2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_Mad8Twiss2Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_MadxTfs2Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_MadxTfs2GmadStrength.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_MadxTfs2GmadStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_Rebdsim2Numpy.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_Rebdsim2Numpy.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_SadFlat2Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_SadFlat2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/_Transport2Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Convert/_Transport2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/__init__.py` & `pybdsim-3.3.2/src/pybdsim/Convert/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Convert/collimator_analysis.py` & `pybdsim-3.3.2/src/pybdsim/Convert/collimator_analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Data.py` & `pybdsim-3.3.2/src/pybdsim/Data.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import glob as _glob
 import itertools as _itertools
 import math as _math
 import numpy as _np
 import re as _re
 import os as _os
 import pickle as _pickle
-import warnings as _warnings
 
 _useRoot      = True
 _libsLoaded   = False
 
 try:
     import ROOT as _ROOT
 except ImportError:
@@ -62,19 +61,22 @@
     except KeyError:
         pass
 
     # shared libraries
     bdsLoad = _ROOT.gSystem.Load("libbdsimRootEvent")
     reLoad  = _ROOT.gSystem.Load("librebdsim")
     # 0=ok, -1=fail, 1=already loaded
-    if reLoad < 0:
-        _warnings.warn("librebdsim not found")
-    if bdsLoad < 0:
-        _warnings.warn("libbdsimRootEvent not found")
-    _libsLoaded = True
+    if reLoad < 0 or bdsLoad < 0:
+        if reLoad < 0:
+            print("Warning: librebdsim not found")
+        if bdsLoad < 0:
+            print("Warning: libbdsimRootEvent not found")
+        _libsLoaded = False
+    else:
+        _libsLoaded = True
 
 def Load(filepath):
     """
     Load the data with the appropriate loader.
 
     ASCII file   - returns BDSAsciiData instance.
     BDSIM file   - uses ROOT, returns BDSIM DataLoader instance.
@@ -172,17 +174,19 @@
     return result
 
 def _LoadRoot(filepath):
     """
     Inspect file and check it's a BDSIM file of some kind and load.
     """
     if not _useRoot:
-        raise IOError("ROOT in python not available - can't load ROOT file")
+        raise IOError("ROOT in python not available - cannot load ROOT file")
 
     LoadROOTLibraries()
+    if not _libsLoaded:
+        raise IOError("BDSIM ROOT libraries not found - cannot load data - source bdsim.sh")
 
     fileType = _ROOTFileType(filepath) #throws warning if not a bdsim file
 
     if fileType == "BDSIM":
         print('BDSIM output file - using DataLoader')
         d = _ROOT.DataLoader(filepath)
         d.model = GetModelForPlotting(d) # attach BDSAsciiData instance for convenience
@@ -306,14 +310,18 @@
         self.fileType      = ""
         self.dataVersion   = -1
         self.analysedFiles = []
         self.combinedFiles = []
         self.trajectoryFilters = []
         self.skimmedFile   = False
         self.nOriginalEvents = 0
+        self.nEventsRequested = 0
+        self.nEventsInFileSkipped = 0
+        self.nEventsInFile = 0
+        self.distrFileLoopNTimes = 0
         if 'TFile' in kwargs:
             self._FillFromTFile(kwargs['TFile'])
         elif 'Header' in kwargs:
             self._Fill(kwargs['Header'])
         elif 'HeaderTree' in kwargs:
             self._FillFromHeaderTree(kwargs['HeaderTree'])
 
@@ -340,14 +348,17 @@
         self.fileType      = str(hi.fileType)
         self.dataVersion   = int(hi.dataVersion)
         self.analysedFiles = [str(s) for s in hi.analysedFiles]
         self.combinedFiles = [str(s) for s in hi.combinedFiles]
         self.trajectoryFilters = [str(s) for s in hi.trajectoryFilters]
         self.skimmedFile   = bool(hi.skimmedFile)
         self.nOriginalEvents = int(hi.nOriginalEvents)
+        for variable in ["nEventsRequested", "nEventsInFileSkipped", "nEventsInFile", "distrFileLoopNTimes"]:
+            if hasattr(hi, variable):
+                setattr(self, variable, int(getattr(hi, variable)))
 
 class Spectra:
     def __init__(self, nameIn=None):
         self.name = nameIn
         self.histograms = {}
         self.histogramspy = {}
         self.pdgids = set()
@@ -632,54 +643,54 @@
     def ConcatenateMachine(self, *args):
         """
         Add 1 or more data instances to this one - suitable only for things that
         could be loaded by this class. Argument can be one or iterable. Either
         of str type or this class.
         """
         #Get final position of the machine (different param for survey)
-        if _General.IsSurvey(self):
+        if IsSurvey(self):
             lastSpos = self.GetColumn('SEnd')[-1]
         else:
             lastSpos = self.GetColumn('S')[-1]
 
         for machine in args:
             if isinstance(machine,_np.str):
                 machine = Load(machine)
 
             #check names sets are equal
             if len(set(self.names).difference(set(machine.names))) != 0:
                 raise AttributeError("Cannot concatenate machine, variable names do not match")
 
             #surveys have multiple s positions per element
-            if _General.IsSurvey(machine):
+            if IsSurvey(machine):
                 sstartind = self.names.index('SStart')
                 smidind = self.names.index('SMid')
                 sendind = self.names.index('SEnd')
             elif self.names.count('S') != 0:
                 sind = self.names.index('S')
             else:
                 raise KeyError("S is not a variable in this data")
 
             #Have to convert each element to a list as tuples can't be modified
             for index in range(len(machine)):
                 element = machine.GetItemTuple(index)
                 elementlist = list(element)
 
                 #update the elements S position
-                if _General.IsSurvey(machine):
+                if IsSurvey(machine):
                     elementlist[sstartind] += lastSpos
                     elementlist[smidind] += lastSpos
                     elementlist[sendind] += lastSpos
                 else:
                     elementlist[sind] += lastSpos
 
                 self.append(tuple(elementlist))
 
             #update the total S position.
-            if _General.IsSurvey(machine):
+            if IsSurvey(machine):
                 lastSpos += machine.GetColumn('SEnd')[-1]
             else:
                 lastSpos += machine.GetColumn('S')[-1]
 
 
     def _AddProperty(self,variablename,variableunit='NA'):
         """
@@ -1170,14 +1181,50 @@
         """
         if not (0 <= index < self.nbinsz):
             raise ValueError("index must be in range [0 : "+str(self.nbinsz-1)+"]")
         self.hist.GetXaxis().SetRange(index+1,index+2)
         h2d = self.hist.Project3D("yze")
         return TH2(h2d)
 
+    def WriteASCII(self, filename, scalingFactor=1.0, comments=None):
+        """
+        Write the contents to a text file. Optionally multiply contents by a numerical factor.
+
+        :param filename: output name to write to - can optionally include .dat suffix.
+        :type filename: str
+        :param scalingFactor: numerical factor to multiply all contents by on writing out only.
+        :type scalingFactor: float
+        :param comments: list of comments to be written at the top of the file.
+        :type comments: list(str)
+        """
+        filename = str(filename)
+        if filename.endswith('.dat'):
+            filename = filename[:-4]
+        fn = filename + "_" + self.name + ".dat"
+        fo = open(fn, "w")
+        shape = self.contents.shape
+        if comments:
+            for comment in comments:
+                fo.write("# " + str(comment) + "\n")
+        fo.write("# scalingFactor: "+str(scalingFactor)+"\n")
+        fo.write("# " + "\t".join(["nx:", str(self.nbinsx), "xmin[m]:", str(self.xrange[0]), "xmax[m]:", str(self.xrange[1])]) + "\n")
+        fo.write("# " + "\t".join(["ny:", str(self.nbinsy), "ymin[m]:", str(self.yrange[0]), "ymax[m]:", str(self.yrange[1])]) + "\n")
+        fo.write("# " + "\t".join(["nz:", str(self.nbinsz), "zmin[m]:", str(self.zrange[0]), "zmax[m]:", str(self.zrange[1])]) + "\n")
+        columns = ['%18s' % s for s in ["x[m]", "y[m]", "z[m]", "Contents"]]
+        fo.write("!" + "\t".join(columns) + "\n")
+        for zi in range(shape[2]):
+            for yi in range(shape[1]):
+                for xi in range(shape[0]):
+                    value = [self.xcentres[xi], self.ycentres[yi], self.zcentres[zi], scalingFactor * self.contents[xi, yi, zi]]
+                    strings = ['%.8E' % x for x in value]
+                    stringsFW = ['%18s' % s for s in strings]
+                    fo.write("\t".join(stringsFW) + "\n")
+        fo.close()
+
+    
 class BDSBH4D():
     """
     Wrapper for a BDSBH instance. Converts to numpy data.
 
     """
     def __init__(self, hist, extractData=True):
         # these members are made to be the same as our "ROOTHist" class
@@ -2124,18 +2171,20 @@
 
     def _getData(self, interface, rootobj):
         for name in interface:
             setattr(self, name, getattr(rootobj, name))
 
 
 def _filterROOTObject(rootobj):
-    """Gets the names of the attributes which are just data and
-    specific to the class.  That is to say it removes all the
+    """
+    Gets the names of the attributes which are just data and
+    specific to the class. That is to say it removes all the
     clutter inherited from TObject, any methods, and some other
-    stuff.  Should retain strictly only the data."""
+    stuff. Should retain strictly only the data.
+    """
     # Define an instance of TObject which we can use to extract
     # the interface of our rootobj, leaving out all the rubbish.
     tobject_interface = set(dir(_ROOT.TObject()))
     rootobj_interface = set(dir(rootobj))
     interface = rootobj_interface.difference(tobject_interface)
 
     # remove other stuff
@@ -2217,7 +2266,69 @@
 
     # overwrite everything repeatedly for simplicity
     for en,et,pn,pv in zip(elementName,elementType,parameterName,parameterValue):
         result[en][pn] = pv
         result[en]['KEYWORD'] = et
 
     return result
+
+def GetFileName(ob):
+    if type(ob) == str:
+        return ob
+    elif type(ob) == RebdsimFile:
+        return ob.filename
+    elif type(ob) == BDSAsciiData:
+        return ob.filename
+    else:
+        return ""
+
+def CheckItsBDSAsciiData(bfile, requireOptics=False):
+    def CheckOptics(obj, requireOpticsL=False):
+        if hasattr(obj, 'Optics'):
+            return obj.Optics
+        elif hasattr(obj, 'optics'):
+            return obj.optics
+        else:
+            if requireOpticsL:
+                raise IOError("No optics found in pybdsim.Data.BDSAsciiData instance")
+            else:
+                return None
+
+    if type(bfile) == str:
+        data = Load(bfile)
+        data2 = CheckOptics(data, requireOptics)
+        if data2 is not None:
+            data = data2
+    elif type(bfile) == BDSAsciiData:
+        data = bfile
+    elif type(bfile) == RebdsimFile:
+        data = CheckOptics(bfile, requireOptics)
+    else:
+        raise IOError("Not pybdsim.Data.BDSAsciiData file type: " + str(bfile))
+    return data
+
+
+def CheckBdsimDataHasSurveyModel(bfile):
+    data = None
+    if isinstance(bfile, str):
+        data = Load(bfile)
+    elif type(bfile) == BDSAsciiData:
+        data = bfile
+    elif type(bfile) == RebdsimFile:
+        data = bfile
+    else:
+        data = bfile
+
+    return hasattr(data, "model")
+
+def IsSurvey(file):
+    """
+    Checks if input is a BDSIM generated survey
+    """
+    if isinstance(file,_np.str):
+        machine = Load(file)
+    elif isinstance(file, BDSAsciiData):
+        machine = file
+    else:
+        raise IOError("Unknown input type - not BDSIM data")
+
+    return machine.names.count('SStart') != 0
```

### Comparing `pybdsim-3.3.1/src/pybdsim/DataUproot.py` & `pybdsim-3.3.2/src/pybdsim/DataUproot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Field/FieldPlotter.py` & `pybdsim-3.3.2/src/pybdsim/Field/FieldPlotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,19 +348,19 @@
     else:
         _plt.streamplot(cx,cz,fx,fz,density=density)
     _Niceties('X (cm)', 'Z (cm)', zlabel="|$B_{x,z}$| (T)", aspect=aspect)
 
 def Plot2DXYConnectionOrder(filename):
     """
     Plot a point in orange and a line in blue (default matplotlib colours)
-    for each locationin the field map. If the field map is constructed
+    for each location in the field map. If the field map is constructed
     correctly, this should show a set of lines with diagonals between them.
     The other plots with the arrows are independent of order unlike when
     BDSIM loads the fields. So you might see an OK field map, but it could
-    be wrong if hand written.
+    be wrong if handwritten.
     """
     d = TwoDData(filename)
     _plt.figure()
     _plt.plot(d.x,d.y)
     _plt.plot(d.x,d.y,'.')
     _plt.xlabel('X (cm)')
     _plt.ylabel('Y (cm)')
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Field/FieldPlotterVtk.py` & `pybdsim-3.3.2/src/pybdsim/Field/FieldPlotterVtk.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Field/_Field.py` & `pybdsim-3.3.2/src/pybdsim/Field/_Field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import gzip as _gzip
 import numpy as _np
 import tarfile as _tarfile
-
+from copy import deepcopy as _deepcopy
 
 class Field(object):
     """
     Base class used for common writing procedures for BDSIM field format.
 
     This does not support arbitrary loop ordering - only the originally intended
     xyzt.
@@ -14,14 +14,38 @@
         self.data            = array
         self.columns         = columns
         self.header          = {}
         self.flip            = flip
         self.doublePrecision = doublePrecision
         self.nDimensions     = 0
         self.comments        = []
+    def __add__(field1, field2):
+        if field1.nDimensions == field2.nDimensions:
+            result = _deepcopy(field1)
+            result.data[..., result.nDimensions:] = field1.data[..., field1.nDimensions:] + field2.data[..., field2.nDimensions:]
+            return result
+        else:
+            raise ValueError("The two field maps do not have the same dimension!")
+        
+    def __mul__(field, scalingFactor):
+        result = _deepcopy(field)
+        result.data[..., result.nDimensions:] *= scalingFactor
+        return result
+
+    def __iadd__(self, field):
+        self = self + field
+
+    def __imul__(self, scalingFactor):
+        self = self * scalingFactor
+
+    def ScaleField(self, scalingFactor):
+        self *= scalingFactor
+
+    def AddField(self, field):
+        self += field
 
     def AddComment(self, commentString):
         """
         Add a string that will be put on a comment line at the beginning of the file.
         """
         self.comments.append(str(commentString))
         
@@ -47,15 +71,15 @@
         def write(fn, s):
             if compressed:
                 fn.write(s.encode('ascii'))
             else:
                 fn.write(s)
         write(f, "# units: cm, T\n")
         for comment in self.comments:
-            write(f, "# "+str(comment)+"\n")
+            write(f, "# "+str(comment).strip()+"\n")
         for key,value in self.header.items():
             write(f, str(key)+'> '+ str(value) + '\n')
         if overrideLoopOrder:
             if overrideLoopOrder not in ['xyzt', 'tzyx']:
                 raise ValueError("overrideLoopOrder must be one of 'xyzt', 'tzyx'")
             write(f, "loopOrder> "+overrideLoopOrder+"\n")
         else:
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Field/__init__.py` & `pybdsim-3.3.2/src/pybdsim/Field/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Geant4.py` & `pybdsim-3.3.2/src/pybdsim/Geant4.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Gmad.py` & `pybdsim-3.3.2/src/pybdsim/Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Joinhistograms.py` & `pybdsim-3.3.2/src/pybdsim/Joinhistograms.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/ModelProcessing.py` & `pybdsim-3.3.2/src/pybdsim/ModelProcessing.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Analysis.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Event.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Event.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Processed.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Processed.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/Root.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/Root.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Obsolete/Rebdsim/__init__.py` & `pybdsim-3.3.2/src/pybdsim/Obsolete/Rebdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Optics.py` & `pybdsim-3.3.2/src/pybdsim/Optics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Options.py` & `pybdsim-3.3.2/src/pybdsim/Options.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Plot.py` & `pybdsim-3.3.2/src/pybdsim/Plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import matplotlib.patches as _patches
 import numpy as _np
 import datetime as _datetime
 from matplotlib.backends.backend_pdf import PdfPages as _PdfPages
 from scipy import constants as _con
 import os.path as _ospath
 
-from ._General import CheckItsBDSAsciiData as _CheckItsBDSAsciiData
-from ._General import CheckBdsimDataHasSurveyModel as _CheckBdsimDataHasSurveyModel
+from .Data import CheckItsBDSAsciiData as _CheckItsBDSAsciiData
+from .Data import CheckBdsimDataHasSurveyModel as _CheckBdsimDataHasSurveyModel
 
 class _My_Axes(_matplotlib.axes.Axes):
     """
     Inherit matplotlib.axes.Axes but override pan action for mouse.
     Only allow horizontal panning - useful for lattice axes.
     """
     name = "_My_Axes"
```

### Comparing `pybdsim-3.3.1/src/pybdsim/Run.py` & `pybdsim-3.3.2/src/pybdsim/Run.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Testing/bdsimMadx.py` & `pybdsim-3.3.2/src/pybdsim/Testing/bdsimMadx.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Testing/trackingTester.py` & `pybdsim-3.3.2/src/pybdsim/Testing/trackingTester.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Visualisation.py` & `pybdsim-3.3.2/src/pybdsim/Visualisation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/Writer.py` & `pybdsim-3.3.2/src/pybdsim/Writer.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/XSecBias.py` & `pybdsim-3.3.2/src/pybdsim/XSecBias.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim/__init__.py` & `pybdsim-3.3.2/src/pybdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/src/pybdsim.egg-info/PKG-INFO` & `pybdsim-3.3.2/src/pybdsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.3.1
+Version: 3.3.2
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.3.1/src/pybdsim.egg-info/SOURCES.txt` & `pybdsim-3.3.2/src/pybdsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz` & `pybdsim-3.3.2/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_input/model-model-aper.tfs.gz` & `pybdsim-3.3.2/tests/test_input/model-model-aper.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_input/model-model.tfs.gz` & `pybdsim-3.3.2/tests/test_input/model-model.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.3.2/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output/model-model/model_components.gmad` & `pybdsim-3.3.2/tests/test_output/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output/model-model/model_sequence.gmad` & `pybdsim-3.3.2/tests/test_output/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.3.2/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output2/model-model/model_components.gmad` & `pybdsim-3.3.2/tests/test_output2/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/test_output2/model-model/model_sequence.gmad` & `pybdsim-3.3.2/tests/test_output2/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/tests/pybdsim_test_utils.py` & `pybdsim-3.3.2/tests/tests/pybdsim_test_utils.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/tests/test_MadxTfs2Gmad.py` & `pybdsim-3.3.2/tests/tests/test_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/tests/testratio.py` & `pybdsim-3.3.2/tests/tests/testratio.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/tests/write_test_outputs.py` & `pybdsim-3.3.2/tests/tests/write_test_outputs.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.3.1/tests/unit/test_Builder.py` & `pybdsim-3.3.2/tests/unit/test_Builder.py`

 * *Files identical despite different names*

