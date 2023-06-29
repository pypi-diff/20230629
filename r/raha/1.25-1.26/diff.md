# Comparing `tmp/raha-1.25.tar.gz` & `tmp/raha-1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/raha-1.25.tar", last modified: Thu Nov 26 12:51:42 2020, max compression
+gzip compressed data, was "raha-1.26.tar", last modified: Thu Jun 29 11:16:58 2023, max compression
```

## Comparing `raha-1.25.tar` & `raha-1.26.tar`

### file list

```diff
@@ -1,214 +1,187 @@
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      119 2020-11-11 11:03:45.000000 raha-1.25/MANIFEST.in
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      428 2020-11-26 12:51:42.000000 raha-1.25/PKG-INFO
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    19684 2020-11-11 09:39:35.000000 raha-1.25/raha/baselines.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    31877 2020-04-15 11:07:36.000000 raha-1.25/raha/benchmark.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    31854 2020-11-24 12:42:49.000000 raha-1.25/raha/correction.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5544 2020-05-28 12:31:47.000000 raha-1.25/raha/dataset.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    24539 2020-11-24 12:14:46.000000 raha-1.25/raha/detection.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/datasets/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      278 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/all
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2769 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/invocation.md
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/datasets/synthetic/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      391 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/synthetic/countrydata.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     9172 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/synthetic/country_data
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      886 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/synthetic/fizzbuzz.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1505 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/synthetic/logins.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1142 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/synthetic/utils.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       67 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/datasets/urls.txt
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4508 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/cords.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2233 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/discrete.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2633 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/statistical.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1506 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/utils.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      140 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__pycache__/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3828 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__pycache__/cords.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2522 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__pycache__/discrete.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3168 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__pycache__/statistical.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2003 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__pycache__/utils.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      415 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/analyzers/__pycache__/__init__.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5658 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/cli.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1519 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/dboost-stdin.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/features/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      187 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/features/utils.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3335 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/features/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/features/__pycache__/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5722 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/features/__pycache__/__init__.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1679 2019-11-04 09:11:39.000000 raha-1.25/raha/tools/dBoost/dboost/imported_dboost.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/models/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4038 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/models/discrete.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4026 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/models/discretepart.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1926 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/models/gaussian.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3328 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/models/mixture.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      203 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/models/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/models/__pycache__/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4362 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/models/__pycache__/discrete.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4773 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/models/__pycache__/discretepart.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2767 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/models/__pycache__/gaussian.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4284 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/models/__pycache__/mixture.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      472 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/models/__pycache__/__init__.cpython-36.pyc
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/utils/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      235 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/autoconv.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      613 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/color.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      300 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/db.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3988 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/printing.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1544 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/read.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3042 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/tupleops.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      402 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/autoconv.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      955 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/color.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4206 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/printing.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1884 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/read.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     8301 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/tupleops.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      172 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/dBoost/dboost/utils/__pycache__/__init__.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1757 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/dboost/__pycache__/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5282 2019-11-18 10:12:04.000000 raha-1.25/raha/tools/dBoost/dboost/__pycache__/cli.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1409 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/dBoost/dboost/__pycache__/imported_dboost.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2174 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/dBoost/dboost/__pycache__/__init__.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1744 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/dboost-mimic2.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/graphics/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1047 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/3d-plots.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2727 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/csail-stats.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1197 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/gaussians-preview.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      907 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/histograms-preview.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      466 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/lof-plots.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1763 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/mixtures-preview.png.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6630 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/peakiness.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    11395 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/pipeline.pdf
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    97847 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/pipeline.svg
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2629 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/scalability.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      643 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/sensor-gaus-plots.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      638 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/sensor-mix-plots.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      695 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/sensor-plots.pdf.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1448 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/table-histograms.pdf.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/graphics/utils/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4800 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/utils/plots_helper.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    69079 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/utils/_multivariate.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2735 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/utils/_util.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1422 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/graphics/utils/__init__.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      145 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/group-list.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    35122 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/LICENSE
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/meetings/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1358 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-10-15.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1201 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-10-22.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      602 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-10-29.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      364 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-11-05.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1104 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-11-17.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3449 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-11-21.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1176 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-12-16.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      597 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2014-12-3.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      175 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2015-02-03.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      478 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/meetings/2015-04-08.md
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/paper/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      147 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/.dir-locals.el
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/paper/icde/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      406 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/implementation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1292 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/abstract.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      240 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/acknowledgments.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3903 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/author-response.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    33507 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/changelog.txt
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1297 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/conclusion.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6479 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/csail-directory-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4737 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6415 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/expansion.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2963 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/fizzbuzz-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       50 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/future-work.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    17394 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/IEEEabrv.bib
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    39651 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/IEEEexample.bib
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    19159 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/IEEEfull.bib
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    59215 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/IEEEtran.bst
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)   202657 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/IEEEtran.cls
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    62786 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/IEEEtranS.bst
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5749 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/intel-lab-data-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6158 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/introduction.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2512 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/logins-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1012 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/Makefile
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       50 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/mimic2-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     9599 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/model-creation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     7219 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/outlier-detection.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6294 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/overview.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    11867 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/paper.bib
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)  2645253 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/paper.pdf
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6078 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/paper.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1628 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/performance-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2258 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/plots.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4086 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/preamble.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6140 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/preprocessing.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      112 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/presidential-campaign-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2846 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/related-work.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3932 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/icde/statistical-analysis.tex
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/paper/vldb/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1292 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/abstract.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      240 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/acknowledgments.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1297 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/conclusion.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6477 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/csail-directory-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4542 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6072 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/expansion.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2961 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/fizzbuzz-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       50 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/future-work.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      509 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/implementation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5758 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/intel-lab-data-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     5079 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/introduction.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2512 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/logins-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1012 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/Makefile
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       50 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/mimic2-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     9435 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/model-creation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6938 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/outlier-detection.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6326 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/overview.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    11867 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/paper.bib
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2460 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/paper.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1626 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/performance-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2119 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/plots.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3930 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/preamble.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     6140 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/preprocessing.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      112 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/presidential-campaign-evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2846 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/related-work.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4251 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/statistical-analysis.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    47804 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/paper/vldb/vldb.cls
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/poster/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1359 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/analysis-and-modeling.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2674 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/beamerthemeCPC.sty
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      503 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/csail-example.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      483 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/evaluation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      408 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/future-work.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      494 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/header.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      468 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/Makefile
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1697 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/master.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      451 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/motivation.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      656 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/our-approach.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      165 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/pipeline-diagram.tex
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1287 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/poster/tango-colors.sty
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     1391 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/README.md
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/dBoost/scripts/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2080 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/scripts/csail-scalability.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      888 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/scripts/run_sensor_experiments.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3346 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/scripts/scalability_experiment.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     4372 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/TODO
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2046 2019-10-28 12:17:24.000000 raha-1.25/raha/tools/dBoost/twitter.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/KATARA/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3146 2019-11-04 09:09:33.000000 raha-1.25/raha/tools/KATARA/katara.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/KATARA/knowledge-base/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)  1209037 2019-10-28 12:17:33.000000 raha-1.25/raha/tools/KATARA/knowledge-base/zipHasCity.rel.txt
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       21 2020-04-15 08:48:24.000000 raha-1.25/raha/tools/KATARA/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha/tools/KATARA/__pycache__/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     2373 2019-11-13 11:12:12.000000 raha-1.25/raha/tools/KATARA/__pycache__/katara.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      182 2020-04-15 08:50:06.000000 raha-1.25/raha/tools/KATARA/__pycache__/__init__.cpython-36.pyc
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       73 2020-04-15 08:48:24.000000 raha-1.25/raha/tools/__init__.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)    19809 2020-11-17 10:28:55.000000 raha-1.25/raha/utilities.py
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      234 2020-07-03 13:29:28.000000 raha-1.25/raha/__init__.py
-drwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        0 2020-11-26 12:51:42.000000 raha-1.25/raha.egg-info/
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        1 2020-11-26 12:51:42.000000 raha-1.25/raha.egg-info/dependency_links.txt
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      428 2020-11-26 12:51:42.000000 raha-1.25/raha.egg-info/PKG-INFO
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       88 2020-11-26 12:51:42.000000 raha-1.25/raha.egg-info/requires.txt
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     8246 2020-11-26 12:51:42.000000 raha-1.25/raha.egg-info/SOURCES.txt
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)        5 2020-11-26 12:51:42.000000 raha-1.25/raha.egg-info/top_level.txt
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)     3934 2020-11-26 12:47:40.000000 raha-1.25/README.md
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)       79 2020-11-26 12:51:42.000000 raha-1.25/setup.cfg
--rwxrwxrwx   0 mohammad  (1000) mohammad  (1000)      690 2020-11-26 12:42:52.000000 raha-1.25/setup.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.242198 raha-1.26/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    11346 2023-06-29 10:56:50.000000 raha-1.26/LICENSE.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      119 2023-06-29 10:56:50.000000 raha-1.26/MANIFEST.in
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)      414 2023-06-29 11:16:58.242366 raha-1.26/PKG-INFO
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4344 2023-06-29 10:56:50.000000 raha-1.26/README.md
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.143504 raha-1.26/raha/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      234 2023-06-29 10:56:50.000000 raha-1.26/raha/__init__.py
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)    19684 2023-06-29 10:56:50.000000 raha-1.26/raha/baselines.py
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)    31877 2023-06-29 10:56:50.000000 raha-1.26/raha/benchmark.py
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)    35305 2023-06-29 10:56:50.000000 raha-1.26/raha/correction.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     5544 2023-06-29 10:56:50.000000 raha-1.26/raha/dataset.py
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)    24535 2023-06-29 10:56:50.000000 raha-1.26/raha/detection.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.147341 raha-1.26/raha/tools/
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.148390 raha-1.26/raha/tools/KATARA/
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)       21 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/KATARA/__init__.py
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)     3146 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/KATARA/katara.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.148890 raha-1.26/raha/tools/KATARA/knowledge-base/
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)  1209037 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/KATARA/knowledge-base/zipHasCity.rel.txt
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)       73 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/__init__.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.154108 raha-1.26/raha/tools/dBoost/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    35122 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/LICENSE
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1391 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/README.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4372 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/TODO
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.155542 raha-1.26/raha/tools/dBoost/datasets/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      278 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/all
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2769 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/invocation.md
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.158072 raha-1.26/raha/tools/dBoost/datasets/synthetic/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     9172 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/synthetic/country_data
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      391 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/synthetic/countrydata.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      886 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/synthetic/fizzbuzz.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1505 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/synthetic/logins.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1142 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/synthetic/utils.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)       67 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/datasets/urls.txt
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.160193 raha-1.26/raha/tools/dBoost/dboost/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1757 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/__init__.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.163412 raha-1.26/raha/tools/dBoost/dboost/analyzers/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      140 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/analyzers/__init__.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4508 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/analyzers/cords.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2233 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/analyzers/discrete.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2633 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/analyzers/statistical.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1506 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/analyzers/utils.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     5658 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/cli.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1519 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/dboost-stdin.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.164637 raha-1.26/raha/tools/dBoost/dboost/features/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3335 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/features/__init__.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      187 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/features/utils.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1679 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/imported_dboost.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.168088 raha-1.26/raha/tools/dBoost/dboost/models/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      203 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/models/__init__.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4038 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/models/discrete.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4026 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/models/discretepart.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1926 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/models/gaussian.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3328 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/models/mixture.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.172117 raha-1.26/raha/tools/dBoost/dboost/utils/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/__init__.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      235 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/autoconv.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      613 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/color.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      300 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/db.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3988 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/printing.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1544 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/read.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3042 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost/utils/tupleops.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1744 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/dboost-mimic2.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.180150 raha-1.26/raha/tools/dBoost/graphics/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1047 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/3d-plots.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2727 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/csail-stats.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1197 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/gaussians-preview.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      907 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/histograms-preview.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      466 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/lof-plots.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1763 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/mixtures-preview.png.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6630 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/peakiness.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    11395 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/pipeline.pdf
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    97847 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/pipeline.svg
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2629 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/scalability.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      643 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/sensor-gaus-plots.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      638 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/sensor-mix-plots.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      695 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/sensor-plots.pdf.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1448 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/table-histograms.pdf.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.182543 raha-1.26/raha/tools/dBoost/graphics/utils/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1422 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/utils/__init__.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    69079 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/utils/_multivariate.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2735 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/utils/_util.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4800 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/graphics/utils/plots_helper.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      145 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/group-list.md
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.187622 raha-1.26/raha/tools/dBoost/meetings/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1358 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-10-15.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1201 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-10-22.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      602 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-10-29.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      364 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-11-05.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1104 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-11-17.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3449 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-11-21.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1176 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-12-16.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      597 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2014-12-3.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      175 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2015-02-03.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      478 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/meetings/2015-04-08.md
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.188379 raha-1.26/raha/tools/dBoost/paper/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      147 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/.dir-locals.el
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.217721 raha-1.26/raha/tools/dBoost/paper/icde/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    17394 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/IEEEabrv.bib
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    39651 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/IEEEexample.bib
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    19159 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/IEEEfull.bib
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    59215 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/IEEEtran.bst
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)   202657 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/IEEEtran.cls
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    62786 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/IEEEtranS.bst
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1012 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/Makefile
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1292 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/abstract.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      240 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/acknowledgments.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3903 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/author-response.md
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    33507 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/changelog.txt
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1297 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/conclusion.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6479 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/csail-directory-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4737 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6415 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/expansion.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2963 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/fizzbuzz-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)       50 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/future-work.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      406 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/implementation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     5749 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/intel-lab-data-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6158 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/introduction.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2512 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/logins-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)       50 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/mimic2-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     9599 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/model-creation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     7219 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/outlier-detection.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6294 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/overview.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    11867 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/paper.bib
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)  2645253 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/paper.pdf
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6078 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/paper.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1628 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/performance-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2258 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/plots.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4086 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/preamble.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6140 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/preprocessing.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      112 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/presidential-campaign-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2846 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/related-work.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3932 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/icde/statistical-analysis.tex
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.235160 raha-1.26/raha/tools/dBoost/paper/vldb/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1012 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/Makefile
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1292 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/abstract.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      240 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/acknowledgments.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1297 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/conclusion.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6477 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/csail-directory-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4542 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6072 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/expansion.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2961 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/fizzbuzz-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)       50 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/future-work.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      509 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/implementation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     5758 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/intel-lab-data-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     5079 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/introduction.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2512 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/logins-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)       50 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/mimic2-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     9435 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/model-creation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6938 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/outlier-detection.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6326 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/overview.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    11867 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/paper.bib
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2460 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/paper.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1626 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/performance-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2119 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/plots.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3930 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/preamble.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     6140 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/preprocessing.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      112 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/presidential-campaign-evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2846 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/related-work.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     4251 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/statistical-analysis.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)    47804 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/paper/vldb/vldb.cls
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.240530 raha-1.26/raha/tools/dBoost/poster/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      468 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/Makefile
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1359 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/analysis-and-modeling.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2674 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/beamerthemeCPC.sty
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      503 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/csail-example.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      483 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/evaluation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      408 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/future-work.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      494 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/header.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1697 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/master.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      451 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/motivation.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      656 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/our-approach.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      165 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/pipeline-diagram.tex
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     1287 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/poster/tango-colors.sty
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.241789 raha-1.26/raha/tools/dBoost/scripts/
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2080 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/scripts/csail-scalability.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      888 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/scripts/run_sensor_experiments.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     3346 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/scripts/scalability_experiment.py
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)     2046 2023-06-29 10:56:50.000000 raha-1.26/raha/tools/dBoost/twitter.py
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)    19809 2023-06-29 10:56:50.000000 raha-1.26/raha/utilities.py
+drwxr-xr-x   0 fatemehahmadi   (501) staff       (20)        0 2023-06-29 11:16:58.146827 raha-1.26/raha.egg-info/
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)      414 2023-06-29 11:16:58.000000 raha-1.26/raha.egg-info/PKG-INFO
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)     6806 2023-06-29 11:16:58.000000 raha-1.26/raha.egg-info/SOURCES.txt
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)        1 2023-06-29 11:16:58.000000 raha-1.26/raha.egg-info/dependency_links.txt
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)       93 2023-06-29 11:16:58.000000 raha-1.26/raha.egg-info/requires.txt
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)        5 2023-06-29 11:16:58.000000 raha-1.26/raha.egg-info/top_level.txt
+-rw-r--r--   0 fatemehahmadi   (501) staff       (20)       79 2023-06-29 11:16:58.242971 raha-1.26/setup.cfg
+-rwxr-xr-x   0 fatemehahmadi   (501) staff       (20)      695 2023-06-29 11:16:09.000000 raha-1.26/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `raha-1.25/raha/baselines.py` & `raha-1.26/raha/baselines.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/benchmark.py` & `raha-1.26/raha/benchmark.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/correction.py` & `raha-1.26/raha/correction.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,40 @@
 import io
 import sys
 import math
 import json
 import pickle
 import difflib
 import unicodedata
-import multiprocessing
+import itertools
+import functools
+from multiprocessing import Pool
 
 import bs4
 import bz2
 import numpy
 import py7zr
 import mwparserfromhell
 import sklearn.svm
 import sklearn.ensemble
 import sklearn.naive_bayes
 import sklearn.linear_model
 
 import raha
 ########################################
 
+def worker_init_prediction(dataset, cls_model):
+    global d
+    d = dataset 
+    global classification_model
+    classification_model = cls_model
+
+def worker_init_feat_generation(dataset):
+    global d
+    d = dataset 
 
 ########################################
 class Correction:
     """
     The main class.
     """
 
@@ -52,14 +63,16 @@
         self.SAVE_RESULTS = True
         self.ONLINE_PHASE = False
         self.LABELING_BUDGET = 20
         self.MIN_CORRECTION_CANDIDATE_PROBABILITY = 0.0
         self.MIN_CORRECTION_OCCURRENCE = 2
         self.MAX_VALUE_LENGTH = 50
         self.REVISION_WINDOW_SIZE = 5
+        self.NUM_WORKERS = os.cpu_count()
+        self.CHUNK_SIZE = 100
 
     @staticmethod
     def _wikitext_segmenter(wikitext):
         """
         This method takes a Wikipedia page revision text in wikitext and segments it recursively.
         """
         def recursive_segmenter(node):
@@ -454,101 +467,190 @@
             else:
                 update_dictionary["vicinity"] = [cv if j != cj and d.labeled_cells[(d.sampled_tuple, cj)][0] == 1
                                                  else self.IGNORE_SIGN for cj, cv in enumerate(cleaned_sampled_tuple)]
             self._vicinity_based_models_updater(d.vicinity_models, update_dictionary)
         if self.VERBOSE:
             print("The error corrector models are updated with new labeled tuple {}.".format(d.sampled_tuple))
 
-    def _feature_generator_process(self, args):
+    def _feature_generator_process(self, cell_list, dataset=None):
         """
         This method generates features for each data column in a parallel process.
         """
-        d, cell = args
-        error_dictionary = {"column": cell[1], "old_value": d.dataframe.iloc[cell], "vicinity": list(d.dataframe.iloc[cell[0], :])}
-        value_corrections = self._value_based_corrector(d.value_models, error_dictionary)
-        vicinity_corrections = self._vicinity_based_corrector(d.vicinity_models, error_dictionary)
-        domain_corrections = self._domain_based_corrector(d.domain_models, error_dictionary)
-        models_corrections = value_corrections + vicinity_corrections + domain_corrections
-        corrections_features = {}
-        for mi, model in enumerate(models_corrections):
-            for correction in model:
-                if correction not in corrections_features:
-                    corrections_features[correction] = numpy.zeros(len(models_corrections))
-                corrections_features[correction][mi] = model[correction]
-        return corrections_features
+        pairs_counter = 0
+        pair_features = {}
+        ret_cells = []
+        if dataset == None:
+            global d
+        else:
+            d = dataset
+
+        for cell in filter(lambda cell: cell is not None, cell_list):
+            error_dictionary = {"column": cell[1], "old_value": d.dataframe.iloc[cell], "vicinity": list(d.dataframe.iloc[cell[0], :])}
+            value_corrections = self._value_based_corrector(d.value_models, error_dictionary)
+            vicinity_corrections = self._vicinity_based_corrector(d.vicinity_models, error_dictionary)
+            domain_corrections = self._domain_based_corrector(d.domain_models, error_dictionary)
+            models_corrections = value_corrections + vicinity_corrections + domain_corrections
+            corrections_features = {}
+            for mi, model in enumerate(models_corrections):
+                for correction in model:
+                    if correction not in corrections_features:
+                        corrections_features[correction] = numpy.zeros(len(models_corrections))
+                    corrections_features[correction][mi] = model[correction]
+
+            pair_features[cell] = {}
+            ret_cells.append(cell)
+            for correction in corrections_features:
+                pair_features[cell][correction] = corrections_features[correction]
+                pairs_counter += 1
+
+        return pairs_counter, pair_features, ret_cells
 
-    def generate_features(self, d):
+    def generate_features(self, d, cells):
         """
         This method generates a feature vector for each pair of a data error and a potential correction.
         """
-        d.pair_features = {}
-        pairs_counter = 0
-        process_args_list = [[d, cell] for cell in d.detected_cells]
-        pool = multiprocessing.Pool()
-        feature_generation_results = pool.map(self._feature_generator_process, process_args_list)
-        pool.close()
-        for ci, corrections_features in enumerate(feature_generation_results):
-            cell = process_args_list[ci][1]
-            d.pair_features[cell] = {}
-            for correction in corrections_features:
-                d.pair_features[cell][correction] = corrections_features[correction]
-                pairs_counter += 1
-        if self.VERBOSE:
-            print("{} pairs of (a data error, a potential correction) are featurized.".format(pairs_counter))
+        if len(cells) == 0:
+            yield {}, []
+        else:
+            pool = Pool(max(self.NUM_WORKERS-1, 1), initargs=(d,), initializer=worker_init_feat_generation)
+            pairs_counter = 0
+            process_args_generator = itertools.zip_longest(*[iter(cells)] * self.CHUNK_SIZE)
+
+            feature_generation_iterator = pool.imap(self._feature_generator_process, process_args_generator)
+
+            for pairs_counter_out, pair_features_out, cell_list in feature_generation_iterator:
+                pairs_counter += pairs_counter_out
+                yield pair_features_out, cell_list
+
+            pool.close()
+            if self.VERBOSE:
+                print("{} pairs of (a data error, a potential correction) are featurized.".format(pairs_counter))
+
+
+    def _prediction_process(self, cell_list, all_ones, all_zeros, dataset=None, cls_model=None):
+        """
+        This method generates the features for each data error cell and predicts a correction for each of them.
+        """
+        if dataset == None:
+            global d
+        else:
+            d = dataset
+
+        if cls_model == None:
+            global classification_model
+        else:
+            classification_model = cls_model
+        
+        correction_dict = {}
+
+        for cell in filter(lambda cell: cell is not None, cell_list):
+            _, pair_features, _ = self._feature_generator_process([cell], dataset=d)
+            
+            if all_ones:
+                predictions = numpy.ones(len(pair_features[cell]))
+            elif all_zeros:
+                continue
+            else:
+                predictions = classification_model.predict(list(pair_features[cell].values()))
+
+            dict_keys = list(pair_features[cell].keys())
+            for index, predicted_label in enumerate(predictions):
+                if predicted_label:
+                    correction_dict[cell] = dict_keys[index]
+
+        return correction_dict
+                
+
+    def predict_correction_multicore(self, classification_model, used_cells_test, d, all_zeros, all_ones):
+        """
+        This method predicts the correction for each data error in a parallel process.
+        """
+        pool = Pool(self.NUM_WORKERS,initargs=(d,classification_model), initializer=worker_init_prediction)
 
+        prediction_args_generator = itertools.zip_longest(*[iter(used_cells_test)] * self.CHUNK_SIZE)
+
+        correction_iterator = pool.imap(functools.partial(self._prediction_process, all_zeros=all_zeros, all_ones=all_ones), prediction_args_generator)
+
+        for i, correction_dict in enumerate(correction_iterator):
+            d.corrected_cells.update(correction_dict)
+            if self.VERBOSE:
+                print(f"{i*self.CHUNK_SIZE}/{len(used_cells_test)} predicted correction", end="\r")
+
+        pool.close()
+        
     def predict_corrections(self, d):
         """
-        This method predicts
+        This method predicts corrections for each data error.
         """
-        for j in d.column_errors:
+        if self.VERBOSE:
+            print("Predicting module...")
+
+        len_column_errors = len(d.column_errors)
+        for column_idx, j in enumerate(d.column_errors):
+            if self.VERBOSE:
+                print("------------------------------------------------------------------------")
+                print(f"{column_idx+1}/{len_column_errors} columns({d.dataframe.columns[j]})")
+            
+            used_cells_train = []
+            used_cells_test = []
+            for k, cell in enumerate(d.column_errors[j]):
+                if cell in d.detected_cells:
+                    if cell in d.labeled_cells and d.labeled_cells[cell][0] == 1:
+                        used_cells_train.append(cell)
+                    else:
+                        used_cells_test.append(cell)
+
             x_train = []
             y_train = []
-            x_test = []
-            test_cell_correction_list = []
-            for k, cell in enumerate(d.column_errors[j]):
-                if cell in d.pair_features:
-                    for correction in d.pair_features[cell]:
-                        if cell in d.labeled_cells and d.labeled_cells[cell][0] == 1:
-                            x_train.append(d.pair_features[cell][correction])
-                            y_train.append(int(correction == d.labeled_cells[cell][1]))
-                            d.corrected_cells[cell] = d.labeled_cells[cell][1]
-                        else:
-                            x_test.append(d.pair_features[cell][correction])
-                            test_cell_correction_list.append([cell, correction])
-            if self.CLASSIFICATION_MODEL == "ABC":
-                classification_model = sklearn.ensemble.AdaBoostClassifier(n_estimators=100)
-            if self.CLASSIFICATION_MODEL == "DTC":
-                classification_model = sklearn.tree.DecisionTreeClassifier(criterion="gini")
-            if self.CLASSIFICATION_MODEL == "GBC":
-                classification_model = sklearn.ensemble.GradientBoostingClassifier(n_estimators=100)
-            if self.CLASSIFICATION_MODEL == "GNB":
-                classification_model = sklearn.naive_bayes.GaussianNB()
-            if self.CLASSIFICATION_MODEL == "KNC":
-                classification_model = sklearn.neighbors.KNeighborsClassifier(n_neighbors=1)
-            if self.CLASSIFICATION_MODEL == "SGDC":
-                classification_model = sklearn.linear_model.SGDClassifier(loss="hinge", penalty="l2")
-            if self.CLASSIFICATION_MODEL == "SVC":
-                classification_model = sklearn.svm.SVC(kernel="sigmoid")
-            if x_train and x_test:
+            
+            if self.VERBOSE:
+                print(f"Generating train features({len(used_cells_train)}) ...")
+
+            len_used_cells_train = len(used_cells_train)
+            for k, (pair_features, cells) in enumerate(self.generate_features(d, used_cells_train)):
+                if self.VERBOSE:
+                    print(f"{(k)*self.CHUNK_SIZE}/{len_used_cells_train} creating train features",end="\r")
+                for cell in cells:
+                    for correction, value in pair_features[cell].items():
+                        x_train.append(value)
+                        y_train.append(int(correction == d.labeled_cells[cell][1]))
+                        d.corrected_cells[cell] = d.labeled_cells[cell][1]
+        
+            if x_train:
+                if self.VERBOSE:
+                    print("Training classifier ...") 
+                if self.CLASSIFICATION_MODEL == "ABC":
+                    classification_model = sklearn.ensemble.AdaBoostClassifier(n_estimators=100)
+                if self.CLASSIFICATION_MODEL == "DTC":
+                    classification_model = sklearn.tree.DecisionTreeClassifier(criterion="gini")
+                if self.CLASSIFICATION_MODEL == "GBC":
+                    classification_model = sklearn.ensemble.GradientBoostingClassifier(n_estimators=100)
+                if self.CLASSIFICATION_MODEL == "GNB":
+                    classification_model = sklearn.naive_bayes.GaussianNB()
+                if self.CLASSIFICATION_MODEL == "KNC":
+                    classification_model = sklearn.neighbors.KNeighborsClassifier(n_neighbors=1)
+                if self.CLASSIFICATION_MODEL == "SGDC":
+                    classification_model = sklearn.linear_model.SGDClassifier(loss="hinge", penalty="l2")
+                if self.CLASSIFICATION_MODEL == "SVC":
+                    classification_model = sklearn.svm.SVC(kernel="sigmoid")
+
+                all_zeros = False
+                all_ones = False
                 if sum(y_train) == 0:
-                    predicted_labels = numpy.zeros(len(x_test))
+                    all_zeros = True
                 elif sum(y_train) == len(y_train):
-                    predicted_labels = numpy.ones(len(x_test))
+                    all_ones = True
                 else:
                     classification_model.fit(x_train, y_train)
-                    predicted_labels = classification_model.predict(x_test)
-                # predicted_probabilities = classification_model.predict_proba(x_test)
-                # correction_confidence = {}
-                for index, predicted_label in enumerate(predicted_labels):
-                    cell, predicted_correction = test_cell_correction_list[index]
-                    # confidence = predicted_probabilities[index][1]
-                    if predicted_label:
-                        # if cell not in correction_confidence or confidence > correction_confidence[cell]:
-                        #     correction_confidence[cell] = confidence
-                        d.corrected_cells[cell] = predicted_correction
+
+                if self.VERBOSE:
+                    print("Predicting corrections...")
+
+                self.predict_correction_multicore(classification_model, used_cells_test, d, all_zeros, all_ones)
+
         if self.VERBOSE:
             print("{:.0f}% ({} / {}) of data errors are corrected.".format(100 * len(d.corrected_cells) / len(d.detected_cells),
                                                                            len(d.corrected_cells), len(d.detected_cells)))
 
     def store_results(self, d):
         """
         This method stores the results.
@@ -575,21 +677,22 @@
                   "------------------------------------------------------------------------")
         self.initialize_models(d)
         if self.VERBOSE:
             print("------------------------------------------------------------------------\n"
                   "--------------Iterative Tuple Sampling, Labeling, and Learning----------\n"
                   "------------------------------------------------------------------------")
         while len(d.labeled_tuples) < self.LABELING_BUDGET:
+            if self.VERBOSE:
+                print(f"Label round {len(d.labeled_tuples)+1}/{self.LABELING_BUDGET}")
             self.sample_tuple(d)
             if d.has_ground_truth:
                 self.label_with_ground_truth(d)
             # else:
             #   In this case, user should label the tuple interactively as shown in the Jupyter notebook.
             self.update_models(d)
-            self.generate_features(d)
             self.predict_corrections(d)
             if self.VERBOSE:
                 print("------------------------------------------------------------------------")
         if self.SAVE_RESULTS:
             if self.VERBOSE:
                 print("------------------------------------------------------------------------\n"
                       "---------------------------Storing the Results--------------------------\n"
```

