# Comparing `tmp/ezcharts-0.4.0.tar.gz` & `tmp/ezcharts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcharts-0.4.0.tar", last modified: Thu Jun 15 21:28:25 2023, max compression
+gzip compressed data, was "ezcharts-0.5.0.tar", last modified: Wed Jun 28 15:01:42 2023, max compression
```

## Comparing `ezcharts-0.4.0.tar` & `ezcharts-0.5.0.tar`

### file list

```diff
@@ -1,205 +1,220 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.134972 ezcharts-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    15820 2023-06-15 21:25:19.000000 ezcharts-0.4.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-15 21:25:19.000000 ezcharts-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5779 2023-06-15 21:28:25.134972 ezcharts-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-06-15 21:25:19.000000 ezcharts-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.090969 ezcharts-0.4.0/ezcharts/
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.090969 ezcharts-0.4.0/ezcharts/components/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/ezchart.py
--rw-rw-rw-   0 root         (0) root         (0)     6366 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.094969 ezcharts-0.4.0/ezcharts/components/reports/
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/reports/comp.py
--rw-rw-rw-   0 root         (0) root         (0)     7295 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/reports/labs.py
--rw-rw-rw-   0 root         (0) root         (0)     7349 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/reports/ond.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/components/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.086968 ezcharts-0.4.0/ezcharts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.094969 ezcharts-0.4.0/ezcharts/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/images/LAB_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/images/OND_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    33283 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/images/OND_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/images/ONT_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)   894078 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/images/dots.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.086968 ezcharts-0.4.0/ezcharts/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.094969 ezcharts-0.4.0/ezcharts/data/reference/hg19/
--rw-rw-rw-   0 root         (0) root         (0)     6297 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/reference/hg19/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.094969 ezcharts-0.4.0/ezcharts/data/reference/hg38/
--rw-rw-rw-   0 root         (0) root         (0)    11449 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/reference/hg38/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.098969 ezcharts-0.4.0/ezcharts/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/scripts/epi2melabs.js
--rw-rw-rw-   0 root         (0) root         (0)   394601 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/scripts/metagenomics-sankey-util.js
--rw-rw-rw-   0 root         (0) root         (0)    22324 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/scripts/metagenomics-sankey.js
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/scripts/nextclade.html
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/scripts/ond.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.098969 ezcharts-0.4.0/ezcharts/data/styles/
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/styles/epi2melabs.scss
--rw-rw-rw-   0 root         (0) root         (0)     2585 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/styles/metagenomics-sankey.css
--rw-rw-rw-   0 root         (0) root         (0)   898896 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/styles/ond.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.098969 ezcharts-0.4.0/ezcharts/data/test/
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/fastcat.stats.gz
--rw-rw-rw-   0 root         (0) root         (0)    28549 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/hg38_cnv.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)     2420 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/hg38_some_bands.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)    16943 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/nextclade.json
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/params.json
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/plot-spec.json
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/sankey.json
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/test/versions.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.098969 ezcharts-0.4.0/ezcharts/data/themes/
--rw-rw-rw-   0 root         (0) root         (0)     5771 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/themes/epi2melabs.json
--rw-rw-rw-   0 root         (0) root         (0)     5764 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/themes/ond.json
--rw-rw-rw-   0 root         (0) root         (0)     5536 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/themes/walden.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.098969 ezcharts-0.4.0/ezcharts/data/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.086968 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.102970 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/js/
--rw-rw-rw-   0 root         (0) root         (0)    80599 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.106970 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/
--rw-rw-rw-   0 root         (0) root         (0)     5066 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
--rw-rw-rw-   0 root         (0) root         (0)     2055 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
--rw-rw-rw-   0 root         (0) root         (0)     1751 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
--rw-rw-rw-   0 root         (0) root         (0)     3195 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     6941 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1948 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
--rw-rw-rw-   0 root         (0) root         (0)     8093 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)    10554 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)     7762 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     4725 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
--rw-rw-rw-   0 root         (0) root         (0)     3944 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
--rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)     7371 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
--rw-rw-rw-   0 root         (0) root         (0)    17886 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
--rw-rw-rw-   0 root         (0) root         (0)    73610 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1253 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.110970 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
--rw-rw-rw-   0 root         (0) root         (0)     5868 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
--rw-rw-rw-   0 root         (0) root         (0)      478 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.110970 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.114971 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0 root         (0) root         (0)     4580 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
--rw-rw-rw-   0 root         (0) root         (0)     4164 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
--rw-rw-rw-   0 root         (0) root         (0)     4726 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
--rw-rw-rw-   0 root         (0) root         (0)     3380 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.114971 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.114971 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
--rw-rw-rw-   0 root         (0) root         (0)    10029 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
--rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/echarts.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.118971 ezcharts-0.4.0/ezcharts/data/vendor/simple-datatables/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css
--rw-rw-rw-   0 root         (0) root         (0)    38201 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js
--rw-rw-rw-   0 root         (0) root         (0)     9862 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.118971 ezcharts-0.4.0/ezcharts/layout/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.118971 ezcharts-0.4.0/ezcharts/layout/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/banner.py
--rw-rw-rw-   0 root         (0) root         (0)     2119 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/offcanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/section.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     7587 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/table.py
--rw-rw-rw-   0 root         (0) root         (0)     5636 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/snippets/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/layout/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.134972 ezcharts-0.4.0/ezcharts/plots/
--rw-rw-rw-   0 root         (0) root         (0)     9172 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/_base.py
--rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/axisgrid.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/categorical.py
--rw-rw-rw-   0 root         (0) root         (0)     5065 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)    12727 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/ideogram.py
--rw-rw-rw-   0 root         (0) root         (0)     2903 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/matrix.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/metagenomics_sankey.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/relational.py
--rwxrwxrwx   0 root         (0) root         (0)     3444 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/sunburst.py
--rw-rw-rw-   0 root         (0) root         (0)     7208 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/plots/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-15 21:25:19.000000 ezcharts-0.4.0/ezcharts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 21:28:25.090969 ezcharts-0.4.0/ezcharts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5779 2023-06-15 21:28:25.000000 ezcharts-0.4.0/ezcharts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8330 2023-06-15 21:28:25.000000 ezcharts-0.4.0/ezcharts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 21:28:25.000000 ezcharts-0.4.0/ezcharts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-15 21:28:25.000000 ezcharts-0.4.0/ezcharts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 21:27:28.000000 ezcharts-0.4.0/ezcharts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-15 21:28:25.000000 ezcharts-0.4.0/ezcharts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-15 21:28:25.000000 ezcharts-0.4.0/ezcharts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-15 21:25:19.000000 ezcharts-0.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 21:28:25.134972 ezcharts-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-06-15 21:25:19.000000 ezcharts-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.394006 ezcharts-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    15820 2023-06-27 08:33:48.000000 ezcharts-0.5.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-27 08:33:48.000000 ezcharts-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5779 2023-06-28 15:01:42.390006 ezcharts-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-06-27 08:33:48.000000 ezcharts-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.325999 ezcharts-0.5.0/ezcharts/
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.330000 ezcharts-0.5.0/ezcharts/components/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6160 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/components/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    13649 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/components/dss.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/ezchart.py
+-rw-rw-rw-   0 root         (0) root         (0)    15727 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11683 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/components/modkit.py
+-rw-rw-rw-   0 root         (0) root         (0)    12562 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/components/mosdepth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.330000 ezcharts-0.5.0/ezcharts/components/reports/
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/reports/comp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7295 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/reports/labs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/reports/ond.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/components/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.321999 ezcharts-0.5.0/ezcharts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.330000 ezcharts-0.5.0/ezcharts/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/images/LAB_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/images/OND_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/images/OND_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/images/ONT_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)   894078 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/images/dots.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.317998 ezcharts-0.5.0/ezcharts/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.330000 ezcharts-0.5.0/ezcharts/data/reference/hg19/
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/reference/hg19/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.334000 ezcharts-0.5.0/ezcharts/data/reference/hg38/
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/reference/hg38/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.334000 ezcharts-0.5.0/ezcharts/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/scripts/epi2melabs.js
+-rw-rw-rw-   0 root         (0) root         (0)   394601 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/scripts/metagenomics-sankey-util.js
+-rw-rw-rw-   0 root         (0) root         (0)    22324 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/scripts/metagenomics-sankey.js
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/scripts/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/scripts/ond.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.334000 ezcharts-0.5.0/ezcharts/data/styles/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/styles/epi2melabs.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/styles/metagenomics-sankey.css
+-rw-rw-rw-   0 root         (0) root         (0)   898896 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/styles/ond.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.346001 ezcharts-0.5.0/ezcharts/data/test/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)  1916228 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/fastcat.stats.gz
+-rw-rw-rw-   0 root         (0) root         (0)    28549 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/hg38_cnv.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/hg38_some_bands.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)   427338 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/karyomap_vals.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    16943 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/nextclade.json
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/plot-spec.json
+-rwxrwxrwx   0 root         (0) root         (0)      790 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/ref.fa.fai
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/sankey.json
+-rw-rw-rw-   0 root         (0) root         (0)  1125122 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/test_dml.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    35285 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/test_dmr.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)  1458860 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/test_modkit.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/test_modkit_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     7150 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/test_mosdepth.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/test_mosdepth_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/test/versions.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.346001 ezcharts-0.5.0/ezcharts/data/themes/
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/themes/epi2melabs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/themes/ond.json
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/themes/walden.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.346001 ezcharts-0.5.0/ezcharts/data/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.321999 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.350002 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/js/
+-rw-rw-rw-   0 root         (0) root         (0)    80599 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.358002 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
+-rw-rw-rw-   0 root         (0) root         (0)    17886 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
+-rw-rw-rw-   0 root         (0) root         (0)    73610 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.358002 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.362003 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.366003 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.366003 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.366003 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1017477 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/echarts.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.370004 ezcharts-0.5.0/ezcharts/data/vendor/simple-datatables/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css
+-rw-rw-rw-   0 root         (0) root         (0)    38201 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js
+-rw-rw-rw-   0 root         (0) root         (0)    12531 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/demo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.370004 ezcharts-0.5.0/ezcharts/layout/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.370004 ezcharts-0.5.0/ezcharts/layout/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/banner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/offcanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     7587 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/snippets/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/layout/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.390006 ezcharts-0.5.0/ezcharts/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     9172 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/_base.py
+-rw-rw-rw-   0 root         (0) root         (0) 13970130 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/axisgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/categorical.py
+-rw-rw-rw-   0 root         (0) root         (0)     5065 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12727 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/ideogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2023-06-28 14:54:36.000000 ezcharts-0.5.0/ezcharts/plots/karyomap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/metagenomics_sankey.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/relational.py
+-rwxrwxrwx   0 root         (0) root         (0)     3444 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/sunburst.py
+-rw-rw-rw-   0 root         (0) root         (0)     7208 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/plots/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-27 08:33:48.000000 ezcharts-0.5.0/ezcharts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:01:42.325999 ezcharts-0.5.0/ezcharts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5779 2023-06-28 15:01:42.000000 ezcharts-0.5.0/ezcharts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8868 2023-06-28 15:01:42.000000 ezcharts-0.5.0/ezcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:01:42.000000 ezcharts-0.5.0/ezcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-28 15:01:42.000000 ezcharts-0.5.0/ezcharts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:00:00.000000 ezcharts-0.5.0/ezcharts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-28 15:01:42.000000 ezcharts-0.5.0/ezcharts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-28 15:01:42.000000 ezcharts-0.5.0/ezcharts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-27 08:33:48.000000 ezcharts-0.5.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:01:42.394006 ezcharts-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-06-27 08:33:48.000000 ezcharts-0.5.0/setup.py
```

### Comparing `ezcharts-0.4.0/LICENSE.md` & `ezcharts-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/PKG-INFO` & `ezcharts-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.4.0
+Version: 0.5.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ezcharts-0.4.0/README.md` & `ezcharts-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/__init__.py` & `ezcharts-0.5.0/ezcharts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Simple eCharts API."""
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 import argparse
 import importlib
 import logging
 
 from ezcharts import util
 from ezcharts.plots.axisgrid import *  # noqa: F401,F403
@@ -30,15 +30,15 @@
 
     subparsers = parser.add_subparsers(
         title='subcommands', description='valid commands',
         help='additional help', dest='command')
     subparsers.required = True
 
     # all component demos, plus some others
-    components = ['params', 'nextclade', 'fastcat']
+    components = ['params', 'nextclade', 'fastcat', 'dss', 'modkit', 'mosdepth']
     others = ['ezcharts.demo', 'ezcharts.plots', 'ezcharts.plots.ideogram']
 
     demos = [f'ezcharts.components.{comp}' for comp in components] + others
     for module in demos:
         mod = importlib.import_module(module)
         p = subparsers.add_parser(
             module.split(".")[-1], parents=[mod.argparser()])
```

### Comparing `ezcharts-0.4.0/ezcharts/components/ezchart.py` & `ezcharts-0.5.0/ezcharts/components/ezchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/nextclade.py` & `ezcharts-0.5.0/ezcharts/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/params.py` & `ezcharts-0.5.0/ezcharts/components/params.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/reports/__init__.py` & `ezcharts-0.5.0/ezcharts/components/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/reports/comp.py` & `ezcharts-0.5.0/ezcharts/components/reports/comp.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/reports/labs.py` & `ezcharts-0.5.0/ezcharts/components/reports/labs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/reports/ond.py` & `ezcharts-0.5.0/ezcharts/components/reports/ond.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/theme.py` & `ezcharts-0.5.0/ezcharts/components/theme.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/components/versions.py` & `ezcharts-0.5.0/ezcharts/components/versions.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/images/LAB_logo.svg` & `ezcharts-0.5.0/ezcharts/data/images/LAB_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/images/OND_logo.svg` & `ezcharts-0.5.0/ezcharts/data/images/OND_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/images/OND_logo.txt` & `ezcharts-0.5.0/ezcharts/data/images/OND_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/images/ONT_logo.txt` & `ezcharts-0.5.0/ezcharts/data/images/ONT_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/images/dots.svg` & `ezcharts-0.5.0/ezcharts/data/images/dots.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/reference/hg19/cytoBand.txt.gz` & `ezcharts-0.5.0/ezcharts/data/reference/hg19/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/reference/hg38/cytoBand.txt.gz` & `ezcharts-0.5.0/ezcharts/data/reference/hg38/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/scripts/epi2melabs.js` & `ezcharts-0.5.0/ezcharts/data/scripts/epi2melabs.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/scripts/metagenomics-sankey-util.js` & `ezcharts-0.5.0/ezcharts/data/scripts/metagenomics-sankey-util.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/scripts/metagenomics-sankey.js` & `ezcharts-0.5.0/ezcharts/data/scripts/metagenomics-sankey.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/scripts/ond.js` & `ezcharts-0.5.0/ezcharts/data/scripts/ond.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/styles/epi2melabs.scss` & `ezcharts-0.5.0/ezcharts/data/styles/epi2melabs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/styles/metagenomics-sankey.css` & `ezcharts-0.5.0/ezcharts/data/styles/metagenomics-sankey.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/styles/ond.scss` & `ezcharts-0.5.0/ezcharts/data/styles/ond.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/fastcat.stats.gz` & `ezcharts-0.5.0/ezcharts/data/test/fastcat.stats.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/hg38_cnv.bed.gz` & `ezcharts-0.5.0/ezcharts/data/test/hg38_cnv.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/hg38_some_bands.bed.gz` & `ezcharts-0.5.0/ezcharts/data/test/hg38_some_bands.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/nextclade.json` & `ezcharts-0.5.0/ezcharts/data/test/nextclade.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/params.json` & `ezcharts-0.5.0/ezcharts/data/test/params.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/plot-spec.json` & `ezcharts-0.5.0/ezcharts/data/test/plot-spec.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/test/sankey.json` & `ezcharts-0.5.0/ezcharts/data/test/sankey.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/themes/epi2melabs.json` & `ezcharts-0.5.0/ezcharts/data/themes/epi2melabs.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/themes/ond.json` & `ezcharts-0.5.0/ezcharts/data/themes/ond.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/themes/walden.json` & `ezcharts-0.5.0/ezcharts/data/themes/walden.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss` & `ezcharts-0.5.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/echarts.min.js` & `ezcharts-0.5.0/ezcharts/data/vendor/echarts.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css` & `ezcharts-0.5.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js` & `ezcharts-0.5.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/demo.py` & `ezcharts-0.5.0/ezcharts/demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 from dominate.tags import p
 import numpy as np
 import pandas as pd
 from pkg_resources import resource_filename
 
 import ezcharts as ezc
 from ezcharts import util
+from ezcharts.components.common import fasta_idx, HSA_CHROMOSOME_ORDER
+from ezcharts.components.dss import load_dml, load_dmr
 from ezcharts.components.ezchart import EZChart
+from ezcharts.components.fastcat import load_bamstats_flagstat, load_stats
 from ezcharts.components.fastcat import SeqSummary
+from ezcharts.components.modkit import load_bedmethyl, load_modkit_summary
+from ezcharts.components.mosdepth import load_mosdepth_regions, load_mosdepth_summary
 from ezcharts.components.nextclade import NextClade, NXTComponent
 from ezcharts.components.reports.labs import LabsReport
 from ezcharts.components.theme import LAB_head_resources
 from ezcharts.layout.snippets import DataTable
 from ezcharts.layout.snippets import Grid
 from ezcharts.layout.snippets import OffCanvas
 from ezcharts.layout.snippets import Progress
 from ezcharts.layout.snippets import Stats
 from ezcharts.layout.snippets import Tabs
 from ezcharts.layout.snippets.cards import Cards
 from ezcharts.layout.snippets.cards import ICard
 from ezcharts.plots import Plot
 from ezcharts.plots.ideogram import ideogram
+from ezcharts.plots.karyomap import karyomap
 
 # Setup simple globals
 WORKFLOW_NAME = 'wf-template'
 REPORT_TITLE = f'{WORKFLOW_NAME}-report'
 
 
 def main(args):
@@ -187,14 +193,24 @@
         EZChart(example_plot("heatmap"), 'epi2melabs')
 
     with report.add_section('Human Genome', 'Genome'):
         EZChart(
             ideogram(blocks='cytobands'),
             'epi2melabs', height="800px")
 
+    with report.add_section('Human karyotype heatmap', 'Karyomap'):
+        vals = pd.read_csv(
+            resource_filename('ezcharts', "data/test/karyomap_vals.tsv.gz"), sep='\t')
+        faidx = fasta_idx(resource_filename('ezcharts', "data/test/ref.fa.fai"))
+        EZChart(karyomap(
+            vals, 'chr', 'pos', 'values',
+            stats='count',
+            ref_lengths=faidx,
+            order=HSA_CHROMOSOME_ORDER), 'epi2melabs')
+
     with report.add_section('Sunburst', 'Sunburst'):
         lineages = [{'name': 'Bacteria', 'value': 600, 'children': [
             {'name': 'Firmicutes', 'value': 600, 'children': [
                 {'name': 'Bacilli', 'value': 600, 'children': [
                     {'name': 'Bacillales', 'value': 600, 'children': [
                         {'name': 'Bacillaceae', 'value': 500, 'children': [
                             {'name': 'Bacillus', 'value': 500, 'children': [
@@ -224,14 +240,50 @@
 
     with report.add_section('Sankey plot', 'Sankey'):
         sankey_json = resource_filename('ezcharts', "data/test/sankey.json")
         with open(sankey_json, 'r') as sfh:
             sankey_dict = json.load(sfh)
             ezc.metagenomics_sankey(sankey_dict)
 
+    dataset_examples = {
+        'fastcat': load_stats(resource_filename(
+            'ezcharts', "data/test/fastcat.stats.gz"), format='fastcat'),
+        'bamstats': load_stats(resource_filename(
+            'ezcharts', "data/test/bamstats.readstats.tsv.gz"), format='bamstats'),
+        'flagstat': load_bamstats_flagstat(resource_filename(
+            'ezcharts', "data/test/bamstats.flagstat.tsv")),
+        'modkit summary': load_modkit_summary(resource_filename(
+            'ezcharts', "data/test/test_modkit_summary.tsv")),
+        'modkit bedMethyl': load_bedmethyl(resource_filename(
+            'ezcharts', "data/test/test_modkit.bed.gz")),
+        'DSS DML': load_dml(resource_filename(
+            'ezcharts', "data/test/test_dml.tsv.gz")),
+        'DSS DMR': load_dmr(resource_filename(
+            'ezcharts', "data/test/test_dmr.tsv.gz")),
+        'mosdepth summary': load_mosdepth_summary(resource_filename(
+            'ezcharts', "data/test/test_mosdepth_summary.tsv")),
+        'mosdepth regions': load_mosdepth_regions(resource_filename(
+            'ezcharts', "data/test/test_mosdepth.bed.gz")),
+        'fai index': fasta_idx(resource_filename(
+            'ezcharts', "data/test/ref.fa.fai")),
+    }
+    with report.add_section('Data types', 'Data'):
+        p(
+            "The workflow comes with a range of data loaders, as shown in the",
+            "tables below (10 rows max displayed).")
+        tabs = Tabs()
+        for data_type in dataset_examples.keys():
+            df = dataset_examples[data_type]
+            with tabs.add_tab(data_type):
+                if isinstance(df, tuple) or isinstance(df, tuple):
+                    for d in df:
+                        DataTable.from_pandas(d.head(10))
+                else:
+                    DataTable.from_pandas(df.head(10))
+
     logger.info('Reticulating splines')
     report.write(args.output)
 
 
 def argparser():
     """Argument parser for entrypoint."""
     parser = argparse.ArgumentParser(
```

### Comparing `ezcharts-0.4.0/ezcharts/layout/base.py` & `ezcharts-0.5.0/ezcharts/layout/base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/resource.py` & `ezcharts-0.5.0/ezcharts/layout/resource.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/__init__.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/banner.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/banner.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/cards.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/cards.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/document.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/document.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/grid.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/grid.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/offcanvas.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/offcanvas.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/progress.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/progress.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/section.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/section.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/stats.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/stats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/table.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/table.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/snippets/tabs.py` & `ezcharts-0.5.0/ezcharts/layout/snippets/tabs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/layout/util.py` & `ezcharts-0.5.0/ezcharts/layout/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/__init__.py` & `ezcharts-0.5.0/ezcharts/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/_base.py` & `ezcharts-0.5.0/ezcharts/plots/_base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/_model.py` & `ezcharts-0.5.0/ezcharts/plots/_model.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/categorical.py` & `ezcharts-0.5.0/ezcharts/plots/categorical.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Categorical plots."""
 
