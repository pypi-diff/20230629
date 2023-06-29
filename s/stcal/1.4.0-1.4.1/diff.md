# Comparing `tmp/stcal-1.4.0.tar.gz` & `tmp/stcal-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stcal-1.4.0.tar", last modified: Tue Jun 27 19:10:26 2023, max compression
+gzip compressed data, was "stcal-1.4.1.tar", last modified: Thu Jun 29 13:33:24 2023, max compression
```

## Comparing `stcal-1.4.0.tar` & `stcal-1.4.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.236657 stcal-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-27 19:10:12.000000 stcal-1.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-27 19:10:12.000000 stcal-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-27 19:10:12.000000 stcal-1.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-06-27 19:10:12.000000 stcal-1.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-27 19:10:12.000000 stcal-1.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-27 19:10:12.000000 stcal-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-27 19:10:12.000000 stcal-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-27 19:10:26.236657 stcal-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-27 19:10:12.000000 stcal-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-27 19:10:12.000000 stcal-1.4.0/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-27 19:10:12.000000 stcal-1.4.0/benchmarks/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.128656 stcal-1.4.0/docs/stcal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/docs/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/docs/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 19:10:12.000000 stcal-1.4.0/docs/stcal/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-27 19:10:12.000000 stcal-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:10:26.236657 stcal-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.124656 stcal-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/src/stcal/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/src/stcal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dark_current/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dark_current/dark_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dark_current/dark_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/dynamicdq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    36348 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/jump/twopoint_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/linearity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/linearity/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)   127963 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/ols_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    56323 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/ramp_fitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.136656 stcal-1.4.0/src/stcal/saturation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-27 19:10:12.000000 stcal-1.4.0/src/stcal/saturation/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.132656 stcal-1.4.0/src/stcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-27 19:10:26.000000 stcal-1.4.0/src/stcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:10:25.000000 stcal-1.4.0/src/stcal.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.184657 stcal-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/current_gdqfits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:10:26.236657 stcal-1.4.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/data/input_gdq_flarge.fits
--rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/data/large_event_input_dq_cube2.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/data/snowball1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    53011 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_ramp_fitting_gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-06-27 19:10:12.000000 stcal-1.4.0/tests/test_twopoint_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-27 19:10:12.000000 stcal-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.789134 stcal-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.709134 stcal-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.709134 stcal-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-29 13:33:12.000000 stcal-1.4.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-29 13:33:12.000000 stcal-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-29 13:33:12.000000 stcal-1.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-06-29 13:33:12.000000 stcal-1.4.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-29 13:33:12.000000 stcal-1.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-29 13:33:12.000000 stcal-1.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-29 13:33:12.000000 stcal-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-29 13:33:24.785134 stcal-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-29 13:33:12.000000 stcal-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 13:33:12.000000 stcal-1.4.1/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-29 13:33:12.000000 stcal-1.4.1/benchmarks/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/stcal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/docs/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 13:33:12.000000 stcal-1.4.1/docs/stcal/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-29 13:33:12.000000 stcal-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:33:24.789134 stcal-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.709134 stcal-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dark_current/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dark_current/dark_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dark_current/dark_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/dynamicdq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36437 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/jump/twopoint_difference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/linearity/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.717134 stcal-1.4.1/src/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127963 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/ols_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56323 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/ramp_fitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.717134 stcal-1.4.1/src/stcal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-29 13:33:12.000000 stcal-1.4.1/src/stcal/saturation/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.713134 stcal-1.4.1/src/stcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:33:24.000000 stcal-1.4.1/src/stcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:33:23.000000 stcal-1.4.1/src/stcal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.753134 stcal-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/current_gdqfits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:33:24.785134 stcal-1.4.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/data/input_gdq_flarge.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/data/large_event_input_dq_cube2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/data/snowball1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53011 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_ramp_fitting_gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50096 2023-06-29 13:33:12.000000 stcal-1.4.1/tests/test_twopoint_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-29 13:33:12.000000 stcal-1.4.1/tox.ini
```

### Comparing `stcal-1.4.0/.github/labeler.yml` & `stcal-1.4.1/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/.github/pull_request_template.md` & `stcal-1.4.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/.github/workflows/ci.yml` & `stcal-1.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/.github/workflows/publish-to-pypi.yml` & `stcal-1.4.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/.gitignore` & `stcal-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/.readthedocs.yaml` & `stcal-1.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/CHANGES.rst` & `stcal-1.4.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+1.4.1 (2023-06-29)
+==================
+
+Bug Fixes
+---------
+
+jump
+~~~~
+
+- Added statement to prevent the number of cores used in multiprocessing from
+  being larger than the number of rows. This was causing some CI tests to fail. [#176]
+
 1.4.0 (2023-06-27)
 ==================
 
 Bug Fixes
 ---------
 
 jump
```

### Comparing `stcal-1.4.0/CODE_OF_CONDUCT.md` & `stcal-1.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/CONTRIBUTING.md` & `stcal-1.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/LICENSE` & `stcal-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/PKG-INFO` & `stcal-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.4.0
+Version: 1.4.1
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.4.0/README.md` & `stcal-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/benchmarks/dark_current.py` & `stcal-1.4.1/benchmarks/dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/benchmarks/linearity.py` & `stcal-1.4.1/benchmarks/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/benchmarks/ramp_fitting.py` & `stcal-1.4.1/benchmarks/ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/benchmarks/saturation.py` & `stcal-1.4.1/benchmarks/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/docs/Makefile` & `stcal-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/docs/conf.py` & `stcal-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/docs/stcal/jump/description.rst` & `stcal-1.4.1/docs/stcal/jump/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/docs/stcal/ramp_fitting/description.rst` & `stcal-1.4.1/docs/stcal/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/pyproject.toml` & `stcal-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/dark_current/dark_class.py` & `stcal-1.4.1/src/stcal/dark_current/dark_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/dark_current/dark_sub.py` & `stcal-1.4.1/src/stcal/dark_current/dark_sub.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/dqflags.py` & `stcal-1.4.1/src/stcal/dqflags.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/jump/jump.py` & `stcal-1.4.1/src/stcal/jump/jump.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,16 @@
         n_slices = 1
     elif max_cores == 'quarter':
         n_slices = max_available // 4 or 1
     elif max_cores == 'half':
         n_slices = max_available // 2 or 1
     elif max_cores == 'all':
         n_slices = max_available
-
+    # Make sure we don't have more slices than rows.
+    n_slices = min(n_rows, n_slices)
     if n_slices == 1:
         gdq, row_below_dq, row_above_dq, total_primary_crs, stddev = \
             twopt.find_crs(data, gdq, readnoise_2d, rejection_thresh,
                            three_grp_thresh, four_grp_thresh, frames_per_group,
                            flag_4_neighbors, max_jump_to_flag_neighbors,
                            min_jump_to_flag_neighbors, dqflags,
                            after_jump_flag_e1=after_jump_flag_e1,
```

### Comparing `stcal-1.4.0/src/stcal/jump/twopoint_difference.py` & `stcal-1.4.1/src/stcal/jump/twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/linearity/linearity.py` & `stcal-1.4.1/src/stcal/linearity/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/ramp_fitting/gls_fit.py` & `stcal-1.4.1/src/stcal/ramp_fitting/gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/ramp_fitting/ols_fit.py` & `stcal-1.4.1/src/stcal/ramp_fitting/ols_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit.py` & `stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/ramp_fitting/ramp_fit_class.py` & `stcal-1.4.1/src/stcal/ramp_fitting/ramp_fit_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/ramp_fitting/utils.py` & `stcal-1.4.1/src/stcal/ramp_fitting/utils.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal/saturation/saturation.py` & `stcal-1.4.1/src/stcal/saturation/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/src/stcal.egg-info/PKG-INFO` & `stcal-1.4.1/src/stcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.4.0
+Version: 1.4.1
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.4.0/src/stcal.egg-info/SOURCES.txt` & `stcal-1.4.1/src/stcal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/current_gdqfits` & `stcal-1.4.1/tests/current_gdqfits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/data/input_gdq_flarge.fits` & `stcal-1.4.1/tests/data/input_gdq_flarge.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/data/large_event_input_dq_cube2.fits` & `stcal-1.4.1/tests/data/large_event_input_dq_cube2.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/data/snowball1.fits` & `stcal-1.4.1/tests/data/snowball1.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_dark_current.py` & `stcal-1.4.1/tests/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_dq.py` & `stcal-1.4.1/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_jump.py` & `stcal-1.4.1/tests/test_jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_linearity.py` & `stcal-1.4.1/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_ramp_fitting.py` & `stcal-1.4.1/tests/test_ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_ramp_fitting_gls_fit.py` & `stcal-1.4.1/tests/test_ramp_fitting_gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_saturation.py` & `stcal-1.4.1/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tests/test_twopoint_difference.py` & `stcal-1.4.1/tests/test_twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.4.0/tox.ini` & `stcal-1.4.1/tox.ini`

 * *Files identical despite different names*