### Comparing `raha-1.25/raha/dataset.py` & `raha-1.26/raha/dataset.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/detection.py` & `raha-1.26/raha/detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     if int(i) > 0:
                         outputted_cells[(int(i) - 1, int(j))] = ""
                 os.remove(algorithm_results_path)
             os.remove(dataset_path)
         elif algorithm == "PVD":
             attribute, ch = configuration
             j = d.dataframe.columns.get_loc(attribute)
-            for i, value in d.dataframe[attribute].iteritems():
+            for i, value in d.dataframe[attribute].items():
                 try:
                     if len(re.findall("[" + ch + "]", value, re.UNICODE)) > 0:
                         outputted_cells[(i, j)] = ""
                 except:
                     continue
         elif algorithm == "RVD":
             l_attribute, r_attribute = configuration
```

### Comparing `raha-1.25/raha/tools/dBoost/datasets/invocation.md` & `raha-1.26/raha/tools/dBoost/datasets/invocation.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/datasets/synthetic/country_data` & `raha-1.26/raha/tools/dBoost/datasets/synthetic/country_data`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/datasets/synthetic/fizzbuzz.py` & `raha-1.26/raha/tools/dBoost/datasets/synthetic/fizzbuzz.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/datasets/synthetic/logins.py` & `raha-1.26/raha/tools/dBoost/datasets/synthetic/logins.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/datasets/synthetic/utils.py` & `raha-1.26/raha/tools/dBoost/datasets/synthetic/utils.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/analyzers/cords.py` & `raha-1.26/raha/tools/dBoost/dboost/analyzers/cords.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/analyzers/discrete.py` & `raha-1.26/raha/tools/dBoost/dboost/analyzers/discrete.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/analyzers/statistical.py` & `raha-1.26/raha/tools/dBoost/dboost/analyzers/statistical.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/analyzers/utils.py` & `raha-1.26/raha/tools/dBoost/dboost/analyzers/utils.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/cli.py` & `raha-1.26/raha/tools/dBoost/dboost/cli.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/dboost-stdin.py` & `raha-1.26/raha/tools/dBoost/dboost/dboost-stdin.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/features/__init__.py` & `raha-1.26/raha/tools/dBoost/dboost/features/__init__.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/imported_dboost.py` & `raha-1.26/raha/tools/dBoost/dboost/imported_dboost.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/models/discrete.py` & `raha-1.26/raha/tools/dBoost/dboost/models/discrete.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/models/discretepart.py` & `raha-1.26/raha/tools/dBoost/dboost/models/discretepart.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/models/gaussian.py` & `raha-1.26/raha/tools/dBoost/dboost/models/gaussian.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/models/mixture.py` & `raha-1.26/raha/tools/dBoost/dboost/models/mixture.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/utils/color.py` & `raha-1.26/raha/tools/dBoost/dboost/utils/color.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/utils/printing.py` & `raha-1.26/raha/tools/dBoost/dboost/utils/printing.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/utils/read.py` & `raha-1.26/raha/tools/dBoost/dboost/utils/read.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/utils/tupleops.py` & `raha-1.26/raha/tools/dBoost/dboost/utils/tupleops.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost/__init__.py` & `raha-1.26/raha/tools/dBoost/dboost/__init__.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/dboost-mimic2.py` & `raha-1.26/raha/tools/dBoost/dboost-mimic2.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/3d-plots.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/3d-plots.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/csail-stats.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/csail-stats.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/gaussians-preview.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/gaussians-preview.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/histograms-preview.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/histograms-preview.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/mixtures-preview.png.py` & `raha-1.26/raha/tools/dBoost/graphics/mixtures-preview.png.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/peakiness.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/peakiness.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/pipeline.pdf` & `raha-1.26/raha/tools/dBoost/graphics/pipeline.pdf`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/pipeline.svg` & `raha-1.26/raha/tools/dBoost/graphics/pipeline.svg`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/scalability.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/scalability.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/sensor-gaus-plots.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/sensor-gaus-plots.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/sensor-mix-plots.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/sensor-mix-plots.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/sensor-plots.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/sensor-plots.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/table-histograms.pdf.py` & `raha-1.26/raha/tools/dBoost/graphics/table-histograms.pdf.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/utils/plots_helper.py` & `raha-1.26/raha/tools/dBoost/graphics/utils/plots_helper.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/utils/_multivariate.py` & `raha-1.26/raha/tools/dBoost/graphics/utils/_multivariate.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/utils/_util.py` & `raha-1.26/raha/tools/dBoost/graphics/utils/_util.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/graphics/utils/__init__.py` & `raha-1.26/raha/tools/dBoost/graphics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/LICENSE` & `raha-1.26/raha/tools/dBoost/LICENSE`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-10-15.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-10-15.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-10-22.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-10-22.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-10-29.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-10-29.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-11-17.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-11-17.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-11-21.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-11-21.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-12-16.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-12-16.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/meetings/2014-12-3.md` & `raha-1.26/raha/tools/dBoost/meetings/2014-12-3.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/abstract.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/abstract.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/author-response.md` & `raha-1.26/raha/tools/dBoost/paper/icde/author-response.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/changelog.txt` & `raha-1.26/raha/tools/dBoost/paper/icde/changelog.txt`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/conclusion.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/conclusion.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/csail-directory-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/csail-directory-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/expansion.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/expansion.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/fizzbuzz-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/fizzbuzz-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/IEEEabrv.bib` & `raha-1.26/raha/tools/dBoost/paper/icde/IEEEabrv.bib`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/IEEEexample.bib` & `raha-1.26/raha/tools/dBoost/paper/icde/IEEEexample.bib`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/IEEEfull.bib` & `raha-1.26/raha/tools/dBoost/paper/icde/IEEEfull.bib`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/IEEEtran.bst` & `raha-1.26/raha/tools/dBoost/paper/icde/IEEEtran.bst`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/IEEEtran.cls` & `raha-1.26/raha/tools/dBoost/paper/icde/IEEEtran.cls`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/IEEEtranS.bst` & `raha-1.26/raha/tools/dBoost/paper/icde/IEEEtranS.bst`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/intel-lab-data-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/intel-lab-data-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/introduction.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/introduction.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/logins-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/logins-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/Makefile` & `raha-1.26/raha/tools/dBoost/paper/icde/Makefile`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/model-creation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/model-creation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/outlier-detection.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/outlier-detection.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/overview.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/overview.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/paper.bib` & `raha-1.26/raha/tools/dBoost/paper/icde/paper.bib`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/paper.pdf` & `raha-1.26/raha/tools/dBoost/paper/icde/paper.pdf`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/paper.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/paper.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/performance-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/performance-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/plots.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/plots.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/preamble.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/preamble.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/preprocessing.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/preprocessing.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/related-work.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/related-work.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/icde/statistical-analysis.tex` & `raha-1.26/raha/tools/dBoost/paper/icde/statistical-analysis.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/abstract.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/abstract.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/conclusion.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/conclusion.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/csail-directory-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/csail-directory-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/expansion.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/expansion.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/fizzbuzz-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/fizzbuzz-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/intel-lab-data-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/intel-lab-data-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/introduction.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/introduction.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/logins-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/logins-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/Makefile` & `raha-1.26/raha/tools/dBoost/paper/vldb/Makefile`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/model-creation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/model-creation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/outlier-detection.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/outlier-detection.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/overview.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/overview.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/paper.bib` & `raha-1.26/raha/tools/dBoost/paper/vldb/paper.bib`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/paper.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/paper.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/performance-evaluation.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/performance-evaluation.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/plots.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/plots.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/preamble.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/preamble.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/preprocessing.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/preprocessing.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/related-work.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/related-work.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/statistical-analysis.tex` & `raha-1.26/raha/tools/dBoost/paper/vldb/statistical-analysis.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/paper/vldb/vldb.cls` & `raha-1.26/raha/tools/dBoost/paper/vldb/vldb.cls`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/poster/analysis-and-modeling.tex` & `raha-1.26/raha/tools/dBoost/poster/analysis-and-modeling.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/poster/beamerthemeCPC.sty` & `raha-1.26/raha/tools/dBoost/poster/beamerthemeCPC.sty`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/poster/master.tex` & `raha-1.26/raha/tools/dBoost/poster/master.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/poster/our-approach.tex` & `raha-1.26/raha/tools/dBoost/poster/our-approach.tex`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/poster/tango-colors.sty` & `raha-1.26/raha/tools/dBoost/poster/tango-colors.sty`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/README.md` & `raha-1.26/raha/tools/dBoost/README.md`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/scripts/csail-scalability.py` & `raha-1.26/raha/tools/dBoost/scripts/csail-scalability.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/scripts/run_sensor_experiments.py` & `raha-1.26/raha/tools/dBoost/scripts/run_sensor_experiments.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/scripts/scalability_experiment.py` & `raha-1.26/raha/tools/dBoost/scripts/scalability_experiment.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/TODO` & `raha-1.26/raha/tools/dBoost/TODO`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/dBoost/twitter.py` & `raha-1.26/raha/tools/dBoost/twitter.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/KATARA/katara.py` & `raha-1.26/raha/tools/KATARA/katara.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/tools/KATARA/knowledge-base/zipHasCity.rel.txt` & `raha-1.26/raha/tools/KATARA/knowledge-base/zipHasCity.rel.txt`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha/utilities.py` & `raha-1.26/raha/utilities.py`

 * *Files identical despite different names*

