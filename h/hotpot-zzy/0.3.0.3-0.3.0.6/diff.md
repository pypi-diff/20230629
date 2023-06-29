# Comparing `tmp/hotpot-zzy-0.3.0.3.tar.gz` & `tmp/hotpot-zzy-0.3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zzy/hotpot/dist/.tmp-mowkm3gi/hotpot-zzy-0.3.0.3.tar", last modified: Tue Jun 20 11:21:54 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-ejfe6vph/hotpot-zzy-0.3.0.6.tar", last modified: Thu Jun 29 09:00:36 2023, max compression
```

## Comparing `hotpot-zzy-0.3.0.3.tar` & `hotpot-zzy-0.3.0.6.tar`

### file list

```diff
@@ -1,124 +1,127 @@
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.685076 hotpot-zzy-0.3.0.3/
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1090 2023-06-20 08:50:11.000000 hotpot-zzy-0.3.0.3/LICENSE
--rwxrwx---   0 zzy       (1002) zzy       (1002)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/MANIFEST.in
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       78 2023-06-20 11:21:54.685076 hotpot-zzy-0.3.0.3/PKG-INFO
--rwxrwx---   0 zzy       (1002) zzy       (1002)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.3.0.3/README.md
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.677076 hotpot-zzy-0.3.0.3/hotpot/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      437 2023-06-19 12:37:49.000000 hotpot-zzy-0.3.0.3/hotpot/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)    40740 2023-06-20 08:25:13.000000 hotpot-zzy-0.3.0.3/hotpot/_io.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.3.0.3/hotpot/bundle.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)   104270 2023-06-20 10:57:33.000000 hotpot-zzy-0.3.0.3/hotpot/cheminfo.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.677076 hotpot-zzy-0.3.0.3/hotpot/data/
--rwxrwx---   0 zzy       (1002) zzy       (1002)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.3.0.3/hotpot/data/atom_single_point.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.677076 hotpot-zzy-0.3.0.3/hotpot/data/force_field/
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.677076 hotpot-zzy-0.3.0.3/hotpot/data/force_field/UFF/
--rwxrwx---   0 zzy       (1002) zzy       (1002)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.677076 hotpot-zzy-0.3.0.3/hotpot/data/force_field/aMaterials/
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/force_field/aMaterials/SiC.tersoff
--rwxrwx---   0 zzy       (1002) zzy       (1002)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/force_field/contents.json
--rwxrwx---   0 zzy       (1002) zzy       (1002)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.681076 hotpot-zzy-0.3.0.3/hotpot/data/solvents/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1-dichloroethene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,2-dichloroethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,2-dichloroethene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,4-dioxane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1-butanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1-pentanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/1-propanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-butanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-ethoxyethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-methoxyethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/DCM.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/DMF.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/DMSO.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/THF.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/acetic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/acetone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/acetonitrile.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/benzene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/butylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/carbon_tetrachloride.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/chlorobenzene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/chloroform.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/cumene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/cyclohexane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/diethylether.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/diisopropylamine.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethyl_formate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethyleneglycol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/formamide.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/formic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/heptane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/hexane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/isobutyl_acetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/isooctane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/isopropanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/isopropylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/isopropylether.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/meta-xylene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methanol.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methoxybenzene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylbutylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylcyclohexane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylethylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylisobutylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylisopropylketone.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/morpholine.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/nitromethane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/ortho-xylene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/para-xylene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/pentane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/propylacetate.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/pyridine.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/sulfolane.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/t-butylmethylether.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/tetralin.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/toluene.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/trichloroacetic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/solvents/water.mol2
--rwxrwx---   0 zzy       (1002) zzy       (1002)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/data/units.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.681076 hotpot-zzy-0.3.0.3/hotpot/tanks/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     9488 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/cc.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/features.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.681076 hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/base.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/gcmc.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/materials.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     8528 2023-06-20 05:01:10.000000 hotpot-zzy-0.3.0.3/hotpot/tanks/quantum.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tmo.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/tools.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.681076 hotpot-zzy-0.3.0.3/hotpot/utils/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/utils/__init__.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/utils/load_chem_lib.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.681076 hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       78 2023-06-20 11:21:54.000000 hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     3862 2023-06-20 11:21:54.000000 hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)        1 2023-06-20 11:21:54.000000 hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       51 2023-06-20 11:21:54.000000 hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)        7 2023-06-20 11:21:54.000000 hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/top_level.txt
--rwxrwx---   0 zzy       (1002) zzy       (1002)      314 2023-06-20 11:21:02.000000 hotpot-zzy-0.3.0.3/pyproject.toml
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       38 2023-06-20 11:21:54.685076 hotpot-zzy-0.3.0.3/setup.cfg
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-20 11:21:54.685076 hotpot-zzy-0.3.0.3/test/
--rwxrwx---   0 zzy       (1002) zzy       (1002)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/test/test_amorphous_maker.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.3.0.3/test/test_bundle.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.3.0.3/test/test_chemif.py
--rwxrwx---   0 zzy       (1002) zzy       (1002)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.3/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1090 2023-06-27 23:43:15.000000 hotpot-zzy-0.3.0.6/LICENSE
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       78 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     6794 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/README.md
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.752101 hotpot-zzy-0.3.0.6/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      439 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    41382 2023-06-29 08:42:58.000000 hotpot-zzy-0.3.0.6/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    22583 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   112055 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.756101 hotpot-zzy-0.3.0.6/hotpot/data/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       71 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/atom_single_point.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1932 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/data/deepmd_script.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.756101 hotpot-zzy-0.3.0.6/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.756101 hotpot-zzy-0.3.0.6/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.756101 hotpot-zzy-0.3.0.6/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.764101 hotpot-zzy-0.3.0.6/hotpot/data/solvents/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      973 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1068 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      783 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      780 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2586 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1447 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      970 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      780 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1731 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1558 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,4-dioxane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1626 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1912 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1-pentanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1342 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2017 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1626 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1727 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1443 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-methoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1636 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1760 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1920 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      670 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/DCM.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1335 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/DMF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1146 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/DMSO.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1638 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1756 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1455 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/THF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      963 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/acetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1149 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/acetone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      774 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/acetonitrile.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1364 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/benzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2104 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/butylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      687 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1370 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/chlorobenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      677 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/chloroform.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2218 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/cumene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1938 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/cyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1629 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/diethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2298 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/diisopropylamine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1054 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1250 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethyl_formate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1534 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1156 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethyleneglycol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      771 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/formamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      678 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/formic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2384 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/heptane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2098 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/hexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2108 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/isobutyl_acetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2671 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/isooctane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1343 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/isopropanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1823 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/isopropylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2201 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/isopropylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1938 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/meta-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      770 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1751 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methoxybenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1250 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2014 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylbutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2229 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylcyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1444 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylethylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2017 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylisobutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1733 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylisopropylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1652 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/morpholine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      869 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/nitromethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1939 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/ortho-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1938 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/para-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1814 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/pentane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1820 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/propylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1270 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/pyridine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1651 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/sulfolane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1920 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/t-butylmethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2340 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/tetralin.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1649 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/toluene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      972 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      972 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      482 2023-06-25 14:01:32.000000 hotpot-zzy-0.3.0.6/hotpot/data/solvents/water.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.764101 hotpot-zzy-0.3.0.6/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    10087 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      325 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/deepmd.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8801 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9398 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/materials.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8640 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4091 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/utils/library.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/hotpot/utils/manage_machine.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       78 2023-06-29 09:00:36.000000 hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3941 2023-06-29 09:00:36.000000 hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-29 09:00:36.000000 hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       58 2023-06-29 09:00:36.000000 hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-29 09:00:36.000000 hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      331 2023-06-29 09:00:18.000000 hotpot-zzy-0.3.0.6/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-29 09:00:36.768101 hotpot-zzy-0.3.0.6/test/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/test/test_amorphous_maker.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1868 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/test/test_bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3020 2023-06-29 08:41:50.000000 hotpot-zzy-0.3.0.6/test/test_chemif.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.6/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.3.0.3/LICENSE` & `hotpot-zzy-0.3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/README.md` & `hotpot-zzy-0.3.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 cclib
 lammps
 ````
 
 ### Install requirement
 Before installing the `Hotpot`, you should install the requirements at the first. It is
 recommended to create a new conda environment to run the package.
-> conda create -n hp python==3.9 openbabel cclib lammps -c conda-forge
+> conda create -n hp python==3.9 openbabel cclib lammps rdkit -c conda-forge
 
 ### Install
 After the requirements are installed, now the ''Hotpot'' could be installed by pip
+> conda activate hp
+
 > pip install hotpot-zzy
 
 
 ## Usage
 The Hotpot is very easy to use, the core class of Hotpot is the `Molecule`, which is designed
 as the general interface for all functions across the entire the package. In the following
 example, we first load a Molecule object by `SMILES` string, and then the build their 3D conformer:
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/_io.py` & `hotpot-zzy-0.3.0.6/hotpot/_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             ...
         ---------------------------------- END ---------------------------------------
 """
 
 
 # Define custom Exceptions
 class IOEarlyStop(BaseException):
-    """ monitor the situation that the IO should early stop and return None a the IO result """
+    """ monitor the situation that the IO should early stop and return None and the IO result """
 
 
 # Define the IO function types
 IOFuncPrefix = Literal['pre', 'io', 'post']
 IOStream = Union[IOBase, str, bytes]
 
 
@@ -130,15 +130,15 @@
 
 class Register:
     """
     Register the IO function for Dumper, Parser or so on
     """
     def __init__(self):
         # these dicts are container to store the custom io functions
-        # the keys of the dict are serve as the have to get the mapped io functions(the values)
+        # the keys of the dict are serve as the handle to get the mapped io functions(the values)
         self.pre_methods = {}
         self.io_methods = {}
         self.post_methods = {}
 
     def __repr__(self):
         return f"Register:\n" + \
                f"pre_method:\n" + \
@@ -180,15 +180,15 @@
     def io(self, fmt: str):
         return self.io_methods.get(fmt)
 
     def post(self, fmt: str):
         return self.post_methods.get(fmt)
 
 
-# Retrieve the IO class by it's format name
+# Retrieve the IO class by its format name
 def retrieve_format(fmt: str = None):
     return _MoleculeIO.registered_format().get(fmt)
 
 
 # Get all registered format name
 def registered_format_name():
     return tuple(_MoleculeIO.registered_format().keys())
@@ -217,15 +217,15 @@
     @classmethod
     def registered_format(mcs):
         return copy(mcs._registered_format)
 
 
 class MetaIO(type):
     """
-    Meta class to specify how to construct the IO class
+    The Meta class to specify how to construct the IO class
     This Meta class is defined to register IO function conveniently.
 
     The IO functions are divided into three categories:
         - preprocess: do something before performing any of IO operation, with prefix '_pre'
         - io: performing the IO operation, with prefix '_io'
         - postprocess: do something after preforming IO operation, with prefix '_post'
 
@@ -430,17 +430,19 @@
             self.src.compact_crystal(inplace=True)
 
         if self.src.crystal().space_group:
             self.src.crystal().space_group = 'P1'
 
     def _pre_gjf(self):
         """ Assign the Molecule charge before to dump to gjf file """
-        self.src.determine_mol_charge()
         if not self.src.has_3d:
-            self.src.build_conformer()
+            self.src.build_3d()
+
+        self.src.assign_atoms_formal_charge()
+        self.src.identifier = self.src.formula
 
     def _io_dpmd_sys(self):
         """ convert molecule information to numpy arrays """
         required_items = ['coord', 'type']
         check_atom_num = ['coord', 'force', 'charge']
         share_same_configures = ['type', 'coord', 'energy', 'force', 'charge', 'virial']
         need_reshape = ['coord', 'force']
