# Comparing `tmp/pyrocko-2023.6.29.tar.gz` & `tmp/pyrocko-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrocko-2023.6.29.tar", last modified: Thu Jun 29 21:45:37 2023, max compression
+gzip compressed data, was "pyrocko-2023.6.7.tar", last modified: Wed Jun  7 10:48:46 2023, max compression
```

## Comparing `pyrocko-2023.6.29.tar` & `pyrocko-2023.6.7.tar`

### file list

```diff
@@ -1,435 +1,435 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.820906 pyrocko-2023.6.29/
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/AUTHORS.md
--rw-r--r--   0 root         (0) root         (0)    23284 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     6789 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    32196 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-29 21:45:37.820906 pyrocko-2023.6.29/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/README.md
--rw-r--r--   0 root         (0) root         (0)   418072 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/evalresp-3.3.0.tar.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.744902 pyrocko-2023.6.29/extras/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/extras/fomosto
--rw-r--r--   0 root         (0) root         (0)     2184 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/extras/pyrocko
--rw-r--r--   0 root         (0) root         (0)      447 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/libmseed-2.19.6-fix-blkt-395-bswap.patch
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/libmseed-2.19.6-selection-fallthru.patch
--rw-r--r--   0 root         (0) root         (0)     5828 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/libmseed-2.19.6-speedread.patch
--rw-r--r--   0 root         (0) root         (0)   322651 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/libmseed-2.19.6.tar.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.744902 pyrocko-2023.6.29/maintenance/
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/maintenance/readme-pip.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.744902 pyrocko-2023.6.29/prerequisites/
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/prerequisites/prerequisites.bat
--rwxr-xr-x   0 root         (0) root         (0)      550 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/prerequisites/prerequisites.sh
--rwxr-xr-x   0 root         (0) root         (0)      319 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/prerequisites/prerequisites_arch_python3.sh
--rwxr-xr-x   0 root         (0) root         (0)      533 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/prerequisites/prerequisites_debian_python3.sh
--rwxr-xr-x   0 root         (0) root         (0)      312 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/prerequisites/prerequisites_opensuse_python3.sh
--rwxr-xr-x   0 root         (0) root         (0)      351 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/prerequisites/prerequisites_rpm_python3.sh
--rw-r--r--   0 root         (0) root         (0)     3030 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.744902 pyrocko-2023.6.29/pyrocko.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-29 21:45:37.000000 pyrocko-2023.6.29/pyrocko.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10548 2023-06-29 21:45:37.000000 pyrocko-2023.6.29/pyrocko.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 21:45:37.000000 pyrocko-2023.6.29/pyrocko.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-29 21:45:37.000000 pyrocko-2023.6.29/pyrocko.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-06-29 21:45:37.000000 pyrocko-2023.6.29/pyrocko.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-29 21:45:37.000000 pyrocko-2023.6.29/pyrocko.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-29 21:45:37.820906 pyrocko-2023.6.29/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    18566 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.748902 pyrocko-2023.6.29/src/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5215 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ahfullgreen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.752903 pyrocko-2023.6.29/src/apps/
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8408 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/automap.py
--rw-r--r--   0 root         (0) root         (0)    29520 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/cake.py
--rw-r--r--   0 root         (0) root         (0)     7497 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/colosseo.py
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/drum.py
--rwxr-xr-x   0 root         (0) root         (0)    38916 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/fomosto.py
--rwxr-xr-x   0 root         (0) root         (0)    21092 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/gmtpy-epstopdf
--rw-r--r--   0 root         (0) root         (0)     4338 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/hamster.py
--rwxr-xr-x   0 root         (0) root         (0)    19320 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/jackseis.py
--rw-r--r--   0 root         (0) root         (0)     2635 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/pyrocko.py
--rwxr-xr-x   0 root         (0) root         (0)      266 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/snuffler.py
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/sparrow.py
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/apps/squirrel.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/autopick.py
--rw-r--r--   0 root         (0) root         (0)   131029 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/cake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.752903 pyrocko-2023.6.29/src/client/
--rw-r--r--   0 root         (0) root         (0)      900 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/README.md
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/base_catalog.py
--rw-r--r--   0 root         (0) root         (0)      346 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/catalog.py
--rw-r--r--   0 root         (0) root         (0)    29155 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/fdsn.py
--rw-r--r--   0 root         (0) root         (0)     5791 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/geofon.py
--rw-r--r--   0 root         (0) root         (0)     6794 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/globalcmt.py
--rw-r--r--   0 root         (0) root         (0)     9929 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/iris.py
--rw-r--r--   0 root         (0) root         (0)     5535 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/isc.py
--rw-r--r--   0 root         (0) root         (0)     2547 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/saxony.py
--rw-r--r--   0 root         (0) root         (0)     3724 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/usgs.py
--rw-r--r--   0 root         (0) root         (0)    10013 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/client/wadl.py
--rw-r--r--   0 root         (0) root         (0)    12606 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/color.py
--rw-r--r--   0 root         (0) root         (0)     6430 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.752903 pyrocko-2023.6.29/src/data/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.756903 pyrocko-2023.6.29/src/data/colortables/
--rw-r--r--   0 root         (0) root         (0)      370 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/global_event_depth_1.cpt
--rw-r--r--   0 root         (0) root         (0)      356 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/global_event_depth_2.cpt
--rw-r--r--   0 root         (0) root         (0)      342 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/global_event_depth_3.cpt
--rw-r--r--   0 root         (0) root         (0)      667 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/light_land.cpt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/light_land_uniform.cpt
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/light_sea.cpt
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/light_sea_land.cpt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/light_sea_uniform.cpt
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/slip_colors.cpt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/colortables/white_sea_land.cpt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.756903 pyrocko-2023.6.29/src/data/earthmodels/
--rw-r--r--   0 root         (0) root         (0)    12720 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average-no-ocean.f.nd
--rw-r--r--   0 root         (0) root         (0)     2729 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average-no-ocean.l.nd
--rw-r--r--   0 root         (0) root         (0)     3899 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average-no-ocean.m.nd
--rw-r--r--   0 root         (0) root         (0)    13080 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.f.nd
--rw-r--r--   0 root         (0) root         (0)     3089 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.l.nd
--rw-r--r--   0 root         (0) root         (0)     4259 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.m.nd
--rw-r--r--   0 root         (0) root         (0)     6624 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.vf.nd
--rw-r--r--   0 root         (0) root         (0)    12566 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-continental.f.nd
--rw-r--r--   0 root         (0) root         (0)     2729 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-continental.l.nd
--rw-r--r--   0 root         (0) root         (0)     3899 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/ak135-f-continental.m.nd
--rw-r--r--   0 root         (0) root         (0)     4883 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/prem-no-ocean.f.nd
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/prem-no-ocean.l.nd
--rw-r--r--   0 root         (0) root         (0)     3449 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/prem-no-ocean.m.nd
--rw-r--r--   0 root         (0) root         (0)     5063 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/prem.f.nd
--rw-r--r--   0 root         (0) root         (0)     2819 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/prem.l.nd
--rw-r--r--   0 root         (0) root         (0)     3629 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/earthmodels/prem.m.nd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.756903 pyrocko-2023.6.29/src/data/fomosto_report/
--rw-r--r--   0 root         (0) root         (0)     3346 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/fomosto_report/gfreport.html
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/fomosto_report/gfreport.tex
--rw-r--r--   0 root         (0) root         (0)     6153 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/snuffler.png
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/snuffler_about.html
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/snuffler_help.html
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/snuffler_help_epilog.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.756903 pyrocko-2023.6.29/src/data/tectonics/
--rw-r--r--   0 root         (0) root         (0)      976 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/tectonics/bird2003_plates.txt
--rw-r--r--   0 root         (0) root         (0)      346 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/data/tectonics/gsrm1_plates.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.760903 pyrocko-2023.6.29/src/dataset/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/README.md
--rw-r--r--   0 root         (0) root         (0)      225 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3929 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/active_faults.py
--rw-r--r--   0 root         (0) root         (0)    12280 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/crust2x2.py
--rw-r--r--   0 root         (0) root         (0)    62738 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/crust2x2_data.py
--rwxr-xr-x   0 root         (0) root         (0)    35474 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/crustdb.py
--rw-r--r--   0 root         (0) root         (0)    21503 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/crustdb_abbr.py
--rw-r--r--   0 root         (0) root         (0)     4301 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/geonames.py
--rw-r--r--   0 root         (0) root         (0)    16408 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/gshhg.py
--rw-r--r--   0 root         (0) root         (0)    10783 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/tectonics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.760903 pyrocko-2023.6.29/src/dataset/topo/
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/topo/README.md
--rw-r--r--   0 root         (0) root         (0)     3773 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/topo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6916 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/topo/dataset.py
--rw-r--r--   0 root         (0) root         (0)     2848 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/topo/etopo1.py
--rw-r--r--   0 root         (0) root         (0)     4840 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/topo/srtmgl3.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/topo/tile.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/util.py
--rw-r--r--   0 root         (0) root         (0)     4953 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dataset/volcanoes.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/deps.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/dummy_progressbar.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/evalresp.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.760903 pyrocko-2023.6.29/src/ext/
--rw-r--r--   0 root         (0) root         (0)    12348 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/ahfullgreen_ext.c
--rw-r--r--   0 root         (0) root         (0)     5826 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/autopick_ext.c
--rw-r--r--   0 root         (0) root         (0)    13372 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/eikonal_ext.c
--rw-r--r--   0 root         (0) root         (0)     4859 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/evalresp_ext.c
--rw-r--r--   0 root         (0) root         (0)    14750 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/orthodrome_ext.c
--rw-r--r--   0 root         (0) root         (0)    17230 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/parstack_ext.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.760903 pyrocko-2023.6.29/src/ext/pyavl-1.12/
--rw-r--r--   0 root         (0) root         (0)     1095 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)       37 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/PROBLEMS
--rwxr-xr-x   0 root         (0) root         (0)     3173 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/README.md
--rwxr-xr-x   0 root         (0) root         (0)    49200 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/avl.c
--rwxr-xr-x   0 root         (0) root         (0)    12058 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/avl.h
--rwxr-xr-x   0 root         (0) root         (0)    40600 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/avlmodule.c
--rw-r--r--   0 root         (0) root         (0)   148027 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/pyavl-a4.pdf
--rwxr-xr-x   0 root         (0) root         (0)      307 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/pyavl-hysetup.tex
--rw-r--r--   0 root         (0) root         (0)    17645 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/pyavl.tex
--rw-r--r--   0 root         (0) root         (0)     2116 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/setup.py
--rwxr-xr-x   0 root         (0) root         (0)      439 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/test.make
--rwxr-xr-x   0 root         (0) root         (0)     8826 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/pyavl-1.12/test_avl.c
--rw-r--r--   0 root         (0) root         (0)     8355 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/signal_ext.c
--rw-r--r--   0 root         (0) root         (0)     6942 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/ext/util_ext.c
--rw-r--r--   0 root         (0) root         (0)    10706 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.764903 pyrocko-2023.6.29/src/fomosto/
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/README.md
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9223 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/ahfullgreen.py
--rw-r--r--   0 root         (0) root         (0)     3066 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/dummy.py
--rw-r--r--   0 root         (0) root         (0)    20951 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/poel.py
--rw-r--r--   0 root         (0) root         (0)    59975 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/psgrn_pscmp.py
--rw-r--r--   0 root         (0) root         (0)    40798 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/qseis.py
--rw-r--r--   0 root         (0) root         (0)    39770 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/qseis2d.py
--rw-r--r--   0 root         (0) root         (0)    43340 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/qssp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.764903 pyrocko-2023.6.29/src/fomosto/report/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19502 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/report/report_call.py
--rw-r--r--   0 root         (0) root         (0)    58247 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/fomosto/report/report_main.py
--rw-r--r--   0 root         (0) root         (0)     6778 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/geometry.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/get_terminal_size.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.764903 pyrocko-2023.6.29/src/gf/
--rw-r--r--   0 root         (0) root         (0)      827 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/README.md
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5936 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/builder.py
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.764903 pyrocko-2023.6.29/src/gf/ext/
--rw-r--r--   0 root         (0) root         (0)   101941 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/ext/store_ext.c
--rw-r--r--   0 root         (0) root         (0)    97256 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/meta.py
--rw-r--r--   0 root         (0) root         (0)   184332 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/seismosizer.py
--rw-r--r--   0 root         (0) root         (0)    25256 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/server.py
--rw-r--r--   0 root         (0) root         (0)    74441 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/store.py
--rw-r--r--   0 root         (0) root         (0)    13189 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/targets.py
--rw-r--r--   0 root         (0) root         (0)    12358 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/tractions.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gf/ws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.768903 pyrocko-2023.6.29/src/gui/
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/README.md
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.768903 pyrocko-2023.6.29/src/gui/drum/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/drum/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4027 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/drum/cli.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/drum/main.py
--rw-r--r--   0 root         (0) root         (0)     4114 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/drum/state.py
--rw-r--r--   0 root         (0) root         (0)    27611 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/drum/view.py
--rw-r--r--   0 root         (0) root         (0)     4214 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/moment_tensor_viewer.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/qt_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.768903 pyrocko-2023.6.29/src/gui/snuffler/
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25560 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/marker.py
--rw-r--r--   0 root         (0) root         (0)    26961 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/marker_editor.py
--rw-r--r--   0 root         (0) root         (0)   161620 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/pile_viewer.py
--rw-r--r--   0 root         (0) root         (0)     5816 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/pile_viewer_waterfall.py
--rw-r--r--   0 root         (0) root         (0)    10365 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snuffler.py
--rw-r--r--   0 root         (0) root         (0)    24471 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snuffler_app.py
--rw-r--r--   0 root         (0) root         (0)    61211 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snuffling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.772904 pyrocko-2023.6.29/src/gui/snuffler/snufflings/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/README.md
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5015 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/ampspec.py
--rw-r--r--   0 root         (0) root         (0)     7997 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/cake_phase.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/catalogs.py
--rw-r--r--   0 root         (0) root         (0)     5240 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/download.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/geofon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.772904 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/
--rw-r--r--   0 root         (0) root         (0)    15503 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/__init__.py
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/loadxmldoc.js
--rwxr-xr-x   0 root         (0) root         (0)    13362 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/map_googlemaps.html
--rw-r--r--   0 root         (0) root         (0)    19032 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/map_osm.html
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/map_util.js
--rw-r--r--   0 root         (0) root         (0)   164938 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/plates.kml
--rw-r--r--   0 root         (0) root         (0)     1129 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/xmlMarker.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/minmax.py
--rw-r--r--   0 root         (0) root         (0)    31892 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/polarization.py
--rw-r--r--   0 root         (0) root         (0)     5664 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/rms.py
--rw-r--r--   0 root         (0) root         (0)    16685 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/seismosizer.py
--rw-r--r--   0 root         (0) root         (0)    10792 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/spectrogram.py
--rw-r--r--   0 root         (0) root         (0)     8142 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/snuffler/snufflings/stalta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.772904 pyrocko-2023.6.29/src/gui/sparrow/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4685 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/cli.py
--rw-r--r--   0 root         (0) root         (0)    12260 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.800905 pyrocko-2023.6.29/src/gui/sparrow/elements/
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/active_faults.py
--rw-r--r--   0 root         (0) root         (0)    14031 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/axes_box.py
--rw-r--r--   0 root         (0) root         (0)    10862 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/base.py
--rw-r--r--   0 root         (0) root         (0)    13831 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/catalog.py
--rw-r--r--   0 root         (0) root         (0)     7473 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/coastlines.py
--rw-r--r--   0 root         (0) root         (0)     6052 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/crosshair.py
--rw-r--r--   0 root         (0) root         (0)     6200 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/custom_topo.py
--rw-r--r--   0 root         (0) root         (0)    15091 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/geometry.py
--rw-r--r--   0 root         (0) root         (0)     5950 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/grid.py
--rw-r--r--   0 root         (0) root         (0)     5719 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/hud.py
--rw-r--r--   0 root         (0) root         (0)     7290 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/icosphere.py
--rw-r--r--   0 root         (0) root         (0)     8267 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/kite_insar.py
--rw-r--r--   0 root         (0) root         (0)     5853 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/plates.py
--rw-r--r--   0 root         (0) root         (0)    19077 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/source.py
--rw-r--r--   0 root         (0) root         (0)     5596 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/spheroid.py
--rw-r--r--   0 root         (0) root         (0)     6984 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/stations.py
--rw-r--r--   0 root         (0) root         (0)    17247 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/table.py
--rw-r--r--   0 root         (0) root         (0)    14119 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/topo.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/elements/volcanoes.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/light.py
--rw-r--r--   0 root         (0) root         (0)    60547 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/main.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/overlays.py
--rw-r--r--   0 root         (0) root         (0)    25601 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/snapshots.py
--rw-r--r--   0 root         (0) root         (0)    16514 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/sparrow/state.py
--rw-r--r--   0 root         (0) root         (0)    15736 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/talkie.py
--rw-r--r--   0 root         (0) root         (0)    56954 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/util.py
--rw-r--r--   0 root         (0) root         (0)    25781 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/gui/vtk_util.py
--rw-r--r--   0 root         (0) root         (0)    66426 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/guts.py
--rw-r--r--   0 root         (0) root         (0)     4562 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/guts_agnostic.py
--rw-r--r--   0 root         (0) root         (0)     7536 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/guts_array.py
--rw-r--r--   0 root         (0) root         (0)     6749 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/hamster_pile.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/has_paths.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/himesh.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/icosphere.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.804905 pyrocko-2023.6.29/src/io/
--rw-r--r--   0 root         (0) root         (0)     2211 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/README.md
--rw-r--r--   0 root         (0) root         (0)     8432 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6068 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/css.py
--rw-r--r--   0 root         (0) root         (0)    22115 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/datacube.py
--rw-r--r--   0 root         (0) root         (0)     5545 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/enhanced_sacpz.py
--rw-r--r--   0 root         (0) root         (0)     5797 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/eventdata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.804905 pyrocko-2023.6.29/src/io/ext/
--rw-r--r--   0 root         (0) root         (0)    34750 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/ext/datacube_ext.c
--rw-r--r--   0 root         (0) root         (0)     9781 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/ext/ims_ext.c
--rw-r--r--   0 root         (0) root         (0)    16960 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/ext/mseed_ext.c
--rw-r--r--   0 root         (0) root         (0)     6930 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/gcf.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/gse1.py
--rw-r--r--   0 root         (0) root         (0)     2816 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/gse2.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/hdf5_idas.py
--rw-r--r--   0 root         (0) root         (0)    73588 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/ims.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/io_common.py
--rw-r--r--   0 root         (0) root         (0)     2896 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/kan.py
--rw-r--r--   0 root         (0) root         (0)     6258 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/mseed.py
--rw-r--r--   0 root         (0) root         (0)    37116 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/quakeml.py
--rw-r--r--   0 root         (0) root         (0)    13300 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/rdseed.py
--rw-r--r--   0 root         (0) root         (0)    17515 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/resp.py
--rw-r--r--   0 root         (0) root         (0)    14012 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/sac.py
--rw-r--r--   0 root         (0) root         (0)     7645 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/segy.py
--rw-r--r--   0 root         (0) root         (0)     9771 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/seisan_response.py
--rw-r--r--   0 root         (0) root         (0)     5007 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/seisan_waveform.py
--rw-r--r--   0 root         (0) root         (0)    80390 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/stationxml.py
--rw-r--r--   0 root         (0) root         (0)     8493 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/suds.py
--rw-r--r--   0 root         (0) root         (0)    20209 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/tdms_idas.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/io/yaff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.804905 pyrocko-2023.6.29/src/model/
--rw-r--r--   0 root         (0) root         (0)      383 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/README.md
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/content.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/event.py
--rw-r--r--   0 root         (0) root         (0)     5278 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/geometry.py
--rw-r--r--   0 root         (0) root         (0)     7997 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/gnss.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/location.py
--rw-r--r--   0 root         (0) root         (0)    17639 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/model/station.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.808905 pyrocko-2023.6.29/src/modelling/
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/modelling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7748 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/modelling/cracksol.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/modelling/eikonal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.808905 pyrocko-2023.6.29/src/modelling/ext/
--rw-r--r--   0 root         (0) root         (0)    40320 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/modelling/ext/okada_ext.c
--rw-r--r--   0 root         (0) root         (0)    20862 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/modelling/okada.py
--rw-r--r--   0 root         (0) root         (0)    32824 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/moment_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.808905 pyrocko-2023.6.29/src/obspy_compat/
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/obspy_compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12902 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/obspy_compat/base.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/obspy_compat/snuffling.py
--rw-r--r--   0 root         (0) root         (0)    44973 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/orthodrome.py
--rw-r--r--   0 root         (0) root         (0)     4730 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/parimap.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/parstack.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/pchain.py
--rw-r--r--   0 root         (0) root         (0)    50818 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/pile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.808905 pyrocko-2023.6.29/src/plot/
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/README.md
--rw-r--r--   0 root         (0) root         (0)    24761 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43745 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/automap.py
--rw-r--r--   0 root         (0) root         (0)    28241 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/beachball.py
--rw-r--r--   0 root         (0) root         (0)    21608 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/cake_plot.py
--rw-r--r--   0 root         (0) root         (0)     5812 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/cpt.py
--rw-r--r--   0 root         (0) root         (0)    14412 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/directivity.py
--rw-r--r--   0 root         (0) root         (0)    63995 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/dynamic_rupture.py
--rw-r--r--   0 root         (0) root         (0)   129444 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/gmtpy.py
--rw-r--r--   0 root         (0) root         (0)     2758 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/hudson.py
--rw-r--r--   0 root         (0) root         (0)    18905 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/response.py
--rw-r--r--   0 root         (0) root         (0)    30340 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/smartplot.py
--rw-r--r--   0 root         (0) root         (0)     5488 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/plot/terminal.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/print_version.py
--rw-r--r--   0 root         (0) root         (0)    10462 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/progress.py
--rw-r--r--   0 root         (0) root         (0)     6704 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/pz.py
--rw-r--r--   0 root         (0) root         (0)    24692 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.812905 pyrocko-2023.6.29/src/scenario/
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/base.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/collection.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/error.py
--rw-r--r--   0 root         (0) root         (0)    14611 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.812905 pyrocko-2023.6.29/src/scenario/sources/
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3146 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/sources/base.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/sources/dcsource.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/sources/pseudodynrupture.py
--rw-r--r--   0 root         (0) root         (0)     2742 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/sources/rectangularsource.py
--rw-r--r--   0 root         (0) root         (0)     6830 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/station.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.812905 pyrocko-2023.6.29/src/scenario/targets/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/targets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/targets/base.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/targets/gnss_campaign.py
--rw-r--r--   0 root         (0) root         (0)    16200 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/targets/insar.py
--rw-r--r--   0 root         (0) root         (0)    16424 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/targets/waveform.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/scenario/util.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/shadow_pile.py
--rw-r--r--   0 root         (0) root         (0)    16714 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/spit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.812905 pyrocko-2023.6.29/src/squirrel/
--rw-r--r--   0 root         (0) root         (0)      826 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111727 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/base.py
--rw-r--r--   0 root         (0) root         (0)     7628 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/cache.py
--rw-r--r--   0 root         (0) root         (0)    10220 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.812905 pyrocko-2023.6.29/src/squirrel/client/
--rw-r--r--   0 root         (0) root         (0)      341 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/client/base.py
--rw-r--r--   0 root         (0) root         (0)    10965 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/client/catalog.py
--rw-r--r--   0 root         (0) root         (0)    28507 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/client/fdsn.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/client/local.py
--rw-r--r--   0 root         (0) root         (0)    32856 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/database.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/dataset.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/environment.py
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.816906 pyrocko-2023.6.29/src/squirrel/io/
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.816906 pyrocko-2023.6.29/src/squirrel/io/backends/
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/datacube.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/mseed.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/sac.py
--rw-r--r--   0 root         (0) root         (0)     4481 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/stationxml.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/tdms_idas.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/textfiles.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/virtual.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/backends/yaml.py
--rw-r--r--   0 root         (0) root         (0)    13286 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/io/base.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/lock.py
--rw-r--r--   0 root         (0) root         (0)    46061 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.816906 pyrocko-2023.6.29/src/squirrel/operators/
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11029 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/operators/base.py
--rw-r--r--   0 root         (0) root         (0)    14057 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/pile.py
--rw-r--r--   0 root         (0) root         (0)    23075 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/selection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.816906 pyrocko-2023.6.29/src/squirrel/tool/
--rw-r--r--   0 root         (0) root         (0)      233 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3479 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.820906 pyrocko-2023.6.29/src/squirrel/tool/commands/
--rw-r--r--   0 root         (0) root         (0)      287 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/check.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/codes.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/coverage.py
--rw-r--r--   0 root         (0) root         (0)     4332 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/database.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/files.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/init.py
--rw-r--r--   0 root         (0) root         (0)    19902 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/jackseis.py
--rw-r--r--   0 root         (0) root         (0)     7378 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/jackseis_classic.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/nuts.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/operators.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/persistent.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/response.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/scan.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/snuffler.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/stationxml.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/summon.py
--rw-r--r--   0 root         (0) root         (0)     5595 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/template.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/commands/update.py
--rw-r--r--   0 root         (0) root         (0)    23094 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/squirrel/tool/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 21:45:37.820906 pyrocko-2023.6.29/src/streaming/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/streaming/README.md
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/streaming/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6088 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/streaming/datacube.py
--rw-r--r--   0 root         (0) root         (0)    15337 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/streaming/edl.py
--rw-r--r--   0 root         (0) root         (0)    16075 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/streaming/serial_hamster.py
--rw-r--r--   0 root         (0) root         (0)     3733 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/streaming/slink.py
--rw-r--r--   0 root         (0) root         (0)    16294 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/table.py
--rw-r--r--   0 root         (0) root         (0)   114799 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/trace.py
--rw-r--r--   0 root         (0) root         (0)    76673 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/util.py
--rw-r--r--   0 root         (0) root         (0)     3897 2023-06-29 21:45:35.000000 pyrocko-2023.6.29/src/weeding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.939187 pyrocko-2023.6.7/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/AUTHORS.md
+-rw-r--r--   0 root         (0) root         (0)    22512 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     6789 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    32196 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-06-07 10:48:46.939187 pyrocko-2023.6.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/README.md
+-rw-r--r--   0 root         (0) root         (0)   418072 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/evalresp-3.3.0.tar.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.879184 pyrocko-2023.6.7/extras/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/extras/fomosto
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/extras/pyrocko
+-rw-r--r--   0 root         (0) root         (0)      447 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/libmseed-2.19.6-fix-blkt-395-bswap.patch
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/libmseed-2.19.6-selection-fallthru.patch
+-rw-r--r--   0 root         (0) root         (0)     5828 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/libmseed-2.19.6-speedread.patch
+-rw-r--r--   0 root         (0) root         (0)   322651 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/libmseed-2.19.6.tar.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.879184 pyrocko-2023.6.7/maintenance/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/maintenance/readme-pip.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.879184 pyrocko-2023.6.7/prerequisites/
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/prerequisites/prerequisites.bat
+-rwxr-xr-x   0 root         (0) root         (0)      550 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/prerequisites/prerequisites.sh
+-rwxr-xr-x   0 root         (0) root         (0)      319 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/prerequisites/prerequisites_arch_python3.sh
+-rwxr-xr-x   0 root         (0) root         (0)      507 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/prerequisites/prerequisites_debian_python3.sh
+-rwxr-xr-x   0 root         (0) root         (0)      312 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/prerequisites/prerequisites_opensuse_python3.sh
+-rwxr-xr-x   0 root         (0) root         (0)      351 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/prerequisites/prerequisites_rpm_python3.sh
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.879184 pyrocko-2023.6.7/pyrocko.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-06-07 10:48:46.000000 pyrocko-2023.6.7/pyrocko.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-06-07 10:48:46.000000 pyrocko-2023.6.7/pyrocko.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 10:48:46.000000 pyrocko-2023.6.7/pyrocko.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-07 10:48:46.000000 pyrocko-2023.6.7/pyrocko.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-07 10:48:46.000000 pyrocko-2023.6.7/pyrocko.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-07 10:48:46.000000 pyrocko-2023.6.7/pyrocko.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-07 10:48:46.943187 pyrocko-2023.6.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    18566 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.887185 pyrocko-2023.6.7/src/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5215 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ahfullgreen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.891185 pyrocko-2023.6.7/src/apps/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8408 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/automap.py
+-rw-r--r--   0 root         (0) root         (0)    29520 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/cake.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/colosseo.py
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/drum.py
+-rwxr-xr-x   0 root         (0) root         (0)    38916 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/fomosto.py
+-rwxr-xr-x   0 root         (0) root         (0)    21092 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/gmtpy-epstopdf
+-rw-r--r--   0 root         (0) root         (0)     4338 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/hamster.py
+-rwxr-xr-x   0 root         (0) root         (0)    19320 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/jackseis.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/pyrocko.py
+-rwxr-xr-x   0 root         (0) root         (0)      266 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/snuffler.py
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/sparrow.py
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/apps/squirrel.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/autopick.py
+-rw-r--r--   0 root         (0) root         (0)   131029 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/cake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.891185 pyrocko-2023.6.7/src/client/
+-rw-r--r--   0 root         (0) root         (0)      900 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/README.md
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/base_catalog.py
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/catalog.py
+-rw-r--r--   0 root         (0) root         (0)    29155 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/fdsn.py
+-rw-r--r--   0 root         (0) root         (0)     5791 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/geofon.py
+-rw-r--r--   0 root         (0) root         (0)     6794 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/globalcmt.py
+-rw-r--r--   0 root         (0) root         (0)     9929 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/iris.py
+-rw-r--r--   0 root         (0) root         (0)     5535 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/isc.py
+-rw-r--r--   0 root         (0) root         (0)     2547 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/saxony.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/usgs.py
+-rw-r--r--   0 root         (0) root         (0)    10013 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/client/wadl.py
+-rw-r--r--   0 root         (0) root         (0)    12606 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/color.py
+-rw-r--r--   0 root         (0) root         (0)     6430 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.891185 pyrocko-2023.6.7/src/data/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.895185 pyrocko-2023.6.7/src/data/colortables/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/global_event_depth_1.cpt
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/global_event_depth_2.cpt
+-rw-r--r--   0 root         (0) root         (0)      342 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/global_event_depth_3.cpt
+-rw-r--r--   0 root         (0) root         (0)      667 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/light_land.cpt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/light_land_uniform.cpt
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/light_sea.cpt
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/light_sea_land.cpt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/light_sea_uniform.cpt
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/slip_colors.cpt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/colortables/white_sea_land.cpt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.895185 pyrocko-2023.6.7/src/data/earthmodels/
+-rw-r--r--   0 root         (0) root         (0)    12720 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average-no-ocean.f.nd
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average-no-ocean.l.nd
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average-no-ocean.m.nd
+-rw-r--r--   0 root         (0) root         (0)    13080 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.f.nd
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.l.nd
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.m.nd
+-rw-r--r--   0 root         (0) root         (0)     6624 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.vf.nd
+-rw-r--r--   0 root         (0) root         (0)    12566 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-continental.f.nd
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-continental.l.nd
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/ak135-f-continental.m.nd
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/prem-no-ocean.f.nd
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/prem-no-ocean.l.nd
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/prem-no-ocean.m.nd
+-rw-r--r--   0 root         (0) root         (0)     5063 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/prem.f.nd
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/prem.l.nd
+-rw-r--r--   0 root         (0) root         (0)     3629 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/earthmodels/prem.m.nd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.895185 pyrocko-2023.6.7/src/data/fomosto_report/
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/fomosto_report/gfreport.html
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/fomosto_report/gfreport.tex
+-rw-r--r--   0 root         (0) root         (0)     6153 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/snuffler.png
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/snuffler_about.html
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/snuffler_help.html
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/snuffler_help_epilog.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.895185 pyrocko-2023.6.7/src/data/tectonics/
+-rw-r--r--   0 root         (0) root         (0)      976 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/tectonics/bird2003_plates.txt
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/data/tectonics/gsrm1_plates.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.899185 pyrocko-2023.6.7/src/dataset/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/README.md
+-rw-r--r--   0 root         (0) root         (0)      225 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/active_faults.py
+-rw-r--r--   0 root         (0) root         (0)    12280 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/crust2x2.py
+-rw-r--r--   0 root         (0) root         (0)    62738 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/crust2x2_data.py
+-rwxr-xr-x   0 root         (0) root         (0)    35474 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/crustdb.py
+-rw-r--r--   0 root         (0) root         (0)    21503 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/crustdb_abbr.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/geonames.py
+-rw-r--r--   0 root         (0) root         (0)    16408 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/gshhg.py
+-rw-r--r--   0 root         (0) root         (0)    10783 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/tectonics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.899185 pyrocko-2023.6.7/src/dataset/topo/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/topo/README.md
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/topo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6916 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/topo/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/topo/etopo1.py
+-rw-r--r--   0 root         (0) root         (0)     4840 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/topo/srtmgl3.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/topo/tile.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/util.py
+-rw-r--r--   0 root         (0) root         (0)     4953 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dataset/volcanoes.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/deps.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/dummy_progressbar.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/evalresp.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.899185 pyrocko-2023.6.7/src/ext/
+-rw-r--r--   0 root         (0) root         (0)    12348 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/ahfullgreen_ext.c
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/autopick_ext.c
+-rw-r--r--   0 root         (0) root         (0)    13372 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/eikonal_ext.c
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/evalresp_ext.c
+-rw-r--r--   0 root         (0) root         (0)    14750 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/orthodrome_ext.c
+-rw-r--r--   0 root         (0) root         (0)    17230 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/parstack_ext.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.903185 pyrocko-2023.6.7/src/ext/pyavl-1.12/
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)       37 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/PROBLEMS
+-rwxr-xr-x   0 root         (0) root         (0)     3173 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/README.md
+-rwxr-xr-x   0 root         (0) root         (0)    49200 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/avl.c
+-rwxr-xr-x   0 root         (0) root         (0)    12058 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/avl.h
+-rwxr-xr-x   0 root         (0) root         (0)    40600 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/avlmodule.c
+-rw-r--r--   0 root         (0) root         (0)   148027 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/pyavl-a4.pdf
+-rwxr-xr-x   0 root         (0) root         (0)      307 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/pyavl-hysetup.tex
+-rw-r--r--   0 root         (0) root         (0)    17645 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/pyavl.tex
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)      439 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/test.make
+-rwxr-xr-x   0 root         (0) root         (0)     8826 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/pyavl-1.12/test_avl.c
+-rw-r--r--   0 root         (0) root         (0)     8355 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/signal_ext.c
+-rw-r--r--   0 root         (0) root         (0)     6942 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/ext/util_ext.c
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.903185 pyrocko-2023.6.7/src/fomosto/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/README.md
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9223 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/ahfullgreen.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    20951 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/poel.py
+-rw-r--r--   0 root         (0) root         (0)    59975 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/psgrn_pscmp.py
+-rw-r--r--   0 root         (0) root         (0)    40798 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/qseis.py
+-rw-r--r--   0 root         (0) root         (0)    39770 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/qseis2d.py
+-rw-r--r--   0 root         (0) root         (0)    43340 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/qssp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.903185 pyrocko-2023.6.7/src/fomosto/report/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19502 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/report/report_call.py
+-rw-r--r--   0 root         (0) root         (0)    58247 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/fomosto/report/report_main.py
+-rw-r--r--   0 root         (0) root         (0)     6778 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/get_terminal_size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.907186 pyrocko-2023.6.7/src/gf/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/README.md
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5936 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/builder.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.907186 pyrocko-2023.6.7/src/gf/ext/
+-rw-r--r--   0 root         (0) root         (0)   101941 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/ext/store_ext.c
+-rw-r--r--   0 root         (0) root         (0)    97265 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/meta.py
+-rw-r--r--   0 root         (0) root         (0)   184332 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/seismosizer.py
+-rw-r--r--   0 root         (0) root         (0)    25256 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/server.py
+-rw-r--r--   0 root         (0) root         (0)    74441 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/store.py
+-rw-r--r--   0 root         (0) root         (0)    13189 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/targets.py
+-rw-r--r--   0 root         (0) root         (0)    12358 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/tractions.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gf/ws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.907186 pyrocko-2023.6.7/src/gui/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/README.md
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.911186 pyrocko-2023.6.7/src/gui/drum/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/drum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4027 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/drum/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/drum/main.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/drum/state.py
+-rw-r--r--   0 root         (0) root         (0)    27611 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/drum/view.py
+-rw-r--r--   0 root         (0) root         (0)     4214 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/moment_tensor_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/qt_compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.911186 pyrocko-2023.6.7/src/gui/snuffler/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25560 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/marker.py
+-rw-r--r--   0 root         (0) root         (0)    26961 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/marker_editor.py
+-rw-r--r--   0 root         (0) root         (0)   161620 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/pile_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     5816 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/pile_viewer_waterfall.py
+-rw-r--r--   0 root         (0) root         (0)    10365 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snuffler.py
+-rw-r--r--   0 root         (0) root         (0)    24471 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snuffler_app.py
+-rw-r--r--   0 root         (0) root         (0)    61183 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snuffling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.915186 pyrocko-2023.6.7/src/gui/snuffler/snufflings/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/README.md
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5015 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/ampspec.py
+-rw-r--r--   0 root         (0) root         (0)     7997 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/cake_phase.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/catalogs.py
+-rw-r--r--   0 root         (0) root         (0)     5240 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/download.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/geofon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.915186 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/
+-rw-r--r--   0 root         (0) root         (0)    15503 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/loadxmldoc.js
+-rwxr-xr-x   0 root         (0) root         (0)    13362 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/map_googlemaps.html
+-rw-r--r--   0 root         (0) root         (0)    19032 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/map_osm.html
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/map_util.js
+-rw-r--r--   0 root         (0) root         (0)   164938 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/plates.kml
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/xmlMarker.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/minmax.py
+-rw-r--r--   0 root         (0) root         (0)    31892 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/polarization.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/rms.py
+-rw-r--r--   0 root         (0) root         (0)    16685 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/seismosizer.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/spectrogram.py
+-rw-r--r--   0 root         (0) root         (0)     7529 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/snuffler/snufflings/stalta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.915186 pyrocko-2023.6.7/src/gui/sparrow/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4685 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/cli.py
+-rw-r--r--   0 root         (0) root         (0)    12260 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.919186 pyrocko-2023.6.7/src/gui/sparrow/elements/
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/active_faults.py
+-rw-r--r--   0 root         (0) root         (0)    14031 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/axes_box.py
+-rw-r--r--   0 root         (0) root         (0)    10862 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/base.py
+-rw-r--r--   0 root         (0) root         (0)    13831 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7473 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/coastlines.py
+-rw-r--r--   0 root         (0) root         (0)     6052 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/crosshair.py
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/custom_topo.py
+-rw-r--r--   0 root         (0) root         (0)    15091 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     5950 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/grid.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/hud.py
+-rw-r--r--   0 root         (0) root         (0)     7290 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/icosphere.py
+-rw-r--r--   0 root         (0) root         (0)     8267 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/kite_insar.py
+-rw-r--r--   0 root         (0) root         (0)     5853 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/plates.py
+-rw-r--r--   0 root         (0) root         (0)    19077 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/source.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/spheroid.py
+-rw-r--r--   0 root         (0) root         (0)     6984 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/stations.py
+-rw-r--r--   0 root         (0) root         (0)    17247 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/table.py
+-rw-r--r--   0 root         (0) root         (0)    14119 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/topo.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/elements/volcanoes.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/light.py
+-rw-r--r--   0 root         (0) root         (0)    60547 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/main.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/overlays.py
+-rw-r--r--   0 root         (0) root         (0)    25601 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)    16514 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/sparrow/state.py
+-rw-r--r--   0 root         (0) root         (0)    15736 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/talkie.py
+-rw-r--r--   0 root         (0) root         (0)    56954 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/util.py
+-rw-r--r--   0 root         (0) root         (0)    25781 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/gui/vtk_util.py
+-rw-r--r--   0 root         (0) root         (0)    66426 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/guts.py
+-rw-r--r--   0 root         (0) root         (0)     4562 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/guts_agnostic.py
+-rw-r--r--   0 root         (0) root         (0)     7539 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/guts_array.py
+-rw-r--r--   0 root         (0) root         (0)     6749 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/hamster_pile.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/has_paths.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/himesh.py
+-rw-r--r--   0 root         (0) root         (0)     6404 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/icosphere.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.923186 pyrocko-2023.6.7/src/io/
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/README.md
+-rw-r--r--   0 root         (0) root         (0)     8432 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6068 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/css.py
+-rw-r--r--   0 root         (0) root         (0)    22115 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/datacube.py
+-rw-r--r--   0 root         (0) root         (0)     5545 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/enhanced_sacpz.py
+-rw-r--r--   0 root         (0) root         (0)     5797 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/eventdata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.923186 pyrocko-2023.6.7/src/io/ext/
+-rw-r--r--   0 root         (0) root         (0)    34750 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/ext/datacube_ext.c
+-rw-r--r--   0 root         (0) root         (0)     9781 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/ext/ims_ext.c
+-rw-r--r--   0 root         (0) root         (0)    16960 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/ext/mseed_ext.c
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/gcf.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/gse1.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/gse2.py
+-rw-r--r--   0 root         (0) root         (0)     4200 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/hdf5_idas.py
+-rw-r--r--   0 root         (0) root         (0)    73588 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/ims.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/io_common.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/kan.py
+-rw-r--r--   0 root         (0) root         (0)     6258 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/mseed.py
+-rw-r--r--   0 root         (0) root         (0)    37116 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/quakeml.py
+-rw-r--r--   0 root         (0) root         (0)    13300 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/rdseed.py
+-rw-r--r--   0 root         (0) root         (0)    17515 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/resp.py
+-rw-r--r--   0 root         (0) root         (0)    14012 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/sac.py
+-rw-r--r--   0 root         (0) root         (0)     7645 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/segy.py
+-rw-r--r--   0 root         (0) root         (0)     9771 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/seisan_response.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/seisan_waveform.py
+-rw-r--r--   0 root         (0) root         (0)    80390 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/stationxml.py
+-rw-r--r--   0 root         (0) root         (0)     8493 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/suds.py
+-rw-r--r--   0 root         (0) root         (0)    20209 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/tdms_idas.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/io/yaff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.923186 pyrocko-2023.6.7/src/model/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/README.md
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/content.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/event.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     7997 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/gnss.py
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/location.py
+-rw-r--r--   0 root         (0) root         (0)    17639 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/model/station.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.927187 pyrocko-2023.6.7/src/modelling/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/modelling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7748 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/modelling/cracksol.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/modelling/eikonal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.927187 pyrocko-2023.6.7/src/modelling/ext/
+-rw-r--r--   0 root         (0) root         (0)    40320 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/modelling/ext/okada_ext.c
+-rw-r--r--   0 root         (0) root         (0)    20862 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/modelling/okada.py
+-rw-r--r--   0 root         (0) root         (0)    32820 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/moment_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.927187 pyrocko-2023.6.7/src/obspy_compat/
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/obspy_compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12902 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/obspy_compat/base.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/obspy_compat/snuffling.py
+-rw-r--r--   0 root         (0) root         (0)    44973 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/orthodrome.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/parimap.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/parstack.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/pchain.py
+-rw-r--r--   0 root         (0) root         (0)    50818 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/pile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.927187 pyrocko-2023.6.7/src/plot/
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/README.md
+-rw-r--r--   0 root         (0) root         (0)    24761 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43745 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/automap.py
+-rw-r--r--   0 root         (0) root         (0)    27847 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/beachball.py
+-rw-r--r--   0 root         (0) root         (0)    21608 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/cake_plot.py
+-rw-r--r--   0 root         (0) root         (0)     5812 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/cpt.py
+-rw-r--r--   0 root         (0) root         (0)    14412 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/directivity.py
+-rw-r--r--   0 root         (0) root         (0)    63995 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/dynamic_rupture.py
+-rw-r--r--   0 root         (0) root         (0)   129444 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/gmtpy.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/hudson.py
+-rw-r--r--   0 root         (0) root         (0)    18905 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/response.py
+-rw-r--r--   0 root         (0) root         (0)    30238 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/smartplot.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/plot/terminal.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/print_version.py
+-rw-r--r--   0 root         (0) root         (0)    10462 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/progress.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/pz.py
+-rw-r--r--   0 root         (0) root         (0)    24695 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.931187 pyrocko-2023.6.7/src/scenario/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/base.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/collection.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/error.py
+-rw-r--r--   0 root         (0) root         (0)    14611 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.931187 pyrocko-2023.6.7/src/scenario/sources/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/sources/base.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/sources/dcsource.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/sources/pseudodynrupture.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/sources/rectangularsource.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/station.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.931187 pyrocko-2023.6.7/src/scenario/targets/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/targets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/targets/base.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/targets/gnss_campaign.py
+-rw-r--r--   0 root         (0) root         (0)    16200 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/targets/insar.py
+-rw-r--r--   0 root         (0) root         (0)    16424 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/targets/waveform.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/scenario/util.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/shadow_pile.py
+-rw-r--r--   0 root         (0) root         (0)    16720 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/spit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.935187 pyrocko-2023.6.7/src/squirrel/
+-rw-r--r--   0 root         (0) root         (0)      826 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109068 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/base.py
+-rw-r--r--   0 root         (0) root         (0)     7569 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/cache.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.935187 pyrocko-2023.6.7/src/squirrel/client/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/client/base.py
+-rw-r--r--   0 root         (0) root         (0)    10908 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/client/catalog.py
+-rw-r--r--   0 root         (0) root         (0)    28354 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/client/fdsn.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/client/local.py
+-rw-r--r--   0 root         (0) root         (0)    32856 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/database.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/environment.py
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.935187 pyrocko-2023.6.7/src/squirrel/io/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.935187 pyrocko-2023.6.7/src/squirrel/io/backends/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/datacube.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/mseed.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/sac.py
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/stationxml.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/tdms_idas.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/textfiles.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/virtual.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/backends/yaml.py
+-rw-r--r--   0 root         (0) root         (0)    13286 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/io/base.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/lock.py
+-rw-r--r--   0 root         (0) root         (0)    45885 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.935187 pyrocko-2023.6.7/src/squirrel/operators/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11029 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/operators/base.py
+-rw-r--r--   0 root         (0) root         (0)    14070 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/pile.py
+-rw-r--r--   0 root         (0) root         (0)    23075 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.935187 pyrocko-2023.6.7/src/squirrel/tool/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.939187 pyrocko-2023.6.7/src/squirrel/tool/commands/
+-rw-r--r--   0 root         (0) root         (0)      287 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/check.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/codes.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/coverage.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/database.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/files.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/init.py
+-rw-r--r--   0 root         (0) root         (0)    19902 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/jackseis.py
+-rw-r--r--   0 root         (0) root         (0)     7378 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/jackseis_classic.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/nuts.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/operators.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/persistent.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/response.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/scan.py
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/snuffler.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/stationxml.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/summon.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/template.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/commands/update.py
+-rw-r--r--   0 root         (0) root         (0)    23094 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/squirrel/tool/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:48:46.939187 pyrocko-2023.6.7/src/streaming/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/streaming/README.md
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/streaming/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/streaming/datacube.py
+-rw-r--r--   0 root         (0) root         (0)    15337 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/streaming/edl.py
+-rw-r--r--   0 root         (0) root         (0)    16075 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/streaming/serial_hamster.py
+-rw-r--r--   0 root         (0) root         (0)     3733 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/streaming/slink.py
+-rw-r--r--   0 root         (0) root         (0)    16294 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/table.py
+-rw-r--r--   0 root         (0) root         (0)   114799 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/trace.py
+-rw-r--r--   0 root         (0) root         (0)    76626 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/util.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-06-07 10:48:43.000000 pyrocko-2023.6.7/src/weeding.py
```

### Comparing `pyrocko-2023.6.29/AUTHORS.md` & `pyrocko-2023.6.7/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/CHANGELOG.md` & `pyrocko-2023.6.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,36 +4,14 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Unreleased
 
 *empty*
 