### Comparing `raha-1.25/raha.egg-info/SOURCES.txt` & `raha-1.26/raha.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 raha/__init__.py
 raha/baselines.py
 raha/benchmark.py
@@ -13,16 +14,14 @@
 raha.egg-info/SOURCES.txt
 raha.egg-info/dependency_links.txt
 raha.egg-info/requires.txt
 raha.egg-info/top_level.txt
 raha/tools/__init__.py
 raha/tools/KATARA/__init__.py
 raha/tools/KATARA/katara.py
-raha/tools/KATARA/__pycache__/__init__.cpython-36.pyc
-raha/tools/KATARA/__pycache__/katara.cpython-36.pyc
 raha/tools/KATARA/knowledge-base/zipHasCity.rel.txt
 raha/tools/dBoost/LICENSE
 raha/tools/dBoost/README.md
 raha/tools/dBoost/TODO
 raha/tools/dBoost/dboost-mimic2.py
 raha/tools/dBoost/group-list.md
 raha/tools/dBoost/twitter.py
@@ -34,53 +33,33 @@
 raha/tools/dBoost/datasets/synthetic/fizzbuzz.py
 raha/tools/dBoost/datasets/synthetic/logins.py
 raha/tools/dBoost/datasets/synthetic/utils.py
 raha/tools/dBoost/dboost/__init__.py
 raha/tools/dBoost/dboost/cli.py
 raha/tools/dBoost/dboost/dboost-stdin.py
 raha/tools/dBoost/dboost/imported_dboost.py
