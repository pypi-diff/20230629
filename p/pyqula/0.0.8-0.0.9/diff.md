# Comparing `tmp/pyqula-0.0.8.tar.gz` & `tmp/pyqula-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/joselado/Documents/programs/pyqula/dist/tmpzd892je1/pyqula-0.0.8.tar", last modified: Sun Aug  8 15:54:44 2021, max compression
+gzip compressed data, was "/home/joselado/Documents/programs/pyqula/dist/tmpkke3qxgi/pyqula-0.0.9.tar", last modified: Sun Sep 19 06:49:23 2021, max compression
```

## Comparing `pyqula-0.0.8.tar` & `pyqula-0.0.9.tar`

### file list

```diff
@@ -1,196 +1,203 @@
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.758593 pyqula-0.0.8/
--rw-r--r--   0 joselado  (1000) joselado  (1000)    35141 2021-07-28 06:45:35.000000 pyqula-0.0.8/LICENSE.md
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     5912 2021-08-08 15:54:44.754593 pyqula-0.0.8/PKG-INFO
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5361 2021-08-08 08:05:01.000000 pyqula-0.0.8/README.md
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      104 2021-07-28 14:47:45.000000 pyqula-0.0.8/pyproject.toml
--rw-rw-r--   0 joselado  (1000) joselado  (1000)       38 2021-08-08 15:54:44.758593 pyqula-0.0.8/setup.cfg
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      811 2021-08-08 15:54:36.000000 pyqula-0.0.8/setup.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.742593 pyqula-0.0.8/src/
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/
--rw-r--r--   0 joselado  (1000) joselado  (1000)      663 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6348 2021-07-28 15:34:45.000000 pyqula-0.0.8/src/pyqula/algebra.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/algebratk/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:56:12.000000 pyqula-0.0.8/src/pyqula/algebratk/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      385 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/algebratk/hamiltonianalgebra.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      891 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/algebratk/matrixcrop.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1615 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/algebratk/sparsetensor.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)       92 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/alloy.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4142 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/angular.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     7739 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/bandstructure.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1566 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/check.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      156 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/checkclass.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3675 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/chi.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/chitk/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:36.000000 pyqula-0.0.8/src/pyqula/chitk/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     2369 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/chitk/epsilon.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     3997 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/chitk/qpi.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    11107 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/classicalspin.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      365 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/clean.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2123 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/compilefortran.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      535 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/convolution.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1860 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/correlator.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1937 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/crystalfield.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2716 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/current.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      476 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/data.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2349 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/density.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3969 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/densitymatrix.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      280 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/diagonalize.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      711 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/disorder.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3961 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/disorder_heterostructure.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    18327 2021-07-29 04:57:10.000000 pyqula-0.0.8/src/pyqula/dos.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3297 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/dyson.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      712 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/effective.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     9842 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/embedding.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/energeticstk/
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:11.000000 pyqula-0.0.8/src/pyqula/energeticstk/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     7527 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/energeticstk/alloytk.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1237 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/estimators.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     7397 2021-08-04 10:43:03.000000 pyqula-0.0.8/src/pyqula/extract.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3160 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/fermisurface.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      495 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/filesystem.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1363 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/films.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/fitting.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6678 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/gap.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1514 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/gauge.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    49161 2021-08-04 11:28:18.000000 pyqula-0.0.8/src/pyqula/geometry.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/geometrytk/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:52:15.000000 pyqula-0.0.8/src/pyqula/geometrytk/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     1042 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/geometrytk/readgeometry.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    24218 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/green.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2906 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/groundstate.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1036 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/gsenergy.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1816 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/hall.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    35286 2021-08-06 10:10:46.000000 pyqula-0.0.8/src/pyqula/hamiltonians.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      125 2021-08-03 13:42:09.000000 pyqula-0.0.8/src/pyqula/helptk.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    40466 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/heterostructures.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4327 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/hexagonal.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/htk/
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2644 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/eigenvectors.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      592 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/fusion.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     2086 2021-08-07 12:17:00.000000 pyqula-0.0.8/src/pyqula/htk/g2h.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      907 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/hamiltonianmodify.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1337 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/matrixcomponent.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1546 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/mode.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      661 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/htk/symmetry.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2964 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/hybrid.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2923 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/increase_hilbert.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1388 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/indexing.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2157 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/inout.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2585 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/integration.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/interactions/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:55:04.000000 pyqula-0.0.8/src/pyqula/interactions/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     1435 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/interactions/vijkl.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/interpolatetk/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:24.000000 pyqula-0.0.8/src/pyqula/interpolatetk/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     2235 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/interpolatetk/atomicinterpolation.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2321 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/interpolation.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1151 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ipr.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1789 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/islands.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5065 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/junctions.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    16781 2021-07-29 04:57:47.000000 pyqula-0.0.8/src/pyqula/kanemele.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    12103 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/kdos.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      345 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/kdotp.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5568 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/kekule.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5822 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/keldysh.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     8545 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/klist.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    15449 2021-07-29 04:58:02.000000 pyqula-0.0.8/src/pyqula/kpm.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1811 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/kwantlink.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    17596 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ldos.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/ldostk/
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ldostk/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6597 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ldostk/atomicmultildos.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1799 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ldostk/ldosr.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)       70 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/limits.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     2237 2021-07-28 06:49:26.000000 pyqula-0.0.8/src/pyqula/magneticexchange.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5927 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/magnetism.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2471 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/massive_green.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    15573 2021-08-03 09:22:40.000000 pyqula-0.0.8/src/pyqula/meanfield.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1280 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/merge.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4793 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/mullen.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    20645 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/multicell.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4152 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/multihopping.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     9083 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/multilayers.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4434 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/multiterminal.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     7264 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/neighbor.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1090 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/nodes.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/nonhermitian/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:01.000000 pyqula-0.0.8/src/pyqula/nonhermitian/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      540 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/nonhermitian/orthogonality.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1093 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/numbaneighbor.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6784 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/old_chi.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3562 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/operatorlist.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    20997 2021-08-06 05:53:35.000000 pyqula-0.0.8/src/pyqula/operators.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2433 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/parallel.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3823 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/parallelslurm.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6257 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/peierls.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2376 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/phasediagram.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6182 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/potentials.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1023 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/pseudocontact.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2904 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/rashba.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     1555 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/reciprocalmap.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      965 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/reduce.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1515 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/response.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1394 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ribbon.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3027 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/ribbonizate.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4193 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/rkky.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6703 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/rotate_spin.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      834 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/sanitycheck.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/scftk/
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/scftk/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3156 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/scftk/updatescf.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    25529 2021-07-29 04:58:13.000000 pyqula-0.0.8/src/pyqula/scftypes.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/sctk/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:53:45.000000 pyqula-0.0.8/src/pyqula/sctk/__init__.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     5033 2021-08-05 15:42:39.000000 pyqula-0.0.8/src/pyqula/sctk/dvector.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4269 2021-08-03 10:14:03.000000 pyqula-0.0.8/src/pyqula/sctk/extract.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      652 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/sctk/orderparameter.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     4583 2021-08-05 15:53:06.000000 pyqula-0.0.8/src/pyqula/sctk/pairing.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4511 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/sctk/spinless.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    14000 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/sculpt.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/selfconsistency/
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      370 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/accelerate.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2408 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/attractive_hubbard_spinless.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6097 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/coulomb.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    19822 2021-08-06 05:42:52.000000 pyqula-0.0.8/src/pyqula/selfconsistency/densitydensity.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     9815 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/hubbard.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3624 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/mfconstrains.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      760 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/mixing.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      633 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/potentials.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3406 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/selfconsistency/superscf.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     7658 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/skeleton.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      428 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/slabs.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    11693 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/specialgeometry.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     4589 2021-07-28 06:50:08.000000 pyqula-0.0.8/src/pyqula/specialhamiltonian.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6001 2021-07-29 04:58:29.000000 pyqula-0.0.8/src/pyqula/specialhopping.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    17366 2021-08-06 10:02:52.000000 pyqula-0.0.8/src/pyqula/spectrum.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     2315 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/spintexture.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5968 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/spinwaves.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3346 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/states.py
--rw-rw-r--   0 joselado  (1000) joselado  (1000)      140 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/strain.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     6934 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/supercell.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     3123 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/supercell_hamiltonians.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    17526 2021-08-05 15:09:06.000000 pyqula-0.0.8/src/pyqula/superconductivity.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1593 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/surface_TI.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1475 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/susceptibility.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    14348 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/symmetrize.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     5103 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/symmetry.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2796 2021-07-29 05:00:00.000000 pyqula-0.0.8/src/pyqula/tails.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2267 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/timeevolution.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1067 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/timing.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1472 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/tojulia.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    24956 2021-08-08 15:53:45.000000 pyqula-0.0.8/src/pyqula/topology.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/topologytk/
--rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/topologytk/__init__.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     1362 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/topologytk/realspace.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)     2152 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/unfolding.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)      118 2021-08-05 13:56:28.000000 pyqula-0.0.8/src/pyqula/utilities.py
--rw-r--r--   0 joselado  (1000) joselado  (1000)    28979 2021-07-28 06:45:35.000000 pyqula-0.0.8/src/pyqula/wannier.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula/wanniertk/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:53:53.000000 pyqula-0.0.8/src/pyqula/wanniertk/__init__.py
-drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-08-08 15:54:44.754593 pyqula-0.0.8/src/pyqula.egg-info/
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     5912 2021-08-08 15:54:44.000000 pyqula-0.0.8/src/pyqula.egg-info/PKG-INFO
--rw-rw-r--   0 joselado  (1000) joselado  (1000)     4698 2021-08-08 15:54:44.000000 pyqula-0.0.8/src/pyqula.egg-info/SOURCES.txt
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        1 2021-08-08 15:54:44.000000 pyqula-0.0.8/src/pyqula.egg-info/dependency_links.txt
--rw-rw-r--   0 joselado  (1000) joselado  (1000)        7 2021-08-08 15:54:44.000000 pyqula-0.0.8/src/pyqula.egg-info/top_level.txt
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    35141 2021-07-28 06:45:35.000000 pyqula-0.0.9/LICENSE.md
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     5912 2021-09-19 06:49:23.912862 pyqula-0.0.9/PKG-INFO
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5361 2021-08-08 08:05:01.000000 pyqula-0.0.9/README.md
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      104 2021-07-28 14:47:45.000000 pyqula-0.0.9/pyproject.toml
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)       38 2021-09-19 06:49:23.912862 pyqula-0.0.9/setup.cfg
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      811 2021-09-19 06:49:14.000000 pyqula-0.0.9/setup.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.888863 pyqula-0.0.9/src/
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.908863 pyqula-0.0.9/src/pyqula/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      663 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/__init__.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     7152 2021-08-22 08:54:57.000000 pyqula-0.0.9/src/pyqula/algebra.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.908863 pyqula-0.0.9/src/pyqula/algebratk/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:56:12.000000 pyqula-0.0.9/src/pyqula/algebratk/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      385 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/algebratk/hamiltonianalgebra.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      891 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/algebratk/matrixcrop.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1615 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/algebratk/sparsetensor.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      751 2021-08-21 14:27:11.000000 pyqula-0.0.9/src/pyqula/algebratk/unitary.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)       92 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/alloy.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4142 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/angular.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     7591 2021-09-18 14:22:10.000000 pyqula-0.0.9/src/pyqula/bandstructure.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1566 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/check.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      156 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/checkclass.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4328 2021-09-18 15:15:39.000000 pyqula-0.0.9/src/pyqula/chi.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.908863 pyqula-0.0.9/src/pyqula/chitk/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:36.000000 pyqula-0.0.9/src/pyqula/chitk/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     2369 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/chitk/epsilon.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     3997 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/chitk/qpi.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    11107 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/classicalspin.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      365 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/clean.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2123 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/compilefortran.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      602 2021-09-01 12:05:14.000000 pyqula-0.0.9/src/pyqula/convolution.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1860 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/correlator.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1937 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/crystalfield.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2716 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/current.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      476 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/data.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2349 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/density.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3969 2021-08-30 14:02:14.000000 pyqula-0.0.9/src/pyqula/densitymatrix.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      280 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/diagonalize.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      711 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/disorder.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3961 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/disorder_heterostructure.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    19381 2021-09-16 14:51:59.000000 pyqula-0.0.9/src/pyqula/dos.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3297 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/dyson.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      712 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/effective.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     9842 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/embedding.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.908863 pyqula-0.0.9/src/pyqula/energeticstk/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:11.000000 pyqula-0.0.9/src/pyqula/energeticstk/__init__.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     7527 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/energeticstk/alloytk.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1237 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/estimators.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     7397 2021-08-04 10:43:03.000000 pyqula-0.0.9/src/pyqula/extract.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3160 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/fermisurface.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      495 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/filesystem.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1363 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/films.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/fitting.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6678 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/gap.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1514 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/gauge.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    48885 2021-09-05 09:21:28.000000 pyqula-0.0.9/src/pyqula/geometry.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.908863 pyqula-0.0.9/src/pyqula/geometrytk/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:52:15.000000 pyqula-0.0.9/src/pyqula/geometrytk/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     1042 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/geometrytk/readgeometry.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    25486 2021-09-18 14:12:00.000000 pyqula-0.0.9/src/pyqula/green.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2906 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/groundstate.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1036 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/gsenergy.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1816 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/hall.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    33231 2021-08-30 15:45:50.000000 pyqula-0.0.9/src/pyqula/hamiltonians.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      125 2021-08-03 13:42:09.000000 pyqula-0.0.9/src/pyqula/helptk.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    33072 2021-09-16 09:44:18.000000 pyqula-0.0.9/src/pyqula/heterostructures.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4327 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/hexagonal.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/htk/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/htk/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      773 2021-08-29 16:51:38.000000 pyqula-0.0.9/src/pyqula/htk/cdw.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     1290 2021-08-30 15:43:18.000000 pyqula-0.0.9/src/pyqula/htk/dummy.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2644 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/htk/eigenvectors.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      592 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/htk/fusion.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     2086 2021-08-07 12:17:00.000000 pyqula-0.0.9/src/pyqula/htk/g2h.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      907 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/htk/hamiltonianmodify.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1337 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/htk/matrixcomponent.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2135 2021-08-29 16:46:20.000000 pyqula-0.0.9/src/pyqula/htk/mode.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      674 2021-08-29 16:55:10.000000 pyqula-0.0.9/src/pyqula/htk/modify.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      661 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/htk/symmetry.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2964 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/hybrid.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2923 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/increase_hilbert.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1388 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/indexing.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2157 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/inout.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2909 2021-09-01 15:06:12.000000 pyqula-0.0.9/src/pyqula/integration.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/interactions/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:55:04.000000 pyqula-0.0.9/src/pyqula/interactions/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     1435 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/interactions/vijkl.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/interpolatetk/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:24.000000 pyqula-0.0.9/src/pyqula/interpolatetk/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     2235 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/interpolatetk/atomicinterpolation.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      440 2021-08-21 12:38:06.000000 pyqula-0.0.9/src/pyqula/interpolatetk/constrainedinterpolation.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      294 2021-08-21 13:17:20.000000 pyqula-0.0.9/src/pyqula/interpolatetk/outlier.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2321 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/interpolation.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1151 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/ipr.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1789 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/islands.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5065 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/junctions.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    16781 2021-07-29 04:57:47.000000 pyqula-0.0.9/src/pyqula/kanemele.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    12062 2021-08-29 16:40:08.000000 pyqula-0.0.9/src/pyqula/kdos.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      345 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/kdotp.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5568 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/kekule.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5822 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/keldysh.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     8545 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/klist.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    15449 2021-07-29 04:58:02.000000 pyqula-0.0.9/src/pyqula/kpm.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1811 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/kwantlink.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    17671 2021-09-17 06:34:21.000000 pyqula-0.0.9/src/pyqula/ldos.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/ldostk/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/ldostk/__init__.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6597 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/ldostk/atomicmultildos.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1799 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/ldostk/ldosr.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)       70 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/limits.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     2237 2021-07-28 06:49:26.000000 pyqula-0.0.9/src/pyqula/magneticexchange.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5269 2021-08-30 14:16:17.000000 pyqula-0.0.9/src/pyqula/magnetism.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2471 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/massive_green.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    15573 2021-08-03 09:22:40.000000 pyqula-0.0.9/src/pyqula/meanfield.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1280 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/merge.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4793 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/mullen.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    20645 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/multicell.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4152 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/multihopping.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     9083 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/multilayers.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4434 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/multiterminal.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     7264 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/neighbor.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1090 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/nodes.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/nonhermitian/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:54:01.000000 pyqula-0.0.9/src/pyqula/nonhermitian/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      540 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/nonhermitian/orthogonality.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1093 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/numbaneighbor.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6784 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/old_chi.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3562 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/operatorlist.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    20997 2021-08-06 05:53:35.000000 pyqula-0.0.9/src/pyqula/operators.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2433 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/parallel.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3830 2021-08-31 12:47:40.000000 pyqula-0.0.9/src/pyqula/parallelslurm.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6257 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/peierls.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2376 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/phasediagram.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6182 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/potentials.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1023 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/pseudocontact.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2904 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/rashba.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     1555 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/reciprocalmap.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      965 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/reduce.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1515 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/response.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1394 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/ribbon.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3027 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/ribbonizate.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4193 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/rkky.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6703 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/rotate_spin.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)       44 2021-09-18 15:16:23.000000 pyqula-0.0.9/src/pyqula/rpa.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      834 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/sanitycheck.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/scftk/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/scftk/__init__.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3156 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/scftk/updatescf.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    25529 2021-07-29 04:58:13.000000 pyqula-0.0.9/src/pyqula/scftypes.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/sctk/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:53:45.000000 pyqula-0.0.9/src/pyqula/sctk/__init__.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     5033 2021-08-05 15:42:39.000000 pyqula-0.0.9/src/pyqula/sctk/dvector.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4269 2021-08-03 10:14:03.000000 pyqula-0.0.9/src/pyqula/sctk/extract.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      652 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/sctk/orderparameter.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     4852 2021-08-18 15:09:20.000000 pyqula-0.0.9/src/pyqula/sctk/pairing.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4511 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/sctk/spinless.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    14000 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/sculpt.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/selfconsistency/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/__init__.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      370 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/accelerate.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2408 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/attractive_hubbard_spinless.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6097 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/coulomb.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    19822 2021-08-06 05:42:52.000000 pyqula-0.0.9/src/pyqula/selfconsistency/densitydensity.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     9815 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/hubbard.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3624 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/mfconstrains.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      760 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/mixing.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      633 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/potentials.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3406 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/selfconsistency/superscf.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     7658 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/skeleton.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      428 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/slabs.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    11707 2021-08-14 12:19:01.000000 pyqula-0.0.9/src/pyqula/specialgeometry.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     4470 2021-09-12 08:37:55.000000 pyqula-0.0.9/src/pyqula/specialhamiltonian.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6001 2021-07-29 04:58:29.000000 pyqula-0.0.9/src/pyqula/specialhopping.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    17366 2021-08-06 10:02:52.000000 pyqula-0.0.9/src/pyqula/spectrum.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     2315 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/spintexture.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5968 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/spinwaves.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3346 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/states.py
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)      140 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/strain.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     6934 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/supercell.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     3123 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/supercell_hamiltonians.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    17526 2021-08-05 15:09:06.000000 pyqula-0.0.9/src/pyqula/superconductivity.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1593 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/surface_TI.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1475 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/susceptibility.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    14348 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/symmetrize.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     5103 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/symmetry.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2796 2021-07-29 05:00:00.000000 pyqula-0.0.9/src/pyqula/tails.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2267 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/timeevolution.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1067 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/timing.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1472 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/tojulia.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    24956 2021-08-08 15:53:45.000000 pyqula-0.0.9/src/pyqula/topology.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/topologytk/
+-rw-r--r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/topologytk/__init__.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     1362 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/topologytk/realspace.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)     2152 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/unfolding.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)      118 2021-08-05 13:56:28.000000 pyqula-0.0.9/src/pyqula/utilities.py
+-rw-r--r--   0 joselado  (1000) joselado  (1000)    28979 2021-07-28 06:45:35.000000 pyqula-0.0.9/src/pyqula/wannier.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.912862 pyqula-0.0.9/src/pyqula/wanniertk/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        0 2021-07-28 16:53:53.000000 pyqula-0.0.9/src/pyqula/wanniertk/__init__.py
+drwxrwxr-x   0 joselado  (1000) joselado  (1000)        0 2021-09-19 06:49:23.908863 pyqula-0.0.9/src/pyqula.egg-info/
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     5912 2021-09-19 06:49:23.000000 pyqula-0.0.9/src/pyqula.egg-info/PKG-INFO
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)     4908 2021-09-19 06:49:23.000000 pyqula-0.0.9/src/pyqula.egg-info/SOURCES.txt
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        1 2021-09-19 06:49:23.000000 pyqula-0.0.9/src/pyqula.egg-info/dependency_links.txt
+-rw-rw-r--   0 joselado  (1000) joselado  (1000)        7 2021-09-19 06:49:23.000000 pyqula-0.0.9/src/pyqula.egg-info/top_level.txt
```

### Comparing `pyqula-0.0.8/LICENSE.md` & `pyqula-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/PKG-INFO` & `pyqula-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqula
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for quantum lattice tight binding models
 Home-page: https://github.com/joselado/pyqula
 Author: Jose Lado
 Author-email: joselado@aalto.fi
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/joselado/pyqula/issues
 Platform: UNKNOWN