-## v2023.06.29
-
-### Added
-- Beachball example: explain syntetic polarity calulation.
-- Squirrel: support `now` in command line time arguments.
-
-### Changed
-- Disallow automatic downloads in `squirrel snuffler`.
-- Allow ignoring some errors when getting pyrocko stations.
-- Squirrel: improve behaviour when downloading close to real time data.
-
-### Fixed
-- Snuffler: improve robustness against broken snufflings.
-- Fix broken beachball.amplitudes which used incorrect units rad instead of 
-  deg.
-- Snufflings rms, spectrogram, stalta: filter ranges now adapt to data sampling
-  rates.
-- `squirrel snuffler`: fix crash due to incorrect pile emulation.
-- Squirrel: Fix crash when chopping over sequence without any waveforms.
-- Smartplot: fix tick label placement issues.
-
-
 ## v2023.06.07
 
 ### Added
 - The Sparrow.
 - Squirrel:
     - `squirrel jackseis`: add `--rename-*` options to change nslc codes.
     - `squirrel jackseis`: support more downsamling ratios.
```

### Comparing `pyrocko-2023.6.29/CONTRIBUTING.md` & `pyrocko-2023.6.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/LICENSE.md` & `pyrocko-2023.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/PKG-INFO` & `pyrocko-2023.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrocko
-Version: 2023.6.29
+Version: 2023.6.7
 Summary: A versatile seismology toolkit for Python.
 Home-page: https://pyrocko.org
 Author: The Pyrocko Developers
 Author-email: info@pyrocko.org
 License: GPLv3
 Description: Pyrocko is an open source seismology toolbox and library, written in the Python
         programming language. It can be utilized flexibly for a variety of geophysical