-raha/tools/dBoost/dboost/__pycache__/__init__.cpython-36.pyc
-raha/tools/dBoost/dboost/__pycache__/cli.cpython-36.pyc
-raha/tools/dBoost/dboost/__pycache__/imported_dboost.cpython-36.pyc
 raha/tools/dBoost/dboost/analyzers/__init__.py
 raha/tools/dBoost/dboost/analyzers/cords.py
 raha/tools/dBoost/dboost/analyzers/discrete.py
 raha/tools/dBoost/dboost/analyzers/statistical.py
 raha/tools/dBoost/dboost/analyzers/utils.py
-raha/tools/dBoost/dboost/analyzers/__pycache__/__init__.cpython-36.pyc
-raha/tools/dBoost/dboost/analyzers/__pycache__/cords.cpython-36.pyc
-raha/tools/dBoost/dboost/analyzers/__pycache__/discrete.cpython-36.pyc
-raha/tools/dBoost/dboost/analyzers/__pycache__/statistical.cpython-36.pyc
-raha/tools/dBoost/dboost/analyzers/__pycache__/utils.cpython-36.pyc
 raha/tools/dBoost/dboost/features/__init__.py
 raha/tools/dBoost/dboost/features/utils.py
-raha/tools/dBoost/dboost/features/__pycache__/__init__.cpython-36.pyc
 raha/tools/dBoost/dboost/models/__init__.py
 raha/tools/dBoost/dboost/models/discrete.py
 raha/tools/dBoost/dboost/models/discretepart.py
 raha/tools/dBoost/dboost/models/gaussian.py
 raha/tools/dBoost/dboost/models/mixture.py
