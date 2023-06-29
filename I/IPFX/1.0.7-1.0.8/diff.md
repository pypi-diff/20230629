# Comparing `tmp/IPFX-1.0.7.tar.gz` & `tmp/IPFX-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/IPFX-1.0.7.tar", last modified: Tue Dec  6 04:17:56 2022, max compression
+gzip compressed data, was "dist/IPFX-1.0.8.tar", last modified: Thu Jun 29 20:11:10 2023, max compression
```

## Comparing `IPFX-1.0.7.tar` & `IPFX-1.0.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/IPFX.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2337 2022-12-06 04:17:55.000000 IPFX-1.0.7/IPFX.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3596 2022-12-06 04:17:55.000000 IPFX-1.0.7/IPFX.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-12-06 04:17:55.000000 IPFX-1.0.7/IPFX.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-12-06 04:17:55.000000 IPFX-1.0.7/IPFX.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-12-06 04:17:55.000000 IPFX-1.0.7/IPFX.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/docs/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/docs/aibs_sphinx/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/docs/aibs_sphinx/static/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       58 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/arrow_off.gif
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       58 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/arrow_on.gif
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       58 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/arrow_over.gif
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    17447 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     8238 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      351 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/tab_blue.gif
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/docs/aibs_sphinx/static/style/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      401 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/style/comment.png
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      415 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/aibs_sphinx/static/style/nocomment.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6905 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/Makefile
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/authors.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10098 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/contributing.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2561 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/download_data.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1018 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/installation.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6455 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/make.bat
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1694 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/pipeline.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      819 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/quick_start.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/stimuli.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6148 2022-12-06 04:17:39.000000 IPFX-1.0.7/docs/tutorial.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/attach_metadata/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/attach_metadata/doc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10825 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/doc/design.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/attach_metadata/sink/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/sink/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2563 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/sink/dandi_yaml_sink.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3927 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/sink/metadata_sink.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8631 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/sink/nwb2_sink.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4024 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4003 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/attach_metadata/_schemas.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/bin/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      788 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/README.md
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3078 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/generate_fx_input.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1580 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/generate_pipeline_input.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3053 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/generate_qc_input.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1243 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/generate_se_input.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2048 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/get_fx_output.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2180 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/make_stimulus_ontology.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3053 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/mcc-output.json
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    40077 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/mcc_get_settings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/misc-settings.json
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    15101 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/nwb_to_pdf.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1430 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/pipeline_from_specimen_id.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4662 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/plot_ephys_nwb.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5462 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_chirp_fv_extraction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10442 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_feature_collection.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4101 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_feature_extraction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13005 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_feature_vector_extraction.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2273 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_pipeline.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3484 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_pipeline_from_nwb_file.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3030 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_qc.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2543 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_sweep_extraction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7376 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_synphys_feature_vector_extraction.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6190 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/run_x_to_nwb_conversion.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5739 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/bin/validate_experiment.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/data_release/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   179608 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_release/2020-06-26_human_file_manifest.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)  5783047 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_release/2020-06-26_mouse_file_manifest.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)    61631 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_release/20200625_patchseq_metadata_human.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)  1064422 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_release/20200625_patchseq_metadata_mouse.csv
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/dataset/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3339 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/create.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/ephys_data_interface.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13486 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/ephys_data_set.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11356 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/ephys_nwb_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/hbg_nwb_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7075 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/labnotebook.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1979 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/dataset/mies_nwb_data.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/defaults/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/defaults/qc_criteria.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21748 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/defaults/stimulus_ontology.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-06 04:17:56.000000 IPFX-1.0.7/ipfx/x_to_nwb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25754 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/ABFConverter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25499 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/DatConverter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3646 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/Readme.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5529 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/conversion_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6083 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/hr_bundle.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    48278 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/hr_nodes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11329 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/hr_segments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2263 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/hr_stimsetgenerator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6168 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/hr_struct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2182 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/x_to_nwb/hr_treenode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4922 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/_schemas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3672 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/chirp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1949 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_access.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14526 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_set_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      349 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/data_set_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      328 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/ephys_data_set.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4157 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/epochs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/error.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13087 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/feature_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3544 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/feature_record.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37419 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/feature_vectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/lab_notebook_reader.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6604 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/lims_queries.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1083 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/logging_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2496 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/nwb_append.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30207 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/plot_qc_figures.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8418 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/qc_feature_evaluator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10709 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/qc_feature_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3410 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/qc_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13877 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/script_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16570 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/spike_detector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16217 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/spike_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14671 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/spike_train_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2041 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/stim_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6014 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/stimulus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12947 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/stimulus_protocol_analysis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/string_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8195 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/subthresh_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3225 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/sweep.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/sweep_props.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2935 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/time_series_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1413 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/utilities.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-12-06 04:17:39.000000 IPFX-1.0.7/ipfx/version.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      271 2022-12-06 04:17:39.000000 IPFX-1.0.7/AUTHORS.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1999 2022-12-06 04:17:39.000000 IPFX-1.0.7/CHANGELOG.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1845 2022-12-06 04:17:39.000000 IPFX-1.0.7/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      327 2022-12-06 04:17:39.000000 IPFX-1.0.7/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1466 2022-12-06 04:17:39.000000 IPFX-1.0.7/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-12-06 04:17:39.000000 IPFX-1.0.7/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-12-06 04:17:56.000000 IPFX-1.0.7/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2491 2022-12-06 04:17:39.000000 IPFX-1.0.7/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2337 2022-12-06 04:17:56.000000 IPFX-1.0.7/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/IPFX.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2337 2023-06-29 20:11:10.000000 IPFX-1.0.8/IPFX.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3596 2023-06-29 20:11:10.000000 IPFX-1.0.8/IPFX.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-29 20:11:10.000000 IPFX-1.0.8/IPFX.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2023-06-29 20:11:10.000000 IPFX-1.0.8/IPFX.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-06-29 20:11:10.000000 IPFX-1.0.8/IPFX.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/docs/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/docs/aibs_sphinx/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/docs/aibs_sphinx/static/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       58 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/arrow_off.gif
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       58 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/arrow_on.gif
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       58 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/arrow_over.gif
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    17447 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     8238 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      351 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/tab_blue.gif
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/docs/aibs_sphinx/static/style/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      401 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/style/comment.png
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      415 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/aibs_sphinx/static/style/nocomment.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6905 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/Makefile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/authors.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10098 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/conf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/contributing.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2561 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/download_data.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/index.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1018 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/installation.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6455 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/make.bat
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1694 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/pipeline.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      819 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/quick_start.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/stimuli.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6148 2023-06-29 20:10:57.000000 IPFX-1.0.8/docs/tutorial.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/attach_metadata/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/attach_metadata/doc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10825 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/doc/design.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/attach_metadata/sink/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/sink/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2563 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/sink/dandi_yaml_sink.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3927 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/sink/metadata_sink.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8631 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/sink/nwb2_sink.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4024 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4003 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/attach_metadata/_schemas.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/bin/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      788 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/README.md
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3078 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/generate_fx_input.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1580 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/generate_pipeline_input.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3053 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/generate_qc_input.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1243 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/generate_se_input.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2048 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/get_fx_output.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2180 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/make_stimulus_ontology.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3053 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/mcc-output.json
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    40077 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/mcc_get_settings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/misc-settings.json
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    15101 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/nwb_to_pdf.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1430 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/pipeline_from_specimen_id.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4662 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/plot_ephys_nwb.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5462 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_chirp_fv_extraction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10442 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_feature_collection.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4101 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_feature_extraction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13005 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_feature_vector_extraction.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2273 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_pipeline.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3484 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_pipeline_from_nwb_file.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3030 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_qc.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2543 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_sweep_extraction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7376 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_synphys_feature_vector_extraction.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6190 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/run_x_to_nwb_conversion.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5739 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/bin/validate_experiment.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/data_release/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   179608 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_release/2020-06-26_human_file_manifest.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  5783047 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_release/2020-06-26_mouse_file_manifest.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    61631 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_release/20200625_patchseq_metadata_human.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  1064422 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_release/20200625_patchseq_metadata_mouse.csv
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/dataset/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3339 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/create.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/ephys_data_interface.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13486 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/ephys_data_set.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11250 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/ephys_nwb_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/hbg_nwb_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7075 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/labnotebook.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1979 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/dataset/mies_nwb_data.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/defaults/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/defaults/qc_criteria.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21748 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/defaults/stimulus_ontology.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:11:10.000000 IPFX-1.0.8/ipfx/x_to_nwb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25754 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/ABFConverter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25499 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/DatConverter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3646 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/Readme.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5529 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/conversion_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6083 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/hr_bundle.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48278 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/hr_nodes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11329 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/hr_segments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2263 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/hr_stimsetgenerator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6168 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/hr_struct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2182 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/x_to_nwb/hr_treenode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4922 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/_schemas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3672 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/chirp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1949 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_access.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14526 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_set_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      349 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/data_set_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      328 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/ephys_data_set.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4157 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/epochs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/error.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13087 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/feature_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3544 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/feature_record.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37419 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/feature_vectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/lab_notebook_reader.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6604 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/lims_queries.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1083 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/logging_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2496 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/nwb_append.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30207 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/plot_qc_figures.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8418 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/qc_feature_evaluator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10709 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/qc_feature_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3410 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/qc_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13877 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/script_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16570 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/spike_detector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16217 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/spike_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14671 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/spike_train_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2041 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/stim_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6014 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/stimulus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12947 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/stimulus_protocol_analysis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/string_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8195 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/subthresh_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3225 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/sweep.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/sweep_props.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2935 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/time_series_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1413 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/utilities.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-29 20:10:57.000000 IPFX-1.0.8/ipfx/version.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      271 2023-06-29 20:10:57.000000 IPFX-1.0.8/AUTHORS.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2149 2023-06-29 20:10:57.000000 IPFX-1.0.8/CHANGELOG.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1845 2023-06-29 20:10:57.000000 IPFX-1.0.8/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      327 2023-06-29 20:10:57.000000 IPFX-1.0.8/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1466 2023-06-29 20:10:57.000000 IPFX-1.0.8/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2023-06-29 20:10:57.000000 IPFX-1.0.8/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2023-06-29 20:11:10.000000 IPFX-1.0.8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2491 2023-06-29 20:10:57.000000 IPFX-1.0.8/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2337 2023-06-29 20:11:10.000000 IPFX-1.0.8/PKG-INFO
```

### Comparing `IPFX-1.0.7/IPFX.egg-info/PKG-INFO` & `IPFX-1.0.8/IPFX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFX
-Version: 1.0.7
+Version: 1.0.8
 Summary: Intrinsic Physiology Feature Extractor (IPFX) - tool for computing neuronal features from the intracellular electrophysiological recordings
 Home-page: https://github.com/AllenInstitute/ipfx
 Author: Allen Institute for Brain Science
 Author-email: Marmot@AllenInstitute.onmicrosoft.com
 License: UNKNOWN
 Keywords: neuroscience,bioinformatics,scientific
 Platform: UNKNOWN