```

### Comparing `pyrocko-2023.6.29/README.md` & `pyrocko-2023.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/evalresp-3.3.0.tar.gz` & `pyrocko-2023.6.7/evalresp-3.3.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/extras/fomosto` & `pyrocko-2023.6.7/extras/fomosto`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/extras/pyrocko` & `pyrocko-2023.6.7/extras/pyrocko`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/libmseed-2.19.6-speedread.patch` & `pyrocko-2023.6.7/libmseed-2.19.6-speedread.patch`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/libmseed-2.19.6.tar.gz` & `pyrocko-2023.6.7/libmseed-2.19.6.tar.gz`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/maintenance/readme-pip.rst` & `pyrocko-2023.6.7/maintenance/readme-pip.rst`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/prerequisites/prerequisites.sh` & `pyrocko-2023.6.7/prerequisites/prerequisites.sh`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/pyproject.toml` & `pyrocko-2023.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "oldest-supported-numpy"]
 
 [project]
 name = "pyrocko"
-version = "2023.06.29"
+version = "2023.06.07"
 authors = [
     {name = "The Pyrocko Developers", email = "info@pyrocko.org"},
 ]
 maintainers = [
     {name = "Sebastian Heimann", email = "sebastian.heimann@uni-potsdam.de"}
 ]
 description = "A versatile seismology toolkit for Python."