-raha/tools/dBoost/dboost/models/__pycache__/__init__.cpython-36.pyc
-raha/tools/dBoost/dboost/models/__pycache__/discrete.cpython-36.pyc
-raha/tools/dBoost/dboost/models/__pycache__/discretepart.cpython-36.pyc
-raha/tools/dBoost/dboost/models/__pycache__/gaussian.cpython-36.pyc
-raha/tools/dBoost/dboost/models/__pycache__/mixture.cpython-36.pyc
 raha/tools/dBoost/dboost/utils/__init__.py
 raha/tools/dBoost/dboost/utils/autoconv.py
 raha/tools/dBoost/dboost/utils/color.py
 raha/tools/dBoost/dboost/utils/db.py
 raha/tools/dBoost/dboost/utils/printing.py
 raha/tools/dBoost/dboost/utils/read.py
 raha/tools/dBoost/dboost/utils/tupleops.py
-raha/tools/dBoost/dboost/utils/__pycache__/__init__.cpython-36.pyc
-raha/tools/dBoost/dboost/utils/__pycache__/autoconv.cpython-36.pyc
-raha/tools/dBoost/dboost/utils/__pycache__/color.cpython-36.pyc
-raha/tools/dBoost/dboost/utils/__pycache__/printing.cpython-36.pyc
-raha/tools/dBoost/dboost/utils/__pycache__/read.cpython-36.pyc
-raha/tools/dBoost/dboost/utils/__pycache__/tupleops.cpython-36.pyc
 raha/tools/dBoost/graphics/3d-plots.pdf.py
 raha/tools/dBoost/graphics/csail-stats.pdf.py
 raha/tools/dBoost/graphics/gaussians-preview.pdf.py
 raha/tools/dBoost/graphics/histograms-preview.pdf.py
 raha/tools/dBoost/graphics/lof-plots.pdf.py
 raha/tools/dBoost/graphics/mixtures-preview.png.py
 raha/tools/dBoost/graphics/peakiness.pdf.py
