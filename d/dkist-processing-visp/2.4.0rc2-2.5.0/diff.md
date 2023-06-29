# Comparing `tmp/dkist_processing_visp-2.4.0rc2.tar.gz` & `tmp/dkist_processing_visp-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.4.0rc2.tar", last modified: Tue Jun 27 19:52:25 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.5.0.tar", last modified: Thu Jun 29 20:44:35 2023, max compression
```

## Comparing `dkist_processing_visp-2.4.0rc2.tar` & `dkist_processing_visp-2.5.0.tar`

### file list

```diff
@@ -1,116 +1,114 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    20545 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.652426 dkist_processing_visp-2.4.0rc2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/changelog/116.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/changelog/117.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.652426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.652426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.652426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11306 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.656426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.656426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14744 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    40558 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20368 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.656426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10506 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    28801 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16332 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18994 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14009 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11818 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16234 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5091 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/single_task_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/trial_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.652426 dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-27 19:52:25.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-06-27 19:52:25.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 19:52:25.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-27 19:52:25.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 19:52:25.000000 dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:52:25.660426 dkist_processing_visp-2.4.0rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-06-27 19:52:25.664426 dkist_processing_visp-2.4.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-27 19:52:19.000000 dkist_processing_visp-2.4.0rc2/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.014332 dkist_processing_visp-2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    21516 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-29 20:44:35.014332 dkist_processing_visp-2.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.002332 dkist_processing_visp-2.5.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.002332 dkist_processing_visp-2.5.0/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.006332 dkist_processing_visp-2.5.0/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.006332 dkist_processing_visp-2.5.0/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11306 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.006332 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.006332 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14744 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    41082 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20368 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.010332 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10506 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4604 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    28801 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.010332 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16409 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.010332 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18994 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14009 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11818 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16234 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5091 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.010332 dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/single_task_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.002332 dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-29 20:44:34.000000 dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3873 2023-06-29 20:44:34.000000 dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 20:44:34.000000 dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-29 20:44:34.000000 dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-29 20:44:34.000000 dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.014332 dkist_processing_visp-2.5.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 20:44:35.014332 dkist_processing_visp-2.5.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-06-29 20:44:35.014332 dkist_processing_visp-2.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-29 20:44:30.000000 dkist_processing_visp-2.5.0/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.4.0rc2/.gitignore` & `dkist_processing_visp-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/.pre-commit-config.yaml` & `dkist_processing_visp-2.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/CHANGELOG.rst` & `dkist_processing_visp-2.5.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+v2.5.0 (2023-06-29)
+===================
+
+Misc
+----
+
+- Update to python 3.11 and update library package versions. (`#119 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/119>`__)
+
+
+v2.4.0 (2023-06-27)
+===================
+
+Features
+--------
+
+- Wield `*-common`'s development framework to tag DEBUG frames and create new trial workflows for local and PROD-level testing. (`#116 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/116>`__)
+
+
+Misc
+----
+
+- Update to support `dkist-processing-common` 3.0.0. Specifically the new signature of some of the `FitsDataMixin` methods. (`#117 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/117>`__)
+
+
+v2.3.1 (2023-06-15)
+===================
+
+Bugfixes
+--------
+
+- Fix failure in Geometric task that happened when some modstates had a a different number of identified hairline regions than others. (`#118 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/118>`__)
+
+
 v2.3.0 (2023-05-17)
 ===================
 
 Misc
 ----
 
 - Bumping common to 2.7.0: ParseL0InputData --> ParseL0InputDataBase, constant_flowers --> constant_buds (`#115 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/115>`__)
```

### Comparing `dkist_processing_visp-2.4.0rc2/PKG-INFO` & `dkist_processing_visp-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.4.0rc2
+Version: 2.5.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: grogu
 Provides-Extra: docs
 
 dkist-processing-visp
 =====================
```

### Comparing `dkist_processing_visp-2.4.0rc2/README.rst` & `dkist_processing_visp-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.5.0/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/bitbucket-pipelines.yml` & `dkist_processing_visp-2.5.0/bitbucket-pipelines.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #Build Configuration for docker deployment to artifactory
-image: python:3.10
+image: python:3.11
 
 definitions:
   services:
     redis:
       image: redis
   steps:
     - step: &lint