```

### Comparing `pyrocko-2023.6.29/pyrocko.egg-info/PKG-INFO` & `pyrocko-2023.6.7/pyrocko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrocko
-Version: 2023.6.29
+Version: 2023.6.7
 Summary: A versatile seismology toolkit for Python.
 Home-page: https://pyrocko.org
 Author: The Pyrocko Developers
 Author-email: info@pyrocko.org
 License: GPLv3
 Description: Pyrocko is an open source seismology toolbox and library, written in the Python
         programming language. It can be utilized flexibly for a variety of geophysical
```

### Comparing `pyrocko-2023.6.29/pyrocko.egg-info/SOURCES.txt` & `pyrocko-2023.6.7/pyrocko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/setup.py` & `pyrocko-2023.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools.command.build_ext import build_ext
 
 is_windows = sys.platform.startswith('win')
 
 have_pep621_support = pv(setuptools_version) >= pv('61.0.0')
 
 packname = 'pyrocko'
-version = '2023.06.29'
+version = '2023.06.07'
 
 
 def get_numpy_include():
     import numpy
     return numpy.get_include()
```

### Comparing `pyrocko-2023.6.29/src/__init__.py` & `pyrocko-2023.6.7/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ahfullgreen.py` & `pyrocko-2023.6.7/src/ahfullgreen.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/automap.py` & `pyrocko-2023.6.7/src/apps/automap.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/cake.py` & `pyrocko-2023.6.7/src/apps/cake.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/colosseo.py` & `pyrocko-2023.6.7/src/apps/colosseo.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/fomosto.py` & `pyrocko-2023.6.7/src/apps/fomosto.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/gmtpy-epstopdf` & `pyrocko-2023.6.7/src/apps/gmtpy-epstopdf`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/hamster.py` & `pyrocko-2023.6.7/src/apps/hamster.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/jackseis.py` & `pyrocko-2023.6.7/src/apps/jackseis.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/apps/pyrocko.py` & `pyrocko-2023.6.7/src/apps/pyrocko.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/autopick.py` & `pyrocko-2023.6.7/src/autopick.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/cake.py` & `pyrocko-2023.6.7/src/cake.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/README.md` & `pyrocko-2023.6.7/src/client/README.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/base_catalog.py` & `pyrocko-2023.6.7/src/client/base_catalog.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/fdsn.py` & `pyrocko-2023.6.7/src/client/fdsn.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/geofon.py` & `pyrocko-2023.6.7/src/client/geofon.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/globalcmt.py` & `pyrocko-2023.6.7/src/client/globalcmt.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/iris.py` & `pyrocko-2023.6.7/src/client/iris.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/isc.py` & `pyrocko-2023.6.7/src/client/isc.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/saxony.py` & `pyrocko-2023.6.7/src/client/saxony.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/usgs.py` & `pyrocko-2023.6.7/src/client/usgs.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/client/wadl.py` & `pyrocko-2023.6.7/src/client/wadl.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/color.py` & `pyrocko-2023.6.7/src/color.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/config.py` & `pyrocko-2023.6.7/src/config.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/colortables/light_land.cpt` & `pyrocko-2023.6.7/src/data/colortables/light_land.cpt`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/colortables/light_sea_land.cpt` & `pyrocko-2023.6.7/src/data/colortables/light_sea_land.cpt`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/colortables/slip_colors.cpt` & `pyrocko-2023.6.7/src/data/colortables/slip_colors.cpt`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average-no-ocean.f.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average-no-ocean.f.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average-no-ocean.l.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average-no-ocean.l.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average-no-ocean.m.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average-no-ocean.m.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.f.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.f.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.l.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.l.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.m.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.m.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-average.vf.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-average.vf.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-continental.f.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-continental.f.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-continental.l.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-continental.l.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/ak135-f-continental.m.nd` & `pyrocko-2023.6.7/src/data/earthmodels/ak135-f-continental.m.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/prem-no-ocean.f.nd` & `pyrocko-2023.6.7/src/data/earthmodels/prem-no-ocean.f.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/prem-no-ocean.l.nd` & `pyrocko-2023.6.7/src/data/earthmodels/prem-no-ocean.l.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/prem-no-ocean.m.nd` & `pyrocko-2023.6.7/src/data/earthmodels/prem-no-ocean.m.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/prem.f.nd` & `pyrocko-2023.6.7/src/data/earthmodels/prem.f.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/prem.l.nd` & `pyrocko-2023.6.7/src/data/earthmodels/prem.l.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/earthmodels/prem.m.nd` & `pyrocko-2023.6.7/src/data/earthmodels/prem.m.nd`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/fomosto_report/gfreport.html` & `pyrocko-2023.6.7/src/data/fomosto_report/gfreport.html`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/fomosto_report/gfreport.tex` & `pyrocko-2023.6.7/src/data/fomosto_report/gfreport.tex`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/snuffler.png` & `pyrocko-2023.6.7/src/data/snuffler.png`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/snuffler_about.html` & `pyrocko-2023.6.7/src/data/snuffler_about.html`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/snuffler_help.html` & `pyrocko-2023.6.7/src/data/snuffler_help.html`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/data/tectonics/bird2003_plates.txt` & `pyrocko-2023.6.7/src/data/tectonics/bird2003_plates.txt`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/README.md` & `pyrocko-2023.6.7/src/dataset/README.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/active_faults.py` & `pyrocko-2023.6.7/src/dataset/active_faults.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/crust2x2.py` & `pyrocko-2023.6.7/src/dataset/crust2x2.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/crust2x2_data.py` & `pyrocko-2023.6.7/src/dataset/crust2x2_data.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/crustdb.py` & `pyrocko-2023.6.7/src/dataset/crustdb.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/crustdb_abbr.py` & `pyrocko-2023.6.7/src/dataset/crustdb_abbr.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/geonames.py` & `pyrocko-2023.6.7/src/dataset/geonames.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/gshhg.py` & `pyrocko-2023.6.7/src/dataset/gshhg.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/tectonics.py` & `pyrocko-2023.6.7/src/dataset/tectonics.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/topo/__init__.py` & `pyrocko-2023.6.7/src/dataset/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/topo/dataset.py` & `pyrocko-2023.6.7/src/dataset/topo/dataset.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/topo/etopo1.py` & `pyrocko-2023.6.7/src/dataset/topo/etopo1.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/topo/srtmgl3.py` & `pyrocko-2023.6.7/src/dataset/topo/srtmgl3.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/topo/tile.py` & `pyrocko-2023.6.7/src/dataset/topo/tile.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/util.py` & `pyrocko-2023.6.7/src/dataset/util.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dataset/volcanoes.py` & `pyrocko-2023.6.7/src/dataset/volcanoes.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/deps.py` & `pyrocko-2023.6.7/src/deps.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/dummy_progressbar.py` & `pyrocko-2023.6.7/src/dummy_progressbar.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/evalresp.py` & `pyrocko-2023.6.7/src/evalresp.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/example.py` & `pyrocko-2023.6.7/src/example.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/ahfullgreen_ext.c` & `pyrocko-2023.6.7/src/ext/ahfullgreen_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/autopick_ext.c` & `pyrocko-2023.6.7/src/ext/autopick_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/eikonal_ext.c` & `pyrocko-2023.6.7/src/ext/eikonal_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/evalresp_ext.c` & `pyrocko-2023.6.7/src/ext/evalresp_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/orthodrome_ext.c` & `pyrocko-2023.6.7/src/ext/orthodrome_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/parstack_ext.c` & `pyrocko-2023.6.7/src/ext/parstack_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/PKG-INFO` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/README.md` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/README.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/avl.c` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/avl.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/avl.h` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/avl.h`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/avlmodule.c` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/avlmodule.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/pyavl-a4.pdf` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/pyavl-a4.pdf`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/pyavl.tex` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/pyavl.tex`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/setup.py` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/setup.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/pyavl-1.12/test_avl.c` & `pyrocko-2023.6.7/src/ext/pyavl-1.12/test_avl.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/signal_ext.c` & `pyrocko-2023.6.7/src/ext/signal_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/ext/util_ext.c` & `pyrocko-2023.6.7/src/ext/util_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/file.py` & `pyrocko-2023.6.7/src/file.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/ahfullgreen.py` & `pyrocko-2023.6.7/src/fomosto/ahfullgreen.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/dummy.py` & `pyrocko-2023.6.7/src/fomosto/dummy.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/poel.py` & `pyrocko-2023.6.7/src/fomosto/poel.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/psgrn_pscmp.py` & `pyrocko-2023.6.7/src/fomosto/psgrn_pscmp.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/qseis.py` & `pyrocko-2023.6.7/src/fomosto/qseis.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/qseis2d.py` & `pyrocko-2023.6.7/src/fomosto/qseis2d.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/qssp.py` & `pyrocko-2023.6.7/src/fomosto/qssp.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/report/report_call.py` & `pyrocko-2023.6.7/src/fomosto/report/report_call.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/fomosto/report/report_main.py` & `pyrocko-2023.6.7/src/fomosto/report/report_main.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/geometry.py` & `pyrocko-2023.6.7/src/geometry.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/get_terminal_size.py` & `pyrocko-2023.6.7/src/get_terminal_size.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/README.md` & `pyrocko-2023.6.7/src/gf/README.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/builder.py` & `pyrocko-2023.6.7/src/gf/builder.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/ext/store_ext.c` & `pyrocko-2023.6.7/src/gf/ext/store_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/meta.py` & `pyrocko-2023.6.7/src/gf/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -2058,15 +2058,15 @@
         self.deltas = num.array(
             [self.source_depth_delta, self.distance_delta],
             dtype=float)
         self.ns = num.floor((self.maxs - self.mins) / self.deltas +
                             vicinity_eps).astype(int) + 1
         self.effective_maxs = self.mins + self.deltas * (self.ns - 1)
         self.deltat = 1.0/self.sample_rate