```

### Comparing `pyqula-0.0.8/README.md` & `pyqula-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/setup.py` & `pyqula-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyqula",
-    version="0.0.8",
+    version="0.0.9",
     author="Jose Lado",
     author_email="joselado@aalto.fi",
     description="Python library for quantum lattice tight binding models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joselado/pyqula",
     project_urls={
```

### Comparing `pyqula-0.0.8/src/pyqula/__init__.py` & `pyqula-0.0.9/src/pyqula/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/algebra.py` & `pyqula-0.0.9/src/pyqula/algebra.py`

 * *Files 8% similar despite different names*

```diff
@@ -233,7 +233,35 @@
         if numw<100: return gap(m,numw=2*numw,**kwargs)
         else: raise
     g = np.min(np.abs(ev))+np.min(ec) # gap
     return g # return gap
 
 
 
+
+
+
+
+def sqrtm(M):
+    """Square root for Hermitian matrix"""
+    (m2,evecs) = sqrtm_rotated(M)
+    m2 = dagger(evecs) @ m2 @ evecs  # change of basis
+    return m2 # return matrix
+
+
+
+def sqrtm_rotated(M,positive=True):
+    """Square root for Hermitian matrix in the diagonal basis,
+    and rotation matrix"""
+    M = (M + dagger(M))/2. # make Hermitian
+    (evals,evecs) = dlg.eigh(M) # eigenvals and eigenvecs
+    if positive:
+        if np.min(evals)<0.:
+            print("Matrix is not positive defined")
+            evals[evals<0.] = 1e-7
+    evecs = dagger(np.matrix(evecs)) # change of basis
+    m2 = np.matrix([[0.0j for i in evals] for j in evals]) # create matrix
+    for i in range(len(evals)):
+        m2[i,i] = np.sqrt(np.abs(evals[i])) # square root
+    return (m2,evecs) # return matrix
+
+
```

### Comparing `pyqula-0.0.8/src/pyqula/algebratk/matrixcrop.py` & `pyqula-0.0.9/src/pyqula/algebratk/matrixcrop.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/algebratk/sparsetensor.py` & `pyqula-0.0.9/src/pyqula/algebratk/sparsetensor.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/angular.py` & `pyqula-0.0.9/src/pyqula/angular.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/bandstructure.py` & `pyqula-0.0.9/src/pyqula/bandstructure.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,15 @@
 
 
 
 
 
 
 def ket_Aw(A,w):
-  w = np.matrix([w]).T # transpose()
-  wo = A*w # get a vector
-  wo = np.array(wo)[:,0] # wo
-  return wo
+  return A@w
 
 
 
 
 
 def get_bands_nd(h,kpath=None,operator=None,num_bands=None,
                     callback=None,central_energy=0.0,nk=400,
@@ -98,15 +95,14 @@
       if operator is None: return eig
       else: return (eig,eigvec)
   # open file and get generator
   hkgen = h.get_hk_gen() # generator hamiltonian
   if kpath is None:
     from . import klist
     kpath = klist.default(h.geometry,nk=nk) # generate default klist
-#    print("Bands in kpoint",k,"of",len(kpath),end="\r")
   def getek(k):
     """Compute this k-point"""
     out = "" # output string
     hk = hkgen(kpath[k]) # get hamiltonian
     if operator is None:
       es = diagf(hk)
       es = np.sort(es) # sort energies
@@ -149,15 +145,15 @@
       if write: f.write(ek) # write this kpoint
       if write: f.flush() # flush in file
   else: # parallel run
       esk = parallel.pcall(getek,range(len(kpath))) # compute all
       esk = "".join(esk) # concatenate all
       if write: f.write(esk)
   if write: f.close()
-  print("\nBANDS finished")
+#  print("\nBANDS finished")
   esk = esk.split("\n") # split
   del esk[-1] # remove last one
   esk = np.array([[float(i) for i in ek.split()] for ek in esk]).T
   return esk # return data
```

### Comparing `pyqula-0.0.8/src/pyqula/check.py` & `pyqula-0.0.9/src/pyqula/check.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/chi.py` & `pyqula-0.0.9/src/pyqula/chi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import numpy as np
 import scipy.linalg as lg
 from . import parallel
 from numba import jit
 
+
 try:
     from . import chif90
     use_fortran = True
 except:
     use_fortran = False
-    print("Error, chif90 not found")
+#    print("Error, chif90 not found")
+
+use_fortran = False
 
 
 def chargechi(h,i=0,j=0,es=np.linspace(-3.0,3.0,100),delta=0.01,temp=1e-7):
     """Compute charge response function"""
     if h.dimensionality!=0: raise
     hk = h.get_hk_gen() # get generator
     m = hk(0) # get Hamiltonian
     esh,ws = lg.eigh(m)
     ws = np.transpose(ws)
     if i<0: raise
     if j<0: raise
-    if use_fortran:
-      return es,chif90.elementchi(ws,esh,ws,esh,es,i+1,j+1,temp,delta)
-    else:
-      out = 0*es + 0j # initialize
-      return es,elementchi(ws,esh,ws,esh,es,i,j,temp,delta,out)
+#    if use_fortran:
+#      return es,chif90.elementchi(ws,esh,ws,esh,es,i+1,j+1,temp,delta)
+#    else:
+    out = 0*es + 0j # initialize
+    return es,elementchi(ws,esh,ws,esh,es,i,j,temp,delta,out)
 
 @jit(nopython=True)
 def elementchi(ws1,es1,ws2,es2,omegas,ii,jj,T,delta,out):
     """Compute the response function"""
     out  = out*0.0 # initialize
     n = len(ws1) # number of wavefunctions
     for i in range(n):
@@ -63,15 +66,15 @@
     if h.dimensionality!=0: raise
     hk = h.get_hk_gen() # get generator
     m = hk(0) # get Hamiltonian
     esh,ws = lg.eigh(m)
     ws = np.transpose(ws)
     out = [] # store
     if i<0: raise
-    f = lambda j: chif90.elementchi(ws,esh,ws,esh,es,i+1,j+1,temp,delta)
+    f = lambda j: elementchi(ws,esh,ws,esh,es,i+1,j+1,temp,delta)
     out = parallel.pcall(f,range(m.shape[0])) # parallel call
     return np.array(out)
 
 
 
 def chargechi_nowf(h,i=0,j=0,es=np.linspace(-3.0,3.0,100),delta=0.01,temp=1e-7):
     """Compute charge response function"""
@@ -111,7 +114,28 @@
           fo.write(str(freq[i])+"  ")
           fo.write(str(es[j])+"  ")
           fo.write(str(np.abs(fcs[j][i]))+"\n")
     fo.close()
 
 
 
+
+@jit(nopython=True)
+def chiAB_jit(ws1,es1,ws2,es2,omegas,A,B,T,delta,out):
+    """Compute the response function"""
+    raise # this is not double checked yet
+    out  = out*0.0 # initialize
+    n = len(ws1) # number of wavefunctions
+    for i in range(n):
+      oi = es1[i]<0.0 # first occupation
+      for j in range(n):
+          oj = es2[j]<0.0 # second occupation
+          fac = np.conjugate(ws1[i]).dot(A@ws2[j]) # add the factor
+          fac *= np.conjugate(ws1[i]).dot(B@ws2[j]) # add the factor
+          fac *= oi - oj # occupation factor
+          out = out + fac*(1./(es1[i]-es2[j] - omegas + 1j*delta))
+    return out
+
+
+
+
+
```

### Comparing `pyqula-0.0.8/src/pyqula/chitk/epsilon.py` & `pyqula-0.0.9/src/pyqula/chitk/epsilon.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/chitk/qpi.py` & `pyqula-0.0.9/src/pyqula/chitk/qpi.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/classicalspin.py` & `pyqula-0.0.9/src/pyqula/classicalspin.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/compilefortran.py` & `pyqula-0.0.9/src/pyqula/compilefortran.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/convolution.py` & `pyqula-0.0.9/src/pyqula/convolution.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,8 +15,13 @@
     for i in range(nx):
       for j in range(ny):
         for ii in range(nx):
           for jj in range(ny):
               out[ii,jj] = ds[(i+ii)%nx,(j+jj)%nx]*ds[i,j] + out[ii,jj]
     return out
 
+from .temperaturetk.convolution import temperature_convolution
+
+
+
+
```

### Comparing `pyqula-0.0.8/src/pyqula/correlator.py` & `pyqula-0.0.9/src/pyqula/correlator.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/crystalfield.py` & `pyqula-0.0.9/src/pyqula/crystalfield.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/current.py` & `pyqula-0.0.9/src/pyqula/current.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/density.py` & `pyqula-0.0.9/src/pyqula/density.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/densitymatrix.py` & `pyqula-0.0.9/src/pyqula/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/disorder.py` & `pyqula-0.0.9/src/pyqula/disorder.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/disorder_heterostructure.py` & `pyqula-0.0.9/src/pyqula/disorder_heterostructure.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/dos.py` & `pyqula-0.0.9/src/pyqula/dos.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,16 @@
   """Calculates the DOS of a surface, and writes in file"""
   if h.dimensionality!=1: raise # only for 1d
   fo = open(output_file,"w")
   fo.write("# energy, DOS surface, DOS bulk\n")
   for e in energies: # loop over energies
     print("Done",e)
     gb,gs = green.green_renormalization(h.intra,h.inter,energy=e,delta=delta)
-    gb = -gb.trace()[0,0].imag
-    gs = -gs.trace()[0,0].imag
+    gb = -np.trace(gb).imag
+    gs = -np.trace(gs).imag
     fo.write(str(e)+"     "+str(gs)+"    "+str(gb)+"\n")
   fo.close()
 
 
 
 
 def dos0d(h,energies=np.linspace(-4,4,500),delta=0.01):
@@ -494,15 +494,15 @@
         return (x,y)
     return dos(h,**kwargs)
 
 
 
 
 def bulkandsurface(h1,energies=np.linspace(-1.,1.,100),operator=None,
-                    delta=0.01,hs=None,nk=30):
+                    delta=0.01,hs=None,nk=30,write=True):
   """Compute the DOS of the bulk and the surface"""
   tr = timing.Testimator("KDOS") # generate object
   ik = 0
   h1 = h1.get_multicell() # multicell Hamiltonian
   kpath = [np.random.random(3) for i in range(nk)] # loop
   dosout = np.zeros((2,len(energies))) # output DOS
   for k in kpath:
@@ -510,23 +510,25 @@
     ik += 1
     outs = green.surface_multienergy(h1,k=k,energies=energies,delta=delta,hs=hs)
     ie = 0
     for (energy,out) in zip(energies,outs): # loop over energies
       # compute dos
       ig = 0
       for g in out: # loop
-        if operator is None: d = -g.trace()[0,0].imag # only the trace 
+        if operator is None: d = -np.trace(g).imag # only the trace 
         elif callable(operator): d = operator(g,k=k) # call the operator
-        else:  d = -(g*operator).trace()[0,0].imag # assume it is a matrix
+        else:  d = -np.trace(g*operator).imag # assume it is a matrix
         dosout[ig,ie] += d # store
         ig += 1 # increase site
       ie += 1 # increase energy
   # write in file
   dosout/=nk # normalize
-  np.savetxt("DOS_BULK_SURFACE.OUT",np.matrix([energies,dosout[0],dosout[1]]).T)
+  if write:
+    np.savetxt("DOS_BULK_SURFACE.OUT",np.array([energies,dosout[0],dosout[1]]).T)
+  return energies,dosout[0],dosout[1]
 
 
 
 
 def surface2bulk(h,n=50,nk=3000,delta=1e-3,e=0.0,**kwargs):
     """Compute the DOS from the surface to the bulk"""
     if h.dimensionality==2:
@@ -541,7 +543,30 @@
     else: raise
     return np.array([range(n),out]) # return array
 
 
 
 
 
+def surface_dos(h,energies=None,klist=None,delta=0.01,
+                         operator=None):
+    bout = [] # empty list, bulk
+    sout = [] # empty list, surface
+    if klist is None:
+        klist = [[i,0.,0.] for i in np.linspace(-.5,.5,50)]
+    if energies is None: energies = np.linspace(-.5,.5,50)
+    h = h.get_no_multicell()
+    def sdos(energy):
+        if h.dimensionality==1:
+            gs,sf = green.green_renormalization(h.intra,h.inter,
+                energy=energy,delta=delta) # surface green function
+            return -np.trace(sf).imag # return result
+        elif h.dimensionality==2:
+            out = 0.0
+            for k in klist: # loop over kpoints
+                gs,sf = green.green_kchain(h,k=k,energy=energy,delta=delta,
+                         only_bulk=False) # surface green function
+                out += -np.trace(sf).imag
+            return out/len(klist)
+        else: raise # not implemented
+    return energies,np.array([sdos(e) for e in energies])          
+
```

### Comparing `pyqula-0.0.8/src/pyqula/dyson.py` & `pyqula-0.0.9/src/pyqula/dyson.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/effective.py` & `pyqula-0.0.9/src/pyqula/effective.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/embedding.py` & `pyqula-0.0.9/src/pyqula/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/energeticstk/alloytk.py` & `pyqula-0.0.9/src/pyqula/energeticstk/alloytk.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/estimators.py` & `pyqula-0.0.9/src/pyqula/estimators.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/extract.py` & `pyqula-0.0.9/src/pyqula/extract.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/fermisurface.py` & `pyqula-0.0.9/src/pyqula/fermisurface.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/films.py` & `pyqula-0.0.9/src/pyqula/films.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/gap.py` & `pyqula-0.0.9/src/pyqula/gap.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/gauge.py` & `pyqula-0.0.9/src/pyqula/gauge.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/geometry.py` & `pyqula-0.0.9/src/pyqula/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,16 +172,17 @@
     return f # return function
   def reciprocal2natural(self,v):
       """
       Return a natural vector in real reciprocal coordinates
       """
       return self.get_k2K_generator()(v)
   def get_fractional(self,center=False):
-    """Fractional coordinates"""
-    get_fractional(self,center=center) # get fractional coordinates
+      """Fractional coordinates"""
+      self.update_reciprocal() # update reciprocal lattice vectors
+      get_fractional(self,center=center) # get fractional coordinates
   def rotate(self,angle):
     """Rotate the geometry"""
     return sculpt.rotate(self,angle*np.pi/180)
   def clean(self,iterative=False):
     return sculpt.remove_unibonded(self,iterative=iterative)
   def get_diameter(self):
     """Return the maximum distance between two atoms"""
@@ -196,15 +197,15 @@
   def shift(self,r0):
     """Shift all the positions by r0"""
     self.x[:] -= r0[0]
     self.y[:] -= r0[1]
     self.z[:] -= r0[2]
     self.xyz2r() # update
     if self.dimensionality>0:
-      self.get_fractional(center=True)
+      self.et_fractional(center=True)
       self.fractional2real()
   def write_function(self,fun,name="FUNCTION.OUT"):
     """Write a certain function"""
     f = open(name,"w")
     ir = 0
     for r in self.r: # loop over positions
       o = fun(r) # evaluate
@@ -272,27 +273,27 @@
       return sculpt.get_central(self,n=n) # get the index
   def update_reciprocal(self):
       """
       Update reciprocal lattice vectors
       """
       self.b1,self.b2,self.b3 = get_reciprocal(self.a1,self.a2,self.a3)
   def get_k2K_generator(self,toreal=False):
-    """
-    Function to turn a reciprocal lattice vector to natural units
-    """
-    R = self.get_k2K() # get matrix
-    if toreal: R = R.H # transform to real coordinates
-    def fun(k0):
-      if len(k0)==3: k = k0 # do nothing
-      elif len(k0)==2: k = np.array([k0[0],k0[1],0.]) # convert to three comp
-      r = np.matrix(k).T # real space vectors
-      out = np.array((R*r).T)[0] # change of basis
-      if len(k0)==2: return np.array([out[0],out[1]]) # return two
-      return out
-    return fun
+      """
+      Function to turn a reciprocal lattice vector to natural units
+      """
+      R = self.get_k2K() # get matrix
+      if toreal: R = R.H # transform to real coordinates
+      def fun(k0):
+        if len(k0)==3: k = k0 # do nothing
+        elif len(k0)==2: k = np.array([k0[0],k0[1],0.]) # convert to three comp
+        r = np.matrix(k).T # real space vectors
+        out = np.array((R*r).T)[0] # change of basis
+        if len(k0)==2: return np.array([out[0],out[1]]) # return two
+        return out
+      return fun
   def fractional2real(self):
     """
     Convert fractional coordinates to real coordinates
     """
     fractional2real(self)
   def real2fractional(self):
     self.get_fractional() # same function
@@ -692,15 +693,15 @@
   g.y = np.array([0.0])
   g.z = np.array([0.0])
   g.a1 = np.array([np.sqrt(3.)/2.,1./2,0.]) # first lattice vector
   g.a2 = np.array([-np.sqrt(3.)/2.,1./2,0.]) # second lattice vector
   g.dimensionality = 2 # two dimensional system
   g.xyz2r() # create r coordinates
   g.has_sublattice = False # has sublattice index
-  g.update_reciprocal() # update reciprocal lattice vectors
+  g.get_fractional() # update reciprocal lattice vectors
   if n>1: return supercelltk.target_angle_volume(g,angle=1./3.,volume=int(n),
           same_length=True) 
   g = sculpt.rotate_a2b(g,g.a1,np.array([1.,0.,0.]))
   return g
 
 
 
@@ -943,24 +944,14 @@
   """
   Geometry for a honeycomb lattice, taking a unit cell
   with C6 rotational symmetry
   """
   g = honeycomb_lattice() # create geometry
   return supercelltk.target_angle_volume(g,angle=1./3.,volume=3,
           same_length=True)
-#  m = [[2,1,0],[1,2,0],[0,0,1]]
-#  g = non_orthogonal_supercell(g,m)
-#  g.r[0] = g.r[0] + g.a2
-#  g.r[1] = g.r[1] + g.a2
-#  g.r[4] = g.r[4] - g.a2 + g.a1
-#  # if it looks stupid but it works, it is not stupid
-#  g.r2xyz()
-#  g.update_reciprocal() # update reciprocal lattice vectors
-#  return g
- 
 
 
 
 
 
 
 
@@ -983,29 +974,28 @@
 def supercell2d(g,n1=1,n2=1,use_fortran=use_fortran):
   """ Creates a supercell for a 2d system"""
   go = g.copy() # copy geometry
   use_fortran = False
   if use_fortran:
     from . import supercellf90
     go.r = supercellf90.supercell2d(g.r,g.a1,g.a2,n1,n2)
-    go.r2xyz() # update xyz
 #    print("Using FORTRAN")
   else:
-    nc = len(g.x) # number of atoms in a cell
+    nc = len(g.r) # number of atoms in a cell
     n = nc*n1*n2 # total number of positions
     a1 = g.a1 # first vector
     a2 = g.a2 # second vector
     rs = []
     for i in range(n1): 
       for j in range(n2): 
         for k in range(nc): 
           ri = i*a1 + j*a2 + g.r[k] 
           rs.append(ri) # store
     go.r = np.array(rs) # store
-    go.r2xyz()
+  go.r2xyz()
   go.a1 = go.a1*n1
   go.a2 = go.a2*n2
   # shift to zero
   go.center() 
   if g.has_sublattice: # supercell sublattice
     go.sublattice = np.concatenate([g.sublattice for i in range(n1*n2)])
   if g.atoms_have_names: # supercell sublattice
@@ -1215,15 +1205,15 @@
 
 
 
 
 def get_k2K(g):
   """Return a matrix that converts vectors
   in the reciprocal space into natural units, useful for drawing
-  2D quantities"""
+  2D/3D quantities"""
   if g.dimensionality == 2:
     (ux,uy,uz) = (g.a1,g.a2,np.array([0.,0.,1]))
   elif g.dimensionality == 3:
     (ux,uy,uz) = (g.a1,g.a2,g.a3)
   else: raise
   ux = ux/np.sqrt(ux.dot(ux))
   uy = uy/np.sqrt(uy.dot(uy))
@@ -1232,21 +1222,20 @@
   r2a = np.matrix([ux,uy,uz]).T.I # from real space to lattice vectors
   R = a2kn@r2a@a2kn.T # rotation matrix
   return R
 
 
 
 def get_reciprocal(a1,a2,a3):
-  """Return a matrix that converts vectors
-  in the reciprocal space into natural units, useful for drawing
-  2D quantities"""
+  """Return the reciprocal lattice vectors
+  By definition, ai*bj = delta_ij"""
   (ux,uy,uz) = (a1,a2,a3)
-  ux = ux/np.sqrt(ux.dot(ux))
-  uy = uy/np.sqrt(uy.dot(uy))
-  uz = uz/np.sqrt(uz.dot(uz))
+#  ux = ux/np.sqrt(ux.dot(ux))
+#  uy = uy/np.sqrt(uy.dot(uy))
+#  uz = uz/np.sqrt(uz.dot(uz))
   a2kn = np.matrix([ux,uy,uz]) # matrix for the change of basis
   r2a = np.matrix([ux,uy,uz]).T.I # from real space to lattice vectors
   b1,b2,b3 = r2a[0,:],r2a[1,:],r2a[2,:]
   b1 = np.array(b1).reshape(3)
   b2 = np.array(b2).reshape(3)
   b3 = np.array(b3).reshape(3)
   return b1,b2,b3
```

### Comparing `pyqula-0.0.8/src/pyqula/geometrytk/readgeometry.py` & `pyqula-0.0.9/src/pyqula/geometrytk/readgeometry.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/green.py` & `pyqula-0.0.9/src/pyqula/green.py`

 * *Files 6% similar despite different names*

```diff
@@ -326,25 +326,32 @@
 
 
 
 
 def green_renormalization(intra,inter,energy=0.0,nite=None,
                             error=0.000001,info=False,delta=0.001,
                             use_fortran = use_fortran):
-  """ Calculates bulk and surface Green function by a renormalization
-  algorithm, as described in I. Phys. F: Met. Phys. 15 (1985) 851-858 """
-  error = delta/100
-  if use_fortran: # use the fortran implementation
-    (ge,gb) = greenf90.renormalization(intra,inter,energy,error,delta)
-    return np.matrix(gb),np.matrix(ge)
-  else:
+    """ Calculates bulk and surface Green function by a renormalization
+    algorithm, as described in I. Phys. F: Met. Phys. 15 (1985) 851-858 """
+    intra = algebra.todense(intra)
+    inter = algebra.todense(inter)
+    error = delta*1e-6 # overwrite error
+#  if use_fortran: # use the fortran implementation
+#    (ge,gb) = greenf90.renormalization(intra,inter,energy,error,delta)
+#    return np.matrix(gb),np.matrix(ge)
+#  else:
+#      g0,g1 = intra*0j,intra*0j
+#      e = np.identity(intra.shape[0],dtype=np.complex) * (energy + 1j*delta)
+#      g0,g1 = green_renormalization_jit(g0,g1,intra,inter,e,nite,
+#                            error,delta)
+#      return np.matrix(g0),np.matrix(g1)
     e = np.matrix(np.identity(intra.shape[0])) * (energy + 1j*delta)
     ite = 0
     alpha = inter.copy()
-    beta = inter.H.copy()
+    beta = algebra.dagger(inter).copy()
     epsilon = intra.copy()
     epsilon_s = intra.copy()
     while True: # implementation of Eq 11
       einv = algebra.inv(e - epsilon) # inverse
       epsilon_s = epsilon_s + alpha @ einv @ beta
       epsilon = epsilon + alpha * einv @ beta + beta @ einv @ alpha
       alpha = alpha @ einv @ alpha  # new alpha
@@ -359,14 +366,48 @@
       print("Converged in ",ite,"iterations")
     g_surf = algebra.inv(e - epsilon_s) # surface green function
     g_bulk = algebra.inv(e - epsilon)  # bulk green function 
     return g_bulk,g_surf
 
 
 
+
+from numba import jit
+
+#@jit(nopython=True)
+### this seems to not work with numba ###
+def green_renormalization_jit(g0,g1,intra,inter,e,nite,error,delta):
+    ite = 0
+    alpha = inter.copy()
+    beta = np.conjugate(inter).T.copy()
+    epsilon = intra.copy()
+    epsilon_s = intra.copy()
+    while True: # implementation of Eq 11
+      einv = np.linalg.inv(e - epsilon) # inverse
+      epsilon_s = epsilon_s + alpha @ einv @ beta
+      epsilon = epsilon + alpha * einv @ beta + beta @ einv @ alpha
+      alpha = alpha @ einv @ alpha  # new alpha
+      beta = beta @ einv @ beta  # new beta
+      ite += 1
+      # stop conditions
+      if np.max(np.abs(alpha))<error and np.max(np.abs(beta))<error: break
+    g_surf = np.linalg.inv(e - epsilon_s) # surface green function
+    g_bulk = np.linalg.inv(e - epsilon)  # bulk green function 
+    g0,g1 = g_bulk*1,g_surf*1
+    return g0,g1
+
+
+
+
+
+
+
+
+
+
 def bloch_selfenergy(h,nk=100,energy = 0.0, delta = 0.01,mode="full",
                          error=0.00001):
   """ Calculates the selfenergy of a cell defect,
       input is a hamiltonian class"""
   if mode=="adaptative": mode = "adaptive"
   def gr(ons,hop):
     """ Calculates G by renormalization"""
```

### Comparing `pyqula-0.0.8/src/pyqula/groundstate.py` & `pyqula-0.0.9/src/pyqula/groundstate.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/gsenergy.py` & `pyqula-0.0.9/src/pyqula/gsenergy.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/hall.py` & `pyqula-0.0.9/src/pyqula/hall.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/hamiltonians.py` & `pyqula-0.0.9/src/pyqula/hamiltonians.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,16 +213,16 @@
         """ Adds swave superconducting pairing"""
         superconductivity.add_swave_to_hamiltonian(self,*args,**kwargs)
     def setup_nambu_spinor(self): self.add_swave(0.0)
     def get_anomalous_hamiltonian(self):
         """Return a Hamiltonian only with the anomalous part"""
         return superconductivity.get_anomalous_hamiltonian(self)
     def add_pairing(self,**kwargs):
-      """ Add a general pairing matrix, uu,dd,ud"""
-      superconductivity.add_pairing_to_hamiltonian(self,**kwargs)
+        """ Add a general pairing matrix, uu,dd,ud"""
+        superconductivity.add_pairing_to_hamiltonian(self,**kwargs)
     def same_hamiltonian(self,*args,**kwargs):
         """Check if two hamiltonians are the same"""
         return hamiltonianmode.same_hamiltonian(self,*args,**kwargs)
     def supercell(self,nsuper):
       """ Creates a supercell of a one dimensional system"""
       if nsuper==1: return self
       if self.dimensionality==0: return self
@@ -265,28 +265,17 @@
         add_zeeman(self,zeeman=zeeman)
     def add_magnetism(self,m):
         """Adds magnetism, new version of zeeman"""
         self.turn_spinful()
         from .magnetism import add_magnetism
         add_magnetism(self,m)
     def add_exchange(self,m): self.add_magnetism(m)
-    def turn_spinful(self,enforce_tr=False):
-      """Turn the hamiltonian spinful""" 
-      if self.has_spin: return # already spinful
-      if self.is_sparse: # sparse Hamiltonian
-        self.turn_dense() # dense Hamiltonian
-        self.turn_spinful(enforce_tr=enforce_tr) # spinful
-        self.turn_sparse()
-      else: # dense Hamiltonian
-        from .increase_hilbert import spinful
-        def fun(m):
-            if enforce_tr: return spinful(m,np.conjugate(m))
-            else: return spinful(m)
-        self.modify_hamiltonian_matrices(fun) # modify the matrices
-        self.has_spin = True # set spinful
+    def turn_spinful(self,**kwargs):
+        from .htk.mode import turn_spinful
+        turn_spinful(self,**kwargs)
     def remove_spin(self):
       """Removes spin degree of freedom"""
       if self.check_mode("spinless"): return # do nothing
       elif self.check_mode("spinful"):
           def f(m): return des_spin(m,component=0)
           self.modify_hamiltonian_matrices(f) # modify the matrices
           self.has_spin = False # set to spinless
@@ -580,42 +569,17 @@
 
 
 
 
 
 def get_first_neighbors(r1,r2):
     """Gets the fist neighbors, input are arrays"""
-#  if optimal:
     from . import neighbor
     pairs = neighbor.find_first_neighbor(r1,r2)
     return pairs
-#  else:
-#    from numpy import array
-#    n=len(r1)
-#    pairs = [] # pairs of neighbors
-#    for i in range(n):
-#      ri=r1[i]
-#      for j in range(n):
-#        rj=r2[j]
-#        dr = ri - rj ; dr = dr.dot(dr)
-#        if .9<dr<1.1 : # check if distance is 1
-#          pairs.append([i,j])  # add to the list
-#    return pairs # return pairs of first neighbors
-
-
-
-
-
-
-
-
-
-
-
-
 
 
 
 
 
 def create_fn_hopping(r1,r2):
   n=len(r1)
@@ -721,37 +685,15 @@
   print("Intracell matrix")
   print(intra)
   print("Intercell matrix")
   print(inter)
   return
 
 
-
-def add_sublattice_imbalance(h,mass):
-  """ Adds to the intracell matrix a sublattice imbalance """
-  if h.geometry.has_sublattice:  # if has sublattice
-    def ab(i): 
-      return h.geometry.sublattice[i]
-  else: 
-    print("WARNING, no sublattice present")
-    return 0. # if does not have sublattice
-  natoms = len(h.geometry.r) # assume spinpolarized calculation 
-  rows = range(natoms)
-  if callable(mass):  # if mass is a function
-    r = h.geometry.r
-    data = [mass(r[i])*ab(i) for i in range(natoms)]
-  else: data = [mass*ab(i) for i in range(natoms)]
-  massterm = csc_matrix((data,(rows,rows)),shape=(natoms,natoms)) # matrix
-  h.intra = h.intra + h.spinless2full(massterm)
-
-
-
-
-
-
+from .htk.cdw import add_sublattice_imbalance
 
 
 def build_eh_nonh(hin,c1=None,c2=None):
   """Creates a electron hole matrix, from an input matrix, coupling couples
      electrons and holes
       - hin is the hamiltonian for electrons, which has the usual common form
       - coupling is the matrix which tells the coupling between electron
@@ -947,34 +889,15 @@
   hop = h.tx + tkxy + tkxmy  # hopping of k-dependent chain
   return (ons,hop)
 
 
 
 # import the function written in the library
 from .kanemele import generalized_kane_mele
-
-
-def modify_hamiltonian_matrices(self,f):
-  """Apply a certain function to all the matrices"""
-  self.intra = f(self.intra)
-  if self.is_multicell: # for multicell hamiltonians
-    for i in range(len(self.hopping)): # loop over hoppings
-      self.hopping[i].m = f(self.hopping[i].m) # put in nambu form
-  else: # conventional way
-    if self.dimensionality==0: pass # one dimensional systems
-    elif self.dimensionality==1: # one dimensional systems
-      self.inter = f(self.inter)
-    elif self.dimensionality==2: # two dimensional systems
-      self.tx = f(self.tx)
-      self.ty = f(self.ty)
-      self.txy = f(self.txy)
-      self.txmy = f(self.txmy)
-    else: raise
-
-
+from .htk.modify import modify_hamiltonian_matrices
 
 from . import inout
 
 def load(input_file="hamiltonian.pkl"):  return inout.load(input_file)
 
 
 def print_hopping(h):
@@ -991,10 +914,11 @@
     for t in h.hopping:
         print("Hopping",t.dir)
         pprint(t.m)
 
 
 
 
-
+from .htk.dummy import generate_dummy_hamiltonian
+generate_hamiltonian_from_dict = generate_dummy_hamiltonian
```

### Comparing `pyqula-0.0.8/src/pyqula/heterostructures.py` & `pyqula-0.0.9/src/pyqula/heterostructures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from __future__ import print_function
 import numpy as np
 import pylab as py
 from copy import deepcopy as dc
+import scipy.linalg as lg
 from scipy.sparse import bmat,coo_matrix,csc_matrix
 from . import green
+from .algebra import dagger
 
+dag = dagger
 
 
 
-
-
-class heterostructure():
+class Heterostructure():
   """Class for a heterostructure"""
   def copy(self):
     """Copy the heterostructure"""
     from copy import deepcopy
     return deepcopy(self)
   def __init__(self,h=None):  # initialization using a hamiltonian
     self.file_right_green = "green_right.dat"  # in/out file for right green
     self.file_left_green = "green_left.dat"   # in/out file for left green
     self.file_heff = "heff.dat"   # out for the effective hamiltonian
     self.scale_rc = 1.0 # scale coupling to the right lead
     self.scale_lc = 1.0 # scale coupling to the left lead
     self.is_sparse = False
     self.dimensionality = 1 # default is one dimensional
+    self.transparency = 1.0 # reference transparency (for kappa)
     self.delta = 0.0001
+    self.extra_delta_central = 0. # additional delta in the central region
+    self.extra_delta_right = 0. # additional delta in the right region
+    self.extra_delta_left = 0. # additional delta in the left region
     self.interpolated_selfenergy = False
     self.block_diagonal = False
     if h is not None:
       self.heff = None  # effective hamiltonian
       self.right_intra = h.intra  # intraterm in the right lead
       self.right_inter = h.inter  # interterm in the right lead (to the right)
       self.right_green = None  # right green function
@@ -47,14 +52,17 @@
   def plot_central_dos(self,energies=[0.0],num_rep=100,
                       mixing=0.7,eps=0.0001,green_guess=None,max_error=0.0001):
     """ Plots the density of states by using a 
     green function approach"""
     return plot_central_dos(self,energies=energies,num_rep=num_rep,
                       mixing=mixing,eps=eps,green_guess=green_guess,
                       max_error=max_error)
+  def surface_dos(self,**kwargs):
+      from .transporttk import sdos
+      return sdos.surface_dos(self,**kwargs)
   def landauer(self,energy=[0.],delta=0.0001,do_leads=True,left_channel=None,
                 right_channel=None):
     """ Return the Landauer transmission"""
     if self.has_eh: raise # invalid if there is electorn-hole
     return landauer(self,energy=energy,delta=delta,do_leads=do_leads,
                     left_channel=left_channel,right_channel=right_channel)
   def write_green(self):
@@ -95,63 +103,39 @@
     self.left_green = g # save green function
     self.energy_green = energy # energy of the Green function
   def copy_surface_green(self,ht):
     """Copy the surface Green fucntions"""
     self.energy_green = ht.energy_green
     self.left_green = ht.left_green
     self.right_green = ht.right_green
-  def get_selfenergy(self,energy,lead=0,delta=None,pristine=False):
-   """Return self energy of iesim lead"""
-   if delta is None:  delta = self.delta
-# if the interpolation function has been created
-   if self.interpolated_selfenergy: 
-     if lead==0: return np.matrix(self.selfgen[0](energy)) # return selfenergy
-     if lead==1: return np.matrix(self.selfgen[1](energy)) # return selfenergy
-# run the calculation
-   else:
-     from .green import green_renormalization
-     if lead==0:
-       intra = self.left_intra
-       inter = self.left_inter
-       if pristine: cou = self.left_inter
-       else: cou = self.left_coupling*self.scale_lc
-     if lead==1:
-       intra = self.right_intra
-       inter = self.right_inter
-       if pristine: cou = self.right_inter
-       else: cou = self.right_coupling*self.scale_rc
-     ggg,gr = green_renormalization(intra,inter,energy=energy,delta=delta)
-     selfr = cou*gr*cou.H # selfenergy
-     return selfr # return selfenergy
+  def get_selfenergy(self,energy,**kwargs):
+     """Return selfenergy of iesim lead"""
+     from .transporttk.selfenergy import get_selfenergy
+     return get_selfenergy(self,energy,**kwargs)
   def setup_selfenergy_interpolation(self,es=np.linspace(-4.0,4.0,100),
            delta=0.0001,pristine=False):
     """Create the functions that interpolate the selfenergy"""
-    from interpolation import intermatrix
+    from .interpolation import intermatrix
     self.interpolated_selfenergy = False # set as False
     fsl = lambda e: self.get_selfenergy(e,delta=delta,lead=0,pristine=pristine)
     fsr = lambda e: self.get_selfenergy(e,delta=delta,lead=1,pristine=pristine)
     fun_sr = intermatrix(fsr,xs=es) # get the function
     fun_sl = intermatrix(fsl,xs=es) # get the function
     self.selfgen = [fun_sl,fun_sr] # store functions
     self.interpolated_selfenergy = True # set as true
-  def didv(self,energy=0.0,delta=None,error=1e-4,nk=10,kwant=False,
-          opl=None,opr=None):
-    if delta is None: delta = self.delta # set the own delta
-    if self.dimensionality==1: # one dimensional
-      return didv(self,energy=energy,delta=delta,kwant=kwant,
-              opl=opl,opr=opr) # return value
-    elif self.dimensionality==2: # two dimensional
-      # function to integrate
-      print("Computing",energy)
-      f = lambda k: self.generate(k).didv(energy=energy,delta=delta)
-      return np.mean([f(x) for x in np.linspace(0.,1.,nk,endpoint=False)])
-    else: raise
+  def didv(self,**kwargs):
+      from .transporttk.didv import generic_didv
+      return generic_didv(self,**kwargs)
   def block2full(self,sparse=False):
-    """Put in full form"""
-    return block2full(self,sparse=sparse)
+      """Put in full form"""
+      return block2full(self,sparse=sparse)
+  def get_kappa(self,energy=[0.],**kwargs):
+      from .transporttk.kappa import get_kappa_ratio
+      return get_kappa_ratio(self,energies=[energy],**kwargs)[0]
+  
 
 
 
 
 def create_leads_and_central(h_right,h_left,h_central,num_central=1,
       interpolation="None",block_diagonal=True):
   """ Creates an heterojunction by giving the hamiltonian
@@ -264,15 +248,15 @@
   ht.right_coupling = tcr
   ht.left_coupling = tcl
   ht.central_intra = hc
   # and modify the geometry
   ht.central_geometry.supercell(num_central) 
   return ht
 
-
+heterostructure = Heterostructure
 
 def central_dos(hetero,energies=[0.0],num_rep=100,project=None):
    """ Calculates the density of states 
        of a heterostructure by a  
     green function approach, input is a heterostructure class"""
    if hetero.block_diagonal: ht = ht.block2full()
    dos = [] # list with the density of states
@@ -340,30 +324,30 @@
      dimhc = len(hetero.central_intra)*intra.shape[0] 
    iden = np.matrix(np.identity(len(intra),dtype=complex)) # create idntity
    selfl = hetero.get_selfenergy(energy,lead=0,delta=delta,pristine=False) # left Sigma
    selfr = hetero.get_selfenergy(energy,lead=1,delta=delta,pristine=False) # right Sigma
    #################################
    # calculate Gammas 
    #################################
-   gammar = 1j*(selfr-selfr.H)
-   gammal = 1j*(selfl-selfl.H)
+   gammar = 1j*(selfr-dagger(selfr))
+   gammal = 1j*(selfl-dagger(selfl))
 
    #################################
    # dyson equation for the center     
    #################################
    # central green function
    intra = hetero.central_intra
    # full matrix
    if not hetero.block_diagonal:
      heff = intra + selfl + selfr
      hetero.heff = heff
      gc = (energy+1j*delta)*iden - heff
      gc = gc.I # calculate inverse
      if has_eh: raise # if it has electron-hole, trace over electrons
-     G = (gammar*gc*gammal*gc.H).trace()[0,0].real
+     G = np.trace(gammar@gc@gammal@dagger(gc)).real
      return G
    # reduced matrix
    if hetero.block_diagonal: 
      from copy import deepcopy
      heff = deepcopy(intra)
      heff[0][0] = intra[0][0] + selfl
      heff[-1][-1] = intra[-1][-1] + selfr
@@ -376,15 +360,15 @@
          if heff[i][j] is not None:
            heff[i][j] = -heff[i][j]
      # calculate green function
      from .green import gauss_inverse  # routine to invert the matrix
      # calculate only some elements of the central green function
      gcn1 = gauss_inverse(heff,len(heff)-1,0) # calculate element 1,n 
      # and apply Landauer formula
-     G = (gammar*gcn1*gammal*gcn1.H).trace()[0,0].real
+     G = np.trace(gammar@gcn1@gammal@dagger(gcn1)).real
    return G # return transmission
 
 
 
 
 
 def block2full(ht,sparse=False):
@@ -416,248 +400,253 @@
     ho.central_intra = bmat(central).todense() # as dense matrix
   return ho
 
 
 
 
 
-
-def plot_landauer(ht,energy=[0.0],delta=0.001,has_eh=False):
-   """ Plots the density of states and Landauer transmission
-    by using a 
-    green function approach"""
-   # get the transmission
-   trans = landauer(ht,energy=energy,delta=delta,has_eh=has_eh)
-   # plot the figure
-   fig = py.figure() # create figure
-   fig.subplots_adjust(0.2,0.2)
-   fig.set_facecolor("white") # face in white
-   strans = fig.add_subplot(111) # create subplot for the transmission
-
-   # transport graph
-   strans.set_xlabel("Energy",size=20)
-   strans.set_ylabel("Transmission",size=20)
-   strans.plot(energy,trans,color="green") # create the plot
-   strans.fill_between(energy,0,trans,color="green")
-   strans.set_ylim([0.0,max(trans)+0.5])
-   strans.set_xlim([min(energy),max(energy)])
-   strans.tick_params(labelsize=20)
-   return fig
-
-
-
-
-def plot_local_central_dos(hetero,energies=0.0,gf=None):
-   """ Plots the local density of states in the central part"""
-   from .green import dyson
-   from .green import gf_convergence
-   from .hamiltonians import is_number
-   if gf==None: gf = gf_convergence("lead")
-   if not hetero.block_diagonal:
-     intra = hetero.central_intra # central intraterm   
-     dimhc = len(intra) # dimension of the central part
-   if hetero.block_diagonal:
-     intra = hetero.central_intra[0][0] # when it is diagonal
-# dimension of the central part
-     dimhc = len(hetero.central_intra)*len(intra)  
-   iden = np.matrix(np.identity(len(intra),dtype=complex)) # create idntity
-   ldos = np.array([0.0 for i in range(dimhc)]) # initialice ldos
-   # initialize ldos
-   for energy in energies: # loop over energies
-     # right green function
-     gr = None
-     gl = None
-     # perform dyson calculation
-
-     intra = hetero.right_intra
-     inter = hetero.right_inter
-     gr = dyson(intra,inter,energy=energy,gf=gf)
-     hetero.right_green = gr # save green function
-     # left green function
-     intra = hetero.left_intra
-     inter = hetero.left_inter
-     gl = dyson(intra,inter,energy=energy,gf=gf)
-     hetero.left_green = gl # save green function
-     # save green functions
-#     hetero.write_green()
-     # left selfenergy
-     inter = hetero.left_coupling
-     selfl = inter*gl*inter.H # left selfenergy
-     # right selfenergy
-     inter = hetero.right_coupling
-     selfr = inter*gr*inter.H # right selfenergy
-     # central green function
-     intra = hetero.central_intra
-# dyson equation for the center     
-     # full matrix
-     if not hetero.block_diagonal:
-       heff = intra + selfl + selfr
-       hetero.heff = heff
-       gc = (energy+1j*eps)*iden - heff
-       gc = gc.I # calculate inverse
-       # get the local density of states
-       ldos += np.array([-gc[i,i].imag for i in range(len(gc))])
-#       if save_heff:
-#         hetero.write_heff() 
-     # reduced matrix
-     if hetero.block_diagonal: 
-       from copy import deepcopy
-       heff = deepcopy(intra)
-       heff[0][0] = intra[0][0] + selfl
-       heff[-1][-1] = intra[-1][-1] + selfr
-       dd = (energy+1j*gf.eps)*iden
-       for i in range(len(intra)):  # add the diagonal energy part
-         heff[i][i] = heff[i][i] - dd  # this has the wrong sign!!
-      # now change the sign
-       for i in range(len(intra)):  
-         for j in range(len(intra)):  
-           try:
-             heff[i][j] = -heff[i][j]
-           except:
-             heff[i][j] = heff[i][j]
-      # save the green function
-       hetero.heff = heff
-#       if save_heff:
-#         from scipy.sparse import bmat
-#         hetero.heff = bmat(heff)
-#         hetero.write_heff() 
-      # calculate the inverse
-       from .green import gauss_inverse  # routine to invert the matrix
-       # list with the diagonal matrices
-       ldos_e = ldos*0.0 # initialice ldos at this energy
-       ii = 0 # counter for the element
-       for i in range(len(heff)): # loop over blocks
-         gci = gauss_inverse(heff,i,i) # calculate each block element      
-         for j in range(len(heff[0][0])): # loop over each block
-           ldos_e[ii] = -gci[j,j].imag 
-           ii += 1 # increase counter
-       if not ii==dimhc:
-         print("Wrong dimensions",ii,dimhc)
-         raise
-       ldos += ldos_e # add to the total ldos
-# save the effective hamiltonian
-
-   if hetero.has_spin: # resum ldos if there is spin degree of freedom
-     ldos = [ldos[2*i]+ldos[2*i+1] for i in range(len(ldos)/2)]
-   if hetero.has_eh: # resum ldos if there is eh 
-     ldos = [ldos[2*i]+ldos[2*i+1] for i in range(len(ldos)/2)]
-  #   ne = len(ldos)/2
-  #   ldos = [ldos[i]+ldos[ne+i] for i in range(ne)]
-
-
-   ldos = np.array(ldos) # transform into an array
-
-   if min(ldos)<0.0:
-     print("Negative density of states")
-     raise
-
-   g = hetero.central_geometry # geometry of the central part
-   fldos = open("LDOS.OUT","w") # open file for ldos
-   fldos.write("# X   Y    LDOS\n")
-   for (ix,iy,il) in zip(g.x,g.y,ldos):
-     fldos.write(str(ix)+"  "+str(iy)+"  "+str(il)+"\n")
-   fldos.close()
-   # scale the ldos
-   # save the LDOS in a file
-   if True:
-#   if True>0.001:
-#     ldos = np.sqrt(ldos)
-#     ldos = np.arctan(7.*ldos/max(ldos))
-     print("Sum of the LDOS =",sum(ldos))
-     ldos = ldos*300/max(ldos)
-   else:
-     ldos = ldos*0.0
-
-
-
-
-
-   # now create the figure
-   fig = py.figure() # create figure
-   fig.subplots_adjust(0.2,0.2)
-   fig.set_facecolor("white") # face in white
-   sldos = fig.add_subplot(111) # create subplot for the DOS
-
-   # plot the lattice
-   if not len(g.x)==len(ldos):
-     raise 
-   sldos.scatter(g.x,g.y,color="red",s=ldos) # plot the lattice
-   sldos.scatter(g.x,g.y,color="black",s=4) # plot the lattice
-   sldos.set_xlabel("X")
-   sldos.set_xlabel("Y")
-   sldos.axis("equal") # same scale in axes
-
-
-
-   return fig
-
+#
+#def plot_landauer(ht,energy=[0.0],delta=0.001,has_eh=False):
+#   """ Plots the density of states and Landauer transmission
+#    by using a 
+#    green function approach"""
+#   # get the transmission
+#   trans = landauer(ht,energy=energy,delta=delta,has_eh=has_eh)
+#   # plot the figure
+#   fig = py.figure() # create figure
+#   fig.subplots_adjust(0.2,0.2)
+#   fig.set_facecolor("white") # face in white
+#   strans = fig.add_subplot(111) # create subplot for the transmission
+#
+#   # transport graph
+#   strans.set_xlabel("Energy",size=20)
+#   strans.set_ylabel("Transmission",size=20)
+#   strans.plot(energy,trans,color="green") # create the plot
+#   strans.fill_between(energy,0,trans,color="green")
+#   strans.set_ylim([0.0,max(trans)+0.5])
+#   strans.set_xlim([min(energy),max(energy)])
+#   strans.tick_params(labelsize=20)
+#   return fig
+#
+#
+
+#
+#def plot_local_central_dos(hetero,energies=0.0,gf=None):
+#   """ Plots the local density of states in the central part"""
+#   from .green import dyson
+#   from .green import gf_convergence
+#   from .hamiltonians import is_number
+#   if gf==None: gf = gf_convergence("lead")
+#   if not hetero.block_diagonal:
+#     intra = hetero.central_intra # central intraterm   
+#     dimhc = len(intra) # dimension of the central part
+#   if hetero.block_diagonal:
+#     intra = hetero.central_intra[0][0] # when it is diagonal
+## dimension of the central part
+#     dimhc = len(hetero.central_intra)*len(intra)  
+#   iden = np.matrix(np.identity(len(intra),dtype=complex)) # create idntity
+#   ldos = np.array([0.0 for i in range(dimhc)]) # initialice ldos
+#   # initialize ldos
+#   for energy in energies: # loop over energies
+#     # right green function
+#     gr = None
+#     gl = None
+#     # perform dyson calculation
+#
+#     intra = hetero.right_intra
+#     inter = hetero.right_inter
+#     gr = dyson(intra,inter,energy=energy,gf=gf)
+#     hetero.right_green = gr # save green function
+#     # left green function
+#     intra = hetero.left_intra
+#     inter = hetero.left_inter
+#     gl = dyson(intra,inter,energy=energy,gf=gf)
+#     hetero.left_green = gl # save green function
+#     # save green functions
+##     hetero.write_green()
+#     # left selfenergy
+#     inter = hetero.left_coupling
+#     selfl = inter*gl*inter.H # left selfenergy
+#     # right selfenergy
+#     inter = hetero.right_coupling
+#     selfr = inter*gr*inter.H # right selfenergy
+#     # central green function
+#     intra = hetero.central_intra
+## dyson equation for the center     
+#     # full matrix
+#     if not hetero.block_diagonal:
+#       heff = intra + selfl + selfr
+#       hetero.heff = heff
+#       gc = (energy+1j*eps)*iden - heff
+#       gc = gc.I # calculate inverse
+#       # get the local density of states
+#       ldos += np.array([-gc[i,i].imag for i in range(len(gc))])
+##       if save_heff:
+##         hetero.write_heff() 
+#     # reduced matrix
+#     if hetero.block_diagonal: 
+#       from copy import deepcopy
+#       heff = deepcopy(intra)
+#       heff[0][0] = intra[0][0] + selfl
+#       heff[-1][-1] = intra[-1][-1] + selfr
+#       dd = (energy+1j*gf.eps)*iden
+#       for i in range(len(intra)):  # add the diagonal energy part
+#         heff[i][i] = heff[i][i] - dd  # this has the wrong sign!!
+#      # now change the sign
+#       for i in range(len(intra)):  
+#         for j in range(len(intra)):  
+#           try:
+#             heff[i][j] = -heff[i][j]
+#           except:
+#             heff[i][j] = heff[i][j]
+#      # save the green function
+#       hetero.heff = heff
+##       if save_heff:
+##         from scipy.sparse import bmat
+##         hetero.heff = bmat(heff)
+##         hetero.write_heff() 
+#      # calculate the inverse
+#       from .green import gauss_inverse  # routine to invert the matrix
+#       # list with the diagonal matrices
+#       ldos_e = ldos*0.0 # initialice ldos at this energy
+#       ii = 0 # counter for the element
+#       for i in range(len(heff)): # loop over blocks
+#         gci = gauss_inverse(heff,i,i) # calculate each block element      
+#         for j in range(len(heff[0][0])): # loop over each block
+#           ldos_e[ii] = -gci[j,j].imag 
+#           ii += 1 # increase counter
+#       if not ii==dimhc:
+#         print("Wrong dimensions",ii,dimhc)
+#         raise
+#       ldos += ldos_e # add to the total ldos
+## save the effective hamiltonian
+#
+#   if hetero.has_spin: # resum ldos if there is spin degree of freedom
+#     ldos = [ldos[2*i]+ldos[2*i+1] for i in range(len(ldos)/2)]
+#   if hetero.has_eh: # resum ldos if there is eh 
+#     ldos = [ldos[2*i]+ldos[2*i+1] for i in range(len(ldos)/2)]
+#  #   ne = len(ldos)/2
+#  #   ldos = [ldos[i]+ldos[ne+i] for i in range(ne)]
+#
+#
+#   ldos = np.array(ldos) # transform into an array
+#
+#   if min(ldos)<0.0:
+#     print("Negative density of states")
+#     raise
+#
+#   g = hetero.central_geometry # geometry of the central part
+#   fldos = open("LDOS.OUT","w") # open file for ldos
+#   fldos.write("# X   Y    LDOS\n")
+#   for (ix,iy,il) in zip(g.x,g.y,ldos):
+#     fldos.write(str(ix)+"  "+str(iy)+"  "+str(il)+"\n")
+#   fldos.close()
+#   # scale the ldos
+#   # save the LDOS in a file
+#   if True:
+##   if True>0.001:
+##     ldos = np.sqrt(ldos)
+##     ldos = np.arctan(7.*ldos/max(ldos))
+#     print("Sum of the LDOS =",sum(ldos))
+#     ldos = ldos*300/max(ldos)
+#   else:
+#     ldos = ldos*0.0
+#
+#
+#
+#
+#
+#   # now create the figure
+#   fig = py.figure() # create figure
+#   fig.subplots_adjust(0.2,0.2)
+#   fig.set_facecolor("white") # face in white
+#   sldos = fig.add_subplot(111) # create subplot for the DOS
+#
+#   # plot the lattice
+#   if not len(g.x)==len(ldos):
+#     raise 
+#   sldos.scatter(g.x,g.y,color="red",s=ldos) # plot the lattice
+#   sldos.scatter(g.x,g.y,color="black",s=4) # plot the lattice
+#   sldos.set_xlabel("X")
+#   sldos.set_xlabel("Y")
+#   sldos.axis("equal") # same scale in axes
+#
+#
+#
+#   return fig
+#
 
 
 
 
 
 
 def create_leads_and_central_list(h_right,h_left,list_h_central,
         right_coupling = None,left_coupling = None,
+        scale_right_coupling = 1.0,
+        scale_left_coupling = 1.0,
         coupling=lambda i,j: 1.0):
-  """ Creates an heterojunction by giving the hamiltonian
-     of the leads and the list of the center """
-  # check the hamiltonians
-#  h_right.check()
-#  h_left.check()
-  # convert to the classical way
-  h_right = h_right.get_no_multicell()
-  h_left = h_left.get_no_multicell()
-  list_h_central = [h.get_no_multicell() for h in list_h_central]
-  if len(list_h_central)==1: # only one central part
-    return create_leads_and_central(h_right,h_left,list_h_central[0])
-  ht = heterostructure(h_right) # create heterostructure
-  # assign matrices of the leads
-  ht.right_intra = h_right.intra.copy() 
-  ht.right_inter = h_right.inter.copy()  
-  ht.left_intra = h_left.intra.copy()  
-  ht.left_inter = h_left.inter.H.copy() 
-  # elecron hole stuff
-  ht.has_eh = h_right.has_eh # if it has electron-hole
-  ht.get_eh_sector = h_right.get_eh_sector # if it has electron-hole
-  # create matrix of the central part and couplings to the leads
-  from scipy.sparse import csc_matrix,bmat
-  z = csc_matrix(h_right.intra*0.0j) # zero matrix
-  num_central = len(list_h_central) # length of the central hamiltonian
-  # create list of lists for the central part
-  hc = [[None for i in range(num_central)] for j in range(num_central)]
-  # create elements of the central hamiltonian
-  for i in range(num_central):  # intra term of the central blocks
-    hc[i][i] = list_h_central[i].intra.copy()  # intra term of the iesim
-  for i in range(num_central-1):  # intra term of the central blocks
-    tr = list_h_central[i].inter + list_h_central[i+1].inter
-    tr = tr/2.*coupling(i,i+1)   # mean value of the hoppings
-    hc[i][i+1] = tr # inter term of the iesim
-    hc[i+1][i] = tr.H # inter term of the iesim
-
-  # hoppings to the leads
-  tcr = h_right.inter.copy()    # this is a matrix
-  tcl = h_left.inter.H.copy()   # this is a matrix
-  ht.block_diagonal = True
-  # hoppings from the center to the leads
-  if right_coupling is not None:
-    ht.right_coupling = right_coupling
-  else:
-    ht.right_coupling = h_right.inter.copy() 
-  if left_coupling is not None:
-    ht.left_coupling = left_coupling
-  else:
-    ht.left_coupling = h_left.inter.H.copy() 
-  # assign central hamiltonian
-  ht.central_intra = hc
-  # and modify the geometry of the central part
-  ht.central_geometry.supercell(num_central) 
-  # put if it si sparse
-  ht.is_sparse = list_h_central[0].is_sparse
-  return ht
+    """ Creates an heterojunction by giving the hamiltonian
+       of the leads and the list of the center """
+    # check the hamiltonians
+  #  h_right.check()
+  #  h_left.check()
+    # convert to the classical way
+    h_right = h_right.get_no_multicell()
+    h_left = h_left.get_no_multicell()
+    list_h_central = [h.get_no_multicell() for h in list_h_central]
+    if len(list_h_central)==1: # only one central part
+      return create_leads_and_central(h_right,h_left,list_h_central[0])
+    ht = heterostructure(h_right) # create heterostructure
+    ht.Hr = h_right # store
+    ht.Hl = h_left # store
+    # assign matrices of the leads
+    ht.right_intra = h_right.intra.copy() 
+    ht.right_inter = h_right.inter.copy()  
+    ht.left_intra = h_left.intra.copy()  
+    ht.left_inter = dagger(h_left.inter).copy() 
+    # elecron hole stuff
+    ht.has_eh = h_right.has_eh # if it has electron-hole
+    ht.get_eh_sector = h_right.get_eh_sector # if it has electron-hole
+    # create matrix of the central part and couplings to the leads
+    from scipy.sparse import csc_matrix,bmat
+    z = csc_matrix(h_right.intra*0.0j) # zero matrix
+    num_central = len(list_h_central) # length of the central hamiltonian
+    # create list of lists for the central part
+    hc = [[None for i in range(num_central)] for j in range(num_central)]
+    # create elements of the central hamiltonian
+    for i in range(num_central):  # intra term of the central blocks
+      hc[i][i] = list_h_central[i].intra.copy()  # intra term of the iesim
+    for i in range(num_central-1):  # intra term of the central blocks
+      tr = list_h_central[i].inter + list_h_central[i+1].inter
+      tr = tr/2.*coupling(i,i+1)   # mean value of the hoppings
+      hc[i][i+1] = tr # inter term of the iesim
+      hc[i+1][i] = tr.H # inter term of the iesim
+  
+    # hoppings to the leads
+    tcr = h_right.inter.copy()    # this is a matrix
+    tcl = dagger(h_left.inter).copy()   # this is a matrix
+    ht.block_diagonal = True
+    # hoppings from the center to the leads
+    if right_coupling is not None:
+      ht.right_coupling = right_coupling*scale_right_coupling
+    else:
+      ht.right_coupling = h_right.inter*scale_right_coupling
+    if left_coupling is not None:
+      ht.left_coupling = left_coupling*scale_left_coupling
+    else:
+      ht.left_coupling = dagger(h_left.inter)*scale_left_coupling
+  
+    # assign central hamiltonian
+    ht.central_intra = hc
+#    # and modify the geometry of the central part
+#    ht.central_geometry.supercell(num_central) 
+#    # put if it si sparse
+#    ht.is_sparse = list_h_central[0].is_sparse
+    return ht
 
 
 def eigenvalues(hetero,numeig=10,effective=False,gf=None,full=False):
   """ Gets the lowest eigenvalues of the central part of the hamiltonian"""
   if not hetero.block_diagonal:
     print(""" heterounction in eigenvalues must be block diagonal""")
     raise
@@ -751,199 +740,70 @@
 #     hetero.heff = bmat(heff)
      if write: # save hamiltonian
        print("Saving effective hamiltonian in ",hetero.file_heff)
        hetero.write_heff() 
    return heff
 
 
-def didv(ht,energy=0.0,delta=0.00001,kwant=False,opl=None,opr=None):
+def didv(ht,energy=0.0,delta=0.00001,kwant=False,opl=None,opr=None,**kwargs):
   """Calculate differential conductance"""
   if ht.has_eh: # for systems with electons and holes
-    s = get_smatrix(ht,energy=energy,delta=delta,check=True) # get the smatrix
+    s = get_smatrix(ht,energy=energy,check=True) # get the smatrix
     r1,r2 = s[0][0],s[1][1] # get the reflection matrices
     get_eh = ht.get_eh_sector # function to read either electron or hole
     # select the normal lead
     # r1 is normal
     if np.sum(np.abs(get_eh(ht.left_intra,i=0,j=1)))<0.0001: r = r1 
     elif np.sum(np.abs(get_eh(ht.right_intra,i=0,j=1)))<0.0001: r = r2
-    else: raise
+    else:
+        print("There is SC in both leads, aborting")
+        raise
     ree = get_eh(r,i=0,j=0) # reflection e-e
     reh = get_eh(r,i=0,j=1) # reflection e-h
-    Ree = (ree.H*ree).trace()[0,0] # total e-e reflection 
-    Reh = (reh.H*reh).trace()[0,0] # total e-h reflection 
-#    print("ee=",Ree,"eh=",Reh,ree.shape)
+    Ree = np.trace(dagger(ree)@ree) # total e-e reflection 
+    Reh = np.trace(dagger(reh)@reh) # total e-h reflection 
     G = (ree.shape[0] - Ree + Reh).real # conductance
     return G
   else: 
     if kwant:
       if opl is not None or opr is not None: raise # not implemented
       from . import kwantlink 
       return kwantlink.transport(ht,energy)
-    s = get_smatrix(ht,energy=energy,delta=delta,check=True) # get the smatrix
+    s = get_smatrix(ht,energy=energy) # get the smatrix
     if opl is not None or opr is not None: # some projector given
       raise # this does not make sense
       U = [[np.identity(s[0][0].shape[0]),None],
                [None,np.identity(s[1][1].shape[0])]] # projector
       if opl is not None: U[0][0] = opl # assign this matrix
       if opr is not None: U[1][1] = opr # assign this matrix
       #### those formulas are not ok
-      s[0][0] = U[0][0]*s[0][0]*U[0][0] # new smatrix
-      s[0][1] = U[0][0]*s[0][1]*U[1][1] # new smatrix
-      s[1][0] = U[1][1]*s[1][0]*U[0][0] # new smatrix
-      s[1][1] = U[1][1]*s[1][1]*U[1][1] # new smatrix
+      s[0][0] = U[0][0]@s[0][0]@U[0][0] # new smatrix
+      s[0][1] = U[0][0]@s[0][1]@U[1][1] # new smatrix
+      s[1][0] = U[1][1]@s[1][0]@U[0][0] # new smatrix
+      s[1][1] = U[1][1]@s[1][1]@U[1][1] # new smatrix
     r1,r2,t = s[0][0],s[1][1],s[0][1] # get the reflection matrices
     # select a normal lead (both of them are)
     # r1 is normal
     ree = r1
-    Ree = (ree.H*ree).trace()[0,0] # total e-e reflection 
+    Ree = np.trace(dagger(ree)@ree) # total e-e reflection 
     G1 = (ree.shape[0] - Ree).real # conductance
-    G2 = (s[0][1]*s[0][1].H).trace()[0,0].real # total e-e transmission
+    G2 = np.trace(s[0][1]@dagger(s[0][1])).real # total e-e transmission
     return (G1+G2)/2.
 #return landauer(ht,energy=energy,delta=delta) # call usual landauer 
     
 
 
 def get_tmatrix(ht,energy=0.0,delta=0.0001):
   """Calculate the S-matrix of an heterostructure"""
   if ht.block_diagonal: raise  # not implemented
-  smatrix = get_smatrix(ht,energy=energy,delta=delta)
+  smatrix = get_smatrix(ht,energy=energy)
   return smatrix[0][1]
 
 
 
-def get_smatrix(ht,energy=0.0,delta=0.000001,as_matrix=False,check=True):
-  """Calculate the S-matrix of an heterostructure"""
-  # now do the Fisher Lee trick
-  smatrix = [[None,None],[None,None]] # smatrix in list form
-  from .green import gauss_inverse # calculate the desired green functions
-  # get the selfenergies, using the same coupling as the lead
-  selfl = ht.get_selfenergy(energy,delta=delta,lead=0,pristine=True)
-  selfr = ht.get_selfenergy(energy,delta=delta,lead=1,pristine=True)
-  if ht.block_diagonal:
-    ht2 = enlarge_hlist(ht) # get the enlaged hlist with the leads
-# selfenergy of the leads (coupled to another cell of the lead)
-    gmatrix = effective_tridiagonal_hamiltonian(ht2.central_intra,selfl,selfr,
-                                                 energy=energy,delta=delta) 
-    test_gauss = False # do the tridiagonal inversion
-#    print(selfr)
-  else: # not block diagonal
-    gmatrix = build_effective_hlist(ht,energy=energy,delta=delta,selfl=selfl,
-                                    selfr=selfr)
-    test_gauss = True # gauss only works with square matrices
-#    print(selfr)
-  # gamma functions
-  gammar = 1j*(selfr-selfr.H)
-  gammal = 1j*(selfl-selfl.H)
-  # calculate the relevant terms of the Green function
-  g11 = gauss_inverse(gmatrix,0,0,test=test_gauss)
-  g12 = gauss_inverse(gmatrix,0,-1,test=test_gauss)
-  g21 = gauss_inverse(gmatrix,-1,0,test=test_gauss)
-  g22 = gauss_inverse(gmatrix,-1,-1,test=test_gauss)
-#  print("NAN",np.sum(np.isnan(g12)))
-#  print (gammal*g12*gammar*g21).trace()
-  ######## now build up the s matrix with the fisher trick
-  # the identity can have different dimension ignore for now....
-  iden = np.matrix(np.identity(g11.shape[0],dtype=complex)) # create identity
-  iden11 = np.matrix(np.identity(g11.shape[0],dtype=complex)) # create identity
-  iden22 = np.matrix(np.identity(g22.shape[0],dtype=complex)) # create identity
-  smatrix[0][0] = -iden + 1j*sqrtm(gammal)*g11*sqrtm(gammal) # matrix
-  smatrix[0][1] = 1j*sqrtm(gammal)*g12*sqrtm(gammar) # transmission matrix
-  smatrix[1][0] = 1j*sqrtm(gammar)*g21*sqrtm(gammal) # transmission matrix
-  smatrix[1][1] = -iden + 1j*sqrtm(gammar)*g22*sqrtm(gammar) # matrix
-  if check: # check whether the matrix is unitary
-      from scipy.sparse import bmat,csc_matrix
-      smatrix2 = [[csc_matrix(smatrix[i][j]) for j in range(2)] for i in range(2)]
-      smatrix2 = bmat(smatrix2).todense()
-  #    print("Determinant",np.abs(np.linalg.det(smatrix2)))
-      error = np.max(np.abs(smatrix2.I -smatrix2.H)) #  check unitarity
-      if error> 100*delta: 
-        print("S-matrix is not unitary",error)
-#        raise
-  if as_matrix: 
-    from scipy.sparse import bmat,csc_matrix
-    smatrix2 = [[csc_matrix(smatrix[i][j]) for j in range(2)] for i in range(2)]
-    smatrix = bmat(smatrix2).todense()
-  return smatrix
-
-
-def enlarge_hlist(ht):
-  """Add a single cell of the leads to the central part"""
-  ho = ht.copy() # copy heterostructure
-  if not ht.block_diagonal: raise # check that is in block diagonal form
-  nc = len(ht.central_intra) # number of cells in the central
-  hcentral = [[None for i in range(nc+2)] for j in range(nc+2)]
-  for i in range(nc): # intraterm
-    hcentral[i+1][i+1] = ht.central_intra[i][i] # common
-  for i in range(nc-1): # interterm
-    hcentral[i+1][i+2] = ht.central_intra[i][i+1] # common
-    hcentral[i+2][i+1] = ht.central_intra[i+1][i] # common
-  # now the new terms
-  hcentral[0][0] = ht.left_intra # left
-  hcentral[0][1] = ht.left_coupling.H*ht.scale_lc # left
-  hcentral[1][0] = ht.left_coupling*ht.scale_lc # left
-  hcentral[-1][-1] = ht.right_intra # right
-  hcentral[-2][-1] = ht.right_coupling*ht.scale_rc # right
-  hcentral[-1][-2] = ht.right_coupling.H*ht.scale_rc # right
-  # store in the object
-  ho.central_intra = hcentral    
-  # and redefine the new lead couplings
-  ho.right_coupling = ht.right_inter
-  ho.left_coupling = ht.left_inter
-  return ho
-
-
-def build_effective_hlist(ht,energy=0.0,delta=0.0001,selfl=None,selfr=None):
-  """ Calculate list of effective Hamiltonian which will be inverted"""
-  if (selfl is None) or (selfr is None):
-    (selfl,selfr) = get_surface_selfenergies(ht,energy=energy,delta=delta) 
-  intra = ht.central_intra # central intracell hamiltonian
-  ce = energy +1j*delta
-  idenc = np.matrix(np.identity(len(ht.central_intra),dtype=complex))*ce
-  idenl = np.matrix(np.identity(len(ht.left_intra),dtype=complex))*ce 
-  idenr = np.matrix(np.identity(len(ht.right_intra),dtype=complex))*ce 
-  hlist = [[None for i in range(3)] for j in range(3)] # list of matrices
-  # set up the different elements
-  # first the intra terms
-  hlist[0][0] = idenl - ht.left_intra - selfl
-  hlist[1][1] = idenc - ht.central_intra
-  hlist[2][2] = idenr - ht.right_intra - selfr
-  # now the inter cell
-  hlist[0][1] = -ht.left_coupling.H
-  hlist[1][0] = -ht.left_coupling
-  hlist[2][1] = -ht.right_coupling.H
-  hlist[1][2] = -ht.right_coupling
-  return hlist
-
-
-
-
-
-def sqrtm(M):
-    """Square root for Hermitian matrix"""
-    (m2,evecs) = sqrtm_rotated(M)
-    m2 = evecs.H * m2 * evecs  # change of basis
-    return m2 # return matrix
-
-
-#from scipy.linalg import sqrtm
-
-
-def sqrtm_rotated(M):
-    """Square root for Hermitian matrix in the diagonal basis,
-    and rotation matrix"""
-    import scipy.linalg as lg
-    (evals,evecs) = lg.eigh(M) # eigenvals and eigenvecs
-    if np.min(evals)<-0.001: 
-      raise  # if it is not positive defined
-    evecs = np.matrix(evecs).H # change of basis
-    m2 = np.matrix([[0.0 for i in evals] for j in evals]) # create matrix
-    for i in range(len(evals)):  m2[i,i] = np.sqrt(np.abs(evals[i])) # square root
-#    m2 = evecs.H * m2 * evecs  # change of basis
-    return (m2,evecs) # return matrix
-
 
 
 
 
 
 
 
@@ -1001,65 +861,22 @@
 def get_surface_selfenergies(hetero,energy=0.0,delta=0.0001,pristine=False):
    """Calculate left and right selfenergies"""
    (gl,gr) = get_surface_green(hetero,energy=energy,delta=delta)
    if pristine:
      inter = hetero.left_inter
    else:
      inter = hetero.left_coupling
-   selfl = inter*gl*inter.H # left selfenergy
+   selfl = inter@gl@np.conjugate(inter).T # left selfenergy
    # right selfenergy
    if pristine:
      inter = hetero.right_inter
    else:
      inter = hetero.right_coupling
-   selfr = inter*gr*inter.H # right selfenergy
+   selfr = inter@gr@np.conjugate(inter).T # right selfenergy
    return (selfl,selfr) # return selfenergies
 
 
-def effective_tridiagonal_hamiltonian(intra,selfl,selfr,
-                                        energy = 0.0, delta=0.00001):
-  """ Calculate effective Hamiltonian""" 
-  if not type(intra) is list: raise # assume is list
-  n = len(intra) # number of blocks
-  iout = [[None for i in range(n)] for j in range(n)] # empty list
-  iden = np.matrix(np.identity(intra[0][0].shape[0],dtype=np.complex))
-  ez = iden*(energy +1j*delta) # complex energy
-  for i in range(n):
-    iout[i][i] = ez - intra[i][i] # simply E -H
-  for i in range(n-1):
-    iout[i][i+1] = -intra[i][i+1] # simply E -H
-    iout[i+1][i] = -intra[i+1][i] # simply E -H
-  # and now the selfenergies
-  iout[0][0] = iout[0][0] -selfl
-  iout[-1][-1] = iout[-1][-1] -selfr
-  return iout
-
 
 
+from .transporttk.builder import build
 
-
-def build(h1,h2,central=None,lc=1.0,rc=1.0,**kwargs):
-  """Create a heterostructure, works also for 2d"""
-  if central is None: central = [h1,h2] # list
-  if h1.dimensionality==1: # one dimensional
-    return create_leads_and_central_list(h1,h2,central) # standard way
-  elif h1.dimensionality==2:  # two dimensional
-    def fun(k):
-      # evaluate at a particular k point
-      h1p = h1.get_1dh(k)
-      h2p = h2.get_1dh(k)
-      centralp = [hc.get_1dh(k) for hc in central]
-      out = create_leads_and_central_list(h1p,h2p,centralp) # standard way
-      out.scale_lc = lc
-      out.scale_rc = rc
-      return out # return 1d heterostructure
-    hout = heterostructure() # create
-    hout.dimensionality = 2 # two dimensional
-    hout.generate = fun # function that generates the heterostructure
-    return hout # function that return a heterostructure
-  else: raise
-
-
-
-def get_full_sparse():
-  """Return a heterostrure in full sparse form"""
-  
+from .transporttk.smatrix import get_smatrix
```

### Comparing `pyqula-0.0.8/src/pyqula/hexagonal.py` & `pyqula-0.0.9/src/pyqula/hexagonal.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/htk/eigenvectors.py` & `pyqula-0.0.9/src/pyqula/htk/eigenvectors.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/htk/fusion.py` & `pyqula-0.0.9/src/pyqula/htk/fusion.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/htk/g2h.py` & `pyqula-0.0.9/src/pyqula/htk/g2h.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/htk/hamiltonianmodify.py` & `pyqula-0.0.9/src/pyqula/htk/hamiltonianmodify.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/htk/matrixcomponent.py` & `pyqula-0.0.9/src/pyqula/htk/matrixcomponent.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/htk/mode.py` & `pyqula-0.0.9/src/pyqula/htk/mode.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,8 +42,21 @@
     for i in range(ntries):
       k = np.random.random(3)
       m = hk1(k) - hk2(k)
       if np.max(np.abs(m))>0.000001: return False
     return True
 
 
-
+def turn_spinful(self,enforce_tr=False):
+    """Turn the hamiltonian spinful"""
+    if self.has_spin: return # already spinful
+    if self.is_sparse: # sparse Hamiltonian
+      self.turn_dense() # dense Hamiltonian
+      self.turn_spinful(enforce_tr=enforce_tr) # spinful
+      self.turn_sparse()
+    else: # dense Hamiltonian
+      from ..increase_hilbert import spinful
+      def fun(m):
+          if enforce_tr: return spinful(m,np.conjugate(m))
+          else: return spinful(m)
+      self.modify_hamiltonian_matrices(fun) # modify the matrices
+      self.has_spin = True # set spinful
```

### Comparing `pyqula-0.0.8/src/pyqula/htk/symmetry.py` & `pyqula-0.0.9/src/pyqula/htk/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/hybrid.py` & `pyqula-0.0.9/src/pyqula/hybrid.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/increase_hilbert.py` & `pyqula-0.0.9/src/pyqula/increase_hilbert.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/indexing.py` & `pyqula-0.0.9/src/pyqula/indexing.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/inout.py` & `pyqula-0.0.9/src/pyqula/inout.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/integration.py` & `pyqula-0.0.9/src/pyqula/integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -77,13 +77,18 @@
       if np.mean(np.abs(diff))<np.mean(np.max(yt/(it+1.)))*df:
           break
       yold = yt + 0. # update
     return yt/(it+1.) # return result
 
 
 
-
-
+def peak_integrate(f,x0,x1,xp=0.0,dp=1e-6,**kwargs):
+    """Wrapper to quad, for function that has a peak"""
+    from scipy.integrate import quad
+    i0 = quad(f,x0,xp-dp,**kwargs) # first interval
+    i1 = quad(f,xp-dp,xp+dp,**kwargs) # second interval
+    i2 = quad(f,xp+dp,x1,**kwargs) # third interval
+    return i1+i2+i2
```

### Comparing `pyqula-0.0.8/src/pyqula/interactions/vijkl.py` & `pyqula-0.0.9/src/pyqula/interactions/vijkl.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/interpolatetk/atomicinterpolation.py` & `pyqula-0.0.9/src/pyqula/interpolatetk/atomicinterpolation.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/interpolation.py` & `pyqula-0.0.9/src/pyqula/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/ipr.py` & `pyqula-0.0.9/src/pyqula/ipr.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/islands.py` & `pyqula-0.0.9/src/pyqula/islands.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/junctions.py` & `pyqula-0.0.9/src/pyqula/junctions.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/kanemele.py` & `pyqula-0.0.9/src/pyqula/kanemele.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/kdos.py` & `pyqula-0.0.9/src/pyqula/kdos.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,17 +286,14 @@
     return outstr
   out = parallel.pcall(computek,range(len(kpath))) # compute all
   fo = open("KDOS_INTERFACE.OUT","w")
   fo.write("# k, E, Bulk1, Surf1, Bulk2, Surf2, interface\n")
   for o in out: fo.write(o)
   fo.close()
 
-#      fo.flush() # flush
-#  fo.close()
-
 
 
 
 
 
 
 def surface(h1,energies=np.linspace(-1.,1.,100),operator=None,
```

### Comparing `pyqula-0.0.8/src/pyqula/kekule.py` & `pyqula-0.0.9/src/pyqula/kekule.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/keldysh.py` & `pyqula-0.0.9/src/pyqula/keldysh.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/klist.py` & `pyqula-0.0.9/src/pyqula/klist.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/kpm.py` & `pyqula-0.0.9/src/pyqula/kpm.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/kwantlink.py` & `pyqula-0.0.9/src/pyqula/kwantlink.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/ldos.py` & `pyqula-0.0.9/src/pyqula/ldos.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,18 +188,20 @@
 
 
 
 
 def ldosmap(h,energies=np.linspace(-1.0,1.0,40),delta=None,
         nk=40,operator=None,**kwargs):
   """Write a map of the ldos using full diagonalization"""
+  if h.dimensionality == 0: nk = 1
   if delta is None:
     delta = (np.max(energies)-np.min(energies))/len(energies) # delta
   hkgen = h.get_hk_gen() # get generator
   dstot = np.zeros((len(energies),h.intra.shape[0])) # initialize
+  operator = h.get_operator(operator)
   def getd(k): # get LDOS
     hk = hkgen(k) # get Hamiltonian
     # LDOS for this kpoint
     ds = ldos_waves(hk,k=k,es=energies,delta=delta,operator=operator,**kwargs) 
     return ds
   ks = [np.random.random(3) for ik in range(nk)] # kpoints
   ds = parallel.pcall(getd,ks) # get densities
@@ -209,18 +211,17 @@
   return energies,np.array(dstot)
 
 
 
 def spatial_energy_profile(h,**kwargs):
   """Computes the DOS for each site of an slab, only for 2d"""
   if h.dimensionality==0:
-      pos = h.geometry.x
-      nk = 1
-  elif h.dimensionality==1: pos = h.geometry.y
-  elif h.dimensionality==2: pos = h.geometry.z
+      pos = h.geometry.r[:,0]
+  elif h.dimensionality==1: pos = h.geometry.r[:,1]
+  elif h.dimensionality==2: pos = h.geometry.r[:,2]
   else: raise
   es,ds = ldosmap(h,**kwargs)
   if len(ds[0])!=len(pos): 
     print("Wrong dimensions",len(ds[0]),len(pos))
     raise
   f = open("DOSMAP.OUT","w")
   f.write("# energy, index, DOS, position\n")
```

### Comparing `pyqula-0.0.8/src/pyqula/ldostk/atomicmultildos.py` & `pyqula-0.0.9/src/pyqula/ldostk/atomicmultildos.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/ldostk/ldosr.py` & `pyqula-0.0.9/src/pyqula/ldostk/ldosr.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/magneticexchange.py` & `pyqula-0.0.9/src/pyqula/magneticexchange.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/magnetism.py` & `pyqula-0.0.9/src/pyqula/magnetism.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,28 +26,25 @@
     elif callable(z): # it is a function
         m = z(r) # call
         if checkclass.is_iterable(m): return np.array(m) # it is an array
         else: return np.array([0.,0.,m]) # number
     else: return np.array([0.,0.,z]) # just a number
   from scipy.sparse import coo_matrix as coo
   from scipy.sparse import bmat
-  if h.has_spin: # only if the system has spin
-   # no = h.num_orbitals # number of orbitals (without spin)
-    no = len(h.geometry.r) # number of orbitals (without spin)
-    # create matrix to add to the hamiltonian
-    bzee = [[None for i in range(no)] for j in range(no)]
-    # assign diagonal terms
-    r = h.geometry.r  # z position
-    for i in range(no):
-        JJ = evaluate_J(zeeman,r[i],i) # evaluate the exchange
-        bzee[i][i] = JJ[0]*sx+JJ[1]*sy+JJ[2]*sz
-    bzee = bmat(bzee) # create matrix
-    h.intra = h.intra + h.spinful2full(bzee) # Add matrix 
-  if not h.has_spin:  # still have to implement this...
-    raise
+  if not h.has_spin:  h.turn_spinful()
+  no = len(h.geometry.r) # number of orbitals (without spin)
+  # create matrix to add to the hamiltonian
+  bzee = [[None for i in range(no)] for j in range(no)]
+  # assign diagonal terms
+  r = h.geometry.r  # z position
+  for i in range(no):
+      JJ = evaluate_J(zeeman,r[i],i) # evaluate the exchange
+      bzee[i][i] = JJ[0]*sx+JJ[1]*sy+JJ[2]*sz
+  bzee = bmat(bzee) # create matrix
+  h.intra = h.intra + h.spinful2full(bzee) # Add matrix 
 
 
 
 
 
 def add_antiferromagnetism(h,m):
   """ Adds to the intracell matrix an antiferromagnetic imbalance """
@@ -133,31 +130,19 @@
       ms.append(-g.r[int(ii)]*m) # save this one
   h.add_magnetism(ms) # add the magnetization
 
 
 
 
 
-def get_magnetization(h,nkp=20):
+def compute_magnetization(h,**kwargs):
   """Return the magnetization of the system"""
-  totkp = nkp**(h.dimensionality)
-  nat = h.intra.shape[0]//2 # number of atoms
-  eigvals,eigvecs = h.get_eigenvectors(nk=nkp)
-  voccs = [] # accupied vectors
-  eoccs = [] # accupied eigenvalues
-  occs = [] # accupied eigenvalues
-  for (e,v) in zip(eigvals,eigvecs): # loop over eigenvals,eigenvecs
-    if e<0.0000001:  # if level is filled, add contribution
-      voccs.append(v) # store
-      eoccs.append(e) # store
-  pdup = np.array([[2*i,2*i] for i in range(nat)]) # up density
-  pddn = pdup + 1 # down density
-  pxc = np.array([[2*i,2*i+1] for i in range(nat)]) # exchange
-  from . import correlatorsf90
-  vdup = correlatorsf90.correlators(voccs,pdup)/totkp
-  vddn = correlatorsf90.correlators(voccs,pddn)/totkp
-  vxc = correlatorsf90.correlators(voccs,pxc)/totkp
-  magnetization = np.array([vxc.real,vxc.imag,vdup-vddn]).transpose().real
-  from .scftypes import write_magnetization
-  write_magnetization(magnetization)
-
+  if not h.has_spin: raise # meaningless
+  if h.has_eh: raise # not implemented
+  from .densitymatrix import full_dm
+  dm = full_dm(h,**kwargs) # compute density matrix
+  n = dm.shape[0]//2 # number of orbitals
+  mz = np.array([dm[2*i,2*i] - dm[2*i+1,2*i+1] for i in range(n)])/2..real
+  mx = np.array([dm[2*i,2*i+1].real for i in range(n)])
+  my = np.array([dm[2*i,2*i+1].imag for i in range(n)])
+  return (mx,my,mz)
```

### Comparing `pyqula-0.0.8/src/pyqula/massive_green.py` & `pyqula-0.0.9/src/pyqula/massive_green.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/meanfield.py` & `pyqula-0.0.9/src/pyqula/meanfield.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/merge.py` & `pyqula-0.0.9/src/pyqula/merge.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/mullen.py` & `pyqula-0.0.9/src/pyqula/mullen.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/multicell.py` & `pyqula-0.0.9/src/pyqula/multicell.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/multihopping.py` & `pyqula-0.0.9/src/pyqula/multihopping.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/multilayers.py` & `pyqula-0.0.9/src/pyqula/multilayers.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/multiterminal.py` & `pyqula-0.0.9/src/pyqula/multiterminal.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/neighbor.py` & `pyqula-0.0.9/src/pyqula/neighbor.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/nodes.py` & `pyqula-0.0.9/src/pyqula/nodes.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/nonhermitian/orthogonality.py` & `pyqula-0.0.9/src/pyqula/nonhermitian/orthogonality.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/numbaneighbor.py` & `pyqula-0.0.9/src/pyqula/numbaneighbor.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/old_chi.py` & `pyqula-0.0.9/src/pyqula/old_chi.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/operatorlist.py` & `pyqula-0.0.9/src/pyqula/operatorlist.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/operators.py` & `pyqula-0.0.9/src/pyqula/operators.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/parallel.py` & `pyqula-0.0.9/src/pyqula/parallel.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/parallelslurm.py` & `pyqula-0.0.9/src/pyqula/parallelslurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import dill as pickle
 import os
 from . import filesystem as fs
 import signal
 import subprocess
 
-srcpath = os.path.dirname(os.path.realpath(__file__)) 
+srcpath = os.path.dirname(os.path.realpath(__file__))+"/.." 
 
-#pickle.settings['recurse'] = True
+pickle.settings['recurse'] = True
 
 def pcall(fin,xs,batch_size=1,**kwargs):
     """Wrapper to allow for a batch size"""
     if batch_size==1: return pcall_single(fin,xs,**kwargs)
     else: 
         nx = len(xs) # number of xs
         xsn = [] # empty list
@@ -30,15 +30,15 @@
 
 
 def pcall_single(fin,xs,time=10,error=None):
     """Run a parallel calculation with slurm"""
     n = len(xs) # number of calculations
     f = lambda x: fin(x)
     main = "import dill as pickle\nimport os\n"
-    main += "import sys ; sys.path.append("+srcpath+")\n"
+    main += "import sys ; sys.path.append('"+srcpath+"')\n"
     main += "try: ii = int(os.environ['SLURM_ARRAY_TASK_ID'])\n"
     main += "except: ii = 0\n"
     main += "f = pickle.load(open('function.obj','rb'))\n"
     main += "v = pickle.load(open('array.obj','rb'))\n"
     main += "folder = 'folder_'+str(ii)\n"
     main += "os.system('mkdir '+folder)\n"
     main += "os.chdir(folder)\n"
```

### Comparing `pyqula-0.0.8/src/pyqula/peierls.py` & `pyqula-0.0.9/src/pyqula/peierls.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/phasediagram.py` & `pyqula-0.0.9/src/pyqula/phasediagram.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/potentials.py` & `pyqula-0.0.9/src/pyqula/potentials.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/pseudocontact.py` & `pyqula-0.0.9/src/pyqula/pseudocontact.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/rashba.py` & `pyqula-0.0.9/src/pyqula/rashba.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/reciprocalmap.py` & `pyqula-0.0.9/src/pyqula/reciprocalmap.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/reduce.py` & `pyqula-0.0.9/src/pyqula/reduce.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/response.py` & `pyqula-0.0.9/src/pyqula/response.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/ribbon.py` & `pyqula-0.0.9/src/pyqula/ribbon.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/ribbonizate.py` & `pyqula-0.0.9/src/pyqula/ribbonizate.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/rkky.py` & `pyqula-0.0.9/src/pyqula/rkky.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/rotate_spin.py` & `pyqula-0.0.9/src/pyqula/rotate_spin.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/sanitycheck.py` & `pyqula-0.0.9/src/pyqula/sanitycheck.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/scftk/updatescf.py` & `pyqula-0.0.9/src/pyqula/scftk/updatescf.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/scftypes.py` & `pyqula-0.0.9/src/pyqula/scftypes.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/sctk/dvector.py` & `pyqula-0.0.9/src/pyqula/sctk/dvector.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/sctk/extract.py` & `pyqula-0.0.9/src/pyqula/sctk/extract.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/sctk/orderparameter.py` & `pyqula-0.0.9/src/pyqula/sctk/orderparameter.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/sctk/pairing.py` & `pyqula-0.0.9/src/pyqula/sctk/pairing.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     elif mode=="swaveB":
         weightf = lambda r1,r2: swaveB(self.geometry,r1,r2)
     elif mode=="swavesublattice":
         def weightf(r1,r2):
           return swaveB(self.geometry,r1,r2) - swaveA(self.geometry,r1,r2)
     elif mode=="dx2y2":
         weightf = lambda r1,r2: dx2y2(r1,r2)
+    elif mode=="dxy":
+        weightf = lambda r1,r2: dxy(r1,r2)
     elif mode=="snn":
         weightf = lambda r1,r2: swavenn(r1,r2)
     elif mode=="C3nn":
         weightf = lambda r1,r2: C3nn(r1,r2)
     elif mode=="SnnAB":
         weightf = lambda r1,r2: SnnAB(self.geometry,r1,r2)
     else: raise
@@ -69,14 +71,26 @@
     dr = r1-r2
     dr2 = dr.dot(dr)
     if 0.99<dr2<1.001: # first neighbor
         return (dr[0]**2 - dr[1]**2)*iden
     return 0.0*iden
 
 
+def dxy(r1,r2):
+    """Function with first neighbor dx2y2 profile"""
+    dr = r1-r2
+    dr2 = dr.dot(dr)
+    if 0.99<dr2<1.001: # first neighbor
+        return (dr[0]*dr[1])*iden
+    return 0.0*iden
+
+
+
+
+
 def C3nn(r1,r2):
     """Function with first neighbor C3 profile"""
     dr = r1-r2
     dr2 = dr.dot(dr)
     if 0.99<dr2<1.001: # first neighbor
 #        return dr[0]
         phi = np.arctan2(dr[1],dr[0]) # angle
```

### Comparing `pyqula-0.0.8/src/pyqula/sctk/spinless.py` & `pyqula-0.0.9/src/pyqula/sctk/spinless.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/sculpt.py` & `pyqula-0.0.9/src/pyqula/sculpt.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/attractive_hubbard_spinless.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/attractive_hubbard_spinless.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/coulomb.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/coulomb.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/densitydensity.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/densitydensity.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/hubbard.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/hubbard.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/mfconstrains.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/mfconstrains.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/mixing.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/mixing.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/potentials.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/potentials.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/selfconsistency/superscf.py` & `pyqula-0.0.9/src/pyqula/selfconsistency/superscf.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/skeleton.py` & `pyqula-0.0.9/src/pyqula/skeleton.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/specialgeometry.py` & `pyqula-0.0.9/src/pyqula/specialgeometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,21 +298,21 @@
 def parse_twisted_multimultilayer(name,n=3):
     """Given a name for a multilayer, return the geometry"""
     # name is two element list
     # second element is the list with aligned stacking
     # thirs element determines whether if they are rotated
     gs = [] # empty list
     for ni in name[0]: # loop over names of the layers
-            if ni in ["","A"]: gi = multilayer_graphene([0]) # normal honeycomb
-            elif ni=="AA": gi = multilayer_graphene([0,0]) 
-            elif ni=="AB": gi = multilayer_graphene([0,1]) 
-            elif ni=="BA": gi = multilayer_graphene([1,0]) 
-            elif ni=="ABC": gi = multilayer_graphene([0,1,2]) 
-            elif ni=="ABAB": gi = multilayer_graphene([0,1,0,1]) 
-            elif ni=="ABBA": gi = multilayer_graphene([0,1,1,0]) 
+            if ni in ["","A"]: gi = multilayer_graphene(l=[0]) # normal honeycomb
+            elif ni=="AA": gi = multilayer_graphene(l=[0,0]) 
+            elif ni=="AB": gi = multilayer_graphene(l=[0,1]) 
+            elif ni=="BA": gi = multilayer_graphene(l=[1,0]) 
+            elif ni=="ABC": gi = multilayer_graphene(l=[0,1,2]) 
+            elif ni=="ABAB": gi = multilayer_graphene(l=[0,1,0,1]) 
+            elif ni=="ABBA": gi = multilayer_graphene(l=[0,1,1,0]) 
             else: raise
             gs.append(gi) # store
     rot = name[1] # rotations
     return twisted_multimultilayer(rot=rot,g=gs,m0=n)
```

### Comparing `pyqula-0.0.8/src/pyqula/specialhamiltonian.py` & `pyqula-0.0.9/src/pyqula/specialhamiltonian.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,19 +66,16 @@
     #return TMDC_MX2(**kwargs,ts=[0.2,2.,0.6,0.2,0.])
 
 def TMDC_MX2(soc=0.0,cdw=0.0,g=None,ts=[1.0]):
     """Return the Hamiltonian of NbSe2"""
     if g is None: 
         g = geometry.triangular_lattice()  # triangular lattice
         if cdw!=0.0: g = g.supercell(3)
-#    ts = np.array([86.8,139.9,29.6,3.5,3.3])
-#    ts = np.array([46.,257.5,4.4,-15,6])
     ts = np.array(ts)
     t = ts[0]/np.max(ts) # 1NN 
-#    ts[0] = 0.0 # set to zero
     ts = ts/np.max(ts) # normalize
     fm = specialhopping.neighbor_hopping_matrix(g,ts) # function for hoppings
     h = g.get_hamiltonian(mgenerator=fm,is_multicell=True,has_spin=False,
             cutoff=len(ts))
     ## Now add the SOC if necessary
     if soc!=0.0: # add the SOC
         h.turn_spinful() # turn spinful
@@ -105,15 +102,15 @@
     
 
 
 
 def triangular_pi_flux(g=None,**kwargs):
     """Return a pi-flux Hamiltonian"""
     if g is None: # no geometry given
-        g = geometry.triangular_lattice() # geometry of a traingular lattice
+        g = geometry.triangular_lattice() # geometry of a triangular lattice
     g = g.supercell((2,1)) # create a supercell with 2 atoms
     ft = specialhopping.phase_C3_matrix(g,phi=.5)
     h = g.get_hamiltonian(mgenerator=ft,is_multicell=True,**kwargs) # return the Hamiltonian
     h.add_peierls(2*np.pi*1./np.sqrt(3.),gauge="Landau") # field
     from . import gauge
 #    h = gauge.hamiltonian_gauge_transformation(h,[0.,0.25])
 #    return h
```

### Comparing `pyqula-0.0.8/src/pyqula/specialhopping.py` & `pyqula-0.0.9/src/pyqula/specialhopping.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/spectrum.py` & `pyqula-0.0.9/src/pyqula/spectrum.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/spintexture.py` & `pyqula-0.0.9/src/pyqula/spintexture.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/spinwaves.py` & `pyqula-0.0.9/src/pyqula/spinwaves.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/states.py` & `pyqula-0.0.9/src/pyqula/states.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/supercell.py` & `pyqula-0.0.9/src/pyqula/supercell.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/supercell_hamiltonians.py` & `pyqula-0.0.9/src/pyqula/supercell_hamiltonians.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/superconductivity.py` & `pyqula-0.0.9/src/pyqula/superconductivity.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/surface_TI.py` & `pyqula-0.0.9/src/pyqula/surface_TI.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/susceptibility.py` & `pyqula-0.0.9/src/pyqula/susceptibility.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/symmetrize.py` & `pyqula-0.0.9/src/pyqula/symmetrize.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/symmetry.py` & `pyqula-0.0.9/src/pyqula/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/tails.py` & `pyqula-0.0.9/src/pyqula/tails.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/timeevolution.py` & `pyqula-0.0.9/src/pyqula/timeevolution.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/timing.py` & `pyqula-0.0.9/src/pyqula/timing.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/tojulia.py` & `pyqula-0.0.9/src/pyqula/tojulia.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/topology.py` & `pyqula-0.0.9/src/pyqula/topology.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/topologytk/realspace.py` & `pyqula-0.0.9/src/pyqula/topologytk/realspace.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/unfolding.py` & `pyqula-0.0.9/src/pyqula/unfolding.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula/wannier.py` & `pyqula-0.0.9/src/pyqula/wannier.py`

 * *Files identical despite different names*

### Comparing `pyqula-0.0.8/src/pyqula.egg-info/PKG-INFO` & `pyqula-0.0.9/src/pyqula.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqula
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for quantum lattice tight binding models
 Home-page: https://github.com/joselado/pyqula
 Author: Jose Lado
 Author-email: joselado@aalto.fi
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/joselado/pyqula/issues
 Platform: UNKNOWN
```

### Comparing `pyqula-0.0.8/src/pyqula.egg-info/SOURCES.txt` & `pyqula-0.0.9/src/pyqula.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 src/pyqula/reciprocalmap.py
 src/pyqula/reduce.py
 src/pyqula/response.py
 src/pyqula/ribbon.py
 src/pyqula/ribbonizate.py
 src/pyqula/rkky.py
 src/pyqula/rotate_spin.py
+src/pyqula/rpa.py
 src/pyqula/sanitycheck.py
 src/pyqula/scftypes.py
 src/pyqula/sculpt.py
 src/pyqula/skeleton.py
 src/pyqula/slabs.py
 src/pyqula/specialgeometry.py
 src/pyqula/specialhamiltonian.py
@@ -125,33 +126,39 @@
 src/pyqula.egg-info/SOURCES.txt
 src/pyqula.egg-info/dependency_links.txt
 src/pyqula.egg-info/top_level.txt
 src/pyqula/algebratk/__init__.py
 src/pyqula/algebratk/hamiltonianalgebra.py
 src/pyqula/algebratk/matrixcrop.py
 src/pyqula/algebratk/sparsetensor.py
+src/pyqula/algebratk/unitary.py
 src/pyqula/chitk/__init__.py
 src/pyqula/chitk/epsilon.py
 src/pyqula/chitk/qpi.py
 src/pyqula/energeticstk/__init__.py
 src/pyqula/energeticstk/alloytk.py
 src/pyqula/geometrytk/__init__.py
 src/pyqula/geometrytk/readgeometry.py
 src/pyqula/htk/__init__.py
+src/pyqula/htk/cdw.py
+src/pyqula/htk/dummy.py
 src/pyqula/htk/eigenvectors.py
 src/pyqula/htk/fusion.py
 src/pyqula/htk/g2h.py
 src/pyqula/htk/hamiltonianmodify.py
 src/pyqula/htk/matrixcomponent.py
 src/pyqula/htk/mode.py
+src/pyqula/htk/modify.py
 src/pyqula/htk/symmetry.py
 src/pyqula/interactions/__init__.py
 src/pyqula/interactions/vijkl.py
 src/pyqula/interpolatetk/__init__.py
 src/pyqula/interpolatetk/atomicinterpolation.py
+src/pyqula/interpolatetk/constrainedinterpolation.py
+src/pyqula/interpolatetk/outlier.py
 src/pyqula/ldostk/__init__.py
 src/pyqula/ldostk/atomicmultildos.py
 src/pyqula/ldostk/ldosr.py
 src/pyqula/nonhermitian/__init__.py
 src/pyqula/nonhermitian/orthogonality.py
 src/pyqula/scftk/__init__.py
 src/pyqula/scftk/updatescf.py
```