```

### Comparing `raha-1.25/README.md` & `raha-1.26/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,37 @@
 
 
 ## Installation
 To install Raha and Baran, you can run:
 ```console
 pip3 install raha
 ```
+
+To install Raha and Baran using the github repository:
+```console
+git clone git@github.com:BigDaMa/raha.git
+pip3 install -e raha
+```
+
 To uninstall them, you can run:
 ```console
 pip3 uninstall raha
 ```
 
 ## Usage
 Running Raha and Baran is simple!
    - **Benchmarking**: If you have a dirty dataset and its corresponding clean dataset and you want to benchmark Raha and Baran, please check the sample codes in `raha/benchmark.py`, `raha/detection.py`, and `raha/correction.py`.
    - **Interactive data cleaning with Raha and Baran**: If you have a dirty dataset and you want to interatively detect and correct data errors, please check our interactive Jupyter notebooks in the `raha` folder. The Jupyter notebooks provide graphical user interfaces.
    ![Data Annotation](pictures/ui.png)   
    ![Promising Strategies](pictures/ui_strategies.png)   
    ![Drill Down](pictures/ui_clusters.png)   
    ![Dashboard](pictures/ui_dashboard.png) 
+   
+Hint:
+The pre-trained model inside the repo is only a sample for using the notebooks. Refrain from relying on that for your experiments. If you need to use the pre-trained models for Baran, please download the Wikipedia revision histories and use Baran to train a model.
 
 ## References
 You can find more information about this project and the authors [here](https://dl.acm.org/doi/abs/10.1145/3299869.3324956) and [here](https://dl.acm.org/doi/abs/10.14778/3407790.3407801). You can also use the following bib entries to cite this project and the corresponding research papers.
 
 ### Citing Raha
 ```
 @inproceedings{mahdavi2019raha,
```

### Comparing `raha-1.25/setup.py` & `raha-1.26/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="raha",
-    version="1.25",
+    version="1.26",
     packages=find_packages(),
     url="https://github.com/bigdama/raha",
     license="Apache 2.0",
     author="Mohammad Mahdavi",
     author_email="moh.mahdavi.l@gmail.com",
     description="Raha and Baran: An End-to-End Data Cleaning System",
     keywords=["Data Cleaning", "Machine Learning", "Error Detection", "Error Correction", "Data Repairing"],
-    install_requires=["numpy", "pandas", "scipy", "sklearn", "matplotlib", 
+    install_requires=["numpy", "pandas", "scipy", "scikit-learn", "matplotlib", 
     "prettytable", "mwparserfromhell", "beautifulsoup4", "py7zr"],
     include_package_data=True,
-    download_url="https://github.com/BigDaMa/raha/archive/v1.25.tar.gz"
+    download_url="https://github.com/BigDaMa/raha/archive/v1.26.tar.gz"
 )
```