-        self.nrecords = num.prod(self.ns) * self.ncomponents
+        self.nrecords = num.product(self.ns) * self.ncomponents
         self.coords = tuple(num.linspace(mi, ma, n) for
                             (mi, ma, n) in
                             zip(self.mins, self.effective_maxs, self.ns)) + \
             (num.arange(self.ncomponents),)
 
         self.nsource_depths, self.ndistances = self.ns
 
@@ -2323,15 +2323,15 @@
             self.distance_delta],
             dtype=float)
 
         self.ns = num.floor((self.maxs - self.mins) / self.deltas +
                             vicinity_eps).astype(int) + 1
         self.effective_maxs = self.mins + self.deltas * (self.ns - 1)
         self.deltat = 1.0/self.sample_rate
-        self.nrecords = num.prod(self.ns) * self.ncomponents
+        self.nrecords = num.product(self.ns) * self.ncomponents
         self.coords = tuple(num.linspace(mi, ma, n) for
                             (mi, ma, n) in
                             zip(self.mins, self.effective_maxs, self.ns)) + \
             (num.arange(self.ncomponents),)
         self.nreceiver_depths, self.nsource_depths, self.ndistances = self.ns
 
     def _make_index_functions(self):
@@ -2651,15 +2651,15 @@
             self.source_north_shift_delta],
             dtype=float)
 
         self.ns = num.floor((self.maxs - self.mins) / self.deltas +
                             vicinity_eps).astype(int) + 1
         self.effective_maxs = self.mins + self.deltas * (self.ns - 1)
         self.deltat = 1.0/self.sample_rate
-        self.nrecords = num.prod(self.ns) * self.ncomponents
+        self.nrecords = num.product(self.ns) * self.ncomponents
 
         self.coords = tuple(
             num.linspace(mi, ma, n) for (mi, ma, n) in
             zip(self.mins, self.effective_maxs, self.ns)) + \
             (num.arange(self.ncomponents),)
 
     def _make_index_functions(self):
```

### Comparing `pyrocko-2023.6.29/src/gf/seismosizer.py` & `pyrocko-2023.6.7/src/gf/seismosizer.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/server.py` & `pyrocko-2023.6.7/src/gf/server.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/store.py` & `pyrocko-2023.6.7/src/gf/store.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/targets.py` & `pyrocko-2023.6.7/src/gf/targets.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/tractions.py` & `pyrocko-2023.6.7/src/gf/tractions.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gf/ws.py` & `pyrocko-2023.6.7/src/gf/ws.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/drum/cli.py` & `pyrocko-2023.6.7/src/gui/drum/cli.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/drum/main.py` & `pyrocko-2023.6.7/src/gui/drum/main.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/drum/state.py` & `pyrocko-2023.6.7/src/gui/drum/state.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/drum/view.py` & `pyrocko-2023.6.7/src/gui/drum/view.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/moment_tensor_viewer.py` & `pyrocko-2023.6.7/src/gui/moment_tensor_viewer.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/qt_compat.py` & `pyrocko-2023.6.7/src/gui/qt_compat.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/marker.py` & `pyrocko-2023.6.7/src/gui/snuffler/marker.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/marker_editor.py` & `pyrocko-2023.6.7/src/gui/snuffler/marker_editor.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/pile_viewer.py` & `pyrocko-2023.6.7/src/gui/snuffler/pile_viewer.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/pile_viewer_waterfall.py` & `pyrocko-2023.6.7/src/gui/snuffler/pile_viewer_waterfall.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snuffler.py` & `pyrocko-2023.6.7/src/gui/snuffler/snuffler.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snuffler_app.py` & `pyrocko-2023.6.7/src/gui/snuffler/snuffler_app.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snuffling.py` & `pyrocko-2023.6.7/src/gui/snuffler/snuffling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1836,15 +1836,15 @@
                 self._module = __import__(self._name)
                 del sys.modules[self._name]
 
                 for snuffling in self._module.__snufflings__():
                     snuffling._filename = filename
                     self.add_snuffling(snuffling)
 
-            except (Exception, SystemExit):
+            except Exception:
                 logger.error(traceback.format_exc())
                 raise BrokenSnufflingModule(filename)
 
             finally:
                 sys.path[0:1] = []
 
         elif self._mtime != mtime:
@@ -1862,15 +1862,15 @@
                     snuffling._filename = filename
                     self.add_snuffling(snuffling, reloaded=True)
 
                 if len(self._snufflings) == len(settings):
                     for sett, snuf in zip(settings, self._snufflings):
                         snuf.set_settings(sett)
 
-            except (Exception, SystemExit):
+            except Exception:
                 logger.error(traceback.format_exc())
                 raise BrokenSnufflingModule(filename)
 
             finally:
                 sys.path[0:1] = []
 
         self._mtime = mtime
```

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/__init__.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/ampspec.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/ampspec.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/cake_phase.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/cake_phase.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/catalogs.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/catalogs.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/download.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/download.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/geofon.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/geofon.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/__init__.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/map_googlemaps.html` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/map_googlemaps.html`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/map_osm.html` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/map_osm.html`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/map_util.js` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/map_util.js`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/plates.kml` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/plates.kml`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/map/xmlMarker.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/map/xmlMarker.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/minmax.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/minmax.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/polarization.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/polarization.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/rms.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/rms.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,31 +47,14 @@
             'Log RMS', 'log', False))
 
         self.add_trigger(
             'Copy passband from Main', self.copy_passband)
 
         self.set_live_update(False)
 
-    def panel_visibility_changed(self, visible):
-        viewer = self.get_viewer()
-        if visible:
-            viewer.pile_has_changed_signal.connect(self.adjust_controls)
-            self.adjust_controls()
-
-        else:
-            viewer.pile_has_changed_signal.disconnect(self.adjust_controls)
-
-    def adjust_controls(self):
-        viewer = self.get_viewer()
-        dtmin, dtmax = viewer.content_deltat_range()
-        maxfreq = 0.5/dtmin
-        minfreq = (0.5/dtmax)*0.001
-        self.set_parameter_range('lowpass', minfreq, maxfreq)
-        self.set_parameter_range('highpass', minfreq, maxfreq)
-
     def copy_passband(self):
         viewer = self.get_viewer()
         self.set_parameter('lowpass', viewer.lowpass)
         self.set_parameter('highpass', viewer.highpass)
 
     def call(self):
         '''
```

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/seismosizer.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/seismosizer.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/spectrogram.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/spectrogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,31 +89,14 @@
 
         self.set_live_update(False)
         self._tapers = {}
         self.nt_max = 2000
         self.nf_max = 500
         self.iframe = 0
 
-    def panel_visibility_changed(self, visible):
-        viewer = self.get_viewer()
-        if visible:
-            viewer.pile_has_changed_signal.connect(self.adjust_controls)
-            self.adjust_controls()
-
-        else:
-            viewer.pile_has_changed_signal.disconnect(self.adjust_controls)
-
-    def adjust_controls(self):
-        viewer = self.get_viewer()
-        dtmin, dtmax = viewer.content_deltat_range()
-        maxfreq = 0.5/dtmin
-        minfreq = (0.5/dtmax)*0.001
-        self.set_parameter_range('fmin', minfreq, maxfreq)
-        self.set_parameter_range('fmax', minfreq, maxfreq)
-
     def get_taper(self, name, n):
 
         taper_key = (name, n)
 
         if taper_key not in self._tapers:
             self._tapers[taper_key] = name_to_taper[name](n)
 
@@ -132,15 +115,15 @@
 
         if self.fmin is not None:
             ifmin = int(math.ceil(self.fmin / df))
         else:
             ifmin = 0
 
         if self.fmax is not None:
-            ifmax = min(int(math.floor(self.fmax / df)) + 1, nf)
+            ifmax = int(math.floor(self.fmax / df)) + 1
         else:
             ifmax = nf
 
         nf_show = ifmax - ifmin
         assert nf_show >= 2
 
         nf_show_ds, nf_mean = downsample_plan(nf_show, self.nf_max)
```

### Comparing `pyrocko-2023.6.29/src/gui/snuffler/snufflings/stalta.py` & `pyrocko-2023.6.7/src/gui/snuffler/snufflings/stalta.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,31 +97,14 @@
             Switch('Detect on sum trace', 'apply_to_sum', False))
 
         self.add_trigger(
             'Copy passband from Main', self.copy_passband)
 
         self.set_live_update(False)
 