```

### Comparing `IPFX-1.0.7/IPFX.egg-info/SOURCES.txt` & `IPFX-1.0.8/IPFX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif` & `IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif` & `IPFX-1.0.8/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/Makefile` & `IPFX-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/conf.py` & `IPFX-1.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/download_data.rst` & `IPFX-1.0.8/docs/download_data.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/index.rst` & `IPFX-1.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/installation.rst` & `IPFX-1.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/make.bat` & `IPFX-1.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/pipeline.rst` & `IPFX-1.0.8/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/quick_start.rst` & `IPFX-1.0.8/docs/quick_start.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/stimuli.rst` & `IPFX-1.0.8/docs/stimuli.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/docs/tutorial.rst` & `IPFX-1.0.8/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/attach_metadata/doc/design.md` & `IPFX-1.0.8/ipfx/attach_metadata/doc/design.md`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/attach_metadata/sink/dandi_yaml_sink.py` & `IPFX-1.0.8/ipfx/attach_metadata/sink/dandi_yaml_sink.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/attach_metadata/sink/metadata_sink.py` & `IPFX-1.0.8/ipfx/attach_metadata/sink/metadata_sink.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/attach_metadata/sink/nwb2_sink.py` & `IPFX-1.0.8/ipfx/attach_metadata/sink/nwb2_sink.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/attach_metadata/__main__.py` & `IPFX-1.0.8/ipfx/attach_metadata/__main__.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/attach_metadata/_schemas.py` & `IPFX-1.0.8/ipfx/attach_metadata/_schemas.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/README.md` & `IPFX-1.0.8/ipfx/bin/README.md`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/generate_fx_input.py` & `IPFX-1.0.8/ipfx/bin/generate_fx_input.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/generate_pipeline_input.py` & `IPFX-1.0.8/ipfx/bin/generate_pipeline_input.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/generate_qc_input.py` & `IPFX-1.0.8/ipfx/bin/generate_qc_input.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/generate_se_input.py` & `IPFX-1.0.8/ipfx/bin/generate_se_input.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/get_fx_output.py` & `IPFX-1.0.8/ipfx/bin/get_fx_output.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/make_stimulus_ontology.py` & `IPFX-1.0.8/ipfx/bin/make_stimulus_ontology.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/mcc-output.json` & `IPFX-1.0.8/ipfx/bin/mcc-output.json`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/mcc_get_settings.py` & `IPFX-1.0.8/ipfx/bin/mcc_get_settings.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/nwb_to_pdf.py` & `IPFX-1.0.8/ipfx/bin/nwb_to_pdf.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/pipeline_from_specimen_id.py` & `IPFX-1.0.8/ipfx/bin/pipeline_from_specimen_id.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/plot_ephys_nwb.py` & `IPFX-1.0.8/ipfx/bin/plot_ephys_nwb.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_chirp_fv_extraction.py` & `IPFX-1.0.8/ipfx/bin/run_chirp_fv_extraction.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_feature_collection.py` & `IPFX-1.0.8/ipfx/bin/run_feature_collection.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_feature_extraction.py` & `IPFX-1.0.8/ipfx/bin/run_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_feature_vector_extraction.py` & `IPFX-1.0.8/ipfx/bin/run_feature_vector_extraction.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_pipeline.py` & `IPFX-1.0.8/ipfx/bin/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_pipeline_from_nwb_file.py` & `IPFX-1.0.8/ipfx/bin/run_pipeline_from_nwb_file.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_qc.py` & `IPFX-1.0.8/ipfx/bin/run_qc.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_sweep_extraction.py` & `IPFX-1.0.8/ipfx/bin/run_sweep_extraction.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_synphys_feature_vector_extraction.py` & `IPFX-1.0.8/ipfx/bin/run_synphys_feature_vector_extraction.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/run_x_to_nwb_conversion.py` & `IPFX-1.0.8/ipfx/bin/run_x_to_nwb_conversion.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/bin/validate_experiment.py` & `IPFX-1.0.8/ipfx/bin/validate_experiment.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/data_release/2020-06-26_human_file_manifest.csv` & `IPFX-1.0.8/ipfx/data_release/2020-06-26_human_file_manifest.csv`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/data_release/2020-06-26_mouse_file_manifest.csv` & `IPFX-1.0.8/ipfx/data_release/2020-06-26_mouse_file_manifest.csv`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/data_release/20200625_patchseq_metadata_human.csv` & `IPFX-1.0.8/ipfx/data_release/20200625_patchseq_metadata_human.csv`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/data_release/20200625_patchseq_metadata_mouse.csv` & `IPFX-1.0.8/ipfx/data_release/20200625_patchseq_metadata_mouse.csv`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/dataset/create.py` & `IPFX-1.0.8/ipfx/dataset/create.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/dataset/ephys_data_interface.py` & `IPFX-1.0.8/ipfx/dataset/ephys_data_interface.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/dataset/ephys_data_set.py` & `IPFX-1.0.8/ipfx/dataset/ephys_data_set.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/dataset/ephys_nwb_data.py` & `IPFX-1.0.8/ipfx/dataset/ephys_nwb_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,55 +143,53 @@
         ):
             raise TypeError(
                 f"Sweep_number must be an integer, but it is {type(sweep_number)}"
             )
 
         series = self.nwb.sweep_table.get_series(sweep_number)
 
-        if series is None:
+        if not series:
             raise ValueError(
                 f"No TimeSeries found for sweep number {sweep_number}."
             )
 
         matching_series = []
 
-        # Look for instances of stimulus or response PatchCLampSeries
+        # Look for instances of matching series types PatchCLampSeries
         for s in series:
             if isinstance(s, series_class):
                 matching_series.append(s)
 
         # check how many series we have to make sure we only got 1 TimeSeries
         num_series = len(matching_series)
         if num_series == 1:
             return matching_series[0]
         else:
-            # check series type so we can display an appropriate error
-
-            if isinstance(series_class, self.STIMULUS):
+            # simplify series class to stimulus or response for error messages
+            if series_class == self.STIMULUS:
                 series_name = "stimulus"
-            elif isinstance(series_class, self.RESPONSE):
+            elif series_class == self.RESPONSE:
                 series_name = "response"
             else:
-                raise TypeError(
-                    f"{type(series_class)} is not a stimulus or response PatchClampSeries"
-                )
+                # Unknown series categorization so don't simplify
+                series_name = series_class
 
-            if num_series == 0:
+            if num_series > 1:
                 raise ValueError(
-                    f"Could not find any {series_name} PatchClampSeries "
+                    f"Found {num_series} {series_name} PatchClampSeries "
+                    f"{[s.name for s in matching_series]} "
                     f"for sweep number {sweep_number}."
                 )
             else:
-                # check how many matching series we have
                 raise ValueError(
-                    f"Found {num_series} {series_name} PatchClampSeries "
-                    f"{[s.name for s in matching_series]} "
+                    f"Could not find any {series_name} PatchClampSeries "
                     f"for sweep number {sweep_number}."
                 )
 
+
     def get_sweep_data(
         self, sweep_number: int
     ) -> Dict[str, Union[np.ndarray, str, float]]:
         """Extracts numpy arrays, stimulus unit, and sampling rate from sweep.
 
         Grabs stimulus and response PatchClampSeries and extracts numpy arrays
         for the stimulus and response time series data as well as the stimulus
```

