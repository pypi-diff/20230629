# Comparing `tmp/circuitpython-jled-1.0.3.tar.gz` & `tmp/circuitpython-jled-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-jled-1.0.3.tar", last modified: Sun Jan 15 11:27:40 2023, max compression
+gzip compressed data, was "circuitpython-jled-1.0.4.tar", last modified: Thu Jun 29 20:00:49 2023, max compression
```

## Comparing `circuitpython-jled-1.0.3.tar` & `circuitpython-jled-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.813454 circuitpython-jled-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.801455 circuitpython-jled-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.805455 circuitpython-jled-1.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.805455 circuitpython-jled-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.805455 circuitpython-jled-1.0.3/.images/
--rw-r--r--   0 runner    (1001) docker     (123)   503809 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.images/jled.gif
--rw-r--r--   0 runner    (1001) docker     (123)   523086 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.images/jled_cheat_sheet.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-01-15 11:27:40.813454 circuitpython-jled-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.809455 circuitpython-jled-1.0.3/circuitpython_jled.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-01-15 11:27:40.000000 circuitpython-jled-1.0.3/circuitpython_jled.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-01-15 11:27:40.000000 circuitpython-jled-1.0.3/circuitpython_jled.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 11:27:40.000000 circuitpython-jled-1.0.3/circuitpython_jled.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-15 11:27:40.000000 circuitpython-jled-1.0.3/circuitpython_jled.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-15 11:27:40.000000 circuitpython-jled-1.0.3/circuitpython_jled.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.809455 circuitpython-jled-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/.test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.809455 circuitpython-jled-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.809455 circuitpython-jled-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/examples/jled_breathe.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/examples/jled_micropython.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/examples/jled_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/examples/jled_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/examples/jled_user_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.813454 circuitpython-jled-1.0.3/jled/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/hal_pwm_circuitpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/hal_pwm_micropython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/hal_time_circuitpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/hal_time_micropython.py
--rw-r--r--   0 runner    (1001) docker     (123)    17158 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/jled.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/jled_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/play.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/python_pwm_hal.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/jled/python_time_hal.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.813454 circuitpython-jled-1.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-01-15 11:27:26.000000 circuitpython-jled-1.0.3/scripts/install_mp.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 11:27:40.813454 circuitpython-jled-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 11:27:40.813454 circuitpython-jled-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_circuitpython_pwm_hal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_circuitpython_time_hal.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_fadeon_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_jled.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_jledsequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_lerp8by8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_micropython_pwm_hal.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_play.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-15 11:27:33.000000 circuitpython-jled-1.0.3/tests/test_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.118152 circuitpython-jled-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.110152 circuitpython-jled-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.110152 circuitpython-jled-1.0.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.110152 circuitpython-jled-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.114152 circuitpython-jled-1.0.4/.images/
+-rw-r--r--   0 runner    (1001) docker     (123)   503809 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.images/jled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   523086 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.images/jled_cheat_sheet.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-29 20:00:49.118152 circuitpython-jled-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.114152 circuitpython-jled-1.0.4/circuitpython_jled.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-29 20:00:49.000000 circuitpython-jled-1.0.4/circuitpython_jled.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-29 20:00:49.000000 circuitpython-jled-1.0.4/circuitpython_jled.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:00:49.000000 circuitpython-jled-1.0.4/circuitpython_jled.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 20:00:49.000000 circuitpython-jled-1.0.4/circuitpython_jled.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 20:00:49.000000 circuitpython-jled-1.0.4/circuitpython_jled.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.114152 circuitpython-jled-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.114152 circuitpython-jled-1.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.114152 circuitpython-jled-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/examples/jled_breathe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/examples/jled_micropython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/examples/jled_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/examples/jled_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/examples/jled_user_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.118152 circuitpython-jled-1.0.4/jled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/hal_pwm_circuitpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/hal_pwm_micropython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/hal_time_circuitpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/hal_time_micropython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17158 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/jled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/jled_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/python_pwm_hal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/jled/python_time_hal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.118152 circuitpython-jled-1.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-06-29 20:00:32.000000 circuitpython-jled-1.0.4/scripts/install_mp.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:00:49.118152 circuitpython-jled-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:49.118152 circuitpython-jled-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_circuitpython_pwm_hal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_circuitpython_time_hal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_fadeon_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_jled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_jledsequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_lerp8by8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_micropython_pwm_hal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:00:41.000000 circuitpython-jled-1.0.4/tests/test_scale.py
```

### Comparing `circuitpython-jled-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-jled-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.github/workflows/build.yml` & `circuitpython-jled-1.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.github/workflows/release.yml` & `circuitpython-jled-1.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.gitignore` & `circuitpython-jled-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.images/jled.gif` & `circuitpython-jled-1.0.4/.images/jled.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.images/jled_cheat_sheet.jpg` & `circuitpython-jled-1.0.4/.images/jled_cheat_sheet.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.pre-commit-config.yaml` & `circuitpython-jled-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/.pylintrc` & `circuitpython-jled-1.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/LICENSE` & `circuitpython-jled-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/PKG-INFO` & `circuitpython-jled-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-jled
-Version: 1.0.3
+Version: 1.0.4
 Summary: Non-blocking LED controlling library
 Author-email: Jan Delgado <jdelgado@gmx.net>
 License: MIT
 Project-URL: Homepage, https://github.com/jandelgado/jled-circuitpython
 Keywords: adafruit,blinka,circuitpython,micropython,jled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -34,15 +34,15 @@
 An embedded library for Python to control LEDs. It uses a **non-blocking**
 approach and can control LEDs in simple (**on**/**off**) and complex
 (**blinking**, **breathing** and more) ways in a **time-driven** manner.
 
 This is a pure Python port of my `JLed <https://github.com/jandelgado/jled>`_
 C++ library.
 
-.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.3/.images/jled.gif
+.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.4/.images/jled.gif
     :alt: JLed in action
 
 Features
 ========
 
 - non-blocking
 - effects: simple on/off, breathe, blink, candle, fade, user-defined
@@ -70,15 +70,15 @@
 the LED gets physically updated. Alternatively ``play(led)`` can be call in the
 REPL as a shortcut.  Once finished, call ``led.reset()`` before playing the
 effect again.
 
 Cheat Sheet
 ===========
 
-.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.3/.images/jled_cheat_sheet.jpg
+.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.4/.images/jled_cheat_sheet.jpg
 
 Installation
 =============
 
 On supported GNU/Linux systems like the Raspberry Pi (with `Adafruit-Blinka
 <https://pypi.org/project/Adafruit-Blinka/>`_), you can install the lib
 locally `from PyPI <https://pypi.org/project/circuitpython-jled/>`_.  To
@@ -108,15 +108,15 @@
 
 ``JLed`` is available in the `Circuitpython Community Bundle <https://github.com/adafruit/CircuitPython_Community_Bundle>`_ 
 and can easily installed with `circup <https://pypi.org/project/circup/>`_ by 
 running::
 
     $ circup install jled
 
-Optionally copy also one of the example as ``main.py`` to the root of the filesystem. 
+Optionally copy also one of the example as ``code.py`` to the root of the filesystem. 
 
 Installing on a MicroPython device
 ----------------------------------
 
 Create a directory called ``jled`` on the device and `copy
 <https://pypi.org/project/mpremote/>`_ the following files into this directory:
 into this directory: ``jled.py``, ``jled_sequence.py``
@@ -125,20 +125,20 @@
 root of the filesystem.  The overall structure is:
 
 .. code-block::
 
    /
    ├─ main.py
    └─ jled
-       ├─ __init__.[m]mpy
-       ├─ hal_pwm_micropython.[m]mpy
-       ├─ hal_time_micropython.[m]mpy
-       ├─ jled.[m]mpy
-       ├─ jled_sequence.[m]mpy
-       └─ play.[m]mpy
+       ├─ __init__.[m]py
+       ├─ hal_pwm_micropython.[m]py
+       ├─ hal_time_micropython.[m]py
+       ├─ jled.[m]py
+       ├─ jled_sequence.[m]py
+       └─ play.[m]py
 
 To reduce memory consumption, Python source files can be compiled to binary
 ``mpy`` format using the `mpy-cross <https://pypi.org/project/mpy-cross/>`_
 tool. For convenience, a script to compile and copy jled to a connected device
 is provided here (see ``scripts/install_mp.sh``).
 
 Documentation
```

### Comparing `circuitpython-jled-1.0.3/README.rst` & `circuitpython-jled-1.0.4/circuitpython_jled.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: circuitpython-jled
+Version: 1.0.4
+Summary: Non-blocking LED controlling library
+Author-email: Jan Delgado <jdelgado@gmx.net>
+License: MIT
+Project-URL: Homepage, https://github.com/jandelgado/jled-circuitpython
+Keywords: adafruit,blinka,circuitpython,micropython,jled
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+Provides-Extra: optional
+License-File: LICENSE
+
 Introduction
 ============
 
 .. image:: https://github.com/jandelgado/jled-circuitpython/workflows/Build%20CI/badge.svg
     :target: https://github.com/jandelgado/jled-circuitpython/actions
     :alt: Build Status
 
@@ -16,15 +34,15 @@
 An embedded library for Python to control LEDs. It uses a **non-blocking**
 approach and can control LEDs in simple (**on**/**off**) and complex
 (**blinking**, **breathing** and more) ways in a **time-driven** manner.
 
 This is a pure Python port of my `JLed <https://github.com/jandelgado/jled>`_
 C++ library.
 