```

### Comparing `dkist_processing_visp-2.4.0rc2/check_changelog_updated.sh` & `dkist_processing_visp-2.5.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.5.0/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/geometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Visp geometric calibration task."""
 from typing import Generator
 
 import numpy as np
 import peakutils as pku
 import scipy.ndimage as spnd
 import scipy.optimize as spo
+import skimage.exposure as skie
 import skimage.metrics as skim
 import skimage.morphology as skimo
 import skimage.registration as skir
 from astropy.modeling import fitting
 from astropy.modeling import models
 from astropy.stats import sigma_clip
 from dkist_processing_common.codecs.fits import fits_array_encoder
@@ -363,15 +364,19 @@
         angle_list = []
         for modstate in range(1, self.constants.num_modstates + 1):
             data = self.basic_corrected_lamp_data(beam=beam, modstate=modstate)
             angle = self._compute_single_modstate_angles(data)
             logger.info(f"Angles for {beam = } and {modstate = } = {np.rad2deg(angle)} deg")
             angle_list.append(angle)
 
-        theta = float(np.nanmedian(angle_list))
+        # Flatten the list just in case we got different numbers of hairline regions for the different modstates
+        # (which can happen in data with strong higher-order hairline leaks).
+        flat_angle_list = np.hstack(angle_list)
+
+        theta = float(np.nanmedian(flat_angle_list))
         logger.info(f"Beam angle for {beam = }: {np.rad2deg(theta):0.4f} deg")
         return theta
 
     def _identify_hairlines_and_bad_pixels(
         self, input_array: np.ndarray
     ) -> tuple[np.ndarray, np.ndarray]:
         """
@@ -633,28 +638,32 @@
         )
         # list needed here because np.stack is depreciating working with a generator
         angle_corr_arrays = list(self.corrections_correct_geometry(arrays, angle=angle))
         modstate_avg = np.mean(np.stack(angle_corr_arrays), axis=0)
 
         mask = self.compute_offset_mask(modstate_avg)
         high_pass_filtered_array = self.high_pass_filter_array(modstate_avg)
+        rescaled_high_pass_filtered_array = skie.rescale_intensity(
+            high_pass_filtered_array, out_range=(0.0, 1.0)
+        )
 
-        return high_pass_filtered_array, mask
+        return rescaled_high_pass_filtered_array, mask
 
     @staticmethod
     def refine_ang_func(x, target, image) -> float:
         """Rotate and shift beam 2 then compare for similarity with beam 1."""
         xshift, yshift, ang = x
         rotated = next(GeometricCalibration.corrections_correct_geometry(image, angle=ang))
         shifted = next(
             GeometricCalibration.corrections_correct_geometry(
                 rotated, shift=np.array([xshift, yshift])
             )
         )