-    def panel_visibility_changed(self, visible):
-        viewer = self.get_viewer()
-        if visible:
-            viewer.pile_has_changed_signal.connect(self.adjust_controls)
-            self.adjust_controls()
-
-        else:
-            viewer.pile_has_changed_signal.disconnect(self.adjust_controls)
-
-    def adjust_controls(self):
-        viewer = self.get_viewer()
-        dtmin, dtmax = viewer.content_deltat_range()
-        maxfreq = 0.5/dtmin
-        minfreq = (0.5/dtmax)*0.001
-        self.set_parameter_range('lowpass', minfreq, maxfreq)
-        self.set_parameter_range('highpass', minfreq, maxfreq)
-
     def copy_passband(self):
         viewer = self.get_viewer()
         self.set_parameter('lowpass', viewer.lowpass)
         self.set_parameter('highpass', viewer.highpass)
 
     def call(self):
         '''
```

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/cli.py` & `pyrocko-2023.6.7/src/gui/sparrow/cli.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/common.py` & `pyrocko-2023.6.7/src/gui/sparrow/common.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/__init__.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/active_faults.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/active_faults.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/axes_box.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/axes_box.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/base.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/catalog.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/catalog.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/coastlines.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/coastlines.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/crosshair.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/crosshair.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/custom_topo.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/custom_topo.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/geometry.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/geometry.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/grid.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/grid.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/hud.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/hud.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/icosphere.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/icosphere.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/kite_insar.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/kite_insar.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/plates.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/plates.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/source.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/source.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/spheroid.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/spheroid.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/stations.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/stations.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/table.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/table.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/topo.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/topo.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/elements/volcanoes.py` & `pyrocko-2023.6.7/src/gui/sparrow/elements/volcanoes.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/light.py` & `pyrocko-2023.6.7/src/gui/sparrow/light.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/main.py` & `pyrocko-2023.6.7/src/gui/sparrow/main.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/overlays.py` & `pyrocko-2023.6.7/src/gui/sparrow/overlays.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/snapshots.py` & `pyrocko-2023.6.7/src/gui/sparrow/snapshots.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/sparrow/state.py` & `pyrocko-2023.6.7/src/gui/sparrow/state.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/talkie.py` & `pyrocko-2023.6.7/src/gui/talkie.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/util.py` & `pyrocko-2023.6.7/src/gui/util.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/gui/vtk_util.py` & `pyrocko-2023.6.7/src/gui/vtk_util.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/guts.py` & `pyrocko-2023.6.7/src/guts.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/guts_agnostic.py` & `pyrocko-2023.6.7/src/guts_agnostic.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/guts_array.py` & `pyrocko-2023.6.7/src/guts_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
                     dtype = self.dtype or \
                         restricted_dtype_map_rev[serialize_dtype]
 
                     val = num.frombuffer(
                         data, dtype=serialize_dtype).astype(dtype)
 
-                    if val.size != num.prod(shape):
+                    if val.size != num.product(shape):
                         raise ValidationError('size/shape mismatch')
 
                     val = val.reshape(shape)
 
             else:
                 val = num.asarray(val, dtype=self.dtype)
```

### Comparing `pyrocko-2023.6.29/src/hamster_pile.py` & `pyrocko-2023.6.7/src/hamster_pile.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/has_paths.py` & `pyrocko-2023.6.7/src/has_paths.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/himesh.py` & `pyrocko-2023.6.7/src/himesh.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/icosphere.py` & `pyrocko-2023.6.7/src/icosphere.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/README.md` & `pyrocko-2023.6.7/src/io/README.md`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/__init__.py` & `pyrocko-2023.6.7/src/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/css.py` & `pyrocko-2023.6.7/src/io/css.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/datacube.py` & `pyrocko-2023.6.7/src/io/datacube.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/enhanced_sacpz.py` & `pyrocko-2023.6.7/src/io/enhanced_sacpz.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/eventdata.py` & `pyrocko-2023.6.7/src/io/eventdata.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/ext/datacube_ext.c` & `pyrocko-2023.6.7/src/io/ext/datacube_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/ext/ims_ext.c` & `pyrocko-2023.6.7/src/io/ext/ims_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/ext/mseed_ext.c` & `pyrocko-2023.6.7/src/io/ext/mseed_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/gcf.py` & `pyrocko-2023.6.7/src/io/gcf.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/gse1.py` & `pyrocko-2023.6.7/src/io/gse1.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/gse2.py` & `pyrocko-2023.6.7/src/io/gse2.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/hdf5_idas.py` & `pyrocko-2023.6.7/src/io/hdf5_idas.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/ims.py` & `pyrocko-2023.6.7/src/io/ims.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/io_common.py` & `pyrocko-2023.6.7/src/io/io_common.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/kan.py` & `pyrocko-2023.6.7/src/io/kan.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/mseed.py` & `pyrocko-2023.6.7/src/io/mseed.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/quakeml.py` & `pyrocko-2023.6.7/src/io/quakeml.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/rdseed.py` & `pyrocko-2023.6.7/src/io/rdseed.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/resp.py` & `pyrocko-2023.6.7/src/io/resp.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/sac.py` & `pyrocko-2023.6.7/src/io/sac.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/segy.py` & `pyrocko-2023.6.7/src/io/segy.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/seisan_response.py` & `pyrocko-2023.6.7/src/io/seisan_response.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/seisan_waveform.py` & `pyrocko-2023.6.7/src/io/seisan_waveform.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/stationxml.py` & `pyrocko-2023.6.7/src/io/stationxml.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/suds.py` & `pyrocko-2023.6.7/src/io/suds.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/tdms_idas.py` & `pyrocko-2023.6.7/src/io/tdms_idas.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/io/yaff.py` & `pyrocko-2023.6.7/src/io/yaff.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/model/content.py` & `pyrocko-2023.6.7/src/model/content.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/model/event.py` & `pyrocko-2023.6.7/src/model/event.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/model/geometry.py` & `pyrocko-2023.6.7/src/model/geometry.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/model/gnss.py` & `pyrocko-2023.6.7/src/model/gnss.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/model/location.py` & `pyrocko-2023.6.7/src/model/location.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/model/station.py` & `pyrocko-2023.6.7/src/model/station.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/modelling/cracksol.py` & `pyrocko-2023.6.7/src/modelling/cracksol.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/modelling/eikonal.py` & `pyrocko-2023.6.7/src/modelling/eikonal.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/modelling/ext/okada_ext.c` & `pyrocko-2023.6.7/src/modelling/ext/okada_ext.c`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/modelling/okada.py` & `pyrocko-2023.6.7/src/modelling/okada.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/moment_tensor.py` & `pyrocko-2023.6.7/src/moment_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
     ez = cvec(0., 0., 1.)
     exs = num.dot(rotmat.T, ex)
     ezs = num.dot(rotmat.T, ez)
     enodes = num.cross(ez.T, ezs.T).T
     if num.linalg.norm(enodes) < 1e-10:
         enodes = exs
     enodess = num.dot(rotmat, enodes)
-    cos_alpha = float(num.dot(ez.T, ezs)[0, 0])
+    cos_alpha = float((num.dot(ez.T, ezs)))
     if cos_alpha > 1.:
         cos_alpha = 1.
 
     if cos_alpha < -1.:
         cos_alpha = -1.
 
     alpha = math.acos(cos_alpha)
```

### Comparing `pyrocko-2023.6.29/src/obspy_compat/base.py` & `pyrocko-2023.6.7/src/obspy_compat/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/obspy_compat/snuffling.py` & `pyrocko-2023.6.7/src/obspy_compat/snuffling.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/orthodrome.py` & `pyrocko-2023.6.7/src/orthodrome.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/parimap.py` & `pyrocko-2023.6.7/src/parimap.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/parstack.py` & `pyrocko-2023.6.7/src/parstack.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/pchain.py` & `pyrocko-2023.6.7/src/pchain.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/pile.py` & `pyrocko-2023.6.7/src/pile.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/__init__.py` & `pyrocko-2023.6.7/src/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/automap.py` & `pyrocko-2023.6.7/src/plot/automap.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/beachball.py` & `pyrocko-2023.6.7/src/plot/beachball.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,32 +625,18 @@
     rtp = numpy_xyz2rtp(vecs_e)
     atheta, aphi = rtp[:, 1], rtp[:, 2]
     return ep * num.cos(atheta)**2 + (
         en * num.cos(aphi)**2 + et * num.sin(aphi)**2) * num.sin(atheta)**2
 
 
 def amplitudes(mt, azimuths, takeoff_angles):
-    '''
-    Get beachball amplitude values for selected azimuths and takeoff angles.
-
-    :param azimuths:
-        Azimuths, measured clockwise from north [deg].
-    :type azimuths:
-        :py:class:`~numpy.ndarray`
-
-    :param takeoff_angles:
-        Takeoff angles, measured from downward vertical [deg].
-    :type takeoff_angles:
-        :py:class:`~numpy.ndarray`
-    '''
     azimuths = num.asarray(azimuths, dtype=float)
     takeoff_angles = num.asarray(takeoff_angles, dtype=float)
     assert azimuths.size == takeoff_angles.size
-    rtps = num.vstack(
-        (num.ones(azimuths.size), takeoff_angles*d2r, azimuths*d2r)).T
+    rtps = num.vstack((num.ones(azimuths.size), takeoff_angles, azimuths)).T
     vecs = numpy_rtp2xyz(rtps)
     return amplitudes_ned(mt, vecs)
 
 
 def mts2amps(
         mts,
         projection,
```

### Comparing `pyrocko-2023.6.29/src/plot/cake_plot.py` & `pyrocko-2023.6.7/src/plot/cake_plot.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/cpt.py` & `pyrocko-2023.6.7/src/plot/cpt.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/directivity.py` & `pyrocko-2023.6.7/src/plot/directivity.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/dynamic_rupture.py` & `pyrocko-2023.6.7/src/plot/dynamic_rupture.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/gmtpy.py` & `pyrocko-2023.6.7/src/plot/gmtpy.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/hudson.py` & `pyrocko-2023.6.7/src/plot/hudson.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/response.py` & `pyrocko-2023.6.7/src/plot/response.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/plot/smartplot.py` & `pyrocko-2023.6.7/src/plot/smartplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,16 +626,15 @@
             mr += self._colorbar_width
             mb += self._colorbar_height
             sw = sh = self.separator
 
             nx, ny = self._shape
 
             # data_r = data_h / data_w
-            em = self.config.font_size
-            em_pixels = em / self._pixels
+            em = self.config.font_size / self._pixels
             w = self._width
             h = self._height
             fig_w_avail = w - mr - ml - (nx-1) * sw
             fig_h_avail = h - mt - mb - (ny-1) * sh
 
             if fig_w_avail <= 0.0 or fig_h_avail <= 0.0:
                 raise NotEnoughSpace()
@@ -693,20 +692,20 @@
 
                 axes.set_position(
                     self.rect_to_figure_coords(rect), which='both')
 
                 self.set_label_coords(
                     axes, 'x', [
                         wcenter(rect),
-                        self.config.label_offset_em[0]*em_pixels
+                        self.config.label_offset_em[0]*em
                         + self._colorbar_height])
 
                 self.set_label_coords(
                     axes, 'y', [
-                        self.config.label_offset_em[1]*em_pixels,
+                        self.config.label_offset_em[1]*em,
                         hcenter(rect)])
 
                 axes.get_xaxis().set_tick_params(
                     bottom=(iy == 0), top=(iy == ny-1),
                     labelbottom=(iy == 0), labeltop=False)
 
                 axes.get_yaxis().set_tick_params(
@@ -750,21 +749,20 @@
 
             for axes, orientation, position in self._colorbar_axes:
                 if orientation == 'horizontal':
                     xmin = self.window_xmin(position[0])
                     xmax = self.window_xmax(position[1])
                     ymin = mb - self._colorbar_height
                     ymax = mb - self._colorbar_height \
-                        + self.config.colorbar_width_em * em_pixels
+                        + self.config.colorbar_width_em * em
                 else:
                     ymin = self.window_ymin(position[0])
                     ymax = self.window_ymax(position[1])
                     xmin = w - mr + 2 * sw
-                    xmax = w - mr + 2 * sw \
-                        + self.config.colorbar_width_em * em_pixels
+                    xmax = w - mr + 2 * sw + self.config.colorbar_width_em * em
 
                 rect = [xmin, ymin, xmax-xmin, ymax-ymin]
                 axes.set_position(
                     self.rect_to_figure_coords(rect), which='both')
 
             for ix, axes in enumerate(self.axes_bottom_list):
                 dim = self._x_dims[ix]
@@ -829,21 +827,21 @@
 
         if position is None:
             if orientation == 'vertical':
                 position = (0, self._shape[1])
             else:
                 position = (0, self._shape[0])
 
-        em_pixels = self.config.font_size / self._pixels
+        em = self.config.font_size / self._pixels
 
         if orientation == 'vertical':
-            self._colorbar_width = self.config.colorbar_width_em*em_pixels + \
+            self._colorbar_width = self.config.colorbar_width_em*em + \
                 self.separator * 2.0
         else:
-            self._colorbar_height = self.config.colorbar_width_em*em_pixels + \
+            self._colorbar_height = self.config.colorbar_width_em*em + \
                 self.separator + self.margins[3]
 
         axes = SmartplotAxes(self.fig, [0., 0., 1., 1.])
         self.fig.add_axes(axes)
 
         self._colorbar_axes.append(
             (axes, orientation, position))
```

### Comparing `pyrocko-2023.6.29/src/plot/terminal.py` & `pyrocko-2023.6.7/src/plot/terminal.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/print_version.py` & `pyrocko-2023.6.7/src/print_version.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/progress.py` & `pyrocko-2023.6.7/src/progress.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/pz.py` & `pyrocko-2023.6.7/src/pz.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/response.py` & `pyrocko-2023.6.7/src/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
         return all(resp.is_scalar() for resp in self.responses)
 
     def get_scalar(self):
         '''
         Get factor if this is a flat response.
         '''
         if self.is_scalar():
-            return num.prod(resp.get_scalar() for resp in self.responses)
+            return num.product(resp.get_scalar() for resp in self.responses)
         else:
             raise IsNotScalar()
 
     def simplify(self):
         self.responses = simplify_responses(self.responses)
 
     def construction(self):
```

### Comparing `pyrocko-2023.6.29/src/scenario/base.py` & `pyrocko-2023.6.7/src/scenario/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/collection.py` & `pyrocko-2023.6.7/src/scenario/collection.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/scenario.py` & `pyrocko-2023.6.7/src/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/sources/base.py` & `pyrocko-2023.6.7/src/scenario/sources/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/sources/dcsource.py` & `pyrocko-2023.6.7/src/scenario/sources/dcsource.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/sources/pseudodynrupture.py` & `pyrocko-2023.6.7/src/scenario/sources/pseudodynrupture.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/sources/rectangularsource.py` & `pyrocko-2023.6.7/src/scenario/sources/rectangularsource.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/station.py` & `pyrocko-2023.6.7/src/scenario/station.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/targets/base.py` & `pyrocko-2023.6.7/src/scenario/targets/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/targets/gnss_campaign.py` & `pyrocko-2023.6.7/src/scenario/targets/gnss_campaign.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/targets/insar.py` & `pyrocko-2023.6.7/src/scenario/targets/insar.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/scenario/targets/waveform.py` & `pyrocko-2023.6.7/src/scenario/targets/waveform.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/shadow_pile.py` & `pyrocko-2023.6.7/src/shadow_pile.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/spit.py` & `pyrocko-2023.6.7/src/spit.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,20 +419,20 @@
             if any_(deepen) and all_(cell.depths + deepen <= self.clipdepth):
                 self._deepen_cell(cell)
             else:
                 if any_(deepen):
                     self.cells_to_continue.append(cell)
 
                 cell.bad = True
-                self.fraction_bad += num.prod(1.0/2**cell.depths)
+                self.fraction_bad += num.product(1.0/2**cell.depths)
                 self.nbad += 1
 
     def _deepen_cell(self, cell):
         if cell.bad:
-            self.fraction_bad -= num.prod(1.0/2**cell.depths)
+            self.fraction_bad -= num.product(1.0/2**cell.depths)
             self.nbad -= 1
             cell.bad = False
 
         for iadd in num.ndindex(*(cell.deepen+1)):
             index_child = (cell.index << cell.deepen) + iadd
             child = Cell(self, index_child)
             self.ncells += 1
```

### Comparing `pyrocko-2023.6.29/src/squirrel/__init__.py` & `pyrocko-2023.6.7/src/squirrel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/base.py` & `pyrocko-2023.6.7/src/squirrel/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # http://pyrocko.org - GPLv3
 #
 # The Pyrocko Developers, 21st Century
 # ---|P------/S----------~Lg----------
 
 import sys
 import os
-import time
+
 import math
 import logging
 import threading
 import queue
 from collections import defaultdict
 
 from pyrocko.guts import Object, Int, List, Tuple, String, Timestamp, Dict
@@ -310,16 +310,14 @@
         self._operator_registry = {}
 
         self._pending_orders = []
 
         self._pile = None
         self._n_choppers_active = 0
 
-        self.downloads_enabled = True
-
         self._names.update({
             'nuts': self.name + '_nuts',
             'kind_codes_count': self.name + '_kind_codes_count',
             'coverage': self.name + '_coverage'})
 
         with self.transaction('create tables') as cursor:
             self._create_tables_squirrel(cursor)
@@ -869,47 +867,51 @@
                         (to_kind_id(kind), kscale, tmax_seconds + 1))
             if tmin_cond:
                 cond.append(' ( ' + ' OR '.join(tmin_cond) + ' ) ')
 
         cond.append('%(db)s.%(nuts)s.tmax_seconds >= ?')
         args.append(tmin_seconds)
 
-    def _codes_match_sql(self, positive, kind_id, codes, cond, args):
+    def _codes_match_sql(self, kind_id, codes, cond, args):
         pats = codes_patterns_for_kind(kind_id, codes)
         if pats is None:
             return
 
         pats_exact = []
         pats_nonexact = []
         for pat in pats:
             spat = pat.safe_str
             (pats_exact if _is_exact(spat) else pats_nonexact).append(spat)
 
-        codes_cond = []
+        cond_exact = None
         if pats_exact:
-            codes_cond.append(' ( kind_codes.codes IN ( %s ) ) ' % ', '.join(
-                '?'*len(pats_exact)))
+            cond_exact = ' ( kind_codes.codes IN ( %s ) ) ' % ', '.join(
+                '?'*len(pats_exact))
 
             args.extend(pats_exact)
 
+        cond_nonexact = None
         if pats_nonexact:
-            codes_cond.append(' ( %s ) ' % ' OR '.join(
-                    ('kind_codes.codes GLOB ?',) * len(pats_nonexact)))
+            cond_nonexact = ' ( %s ) ' % ' OR '.join(
+                    ('kind_codes.codes GLOB ?',) * len(pats_nonexact))
 
             args.extend(pats_nonexact)
 
-        if codes_cond:
-            cond.append('%s ( %s )' % (
-                'NOT' if not positive else '',
-                ' OR '.join(codes_cond)))
+        if cond_exact and cond_nonexact:
+            cond.append(' ( %s OR %s ) ' % (cond_exact, cond_nonexact))
+
+        elif cond_exact:
+            cond.append(cond_exact)
+
+        elif cond_nonexact:
+            cond.append(cond_nonexact)
 
     def iter_nuts(
-            self, kind=None, tmin=None, tmax=None, codes=None,
-            codes_exclude=None, sample_rate_min=None, sample_rate_max=None,
-            naiv=False, kind_codes_ids=None, path=None, limit=None):
+            self, kind=None, tmin=None, tmax=None, codes=None, naiv=False,
+            kind_codes_ids=None, path=None, limit=None):
 
         '''
         Iterate over content entities matching given constraints.
 
         :param kind:
             Content kind (or kinds) to extract.
         :type kind:
