# Comparing `tmp/flopy-3.4.0.tar.gz` & `tmp/flopy-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flopy-3.4.0.tar", last modified: Thu Jun 29 03:01:22 2023, max compression
+gzip compressed data, was "flopy-3.4.1.tar", last modified: Thu Jun 29 14:53:33 2023, max compression
```

## Comparing `flopy-3.4.0.tar` & `flopy-3.4.1.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.491979 flopy-3.4.0/
--rw-rw-rw-   0        0        0     2895 2023-06-29 02:56:10.000000 flopy-3.4.0/CITATION.cff
--rw-rw-rw-   0        0        0     1673 2023-06-20 17:54:37.000000 flopy-3.4.0/LICENSE.md
--rw-rw-rw-   0        0        0      139 2023-06-20 17:54:37.000000 flopy-3.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5537 2023-06-29 03:01:22.490979 flopy-3.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    10075 2023-06-29 02:56:10.000000 flopy-3.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.769980 flopy-3.4.0/docs/
--rw-rw-rw-   0        0        0     2579 2023-06-29 02:56:10.000000 flopy-3.4.0/docs/PyPI_release.md
--rw-rw-rw-   0        0        0     5527 2023-06-29 02:56:10.000000 flopy-3.4.0/docs/flopy_method_dependencies.md
--rw-rw-rw-   0        0        0     2689 2023-06-29 02:56:10.000000 flopy-3.4.0/docs/generate_classes.md
--rw-rw-rw-   0        0        0     4163 2023-06-20 17:54:37.000000 flopy-3.4.0/docs/get_modflow.md
--rw-rw-rw-   0        0        0     9180 2023-06-29 02:56:10.000000 flopy-3.4.0/docs/make_release.md
--rw-rw-rw-   0        0        0     3420 2023-06-29 02:56:10.000000 flopy-3.4.0/docs/mf6.md
--rw-rw-rw-   0        0        0     6126 2023-06-20 17:54:37.000000 flopy-3.4.0/docs/mf6_dev_guide.md
--rw-rw-rw-   0        0        0     4154 2023-06-20 17:54:37.000000 flopy-3.4.0/docs/model_checks.md
--rw-rw-rw-   0        0        0      834 2023-06-20 17:54:37.000000 flopy-3.4.0/docs/script_examples.md
--rw-rw-rw-   0        0        0    18577 2023-06-20 17:54:37.000000 flopy-3.4.0/docs/supported_packages.md
--rw-rw-rw-   0        0        0    96614 2023-06-29 02:56:10.000000 flopy-3.4.0/docs/version_changes.md
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.777979 flopy-3.4.0/flopy/
--rw-rw-rw-   0        0        0     1860 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/__init__.py
--rw-rw-rw-   0        0        0     2115 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/datbase.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.834976 flopy-3.4.0/flopy/discretization/
--rw-rw-rw-   0        0        0      128 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/discretization/__init__.py
--rw-rw-rw-   0        0        0    36214 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/discretization/grid.py
--rw-rw-rw-   0        0        0     2319 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/discretization/modeltime.py
--rw-rw-rw-   0        0        0    64705 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/discretization/structuredgrid.py
--rw-rw-rw-   0        0        0    33771 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/discretization/unstructuredgrid.py
--rw-rw-rw-   0        0        0    18627 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/discretization/vertexgrid.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.877975 flopy-3.4.0/flopy/export/
--rw-rw-rw-   0        0        0       98 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/export/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/export/longnames.py
--rw-rw-rw-   0        0        0     9962 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/export/metadata.py
--rw-rw-rw-   0        0        0    51190 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/export/netcdf.py
--rw-rw-rw-   0        0        0    22844 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/export/shapefile_utils.py
--rw-rw-rw-   0        0        0     2116 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/export/unitsformat.py
--rw-rw-rw-   0        0        0    66643 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/export/utils.py
--rw-rw-rw-   0        0        0    69972 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/export/vtk.py
--rw-rw-rw-   0        0        0    61408 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mbase.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.887975 flopy-3.4.0/flopy/mf6/
--rw-rw-rw-   0        0        0      186 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.894974 flopy-3.4.0/flopy/mf6/coordinates/
--rw-rw-rw-   0        0        0        0 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/coordinates/__init__.py
--rw-rw-rw-   0        0        0    32710 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/coordinates/modeldimensions.py
--rw-rw-rw-   0        0        0    26914 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/coordinates/modelgrid.py
--rw-rw-rw-   0        0        0     3066 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/coordinates/simulationtime.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.914982 flopy-3.4.0/flopy/mf6/data/
--rw-rw-rw-   0        0        0       53 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.033976 flopy-3.4.0/flopy/mf6/data/dfn/
--rw-rw-rw-   0        0        0     5695 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/common.dfn
--rw-rw-rw-   0        0        0    11993 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/exg-gwfgwf.dfn
--rw-rw-rw-   0        0        0       70 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/exg-gwfgwt.dfn
--rw-rw-rw-   0        0        0     9619 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/exg-gwtgwt.dfn
--rw-rw-rw-   0        0        0      300 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/data/dfn/flopy.dfn
--rw-rw-rw-   0        0        0     1948 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-api.dfn
--rw-rw-rw-   0        0        0     5055 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-buy.dfn
--rw-rw-rw-   0        0        0     4184 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-chd.dfn
--rw-rw-rw-   0        0        0    22746 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-csub.dfn
--rw-rw-rw-   0        0        0     4108 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-dis.dfn
--rw-rw-rw-   0        0        0    11751 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-disu.dfn
--rw-rw-rw-   0        0        0     6376 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-disv.dfn
--rw-rw-rw-   0        0        0     5663 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-drn.dfn
--rw-rw-rw-   0        0        0     7938 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-evt.dfn
--rw-rw-rw-   0        0        0     5186 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-evta.dfn
--rw-rw-rw-   0        0        0     4858 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-ghb.dfn
--rw-rw-rw-   0        0        0     4504 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-gnc.dfn
--rw-rw-rw-   0        0        0     2834 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-hfb.dfn
--rw-rw-rw-   0        0        0      825 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-ic.dfn
--rw-rw-rw-   0        0        0    29848 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-lak.dfn
--rw-rw-rw-   0        0        0    27849 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-maw.dfn
--rw-rw-rw-   0        0        0     7488 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-mvr.dfn
--rw-rw-rw-   0        0        0     3633 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-nam.dfn
--rw-rw-rw-   0        0        0    18036 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-npf.dfn
--rw-rw-rw-   0        0        0     6097 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-oc.dfn
--rw-rw-rw-   0        0        0     4535 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-rch.dfn
--rw-rw-rw-   0        0        0     4965 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-rcha.dfn
--rw-rw-rw-   0        0        0     5038 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-riv.dfn
--rw-rw-rw-   0        0        0    30358 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-sfr.dfn
--rw-rw-rw-   0        0        0     4536 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-sto.dfn
--rw-rw-rw-   0        0        0    18613 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-uzf.dfn
--rw-rw-rw-   0        0        0     7267 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-vsc.dfn
--rw-rw-rw-   0        0        0     6132 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwf-wel.dfn
--rw-rw-rw-   0        0        0      353 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-adv.dfn
--rw-rw-rw-   0        0        0     1948 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-api.dfn
--rw-rw-rw-   0        0        0     4277 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-cnc.dfn
--rw-rw-rw-   0        0        0     4097 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-dis.dfn
--rw-rw-rw-   0        0        0    11751 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-disu.dfn
--rw-rw-rw-   0        0        0     6365 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-disv.dfn
--rw-rw-rw-   0        0        0     3955 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-dsp.dfn
--rw-rw-rw-   0        0        0     2141 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-fmi.dfn
--rw-rw-rw-   0        0        0      433 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-ic.dfn
--rw-rw-rw-   0        0        0     8645 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-ist.dfn
--rw-rw-rw-   0        0        0    12855 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-lkt.dfn
--rw-rw-rw-   0        0        0     4317 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-mst.dfn
--rw-rw-rw-   0        0        0     2241 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-mvt.dfn
--rw-rw-rw-   0        0        0    11211 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-mwt.dfn
--rw-rw-rw-   0        0        0     2603 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-nam.dfn
--rw-rw-rw-   0        0        0     6187 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-oc.dfn
--rw-rw-rw-   0        0        0    12840 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-sft.dfn
--rw-rw-rw-   0        0        0     4229 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-src.dfn
--rw-rw-rw-   0        0        0     4899 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-ssm.dfn
--rw-rw-rw-   0        0        0    12007 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/gwt-uzt.dfn
--rw-rw-rw-   0        0        0     5581 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/sim-nam.dfn
--rw-rw-rw-   0        0        0     3279 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/sim-tdis.dfn
--rw-rw-rw-   0        0        0       32 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/sln-ems.dfn
--rw-rw-rw-   0        0        0    26719 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/dfn/sln-ims.dfn
--rw-rw-rw-   0        0        0     3914 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-ats.dfn
--rw-rw-rw-   0        0        0     1956 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-laktab.dfn
--rw-rw-rw-   0        0        0     4298 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-obs.dfn
--rw-rw-rw-   0        0        0     2543 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-sfrtab.dfn
--rw-rw-rw-   0        0        0     2751 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-spc.dfn
--rw-rw-rw-   0        0        0     2132 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-spca.dfn
--rw-rw-rw-   0        0        0     2444 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-tas.dfn
--rw-rw-rw-   0        0        0     3388 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-ts.dfn
--rw-rw-rw-   0        0        0     3984 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-tvk.dfn
--rw-rw-rw-   0        0        0     3716 2023-06-27 21:11:39.000000 flopy-3.4.0/flopy/mf6/data/dfn/utl-tvs.dfn
--rw-rw-rw-   0        0        0    22482 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mfdata.py
--rw-rw-rw-   0        0        0    79746 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mfdataarray.py
--rw-rw-rw-   0        0        0    88676 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mfdatalist.py
--rw-rw-rw-   0        0        0    36959 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mfdatascalar.py
--rw-rw-rw-   0        0        0   129016 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mfdatastorage.py
--rw-rw-rw-   0        0        0    31528 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/data/mfdatautil.py
--rw-rw-rw-   0        0        0   104443 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mffileaccess.py
--rw-rw-rw-   0        0        0    98421 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/data/mfstructure.py
--rw-rw-rw-   0        0        0    24984 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/mfbase.py
--rw-rw-rw-   0        0        0    73094 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/mfmodel.py
--rw-rw-rw-   0        0        0   135346 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/mfpackage.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.169979 flopy-3.4.0/flopy/mf6/modflow/
--rw-rw-rw-   0        0        0     2610 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/__init__.py
--rw-rw-rw-   0        0        0     1491 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfems.py
--rw-rw-rw-   0        0        0    11039 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgnc.py
--rw-rw-rw-   0        0        0     5489 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwf.py
--rw-rw-rw-   0        0        0     6584 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfapi.py
--rw-rw-rw-   0        0        0     9485 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfbuy.py
--rw-rw-rw-   0        0        0    13066 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfchd.py
--rw-rw-rw-   0        0        0    42572 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfcsub.py
--rw-rw-rw-   0        0        0     8481 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfdis.py
--rw-rw-rw-   0        0        0    20777 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfdisu.py
--rw-rw-rw-   0        0        0    12416 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfdisv.py
--rw-rw-rw-   0        0        0    15546 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfdrn.py
--rw-rw-rw-   0        0        0    18396 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfevt.py
--rw-rw-rw-   0        0        0    13277 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfevta.py
--rw-rw-rw-   0        0        0    14395 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfghb.py
--rw-rw-rw-   0        0        0    11067 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfgnc.py
--rw-rw-rw-   0        0        0    20061 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfgwf.py
--rw-rw-rw-   0        0        0     1990 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfgwt.py
--rw-rw-rw-   0        0        0     6117 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfhfb.py
--rw-rw-rw-   0        0        0     2634 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfic.py
--rw-rw-rw-   0        0        0    54924 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwflak.py
--rw-rw-rw-   0        0        0    47180 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfmaw.py
--rw-rw-rw-   0        0        0    16986 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfmvr.py
--rw-rw-rw-   0        0        0     7068 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfnam.py
--rw-rw-rw-   0        0        0    27491 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfnpf.py
--rw-rw-rw-   0        0        0    13855 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfoc.py
--rw-rw-rw-   0        0        0    13694 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfrch.py
--rw-rw-rw-   0        0        0    12620 2023-06-29 02:56:10.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfrcha.py
--rw-rw-rw-   0        0        0    14734 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfriv.py
--rw-rw-rw-   0        0        0    55501 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfsfr.py
--rw-rw-rw-   0        0        0     9146 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfsto.py
--rw-rw-rw-   0        0        0    36307 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfuzf.py
--rw-rw-rw-   0        0        0    12367 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfvsc.py
--rw-rw-rw-   0        0        0    16361 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwfwel.py
--rw-rw-rw-   0        0        0     5069 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwt.py
--rw-rw-rw-   0        0        0     1958 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtadv.py
--rw-rw-rw-   0        0        0     6584 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtapi.py
--rw-rw-rw-   0        0        0    13111 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtcnc.py
--rw-rw-rw-   0        0        0     8470 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtdis.py
--rw-rw-rw-   0        0        0    20777 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtdisu.py
--rw-rw-rw-   0        0        0    12405 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtdisv.py
--rw-rw-rw-   0        0        0     7529 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtdsp.py
--rw-rw-rw-   0        0        0     4832 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtfmi.py
--rw-rw-rw-   0        0        0    18746 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtgwt.py
--rw-rw-rw-   0        0        0     2168 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtic.py
--rw-rw-rw-   0        0        0    16720 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtist.py
--rw-rw-rw-   0        0        0    27243 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtlkt.py
--rw-rw-rw-   0        0        0     8957 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtmst.py
--rw-rw-rw-   0        0        0     8120 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtmvt.py
--rw-rw-rw-   0        0        0    24654 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtmwt.py
--rw-rw-rw-   0        0        0     6048 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtnam.py
--rw-rw-rw-   0        0        0    14091 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtoc.py
--rw-rw-rw-   0        0        0    27170 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtsft.py
--rw-rw-rw-   0        0        0    13160 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtsrc.py
--rw-rw-rw-   0        0        0     8370 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtssm.py
--rw-rw-rw-   0        0        0    25731 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfgwtuzt.py
--rw-rw-rw-   0        0        0    39403 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfims.py
--rw-rw-rw-   0        0        0    16959 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfmvr.py
--rw-rw-rw-   0        0        0     8054 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfmvt.py
--rw-rw-rw-   0        0        0    10086 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfnam.py
--rw-rw-rw-   0        0        0    91692 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfsimulation.py
--rw-rw-rw-   0        0        0     6801 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mftdis.py
--rw-rw-rw-   0        0        0     8193 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutlats.py
--rw-rw-rw-   0        0        0     4524 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutllaktab.py
--rw-rw-rw-   0        0        0     8626 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutlobs.py
--rw-rw-rw-   0        0        0     5137 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutlsfrtab.py
--rw-rw-rw-   0        0        0     6920 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutlspc.py
--rw-rw-rw-   0        0        0     5491 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutlspca.py
--rw-rw-rw-   0        0        0     7986 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutltas.py
--rw-rw-rw-   0        0        0    11031 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutlts.py
--rw-rw-rw-   0        0        0    10296 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutltvk.py
--rw-rw-rw-   0        0        0    10518 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/modflow/mfutltvs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.218977 flopy-3.4.0/flopy/mf6/utils/
--rw-rw-rw-   0        0        0      275 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/__init__.py
--rw-rw-rw-   0        0        0    13755 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/utils/binaryfile_utils.py
--rw-rw-rw-   0        0        0    20017 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/binarygrid_util.py
--rw-rw-rw-   0        0        0    36478 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/createpackages.py
--rw-rw-rw-   0        0        0     5726 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/generate_classes.py
--rw-rw-rw-   0        0        0    10172 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/lakpak_utils.py
--rw-rw-rw-   0        0        0      195 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/utils/mfenums.py
--rw-rw-rw-   0        0        0    18064 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/utils/mfobservation.py
--rw-rw-rw-   0        0        0   116265 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/model_splitter.py
--rw-rw-rw-   0        0        0    13522 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/utils/output_util.py
--rw-rw-rw-   0        0        0     4686 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/utils/postprocessing.py
--rw-rw-rw-   0        0        0    27947 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mf6/utils/reference.py
--rw-rw-rw-   0        0        0     7300 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mf6/utils/testutils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.241980 flopy-3.4.0/flopy/mfusg/
--rw-rw-rw-   0        0        0      492 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mfusg/__init__.py
--rw-rw-rw-   0        0        0     5905 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mfusg/cln_dtypes.py
--rw-rw-rw-   0        0        0    20088 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusg.py
--rw-rw-rw-   0        0        0    23902 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusgbcf.py
--rw-rw-rw-   0        0        0    30846 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusgcln.py
--rw-rw-rw-   0        0        0    30582 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusgdisu.py
--rw-rw-rw-   0        0        0    10742 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusggnc.py
--rw-rw-rw-   0        0        0    31541 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusglpf.py
--rw-rw-rw-   0        0        0    24457 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mfusg/mfusgsms.py
--rw-rw-rw-   0        0        0    10499 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mfusg/mfusgwel.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.327979 flopy-3.4.0/flopy/modflow/
--rw-rw-rw-   0        0        0     1545 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/__init__.py
--rw-rw-rw-   0        0        0    33244 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mf.py
--rw-rw-rw-   0        0        0      504 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfaddoutsidefile.py
--rw-rw-rw-   0        0        0    32852 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfag.py
--rw-rw-rw-   0        0        0    12176 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfbas.py
--rw-rw-rw-   0        0        0    17362 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfbcf.py
--rw-rw-rw-   0        0        0     4763 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfbct.py
--rw-rw-rw-   0        0        0     8364 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfchd.py
--rw-rw-rw-   0        0        0    10474 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfde4.py
--rw-rw-rw-   0        0        0    31053 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfdis.py
--rw-rw-rw-   0        0        0    10511 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfdrn.py
--rw-rw-rw-   0        0        0    10292 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfdrt.py
--rw-rw-rw-   0        0        0    14869 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfevt.py
--rw-rw-rw-   0        0        0    25258 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mffhb.py
--rw-rw-rw-   0        0        0    20697 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfflwob.py
--rw-rw-rw-   0        0        0    12628 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfgage.py
--rw-rw-rw-   0        0        0     9651 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfghb.py
--rw-rw-rw-   0        0        0    15137 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfgmg.py
--rw-rw-rw-   0        0        0    14397 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfhfb.py
--rw-rw-rw-   0        0        0    24314 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfhob.py
--rw-rw-rw-   0        0        0    11947 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfhyd.py
--rw-rw-rw-   0        0        0    36742 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mflak.py
--rw-rw-rw-   0        0        0     8154 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mflmt.py
--rw-rw-rw-   0        0        0    26722 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mflpf.py
--rw-rw-rw-   0        0        0     7421 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfmlt.py
--rw-rw-rw-   0        0        0    17456 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfmnw1.py
--rw-rw-rw-   0        0        0    79248 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfmnw2.py
--rw-rw-rw-   0        0        0    12038 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfmnwi.py
--rw-rw-rw-   0        0        0    20041 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfnwt.py
--rw-rw-rw-   0        0        0    40037 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfoc.py
--rw-rw-rw-   0        0        0    11543 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfpar.py
--rw-rw-rw-   0        0        0     9275 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfparbc.py
--rw-rw-rw-   0        0        0     3756 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfpbc.py
--rw-rw-rw-   0        0        0    10977 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfpcg.py
--rw-rw-rw-   0        0        0    20840 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfpcgn.py
--rw-rw-rw-   0        0        0     7989 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfpks.py
--rw-rw-rw-   0        0        0     5552 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfpval.py
--rw-rw-rw-   0        0        0    19054 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfrch.py
--rw-rw-rw-   0        0        0    12738 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfriv.py
--rw-rw-rw-   0        0        0   134537 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfsfr2.py
--rw-rw-rw-   0        0        0     8007 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfsip.py
--rw-rw-rw-   0        0        0     5635 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfsor.py
--rw-rw-rw-   0        0        0    37392 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfstr.py
--rw-rw-rw-   0        0        0    32200 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfsub.py
--rw-rw-rw-   0        0        0    26472 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfswi2.py
--rw-rw-rw-   0        0        0     4711 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfswr1.py
--rw-rw-rw-   0        0        0    32415 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfswt.py
--rw-rw-rw-   0        0        0    21559 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfupw.py
--rw-rw-rw-   0        0        0    46190 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfuzf1.py
--rw-rw-rw-   0        0        0    13201 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflow/mfwel.py
--rw-rw-rw-   0        0        0     6026 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflow/mfzon.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.331980 flopy-3.4.0/flopy/modflowlgr/
--rw-rw-rw-   0        0        0       41 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modflowlgr/__init__.py
--rw-rw-rw-   0        0        0    21424 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modflowlgr/mflgr.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.343974 flopy-3.4.0/flopy/modpath/
--rw-rw-rw-   0        0        0      442 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modpath/__init__.py
--rw-rw-rw-   0        0        0    19916 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modpath/mp6.py
--rw-rw-rw-   0        0        0     7212 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modpath/mp6bas.py
--rw-rw-rw-   0        0        0    20802 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modpath/mp6sim.py
--rw-rw-rw-   0        0        0    17266 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modpath/mp7.py
--rw-rw-rw-   0        0        0     4324 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modpath/mp7bas.py
--rw-rw-rw-   0        0        0    36405 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modpath/mp7particledata.py
--rw-rw-rw-   0        0        0    15842 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/modpath/mp7particlegroup.py
--rw-rw-rw-   0        0        0    25974 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/modpath/mp7sim.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.368974 flopy-3.4.0/flopy/mt3d/
--rw-rw-rw-   0        0        0      332 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mt3d/__init__.py
--rw-rw-rw-   0        0        0    27354 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mt.py
--rw-rw-rw-   0        0        0    16476 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtadv.py
--rw-rw-rw-   0        0        0    40495 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtbtn.py
--rw-rw-rw-   0        0        0    12527 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/mt3d/mtcts.py
--rw-rw-rw-   0        0        0    16069 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtdsp.py
--rw-rw-rw-   0        0        0     7094 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtgcg.py
--rw-rw-rw-   0        0        0    18242 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtlkt.py
--rw-rw-rw-   0        0        0     3303 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtphc.py
--rw-rw-rw-   0        0        0    28302 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtrct.py
--rw-rw-rw-   0        0        0    29621 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtsft.py
--rw-rw-rw-   0        0        0    30132 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtssm.py
--rw-rw-rw-   0        0        0     3468 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mttob.py
--rw-rw-rw-   0        0        0    28333 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/mt3d/mtuzt.py
--rw-rw-rw-   0        0        0    44370 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/pakbase.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.374975 flopy-3.4.0/flopy/pest/
--rw-rw-rw-   0        0        0      150 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/pest/__init__.py
--rw-rw-rw-   0        0        0     2957 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/pest/params.py
--rw-rw-rw-   0        0        0     3235 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/pest/templatewriter.py
--rw-rw-rw-   0        0        0     5981 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/pest/tplarray.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.383976 flopy-3.4.0/flopy/plot/
--rw-rw-rw-   0        0        0      449 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/plot/__init__.py
--rw-rw-rw-   0        0        0    51043 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/plot/crosssection.py
--rw-rw-rw-   0        0        0    32425 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/plot/map.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.406977 flopy-3.4.0/flopy/plot/mplstyle/
--rw-rw-rw-   0        0        0      595 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/plot/mplstyle/usgsmap.mplstyle
--rw-rw-rw-   0        0        0      605 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/plot/mplstyle/usgsmap_linux.mplstyle
--rw-rw-rw-   0        0        0      595 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/plot/mplstyle/usgsplot.mplstyle
--rw-rw-rw-   0        0        0      605 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/plot/mplstyle/usgsplot_linux.mplstyle
--rw-rw-rw-   0        0        0    97411 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/plot/plotutil.py
--rw-rw-rw-   0        0        0    12926 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/plot/styles.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.413976 flopy-3.4.0/flopy/seawat/
--rw-rw-rw-   0        0        0       87 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/seawat/__init__.py
--rw-rw-rw-   0        0        0    15366 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/seawat/swt.py
--rw-rw-rw-   0        0        0    20834 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/seawat/swtvdf.py
--rw-rw-rw-   0        0        0    17841 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/seawat/swtvsc.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:22.488976 flopy-3.4.0/flopy/utils/
--rw-rw-rw-   0        0        0     1655 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/utils/__init__.py
--rw-rw-rw-   0        0        0    69734 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/binaryfile.py
--rw-rw-rw-   0        0        0    33129 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/check.py
--rw-rw-rw-   0        0        0    51468 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/compare.py
--rw-rw-rw-   0        0        0     5215 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/crs.py
--rw-rw-rw-   0        0        0    12470 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/cvfdutil.py
--rw-rw-rw-   0        0        0    20549 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/datafile.py
--rw-rw-rw-   0        0        0    27811 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/datautil.py
--rw-rw-rw-   0        0        0    18488 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/flopy_io.py
--rw-rw-rw-   0        0        0    13059 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/formattedfile.py
--rw-rw-rw-   0        0        0    25467 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/geometry.py
--rw-rw-rw-   0        0        0    14411 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/geospatial_utils.py
--rw-rw-rw-   0        0        0    27289 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/get_modflow.py
--rw-rw-rw-   0        0        0    62075 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/gridgen.py
--rw-rw-rw-   0        0        0    88523 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/gridintersect.py
--rw-rw-rw-   0        0        0     6784 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/gridutil.py
--rw-rw-rw-   0        0        0    19023 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/lgrutil.py
--rw-rw-rw-   0        0        0    32934 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/mflistfile.py
--rw-rw-rw-   0        0        0    24089 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/mfreadnam.py
--rw-rw-rw-   0        0        0    52927 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/modpathfile.py
--rw-rw-rw-   0        0        0    17528 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/mtlistfile.py
--rw-rw-rw-   0        0        0    20727 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/observationfile.py
--rw-rw-rw-   0        0        0    15396 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/optionblock.py
--rw-rw-rw-   0        0        0    16962 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/parse_version.py
--rw-rw-rw-   0        0        0    29673 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/postprocessing.py
--rw-rw-rw-   0        0        0    26050 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/rasters.py
--rw-rw-rw-   0        0        0     2670 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/utils/recarray_utils.py
--rw-rw-rw-   0        0        0      829 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/utils/reference.py
--rw-rw-rw-   0        0        0     7323 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/utils/sfroutputfile.py
--rw-rw-rw-   0        0        0    24453 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/swroutputfile.py
--rw-rw-rw-   0        0        0    23596 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/triangle.py
--rw-rw-rw-   0        0        0   104820 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/util_array.py
--rw-rw-rw-   0        0        0    44538 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/util_list.py
--rw-rw-rw-   0        0        0     7140 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/utils_def.py
--rw-rw-rw-   0        0        0     5974 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/utils/utl_import.py
--rw-rw-rw-   0        0        0    12649 2023-06-20 17:54:40.000000 flopy-3.4.0/flopy/utils/voronoi.py
--rw-rw-rw-   0        0        0   105704 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/utils/zonbud.py
--rw-rw-rw-   0        0        0      307 2023-06-29 02:56:11.000000 flopy-3.4.0/flopy/version.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:01:21.822979 flopy-3.4.0/flopy.egg-info/
--rw-rw-rw-   0        0        0     5537 2023-06-29 03:01:21.000000 flopy-3.4.0/flopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9589 2023-06-29 03:01:21.000000 flopy-3.4.0/flopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 03:01:21.000000 flopy-3.4.0/flopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-29 03:01:21.000000 flopy-3.4.0/flopy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 17:56:21.000000 flopy-3.4.0/flopy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      597 2023-06-29 03:01:21.000000 flopy-3.4.0/flopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 03:01:21.000000 flopy-3.4.0/flopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2952 2023-06-29 02:56:11.000000 flopy-3.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 03:01:22.491979 flopy-3.4.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2023-06-29 02:56:11.000000 flopy-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.745468 flopy-3.4.1/
+-rw-rw-rw-   0        0        0     2895 2023-06-29 14:52:07.000000 flopy-3.4.1/CITATION.cff
+-rw-rw-rw-   0        0        0     1673 2023-06-20 17:54:37.000000 flopy-3.4.1/LICENSE.md
+-rw-rw-rw-   0        0        0      139 2023-06-20 17:54:37.000000 flopy-3.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5537 2023-06-29 14:53:33.744468 flopy-3.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10075 2023-06-29 14:52:07.000000 flopy-3.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.012468 flopy-3.4.1/docs/
+-rw-rw-rw-   0        0        0     2579 2023-06-29 14:52:07.000000 flopy-3.4.1/docs/PyPI_release.md
+-rw-rw-rw-   0        0        0     5527 2023-06-29 02:56:10.000000 flopy-3.4.1/docs/flopy_method_dependencies.md
+-rw-rw-rw-   0        0        0     2689 2023-06-29 02:56:10.000000 flopy-3.4.1/docs/generate_classes.md
+-rw-rw-rw-   0        0        0     4163 2023-06-20 17:54:37.000000 flopy-3.4.1/docs/get_modflow.md
+-rw-rw-rw-   0        0        0     9087 2023-06-29 14:50:18.000000 flopy-3.4.1/docs/make_release.md
+-rw-rw-rw-   0        0        0     3420 2023-06-29 02:56:10.000000 flopy-3.4.1/docs/mf6.md
+-rw-rw-rw-   0        0        0     6126 2023-06-20 17:54:37.000000 flopy-3.4.1/docs/mf6_dev_guide.md
+-rw-rw-rw-   0        0        0     4154 2023-06-20 17:54:37.000000 flopy-3.4.1/docs/model_checks.md
+-rw-rw-rw-   0        0        0      834 2023-06-20 17:54:37.000000 flopy-3.4.1/docs/script_examples.md
+-rw-rw-rw-   0        0        0    18577 2023-06-20 17:54:37.000000 flopy-3.4.1/docs/supported_packages.md
+-rw-rw-rw-   0        0        0    96851 2023-06-29 14:50:18.000000 flopy-3.4.1/docs/version_changes.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.023474 flopy-3.4.1/flopy/
+-rw-rw-rw-   0        0        0     1860 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/__init__.py
+-rw-rw-rw-   0        0        0     2115 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/datbase.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.061469 flopy-3.4.1/flopy/discretization/
+-rw-rw-rw-   0        0        0      128 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/discretization/__init__.py
+-rw-rw-rw-   0        0        0    36214 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/discretization/grid.py
+-rw-rw-rw-   0        0        0     2319 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/discretization/modeltime.py
+-rw-rw-rw-   0        0        0    64705 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/discretization/structuredgrid.py
+-rw-rw-rw-   0        0        0    33771 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/discretization/unstructuredgrid.py
+-rw-rw-rw-   0        0        0    18627 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/discretization/vertexgrid.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.077474 flopy-3.4.1/flopy/export/
+-rw-rw-rw-   0        0        0       98 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/export/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/export/longnames.py
+-rw-rw-rw-   0        0        0     9962 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/export/metadata.py
+-rw-rw-rw-   0        0        0    51190 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/export/netcdf.py
+-rw-rw-rw-   0        0        0    22844 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/export/shapefile_utils.py
+-rw-rw-rw-   0        0        0     2116 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/export/unitsformat.py
+-rw-rw-rw-   0        0        0    66643 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/export/utils.py
+-rw-rw-rw-   0        0        0    69972 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/export/vtk.py
+-rw-rw-rw-   0        0        0    61408 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mbase.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.085468 flopy-3.4.1/flopy/mf6/
+-rw-rw-rw-   0        0        0      186 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.095467 flopy-3.4.1/flopy/mf6/coordinates/
+-rw-rw-rw-   0        0        0        0 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/coordinates/__init__.py
+-rw-rw-rw-   0        0        0    32710 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/coordinates/modeldimensions.py
+-rw-rw-rw-   0        0        0    26914 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/coordinates/modelgrid.py
+-rw-rw-rw-   0        0        0     3066 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/coordinates/simulationtime.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.114467 flopy-3.4.1/flopy/mf6/data/
+-rw-rw-rw-   0        0        0       53 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.277484 flopy-3.4.1/flopy/mf6/data/dfn/
+-rw-rw-rw-   0        0        0     5695 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/common.dfn
+-rw-rw-rw-   0        0        0    11993 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/exg-gwfgwf.dfn
+-rw-rw-rw-   0        0        0       70 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/exg-gwfgwt.dfn
+-rw-rw-rw-   0        0        0     9619 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/exg-gwtgwt.dfn
+-rw-rw-rw-   0        0        0      300 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/data/dfn/flopy.dfn
+-rw-rw-rw-   0        0        0     1948 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-api.dfn
+-rw-rw-rw-   0        0        0     5055 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-buy.dfn
+-rw-rw-rw-   0        0        0     4184 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-chd.dfn
+-rw-rw-rw-   0        0        0    22746 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-csub.dfn
+-rw-rw-rw-   0        0        0     4108 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-dis.dfn
+-rw-rw-rw-   0        0        0    11751 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-disu.dfn
+-rw-rw-rw-   0        0        0     6376 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-disv.dfn
+-rw-rw-rw-   0        0        0     5663 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-drn.dfn
+-rw-rw-rw-   0        0        0     7938 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-evt.dfn
+-rw-rw-rw-   0        0        0     5186 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-evta.dfn
+-rw-rw-rw-   0        0        0     4858 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-ghb.dfn
+-rw-rw-rw-   0        0        0     4504 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-gnc.dfn
+-rw-rw-rw-   0        0        0     2834 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-hfb.dfn
+-rw-rw-rw-   0        0        0      825 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-ic.dfn
+-rw-rw-rw-   0        0        0    29848 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-lak.dfn
+-rw-rw-rw-   0        0        0    27849 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-maw.dfn
+-rw-rw-rw-   0        0        0     7488 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-mvr.dfn
+-rw-rw-rw-   0        0        0     3633 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-nam.dfn
+-rw-rw-rw-   0        0        0    18036 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-npf.dfn
+-rw-rw-rw-   0        0        0     6097 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-oc.dfn
+-rw-rw-rw-   0        0        0     4535 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-rch.dfn
+-rw-rw-rw-   0        0        0     4965 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-rcha.dfn
+-rw-rw-rw-   0        0        0     5038 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-riv.dfn
+-rw-rw-rw-   0        0        0    30358 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-sfr.dfn
+-rw-rw-rw-   0        0        0     4536 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-sto.dfn
+-rw-rw-rw-   0        0        0    18613 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-uzf.dfn
+-rw-rw-rw-   0        0        0     7267 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-vsc.dfn
+-rw-rw-rw-   0        0        0     6132 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwf-wel.dfn
+-rw-rw-rw-   0        0        0      353 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-adv.dfn
+-rw-rw-rw-   0        0        0     1948 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-api.dfn
+-rw-rw-rw-   0        0        0     4277 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-cnc.dfn
+-rw-rw-rw-   0        0        0     4097 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-dis.dfn
+-rw-rw-rw-   0        0        0    11751 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-disu.dfn
+-rw-rw-rw-   0        0        0     6365 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-disv.dfn
+-rw-rw-rw-   0        0        0     3955 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-dsp.dfn
+-rw-rw-rw-   0        0        0     2141 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-fmi.dfn
+-rw-rw-rw-   0        0        0      433 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-ic.dfn
+-rw-rw-rw-   0        0        0     8645 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-ist.dfn
+-rw-rw-rw-   0        0        0    12855 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-lkt.dfn
+-rw-rw-rw-   0        0        0     4317 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-mst.dfn
+-rw-rw-rw-   0        0        0     2241 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-mvt.dfn
+-rw-rw-rw-   0        0        0    11211 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-mwt.dfn
+-rw-rw-rw-   0        0        0     2603 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-nam.dfn
+-rw-rw-rw-   0        0        0     6187 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-oc.dfn
+-rw-rw-rw-   0        0        0    12840 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-sft.dfn
+-rw-rw-rw-   0        0        0     4229 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-src.dfn
+-rw-rw-rw-   0        0        0     4899 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-ssm.dfn
+-rw-rw-rw-   0        0        0    12007 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/gwt-uzt.dfn
+-rw-rw-rw-   0        0        0     5581 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/sim-nam.dfn
+-rw-rw-rw-   0        0        0     3279 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/sim-tdis.dfn
+-rw-rw-rw-   0        0        0       32 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/data/dfn/sln-ems.dfn
+-rw-rw-rw-   0        0        0    26719 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/dfn/sln-ims.dfn
+-rw-rw-rw-   0        0        0     3914 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-ats.dfn
+-rw-rw-rw-   0        0        0     1956 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-laktab.dfn
+-rw-rw-rw-   0        0        0     4298 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-obs.dfn
+-rw-rw-rw-   0        0        0     2543 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-sfrtab.dfn
+-rw-rw-rw-   0        0        0     2751 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-spc.dfn
+-rw-rw-rw-   0        0        0     2132 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-spca.dfn
+-rw-rw-rw-   0        0        0     2444 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-tas.dfn
+-rw-rw-rw-   0        0        0     3388 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-ts.dfn
+-rw-rw-rw-   0        0        0     3984 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-tvk.dfn
+-rw-rw-rw-   0        0        0     3716 2023-06-27 21:11:39.000000 flopy-3.4.1/flopy/mf6/data/dfn/utl-tvs.dfn
+-rw-rw-rw-   0        0        0    22482 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mfdata.py
+-rw-rw-rw-   0        0        0    79746 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mfdataarray.py
+-rw-rw-rw-   0        0        0    88676 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mfdatalist.py
+-rw-rw-rw-   0        0        0    36959 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mfdatascalar.py
+-rw-rw-rw-   0        0        0   129016 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mfdatastorage.py
+-rw-rw-rw-   0        0        0    31528 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/data/mfdatautil.py
+-rw-rw-rw-   0        0        0   104443 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mffileaccess.py
+-rw-rw-rw-   0        0        0    98421 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/data/mfstructure.py
+-rw-rw-rw-   0        0        0    24984 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/mfbase.py
+-rw-rw-rw-   0        0        0    73094 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/mfmodel.py
+-rw-rw-rw-   0        0        0   135346 2023-06-29 02:56:10.000000 flopy-3.4.1/flopy/mf6/mfpackage.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.402470 flopy-3.4.1/flopy/mf6/modflow/
+-rw-rw-rw-   0        0        0     2610 2023-06-29 05:03:37.000000 flopy-3.4.1/flopy/mf6/modflow/__init__.py
+-rw-rw-rw-   0        0        0     1491 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfems.py
+-rw-rw-rw-   0        0        0    11039 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgnc.py
+-rw-rw-rw-   0        0        0     5489 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwf.py
+-rw-rw-rw-   0        0        0     6584 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfapi.py
+-rw-rw-rw-   0        0        0     9485 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfbuy.py
+-rw-rw-rw-   0        0        0    13066 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfchd.py
+-rw-rw-rw-   0        0        0    42572 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfcsub.py
+-rw-rw-rw-   0        0        0     8481 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfdis.py
+-rw-rw-rw-   0        0        0    20777 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfdisu.py
+-rw-rw-rw-   0        0        0    12416 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfdisv.py
+-rw-rw-rw-   0        0        0    15546 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfdrn.py
+-rw-rw-rw-   0        0        0    18396 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfevt.py
+-rw-rw-rw-   0        0        0    13277 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfevta.py
+-rw-rw-rw-   0        0        0    14395 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfghb.py
+-rw-rw-rw-   0        0        0    11067 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfgnc.py
+-rw-rw-rw-   0        0        0    20061 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfgwf.py
+-rw-rw-rw-   0        0        0     1990 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfgwt.py
+-rw-rw-rw-   0        0        0     6117 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfhfb.py
+-rw-rw-rw-   0        0        0     2634 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfic.py
+-rw-rw-rw-   0        0        0    54924 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwflak.py
+-rw-rw-rw-   0        0        0    47180 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfmaw.py
+-rw-rw-rw-   0        0        0    16986 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfmvr.py
+-rw-rw-rw-   0        0        0     7068 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfnam.py
+-rw-rw-rw-   0        0        0    27491 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfnpf.py
+-rw-rw-rw-   0        0        0    13855 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfoc.py
+-rw-rw-rw-   0        0        0    13694 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfrch.py
+-rw-rw-rw-   0        0        0    12620 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfrcha.py
+-rw-rw-rw-   0        0        0    14734 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfriv.py
+-rw-rw-rw-   0        0        0    55501 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfsfr.py
+-rw-rw-rw-   0        0        0     9146 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfsto.py
+-rw-rw-rw-   0        0        0    36307 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfuzf.py
+-rw-rw-rw-   0        0        0    12367 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfvsc.py
+-rw-rw-rw-   0        0        0    16361 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwfwel.py
+-rw-rw-rw-   0        0        0     5069 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwt.py
+-rw-rw-rw-   0        0        0     1958 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtadv.py
+-rw-rw-rw-   0        0        0     6584 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtapi.py
+-rw-rw-rw-   0        0        0    13111 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtcnc.py
+-rw-rw-rw-   0        0        0     8470 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtdis.py
+-rw-rw-rw-   0        0        0    20777 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtdisu.py
+-rw-rw-rw-   0        0        0    12405 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtdisv.py
+-rw-rw-rw-   0        0        0     7529 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtdsp.py
+-rw-rw-rw-   0        0        0     4832 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtfmi.py
+-rw-rw-rw-   0        0        0    18746 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtgwt.py
+-rw-rw-rw-   0        0        0     2168 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtic.py
+-rw-rw-rw-   0        0        0    16720 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtist.py
+-rw-rw-rw-   0        0        0    27243 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtlkt.py
+-rw-rw-rw-   0        0        0     8957 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtmst.py
+-rw-rw-rw-   0        0        0     8120 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtmvt.py
+-rw-rw-rw-   0        0        0    24654 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtmwt.py
+-rw-rw-rw-   0        0        0     6048 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtnam.py
+-rw-rw-rw-   0        0        0    14091 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtoc.py
+-rw-rw-rw-   0        0        0    27170 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtsft.py
+-rw-rw-rw-   0        0        0    13160 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtsrc.py
+-rw-rw-rw-   0        0        0     8370 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtssm.py
+-rw-rw-rw-   0        0        0    25731 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfgwtuzt.py
+-rw-rw-rw-   0        0        0    39403 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfims.py
+-rw-rw-rw-   0        0        0    16959 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfmvr.py
+-rw-rw-rw-   0        0        0     8054 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfmvt.py
+-rw-rw-rw-   0        0        0    10086 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfnam.py
+-rw-rw-rw-   0        0        0    91692 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/modflow/mfsimulation.py
+-rw-rw-rw-   0        0        0     6801 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mftdis.py
+-rw-rw-rw-   0        0        0     8193 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutlats.py
+-rw-rw-rw-   0        0        0     4524 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutllaktab.py
+-rw-rw-rw-   0        0        0     8626 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutlobs.py
+-rw-rw-rw-   0        0        0     5137 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutlsfrtab.py
+-rw-rw-rw-   0        0        0     6920 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutlspc.py
+-rw-rw-rw-   0        0        0     5491 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutlspca.py
+-rw-rw-rw-   0        0        0     7986 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutltas.py
+-rw-rw-rw-   0        0        0    11031 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutlts.py
+-rw-rw-rw-   0        0        0    10296 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutltvk.py
+-rw-rw-rw-   0        0        0    10518 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/mf6/modflow/mfutltvs.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.426469 flopy-3.4.1/flopy/mf6/utils/
+-rw-rw-rw-   0        0        0      275 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/__init__.py
+-rw-rw-rw-   0        0        0    13755 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/utils/binaryfile_utils.py
+-rw-rw-rw-   0        0        0    20017 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/binarygrid_util.py
+-rw-rw-rw-   0        0        0    36478 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/createpackages.py
+-rw-rw-rw-   0        0        0     5726 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/generate_classes.py
+-rw-rw-rw-   0        0        0    10172 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/lakpak_utils.py
+-rw-rw-rw-   0        0        0      195 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/utils/mfenums.py
+-rw-rw-rw-   0        0        0    18064 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/utils/mfobservation.py
+-rw-rw-rw-   0        0        0   116265 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/model_splitter.py
+-rw-rw-rw-   0        0        0    13522 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/utils/output_util.py
+-rw-rw-rw-   0        0        0     4686 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/utils/postprocessing.py
+-rw-rw-rw-   0        0        0    27947 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mf6/utils/reference.py
+-rw-rw-rw-   0        0        0     7300 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mf6/utils/testutils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.442472 flopy-3.4.1/flopy/mfusg/
+-rw-rw-rw-   0        0        0      492 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mfusg/__init__.py
+-rw-rw-rw-   0        0        0     5905 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mfusg/cln_dtypes.py
+-rw-rw-rw-   0        0        0    20088 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusg.py
+-rw-rw-rw-   0        0        0    23902 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusgbcf.py
+-rw-rw-rw-   0        0        0    30846 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusgcln.py
+-rw-rw-rw-   0        0        0    30582 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusgdisu.py
+-rw-rw-rw-   0        0        0    10742 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusggnc.py
+-rw-rw-rw-   0        0        0    31541 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusglpf.py
+-rw-rw-rw-   0        0        0    24457 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mfusg/mfusgsms.py
+-rw-rw-rw-   0        0        0    10499 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mfusg/mfusgwel.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.531468 flopy-3.4.1/flopy/modflow/
+-rw-rw-rw-   0        0        0     1545 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/__init__.py
+-rw-rw-rw-   0        0        0    33244 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mf.py
+-rw-rw-rw-   0        0        0      504 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfaddoutsidefile.py
+-rw-rw-rw-   0        0        0    32852 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfag.py
+-rw-rw-rw-   0        0        0    12176 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfbas.py
+-rw-rw-rw-   0        0        0    17362 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfbcf.py
+-rw-rw-rw-   0        0        0     4763 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfbct.py
+-rw-rw-rw-   0        0        0     8364 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfchd.py
+-rw-rw-rw-   0        0        0    10474 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfde4.py
+-rw-rw-rw-   0        0        0    31053 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfdis.py
+-rw-rw-rw-   0        0        0    10511 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfdrn.py
+-rw-rw-rw-   0        0        0    10292 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfdrt.py
+-rw-rw-rw-   0        0        0    14869 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfevt.py
+-rw-rw-rw-   0        0        0    25258 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mffhb.py
+-rw-rw-rw-   0        0        0    20697 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfflwob.py
+-rw-rw-rw-   0        0        0    12628 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfgage.py
+-rw-rw-rw-   0        0        0     9651 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfghb.py
+-rw-rw-rw-   0        0        0    15137 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfgmg.py
+-rw-rw-rw-   0        0        0    14397 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfhfb.py
+-rw-rw-rw-   0        0        0    24314 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfhob.py
+-rw-rw-rw-   0        0        0    11947 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfhyd.py
+-rw-rw-rw-   0        0        0    36742 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mflak.py
+-rw-rw-rw-   0        0        0     8154 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mflmt.py
+-rw-rw-rw-   0        0        0    26722 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mflpf.py
+-rw-rw-rw-   0        0        0     7421 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfmlt.py
+-rw-rw-rw-   0        0        0    17456 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfmnw1.py
+-rw-rw-rw-   0        0        0    79248 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfmnw2.py
+-rw-rw-rw-   0        0        0    12038 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfmnwi.py
+-rw-rw-rw-   0        0        0    20041 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfnwt.py
+-rw-rw-rw-   0        0        0    40037 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfoc.py
+-rw-rw-rw-   0        0        0    11543 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfpar.py
+-rw-rw-rw-   0        0        0     9275 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfparbc.py
+-rw-rw-rw-   0        0        0     3756 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfpbc.py
+-rw-rw-rw-   0        0        0    10977 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfpcg.py
+-rw-rw-rw-   0        0        0    20840 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfpcgn.py
+-rw-rw-rw-   0        0        0     7989 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfpks.py
+-rw-rw-rw-   0        0        0     5552 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfpval.py
+-rw-rw-rw-   0        0        0    19054 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfrch.py
+-rw-rw-rw-   0        0        0    12738 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfriv.py
+-rw-rw-rw-   0        0        0   134537 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfsfr2.py
+-rw-rw-rw-   0        0        0     8007 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfsip.py
+-rw-rw-rw-   0        0        0     5635 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfsor.py
+-rw-rw-rw-   0        0        0    37392 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfstr.py
+-rw-rw-rw-   0        0        0    32200 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfsub.py
+-rw-rw-rw-   0        0        0    26472 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfswi2.py
+-rw-rw-rw-   0        0        0     4711 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfswr1.py
+-rw-rw-rw-   0        0        0    32415 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfswt.py
+-rw-rw-rw-   0        0        0    21559 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfupw.py
+-rw-rw-rw-   0        0        0    46190 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfuzf1.py
+-rw-rw-rw-   0        0        0    13201 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflow/mfwel.py
+-rw-rw-rw-   0        0        0     6026 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflow/mfzon.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.533468 flopy-3.4.1/flopy/modflowlgr/
+-rw-rw-rw-   0        0        0       41 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modflowlgr/__init__.py
+-rw-rw-rw-   0        0        0    21424 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modflowlgr/mflgr.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.549467 flopy-3.4.1/flopy/modpath/
+-rw-rw-rw-   0        0        0      442 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modpath/__init__.py
+-rw-rw-rw-   0        0        0    19916 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modpath/mp6.py
+-rw-rw-rw-   0        0        0     7212 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modpath/mp6bas.py
+-rw-rw-rw-   0        0        0    20802 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modpath/mp6sim.py
+-rw-rw-rw-   0        0        0    17266 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modpath/mp7.py
+-rw-rw-rw-   0        0        0     4324 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modpath/mp7bas.py
+-rw-rw-rw-   0        0        0    36405 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modpath/mp7particledata.py
+-rw-rw-rw-   0        0        0    15842 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/modpath/mp7particlegroup.py
+-rw-rw-rw-   0        0        0    25974 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/modpath/mp7sim.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.601472 flopy-3.4.1/flopy/mt3d/
+-rw-rw-rw-   0        0        0      332 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mt3d/__init__.py
+-rw-rw-rw-   0        0        0    27354 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mt.py
+-rw-rw-rw-   0        0        0    16476 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtadv.py
+-rw-rw-rw-   0        0        0    40495 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtbtn.py
+-rw-rw-rw-   0        0        0    12527 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/mt3d/mtcts.py
+-rw-rw-rw-   0        0        0    16069 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtdsp.py
+-rw-rw-rw-   0        0        0     7094 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtgcg.py
+-rw-rw-rw-   0        0        0    18242 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtlkt.py
+-rw-rw-rw-   0        0        0     3303 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtphc.py
+-rw-rw-rw-   0        0        0    28302 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtrct.py
+-rw-rw-rw-   0        0        0    29621 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtsft.py
+-rw-rw-rw-   0        0        0    30132 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtssm.py
+-rw-rw-rw-   0        0        0     3468 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mttob.py
+-rw-rw-rw-   0        0        0    28333 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/mt3d/mtuzt.py
+-rw-rw-rw-   0        0        0    44370 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/pakbase.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.610471 flopy-3.4.1/flopy/pest/
+-rw-rw-rw-   0        0        0      150 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/pest/__init__.py
+-rw-rw-rw-   0        0        0     2957 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/pest/params.py
+-rw-rw-rw-   0        0        0     3235 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/pest/templatewriter.py
+-rw-rw-rw-   0        0        0     5981 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/pest/tplarray.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.627472 flopy-3.4.1/flopy/plot/
+-rw-rw-rw-   0        0        0      449 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/plot/__init__.py
+-rw-rw-rw-   0        0        0    51043 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/plot/crosssection.py
+-rw-rw-rw-   0        0        0    32425 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/plot/map.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.653473 flopy-3.4.1/flopy/plot/mplstyle/
+-rw-rw-rw-   0        0        0      595 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/plot/mplstyle/usgsmap.mplstyle
+-rw-rw-rw-   0        0        0      605 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/plot/mplstyle/usgsmap_linux.mplstyle
+-rw-rw-rw-   0        0        0      595 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/plot/mplstyle/usgsplot.mplstyle
+-rw-rw-rw-   0        0        0      605 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/plot/mplstyle/usgsplot_linux.mplstyle
+-rw-rw-rw-   0        0        0    97411 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/plot/plotutil.py
+-rw-rw-rw-   0        0        0    12926 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/plot/styles.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.662469 flopy-3.4.1/flopy/seawat/
+-rw-rw-rw-   0        0        0       87 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/seawat/__init__.py
+-rw-rw-rw-   0        0        0    15366 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/seawat/swt.py
+-rw-rw-rw-   0        0        0    20834 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/seawat/swtvdf.py
+-rw-rw-rw-   0        0        0    17841 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/seawat/swtvsc.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.741468 flopy-3.4.1/flopy/utils/
+-rw-rw-rw-   0        0        0     1655 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/utils/__init__.py
+-rw-rw-rw-   0        0        0    69734 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/binaryfile.py
+-rw-rw-rw-   0        0        0    33129 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/check.py
+-rw-rw-rw-   0        0        0    51468 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/compare.py
+-rw-rw-rw-   0        0        0     5215 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/crs.py
+-rw-rw-rw-   0        0        0    12470 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/cvfdutil.py
+-rw-rw-rw-   0        0        0    20549 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/datafile.py
+-rw-rw-rw-   0        0        0    27811 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/datautil.py
+-rw-rw-rw-   0        0        0    18488 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/flopy_io.py
+-rw-rw-rw-   0        0        0    13059 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/formattedfile.py
+-rw-rw-rw-   0        0        0    25467 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/geometry.py
+-rw-rw-rw-   0        0        0    14411 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/geospatial_utils.py
+-rw-rw-rw-   0        0        0    27059 2023-06-29 14:50:18.000000 flopy-3.4.1/flopy/utils/get_modflow.py
+-rw-rw-rw-   0        0        0    62075 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/gridgen.py
+-rw-rw-rw-   0        0        0    88523 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/gridintersect.py
+-rw-rw-rw-   0        0        0     6784 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/gridutil.py
+-rw-rw-rw-   0        0        0    19023 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/lgrutil.py
+-rw-rw-rw-   0        0        0    32934 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/mflistfile.py
+-rw-rw-rw-   0        0        0    24089 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/mfreadnam.py
+-rw-rw-rw-   0        0        0    52927 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/modpathfile.py
+-rw-rw-rw-   0        0        0    17528 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/mtlistfile.py
+-rw-rw-rw-   0        0        0    20727 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/observationfile.py
+-rw-rw-rw-   0        0        0    15396 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/optionblock.py
+-rw-rw-rw-   0        0        0    16962 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/parse_version.py
+-rw-rw-rw-   0        0        0    29673 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/postprocessing.py
+-rw-rw-rw-   0        0        0    26050 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/rasters.py
+-rw-rw-rw-   0        0        0     2670 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/utils/recarray_utils.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/utils/reference.py
+-rw-rw-rw-   0        0        0     7323 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/utils/sfroutputfile.py
+-rw-rw-rw-   0        0        0    24453 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/swroutputfile.py
+-rw-rw-rw-   0        0        0    23596 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/triangle.py
+-rw-rw-rw-   0        0        0   104820 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/util_array.py
+-rw-rw-rw-   0        0        0    44538 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/util_list.py
+-rw-rw-rw-   0        0        0     7140 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/utils_def.py
+-rw-rw-rw-   0        0        0     5974 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/utils/utl_import.py
+-rw-rw-rw-   0        0        0    12649 2023-06-20 17:54:40.000000 flopy-3.4.1/flopy/utils/voronoi.py
+-rw-rw-rw-   0        0        0   105704 2023-06-29 02:56:11.000000 flopy-3.4.1/flopy/utils/zonbud.py
+-rw-rw-rw-   0        0        0      119 2023-06-29 14:52:07.000000 flopy-3.4.1/flopy/version.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:53:33.047468 flopy-3.4.1/flopy.egg-info/
+-rw-rw-rw-   0        0        0     5537 2023-06-29 14:53:32.000000 flopy-3.4.1/flopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9589 2023-06-29 14:53:32.000000 flopy-3.4.1/flopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:53:32.000000 flopy-3.4.1/flopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-29 14:53:32.000000 flopy-3.4.1/flopy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 17:56:21.000000 flopy-3.4.1/flopy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      608 2023-06-29 14:53:32.000000 flopy-3.4.1/flopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-29 14:53:32.000000 flopy-3.4.1/flopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2970 2023-06-29 14:50:18.000000 flopy-3.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:53:33.745468 flopy-3.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       96 2023-06-29 02:56:11.000000 flopy-3.4.1/setup.py
```

### Comparing `flopy-3.4.0/CITATION.cff` & `flopy-3.4.1/CITATION.cff`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cff-version: 1.2.0
 message: If you use this software, please cite both the article from preferred-citation
   and the software itself.
 type: software
 title: FloPy
-version: 3.4.0
+version: 3.4.1
 date-released: '2023-06-29'
 doi: 10.5066/F7BK19FH
 abstract: A Python package to create, run, and post-process MODFLOW-based models.
 repository-artifact: https://pypi.org/project/flopy
 repository-code: https://github.com/modflowpy/flopy
 license: CC0-1.0
 authors:
```