@@ -455,15 +457,15 @@
             for i in range(3):
                 box[i, i] = 100.
             is_periodic = False
         box = box.reshape(-1, 9).repeat(conf_num, axis=0)
 
         data = {
             'type': np.array(self.src.atomic_numbers).reshape(1, -1).repeat(conf_num, axis=0),
-            'type_map': ['-'] + list(ci.periodic_table.keys()),
+            'type_map': ['-'] + list(ci.periodic_table.symbols),
             'nopbc': not is_periodic,
             'coord': self.src.all_coordinates,  # angstrom,
             'box': box,
             'energy': self.src.all_energy,  # eV
             'force': self.src.all_forces,  # Hartree/Bohr,
             'charge': self.src.all_atom_charges,  # q
             'virial': None,
@@ -509,20 +511,17 @@
         def bonds(m):
             """ Add bond body """
             bond_str = 'Bonds' + '\n\n'  # bond body title
 
             # the formula of bond_type key: atom1[bond_type]atom2
             uni_bonds = tuple(m.unique_bonds)  # store bonds type
             for j, bond in enumerate(m.bonds, 1):
-                a1_idx = atoms_list.index(bond.atom1) + 1
-                a2_idx = atoms_list.index(bond.atom2) + 1
 
                 bt_id = uni_bonds.index(bond) + 1
-
-                bond_str += f'{j} {bt_id} {a1_idx} {a2_idx}\n'
+                bond_str += f'{j} {bt_id} {bond.ob_atom1_id + 1} {bond.ob_atom2_id + 1}\n'
 
             bond_str += '\n'
 
             return bond_str
 
         def charge():
             """ Retrieve atom charge information """
@@ -659,15 +658,15 @@
 
         # Write link0 command
         if isinstance(link0, str):
             lines[0] = f'%{link0}'
         elif isinstance(link0, list):
             for i, stc in enumerate(link0):  # stc=sentence
                 assert isinstance(stc, str)
-                if not i:  # For the first line of link0, replace the the original line in raw script
+                if not i:  # For the first line of link0, replace the original line in raw script
                     lines[0] = f'%{stc}'
                 else:  # For the other lines, insert into after the 1st line
                     inserted_lines += 1
                     lines.insert(inserted_lines, f'%{stc}')
         else:
             raise TypeError('the link0 should be string or list of string')
 
@@ -927,36 +926,48 @@
             1) Mulliken charge
             2) Spin densities
         """
         def extract_charges_spin():
             """ Extract charges and spin information from g16.log file """
             # Get the line index of Mulliken charges
             head_lines = [i for i, line in enumerate(lines) if line.strip() == 'Mulliken charges and spin densities:']
-            
+            if not head_lines:
+                head_lines = [i for i, line in enumerate(lines) if line.strip() == 'Mulliken charges:']
+                charge_only = True
+            else:
+                charge_only = False
+
+            # Skip the first charge&spin sheet, it can't find corresponding coordinates
             if not head_lines:
                 raise IOEarlyStop
             elif len(head_lines) == obj.configure_number + 1:
                 head_lines = head_lines[1:]
 
             # Extract the Mulliken charge and spin densities
             charges, spin_densities = [], []  # changes(cgs) spin_densities(sds)
             for i in head_lines:
                 # Enhance inspection
-                col1, col2 = lines[i + 1].strip().split()
-                assert col1 == '1' and col2 == '2'
+                col_heads = lines[i + 1].strip().split()
+                if charge_only:
+                    assert len(col_heads) == 1 and col_heads[0] == '1'
+                else:
+                    assert len(col_heads) == 2 and col_heads[0] == '1' and col_heads
 
                 HEAD_LINES_NUM = 2
                 cg, sd = [], []  # change, spin_density
 
                 while True:
                     split_line = lines[i + HEAD_LINES_NUM].strip().split()
-                    if len(split_line) != 4:
-                        break
-                    else:
+                    if charge_only and len(split_line) == 3:
+                        row, syb, c = split_line  # row number, symbol, charges
+                        s = 0.0  # spin density
+                    elif not charge_only and len(split_line) == 4:
                         row, syb, c, s = split_line  # row number, symbol, charges, spin density
+                    else:
+                        break
 
                     try:
                         row, c, s = int(row), float(c), float(s)
                         # check the sheet row number
                         if row != HEAD_LINES_NUM - 1:
                             break
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/bundle.py` & `hotpot-zzy-0.3.0.6/hotpot/bundle.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,42 @@
 @File   : bundle.py
 @Author : Zhiyuan Zhang
 @Date   : 2023/3/22
 @Time   : 3:18
 """
 import copy
 import random
+import time
 from os import PathLike
 from typing import *
 from pathlib import Path
 import numpy as np
 from tqdm import tqdm
 from openbabel import pybel as pb
 import hotpot.cheminfo as ci
 from hotpot.tools import check_path
 import multiprocessing as mp
 
 feature_formats = {
     'basic': ['atomic_number', 's', 'p', 'f']
 }
 
+# the dict to store all defined bundle classes
+_bundle_classes = {}
 
+
+def register_bundles(bundle: Type):
+    """ register the bundle to _bundle_classes """
+    _bundle_classes[bundle.__name__] = bundle
+    return bundle
+
+
+@register_bundles
 class MolBundle:
-    """"""
+    """ The basic class for all molecular bundle """
 
     def __init__(self, mols: Union[Sequence[ci.Molecule], Generator[ci.Molecule, None, None]] = None):
         self._data = {'mols': mols}
 
     def __repr__(self):
         class_name = self.__class__.__name__
         return f"{class_name}(generator)" if isinstance(self.mols, Generator) else f"{class_name}({self.mols})"
@@ -259,14 +270,78 @@
         generator = mol_mp_generator() if num_proc else mol_generator()
 
         if generate:
             return cls(generator)
         else:
             return cls([m for m in tqdm(generator, 'reading molecules')])
 
+    def gcmc_for_isotherm(
+            self, *guest: 'ci.Molecule', force_field: Union[str, PathLike] = None,
+            work_dir: Union[str, PathLike] = None, T: float = 298.15,
+            Ps: Sequence[float] = (1.0,), procs: int = 1, named_identifier: bool = False,
+            **kwargs
+    ):
+        """
+        Run gcmc to determine the adsorption of guest,
+        Args:
+            self: the framework as the sorbent of guest molecule
+            guest(Molecule): the guest molecule to be adsorbed into the framework
+            force_field(str|PathLike): the path to force field file or the self-existent force file contained
+             in force field directory (in the case, a str should be given as a relative path from the root of
+             force field root to the specified self-existent force filed). By default, the force field is UFF
+             which in the relative path 'UFF/LJ.json' for the force field path.
+            work_dir: the user-specified dir to store the result of GCMC and log file.
+            T: the environmental temperature (default, 298.15 K)
+            Ps(Sequence[float]): A sequence of relative pressure related to the saturation vapor in the environmental temperature.
+            procs(int): the number of processes, default 1.
+            named_identifier: Whether to name the dir by the identifier of frames
+        """
+        if isinstance(work_dir, str):
+            work_dir = Path(work_dir)
+
+        # Assemble keywords arguments for multiprocess
+        processes = []
+        for i, frame in enumerate(self.mols, 1):
+
+            # When the running proc more than the specified values, waiting for terminate
+            while len(processes) >= procs:
+                for p in processes:
+                    if not p.is_alive():
+                        processes.pop(processes.index(p))
+                        p.terminate()
+
+                time.sleep(10)
+
+            if named_identifier:
+                sub_work_dir = work_dir.joinpath(frame.identifier)
+            else:
+                idt_map = self._data.setdefault('identifier_map', {})
+                idt_map[i] = frame.identifier
+                sub_work_dir = work_dir.joinpath('mol_' + str(i))
+
+            if not sub_work_dir.exists():
+                sub_work_dir.mkdir()
+
+            kwargs.update({
+                'force_field': force_field,
+                'work_dir': sub_work_dir,
+                'T': T, 'Ps': Ps
+            })
+
+            p = mp.Process(target=frame.gcmc_for_isotherm, args=guest, kwargs=kwargs)
+
+            p.start()
+            processes.append(p)
+
+        for p in processes:
+            p.join()
+            p.terminate()
+
+        return self._data.get('identifier_map')
+
     def graph_representation(self, *feature_names) -> Generator[Union[str, np.ndarray, np.ndarray], None, None]:
         """ Transform molecules to their graph representation """
         for mol in self.mols:
             yield mol.graph_representation(*feature_names)
 
     def gaussian(
             self, g16root: Union[str, PathLike], dir_out: Union[str, PathLike],
@@ -330,15 +405,15 @@
             # Performing the molecule or lattice perturb
             if isinstance(perturb_kwargs, Dict):
                 perturb_kwargs = [perturb_kwargs]  # Wrap it into a list
 
             if isinstance(perturb_kwargs, List) and all(isinstance(pk, dict) for pk in perturb_kwargs):
                 for pk in perturb_kwargs:
                     pk['inplace'] = True  # Force to inplace
-                    mol.perturb_mol_lattice(**pk)
+                    mol.perturb_atoms_coordinates(**pk)
             elif perturb_kwargs is not None:
                 ValueError('The perturb_kwargs should be a dict or list of dict')
 
             # Running the gaussian16
             for config_idx in range(mol.configure_number):
                 mol.configure_select(config_idx)
 
@@ -370,51 +445,30 @@
                 )
 
     @property
     def is_generator(self):
         """ To judge weather the object is a Molecule generator """
         return isinstance(self.mols, Generator)
 
-    def merge_conformers(self):
-        """
-        Get the sum of conformers for all molecule in the mol bundle "self.mols"
-        This method can only be successfully executed
-        when all molecules in the molecular bundle can be added to each other
-        Returns:
-            a Molecule object with all of conformers in the self.mols
-        """
-        atomic_numbers = self.atomic_numbers
-
-        if isinstance(atomic_numbers, tuple):
-            return sum(self.mols[1:], start=self.mols[0])
-        elif isinstance(atomic_numbers, dict):
-            mol_array = np.array(self.mols)
-            return MolBundle([mol_array[i].sum() for ans, i in self.atomic_numbers.items()])
-
-    def merge_atoms_same_mols(self):
-        """ Merge Molecules with same atoms to a MixSameAtomMol """
-        bundle = self.to_mix_mols()
-        atom_num = bundle.atom_num
-
-        if isinstance(atom_num, tuple):
-            return sum(bundle.mols[1:], start=bundle.mols[0])
-        elif isinstance(atom_num, dict):
-            mol_array = np.array(bundle.mols)
-            return MolBundle([mol_array[i].sum() for ans, i in atom_num.items()])
-
     @property
     def mols(self):
         return self._data.get('mols', [])
 
     @mols.setter
     def mols(self, mols):
         self._data['mols'] = mols
 
-    def to_dpmd_sys(self, sys_root):
-        """"""
+    @staticmethod
+    def registered_bundle_names():
+        """ Return all registered bundle names """
+        return list(_bundle_classes.keys())
+
+    def to(self, bundle_name: str):
+        """ Convert this bundle to other bundle type """
+        return _bundle_classes[bundle_name](self.mols)
 
     def to_list(self) -> List[ci.Molecule]:
         """ Convert the molecule container (self.mol) to list """
         if isinstance(self.mols, Generator):
             self.mols = list(self)
 
         return self.mols
@@ -463,7 +517,43 @@
                         uni_mols.append(mol)
 
                 new_mols.extend(uni_mols)
 
             clone.mols = new_mols
 
             return clone
+
+
+@register_bundles
+class DeepModelBundle(MolBundle):
+    """ Specific MolBundle to carry out the tasks in DeepModeling packages """
+
+    def merge_conformers(self):
+        """
+        Get the sum of conformers for all molecule in the mol bundle "self.mols"
+        This method can only be successfully executed
+        when all molecules in the molecular bundle can be added to each other
+        Returns:
+            a Molecule object with all conformers in the self.mols
+        """
+        atomic_numbers = self.atomic_numbers
+
+        if isinstance(atomic_numbers, tuple):
+            return sum(self.mols[1:], start=self.mols[0])
+        elif isinstance(atomic_numbers, dict):
+            mol_array = np.array(self.mols)
+            return self.__class__([mol_array[i].sum() for ans, i in self.atomic_numbers.items()])
+
+    def merge_atoms_same_mols(self):
+        """ Merge Molecules with same atoms to a MixSameAtomMol """
+        bundle = self.to_mix_mols()
+        atom_num = bundle.atom_num
+
+        if isinstance(atom_num, tuple):
+            return sum(bundle.mols[1:], start=bundle.mols[0])
+        elif isinstance(atom_num, dict):
+            mol_array = np.array(bundle.mols)
+            return self.__class__([mol_array[i].sum() for ans, i in atom_num.items()])
+
+    def to_dpmd_sys(self, sys_root):
+        """"""
+
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/cheminfo.py` & `hotpot-zzy-0.3.0.6/hotpot/cheminfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,55 +9,61 @@
 import copy
 import json
 import os
 import re
 from abc import ABC, abstractmethod
 from io import IOBase
 from os import PathLike
-from os.path import join as ptj
+from os.path import join as opj
 from pathlib import Path
 from typing import *
 from itertools import product
 
 import numpy as np
 from openbabel import openbabel as ob, pybel as pb
 from rdkit import Chem