-.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.3/.images/jled.gif
+.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.4/.images/jled.gif
     :alt: JLed in action
 
 Features
 ========
 
 - non-blocking
 - effects: simple on/off, breathe, blink, candle, fade, user-defined
@@ -52,15 +70,15 @@
 the LED gets physically updated. Alternatively ``play(led)`` can be call in the
 REPL as a shortcut.  Once finished, call ``led.reset()`` before playing the
 effect again.
 
 Cheat Sheet
 ===========
 
-.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.3/.images/jled_cheat_sheet.jpg
+.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.4/.images/jled_cheat_sheet.jpg
 
 Installation
 =============
 
 On supported GNU/Linux systems like the Raspberry Pi (with `Adafruit-Blinka
 <https://pypi.org/project/Adafruit-Blinka/>`_), you can install the lib
 locally `from PyPI <https://pypi.org/project/circuitpython-jled/>`_.  To
@@ -90,15 +108,15 @@
 
 ``JLed`` is available in the `Circuitpython Community Bundle <https://github.com/adafruit/CircuitPython_Community_Bundle>`_ 
 and can easily installed with `circup <https://pypi.org/project/circup/>`_ by 
 running::
 
     $ circup install jled
 
-Optionally copy also one of the example as ``main.py`` to the root of the filesystem. 
+Optionally copy also one of the example as ``code.py`` to the root of the filesystem. 
 
 Installing on a MicroPython device
 ----------------------------------
 
 Create a directory called ``jled`` on the device and `copy
 <https://pypi.org/project/mpremote/>`_ the following files into this directory:
 into this directory: ``jled.py``, ``jled_sequence.py``