### Comparing `flopy-3.4.0/LICENSE.md` & `flopy-3.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/PKG-INFO` & `flopy-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flopy
-Version: 3.4.0
+Version: 3.4.1
 Summary: FloPy is a Python package to create, run, and post-process MODFLOW-based models
 Author-email: FloPy Team <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://flopy.readthedocs.io
 Project-URL: Release Notes, https://github.com/modflowpy/flopy/blob/develop/docs/version_changes.md
 Project-URL: Bug Tracker, https://github.com/modflowpy/flopy/issues
@@ -55,15 +55,15 @@
 
 *Citation for FloPy:*
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 *Software/Code citation for FloPy:*
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.0: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.1: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Disclaimer
 ----------
 
 This software is provided "as is" and "as-available", and makes no 
 representations or warranties of any kind concerning the software, whether
```

### Comparing `flopy-3.4.0/README.md` & `flopy-3.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 <img src="https://raw.githubusercontent.com/modflowpy/flopy/master/examples/images/flopy3.png" alt="flopy3" style="width:50;height:20">
 
-### Version 3.4.0
+### Version 3.4.1
 [![flopy continuous integration](https://github.com/modflowpy/flopy/actions/workflows/commit.yml/badge.svg?branch=develop)](https://github.com/modflowpy/flopy/actions/workflows/commit.yml)
 [![Read the Docs](https://github.com/modflowpy/flopy/actions/workflows/rtd.yml/badge.svg?branch=develop)](https://github.com/modflowpy/flopy/actions/workflows/rtd.yml)
 
 [![codecov](https://codecov.io/gh/modflowpy/flopy/branch/develop/graph/badge.svg)](https://codecov.io/gh/modflowpy/flopy)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3f44f457aa474a8f83ad60c1842f7be2)](https://www.codacy.com/gh/modflowpy/flopy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=modflowpy/flopy&amp;utm_campaign=Badge_Grade)
 [![Documentation Status](https://readthedocs.org/projects/flopy/badge/?version=latest)](https://flopy.readthedocs.io/en/latest/?badge=latest)
 
@@ -138,15 +138,15 @@
 
 ##### ***Citation for FloPy:***
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 ##### ***Software/Code citation for FloPy:***
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.0: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.1: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Additional FloPy Related Publications
 -----------------------------------------------
 
 [Leaf A.T, and Fienen M. N., 2022, Flopy&mdash;The Python Interface for MODFLOW: Groundwater, v. 60, no. 6, p. 710-712. doi:10.1111/gwat.13259.](https://doi.org/10.1111/gwat.13259)
```

### Comparing `flopy-3.4.0/docs/PyPI_release.md` & `flopy-3.4.1/docs/PyPI_release.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 *Citation for FloPy:*
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 *Software/Code citation for FloPy:*
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.0: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.1: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Disclaimer
 ----------
 
 This software is provided "as is" and "as-available", and makes no 
 representations or warranties of any kind concerning the software, whether
```

### Comparing `flopy-3.4.0/docs/flopy_method_dependencies.md` & `flopy-3.4.1/docs/flopy_method_dependencies.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/generate_classes.md` & `flopy-3.4.1/docs/generate_classes.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/get_modflow.md` & `flopy-3.4.1/docs/get_modflow.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/make_release.md` & `flopy-3.4.1/docs/make_release.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 #### Production mode
 
 If the branch name does not end with `rc`, the workflow will proceed to open a PR updating `master` from the release branch. Merging this PR to `master` triggers another job to draft a release.
 
 **Note:** the PR should be merged, not squashed. Squashing removes the commit history from the `master` branch and causes `develop` and `master` to diverge, which can cause future PRs updating `master` to replay commits from previous releases.
 
-Publishing the release triggers jobs to publish the `flopy` package to PyPI and open a PR updating `develop` from `master`. This PR also updates version numbers to the just-released version, and appends "+" to the end of the version string to indicate development status.
+Publishing the release triggers a final job to publish the `flopy` package to PyPI.
 
 ##### Trusted publishing
 
 The automated release workflow assumes [trusted publishing](https://docs.pypi.org/trusted-publishers/) has been configured in the PyPI admin interface. A GitHub environment called `release` is also required (however it needs no secrets or environment variables).
 
 ### Manual releases
 
@@ -105,15 +105,15 @@
 - GitHub should have tagged the most recent revision of `master` with the release number &mdash; if for some reason this did not occur automatically, tag `master` with the version number (`git tag <version>`) and push the tag to `modflowpy/flopy` (e.g., if you have your fork's remote named `origin` and `modflowpy/flopy` as `upstream`, as is typical, use `git push upstream --tags`).
 
 
 #### Reinitialize `develop` branch
 
 1.  Merge the `master` branch into the `develop` branch.
 
-2.  Set the version as appropriate: `python scripts/update_version.py -v <semver>`.
+2.  Set the development version as appropriate: `python scripts/update_version.py -v <version>`. The version number must comply with [PEP 440](https://peps.python.org/pep-0440/).
 
 3.  Lint Python files: `python scripts/pull_request_prepare.py`
 
 4.  Commit and push the updated `develop` branch.
 
 
 #### Publish the release
```

### Comparing `flopy-3.4.0/docs/mf6.md` & `flopy-3.4.1/docs/mf6.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/mf6_dev_guide.md` & `flopy-3.4.1/docs/mf6_dev_guide.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/model_checks.md` & `flopy-3.4.1/docs/model_checks.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/script_examples.md` & `flopy-3.4.1/docs/script_examples.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/supported_packages.md` & `flopy-3.4.1/docs/supported_packages.md`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/docs/version_changes.md` & `flopy-3.4.1/docs/version_changes.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+### Version 3.4.1
+
+#### Bug fixes
+
+* [fix(get-modflow)](https://github.com/modflowpy/flopy/commit/b8dffbc6bc7bee70d18d7ec24c96e33517e4f0e8): Accommodate mf6 release asset name change (#1855). Committed by w-bonelli on 2023-06-29.
+
 ### Version 3.4.0
 
 #### New features
 
 * [feat(Simulation)](https://github.com/modflowpy/flopy/commit/e2cbb25ce6356fa44d9ed4ba4460674f3b9e6760): Support pathlike (#1712). Committed by aleaf on 2023-02-13.
 * [feat(solvers)](https://github.com/modflowpy/flopy/commit/ea04e83ed6199bd93fd6926e58a16a2d0d6686e1): Support for multiple solver types (#1706) (#1709). Committed by spaulins-usgs on 2023-02-15.
 * [feat(pathlike)](https://github.com/modflowpy/flopy/commit/656751a5d34c74e9a16ba39fce7cb85505888cc4): Support pathlike in user-facing APIs (#1730). Committed by w-bonelli on 2023-03-03.
```

### Comparing `flopy-3.4.0/flopy/__init__.py` & `flopy-3.4.1/flopy/__init__.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/datbase.py` & `flopy-3.4.1/flopy/datbase.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/discretization/grid.py` & `flopy-3.4.1/flopy/discretization/grid.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/discretization/modeltime.py` & `flopy-3.4.1/flopy/discretization/modeltime.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/discretization/structuredgrid.py` & `flopy-3.4.1/flopy/discretization/structuredgrid.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/discretization/unstructuredgrid.py` & `flopy-3.4.1/flopy/discretization/unstructuredgrid.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/discretization/vertexgrid.py` & `flopy-3.4.1/flopy/discretization/vertexgrid.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/longnames.py` & `flopy-3.4.1/flopy/export/longnames.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/metadata.py` & `flopy-3.4.1/flopy/export/metadata.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/netcdf.py` & `flopy-3.4.1/flopy/export/netcdf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/shapefile_utils.py` & `flopy-3.4.1/flopy/export/shapefile_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/unitsformat.py` & `flopy-3.4.1/flopy/export/unitsformat.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/utils.py` & `flopy-3.4.1/flopy/export/utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/export/vtk.py` & `flopy-3.4.1/flopy/export/vtk.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mbase.py` & `flopy-3.4.1/flopy/mbase.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/coordinates/modeldimensions.py` & `flopy-3.4.1/flopy/mf6/coordinates/modeldimensions.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/coordinates/modelgrid.py` & `flopy-3.4.1/flopy/mf6/coordinates/modelgrid.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/coordinates/simulationtime.py` & `flopy-3.4.1/flopy/mf6/coordinates/simulationtime.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/common.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/common.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/exg-gwfgwf.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/exg-gwfgwf.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/exg-gwtgwt.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/exg-gwtgwt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-api.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-api.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-buy.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-buy.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-chd.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-chd.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-csub.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-csub.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-dis.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-dis.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-disu.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-disu.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-disv.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-disv.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-drn.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-drn.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-evt.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-evt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-evta.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-evta.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-ghb.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-ghb.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-gnc.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-gnc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-hfb.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-hfb.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-ic.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-ic.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-lak.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-lak.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-maw.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-maw.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-mvr.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-mvr.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-nam.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-nam.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-npf.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-npf.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-oc.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-oc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-rch.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-rch.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-rcha.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-rcha.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-riv.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-riv.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-sfr.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-sfr.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-sto.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-sto.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-uzf.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-uzf.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-vsc.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-vsc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwf-wel.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwf-wel.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-api.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-api.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-cnc.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-cnc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-dis.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-dis.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-disu.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-disu.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-disv.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-disv.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-dsp.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-dsp.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-fmi.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-fmi.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-ist.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-ist.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-lkt.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-lkt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-mst.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-mst.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-mvt.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-mvt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-mwt.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-mwt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-nam.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-nam.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-oc.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-oc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-sft.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-sft.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-src.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-src.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-ssm.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-ssm.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/gwt-uzt.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/gwt-uzt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/sim-nam.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/sim-nam.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/sim-tdis.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/sim-tdis.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/sln-ims.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/sln-ims.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-ats.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-ats.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-laktab.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-laktab.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-obs.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-obs.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-sfrtab.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-sfrtab.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-spc.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-spc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-spca.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-spca.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-tas.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-tas.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-ts.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-ts.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-tvk.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-tvk.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/dfn/utl-tvs.dfn` & `flopy-3.4.1/flopy/mf6/data/dfn/utl-tvs.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfdata.py` & `flopy-3.4.1/flopy/mf6/data/mfdata.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfdataarray.py` & `flopy-3.4.1/flopy/mf6/data/mfdataarray.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfdatalist.py` & `flopy-3.4.1/flopy/mf6/data/mfdatalist.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfdatascalar.py` & `flopy-3.4.1/flopy/mf6/data/mfdatascalar.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfdatastorage.py` & `flopy-3.4.1/flopy/mf6/data/mfdatastorage.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfdatautil.py` & `flopy-3.4.1/flopy/mf6/data/mfdatautil.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mffileaccess.py` & `flopy-3.4.1/flopy/mf6/data/mffileaccess.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/data/mfstructure.py` & `flopy-3.4.1/flopy/mf6/data/mfstructure.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/mfbase.py` & `flopy-3.4.1/flopy/mf6/mfbase.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/mfmodel.py` & `flopy-3.4.1/flopy/mf6/mfmodel.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/mfpackage.py` & `flopy-3.4.1/flopy/mf6/mfpackage.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/modflow/__init__.py` & `flopy-3.4.1/flopy/mf6/modflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfems.py` & `flopy-3.4.1/flopy/mf6/modflow/mfems.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 
 
 class ModflowEms(mfpackage.MFPackage):
     """
     ModflowEms defines a ems package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgnc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgnc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGnc(mfpackage.MFPackage):
     """
     ModflowGnc defines a gnc package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwf.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfmodel
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwf(mfmodel.MFModel):
     """
     Modflowgwf defines a gwf model
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfapi.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfapi(mfpackage.MFPackage):
     """
     ModflowGwfapi defines a api package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfbuy.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfbuy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfbuy(mfpackage.MFPackage):
     """
     ModflowGwfbuy defines a buy package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfchd.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfchd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfchd(mfpackage.MFPackage):
     """
     ModflowGwfchd defines a chd package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfcsub.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfcsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfcsub(mfpackage.MFPackage):
     """
     ModflowGwfcsub defines a csub package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfdis.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfdis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwfdis(mfpackage.MFPackage):
     """
     ModflowGwfdis defines a dis package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfdisu.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfdisu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfdisu(mfpackage.MFPackage):
     """
     ModflowGwfdisu defines a disu package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfdisv.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfdisv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfdisv(mfpackage.MFPackage):
     """
     ModflowGwfdisv defines a disv package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfdrn.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfdrn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfdrn(mfpackage.MFPackage):
     """
     ModflowGwfdrn defines a drn package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfevt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfevt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfevt(mfpackage.MFPackage):
     """
     ModflowGwfevt defines a evt package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfevta.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfevta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfevta(mfpackage.MFPackage):
     """
     ModflowGwfevta defines a evta package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfghb.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfghb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfghb(mfpackage.MFPackage):
     """
     ModflowGwfghb defines a ghb package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfgnc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfgnc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfgnc(mfpackage.MFPackage):
     """
     ModflowGwfgnc defines a gnc package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfgwf.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfgwf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:47 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfgwf(mfpackage.MFPackage):
     """
     ModflowGwfgwf defines a gwfgwf package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfgwt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfgwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 
 
 class ModflowGwfgwt(mfpackage.MFPackage):
     """
     ModflowGwfgwt defines a gwfgwt package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfhfb.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfhfb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfhfb(mfpackage.MFPackage):
     """
     ModflowGwfhfb defines a hfb package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfic.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwfic(mfpackage.MFPackage):
     """
     ModflowGwfic defines a ic package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwflak.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwflak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwflak(mfpackage.MFPackage):
     """
     ModflowGwflak defines a lak package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfmaw.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfmaw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfmaw(mfpackage.MFPackage):
     """
     ModflowGwfmaw defines a maw package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfmvr.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfmvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfmvr(mfpackage.MFPackage):
     """
     ModflowGwfmvr defines a mvr package within a gwf6 model. This package
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfnam.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfnam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfnam(mfpackage.MFPackage):
     """
     ModflowGwfnam defines a nam package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfnpf.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfnpf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfnpf(mfpackage.MFPackage):
     """
     ModflowGwfnpf defines a npf package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfoc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfoc(mfpackage.MFPackage):
     """
     ModflowGwfoc defines a oc package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfrch.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfrch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfrch(mfpackage.MFPackage):
     """
     ModflowGwfrch defines a rch package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfrcha.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfrcha.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfrcha(mfpackage.MFPackage):
     """
     ModflowGwfrcha defines a rcha package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfriv.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfriv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfriv(mfpackage.MFPackage):
     """
     ModflowGwfriv defines a riv package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfsfr.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfsfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfsfr(mfpackage.MFPackage):
     """
     ModflowGwfsfr defines a sfr package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfsto.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfsto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfsto(mfpackage.MFPackage):
     """
     ModflowGwfsto defines a sto package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfuzf.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfuzf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfuzf(mfpackage.MFPackage):
     """
     ModflowGwfuzf defines a uzf package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfvsc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfvsc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfvsc(mfpackage.MFPackage):
     """
     ModflowGwfvsc defines a vsc package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwfwel.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwfwel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfwel(mfpackage.MFPackage):
     """
     ModflowGwfwel defines a wel package within a gwf6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfmodel
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwt(mfmodel.MFModel):
     """
     Modflowgwt defines a gwt model
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtadv.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtadv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 
 
 class ModflowGwtadv(mfpackage.MFPackage):
     """
     ModflowGwtadv defines a adv package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtapi.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtapi(mfpackage.MFPackage):
     """
     ModflowGwtapi defines a api package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtcnc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtcnc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtcnc(mfpackage.MFPackage):
     """
     ModflowGwtcnc defines a cnc package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtdis.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtdis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtdis(mfpackage.MFPackage):
     """
     ModflowGwtdis defines a dis package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtdisu.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtdisu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwtdisu(mfpackage.MFPackage):
     """
     ModflowGwtdisu defines a disu package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtdisv.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtdisv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwtdisv(mfpackage.MFPackage):
     """
     ModflowGwtdisv defines a disv package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtdsp.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtdsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtdsp(mfpackage.MFPackage):
     """
     ModflowGwtdsp defines a dsp package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtfmi.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtfmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtfmi(mfpackage.MFPackage):
     """
     ModflowGwtfmi defines a fmi package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtgwt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtgwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtgwt(mfpackage.MFPackage):
     """
     ModflowGwtgwt defines a gwtgwt package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtic.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtic(mfpackage.MFPackage):
     """
     ModflowGwtic defines a ic package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtist.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwtist(mfpackage.MFPackage):
     """
     ModflowGwtist defines a ist package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtlkt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtlkt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtlkt(mfpackage.MFPackage):
     """
     ModflowGwtlkt defines a lkt package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtmst.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtmst.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtmst(mfpackage.MFPackage):
     """
     ModflowGwtmst defines a mst package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtmvt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtmvt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtmvt(mfpackage.MFPackage):
     """
     ModflowGwtmvt defines a mvt package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtmwt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtmwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtmwt(mfpackage.MFPackage):
     """
     ModflowGwtmwt defines a mwt package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtnam.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtnam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtnam(mfpackage.MFPackage):
     """
     ModflowGwtnam defines a nam package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtoc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtoc(mfpackage.MFPackage):
     """
     ModflowGwtoc defines a oc package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtsft.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtsft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtsft(mfpackage.MFPackage):
     """
     ModflowGwtsft defines a sft package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtsrc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtsrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtsrc(mfpackage.MFPackage):
     """
     ModflowGwtsrc defines a src package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtssm.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtssm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtssm(mfpackage.MFPackage):
     """
     ModflowGwtssm defines a ssm package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfgwtuzt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfgwtuzt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtuzt(mfpackage.MFPackage):
     """
     ModflowGwtuzt defines a uzt package within a gwt6 model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfims.py` & `flopy-3.4.1/flopy/mf6/modflow/mfims.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:47 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowIms(mfpackage.MFPackage):
     """
     ModflowIms defines a ims package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfmvr.py` & `flopy-3.4.1/flopy/mf6/modflow/mfmvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:47 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowMvr(mfpackage.MFPackage):
     """
     ModflowMvr defines a mvr package. This package can only be used to move
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfmvt.py` & `flopy-3.4.1/flopy/mf6/modflow/mfmvt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowMvt(mfpackage.MFPackage):
     """
     ModflowMvt defines a mvt package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfnam.py` & `flopy-3.4.1/flopy/mf6/modflow/mfnam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:47 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowNam(mfpackage.MFPackage):
     """
     ModflowNam defines a nam package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfsimulation.py` & `flopy-3.4.1/flopy/mf6/modflow/mfsimulation.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mftdis.py` & `flopy-3.4.1/flopy/mf6/modflow/mftdis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:47 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowTdis(mfpackage.MFPackage):
     """
     ModflowTdis defines a tdis package.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutlats.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutlats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlats(mfpackage.MFPackage):
     """
     ModflowUtlats defines a ats package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutllaktab.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutllaktab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtllaktab(mfpackage.MFPackage):
     """
     ModflowUtllaktab defines a laktab package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutlobs.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutlobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlobs(mfpackage.MFPackage):
     """
     ModflowUtlobs defines a obs package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutlsfrtab.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutlsfrtab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlsfrtab(mfpackage.MFPackage):
     """
     ModflowUtlsfrtab defines a sfrtab package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutlspc.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutlspc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlspc(mfpackage.MFPackage):
     """
     ModflowUtlspc defines a spc package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutlspca.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutlspca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowUtlspca(mfpackage.MFPackage):
     """
     ModflowUtlspca defines a spca package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutltas.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutltas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowUtltas(mfpackage.MFPackage):
     """
     ModflowUtltas defines a tas package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutlts.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutlts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlts(mfpackage.MFPackage):
     """
     ModflowUtlts defines a ts package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutltvk.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutltvk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtltvk(mfpackage.MFPackage):
     """
     ModflowUtltvk defines a tvk package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/modflow/mfutltvs.py` & `flopy-3.4.1/flopy/mf6/modflow/mfutltvs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on June 29, 2023 01:58:48 UTC
+# FILE created on June 29, 2023 14:20:38 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtltvs(mfpackage.MFPackage):
     """
     ModflowUtltvs defines a tvs package within a utl model.
```

### Comparing `flopy-3.4.0/flopy/mf6/utils/binaryfile_utils.py` & `flopy-3.4.1/flopy/mf6/utils/binaryfile_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/binarygrid_util.py` & `flopy-3.4.1/flopy/mf6/utils/binarygrid_util.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/createpackages.py` & `flopy-3.4.1/flopy/mf6/utils/createpackages.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/generate_classes.py` & `flopy-3.4.1/flopy/mf6/utils/generate_classes.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/lakpak_utils.py` & `flopy-3.4.1/flopy/mf6/utils/lakpak_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/mfobservation.py` & `flopy-3.4.1/flopy/mf6/utils/mfobservation.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/model_splitter.py` & `flopy-3.4.1/flopy/mf6/utils/model_splitter.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/output_util.py` & `flopy-3.4.1/flopy/mf6/utils/output_util.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/postprocessing.py` & `flopy-3.4.1/flopy/mf6/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/reference.py` & `flopy-3.4.1/flopy/mf6/utils/reference.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mf6/utils/testutils.py` & `flopy-3.4.1/flopy/mf6/utils/testutils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/cln_dtypes.py` & `flopy-3.4.1/flopy/mfusg/cln_dtypes.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusg.py` & `flopy-3.4.1/flopy/mfusg/mfusg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusgbcf.py` & `flopy-3.4.1/flopy/mfusg/mfusgbcf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusgcln.py` & `flopy-3.4.1/flopy/mfusg/mfusgcln.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusgdisu.py` & `flopy-3.4.1/flopy/mfusg/mfusgdisu.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusggnc.py` & `flopy-3.4.1/flopy/mfusg/mfusggnc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusglpf.py` & `flopy-3.4.1/flopy/mfusg/mfusglpf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusgsms.py` & `flopy-3.4.1/flopy/mfusg/mfusgsms.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mfusg/mfusgwel.py` & `flopy-3.4.1/flopy/mfusg/mfusgwel.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/__init__.py` & `flopy-3.4.1/flopy/modflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mf.py` & `flopy-3.4.1/flopy/modflow/mf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfag.py` & `flopy-3.4.1/flopy/modflow/mfag.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfbas.py` & `flopy-3.4.1/flopy/modflow/mfbas.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfbcf.py` & `flopy-3.4.1/flopy/modflow/mfbcf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfbct.py` & `flopy-3.4.1/flopy/modflow/mfbct.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfchd.py` & `flopy-3.4.1/flopy/modflow/mfchd.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfde4.py` & `flopy-3.4.1/flopy/modflow/mfde4.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfdis.py` & `flopy-3.4.1/flopy/modflow/mfdis.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfdrn.py` & `flopy-3.4.1/flopy/modflow/mfdrn.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfdrt.py` & `flopy-3.4.1/flopy/modflow/mfdrt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfevt.py` & `flopy-3.4.1/flopy/modflow/mfevt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mffhb.py` & `flopy-3.4.1/flopy/modflow/mffhb.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfflwob.py` & `flopy-3.4.1/flopy/modflow/mfflwob.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfgage.py` & `flopy-3.4.1/flopy/modflow/mfgage.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfghb.py` & `flopy-3.4.1/flopy/modflow/mfghb.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfgmg.py` & `flopy-3.4.1/flopy/modflow/mfgmg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfhfb.py` & `flopy-3.4.1/flopy/modflow/mfhfb.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfhob.py` & `flopy-3.4.1/flopy/modflow/mfhob.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfhyd.py` & `flopy-3.4.1/flopy/modflow/mfhyd.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mflak.py` & `flopy-3.4.1/flopy/modflow/mflak.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mflmt.py` & `flopy-3.4.1/flopy/modflow/mflmt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mflpf.py` & `flopy-3.4.1/flopy/modflow/mflpf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfmlt.py` & `flopy-3.4.1/flopy/modflow/mfmlt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfmnw1.py` & `flopy-3.4.1/flopy/modflow/mfmnw1.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfmnw2.py` & `flopy-3.4.1/flopy/modflow/mfmnw2.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfmnwi.py` & `flopy-3.4.1/flopy/modflow/mfmnwi.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfnwt.py` & `flopy-3.4.1/flopy/modflow/mfnwt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfoc.py` & `flopy-3.4.1/flopy/modflow/mfoc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfpar.py` & `flopy-3.4.1/flopy/modflow/mfpar.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfparbc.py` & `flopy-3.4.1/flopy/modflow/mfparbc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfpbc.py` & `flopy-3.4.1/flopy/modflow/mfpbc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfpcg.py` & `flopy-3.4.1/flopy/modflow/mfpcg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfpcgn.py` & `flopy-3.4.1/flopy/modflow/mfpcgn.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfpks.py` & `flopy-3.4.1/flopy/modflow/mfpks.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfpval.py` & `flopy-3.4.1/flopy/modflow/mfpval.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfrch.py` & `flopy-3.4.1/flopy/modflow/mfrch.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfriv.py` & `flopy-3.4.1/flopy/modflow/mfriv.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfsfr2.py` & `flopy-3.4.1/flopy/modflow/mfsfr2.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfsip.py` & `flopy-3.4.1/flopy/modflow/mfsip.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfsor.py` & `flopy-3.4.1/flopy/modflow/mfsor.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfstr.py` & `flopy-3.4.1/flopy/modflow/mfstr.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfsub.py` & `flopy-3.4.1/flopy/modflow/mfsub.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfswi2.py` & `flopy-3.4.1/flopy/modflow/mfswi2.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfswr1.py` & `flopy-3.4.1/flopy/modflow/mfswr1.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfswt.py` & `flopy-3.4.1/flopy/modflow/mfswt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfupw.py` & `flopy-3.4.1/flopy/modflow/mfupw.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfuzf1.py` & `flopy-3.4.1/flopy/modflow/mfuzf1.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfwel.py` & `flopy-3.4.1/flopy/modflow/mfwel.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflow/mfzon.py` & `flopy-3.4.1/flopy/modflow/mfzon.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modflowlgr/mflgr.py` & `flopy-3.4.1/flopy/modflowlgr/mflgr.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp6.py` & `flopy-3.4.1/flopy/modpath/mp6.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp6bas.py` & `flopy-3.4.1/flopy/modpath/mp6bas.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp6sim.py` & `flopy-3.4.1/flopy/modpath/mp6sim.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp7.py` & `flopy-3.4.1/flopy/modpath/mp7.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp7bas.py` & `flopy-3.4.1/flopy/modpath/mp7bas.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp7particledata.py` & `flopy-3.4.1/flopy/modpath/mp7particledata.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp7particlegroup.py` & `flopy-3.4.1/flopy/modpath/mp7particlegroup.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/modpath/mp7sim.py` & `flopy-3.4.1/flopy/modpath/mp7sim.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mt.py` & `flopy-3.4.1/flopy/mt3d/mt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtadv.py` & `flopy-3.4.1/flopy/mt3d/mtadv.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtbtn.py` & `flopy-3.4.1/flopy/mt3d/mtbtn.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtcts.py` & `flopy-3.4.1/flopy/mt3d/mtcts.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtdsp.py` & `flopy-3.4.1/flopy/mt3d/mtdsp.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtgcg.py` & `flopy-3.4.1/flopy/mt3d/mtgcg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtlkt.py` & `flopy-3.4.1/flopy/mt3d/mtlkt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtphc.py` & `flopy-3.4.1/flopy/mt3d/mtphc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtrct.py` & `flopy-3.4.1/flopy/mt3d/mtrct.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtsft.py` & `flopy-3.4.1/flopy/mt3d/mtsft.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtssm.py` & `flopy-3.4.1/flopy/mt3d/mtssm.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mttob.py` & `flopy-3.4.1/flopy/mt3d/mttob.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/mt3d/mtuzt.py` & `flopy-3.4.1/flopy/mt3d/mtuzt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/pakbase.py` & `flopy-3.4.1/flopy/pakbase.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/pest/params.py` & `flopy-3.4.1/flopy/pest/params.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/pest/templatewriter.py` & `flopy-3.4.1/flopy/pest/templatewriter.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/pest/tplarray.py` & `flopy-3.4.1/flopy/pest/tplarray.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/crosssection.py` & `flopy-3.4.1/flopy/plot/crosssection.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/map.py` & `flopy-3.4.1/flopy/plot/map.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/mplstyle/usgsmap.mplstyle` & `flopy-3.4.1/flopy/plot/mplstyle/usgsmap.mplstyle`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/mplstyle/usgsmap_linux.mplstyle` & `flopy-3.4.1/flopy/plot/mplstyle/usgsmap_linux.mplstyle`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/mplstyle/usgsplot.mplstyle` & `flopy-3.4.1/flopy/plot/mplstyle/usgsplot.mplstyle`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/mplstyle/usgsplot_linux.mplstyle` & `flopy-3.4.1/flopy/plot/mplstyle/usgsplot_linux.mplstyle`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/plotutil.py` & `flopy-3.4.1/flopy/plot/plotutil.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/plot/styles.py` & `flopy-3.4.1/flopy/plot/styles.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/seawat/swt.py` & `flopy-3.4.1/flopy/seawat/swt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/seawat/swtvdf.py` & `flopy-3.4.1/flopy/seawat/swtvdf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/seawat/swtvsc.py` & `flopy-3.4.1/flopy/seawat/swtvsc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/__init__.py` & `flopy-3.4.1/flopy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/binaryfile.py` & `flopy-3.4.1/flopy/utils/binaryfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/check.py` & `flopy-3.4.1/flopy/utils/check.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/compare.py` & `flopy-3.4.1/flopy/utils/compare.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/crs.py` & `flopy-3.4.1/flopy/utils/crs.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/cvfdutil.py` & `flopy-3.4.1/flopy/utils/cvfdutil.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/datafile.py` & `flopy-3.4.1/flopy/utils/datafile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/datautil.py` & `flopy-3.4.1/flopy/utils/datautil.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/flopy_io.py` & `flopy-3.4.1/flopy/utils/flopy_io.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/formattedfile.py` & `flopy-3.4.1/flopy/utils/formattedfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/geometry.py` & `flopy-3.4.1/flopy/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/geospatial_utils.py` & `flopy-3.4.1/flopy/utils/geospatial_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/get_modflow.py` & `flopy-3.4.1/flopy/utils/get_modflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,26 +392,22 @@
             f"repo {repo!r} not supported; choose one of {available_repos}"
         )
 
     # get the selected release
     release = get_release(repo, release_id, quiet)
     assets = release.get("assets", [])
 
-    # Windows 64-bit asset in modflow6 repo release has no OS tag
-    if repo == "modflow6" and ostag == "win64":
-        asset = list(sorted(assets, key=lambda a: len(a["name"])))[0]
+    for asset in assets:
+        if ostag in asset["name"]:
+            break
     else:
-        for asset in assets:
-            if ostag in asset["name"]:
-                break
-        else:
-            raise ValueError(
-                f"could not find ostag {ostag!r} from release {release['tag_name']!r}; "
-                f"see available assets here:\n{release['html_url']}"
-            )
+        raise ValueError(
+            f"could not find ostag {ostag!r} from release {release['tag_name']!r}; "
+            f"see available assets here:\n{release['html_url']}"
+        )
     asset_name = asset["name"]
     download_url = asset["browser_download_url"]
     if repo == "modflow6":
         asset_pth = Path(asset_name)
         asset_stem = asset_pth.stem
         asset_suffix = asset_pth.suffix
         dst_fname = "-".join([repo, release["tag_name"], ostag]) + asset_suffix
```

### Comparing `flopy-3.4.0/flopy/utils/gridgen.py` & `flopy-3.4.1/flopy/utils/gridgen.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/gridintersect.py` & `flopy-3.4.1/flopy/utils/gridintersect.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/gridutil.py` & `flopy-3.4.1/flopy/utils/gridutil.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/lgrutil.py` & `flopy-3.4.1/flopy/utils/lgrutil.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/mflistfile.py` & `flopy-3.4.1/flopy/utils/mflistfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/mfreadnam.py` & `flopy-3.4.1/flopy/utils/mfreadnam.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/modpathfile.py` & `flopy-3.4.1/flopy/utils/modpathfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/mtlistfile.py` & `flopy-3.4.1/flopy/utils/mtlistfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/observationfile.py` & `flopy-3.4.1/flopy/utils/observationfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/optionblock.py` & `flopy-3.4.1/flopy/utils/optionblock.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/parse_version.py` & `flopy-3.4.1/flopy/utils/parse_version.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/postprocessing.py` & `flopy-3.4.1/flopy/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/rasters.py` & `flopy-3.4.1/flopy/utils/rasters.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/recarray_utils.py` & `flopy-3.4.1/flopy/utils/recarray_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/reference.py` & `flopy-3.4.1/flopy/utils/reference.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/sfroutputfile.py` & `flopy-3.4.1/flopy/utils/sfroutputfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/swroutputfile.py` & `flopy-3.4.1/flopy/utils/swroutputfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/triangle.py` & `flopy-3.4.1/flopy/utils/triangle.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/util_array.py` & `flopy-3.4.1/flopy/utils/util_array.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/util_list.py` & `flopy-3.4.1/flopy/utils/util_list.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/utils_def.py` & `flopy-3.4.1/flopy/utils/utils_def.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/utl_import.py` & `flopy-3.4.1/flopy/utils/utl_import.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/voronoi.py` & `flopy-3.4.1/flopy/utils/voronoi.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy/utils/zonbud.py` & `flopy-3.4.1/flopy/utils/zonbud.py`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy.egg-info/PKG-INFO` & `flopy-3.4.1/flopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flopy
-Version: 3.4.0
+Version: 3.4.1
 Summary: FloPy is a Python package to create, run, and post-process MODFLOW-based models
 Author-email: FloPy Team <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://flopy.readthedocs.io
 Project-URL: Release Notes, https://github.com/modflowpy/flopy/blob/develop/docs/version_changes.md
 Project-URL: Bug Tracker, https://github.com/modflowpy/flopy/issues
@@ -55,15 +55,15 @@
 
 *Citation for FloPy:*
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 *Software/Code citation for FloPy:*
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.0: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2023, FloPy v3.4.1: U.S. Geological Survey Software Release, 29 June 2023, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Disclaimer
 ----------
 
 This software is provided "as is" and "as-available", and makes no 
 representations or warranties of any kind concerning the software, whether
```

### Comparing `flopy-3.4.0/flopy.egg-info/SOURCES.txt` & `flopy-3.4.1/flopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flopy-3.4.0/flopy.egg-info/requires.txt` & `flopy-3.4.1/flopy.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -53,7 +53,8 @@
 pytest
 pytest-benchmark
 pytest-cases
 pytest-cov
 pytest-dotenv
 pytest-virtualenv
 pytest-xdist
+virtualenv
```

### Comparing `flopy-3.4.0/pyproject.toml` & `flopy-3.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "pytest",
     "pytest-benchmark",
     "pytest-cases",
     "pytest-cov",
     "pytest-dotenv",
     "pytest-virtualenv",
     "pytest-xdist",
+    "virtualenv"
 ]
 optional = [
     "affine",
     "descartes",
     "fiona",
     "geojson",
     "imageio",
```