+from rdkit.Chem import Draw
 
 from hotpot import data_root
 from hotpot.tanks import lmp
-from hotpot.tanks.quantum import Gaussian
-from hotpot.utils.load_chem_lib import library as _lib  # The chemical library
-
+from hotpot.tanks.quantum import Gaussian, GaussianRunError
+from hotpot.utils.library import library as _lib  # The chemical library
 
 # Define Exceptions
 class OperateOBMolFail(BaseException):
     """ Raise for any fail that trys to operate the OBMol """
 
 
 class AddAtomFail(OperateOBMolFail):
     """ Raise when add an atom into Molecule fail """
 
 
 class AddBondFail(OperateOBMolFail):
     """ Raise when add a bond into Molecule fail """
 
 
-periodic_table = json.load(open(ptj(data_root, 'periodic_table.json'), encoding='utf-8'))
-_symbols: List[str] = ['unknown'] + list(periodic_table.keys())
-_max_valences = {n: v['max_valence'] for n, v in periodic_table.items()}
-_max_total_bond_order = {n: v['max_total_bond_order'] for n, v in periodic_table.items()}
+# periodic_table = json.load(open(opj(data_root, 'periodic_table.json'), encoding='utf-8'))
+periodic_table = _lib.get('PeriodicTable')  # hotpot.utils.library.PeriodicTabel
 
 _stable_charges = {
-    "H": 1, "He": 0,
-    "Li": 1, "Be": 2, "B": 3, "C": 4, "N": -3, "O": -2, "F": -1, "Ne": 0,
-    "Na": 1, "Mg": 2, "Al": 3, "Si": 4, "P": -3, "S": -2, "Cl": -1, "Ar": 0,
-    "K": 1, "Ca": 2, "Sc": 3, "Ti": 4, "V": 5, "Cr": 4, "Mn": 3, "Fe": 2, "Co": 2, "Ni": 2, "Cu": 1, "Zn": 2, "Ga": 3, "Ge": 4, "As": -3, "Se": -2, "Br": -1, "Kr": 0,
-    "Rb": 1, "Sr": 2, "Y": 3, "Zr": 4, "Nb": 5, "Mo": 6, "Tc": 7, "Ru": 4, "Rh": 3, "Pd": 2, "Ag": 1, "Cd": 2, "In": 3, "Sn": 2, "Sb": -3, "Te": -2, "I": -1, "Xe": 0,
-    "Cs": 1, "Ba": 2, "La": 3, "Ce": 4, "Pr": 3, "Nd": 3, "Pm": 3, "Sm": 3, "Eu": 2, "Gd": 3, "Tb": 3, "Dy": 3, "Ho": 3, "Er": 3, "Tm": 3, "Yb": 3, "Lu": 3, "Hf": 4, "Ta": 5, "W": 6, "Re": 7, "Os": 4, "Ir": 3, "Pt": 2, "Au": 1, "Hg": 2, "Tl": 3, "Pb": 2, "Bi": 3, "Po": -2, "At": -1, "Rn": 0,
-    "Fr": 1, "Ra": 2, "Ac": 3, "Th": 4, "Pa": 5, "U": 6, "Np": 6, "Pu": 6, "Am": 6, "Cm": 6, "Bk": 6, "Cf": 6, "Es": 6, "Fm": 6, "Md": 6, "No": 6, "Lr": 3, "Rf": 4, "Db": 5, "Sg": 6, "Bh": 7, "Hs": 8, "Mt": 8, "Ds": 8, "Rg": 8, "Cn": 8, "Nh": 8, "Fl": 8, "Mc": 8, "Lv": 8, "Ts": 8, "Og": 8
+    "H": 1,  "He": 0,
+    "Li": 1, "Be": 2, "B": 3,  "C": 4,  "N": -3,  "O": -2,  "F": -1,  "Ne": 0,
+    "Na": 1, "Mg": 2, "Al": 3, "Si": 4, "P": -3,  "S": -2,  "Cl": -1, "Ar": 0,
+    "K": 1,  "Ca": 2, "Ga": 3, "Ge": 4, "As": -3, "Se": -2, "Br": -1, "Kr": 0,
+    "Rb": 1, "Sr": 2, "In": 3, "Sn": 2, "Sb": -3, "Te": -2, "I": -1,  "Xe": 0,
+    "Cs": 1, "Ba": 2, "Tl": 3, "Pb": 2, "Bi": 3,  "Po": -2, "At": -1, "Rn": 0,
+    "Fr": 1, "Ra": 2, "Nh": 8, "Fl": 8, "Mc": 8,  "Lv": 8,  "Ts": 8,  "Og": 8,
+
+    "Sc": 3, "Ti": 4, "V": 5,  "Cr": 3, "Mn": 2,  "Fe": 3,  "Co": 3,  "Ni": 2, "Cu": 2, "Zn": 2,
+    "Y": 3,  "Zr": 4, "Nb": 5, "Mo": 6, "Tc": 7,  "Ru": 4,  "Rh": 3,  "Pd": 2, "Ag": 1, "Cd": 2,
+    "Lu": 3, "Hf": 4, "Ta": 5, "W": 6,  "Re": 7,  "Os": 4,  "Ir": 3,  "Pt": 2, "Au": 1, "Hg": 2,
+    "Lr": 3, "Rf": 4, "Db": 5, "Sg": 6, "Bh": 7,  "Hs": 8,  "Mt": 8,  "Ds": 8, "Rg": 8, "Cn": 8,
+
+    "La": 3, "Ce": 4, "Pr": 3, "Nd": 3, "Pm": 3,  "Sm": 3,  "Eu": 2,  "Gd": 3, "Tb": 3, "Dy": 3, "Ho": 3, "Er": 3, "Tm": 3, "Yb": 3,
+    "Ac": 3, "Th": 4, "Pa": 5, "U": 6,  "Np": 6,  "Pu": 6,  "Am": 6,  "Cm": 6, "Bk": 6, "Cf": 6, "Es": 6, "Fm": 6, "Md": 6, "No": 6,
 }
 
 
 _bond_type = {
     'Unknown': 0,
     'Single': 1,
     'Double': 2,
@@ -118,15 +124,16 @@
 
             if setter:  # if the attribute is exist in the object.
                 assert isinstance(setter, Callable)
                 setter(value)
 
             else:
                 raise NameError(
-                    f'the {name} is cannot be set by Atom.set(), the legal attrs include: {self._attr_setters.keys()}'
+                    f'the {name} is cannot be set by {self.__class__.__name__}.set(), '
+                    f'the legal attrs include: {self._attr_setters.keys()}'
                 )
 
     @property
     @abstractmethod
     def _attr_setters(self) -> Dict[str, Callable]:
         raise NotImplemented
 
@@ -244,15 +251,15 @@
             return bd.MolBundle([self, other])
 
         # if isinstance(other, MixSameAtomMol):
         #     return self.to_mix_mol() + other
 
         # When other obj is a MolBundle
         if isinstance(other, bd.MolBundle):
-            return bd.MolBundle([self] + other.mols)
+            return other.__class__([self] + other.mols)
 
         else:
             raise TypeError('the Molecule only add with Molecule or MolBundle')
 
     def __iadd__(self, other):
         """
         Self add with other Molecule object with consist atoms list,
@@ -327,14 +334,15 @@
             'all_energy': self._set_all_energy,
             'charge': self._set_mol_charge,
             'all_atom_charges': self._set_all_atom_charges,
             'all_atom_spin_densities': self._set_all_atom_spin_densities,
             'spin': self._set_spin_multiplicity,
             'atoms': self._set_atoms,
             'mol_orbital_energies': self._set_mol_orbital_energies,
+            'coordinates': self._set_coordinates,
             'all_coordinates': self._set_all_coordinates,
             'all_forces': self._set_all_forces,
             'forces': self._set_forces,
             'crystal': self.create_crystal_by_matrix
         }
 
     def _create_ob_unit_cell(self):
@@ -346,50 +354,25 @@
         """ Remove temp label of all label """
         for a in self.atoms:
             a.remove_ob_data('temp_label')
 
     def _get_critical_params(self, name: str):
         critical_params = self._data.get('critical_params')
         if critical_params is None:
-            critical_params = json.load(open(ptj(data_root, 'thermo', 'critical.json'))).get(self.smiles)
+            critical_params = json.load(open(opj(data_root, 'thermo', 'critical.json'))).get(self.smiles)
             if critical_params:
                 self._data['critical_params'] = critical_params
                 return critical_params[name]
             else:
                 self._data['critical_params'] = False
                 return False
 
         else:
             return critical_params[name]
 
-    # TODO: Discard in last version
-    @property
-    def _ob_atom_indices(self):
-        """ Get the indices for all OBAtom """
-        indices = []
-
-        try:
-            num_ob_atoms = self.ob_mol.NumAtoms()
-        # If there is none of atoms in the OBMol, raise the TypeError.
-        except TypeError:
-            num_ob_atoms = 0
-
-        oba_id = 0  # the id for OBAtom in OBMol
-        while len(indices) < num_ob_atoms:
-            ob_atom = self.ob_mol.GetAtomById(oba_id)
-
-            # if get a OBAtom
-            if ob_atom:
-                assert oba_id == ob_atom.GetId()
-                indices.append(oba_id)
-
-            oba_id += 1
-
-        return indices
-
     def _pert_mol_generate(self, coordinates: Union[Sequence, np.ndarray]):
         """
         Generate new molecule obj according to new given coordinate
         Args:
             coordinates: New coordinates matrix
 
         Returns:
@@ -415,15 +398,15 @@
             oba.SetId(new_ob_id)
             new_atoms[new_ob_id] = atom
 
         self._data['atoms'] = new_atoms
 
         return new_atoms
 
-    def _load_bonds(self) -> Dict[Tuple[int], 'Bond']:
+    def _load_bonds(self) -> Dict[int, 'Bond']:
         """
         Construct bonds dict according to the OBBond in the OBMol,
         where the keys of the dict are the ob_id of OBBond and the values are the the constructed Bond objects
         the constructed dict would be place into the _data dict
         Returns:
             dict of bonds
         """
@@ -445,15 +428,14 @@
             density: float = 1.0, a: float = 25., b: float = 25., c: float = 25.,
             alpha: float = 90., beta: float = 90., gamma: float = 90., time_step: float = 0.0001,
             origin_temp: float = 298.15, melt_temp: float = 4000., highest_temp: float = 10000.,
             ff_args: Sequence = (), path_writefile: Optional[str] = None, path_dump_to: Optional[str] = None,
             dump_every: int = 100,
     ):
         """ to perform the melt-quench by call lmp.AmorphousMaker """
-
         am = lmp.AmorphousMaker(elements, force_field, density, a, b, c, alpha, beta, gamma)
         mol = am.melt_quench(
             *ff_args, mol=mol, path_writefile=path_writefile, path_dump_to=path_dump_to, origin_temp=origin_temp,
             melt_temp=melt_temp, highest_temp=highest_temp, time_step=time_step, dump_every=dump_every
         )
 
         return mol
@@ -481,14 +463,24 @@
 
         for i, items in enumerate(self.conformer_items):
             for item in items:
                 merge_attr(item)
 
         return self
 
+    def _preserve_atoms_data(self):
+        """
+        Preserve atoms data dict before destroy them.
+        Though the atoms are destroyed, their core ob_atom will be prevented,
+        The reserve data will match with the core ob_atoms
+        """
+        # Link the old atoms data dict with new atoms by temp labels
+        self._add_temp_atom_labels()
+        return {a.temp_label: a.data for a in self.atoms}
+
     @property
     def _protected_data(self):
         return 'ob_obj', 'atoms', 'bonds', 'angles'
 
     def _reorder_atom_ob_id(self):
         """ Reorder the ob id of atoms """
         new_atom_dict = {}
@@ -553,14 +545,22 @@
         elif len(all_coordinates.shape) != 3:
             raise ValueError(
                 f'the shape of given all_coordinates should with length 2 or 3, now is {len(all_coordinates.shape)}'
             )
 
         self._data['all_coordinates'] = all_coordinates
 
+    def _set_coordinates(self, coordinates: np.ndarray):
+        """ Assign the coordinates for all atoms in the molecule """
+        assert isinstance(coordinates, np.ndarray)
+        assert coordinates.shape == (self.atom_num, 3)
+
+        for a, c in zip(self.atoms, coordinates):
+            a.coordinates = c
+
     def _set_atom_charges(self, charge: Union[Sequence, np.ndarray]):
         """ Set partial charge for each atoms in the mol """
         if not isinstance(charge, (Sequence, np.ndarray)):
             raise TypeError(f'the charge should be a sequence or np.ndarray, got {type(charge)}')
 
         if isinstance(charge, np.ndarray):
             charge = charge.flatten()