### Comparing `IPFX-1.0.7/ipfx/dataset/hbg_nwb_data.py` & `IPFX-1.0.8/ipfx/dataset/hbg_nwb_data.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/dataset/labnotebook.py` & `IPFX-1.0.8/ipfx/dataset/labnotebook.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/dataset/mies_nwb_data.py` & `IPFX-1.0.8/ipfx/dataset/mies_nwb_data.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/defaults/qc_criteria.json` & `IPFX-1.0.8/ipfx/defaults/qc_criteria.json`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/defaults/stimulus_ontology.json` & `IPFX-1.0.8/ipfx/defaults/stimulus_ontology.json`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/ABFConverter.py` & `IPFX-1.0.8/ipfx/x_to_nwb/ABFConverter.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/DatConverter.py` & `IPFX-1.0.8/ipfx/x_to_nwb/DatConverter.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/Readme.md` & `IPFX-1.0.8/ipfx/x_to_nwb/Readme.md`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/conversion_utils.py` & `IPFX-1.0.8/ipfx/x_to_nwb/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/hr_bundle.py` & `IPFX-1.0.8/ipfx/x_to_nwb/hr_bundle.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/hr_nodes.py` & `IPFX-1.0.8/ipfx/x_to_nwb/hr_nodes.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/hr_segments.py` & `IPFX-1.0.8/ipfx/x_to_nwb/hr_segments.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/hr_stimsetgenerator.py` & `IPFX-1.0.8/ipfx/x_to_nwb/hr_stimsetgenerator.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/hr_struct.py` & `IPFX-1.0.8/ipfx/x_to_nwb/hr_struct.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/x_to_nwb/hr_treenode.py` & `IPFX-1.0.8/ipfx/x_to_nwb/hr_treenode.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/_schemas.py` & `IPFX-1.0.8/ipfx/_schemas.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/chirp.py` & `IPFX-1.0.8/ipfx/chirp.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/data_access.py` & `IPFX-1.0.8/ipfx/data_access.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/data_set_features.py` & `IPFX-1.0.8/ipfx/data_set_features.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/epochs.py` & `IPFX-1.0.8/ipfx/epochs.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/feature_extractor.py` & `IPFX-1.0.8/ipfx/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/feature_record.py` & `IPFX-1.0.8/ipfx/feature_record.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/feature_vectors.py` & `IPFX-1.0.8/ipfx/feature_vectors.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/lims_queries.py` & `IPFX-1.0.8/ipfx/lims_queries.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/logging_utils.py` & `IPFX-1.0.8/ipfx/logging_utils.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/nwb_append.py` & `IPFX-1.0.8/ipfx/nwb_append.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/plot_qc_figures.py` & `IPFX-1.0.8/ipfx/plot_qc_figures.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/qc_feature_evaluator.py` & `IPFX-1.0.8/ipfx/qc_feature_evaluator.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/qc_feature_extractor.py` & `IPFX-1.0.8/ipfx/qc_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/qc_features.py` & `IPFX-1.0.8/ipfx/qc_features.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/script_utils.py` & `IPFX-1.0.8/ipfx/script_utils.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/spike_detector.py` & `IPFX-1.0.8/ipfx/spike_detector.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/spike_features.py` & `IPFX-1.0.8/ipfx/spike_features.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/spike_train_features.py` & `IPFX-1.0.8/ipfx/spike_train_features.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/stim_features.py` & `IPFX-1.0.8/ipfx/stim_features.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/stimulus.py` & `IPFX-1.0.8/ipfx/stimulus.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/stimulus_protocol_analysis.py` & `IPFX-1.0.8/ipfx/stimulus_protocol_analysis.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/subthresh_features.py` & `IPFX-1.0.8/ipfx/subthresh_features.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/sweep.py` & `IPFX-1.0.8/ipfx/sweep.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/sweep_props.py` & `IPFX-1.0.8/ipfx/sweep_props.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/time_series_utils.py` & `IPFX-1.0.8/ipfx/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/ipfx/utilities.py` & `IPFX-1.0.8/ipfx/utilities.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/CHANGELOG.md` & `IPFX-1.0.8/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 ## Unreleased
 
 ### Added
 
 ### Changed
 
+## [1.0.8] = 2023-06-29
+Changed:
+- Fixed an error that was obscuring underlying errors when trying to _get_series information for a PatchClampSeries
+
 ## [1.0.7] = 2022-12-5
 Changed:
 - Added StimulusType and STIMULUS_TYPE_NAME_MAPPING to stimulus ontology, replacing definitions in EphysDataset
 - Updated data_set_features to use correct sweep feature extractor detection parameters based on StimulusType
 
 ## [1.0.6] = 2022-6-29
 Changed:
```

### Comparing `IPFX-1.0.7/LICENSE` & `IPFX-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/README.md` & `IPFX-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/setup.py` & `IPFX-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `IPFX-1.0.7/PKG-INFO` & `IPFX-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFX
-Version: 1.0.7
+Version: 1.0.8
 Summary: Intrinsic Physiology Feature Extractor (IPFX) - tool for computing neuronal features from the intracellular electrophysiological recordings
 Home-page: https://github.com/AllenInstitute/ipfx
 Author: Allen Institute for Brain Science
 Author-email: Marmot@AllenInstitute.onmicrosoft.com
 License: UNKNOWN
 Keywords: neuroscience,bioinformatics,scientific
 Platform: UNKNOWN
```