@@ -986,26 +988,15 @@
 
             self._timerange_sql(tmin, tmax, kind, cond, args, naiv)
 
         cond.append('kind_codes.kind_id == ?')
         args.append(kind_id)
 
         if codes is not None:
-            self._codes_match_sql(True, kind_id, codes, cond, args)
-
-        if codes_exclude is not None:
-            self._codes_match_sql(False, kind_id, codes_exclude, cond, args)
-
-        if sample_rate_min is not None:
-            cond.append('kind_codes.deltat <= ?')
-            args.append(1.0/sample_rate_min)
-
-        if sample_rate_max is not None:
-            cond.append('? <= kind_codes.deltat')
-            args.append(1.0/sample_rate_max)
+            self._codes_match_sql(kind_id, codes, cond, args)
 
         if kind_codes_ids is not None:
             cond.append(
                 ' ( kind_codes.kind_codes_id IN ( %s ) ) ' % ', '.join(
                     '?'*len(kind_codes_ids)))
 
             args.extend(kind_codes_ids)
@@ -1100,15 +1091,15 @@
 
                 cond = []
                 args = []
 
                 self._timerange_sql(tmin, tmax, kind, cond, args, False)
 
                 if codes is not None:
-                    self._codes_match_sql(True, kind_id, codes, cond, args)
+                    self._codes_match_sql(kind_id, codes, cond, args)
 
                 if path is not None:
                     cond.append('files.path == ?')
                     args.append(db.relpath(abspath(path)))
 
                 sql = sql_subst('''
                     SELECT
@@ -1757,15 +1748,15 @@
 
     def get_cache_stats(self, cache_id):
         return self._content_caches[cache_id].get_stats()
 
     @filldocs
     def get_stations(
             self, obj=None, tmin=None, tmax=None, time=None, codes=None,
-            model='squirrel', on_error='raise'):
+            model='squirrel'):
 
         '''
         Get stations matching given constraints.
 
         %(query_args)s
 
         :param model:
@@ -1781,16 +1772,15 @@
             :py:class:`pyrocko.model.Station <pyrocko.model.station.Station>`
             objects if ``model='pyrocko'`` is requested.
 
         See :py:meth:`iter_nuts` for details on time span matching.
         '''
 
         if model == 'pyrocko':
-            return self._get_pyrocko_stations(
-                obj, tmin, tmax, time, codes, on_error=on_error)
+            return self._get_pyrocko_stations(obj, tmin, tmax, time, codes)
         elif model in ('squirrel', 'stationxml', 'stationxml+'):
             args = self._get_selection_args(
                 STATION, obj, tmin, tmax, time, codes)
 
             nuts = sorted(
                 self.iter_nuts('station', *args), key=lambda nut: nut.dkey)
 
@@ -2001,61 +1991,60 @@
 
         args = self._get_selection_args(EVENT, obj, tmin, tmax, time, codes)
         nuts = sorted(
             self.iter_nuts('event', *args), key=lambda nut: nut.dkey)
 
         return [self.get_content(nut) for nut in nuts]
 
-    def _redeem_promises(self, *args, order_only=False):
+    def _redeem_promises(self, *args, codes_exclude=None, order_only=False):
 
-        def split_promise(order, tmax=None):
+        def split_promise(order):
             self._split_nuts(
                 'waveform_promise',
-                order.tmin, tmax if tmax is not None else order.tmax,
+                order.tmin, order.tmax,
                 codes=order.codes,
                 path=order.source_id)
 
-        tmin, tmax = args[:2]
+        tmin, tmax, _ = args
 
         waveforms = list(self.iter_nuts('waveform', *args))
         promises = list(self.iter_nuts('waveform_promise', *args))
+        if codes_exclude is not None:
+            promises = [
+                promise for promise in promises
+                if promise.codes not in codes_exclude]
 
         codes_to_avail = defaultdict(list)
         for nut in waveforms:
             codes_to_avail[nut.codes].append((nut.tmin, nut.tmax))
 
         def tts(x):
             if isinstance(x, tuple):
                 return tuple(tts(e) for e in x)
             elif isinstance(x, list):
                 return list(tts(e) for e in x)
             else:
                 return util.time_to_str(x)
 
-        now = time.time()
         orders = []
         for promise in promises:
             waveforms_avail = codes_to_avail[promise.codes]
             for block_tmin, block_tmax in blocks(
                     max(tmin, promise.tmin),
                     min(tmax, promise.tmax),
                     promise.deltat):
 
-                if block_tmin > now:
-                    continue
-
                 orders.append(
                     WaveformOrder(
                         source_id=promise.file_path,
                         codes=promise.codes,
                         tmin=block_tmin,
                         tmax=block_tmax,
                         deltat=promise.deltat,
-                        gaps=gaps(waveforms_avail, block_tmin, block_tmax),
-                        time_created=now))
+                        gaps=gaps(waveforms_avail, block_tmin, block_tmax)))
 
         orders_noop, orders = lpick(lambda order: order.gaps, orders)
 
         order_keys_noop = set(order_key(order) for order in orders_noop)
         if len(order_keys_noop) != 0 or len(orders_noop) != 0:
             logger.info(
                 'Waveform orders already satisified with cached/local data: '
@@ -2108,38 +2097,27 @@
             task = make_task('Waveform orders processed', n_order_groups)
         else:
             task = None
 
         def release_order_group(order):
             okey = order_key(order)
             for followup in order_groups[okey]:
-                if followup is not order:
-                    split_promise(followup)
+                split_promise(followup)
 
             del order_groups[okey]
 
             if task:
                 task.update(n_order_groups - len(order_groups))
 
         def noop(order):
             pass
 
-        def success(order, trs):
+        def success(order):
             release_order_group(order)
-            if order.is_near_real_time():
-                if not trs:
-                    return  # keep promise when no data received at real time
-                else:
-                    tmax = max(tr.tmax+tr.deltat for tr in trs)
-                    tmax = order.tmin \
-                        + round((tmax - order.tmin) / order.deltat) \
-                        * order.deltat
-                    split_promise(order, tmax)
-            else:
-                split_promise(order)
+            split_promise(order)
 
         def batch_add(paths):
             self.add(paths)
 
         calls = queue.Queue()
 
         def enqueue(f):
@@ -2199,42 +2177,37 @@
 
         if task:
             task.done()
 
     @filldocs
     def get_waveform_nuts(
             self, obj=None, tmin=None, tmax=None, time=None, codes=None,
-            codes_exclude=None, sample_rate_min=None, sample_rate_max=None,
-            order_only=False):
+            codes_exclude=None, order_only=False):
 
         '''
         Get waveform content entities matching given constraints.
 
         %(query_args)s
 
         Like :py:meth:`get_nuts` with ``kind='waveform'`` but additionally
         resolves matching waveform promises (downloads waveforms from remote
         sources).
 
         See :py:meth:`iter_nuts` for details on time span matching.
         '''
 
         args = self._get_selection_args(WAVEFORM, obj, tmin, tmax, time, codes)
-
-        if self.downloads_enabled:
-            self._redeem_promises(
-                *args,
-                codes_exclude,
-                sample_rate_min,
-                sample_rate_max,
-                order_only=order_only)
-
+        self._redeem_promises(
+            *args, codes_exclude=codes_exclude, order_only=order_only)
         nuts = sorted(
             self.iter_nuts('waveform', *args), key=lambda nut: nut.dkey)
 
+        if codes_exclude is not None:
+            nuts = [nut for nut in nuts if nut.codes not in codes_exclude]
+
         return nuts
 
     @filldocs
     def have_waveforms(
             self, obj=None, tmin=None, tmax=None, time=None, codes=None):
 
         '''
@@ -2243,43 +2216,30 @@
 
         %(query_args)s
         '''
 
         args = self._get_selection_args(WAVEFORM, obj, tmin, tmax, time, codes)
         return bool(list(
                 self.iter_nuts('waveform', *args, limit=1))) \
-            or (self.downloads_enabled and bool(list(
-                self.iter_nuts('waveform_promise', *args, limit=1))))
+            or bool(list(
+                self.iter_nuts('waveform_promise', *args, limit=1)))
 
     @filldocs
     def get_waveforms(
             self, obj=None, tmin=None, tmax=None, time=None, codes=None,
-            codes_exclude=None, sample_rate_min=None, sample_rate_max=None,
-            uncut=False, want_incomplete=True, degap=True,
+            codes_exclude=None, uncut=False, want_incomplete=True, degap=True,
             maxgap=5, maxlap=None, snap=None, include_last=False,
             load_data=True, accessor_id='default', operator_params=None,
-            order_only=False, channel_priorities=None):
+            order_only=False, channel_priorities=None, target_deltat=None):
 
         '''
         Get waveforms matching given constraints.
 
         %(query_args)s
 
-        :param sample_rate_min:
-            Consider only waveforms with a sampling rate equal to or greater
-            than the given value [Hz].
-        :type sample_rate_min:
-            float
-
-        :param sample_rate_max:
-            Consider only waveforms with a sampling rate equal to or less than
-            the given value [Hz].
-        :type sample_rate_max:
-            float
-
         :param uncut:
             Set to ``True``, to disable cutting traces to [``tmin``, ``tmax``]
             and to disable degapping/deoverlapping. Returns untouched traces as
             they are read from file segment. File segments are always read in
             their entirety.
         :type uncut:
             bool
@@ -2332,24 +2292,14 @@
             management (see :py:mod:`~pyrocko.squirrel.cache`). Used as a key
             to distinguish different points of extraction for the decision of
             when to release cached waveform data. Should be used when data is
             alternately extracted from more than one region / selection.
         :type accessor_id:
             str
 
-        :param channel_priorities:
-            List of band/instrument code combinations to try. For example,
-            giving ``['HH', 'BH']`` would first try to get ``HH?`` channels and
-            then fallback to ``BH?`` if these are not available. The first
-            matching waveforms are returned. Use in combination with
-            ``sample_rate_min`` and ``sample_rate_max`` to constrain the sample
-            rate.
-        :type channel_priorities:
-            list of str
-
         See :py:meth:`iter_nuts` for details on time span matching.
 
         Loaded data is kept in memory (at least) until
         :py:meth:`clear_accessor` has been called or
         :py:meth:`advance_accessor` has been called two consecutive times
         without data being accessed between the two calls (by this accessor).
         Data may still be further kept in the memory cache if held alive by
@@ -2357,28 +2307,24 @@
         '''
 
         tmin, tmax, codes = self._get_selection_args(
             WAVEFORM, obj, tmin, tmax, time, codes)
 
         if channel_priorities is not None:
             return self._get_waveforms_prioritized(
-                tmin=tmin, tmax=tmax, codes=codes, codes_exclude=codes_exclude,
-                sample_rate_min=sample_rate_min,
-                sample_rate_max=sample_rate_max,
+                tmin=tmin, tmax=tmax, codes=codes,
                 uncut=uncut, want_incomplete=want_incomplete, degap=degap,
                 maxgap=maxgap, maxlap=maxlap, snap=snap,
                 include_last=include_last, load_data=load_data,
                 accessor_id=accessor_id, operator_params=operator_params,
-                order_only=order_only, channel_priorities=channel_priorities)
-
-        kinds = ['waveform']
-        if self.downloads_enabled:
-            kinds.append('waveform_promise')
+                order_only=order_only, channel_priorities=channel_priorities,
+                target_deltat=target_deltat)
 
-        self_tmin, self_tmax = self.get_time_span(kinds)
+        self_tmin, self_tmax = self.get_time_span(
+            ['waveform', 'waveform_promise'])
 
         if None in (self_tmin, self_tmax):
             logger.warning(
                 'No waveforms available.')
             return []
 
         tmin = tmin if tmin is not None else self_tmin
@@ -2393,16 +2339,16 @@
                     tmin=tmin, tmax=tmax,
                     uncut=uncut, want_incomplete=want_incomplete, degap=degap,
                     maxgap=maxgap, maxlap=maxlap, snap=snap,
                     include_last=include_last, load_data=load_data,
                     accessor_id=accessor_id, params=operator_params)
 
         nuts = self.get_waveform_nuts(
-            obj, tmin, tmax, time, codes, codes_exclude, sample_rate_min,
-            sample_rate_max, order_only=order_only)
+            obj, tmin, tmax, time, codes, codes_exclude=codes_exclude,
+            order_only=order_only)
 
         if order_only:
             return []
 
         if load_data:
             traces = [
                 self.get_content(nut, 'waveform', accessor_id) for nut in nuts]
@@ -2435,33 +2381,30 @@
 
         processed = self._process_chopped(
             chopped, degap, maxgap, maxlap, want_incomplete, tmin, tmax)
 
         return processed
 
     def _get_waveforms_prioritized(
-            self, tmin=None, tmax=None, codes=None, codes_exclude=None,
-            channel_priorities=None, **kwargs):
+            self, tmin=None, tmax=None, codes=None,
+            channel_priorities=None, target_deltat=None, **kwargs):
 
         trs_all = []
         codes_have = set()
         for channel in channel_priorities:
             assert len(channel) == 2
             if codes is not None:
                 codes_now = [
                     codes_.replace(channel=channel+'?') for codes_ in codes]
             else:
                 codes_now = model.CodesNSLCE('*', '*', '*', channel+'?')
 
-            codes_exclude_now = list(set(
+            codes_exclude_now = set(
                 codes_.replace(channel=channel+codes_.channel[-1])
-                for codes_ in codes_have))
-
-            if codes_exclude:
-                codes_exclude_now.extend(codes_exclude)
+                for codes_ in codes_have)
 
             trs = self.get_waveforms(
                 tmin=tmin,
                 tmax=tmax,
                 codes=codes_now,
                 codes_exclude=codes_exclude_now,
                 **kwargs)
@@ -2470,21 +2413,20 @@
             trs_all.extend(trs)
 
         return trs_all
 
     @filldocs
     def chopper_waveforms(
             self, obj=None, tmin=None, tmax=None, time=None, codes=None,
-            codes_exclude=None, sample_rate_min=None, sample_rate_max=None,
             tinc=None, tpad=0.,
             want_incomplete=True, snap_window=False,
             degap=True, maxgap=5, maxlap=None,
             snap=None, include_last=False, load_data=True,
             accessor_id=None, clear_accessor=True, operator_params=None,
-            grouping=None, channel_priorities=None):
+            grouping=None, channel_priorities=None, target_deltat=None):
 
         '''
         Iterate window-wise over waveform archive.
 
         %(query_args)s
 
         :param tinc:
@@ -2578,19 +2520,16 @@
 
         See :py:meth:`iter_nuts` for details on time span matching.
         '''
 
         tmin, tmax, codes = self._get_selection_args(
             WAVEFORM, obj, tmin, tmax, time, codes)
 
-        kinds = ['waveform']
-        if self.downloads_enabled:
-            kinds.append('waveform_promise')
-
-        self_tmin, self_tmax = self.get_time_span(kinds)
+        self_tmin, self_tmax = self.get_time_span(
+            ['waveform', 'waveform_promise'])
 
         if None in (self_tmin, self_tmax):
             logger.warning(
                 'Content has undefined time span. No waveforms and no '
                 'waveform promises?')
             return
 
@@ -2621,16 +2560,15 @@
                 codes_list = [codes]
             else:
                 operator = Operator(
                     filtering=CodesPatternFiltering(codes=codes),
                     grouping=grouping)
 
                 available = set(self.get_codes(kind='waveform'))
-                if self.downloads_enabled:
-                    available.update(self.get_codes(kind='waveform_promise'))
+                available.update(self.get_codes(kind='waveform_promise'))
                 operator.update_mappings(sorted(available))
 
                 codes_list = [
                     codes_patterns_list(scl)
                     for scl in operator.iter_in_codes()]
 
             ngroups = len(codes_list)
@@ -2638,27 +2576,25 @@
                 for iwin in range(nwin):
                     wmin, wmax = tmin+iwin*tinc, min(tmin+(iwin+1)*tinc, tmax)
 
                     chopped = self.get_waveforms(
                         tmin=wmin-tpad,
                         tmax=wmax+tpad,
                         codes=scl,
-                        codes_exclude=codes_exclude,
-                        sample_rate_min=sample_rate_min,
-                        sample_rate_max=sample_rate_max,
                         snap=snap,
                         include_last=include_last,
                         load_data=load_data,
                         want_incomplete=want_incomplete,
                         degap=degap,
                         maxgap=maxgap,
                         maxlap=maxlap,
                         accessor_id=accessor_id,
                         operator_params=operator_params,
-                        channel_priorities=channel_priorities)
+                        channel_priorities=channel_priorities,
+                        target_deltat=target_deltat)
 
                     self.advance_accessor(accessor_id)
 
                     yield Batch(
                         tmin=wmin,
                         tmax=wmax,
                         i=iwin,
@@ -2695,16 +2631,15 @@
                         chopped_weeded.append(tr)
 
             chopped = chopped_weeded
 
         return chopped
 
     def _get_pyrocko_stations(
-            self, obj=None, tmin=None, tmax=None, time=None, codes=None,
-            on_error='raise'):
+            self, obj=None, tmin=None, tmax=None, time=None, codes=None):
 
         from pyrocko import model as pmodel
 
         if codes is not None:
             codes = codes_patterns_for_kind(STATION, codes)
 
         by_nsl = defaultdict(lambda: (list(), list()))
@@ -2723,29 +2658,27 @@
 
         pstations = []
         nsls = list(by_nsl.keys())
         nsls.sort()
         for nsl in nsls:
             sargs_list, channels_list = by_nsl[nsl]
             sargs = util.consistency_merge(
-                [('',) + x for x in sargs_list],
-                error=on_error)
+                [('',) + x for x in sargs_list])
 
             by_c = defaultdict(list)
             for ch in channels_list:
                 by_c[ch.codes.channel].append(ch._get_pyrocko_channel_args())
 
             chas = list(by_c.keys())
             chas.sort()
             pchannels = []
             for cha in chas:
                 list_of_cargs = by_c[cha]
                 cargs = util.consistency_merge(
-                    [('',) + x for x in list_of_cargs],
-                    error=on_error)
+                    [('',) + x for x in list_of_cargs])
                 pchannels.append(pmodel.Channel(*cargs))
 
             pstations.append(
                 pmodel.Station(*sargs, channels=pchannels))
 
         return pstations
 
@@ -2768,19 +2701,19 @@
         from . import pile
 
         if self._pile is None:
             self._pile = pile.Pile(self)
 
         return self._pile
 
-    def snuffle(self, **kwargs):
+    def snuffle(self):
         '''
         Look at dataset in Snuffler.
         '''
-        self.pile.snuffle(**kwargs)
+        self.pile.snuffle()
 
     def _gather_codes_keys(self, kind, gather, selector):
         return set(
             gather(codes)
             for codes in self.iter_codes(kind)
             if selector is None or selector(codes))
```

### Comparing `pyrocko-2023.6.29/src/squirrel/cache.py` & `pyrocko-2023.6.7/src/squirrel/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,18 +202,15 @@
             if not entry[2]:
                 delete.append(path_segment)
 
         for path_segment in delete:
             logger.debug('Forgetting (clear): %s %s' % path_segment)
             del self._entries[path_segment]
 
-        try:
-            del self._accessor_ticks[accessor]
-        except KeyError:
-            pass
+        del self._accessor_ticks[accessor]
 
     def clear(self):
         '''
         Empty the cache.
         '''
         for accessor in list(self._accessor_ticks.keys()):
             self.clear_accessor(accessor)
```

### Comparing `pyrocko-2023.6.29/src/squirrel/check.py` & `pyrocko-2023.6.7/src/squirrel/check.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/client/base.py` & `pyrocko-2023.6.7/src/squirrel/client/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/client/catalog.py` & `pyrocko-2023.6.7/src/squirrel/client/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,14 @@
 
             if tmin >= tmax:
                 return
 
             tnow = time.time()
             modified = False
 
-            if tmax > tnow:
-                tmax = tnow
-
             if not self._chain:
                 self._chain = [Link(tmin, tmax, tnow)]
                 modified = True
             else:
                 if tmin < self._chain[0].tmin:
                     self._chain[0:0] = [Link(tmin, self._chain[0].tmin, tnow)]
                     modified = True
```

### Comparing `pyrocko-2023.6.29/src/squirrel/client/fdsn.py` & `pyrocko-2023.6.7/src/squirrel/client/fdsn.py`

 * *Files 2% similar despite different names*

```diff
@@ -543,14 +543,15 @@
             return 0.0
 
     def _get_channels_expiration_time(self):
         return self._get_expiration_time(self._get_channels_path())
 
     def update_waveform_promises(self, squirrel, constraint):
         from ..base import gaps
+        now = time.time()
         cpath = os.path.abspath(self._get_channels_path())
 
         ctmin = constraint.tmin
         ctmax = constraint.tmax
 
         nuts = squirrel.iter_nuts(
             'channel',
@@ -584,16 +585,20 @@
                 if subnut.tmax - subnut.tmin < 2*subnut.deltat:
                     continue
 
                 yield subnut
 
         def wanted(nuts):
             for nut in nuts:
-                for nut in sgaps(nut):
-                    yield nut
+                if nut.tmin < now:
+                    if nut.tmax > now:
+                        nut.tmax = now
+
+                    for nut in sgaps(nut):
+                        yield nut
 
         path = self._source_id
         squirrel.add_virtual(
             (make_waveform_promise_nut(
                 file_path=path,
                 **nut.waveform_promise_kwargs) for nut in wanted(nuts)),
             virtual_paths=[path])
@@ -697,18 +702,15 @@
                                 err_this = ('invalid waveform', str(e))
 
                         if len(trs_order) == 0:
                             if err_this is None:
                                 err_this = ('empty result', '')
 
                             elog.append(now, order, *err_this)
-                            if order.is_near_real_time():
-                                error_temporary(order)
-                            else:
-                                error_permanent(order)
+                            error_permanent(order)
                         else:
                             def tsame(ta, tb):
                                 return abs(tb - ta) < 2 * order.deltat
 
                             if len(trs_order) != 1 \
                                     or not tsame(
                                         trs_order[0].tmin, order.tmin) \
@@ -723,24 +725,21 @@
                                 else:
                                     elog.append(now, order, 'partial result')
 
                             paths = self._archive.add(order, trs_order)
                             all_paths.extend(paths)
 
                             nsuccess += 1
-                            success(order, trs_order)
+                            success(order)
 
                 except fdsn.EmptyResult:
                     now = time.time()
                     for order in orders_now:
                         elog.append(now, order, 'empty result')
-                        if order.is_near_real_time():
-                            error_temporary(order)
-                        else:
-                            error_permanent(order)
+                        error_permanent(order)
 
                 except Aborted as e:
                     now = time.time()
                     for order in orders_now:
                         elog.append(now, order, 'aborted', str(e))
                         error_permanent(order)
```

### Comparing `pyrocko-2023.6.29/src/squirrel/client/local.py` & `pyrocko-2023.6.7/src/squirrel/client/local.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/database.py` & `pyrocko-2023.6.7/src/squirrel/database.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/dataset.py` & `pyrocko-2023.6.7/src/squirrel/dataset.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/environment.py` & `pyrocko-2023.6.7/src/squirrel/environment.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/datacube.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/datacube.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/mseed.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/mseed.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/sac.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/sac.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/stationxml.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/stationxml.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/tdms_idas.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/tdms_idas.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/textfiles.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/textfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                     return False
                 if lon < -180. or 180 < lon:
                     return False
 
                 return True
 
             except Exception:
+                raise
                 return False
 
     return False
 
 
 g_event_keys = set('''
 name region catalog magnitude_type latitude longitude magnitude depth duration
```

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/virtual.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/virtual.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/backends/yaml.py` & `pyrocko-2023.6.7/src/squirrel/io/backends/yaml.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/io/base.py` & `pyrocko-2023.6.7/src/squirrel/io/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/lock.py` & `pyrocko-2023.6.7/src/squirrel/lock.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/model.py` & `pyrocko-2023.6.7/src/squirrel/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from base64 import urlsafe_b64encode
 from collections import defaultdict, namedtuple
 
 import numpy as num
 
 from pyrocko import util
 from pyrocko.guts import Object, SObject, String, Timestamp, Float, Int, \
-    Unicode, Tuple, List, StringChoice, Any, Dict, Duration, clone
+    Unicode, Tuple, List, StringChoice, Any, Dict, clone
 from pyrocko.model import squirrel_content, Location
 from pyrocko.response import FrequencyResponse, MultiplyResponse, \
     IntegrationResponse, DifferentiationResponse, simplify_responses, \
     FrequencyResponseCheckpoint
 
 from .error import ConversionError, SquirrelError
 
@@ -1191,16 +1191,14 @@
 
     source_id = String.T()
     codes = CodesNSLCE.T()
     deltat = Float.T()
     tmin = Timestamp.T()
     tmax = Timestamp.T()
     gaps = List.T(Tuple.T(2, Timestamp.T()))
-    time_created = Timestamp.T()
-    anxious = Duration.T(default=600.)
 
     @property
     def client(self):
         return self.source_id.split(':')[1]
 
     def describe(self, site='?'):
         return '%s:%s %s [%s - %s]' % (
@@ -1220,17 +1218,14 @@
 
         if not num.all(num.isfinite(tr.ydata)):
             raise InvalidWaveform('waveform has NaN values')
 
     def estimate_nsamples(self):
         return int(round((self.tmax - self.tmin) / self.deltat))+1
 
-    def is_near_real_time(self):
-        return self.tmax > self.time_created - self.anxious
-
 
 def order_summary(orders):
     codes_list = sorted(set(order.codes for order in orders))
     if len(codes_list) > 3:
         return '%i order%s: %s - %s' % (
             len(orders),
             util.plural_s(orders),
@@ -1684,15 +1679,15 @@
             return 1.0 / self.deltat
 
     @property
     def labels(self):
         srate = self.sample_rate
         return (
             ('%s' % str(self.codes)),
-            '%.4g' % srate if srate else '')
+            '%.3g' % srate if srate else '')
 
     @property
     def total(self):
         total_t = None
         for tmin, tmax, _ in self.iter_spans():
             total_t = (total_t or 0.0) + (tmax - tmin)
```

### Comparing `pyrocko-2023.6.29/src/squirrel/operators/base.py` & `pyrocko-2023.6.7/src/squirrel/operators/base.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/pile.py` & `pyrocko-2023.6.7/src/squirrel/pile.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def add_listener(self, obj):
         self._listeners.append(util.smart_weakref(obj))
 
     def notify_listeners(self, what):
         for ref in self._listeners:
             obj = ref()
             if obj:
-                obj(what, [])
+                obj.pile_changed(what, [])
 
     def get_tmin(self):
         return self.tmin
 
     def get_tmax(self):
         return self.tmax
```

### Comparing `pyrocko-2023.6.29/src/squirrel/selection.py` & `pyrocko-2023.6.7/src/squirrel/selection.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/cli.py` & `pyrocko-2023.6.7/src/squirrel/tool/cli.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/check.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/check.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/codes.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/codes.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/coverage.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/coverage.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/database.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/database.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/files.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/files.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/init.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/init.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/jackseis.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/jackseis.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/jackseis_classic.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/jackseis_classic.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/nuts.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/nuts.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/operators.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/operators.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/persistent.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/persistent.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/remove.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/response.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/response.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/scan.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/scan.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/stationxml.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/stationxml.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/template.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/template.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/commands/update.py` & `pyrocko-2023.6.7/src/squirrel/tool/commands/update.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/squirrel/tool/common.py` & `pyrocko-2023.6.7/src/squirrel/tool/common.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/streaming/datacube.py` & `pyrocko-2023.6.7/src/streaming/datacube.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/streaming/edl.py` & `pyrocko-2023.6.7/src/streaming/edl.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/streaming/serial_hamster.py` & `pyrocko-2023.6.7/src/streaming/serial_hamster.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/streaming/slink.py` & `pyrocko-2023.6.7/src/streaming/slink.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/table.py` & `pyrocko-2023.6.7/src/table.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/trace.py` & `pyrocko-2023.6.7/src/trace.py`

 * *Files identical despite different names*

### Comparing `pyrocko-2023.6.29/src/util.py` & `pyrocko-2023.6.7/src/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1583,17 +1583,14 @@
     '''
     Default :py:func:`str_to_time` with filling in of missing values.
 
     Allows e.g. `'2010-01-01 00:00:00'` as `'2010-01-01 00:00'`,
     `'2010-01-01 00'`, ..., or `'2010'`.
     '''
 
-    if s == 'now':
-        return time.time()
-
     if len(s) in (4, 7, 10, 13, 16):
         s += '0000-01-01 00:00:00'[len(s):]
 
     return str_to_time(s)
 
 
 def time_to_str(t, format='%Y-%m-%d %H:%M:%S.3FRAC'):
```

### Comparing `pyrocko-2023.6.29/src/weeding.py` & `pyrocko-2023.6.7/src/weeding.py`

 * *Files identical despite different names*