@@ -651,33 +651,50 @@
     def _set_mol_orbital_energies(self, orbital_energies: list[np.ndarray]):
         self._data['mol_orbital_energies'] = orbital_energies[0]
 
     def _set_energy(self, energy: float):
         """ set the energy """
         self.ob_mol.SetEnergy(energy)
 
-    def _set_all_energy(self, all_energy: Union[float, np.ndarray], config_index: Optional[int] = None):
+    def _set_all_energy(self, all_energy: Union[float, np.ndarray]):
         """ set the energy for all configures """
         if isinstance(all_energy, float):
             self._data['all_energy'] = np.array([all_energy])
         else:
             all_energy = all_energy.flatten()
             self._data['all_energy'] = all_energy
 
     def _set_identifier(self, identifier):
         self.ob_mol.SetTitle(identifier)
 
     def _set_spin_multiplicity(self, spin):
         self.ob_mol.SetTotalSpinMultiplicity(spin)
 
+    @staticmethod
+    def _transfer_preserve_data_to_new_atoms(tgt_mol: 'Molecule', preserve_data: Dict, rm_temp_label: bool = False):
+        """
+        Transfer preserve data dict to new target Molecule object
+        Args:
+            tgt_mol: The target Molecule
+            preserve_data(dict): the old atoms data dict
+            rm_temp_label: whether to remove temp label after data have been transferred.
+        """
+        for atom in tgt_mol.atoms:
+            temp_label = atom.temp_label
+            if temp_label:
+                atom.update_attr_data(preserve_data[temp_label])
+
+                if rm_temp_label:
+                    atom.remove_ob_data('temp_label')
+
     @property
     def acentric_factor(self):
         return self._get_critical_params('acentric_factor')
 
-    def add_atom(self, atom: Union["Atom", str, int], **atom_attrs):
+    def add_atom(self, atom: Union["Atom", str, int], **atom_attrs) -> 'Atom':
         """
         Add a new atom out of the molecule into the molecule.
         Args:
             atom(Atom|str|int):
 
         atom_kwargs(kwargs for this added atom):
             atomic_number(int): set atomic number
@@ -689,15 +706,15 @@
 
         Returns:
             the copy of atom in the molecule
         """
         oba = ob.OBAtom()  # Initialize a new OBAtom
         data = None
         if isinstance(atom, str):
-            oba.SetAtomicNum(_symbols.index(atom))
+            oba.SetAtomicNum(ob.GetAtomicNum(atom))
         elif isinstance(atom, int):
             oba.SetAtomicNum(atom)
         elif isinstance(atom, Atom):
             oba.SetAtomicNum(atom.atomic_number)
             data = atom.data  # Copy the give atoms data
 
         # add OBAtom to the OBMol
@@ -741,43 +758,47 @@
         # the `Id` of `OBAtom` from 0; but the `Idx` of `OBAtom` from 1.
         # To meet the convention, the `Id` is selected to be the unique `index` to specify `Atom`.
         # However, when try to add a `OBBond` to link each two `OBAtoms`, the `Idx` is the only method
         # to specify the atoms, so our `index` in `Atom` are added 1 to match the 'Idx'
         success = self.ob_mol.AddBond(atoms[0].ob_idx, atoms[1].ob_idx, bond_type)
 
         if success:
-            new_bond_ob_id = [obb for obb in (ob.OBMolBondIter(self.ob_mol))][-1].GetId()
-            bond = self._load_bonds()[new_bond_ob_id]  # the new atoms should place in the terminal of the bond list
+            return self.bonds[-1]  # the new atoms should place in the terminal of the bond list
 
         elif atoms[0].ob_id not in self.atom_indices:
             raise KeyError("the start atom1 doesn't exist in molecule")
 
         elif atoms[1].ob_id not in self.atom_indices:
             raise KeyError("the end atom2 doesn't exist in molecule")
 
         else:
             raise RuntimeError('add bond not successful!')
 
-        # Return the bond have added into the molecule
-        return bond
-
-    def add_hydrogens(self, polar_only: bool = False, correct_for_ph: bool = False, ph: float = 1.0):
+    def add_hydrogens(
+            self,
+            polar_only: bool = False,
+            correct_for_ph: bool = False,
+            ph: float = 1.0,
+            balance_hydrogen: bool = True,
+    ):
         """
         add hydrogens for the molecule
         Args:
             ph: add hydrogen in which PH environment
             polar_only: Whether to add hydrogens only to polar atoms (i.e., not to C atoms)
             correct_for_ph: Correct for pH by applying the OpenBabel::OBPhModel transformations
+            balance_hydrogen: whether to balance the bond valance of heavy atom to their valence
         """
         self.ob_mol.AddHydrogens(polar_only, correct_for_ph, ph)
         self._load_atoms()
         self._load_bonds()