@@ -107,20 +125,20 @@
 root of the filesystem.  The overall structure is:
 
 .. code-block::
 
    /
    ├─ main.py
    └─ jled
-       ├─ __init__.[m]mpy
-       ├─ hal_pwm_micropython.[m]mpy
-       ├─ hal_time_micropython.[m]mpy
-       ├─ jled.[m]mpy
-       ├─ jled_sequence.[m]mpy
-       └─ play.[m]mpy
+       ├─ __init__.[m]py
+       ├─ hal_pwm_micropython.[m]py
+       ├─ hal_time_micropython.[m]py
+       ├─ jled.[m]py
+       ├─ jled_sequence.[m]py
+       └─ play.[m]py
 
 To reduce memory consumption, Python source files can be compiled to binary
 ``mpy`` format using the `mpy-cross <https://pypi.org/project/mpy-cross/>`_
 tool. For convenience, a script to compile and copy jled to a connected device
 is provided here (see ``scripts/install_mp.sh``).
 
 Documentation
```

### Comparing `circuitpython-jled-1.0.3/circuitpython_jled.egg-info/PKG-INFO` & `circuitpython-jled-1.0.4/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: circuitpython-jled
-Version: 1.0.3
-Summary: Non-blocking LED controlling library
-Author-email: Jan Delgado <jdelgado@gmx.net>
-License: MIT
-Project-URL: Homepage, https://github.com/jandelgado/jled-circuitpython
-Keywords: adafruit,blinka,circuitpython,micropython,jled
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-Provides-Extra: optional
-License-File: LICENSE
-
 Introduction
 ============
 
 .. image:: https://github.com/jandelgado/jled-circuitpython/workflows/Build%20CI/badge.svg
     :target: https://github.com/jandelgado/jled-circuitpython/actions
     :alt: Build Status
 