-        metric = 1 - skim.structural_similarity(target, shifted)
+        # data_range = 1. because we rescaled the input images to be (0., 1.0) above
+        metric = 1 - skim.structural_similarity(target, shifted, data_range=1.0)
         return metric
 
     def remove_beam_angle(self, angle: float, beam: int, modstate: int) -> np.ndarray:
         """
         Rotate a single modstate and beam's data by the beam angle.
 
         Parameters
```

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/trial_output_data.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,14 +352,17 @@
 
 
 @dataclass
 class WavelengthParameter:
     values: tuple
     wavelength: tuple = (397.0, 588.0, 630.0, 854.0)  # This must always be in order
 
+    def __hash__(self):
+        return hash((self.values, self.wavelength))
+
 
 @dataclass
 class VispTestingParameters:
     visp_beam_border: int = 1000
     visp_background_on: bool = True
     visp_background_num_spatial_bins: WavelengthParameter = WavelengthParameter(values=(1, 4, 1, 1))
     visp_background_wavelength_subsample_factor: WavelengthParameter = WavelengthParameter(
```

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_trial_output_data.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp/workflows/trial_workflows.py` & `dkist_processing_visp-2.5.0/dkist_processing_visp/workflows/trial_workflows.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.4.0rc2
+Version: 2.5.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
 Provides-Extra: test
 Provides-Extra: grogu
 Provides-Extra: docs
 
 dkist-processing-visp
 =====================
```

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
-changelog/116.feature.rst
-changelog/117.misc.rst
 dkist_processing_visp/__init__.py
 dkist_processing_visp.egg-info/PKG-INFO
 dkist_processing_visp.egg-info/SOURCES.txt
 dkist_processing_visp.egg-info/dependency_links.txt
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
```

### Comparing `dkist_processing_visp-2.4.0rc2/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.5.0/dkist_processing_visp.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-dkist-processing-common==3.0.0
-dkist-processing-math==1.0.1
-dkist-processing-pac==2.1.1
+dkist-processing-common==4.0.0
+dkist-processing-math==2.0.0
+dkist-processing-pac==3.0.0
 dkist-header-validator==3.0.5
 dkist-fits-specifications==3.6.0
-astropy==5.1.1
-numpy==1.23.1
-sunpy==4.1.4
-scipy==1.9.0
-scikit-image==0.19.3
-scikit-learn==1.2.1
+astropy==5.3.0
+numpy==1.24.3
+sunpy==5.0.0
+scipy==1.11.0
+scikit-image==0.21.0
+scikit-learn==1.2.2
 peakutils==1.3.4
-Pillow==9.2.0
+Pillow==9.5.0
 moviepy==1.0.3
 logging42==0.0.8
-dkist-spectral-lines==1.0.0
+dkist-spectral-lines==2.0.0
 
 [docs]
 sphinx
 sphinx-astropy
 sphinx-changelog==1.3.0
 sphinx-autoapi
 pytest
-towncrier==22.12.0
+towncrier
 dkist-sphinx-theme
 packaging
 
 [grogu]
-dkist==1.0.0b11
+dkist==1.0.0b14
 pyparsing
-dkist-inventory==0.16.0
-parfive<2.0.0
+dkist-inventory==0.17.0
+parfive
 
 [test]
 pytest
 pytest-cov
 pytest-xdist
 pytest-mock
 hypothesis
```

### Comparing `dkist_processing_visp-2.4.0rc2/docs/Makefile` & `dkist_processing_visp-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/background_light.rst` & `dkist_processing_visp-2.5.0/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/conf.py` & `dkist_processing_visp-2.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/gain_correction.rst` & `dkist_processing_visp-2.5.0/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.5.0/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/make.bat` & `dkist_processing_visp-2.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/polarization_calibration.rst` & `dkist_processing_visp-2.5.0/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/docs/science_calibration.rst` & `dkist_processing_visp-2.5.0/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/licenses/LICENSE.rst` & `dkist_processing_visp-2.5.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/pyproject.toml` & `dkist_processing_visp-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.4.0rc2/setup.cfg` & `dkist_processing_visp-2.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -7,60 +7,60 @@
 license = MIT
 url = https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 project_urls = 
 	Documentation = https://docs.dkist.nso.edu/projects/visp
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
-python_requires = >=3.10
+python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 3.0.0
-	dkist-processing-math == 1.0.1
-	dkist-processing-pac == 2.1.1
+	dkist-processing-common == 4.0.0
+	dkist-processing-math == 2.0.0
+	dkist-processing-pac == 3.0.0
 	dkist-header-validator == 3.0.5
 	dkist-fits-specifications == 3.6.0
-	astropy == 5.1.1
-	numpy == 1.23.1
-	sunpy == 4.1.4
-	scipy == 1.9.0
-	scikit-image == 0.19.3
-	scikit-learn == 1.2.1
+	astropy == 5.3.0
+	numpy == 1.24.3
+	sunpy == 5.0.0
+	scipy == 1.11.0
+	scikit-image == 0.21.0
+	scikit-learn == 1.2.2
 	peakutils == 1.3.4
-	Pillow == 9.2.0
+	Pillow == 9.5.0
 	moviepy == 1.0.3
 	logging42 == 0.0.8
-	dkist-spectral-lines == 1.0.0
+	dkist-spectral-lines == 2.0.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-xdist
 	pytest-mock
 	hypothesis
 	towncrier
 	dkist-data-simulator >= 2.1.0
 grogu = 
-	dkist == 1.0.0b11
+	dkist == 1.0.0b14
 	pyparsing
-	dkist-inventory == 0.16.0
-	parfive < 2.0.0
+	dkist-inventory == 0.17.0
+	parfive
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog == 1.3.0
 	sphinx-autoapi
 	pytest
-	towncrier == 22.12.0
+	towncrier
 	dkist-sphinx-theme
 	packaging
 
 [build_docs]
 source-dir = docs
 build-dir = docs/_build
 all_files = 1
```