-        # TODO: Beta, test feature
-        for atom in self.atoms:
-            atom.remove_redundant_hydrogen()
+
+        if balance_hydrogen:
+            for atom in self.atoms:
+                atom.balance_hydrogen()
 
     def add_pseudo_atom(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
         """ Add pseudo atom into the molecule """
         list_pseudo_atom = self._data.setdefault('pseudo_atoms', [])
         pa = PseudoAtom(symbol, mass, coordinates, mol=self, molecule=self, **kwargs)
         list_pseudo_atom.append(pa)
 
@@ -840,14 +861,39 @@
         return list(atoms.values())
 
     @property
     def atoms_dict(self) -> Dict[int, 'Atom']:
         return self._load_atoms()
 
     @property
+    def all_atoms_with_unique_symbol(self):
+        return self.atoms_with_unique_symbol + \
+               self.pseudo_atoms_with_unique_symbol
+
+    @property
+    def atoms_with_unique_symbol(self):
+        uni_atoms, uni_symbol = [], set()
+        for a in self.pseudo_atoms:
+            if a.symbol not in uni_symbol:
+                uni_atoms.append(a)
+                uni_symbol.add(a.symbol)
+
+        return uni_atoms
+
+    @property
+    def pseudo_atoms_with_unique_symbol(self):
+        uni_patoms, uni_psymbol = [], set()
+        for a in self.atoms:
+            if a.symbol not in uni_psymbol:
+                uni_patoms.append(a)
+                uni_psymbol.add(a.symbol)
+
+        return uni_patoms
+
+    @property
     def all_atoms(self):
         return self.atoms + self.pseudo_atoms
 
     @property
     def atom_charges(self) -> np.ndarray:
         """ Return all atoms charges as a numpy array """
         return np.array([a.partial_charge for a in self.atoms])
@@ -875,22 +921,53 @@
     @property
     def all_atom_spin_densities(self):
         all_atom_spin_densities = self._data.get('all_atom_spin_densities')
         if all_atom_spin_densities is not None:
             return all_atom_spin_densities
         return self.atom_spin_densities.reshape((-1, self.atom_num))
 
+    def assign_atoms_formal_charge(self):
+        """ Assign the formal charges for all atoms in the molecule """
+        self.add_hydrogens(balance_hydrogen=False)
+
+        for atom in self.atoms:
+            if atom.is_polar_hydrogen:
+                atom.formal_charge = 1
+            elif atom.is_hydrogen or atom.is_carbon:
+                atom.formal_charge = 0
+            elif atom.is_metal:
+                atom.formal_charge = _stable_charges[atom.symbol]
+            elif atom.symbol == 'S':
+                if not [a for a in atom.neighbours if a.symbol == 'O']:
+                    atom.formal_charge = atom.covalent_valence - 2
+                else:
+                    atom.formal_charge = 0
+            elif atom.symbol == 'P':
+                if not [a for a in atom.neighbours if a.symbol == 'O']:
+                    atom.formal_charge = atom.covalent_valence - 2
+                else:
+                    atom.formal_charge = 0
+            elif [a for a in atom.neighbours if a.is_polar_hydrogen]:
+                atom.formal_charge = -(len([a for a in atom.neighbours if a.is_polar_hydrogen]))
+            else:
+                atom.formal_charge = atom.covalent_valence - atom.stable_valence
+
     @property
     def atomic_numbers(self):
         return tuple(a.atomic_number for a in self.atoms)
 
     @property
     def atomic_symbols(self):
         return tuple(a.symbol for a in self.atoms)
 
+    def balance_hydrogens(self):
+        """ Add or remove hydrogens for make or heave atom to achieve the stable valence """
+        for a in self.heavy_atoms():
+            a.balance_hydrogen()
+
     def bond(self, atom1: Union[int, str], atom2: Union[int, str], miss_raise: bool = False) -> 'Bond':
         """
         Return the Bond by given atom index labels in the bond ends
         if the bond is missing in the molecule, return None if given miss_raise is False else raise a KeyError
         Args:
             atom1(int|str): index or label of atom in one of the bond end
             atom2(int|str): index or label of atom in the other end of the bond
@@ -916,25 +993,50 @@
 
     @property
     def bonds(self):
         bonds = self._load_bonds()
         return list(bonds.values())
 
     @property
-    def bonds_dict(self) -> Dict[Tuple[int], 'Bond']:
+    def bonds_dict(self) -> Dict[int, 'Bond']:
         return self._load_bonds()
 
-    def build_bonds(self):
-        self.ob_mol.ConnectTheDots()
+    def build_2d(self):
+        """ build 2d conformer """
+        pmol = pb.Molecule(self.ob_mol)
+        pmol.make2D()
 
-    def build_conformer(self, force_field: str = 'UFF', steps: int = 50):
+    def build_3d(self, force_field: str = 'UFF', steps: int = 50):
         """ build 3D coordinates for the molecule """
+        # Preserve atoms data before building
+        preserve_data = self._preserve_atoms_data()
+
+        # Destroy atoms and bonds wrappers
+        self._data['atoms'] = {}
+        self._data['bonds'] = {}
+
+        # Build 3d conformer
         pymol = pb.Molecule(self.ob_mol)
         pymol.make3D(force_field, steps)
 
+        # Reload atoms and bonds
+        self._load_atoms()
+        self._load_bonds()
+
+        # Transfer preserve data to new
+        self._transfer_preserve_data_to_new_atoms(self, preserve_data)
+        # Delete temp label
+        self._delete_atom_temp_label()
+
+        # Remove redundant hydrogen or supply the lack hydrogens
+        self.balance_hydrogens()
+
+    def build_bonds(self):
+        self.ob_mol.ConnectTheDots()
+
     @property
     def center_of_masses(self):
         return (self.masses * self.coordinates.T).T.sum(axis=0) / self.masses.sum()
 
     @property
     def center_of_shape(self):
         return self.coordinates.mean(axis=0)
@@ -964,23 +1066,22 @@
         if pop:
             return all_coordinates
 
     @property
     def components(self):
         """ get all fragments don't link each by any bonds """
         # Add temp label for each atom first
-        self._add_temp_atom_labels()
-        parent_atom_dict = {a.temp_label: a.data for a in self.atoms}
+        preserve_data = self._preserve_atoms_data()
 
         components = [self.__class__(obc) for obc in self.ob_mol.Separate()]
 
         # Transfer the parent data attr to the children
         for c in components:
             for a in c.atoms:
-                a.update_attr_data(parent_atom_dict[a.temp_label])
+                a.update_attr_data(preserve_data[a.temp_label])
                 a.remove_ob_data('temp_label')
 
         # remove temp labels of all atoms
         self._delete_atom_temp_label()
 
         return components
 
@@ -1031,15 +1132,15 @@
         where the row index point to the atom index;
         the column index point to the (x, y, z)
         """
         return np.array([atom.coordinates for atom in self.atoms], dtype=np.float64)
 
     def copy(self) -> 'Molecule':
         """ Get a clone of this Molecule """
-        clone = Molecule(self.ob_copy())
+        clone = self.__class__(self.ob_copy())
         clone._load_atoms()
         clone._load_bonds()
 
         # Copy the Molecule's attr data to the clone one
         clone.update_attr_data(self.data)
         # Copy the Atoms' attr data to the clone ones
         for atom in clone.atoms:
@@ -1057,32 +1158,14 @@
         mol = self if inplace else self.copy()
         lattice_params = np.concatenate((self.xyz_diff, [90., 90., 90.]))
 
         mol.make_crystal(*lattice_params)
 
         return mol
 
-    def create_atom(self, symbol: str, **kwargs):
-        """
-        Discarded !!!
-        Create a new atom into the molecule
-        Args:
-            symbol: the atomic symbol
-            **kwargs: any attribute for the atom
-
-        Returns:
-            the created atom in the molecule
-        """
-        OBAtom: ob.OBAtom = self.ob_mol.NewAtom()
-        atomic_number = periodic_table[symbol]['number']
-        OBAtom.SetAtomicNum(atomic_number)
-        atom = Atom(OBAtom, mol=self, **kwargs)
-
-        return atom
-
     def create_crystal_by_vectors(
             self,
             va: Union[Sequence, np.ndarray],
             vb: Union[Sequence, np.ndarray],
             vc: Union[Sequence, np.ndarray]
     ):
         """ Create a new crystal with specified cell vectors for the Molecule """
@@ -1156,27 +1239,14 @@
 
         if cell_data:
             ob_unit_cell = ob.toUnitCell(cell_data)
             return Crystal(ob_unit_cell, molecule=self)
         else:
             return None
 
-    def determine_mol_charge(self):
-        """ Determining the molecular charge """
-        if not self.metals:  # if the molecule don't have any metal:
-            self.charge = self.read_from(self.dump('mol2'), 'mol2').charge
-        else:
-            clone = self.copy()
-            clone.remove_metals()
-
-            organic_charge = clone.read_from(clone.dump('mol2'), 'mol2').charge
-            metal_charge = sum(_stable_charges[m.symbol] for m in self.metals)
-
-            self.charge = organic_charge + metal_charge
-
     def dump(self, fmt: str, *args, **kwargs) -> Union[str, bytes, dict]:
         """"""
         dumper = Dumper(fmt=fmt, source=self, *args, **kwargs)
         return dumper()
 
     @property
     def elements(self) -> list[str]:
@@ -1249,15 +1319,15 @@
             route: Union[str, List[str]],
             path_log_file: Union[str, PathLike] = None,
             path_err_file: Union[str, PathLike] = None,
             inplace_attrs: bool = False,
             *args, **kwargs
     ) -> (Union[None, str], str):
         """
-        calculation by gaussion.
+        calculation by Gaussion.
         for running the method normally, MAKE SURE THE Gaussian16 HAVE BEEN INSTALLED AND ALL ENV VAR SET RITHT !!
         Args:
             g16root: the dir Gaussian16 software installed
             link0: the link0 command in gjf script
             route: the route command in gjf script
             path_log_file: Optional, the path to save the out.log file. If not given, the logfile won't be write
              to disk
@@ -1268,41 +1338,65 @@
             **kwargs:
 
         Returns:
             the standard output of g16 log file(string), the standard output of g16 err file(string)
         """
         # For 2d molecule, build its confomer by universal force field first
         if not self.has_3d:
-            self.build_conformer()
+            self.build_3d()
+
+        # TODO: Preserve for restart when encounter a Gaussian error.
+        chk_path = None
+        if isinstance(link0, List):
+            for l0 in link0:
+                if re.match(r'%chk=.+\.chk', l0):
+                    chk_path = l0[5:]
+                    break
 
         # Make the input gjf script
         script = self.dump('gjf', *args, link0=link0, route=route, **kwargs)
 
         # Run Gaussian16
         with Gaussian(g16root) as gaussian:
-            stdout, stderr = gaussian.run(script, args, **kwargs)
+            stdout, stderr = gaussian.run(script)
+
+            # If got an error message, save the error
+            if stderr:
+                # Save error file
+                if not path_err_file:
+                    path_err_file = Path(f'{self.formula}.err')
+                with open(path_err_file, 'w') as writer:
+                    writer.write(stderr)
+
+                # Save log file
+                if not path_log_file:
+                    path_log_file = Path(f'{self.formula}.log')
+                with open(path_log_file, 'w') as writer:
+                    writer.write(stdout)
+
+                raise GaussianRunError(
+                    f'Encourage error when Gaussian is running!\n'
+                    f'Check the Error file in {str(path_err_file.absolute())}\n'
+                    f'Check the output.log file in {str(path_log_file.absolute())}\n'
+                    f'Error massage from gaussian:\n{stderr}'
+                )
 
             # save the calculate result into the molecule data dict
             self._data['gaussian_output'] = stdout
             self._data['gaussian_parse_data'] = gaussian.data
 
             # Inplace the self attribute according to the result from gaussian
             if inplace_attrs:
                 self._set_attrs(**gaussian.molecule_setter_dict)
 
         # Save log file
         if path_log_file:
             with open(path_log_file, 'w') as writer:
                 writer.write(stdout)
 
-        # Save error file
-        if path_err_file:
-            with open(path_err_file, 'w') as writer:
-                writer.write(stderr)
-
         # return results and error info
         return stdout, stderr
 
     def gcmc(
             self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
             work_dir: Union[str, os.PathLike] = None, T: float = 298.15, P: float = 1.0, **kwargs
     ):
@@ -1319,14 +1413,45 @@
             T: the environmental temperature (default, 298.15 K)
             P: the relative pressure related to the saturation vapor in the environmental temperature.
         """
         from tanks.lmp.gcmc import LjGCMC
         gcmc = LjGCMC(self, force_field, *guest, work_dir=work_dir, T=T, P=P, **kwargs)
         return gcmc.run()
 
+    def gcmc_for_isotherm(
+            self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
+            work_dir: Union[str, os.PathLike] = None, T: float = 298.15,
+            Ps: Sequence[float] = (1.0,), **kwargs
+    ):
+        """
+        Run gcmc to determine the adsorption of guest,
+        Args:
+            self: the framework as the sorbent of guest molecule
+            guest(Molecule): the guest molecule to be adsorbed into the framework
+            force_field(str|PathLike): the path to force field file or the self-existent force file contained
+             in force field directory (in the case, a str should be given as a relative path from the root of
+             force field root to the specified self-existent force filed). By default, the force field is UFF
+             which in the relative path 'UFF/LJ.json' for the force field path.
+            work_dir: the user-specified dir to store the result of GCMC and log file.
+            T: the environmental temperature (default, 298.15 K)
+            Ps(Sequence[float]): A sequence of relative pressure related to the saturation vapor in the environmental temperature.
+        """
+        if isinstance(work_dir, str):
+            work_dir = Path(work_dir)
+
+        if not work_dir.exists():
+            work_dir.mkdir()
+
+        for P in Ps:
+            sub_work_dir = work_dir.joinpath('press_' + str(P))
+            if not sub_work_dir.exists():
+                sub_work_dir.mkdir()
+
+            self.gcmc(*guest, force_field=force_field, work_dir=sub_work_dir, T=T, P=P, **kwargs)
+
     def generate_metal_ligand_pair(
             self, metal_symbol: str,
             acceptor_atoms: Sequence = ('O',),
             opti_force_field: str = 'UFF',
             assign_metal_charge: bool = False
     ) -> Generator['Molecule', None, None]:
         """
@@ -1367,15 +1492,15 @@
                 else:  # If the pair has not 3d conformer, add the metal directly
                     added_metal = pair.add_atom(
                         metal_symbol,
                         formal_charge=_stable_charges[metal_symbol] if assign_metal_charge else 0
                     )
 
                 # add the coordinating bond between metal atom and acceptor atoms
-                pair.add_bond(added_metal, acc_atom, 1)
+                pair.add_bond(added_metal, acc_atom, 0)
 
                 # Add hydrogens
                 pair.add_hydrogens()
 
                 # localize optimization of M-L pair by classical force field, if the pair has 3d
                 if pair.has_3d:
                     pair.localed_optimize(opti_force_field)
@@ -1412,33 +1537,35 @@
                 assign_metal_charge
             )),
         )
 
     def graph_representation(self, *feature_names):
         return self.identifier, self.feature_matrix(*feature_names), self.link_matrix
 
+    def heavy_atoms(self):
+        """ Get the atoms except for hydrogens """
+        return [a for a in self.atoms if a.is_heavy]
+
     @property
     def has_3d(self):
         """ Whether atoms in the molecule have 3d coordinates """
         return self.ob_mol.Has3D()
 
     @property
-    def hydrogens(self):
-        return [a for a in self.atoms if a.is_hydrogen]
+    def has_hydrogen_added(self):
+        """ Have hydrogens been added to the molecule by call Molecule.add_hydrogen()? """
+        return self.ob_mol.HasHydrogensAdded()
 
     @property
-    def hydrogens_due_number(self):
-        """ the number of hydrogens when all hydrogens are completed """
-        clone = self.__class__.read_from(self.smiles, 'smi')
-        clone.add_hydrogens()
-        return clone.hydrogens_number
+    def has_unknown_bond(self):
+        return any(not b.type for b in self.bonds)
 
     @property
-    def hydrogens_number(self):
-        return len(self.hydrogens)
+    def hydrogens(self):
+        return [a for a in self.atoms if a.is_hydrogen]
 
     @property
     def identifier(self):
         return self.ob_mol.GetTitle()
 
     @identifier.setter
     def identifier(self, value):
@@ -1521,25 +1648,26 @@
         """ handle to operate the Lammps object """
         return self._data.get('lmp')
 
     def lmp_close(self):
         pop_lmp = self._data.pop('lmp')
         pop_lmp.close()
 
-    def lmp_setup(self, *args, **kwargs):
+    def lmp_setup(self, **kwargs):
         self._data['lmp'] = lmp.HpLammps(self, **kwargs)
 
     @property
     def link_matrix(self):
         return np.array([[b.ob_atom1_id, b.ob_atom2_id] for b in self.bonds]).T
 
     def localed_optimize(self, force_field: str = 'UFF', steps: int = 500):
         """ Locally optimize the coordinates. seeing openbabel.pybel package """
         pymol = pb.Molecule(self.ob_mol)
         pymol.localopt(force_field, steps)
+        self.balance_hydrogens()
 
     def make_crystal(self, a: float, b: float, c: float, alpha: float, beta: float, gamma: float) -> 'Crystal':
         """ Put this molecule into the specified crystal """
         ob_unit_cell = ob.OBUnitCell()
 
         self.ob_mol.CloneData(ob_unit_cell)
         self.crystal().ob_unit_cell.SetData(a, b, c, alpha, beta, gamma)
@@ -1612,30 +1740,28 @@
         element_counts = {}
         for atom in self.atoms:
             count = element_counts.get(atom.symbol, 0)
             count += 1
             element_counts[atom.symbol] = count
             atom.label = f'{atom.symbol}{count}'
 
-    def perturb_mol_lattice(
+    def perturb_atoms_coordinates(
             self,
             random_style='uniform',
             mol_distance=0.5,
-            lattice_fraction=0.05,
             freeze_dim: Sequence[int] = (),
             max_generate_num: int = 10,
             inplace: bool = False
     ) -> Generator["Molecule", None, None]:
         """
-        Perturb the coordinate of atom in the mol or the lattice parameters
+        Perturb the coordinate of atom in the molecule
         generate new mol
         Args:
             random_style: how to sample, 'uniform' or 'normal'
             mol_distance: the max distance of perturbation in 'uniform'; the square variance in 'normal'
-            lattice_fraction: the percentage of the lattice perturbation
             freeze_dim: tuple of int or str, 0 = x, 1 = y, 2 = z
             max_generate_num: the maximum of generated molecule
             inplace
 
         Returns:
             Generator of perturbed molecule
         """
@@ -1662,39 +1788,38 @@
 
                     perturb_matrix[:, dim] = 0.
 
                 new_coord = origin_coordinates + perturb_matrix
 
                 yield new_coord
 
-        def lattice_generator():
-            """ TODO: this function is prepare to generate the new lattice """
-
         if inplace:
             origin_all_coordinates = self._data.get('all_coordinates')
             new_all_coordinates = np.array([c for c in coordinates_generator()])
 
-            # TODO: test changes
             if origin_all_coordinates is not None:
                 self._data['all_coordinates'] = np.concatenate([origin_all_coordinates, new_all_coordinates])
             else:
                 self._data['all_coordinates'] = np.concatenate(
                     [np.reshape(origin_coordinates, (1,) + origin_coordinates.shape), new_all_coordinates]
                 )
 
         else:
             return (self._pert_mol_generate(c) for c in coordinates_generator())
 
+    def perturb_cell_params(self):
+        """ To perturb parameters, i.e., a, b, c, alpha, beta, gamma """
+
     @property
     def pseudo_atoms(self):
         return self._data.get('pseudo_atoms', [])
 
     def quick_build_atoms(self, atomic_numbers: np.ndarray):
         """
-        This method to quick build atoms according a array of atomic numbers.
+        This method to quick build atoms according an array of atomic numbers.
         The method bypass to calling more time-consumed method: add_atom().
         However, the method only assign the elements or atomic number for atoms,
         more fine attributes like coordinates, can't be specified.
         Args:
             atomic_numbers(np.ndarray): 1-D numpy array to add new atoms into the molecule
 
         Returns:
@@ -1731,53 +1856,49 @@
                 fmt = source.suffix.strip('.')
             else:
                 raise ValueError(f'the arguments should be specified for {type(source)} source')
 
         mol = Parser(fmt, source, *args, **kwargs)()  # initialize parser object and call self
 
         # Specify the mol identifier if it's None
-        if not mol.identifier:
+        if isinstance(mol, Molecule) and not mol.identifier:
             mol.identifier = str(source)
 
         return mol
 
     def register_critical_params(self, name: str, temperature: float, pressure: float, acentric: float):
         """ Register new critical parameters into the critical parameters sheet """
-        data = json.load(open(ptj(data_root, 'thermo', 'critical.json')))
+        data = json.load(open(opj(data_root, 'thermo', 'critical.json')))
         data[self.smiles] = {'name': name, 'temperature': temperature, 'pressure': pressure, 'acentric': acentric}
-        with open(ptj(data_root, 'thermo', 'critical.json'), 'w') as writer:
+        with open(opj(data_root, 'thermo', 'critical.json'), 'w') as writer:
             json.dump(data, writer, indent=True)
 
     def remove_atoms(self, *atoms: Union[int, str, 'Atom'], remove_hydrogens: bool = False) -> None:
         """
         Remove atom according to given atom index, label or the atoms self.
         Args:
             atoms(int|str|Atom): the index, label or self of Removed atom
             remove_hydrogens(bool): remove the hydrogens connecting in the atoms synchronously.
 
         Returns:
             None
         """
-        # to_remove_bonds = set()
         for atom in atoms:
 
             # Check and locate the atom
             if isinstance(atom, int):
                 atom = self.atoms_dict[atom]
             elif isinstance(atom, str):
                 atom = self.atom(atom)
             elif isinstance(atom, Atom):
                 if not (atom.molecule is self):
                     raise AttributeError('the given atom not in the molecule')
             else:
                 raise TypeError('the given atom should be int, str or Atom')
 
-            # Record the linking bonds with the atom
-            # to_remove_bonds.update(atom.bonds)
-
             # remove connecting hydrogens
             if remove_hydrogens:
                 for nh in atom.neighbours_hydrogen:
                     self.ob_mol.DeleteAtom(nh.ob_atom)
 
             # Removing the atom
             self.ob_mol.DeleteAtom(atom.ob_atom)
@@ -1835,14 +1956,27 @@
 
         return ml_pairs
 
     @property
     def rotatable_bonds_number(self):
         return self.ob_mol.NumRotors()
 
+    def save_2d_img(self, file_path: Union[str, os.PathLike], **kwargs):
+        """
+        Export 2d image to file
+        Args:
+            file_path:
+            **kwargs: other keywords arguments for 2d image make and save
+
+        Keyword Args:
+
+        """
+        img = self.to_2d_img(**kwargs)
+        img.save(file_path)
+
     def set(self, **kwargs):
         """ Set the attributes directly """
         self._set_attrs(**kwargs)
 
     def set_label(self, ob_id: int, label: str):
         self.atoms_dict[ob_id].label = label
 
@@ -1898,14 +2032,27 @@
     def thermo(self):
         return self._data.get('thermo')
 
     def thermo_close(self):
         _ = self._data.pop('thermo')
         del _
 
+    def to_2d_img(self, **kwargs):
+        """
+        Get a 2D image objects for the molecule
+        Keyword Args:
+            kekulize: whether to applying Kekulize style to aromatical rings
+
+        Returns:
+
+        """
+        clone = self.copy()
+        clone.build_2d()
+        return Draw.MolToImage(clone.to_rdmol(), **kwargs)
+
     def to_dpmd_sys(self, dpmd_sys_root: Union[str, os.PathLike], mode: Literal['std', 'att'] = 'std'):
         """
         convert to DeePMD-Kit System, there are two system mode, that `standard` (std) and `attention` (att)
             1) standard: https://docs.deepmodeling.com/projects/deepmd/en/master/data/system.html
             2) attention: https://docs.deepmodeling.com/projects/deepmd/en/master/model/train-se-atten.html#data-format
 
         Args:
@@ -1949,28 +2096,28 @@
             # Create an empty 'nopbc', when the system is not periodical
             elif name == 'nopbc' and value is True:
                 with open(dpmd_sys_root.joinpath('nopbc'), 'w') as writer:
                     writer.write('')
 
             # Save the numpy format data
             elif isinstance(value, np.ndarray):
-                np.save(set_root.joinpath(f'{name}.npy'), value)
+                np.save(str(set_root.joinpath(f'{name}.npy')), value)
 
     def to_mix_mol(self):
         return MixSameAtomMol(_data=self._data)
 
     def to_mol(self):
         return Molecule(_data=self.data)
 
     def to_rdmol(self):
         """ convert hotpot Molecule object to RdKit mol object """
         return Chem.MolFromMol2Block(self.dump('mol2'))
 
     @property
-    def unique_all_atoms(self):
+    def unique_all_atoms(self) -> List[Union['Atom', 'PseudoAtom']]:
         return self.unique_atoms + self.unique_pseudo_atoms
 
     @property
     def unique_atoms(self):
         uni = []
         for a in self.atoms:
             if a not in uni:
@@ -2043,35 +2190,28 @@
             return True
         return False
 
 
 class Atom(Wrapper, ABC):
     """ The Atom wrapper for OBAtom class in openbabel """
 
-    # TODO: to check the consistence of the method to access the OBAtom in OBMol
-    # TODO: for atom the correct method to access OBAtom from OBMol is by GetAtomById, not GetAtom !!!
-    # TODO: the GetAtomById get OBAtom start from 0
-    # TODO: the GetAtom get OBAtom start from 1
-    # TODO: the Id of OBAtom start from 0
-    # TODO: the Idx of OBAtom start from 1,
     def __init__(
             self,
             ob_atom: ob.OBAtom = None,
             **kwargs
     ):
         # Contain all data to reappear this Atom
         self._data: Dict[str, Any] = {
             'ob_obj': ob_atom if ob_atom else ob.OBAtom(),
         }
 
         self._set_attrs(**kwargs)
 
     def __eq__(self, other):
         if isinstance(other, Atom):
-            # return self.symbol == other.symbol
             return self.ob_atom == other.ob_atom
 
     def __hash__(self):
         return hash(f'Atom({self.atomic_number})')
 
     @property
     def ob_atom(self):
@@ -2086,14 +2226,25 @@
 
     def ob_atom_rewrap(self, ob_atom):
         self._data['ob_obj'] = ob_atom
 
     def __repr__(self):
         return f"Atom({self.label if self.label else self.symbol})"
 
+    def _assign_formal_charge(self):
+        """ assign formal charge for this atom, the formal charge equal its valence minus its covalent valence """
+        if self.is_polar_hydrogen:
+            self.formal_charge = 1
+        elif self.is_hydrogen or self.is_carbon:
+            self.formal_charge = 0
+        elif self.is_metal:
+            self.formal_charge = _stable_charges[self.symbol]
+        else:
+            self.formal_charge = -len([a for a in self.neighbours if a.is_polar_hydrogen])
+
     @property
     def _attr_setters(self) -> Dict[str, Callable]:
         return {
             '_mol': self._set_molecule,
             'mol': self._set_molecule,
             'molecule': self._set_molecule,
             'atomic_number': self._set_atomic_number,
@@ -2106,16 +2257,15 @@
             'spin_density': self._set_spin_density
         }
 
     def _set_atomic_number(self, atomic_number: int):
         self.ob_atom.SetAtomicNum(int(atomic_number))
 
     def _set_atomic_symbol(self, symbol):
-        atomic_number = periodic_table[symbol]['number']
-        self.ob_atom.SetAtomicNum(atomic_number)
+        self.ob_atom.SetAtomicNum(ob.GetAtomicNum(symbol))
 
     def _set_coordinate(self, coordinates):
         self.ob_atom.SetVector(*coordinates)
 
     def _set_force_vector(self, force_vector: Union[Sequence, np.ndarray]):
         if isinstance(force_vector, Sequence):
             if all(isinstance(f, float) for f in force_vector):
@@ -2158,21 +2308,31 @@
         return self.ob_atom.GetType()
 
     def add_atom(self, symbol: str, bond_type=1, **atom_attrs):
         """ add atom to link with this atom """
         new_atom = self.molecule.add_atom(symbol, **atom_attrs)
         self.molecule.add_bond(self, new_atom, bond_type)
 
+    def add_hydrogen(self):
+        """ add hydrogen to the atom """
+        self.add_atom('H')
+
     @property
     def atomic_number(self):
         return self.ob_atom.GetAtomicNum()
 
-    @property
-    def bond_valence(self) -> int:
-        return sum(b.type for b in self.bonds)
+    def balance_hydrogen(self):
+        """ Remove or add hydrogens link with this atom, if the bond valence is not equal to the atomic valence """
+        if self.is_heavy and not self.is_metal:  # Do not add or remove hydrogens to the metal, H or inert elements
+            while self.valence > self.stable_valence and self.neighbours_hydrogen:
+                self.molecule.remove_atoms(self.neighbours_hydrogen[0])
+
+            # add hydrogen, if the bond valence less than the atomic valence
+            while self.valence < self.stable_valence:
+                self.add_hydrogen()
 
     @property
     def bonds(self):
         """ Get all bonds link with the atoms """
         return [self.molecule.bonds_dict[obb.GetId()] for obb in ob.OBAtomBondIter(self.ob_atom)]
 
     @property
@@ -2198,25 +2358,28 @@
             data.pop('mol')
 
         # Copy the information contained in OBAtom
         new_attrs = {
             "atomic_number": self.atomic_number,
             "coordinates": self.coordinates,
             'partial_charge': self.partial_charge,
-            # 'label': self.label,
-            # 'ob_id': self.ob_id
         }
 
         new_attrs.update(**data)
 
         return Atom(**new_attrs)
 
+    @property
+    def covalent_valence(self):
+        """ the number of covalent electrons for this atoms """
+        return sum(b.type if b.is_covalent else 0 for b in self.bonds)
+
     def element_features(self, *feature_names) -> np.ndarray:
         """ Retrieve the feature vector """
-        atom_feature = periodic_table.get(self.symbol)
+        atom_feature = periodic_table[self.symbol]
 
         features = []
         for feature_name in feature_names:
             if feature_name == 'atomic_orbital':
                 features.extend(self._atomic_orbital_feature().values())
             elif feature_name == 'atomic_number':
                 features.append(self.atomic_number)
@@ -2289,14 +2452,18 @@
         return self.ob_atom.GetFormalCharge()
 
     @formal_charge.setter
     def formal_charge(self, value: float):
         self.ob_atom.SetFormalCharge(value)
 
     @property
+    def has_unknown_bond(self) -> bool:
+        return any(not b.type for b in self.bonds)
+
+    @property
     def hybridization(self):
         """ The hybridization of this atom:
         1 for sp, 2 for sp2, 3 for sp3, 4 for sq. planar, 5 for trig. bipy, 6 for octahedral """
         return self.ob_atom.GetHyb()
 
     @property
     def kwargs_attributes(self):
@@ -2311,22 +2478,31 @@
         return self.ob_atom.GetIdx()
 
     @property
     def is_aromatic(self):
         return self.ob_atom.IsAromatic()
 
     @property
+    def is_carbon(self):
+        return self.atomic_number == 6
+
+    @property
     def is_chiral(self):
         return self.ob_atom.IsChiral()
 
     @property
     def is_hydrogen(self):
         return self.ob_atom.GetAtomicNum() == 1
 
     @property
+    def is_heavy(self):
+        """ Whether the atom is heavy atom """
+        return not self.is_hydrogen
+
+    @property
     def is_polar_hydrogen(self) -> bool:
         """ Is this atom a hydrogen connected to a polar atom """
         return self.ob_atom.IsPolarHydrogen()
 
     @property
     def is_metal(self):
         return self.ob_atom.IsMetal()
@@ -2351,16 +2527,17 @@
         return self.ob_atom.GetTotalDegree()
 
     @property
     def mass(self):
         return self.ob_atom.GetAtomicMass()
 
     @property
-    def max_total_bond_order(self):
-        return _max_total_bond_order[self.symbol]
+    def max_bonds(self):
+        """ the max allowed bond order"""
+        return ob.GetMaxBonds(self.atomic_number)
 
     @property
     def molecule(self) -> Molecule:
         return self._data.get('mol')
 
     @molecule.setter
     def molecule(self, mol: 'Molecule'):
@@ -2368,14 +2545,18 @@
 
     @property
     def neighbours_hydrogen(self) -> List['Atom']:
         """ return all neigh hydrogen atoms """
         return [a for a in self.neighbours if a.is_hydrogen]
 
     @property
+    def electronegativity(self):
+        return ob.GetElectroNeg(self.atomic_number)
+
+    @property
     def neighbours(self) -> List['Atom']:
         """ Get all atoms bond with this atom in same molecule """
         if self.molecule:
             _ = self.molecule.atoms  # update the atoms dict
             return [self.molecule.atoms_dict[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
         else:
             return []
@@ -2391,31 +2572,32 @@
         for neigh_atom in self.neighbours:
             yield neigh_atom, neigh_atom.coordinates_array - self.coordinates_array
 
     @property
     def partial_charge(self):
         return self.ob_atom.GetPartialCharge()
 
-    def remove_redundant_hydrogen(self):
-        """ Remove hydrogens link with this atom, if the bond valence is more than the max allowed valence"""
-        if self.is_hydrogen:
-            return None
-
-        # remove redundant hydrogen
-        while self.bond_valence > abs(self.valence_max) and self.neighbours_hydrogen:
-            self.molecule.remove_atoms(self.neighbours_hydrogen[0])
-            self.formal_charge += self.formal_charge - 1
-
     @partial_charge.setter
     def partial_charge(self, value: float):
         # This is necessary to take effect to the assignment.
         # the reason is unknown
         self.ob_atom.GetPartialCharge()
         self._set_partial_charge(value)
 
+    def remove_hydrogen(self):
+        """ remove the first atom linking with the atoms """
+        hydrogens = self.neighbours_hydrogen
+        if hydrogens:
+            self.molecule.remove_atoms(hydrogens[0])
+
+    def remove_hydrogens(self):
+        """ Remove all hydrogens linking with the atom"""
+        hydrogens = self.neighbours_hydrogen
+        self.molecule.remove_atoms(*hydrogens)
+
     def replace_attr_data(self, data: Dict):
         """ Replace the core data dict directly """
         self._data = data
 
     def set(self, **kwargs):
         """
         Set atom attributes by kwargs
@@ -2435,29 +2617,48 @@
 
     @spin_density.setter
     def spin_density(self, spin_density: float):
         self._set_spin_density(spin_density)
 
     @property
     def stable_valence(self) -> int:
-        return _stable_charges.get(self.symbol, None)
+        if self.is_metal:
+            return 0
+        elif self.symbol == 'S':
+            if not [a for a in self.neighbours if a.symbol == 'O']:
+                return 2
+            elif self.covalent_valence <= 2:
+                return 2
+            elif self.covalent_valence <= 4:
+                return 4
+            else:
+                return 6
+        elif self.symbol == 'S':
+            if not [a for a in self.neighbours if a.symbol == 'O']:
+                return 3
+            elif self.covalent_valence == 0:
+                return 0
+            elif self.covalent_valence == 1:
+                return 1
+            elif self.covalent_valence <= 3:
+                return 3
+            else:
+                return 5
+        else:
+            return abs(_stable_charges[self.symbol])
 
     @property
     def symbol(self) -> str:
-        return _symbols[self.atomic_number]
+        return ob.GetSymbol(self.atomic_number)
 
     @property
     def valence(self) -> int:
-        """ The current number of explicit connections """
-        return self.ob_atom.GetTotalValence()
-
-    @property
-    def valence_max(self) -> int:
-        """ The implicit valence of this atom type (i.e. maximum number of connections expected) """
-        return _max_valences[self.symbol]
+        # if self.has_unknown_bond:
+        #     raise AttributeError('Cannot calculate the bond valence, because of the existence of unknown bonds')
+        return sum(b.type if b.type else 0 if b.is_covalent else 1 for b in self.bonds)
 
 
 class PseudoAtom(Wrapper, ABC):
     """ A data wrapper for pseudo atom """
 
     def __init__(self, symbol: str, mass: float, coordinates: Union[Sequence, np.ndarray], **kwargs):
         if isinstance(coordinates, Sequence):
@@ -2547,14 +2748,18 @@
         return self.ob_bond.GetBeginAtom().GetId(), self.ob_bond.GetEndAtom().GetId()
 
     @property
     def begin_end_atomic_number(self):
         return self.ob_bond.GetBeginAtom().GetAtomicNum(), self.ob_bond.GetEndAtom().GetAtomicNum()
 
     @property
+    def is_covalent(self) -> bool:
+        return not self.ob_atom1.IsMetal() and not self.ob_atom2.IsMetal()
+
+    @property
     def ideal_length(self):
         return self.ob_bond.GetEquibLength()
 
     @property
     def ob_id(self):
         return self.ob_bond.GetId()
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.0.6/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.0.6/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.0.6/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.0.6/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tanks/cc.py` & `hotpot-zzy-0.3.0.6/hotpot/tanks/cc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import numpy as np
 import pandas as pd
 from openbabel import openbabel as ob
 
 from hotpot import data_root
 from hotpot.cheminfo import Molecule, Atom
 from hotpot.bundle import MolBundle
+from hotpot.utils.manage_machine import machine
 
 # the atomic single point energies determined Gaussian with various methods and basis sets
 _atom_single_point: dict = json.load(open(Path(data_root).joinpath('atom_single_point.json')))
 
 
 class MetalLigandPair(Molecule):
     """ The Molecule to represent a metal-ligand pair """
@@ -65,21 +66,26 @@
         """
 
         def __init__(self, work_dir: Union[str, os.PathLike]):
             if isinstance(work_dir, str):
                 work_dir = Path(work_dir)
 
             self.work_dir = work_dir
+            self.chk_dir = work_dir.joinpath('chk')
             self.log_dir = work_dir.joinpath('log')
             self.err_dir = work_dir.joinpath('err')
             self.struct_dir = work_dir.joinpath('struct')
             self.energy_path = work_dir.joinpath('energy.csv')
             self.bde_path = work_dir.joinpath('bde.csv')
 
         @property
+        def ligand_chk_path(self):
+            return self.chk_dir.joinpath('ligand.chk')
+
+        @property
         def ligand_log_path(self):
             return self.log_dir.joinpath('ligand.log')
 
         @property
         def ligand_err_path(self):
             return self.err_dir.joinpath('ligand.err')
 
@@ -95,25 +101,32 @@
                 self.log_dir.mkdir()
             if not self.err_dir.exists():
                 self.err_dir.mkdir()
             if not self.struct_dir.exists():
                 self.struct_dir.mkdir()
 
         @property
+        def metal_chk_path(self):
+            return self.chk_dir.joinpath('metal.log')
+
+        @property
         def metal_log_path(self):
             return self.log_dir.joinpath('metal.log')
 
         @property
         def metal_err_path(self):
             return self.err_dir.joinpath('metal.err')
 
         @property
         def metal_struct_path(self):
             return self.struct_dir.joinpath('metal.mol2')
 
+        def pair_chk_path(self, idx: int):
+            return self.chk_dir.joinpath(f'pair_{idx}.chk')
+
         def pair_log_path(self, idx: int):
             return self.log_dir.joinpath(f'pair_{idx}.log')
 
         def pair_err_path(self, idx: int):
             return self.err_dir.joinpath(f'pair_{idx}.err')
 
         def pair_struct_path(self, idx: int):
@@ -146,15 +159,18 @@
 
         # Energy sheet, bond dissociation energy (BDE) sheet
         e_sheet, bde_sheet = [], []
 
         # optimize the configure of ligand and calculate their total energy after optimization
         self.ligand.gaussian(
             g16root,
-            link0=f'CPU=0-{os.cpu_count()-1}',
+            link0=[
+                f'CPU=0-15',
+                f'Mem=32GB'
+            ],
             route=f'opt {method}/{basis_set} ' + route,
             path_log_file=dirs_files.ligand_log_path,
             path_err_file=dirs_files.ligand_err_path,
             inplace_attrs=True
         )
 
         ligand_energy = self.ligand.energy  # Retrieve the energy after optimizing the conformer
@@ -165,15 +181,18 @@
 
         # Calculate the single point (sp) energy for metal
         try:
             metal_sp = _atom_single_point[self.metal.atoms[0].symbol][method][basis_set]
         except KeyError:
             self.metal.gaussian(
                 g16root,
-                link0=f'CPU=0-{os.cpu_count()-1}',
+                link0=[
+                    f'CPU=0-15',
+                    f'Mem=32GB'
+                ],
                 route=f'{method}/{basis_set} ' + route,
                 path_log_file=dirs_files.metal_log_path,
                 path_err_file=dirs_files.ligand_err_path,
                 inplace_attrs=True
             )
 
             ele_dict = _atom_single_point.setdefault(self.metal.atoms[0].symbol, {})
@@ -189,15 +208,18 @@
         # Save metal structure
         self.metal.writefile('mol2', dirs_files.metal_struct_path)
 
         # Optimizing the conformer of metal-ligands pairs and Retrieve the energies in the last stable conformer
         for i, pair in enumerate(self.pairs):
             pair.gaussian(
                 g16root,
-                link0=f'CPU=0-{os.cpu_count() - 1}',
+                link0=[
+                    f'CPU=0-15',
+                    f'Mem=32GB'
+                ],
                 route=f'opt {method}/{basis_set} ' + route,
                 path_log_file=dirs_files.pair_log_path(i),
                 path_err_file=dirs_files.pair_err_path(i),
                 inplace_attrs=True
             )
 
             # Append the pairs energy values to energy sheet
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/gcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self._extract_type_map()
 
     def _extract_type_map(self):
         def ext_tm(mol: 'ci.Molecule', which):
             atom_types_map = self._data.setdefault('atom_types_map', {})
             atom_types = self._data.setdefault('atom_types', {})
             list_atom_types = atom_types.setdefault(which, [])
-            for atom in mol.unique_all_atoms:
+            for atom in mol.all_atoms_with_unique_symbol:
                 atom_type = len(atom_types_map) + 1
                 atom_types_map[atom_type] = atom
                 list_atom_types.append(atom_type)
 
         ext_tm(self.frame, 'frame')
         for guest in self.guests:
             ext_tm(guest, 'guest')
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.0.6/hotpot/tanks/lmp/materials.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 @Date   : 2023/4/26
 @Time   : 1:50
 Notes:
     This package is to perform some specific tasks base on the LAMMPS
 """
 import os
 import os.path as osp
-import json
 from os.path import join as ptj
 from typing import *
 import math
 import random
 import numpy as np
+import openbabel.openbabel as ob
 import hotpot
 import hotpot.cheminfo as ci
 
 
 dir_force_field = osp.abspath(ptj(hotpot.data_root, 'force_field'))
 
 # Constants
@@ -59,19 +59,15 @@
         self.path_force_field = pff
         self.density = density
         self.cryst_params = (a, b, c, alpha, beta, gamma)
 
     @staticmethod
     def calc_cryst_density(cryst):
         """ Calculation the density for Crystal object """
-        mol: ci.Molecule = cryst.molecule
-        sum_mass = sum(ci.periodic_table[a.atom_type]['atomic_mass'] for a in mol.atoms)
-
-        # Density, g/cm^3
-        return (sum_mass * avogadro) / (cryst.volume * angstrom ** 3)
+        return (cryst.molecule.weight * avogadro) / (cryst.volume * angstrom ** 3)  # Density, g/cm^3
 
     @staticmethod
     def density2atom_numbers(ratio_elements: dict, density: float, cryst):
         """
         Calculate the round atom numbers in a crystal.
         Args:
             ratio_elements: Ratio of elements in the crystal
@@ -82,17 +78,16 @@
             int, the number of atoms
         """
         # Convert the dict of elements and possibility to numpy array
         elements = np.array(list(ratio_elements.keys()))
         possibility = np.array(list(ratio_elements.values()))
         possibility = possibility / possibility.sum()  # Normalize
 
-        average_mol_mass = sum(ci.periodic_table[e]['atomic_mass'] * p for e, p in zip(elements, possibility))
+        average_mol_mass = sum(ob.GetMass(ob.GetAtomicNum(e)) * p for e, p in zip(elements, possibility))
 
-        # TODO: Check ..., the formula may be wrong
         # Terms:   [Mole in Crystal(Total Mass in Crystal (gram)/Average Mole Mass)]/Avogadro Number
         # Units:      g/cm^3     angstrom^3  angstrom/cm             g/mol             _
         num_atom = ((density * (cryst.volume * angstrom ** 3)) / average_mol_mass) * avogadro
 
         v1, v2, v3 = cryst.vector  # crystal vectors
         dv1, dv2, dv3 = np.sqrt(sum(v1 ** 2)), np.sqrt(sum(v2 ** 2)), np.sqrt(sum(v3 ** 2))  # length of crystal vectors
         min_dv = min(dv1, dv2, dv3)  # the min length in these vectors
@@ -117,15 +112,15 @@
         fraction_coordinates = np.stack((pv1.flatten(), pv2.flatten(), pv3.flatten()))
 
         # the actual coordinates in the cartesian coordinates
         cartesian_coordinates = np.matmul(cryst.vector, fraction_coordinates).T
 
         num_atom = len(cartesian_coordinates)
         atomic_symbols = np.random.choice(elements, num_atom, p=possibility)
-        atomic_numbers = np.array([ci.periodic_table[symbol]["number"] for symbol in atomic_symbols])
+        atomic_numbers = np.array([ob.GetAtomicNum(symbol) for symbol in atomic_symbols])
 
         return atomic_numbers, cartesian_coordinates
 
     def load_atoms(self):
         mol = ci.Molecule()
         mol.make_crystal(*self.cryst_params)
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tanks/quantum.py` & `hotpot-zzy-0.3.0.6/hotpot/tanks/quantum.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         elif isinstance(g16root, os.PathLike):
             self.g16root = str(g16root)
         else:
             raise TypeError('the g16root should be str or os.PathLike type!')
 
         self.envs = self._set_environs()
         self._set_resource_limits(report_set_resource_error)
+        self.che_path = None
 
         self.data = None  # to receive the data from the cclib parser
         self.g16process = None  # to link to the g16 subprocess
 
     def __enter__(self):
         return self
 
@@ -154,41 +155,45 @@
 
         try:
             resource.setrlimit(resource.RLIMIT_NPROC, (resource.RLIM_INFINITY, resource.RLIM_INFINITY))
         except ValueError:
             if report_error:
                 print(RuntimeWarning('Unable to raise the RLIMIT_NPROC limit.'))
 
-    def run(self, script: str, *args, **kwargs):
+    def run(self, script: str):
         """Runs the Gaussian 16 process with the given script and additional arguments.
 
         This method sets up the required environment variables and resource limits for Gaussian 16 before
         running the process using `subprocess.Popen`. It takes an input script and any additional arguments
         to pass to `Popen`, and returns a tuple of the standard output and standard error of the process.
 
         Args:
             script (str): The input script for the Gaussian 16 process.
             *args: Additional arguments to pass to subprocess.Popen.
             **kwargs: Additional keyword arguments to pass to subprocess.Popen.
 
         Returns:
             Tuple[str, str]: A tuple of the standard output and standard error of the process.
         """
+        with open('input.gjf', 'w') as writer:
+            writer.write(script)
+
         # Run Gaussian using subprocess
         self.g16process = subprocess.Popen(
-            'g16', bufsize=-1, stdin=subprocess.PIPE,
+            ['g16', 'input.gjf', 'output.log'], bufsize=-1, stdin=subprocess.PIPE,
             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
             env=self.envs, universal_newlines=True
         )
-        stdout, stderr = self.g16process.communicate(script)
+        _, stderr = self.g16process.communicate()
+
+        with open('output.log') as file:
+            stdout = file.read()
 
-        # Raise error if got standard error message
         if stderr:
-            print(stderr)
-            raise GaussianRunError
+            return stdout, stderr
 
         self.parse_log(stdout)
 
         return stdout, stderr
 
     def parse_log(self, stdout: str):
         """ Parse the gaussian log file and save them into self """
```

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tmo.py` & `hotpot-zzy-0.3.0.6/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/tools.py` & `hotpot-zzy-0.3.0.6/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.0.6/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.0.6/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 hotpot/__init__.py
 hotpot/_io.py
 hotpot/bundle.py
 hotpot/cheminfo.py
 hotpot/tmo.py
 hotpot/tools.py
 hotpot/data/atom_single_point.json
+hotpot/data/deepmd_script.json
 hotpot/data/periodic_table.json
 hotpot/data/units.json
 hotpot/data/force_field/contents.json
 hotpot/data/force_field/UFF/LJ.json
 hotpot/data/force_field/aMaterials/SiC.tersoff
 hotpot/data/solvents/1,1,1-trichloroethane.mol2
 hotpot/data/solvents/1,1,1-trifluroethanol.mol2
@@ -86,22 +87,24 @@
 hotpot/data/solvents/tetralin.mol2
 hotpot/data/solvents/toluene.mol2
 hotpot/data/solvents/trichloroacetic_acid.mol2
 hotpot/data/solvents/trifluoroacetic_acid.mol2
 hotpot/data/solvents/water.mol2
 hotpot/tanks/__init__.py
 hotpot/tanks/cc.py
+hotpot/tanks/deepmd.py
 hotpot/tanks/features.py
 hotpot/tanks/quantum.py
 hotpot/tanks/lmp/__init__.py
 hotpot/tanks/lmp/base.py
 hotpot/tanks/lmp/gcmc.py
 hotpot/tanks/lmp/materials.py
 hotpot/utils/__init__.py
-hotpot/utils/load_chem_lib.py
+hotpot/utils/library.py
+hotpot/utils/manage_machine.py
 hotpot/utils/units_convert.py
 hotpot_zzy.egg-info/PKG-INFO
 hotpot_zzy.egg-info/SOURCES.txt
 hotpot_zzy.egg-info/dependency_links.txt
 hotpot_zzy.egg-info/requires.txt
 hotpot_zzy.egg-info/top_level.txt
 test/test_amorphous_maker.py
```

### Comparing `hotpot-zzy-0.3.0.3/test/test_amorphous_maker.py` & `hotpot-zzy-0.3.0.6/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.3/test/test_bundle.py` & `hotpot-zzy-0.3.0.6/test/test_bundle.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,36 +2,56 @@
 python v3.7.9
 @Project: hotpot
 @File   : test_bundle.py
 @Author : Zhiyuan Zhang
 @Date   : 2023/3/19
 @Time   : 21:25
 """
-from hotpot import MolBundle
-import json
-import hotpot.cheminfo as ci
+# from hotpot import MolBundle
+# import json
+# import hotpot.cheminfo as ci
+import hotpot as hp
+from pathlib import Path
 
+# if __name__ == '__main__':
+#     dir_log = '/home/zz1/proj/gauss/new/log'
+#     md = MolBundle.read_from('g16log', dir_log, match_pattern='*/*.log', num_proc=2)
+#     mmd = md.merge_conformers()
+#     mamd = mmd.merge_atoms_same_mols()
+#
+#     count = 0
+#     list_error = []
+#     for m in md:
+#         try:
+#             data = m.dump('dpmd_sys')
+#         except ValueError:
+#             count += 1
+#             list_error.append(m.identifier)
+#             print(m.configure_number, len(m.all_energy), len(m.all_forces), len(m.all_atom_spin_densities))
+#
+#     # list_error = json.load(open('/home/zz1/error_file.json'))
+#     # for p_e in list_error:
+#     #     m = ci.Molecule.read_from(p_e, 'g16log')
+#     #     if m:
+#     #         print(m.configure_number, len(m.all_energy), len(m.all_forces), len(m.all_atom_spin_densities))
+#
+#     dm = mmd[0].to_dpmd_sys('/home/zz1/proj/dpmd/std')
+#     dma = mamd[0].to_dpmd_sys('/home/zz1/proj/dpmd/att', 'att')
 
-if __name__ == '__main__':
-    dir_log = '/home/zz1/proj/gauss/new/log'
-    md = MolBundle.read_from('g16log', dir_log, match_pattern='*/*.log', num_proc=2)
-    mmd = md.merge_conformers()
-    mamd = mmd.merge_atoms_same_mols()
+#acarbon1 = hp.Molecule.read_from('/home/qyq/proj/aC_database/cif_48954/cif_10_test/mq_0.6_3000_9662_4132.cif')
+#acarbon2 = hp.Molecule.read_from('/home/qyq/proj/aC_database/cif_48954/cif_10_test/mq_1.0_4098_9724_3312.cif')
+frames_dir = Path('/home/qyq/proj/aC_database/cif_48954/cif_10_test')
+bundle = hp.MolBundle.read_from(
+        'cif', frames_dir, generate=True, num_proc=10
+    )
 
-    count = 0
-    list_error = []
-    for m in md:
-        try:
-            data = m.dump('dpmd_sys')
-        except ValueError:
-            count += 1
-            list_error.append(m.identifier)
-            print(m.configure_number, len(m.all_energy), len(m.all_forces), len(m.all_atom_spin_densities))
-
-    # list_error = json.load(open('/home/zz1/error_file.json'))
-    # for p_e in list_error:
-    #     m = ci.Molecule.read_from(p_e, 'g16log')
-    #     if m:
-    #         print(m.configure_number, len(m.all_energy), len(m.all_forces), len(m.all_atom_spin_densities))
-
-    dm = mmd[0].to_dpmd_sys('/home/zz1/proj/dpmd/std')
-    dma = mamd[0].to_dpmd_sys('/home/zz1/proj/dpmd/att', 'att')
+# print('bundle.mols')
+# for mol in bundle.mols:
+#     pass
+# print(mol)
+# print(mol.identifier)
+# print(type(mol))
+print('bundle')
+for mol in bundle:
+    print(mol)
+    print(mol.identifier)
+print(type(mol))
```

### Comparing `hotpot-zzy-0.3.0.3/test/test_chemif.py` & `hotpot-zzy-0.3.0.6/test/test_chemif.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
     return mol1, mol2, mol3
 
 
 def perturb_cif():
     path_cif = 'examples/struct/aCarbon.cif'
     mol = ci.Molecule.read_from(path_cif, 'cif')
-    gen = mol.perturb_mol_lattice(mol_distance=0.05, max_generate_num=2)
+    gen = mol.perturb_atoms_coordinates(mol_distance=0.05, max_generate_num=2)
 
     for i, gen_mol in enumerate(gen):
         gen_mol.writefile('cif', f'output/gen_cif/aCarbon_{i}.cif')
 
 
 def gen_pairs():
     from openbabel import openbabel as ob
     mol = ci.Molecule.read_from('c1ccc(C(=O)O)c(O)c1CCCC', 'smi')
     mol2 = ci.Molecule.read_from('c1ccc(C(=O)O)c(O)c1CCCC', 'smi')
-    mol.build_conformer('UFF')
-    mol2.build_conformer()
+    mol.build_3d('UFF')
+    mol2.build_3d()
     mol.normalize_labels()
     mol2.normalize_labels()
     g = mol.generate_metal_ligand_pair('Sr')
 
     # for a1, a2 in zip(mol.atoms, mol2.atoms):
     #     print(f'{a1.label}: {a1.partial_charge}---{a2.label}: {a2.partial_charge}')
 
@@ -66,20 +66,38 @@
     ps[1].writefile('mol2', f'/home/zz1/g01.mol2')
 
 
 # TODO: debug, the following code will encounter with error, abnormal exit with 139
 # TODO: check the coordinates and bond property
 def have_bug():
     mol = ci.Molecule.read_from('C=CC(=O)O', 'smi')
-    mol.build_conformer()
+    mol.build_3d()
     mol.normalize_labels()
 
     g = mol.generate_metal_ligand_pair('Sr')
 
     for p in g:
-        p.determine_mol_charge()
+        p.assign_atoms_formal_charge()
         c = p.copy()  # TODO: Guess that the bonds was not assigned correctly during the copy process
-        c.build_conformer()
+        c.build_3d()
+
+def test_valence_charge():
+    """ Test whether could the molecule to assign atoms formal charge and valence correctly """
+    mol = ci.Molecule.read_from('c1nc(CS(=O)(=O)O)c(OCCOP(O)(=O)OC)cc1', 'smi')
+
+    pairs = list(mol.generate_metal_ligand_pair('Cs'))
+
+    for i, pair in enumerate(pairs):
+
+        print(pair.dump('gjf', link0='sldf', route='hfka'))
+        print(pair.smiles, pair.charge)
 
 
 if __name__ == '__main__':
-    pass
+    # from hotpot.utils.load_chem_lib import library as lib
+    #
+    # periodic_table = lib.get('PeriodicTable')
+    #
+    # for element in periodic_table:
+    #     print(element)
+
+    test_valence_charge()
```

### Comparing `hotpot-zzy-0.3.0.3/test/test_lmp.py` & `hotpot-zzy-0.3.0.6/test/test_lmp.py`

 * *Files identical despite different names*