@@ -34,15 +16,15 @@
 An embedded library for Python to control LEDs. It uses a **non-blocking**
 approach and can control LEDs in simple (**on**/**off**) and complex
 (**blinking**, **breathing** and more) ways in a **time-driven** manner.
 
 This is a pure Python port of my `JLed <https://github.com/jandelgado/jled>`_
 C++ library.
 
-.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.3/.images/jled.gif
+.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.4/.images/jled.gif
     :alt: JLed in action
 
 Features
 ========
 
 - non-blocking
 - effects: simple on/off, breathe, blink, candle, fade, user-defined
@@ -70,15 +52,15 @@
 the LED gets physically updated. Alternatively ``play(led)`` can be call in the
 REPL as a shortcut.  Once finished, call ``led.reset()`` before playing the
 effect again.
 
 Cheat Sheet
 ===========
 
-.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.3/.images/jled_cheat_sheet.jpg
+.. image:: https://cdn.jsdelivr.net/gh/jandelgado/jled-circuitpython@v1.0.4/.images/jled_cheat_sheet.jpg
 
 Installation
 =============
 
 On supported GNU/Linux systems like the Raspberry Pi (with `Adafruit-Blinka
 <https://pypi.org/project/Adafruit-Blinka/>`_), you can install the lib
 locally `from PyPI <https://pypi.org/project/circuitpython-jled/>`_.  To
@@ -108,15 +90,15 @@
 
 ``JLed`` is available in the `Circuitpython Community Bundle <https://github.com/adafruit/CircuitPython_Community_Bundle>`_ 
 and can easily installed with `circup <https://pypi.org/project/circup/>`_ by 
 running::
 
     $ circup install jled
 
-Optionally copy also one of the example as ``main.py`` to the root of the filesystem. 
+Optionally copy also one of the example as ``code.py`` to the root of the filesystem. 
 
 Installing on a MicroPython device
 ----------------------------------
 
 Create a directory called ``jled`` on the device and `copy
 <https://pypi.org/project/mpremote/>`_ the following files into this directory:
 into this directory: ``jled.py``, ``jled_sequence.py``
@@ -125,20 +107,20 @@
 root of the filesystem.  The overall structure is:
 
 .. code-block::
 
    /
    ├─ main.py
    └─ jled
-       ├─ __init__.[m]mpy
-       ├─ hal_pwm_micropython.[m]mpy
-       ├─ hal_time_micropython.[m]mpy
-       ├─ jled.[m]mpy
-       ├─ jled_sequence.[m]mpy
-       └─ play.[m]mpy
+       ├─ __init__.[m]py
+       ├─ hal_pwm_micropython.[m]py
+       ├─ hal_time_micropython.[m]py
+       ├─ jled.[m]py
+       ├─ jled_sequence.[m]py
+       └─ play.[m]py
 
 To reduce memory consumption, Python source files can be compiled to binary
 ``mpy`` format using the `mpy-cross <https://pypi.org/project/mpy-cross/>`_
 tool. For convenience, a script to compile and copy jled to a connected device
 is provided here (see ``scripts/install_mp.sh``).
 
 Documentation
```

### Comparing `circuitpython-jled-1.0.3/circuitpython_jled.egg-info/SOURCES.txt` & `circuitpython-jled-1.0.4/circuitpython_jled.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/docs/_static/favicon.ico` & `circuitpython-jled-1.0.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/docs/conf.py` & `circuitpython-jled-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/docs/examples.rst` & `circuitpython-jled-1.0.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/examples/jled_sequence.py` & `circuitpython-jled-1.0.4/examples/jled_sequence.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/examples/jled_user_func.py` & `circuitpython-jled-1.0.4/examples/jled_user_func.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/__init__.py` & `circuitpython-jled-1.0.4/jled/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/hal_pwm_circuitpython.py` & `circuitpython-jled-1.0.4/jled/hal_pwm_circuitpython.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/hal_pwm_micropython.py` & `circuitpython-jled-1.0.4/jled/hal_pwm_micropython.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/hal_time_circuitpython.py` & `circuitpython-jled-1.0.4/jled/hal_time_circuitpython.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/hal_time_micropython.py` & `circuitpython-jled-1.0.4/jled/hal_time_micropython.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/jled.py` & `circuitpython-jled-1.0.4/jled/jled.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 * Author(s): Jan Delgado
 
 """
 
 import random
 
-__version__ = "v1.0.3"
+__version__ = "v1.0.4"
 __repo__ = "https://github.com/jandelgado/jled-circuitpython.git"
 
 FULL_BRIGHTNESS = 255
 ZERO_BRIGHTNESS = 0
 
 
 def scale8(a, factor):
```

### Comparing `circuitpython-jled-1.0.3/jled/jled_sequence.py` & `circuitpython-jled-1.0.4/jled/jled_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 
     def stop(self):
         """Turns off all objects controlled by this ``JLedSequence`` and stops
         the sequence. Further calls to :func:`update` will have no effect.
 
         :return: this JLedSequence object
         """
+        self._is_running = False
         for led in self._leds:
             led.stop()
         return self
 
     def repeat(self, num):
         """Use the ``repeat`` method to specify the number of repetitions. The
         default value is 1 repetition.
```

### Comparing `circuitpython-jled-1.0.3/jled/play.py` & `circuitpython-jled-1.0.4/jled/play.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/python_pwm_hal.py` & `circuitpython-jled-1.0.4/jled/python_pwm_hal.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/jled/python_time_hal.py` & `circuitpython-jled-1.0.4/jled/python_time_hal.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/pyproject.toml` & `circuitpython-jled-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-jled"
 description = "Non-blocking LED controlling library"
-version = "v1.0.3"
+version = "v1.0.4"
 readme = "README.rst"
 authors = [
     {name = "Jan Delgado", email = "jdelgado@gmx.net"}
 ]
 urls = {Homepage = "https://github.com/jandelgado/jled-circuitpython"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-jled-1.0.3/scripts/install_mp.sh` & `circuitpython-jled-1.0.4/scripts/install_mp.sh`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/mocks.py` & `circuitpython-jled-1.0.4/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_circuitpython_pwm_hal.py` & `circuitpython-jled-1.0.4/tests/test_circuitpython_pwm_hal.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_circuitpython_time_hal.py` & `circuitpython-jled-1.0.4/tests/test_circuitpython_time_hal.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_fadeon_func.py` & `circuitpython-jled-1.0.4/tests/test_fadeon_func.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_jled.py` & `circuitpython-jled-1.0.4/tests/test_jled.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_jledsequence.py` & `circuitpython-jled-1.0.4/tests/test_jledsequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,24 @@
     _ = t.tick
     seq2.update()
     assert not led.is_running
     assert not seq1.is_running
     assert not seq2.is_running
 
 
+def test_jledsequence_stays_off_after_stop():
+    fx = MockEffect([255, 255])
+    led = JLed(1).user_func(fx)
+    seq = JLedSequence.parallel([led]).forever()
+
+    assert seq.update()
+    seq.stop()
+    assert not seq.update()
+    assert not seq.is_running
+
 def test_jledsequence_stop_stops_all_leds():
     fx = MockEffect([255, 255])
     led = JLed(1).user_func(fx)
     seq = JLedSequence.parallel([led])
 
     seq.update()
     assert 255 == led._hal.val
```

### Comparing `circuitpython-jled-1.0.3/tests/test_lerp8by8.py` & `circuitpython-jled-1.0.4/tests/test_lerp8by8.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_micropython_pwm_hal.py` & `circuitpython-jled-1.0.4/tests/test_micropython_pwm_hal.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_play.py` & `circuitpython-jled-1.0.4/tests/test_play.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jled-1.0.3/tests/test_scale.py` & `circuitpython-jled-1.0.4/tests/test_scale.py`

 * *Files identical despite different names*