+import numpy as np
 
 from ezcharts.plots import Plot
 
 __all__ = [
     "catplot", "stripplot", "swarmplot", "boxplot", "violinplot",
     "boxenplot", "pointplot", "barplot", "countplot"]
 
@@ -81,14 +82,17 @@
     plt.yAxis = dict(name=y_name, type='value')
 
     plt.add_dataset({
         'id': 'raw',
         'dimensions': data.columns,
         'source': data.values})
 
+    # If there are nan values, replace with zeros
+    plt.dataset[0].source = np.nan_to_num(plt.dataset[0].source, nan=0)
+
     # Automatically map series to columns in the dataset
     if dodge:
         plt.series = [{'type': 'bar'}] * (data.shape[1] - 1)
     else:
         plt.series = [{'type': 'bar', 'stack': x_name}] * (data.shape[1] - 1)
 
     # Show a label per bar by default as ezcharts 'auto' method is very conservative.
```

### Comparing `ezcharts-0.4.0/ezcharts/plots/distribution.py` & `ezcharts-0.5.0/ezcharts/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/ideogram.py` & `ezcharts-0.5.0/ezcharts/plots/ideogram.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/matrix.py` & `ezcharts-0.5.0/ezcharts/plots/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Visualizing matrices of data."""
 import pandas as pd
 import seaborn as sns
 
 from ezcharts.plots import Plot
 
+
 __all__ = ["heatmap", "clustermap"]
 
 
 def heatmap(
         data, *, vmin=None, vmax=None, cmap=None, center=None, robust=False,
         annot=True, fmt='.2g', annot_kws=None, linewidths=0, linecolor='white',
         cbar=True, cbar_kws=None, cbar_ax=None, square=False, xticklabels='auto',
```

### Comparing `ezcharts-0.4.0/ezcharts/plots/metagenomics_sankey.py` & `ezcharts-0.5.0/ezcharts/plots/metagenomics_sankey.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/relational.py` & `ezcharts-0.5.0/ezcharts/plots/relational.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/sunburst.py` & `ezcharts-0.5.0/ezcharts/plots/sunburst.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/plots/util.py` & `ezcharts-0.5.0/ezcharts/plots/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts/util.py` & `ezcharts-0.5.0/ezcharts/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.4.0/ezcharts.egg-info/PKG-INFO` & `ezcharts-0.5.0/ezcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.4.0
+Version: 0.5.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ezcharts-0.4.0/ezcharts.egg-info/SOURCES.txt` & `ezcharts-0.5.0/ezcharts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 ezcharts.egg-info/SOURCES.txt
 ezcharts.egg-info/dependency_links.txt
 ezcharts.egg-info/entry_points.txt
 ezcharts.egg-info/not-zip-safe
 ezcharts.egg-info/requires.txt
 ezcharts.egg-info/top_level.txt
 ezcharts/components/__init__.py
+ezcharts/components/common.py
+ezcharts/components/dss.py
 ezcharts/components/ezchart.py
 ezcharts/components/fastcat.py
+ezcharts/components/modkit.py
+ezcharts/components/mosdepth.py
 ezcharts/components/nextclade.py
 ezcharts/components/params.py
 ezcharts/components/theme.py
 ezcharts/components/versions.py
 ezcharts/components/reports/__init__.py
 ezcharts/components/reports/comp.py
 ezcharts/components/reports/labs.py
@@ -37,21 +41,31 @@
 ezcharts/data/scripts/metagenomics-sankey-util.js
 ezcharts/data/scripts/metagenomics-sankey.js
 ezcharts/data/scripts/nextclade.html
 ezcharts/data/scripts/ond.js
 ezcharts/data/styles/epi2melabs.scss
 ezcharts/data/styles/metagenomics-sankey.css
 ezcharts/data/styles/ond.scss
+ezcharts/data/test/bamstats.flagstat.tsv
+ezcharts/data/test/bamstats.readstats.tsv.gz
 ezcharts/data/test/fastcat.stats.gz
 ezcharts/data/test/hg38_cnv.bed.gz
 ezcharts/data/test/hg38_some_bands.bed.gz
+ezcharts/data/test/karyomap_vals.tsv.gz
 ezcharts/data/test/nextclade.json
 ezcharts/data/test/params.json
 ezcharts/data/test/plot-spec.json
+ezcharts/data/test/ref.fa.fai
 ezcharts/data/test/sankey.json
+ezcharts/data/test/test_dml.tsv.gz
+ezcharts/data/test/test_dmr.tsv.gz
+ezcharts/data/test/test_modkit.bed.gz
+ezcharts/data/test/test_modkit_summary.tsv
+ezcharts/data/test/test_mosdepth.bed.gz
+ezcharts/data/test/test_mosdepth_summary.tsv
 ezcharts/data/test/versions.txt
 ezcharts/data/themes/epi2melabs.json
 ezcharts/data/themes/ond.json
 ezcharts/data/themes/walden.json
 ezcharts/data/vendor/echarts.min.js
 ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
 ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
@@ -164,13 +178,14 @@
 ezcharts/plots/__init__.py
 ezcharts/plots/_base.py
 ezcharts/plots/_model.py
 ezcharts/plots/axisgrid.py
 ezcharts/plots/categorical.py
 ezcharts/plots/distribution.py
 ezcharts/plots/ideogram.py
+ezcharts/plots/karyomap.py
 ezcharts/plots/matrix.py
 ezcharts/plots/metagenomics_sankey.py
 ezcharts/plots/regression.py
 ezcharts/plots/relational.py
 ezcharts/plots/sunburst.py
 ezcharts/plots/util.py
```

### Comparing `ezcharts-0.4.0/setup.py` & `ezcharts-0.5.0/setup.py`

 * *Files identical despite different names*

