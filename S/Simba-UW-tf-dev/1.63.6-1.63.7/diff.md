# Comparing `tmp/Simba-UW-tf-dev-1.63.6.tar.gz` & `tmp/Simba-UW-tf-dev-1.63.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.6.tar", last modified: Tue Jun 20 19:04:54 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.7.tar", last modified: Thu Jun 29 19:37:39 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.63.6.tar` & `Simba-UW-tf-dev-1.63.7.tar`

### file list

```diff
@@ -1,559 +1,581 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.6/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.6/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.63.6/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.6/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.6/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.6/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20696 2023-06-20 18:57:14.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.6/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.6/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-20 18:30:33.000000 Simba-UW-tf-dev-1.63.6/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.6/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 18:25:39.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.63.6/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.63.6/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.63.6/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-20 18:25:39.000000 Simba-UW-tf-dev-1.63.6/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7601 2023-06-18 18:58:51.000000 Simba-UW-tf-dev-1.63.6/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.6/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.63.6/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.63.6/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.6/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.6/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.6/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.6/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.6/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.6/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.6/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.6/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.6/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.6/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.6/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 18:25:39.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.6/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.6/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.6/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.6/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.6/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.6/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.6/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.6/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66068 2023-06-20 18:58:45.000000 Simba-UW-tf-dev-1.63.6/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-17 18:48:05.000000 Simba-UW-tf-dev-1.63.6/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.6/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.6/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.6/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.6/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    20508 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-20 19:04:53.000000 Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.6/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.6/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.6/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.6/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.6/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.6/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.6/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.6/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.6/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.6/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.6/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.6/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.6/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.6/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.6/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.6/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.6/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.6/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.6/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.6/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-20 19:04:52.000000 Simba-UW-tf-dev-1.63.6/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-20 19:04:54.000000 Simba-UW-tf-dev-1.63.6/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9020 2023-06-29 01:16:45.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3599 2023-06-29 19:35:48.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.7/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.7/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.63.7/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.7/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.7/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.7/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-26 17:54:54.000000 Simba-UW-tf-dev-1.63.7/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    16349 2023-06-29 19:29:12.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.7/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.63.7/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.63.7/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7601 2023-06-18 18:58:51.000000 Simba-UW-tf-dev-1.63.7/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.7/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43313 2023-06-27 15:38:38.000000 Simba-UW-tf-dev-1.63.7/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.63.7/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.7/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.7/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.7/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.7/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.7/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.7/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.7/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.7/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.7/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.7/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.7/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.7/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.7/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.7/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/ui/define_px_to_mm_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66068 2023-06-20 18:58:45.000000 Simba-UW-tf-dev-1.63.7/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    21589 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.7/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.7/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.7/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.7/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.7/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.7/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.7/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.7/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.7/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.7/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.7/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.7/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.7/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.7/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.7/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.7/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.7/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.7/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.7/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.7/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-29 19:37:32.000000 Simba-UW-tf-dev-1.63.7/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.63.6/PKG-INFO` & `Simba-UW-tf-dev-1.63.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.6
+Version: 1.63.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/ui/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -253,20 +253,20 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000c 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0002 a412 0000 000b 005f 005f 0070  ..........._._.p
+00001030: 0000 0002 a413 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 2c2b 9e29  moDDblob....,+.)
-00001060: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 9a7e 9921  moDDblob.....~.!
+00001060: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 2c2b 9e29 7b20  dDblob....,+.){ 
+00001080: 6444 626c 6f62 0000 0008 9a7e 9921 1721  dDblob.....~.!.!
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000010b0: 636f 6d70 0000 0000 0003 3000 0000 0007  comp......0.....
 000010c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
 000010d0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
 000010e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000010f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from simba.feature_extractors.feature_subsets import FeatureSubsetsCalculator
 
 
 
 class FeatureSubsetExtractorPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
-        PopUpMixin.__init__(self, title='EXTRACT FEATURE SUBSETS')
+
+        PopUpMixin.__init__(self, title='EXTRACT FEATURE SUBSETS', size=(500, 100))
         ConfigReader.__init__(self, config_path=config_path)
         self.feature_subset_options = ['Two-point body-part distances (mm)',
                                        'Within-animal three-point body-part angles (degrees)',
                                        'Within-animal three-point convex hull perimeters (mm)',
                                        'Within-animal four-point convex hull perimeters (mm)',
                                        'Entire animal convex hull perimeters (mm)',
                                        'Entire animal convex hull area (mm2)',
@@ -26,21 +27,30 @@
                                        'Frame-by-frame distance to ROI centers (mm)',
                                        'Frame-by-frame body-parts inside ROIs (Boolean)']
 
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name='documentation', icon_link=Links.FEATURE_SUBSETS.value)
         self.feature_family_dropdown = DropDownMenu(self.settings_frm, 'FEATURE FAMILY:', self.feature_subset_options, '20')
         self.feature_family_dropdown.setChoices(self.feature_subset_options[0])
         self.save_dir = FolderSelect(self.settings_frm, 'SAVE DIRECTORY:', lblwidth=20)
+        self.append_to_features_extracted_var = BooleanVar(value=False)
+        self.append_to_targets_inserted_var = BooleanVar(value=False)
+        self.append_to_features_cb = Checkbutton(self.settings_frm, text='APPEND RESULTS TO FEATURES EXTRACTED FILES', variable=self.append_to_features_extracted_var)
+        self.append_to_targets_inserted_cb = Checkbutton(self.settings_frm, text='APPEND RESULTS TO TARGET INSERTED FILES', variable=self.append_to_targets_inserted_var)
         self.create_run_frm(run_function=self.run)
-
         self.settings_frm.grid(row=0, column=0, sticky=NW)
         self.feature_family_dropdown.grid(row=0, column=0, sticky=NW)
         self.save_dir.grid(row=1, column=0, sticky=NW)
-
+        self.append_to_features_cb.grid(row=2, column=0, sticky=NW)
+        self.append_to_targets_inserted_cb.grid(row=3, column=0, sticky=NW)
         #self.main_frm.mainloop()
 
     def run(self):
         check_if_dir_exists(in_dir=self.save_dir.folder_path)
         feature_extractor = FeatureSubsetsCalculator(config_path=self.config_path,
                                                      feature_family=self.feature_family_dropdown.getChoices(),
-                                                     save_dir=self.save_dir.folder_path)
-        feature_extractor.run()
+                                                     save_dir=self.save_dir.folder_path,
+                                                     append_to_features_extracted=self.append_to_targets_inserted_var.get(),
+                                                     append_to_targets_inserted=self.append_to_targets_inserted_var.get())
+        feature_extractor.run()
+
+
+#FeatureSubsetExtractorPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.63.7/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/labelling/.DS_Store`

 * *Files 13% similar despite different names*

```diff
@@ -44,20 +44,20 @@
 000002b0: 0062 0065 006c 006c 0069 006e 0067 002f  .b.e.l.l.i.n.g./
 000002c0: 0000 000b 005f 005f 0069 006e 0069 0074  ....._._.i.n.i.t
 000002d0: 005f 005f 002e 0070 0079 7074 624e 7573  ._._...p.yptbNus
 000002e0: 7472 0000 000b 005f 005f 0069 006e 0069  tr....._._.i.n.i
 000002f0: 0074 005f 005f 002e 0070 0079 0000 000b  .t._._...p.y....
 00000300: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000310: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000320: 0000 0001 d1b3 0000 000b 005f 005f 0070  ..........._._.p
+00000320: 0000 0001 d257 0000 000b 005f 005f 0070  .....W....._._.p
 00000330: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000340: 6d6f 4444 626c 6f62 0000 0008 d69d 9c29  moDDblob.......)
-00000350: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+00000340: 6d6f 4444 626c 6f62 0000 0008 2f24 1c69  moDDblob..../$.i
+00000350: 4422 c541 0000 000b 005f 005f 0070 0079  D".A....._._.p.y
 00000360: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000370: 6444 626c 6f62 0000 0008 d69d 9c29 7b20  dDblob.......){ 
+00000370: 6444 626c 6f62 0000 0008 2f24 1c69 4422  dDblob..../$.iD"
 00000380: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00000390: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000003a0: 636f 6d70 0000 0000 0002 2000 0000 0000  comp...... .....
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 except ImportError:
     from typing_extensions import Literal
 
 
 from simba.utils.errors import FrameRangeError
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_config_entry, read_df, write_df, get_fn_ext, get_video_meta_data, get_all_clf_names
-from simba.utils.checks import check_file_exist_and_readable, check_int, check_float
+from simba.utils.checks import check_file_exist_and_readable, check_int, check_float, check_that_column_exist
 from simba.utils.printing import stdout_success
 import simba
 
 class LabellingInterface(ConfigReader):
     """
     Launch ``standard`` or ``pseudo``-labelling (annotation) GUI interface in SimBA.
 
@@ -87,15 +87,18 @@
             elif setting == 'pseudo':
                 check_file_exist_and_readable(file_path=self.machine_results_file_path)
                 self.data_df = read_df(self.machine_results_file_path, self.file_type)
                 for target in self.target_lst:
                     self.data_df.loc[self.data_df['Probability_{}'.format(target)] > self.threshold_dict[target], target] = 1
                     self.data_df.loc[self.data_df['Probability_{}'.format(target)] <= self.threshold_dict[target], target] = 0
                 self.main_window.title('SIMBA ANNOTATION INTERFACE (PSEUDO-LABELLING) - {}'.format(self.video_name))
-        self.data_df_targets = self.data_df[self.target_lst]
+        self.data_df_targets = self.data_df
+        for target in self.target_lst:
+            check_that_column_exist(df=self.data_df_targets, column_name=target, file_name=file_path)
+        self.data_df_targets = self.data_df_targets[self.target_lst]
         self.folder = Frame(self.main_window)
         self.buttons_frm = Frame(self.main_window, bd=2, width=700, height=300)
         self.current_frm_n = IntVar(self.main_window, value=self.frm_no)
         self.change_frm_box = Entry(self.buttons_frm, width=7, textvariable=self.current_frm_n)
         self.frame_number_lbl = Label(self.buttons_frm, text="Frame number")
         self.forward_btn = Button(self.buttons_frm, text=">", command=lambda: self.__advance_frame(new_frm_number=int(self.current_frm_n.get() + 1)))
         self.backward_btn = Button(self.buttons_frm, text="<", command=lambda: self.__advance_frame(new_frm_number=int(self.current_frm_n.get() - 1)))
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.63.7/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.63.7/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 300c 0000 100b 0000 400c  ......0.......@.
 00000020: 0000 500c 0000 0000 0000 0000 0000 0800  ..P.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 000a 0000 0002 0000 00ba  ................
+00000040: 0000 0000 0000 000a 0000 0002 0000 00be  ................
 00000050: 0000 000c 0000 1000 006f 0074 0074 0069  .........o.t.t.i
 00000060: 006e 0067 0000 0000 0000 0000 0000 0000  .n.g............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -113,24 +113,24 @@
 00000700: 7801 7a01 7b01 8101 8a01 8b01 8d01 8e01  x.z.{...........
 00000710: 9601 9f01 a001 a301 a401 ad01 b601 b701  ................
 00000720: b901 ba01 c901 d201 d301 d401 de01 e701  ................
 00000730: ef01 f501 ff02 0002 0202 0302 0e02 1702  ................
 00000740: 1802 1902 2b02 3402 3502 3602 4902 4a02  ....+.4.5.6.I.J.
 00000750: 5302 5c02 6502 6a02 6b00 0000 0000 0002  S.\.e.j.k.......
 00000760: 0100 0000 0000 0000 5e00 0000 0000 0000  ........^.......
-00000770: 0000 0000 0000 0002 6dee 00f7 00f8 00fa  ........m.......
-00000780: 00fb 0108 0111 011d 011e 011f 0128 012d  .............(.-
-00000790: 012f 0130 0131 013a 013f 0141 0142 0143  ./.0.1.:.?.A.B.C
-000007a0: 014c 0152 0154 0155 0156 015f 0167 0169  .L.R.T.U.V._.g.i
-000007b0: 016a 016b 0174 017d 0180 0181 0182 018b  .j.k.t.}........
-000007c0: 019a 019c 019d 019e 01a7 01b1 01b2 01b3  ................
-000007d0: 01b4 01bd 01ca 01cb 0000 0000 0000 0201  ................
-000007e0: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
-000007f0: 0000 0000 0000 01cd 0000 000c 0075 006e  .............u.n
-00000800: 0073 0075 0000 0001 0000 0000 0000 080b  .s.u............
+00000770: 0000 0000 0000 0002 6d3c 0050 0059 0064  ........m<.P.Y.d
+00000780: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
+00000790: 00c6 00ce 00d3 00d6 00d7 00d8 00e1 00ea  ................
+000007a0: 00ec 00ed 00ee 00f7 00f8 00fa 00fb 0108  ................
+000007b0: 0111 011d 011e 011f 0128 012d 012f 0130  .........(.-./.0
+000007c0: 0131 013a 013f 0141 0142 0143 014c 0152  .1.:.?.A.B.C.L.R
+000007d0: 0154 0155 0156 015f 0167 0169 016a 016b  .T.U.V._.g.i.j.k
+000007e0: 0174 017d 0180 0181 0182 018b 019a 019c  .t.}............
+000007f0: 019d 019e 01a7 01b1 01b2 01b3 01b4 01bd  ................
+00000800: 01ca 01cb 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -334,18 +334,18 @@
 000014d0: 2901 2b01 2c01 2d01 3601 3801 3901 3a01  ).+.,.-.6.8.9.:.
 000014e0: 4301 4501 4601 4701 5001 5201 5401 5501  C.E.F.G.P.R.T.U.
 000014f0: 5601 5f01 6101 6301 6401 6501 6e01 7001  V._.a.c.d.e.n.p.
 00001500: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
 00001510: 8c01 8e01 9101 9201 9301 9401 9d01 a201  ................
 00001520: ab00 0000 0000 0002 0100 0000 0000 0000  ................
 00001530: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-00001540: ac00 0000 0c00 0000 0200 7500 6976 5372  ..........u.ivSr
-00001550: 6e6c 6f6e 6700 0000 0100 0000 0d00 0000  nlong...........
-00001560: 0500 7500 7400 6900 6c00 7364 7363 6c62  ..u.t.i.l.sdsclb
-00001570: 6f6f 6c00 0000 0000 0000 0000 0000 0000  ool.............
+00001540: ac00 0000 0c00 0000 0200 7500 696d 6f64  ..........u.imod
+00001550: 4462 6c6f 6200 0000 087e abce 1cd0 1fc5  Dblob....~......
+00001560: 4100 0000 0d00 0000 0500 7500 7400 6900  A.........u.t.i.
+00001570: 6c00 7364 7363 6c62 6f6f 6c00 0000 0000  l.sdsclbool.....
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,64 +457,64 @@
 00001c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 00001c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 00001ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 00001cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 00001cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 00001cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 00001ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00001cf0: 0074 6543 7265 6174 6564 5473 697a 6555  .teCreatedTsizeU
-00001d00: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001d10: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
-00001d20: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00001d30: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-00001d40: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
-00001d50: c808 1008 d419 1718 1624 250a 0a10 0110  .........$%.....
-00001d60: b509 09d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
-00001d70: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
-00001d80: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
-00001d90: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
-00001da0: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
-00001db0: 190a 420a 4409 1101 c709 1000 0823 4028  ..B.D........#@(
-00001dc0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
-00001dd0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
-00001de0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
-00001df0: 00c1 00ce 00da 00df 00e5 00ea 00f2 00f7  ................
-00001e00: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
-00001e10: 0125 012e 012f 0131 0132 0134 013d 013f  .%.../.1.2.4.=.?
-00001e20: 0141 0142 0143 014c 014d 014e 0150 0159  .A.B.C.L.M.N.P.Y
-00001e30: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
-00001e40: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
-00001e50: 0189 018a 018c 0195 0196 0199 019a 019c  ................
-00001e60: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
-00001e70: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
-00001e80: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
-00001e90: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00001ea0: 0064 6d6f 4444 626c 6f62 0000 0008 cbf3  .dmoDDblob......
-00001eb0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
-00001ec0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00001ed0: 0064 6d6f 6444 626c 6f62 0000 0008 cbf3  .dmodDblob......
-00001ee0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
-00001ef0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00001f00: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
-00001f10: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
-00001f20: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
-00001f30: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
-00001f40: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
-00001f50: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00001f60: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00001f70: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00001f80: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00001f90: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00001fa0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00001fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00001fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00001fd0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
-00001fe0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
-00001ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-00002000: 0000 0001 0000 0007 0000 0003 0000 0004  ................
+00001cf0: 0031 363b 4058 636f 6d6d 656e 7473 5e64  .16;@Xcomments^d
+00001d00: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+00001d10: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+00001d20: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+00001d30: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+00001d40: 616d 65d4 1617 1819 1a1b 0a1d 5776 6973  ame.........Wvis
+00001d50: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00001d60: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+00001d70: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
+00001d80: d419 1718 1624 250a 0a10 0110 b509 09d4  .....$%.........
+00001d90: 1617 1819 1a25 1a2b 0808 1002 d416 1718  .....%.+........
+00001da0: 190a 2e1a 3009 1061 0810 03d4 1617 1819  ....0..a........
+00001db0: 1a33 0a35 0810 6409 1005 d416 1718 190a  .3.5..d.........
+00001dc0: 380a 3a09 1073 0910 04d4 1617 1819 1a3d  8.:..s.........=
+00001dd0: 0a3f 0810 4b09 1006 d416 1718 190a 420a  .?..K.........B.
+00001de0: 4409 1101 c709 1000 0823 4028 0000 0000  D........#@(....
+00001df0: 0000 5c64 6174 654d 6f64 6966 6965 6409  ..\dateModified.
+00001e00: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+00001e10: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
+00001e20: 00da 00df 00e5 00ea 00f2 00f7 0100 0108  ................
+00001e30: 010e 0118 011e 011f 0122 0123 0125 012e  .........".#.%..
+00001e40: 012f 0131 0132 0134 013d 013f 0141 0142  ./.1.2.4.=.?.A.B
+00001e50: 0143 014c 014d 014e 0150 0159 015a 015c  .C.L.M.N.P.Y.Z.\
+00001e60: 015d 015f 0168 0169 016b 016c 016e 0177  .]._.h.i.k.l.n.w
+00001e70: 0178 017a 017b 017d 0186 0187 0189 018a  .x.z.{.}........
+00001e80: 018c 0195 0196 0199 019a 019c 019d 01a6  ................
+00001e90: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
+00001ea0: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+00001eb0: 01b4 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+00001ec0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
+00001ed0: 4444 626c 6f62 0000 0008 cbf3 6409 d917  DDblob......d...
+00001ee0: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
+00001ef0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
+00001f00: 6444 626c 6f62 0000 0008 cbf3 6409 d917  dDblob......d...
+00001f10: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
+00001f20: 0065 0072 0076 0069 0073 0065 0064 7068  .e.r.v.i.s.e.dph
+00001f30: 3153 636f 6d70 0000 0000 0004 d000 0000  1Scomp..........
+00001f40: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+00001f50: 0076 0069 0073 0065 0064 7653 726e 6c6f  .v.i.s.e.dvSrnlo
+00001f60: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
+00001f70: 006c 0073 6277 7370 626c 6f62 0000 00c9  .l.sbwspblob....
+00001f80: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00001f90: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+00001fa0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00001fb0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00001fc0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00001fd0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00001fe0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00001ff0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+00002000: 187b 7b32 0000 0007 0000 0003 0000 0004  .{{2............
 00002010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
 00002020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
 00002030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
 00002040: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
 00002050: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
 00002060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00002070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
@@ -764,15 +764,15 @@
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003000: 0000 0000 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0008 6972 0000 0005 0075  mp......ir.....u
+00003020: 6d70 0000 0000 0008 6b70 0000 0005 0075  mp......kp.....u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,18 +848,18 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 0862 b162  smoDDblob....b.b
-00003570: fcec 20c5 4100 0000 0500 7500 7400 6900  .. .A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 0862  l.smodDblob....b
-00003590: b162 fcec 20c5 4100 0000 0500 7500 7400  .b.. .A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 083a fcc1  smoDDblob....:..
+00003570: 5480 22c5 4100 0000 0500 7500 7400 6900  T.".A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 083a  l.smodDblob....:
+00003590: fcc1 5480 22c5 4100 0000 0500 7500 7400  ..T.".A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
 000035b0: 0000 09f0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
@@ -1035,229 +1035,229 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0002  ._lg1Scomp......
-00004110: 5c61 0000 000b 005f 005f 0070 0079 0063  \a....._._.p.y.c
+00004110: 5c68 0000 000b 005f 005f 0070 0079 0063  \h....._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 cf1a a440 ee20 c541  blob.......@. .A
+00004130: 626c 6f62 0000 0008 fef2 7934 1721 c541  blob......y4.!.A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 cf1a a440 ee20 c541 0000  ob.......@. .A..
+00004160: 6f62 0000 0008 fef2 7934 1721 c541 0000  ob......y4.!.A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0002 a000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
-000041b0: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+000041b0: 0000 00b5 6270 6c69 7374 3030 d601 0203  ....bplist00....
 000041c0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 000041d0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 000041e0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 000041f0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00004200: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00004210: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00004220: 0908 095f 1018 7b7b 3637 302c 2033 3939  ..._..{{670, 399
-00004230: 7d2c 207b 3737 302c 2034 3336 7d7d 0908  }, {770, 436}}..
-00004240: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00004250: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00004260: 0000 0000 0000 0000 0000 008b 0000 0006  ................
-00004270: 0061 0073 0073 0065 0074 0073 6c67 3153  .a.s.s.e.t.slg1S
-00004280: 636f 6d70 0000 0000 007d db93 0000 0006  comp.....}......
-00004290: 0061 0073 0073 0065 0074 0073 6c73 7643  .a.s.s.e.t.slsvC
-000042a0: 626c 6f62 0000 02b0 6270 6c69 7374 3030  blob....bplist00
-000042b0: da01 0203 0405 0607 0809 0a0b 0c0d 1a48  ...............H
-000042c0: 4948 4a0c 4c58 6963 6f6e 5369 7a65 5f10  IHJ.LXiconSize_.
-000042d0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-000042e0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-000042f0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00004300: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00004310: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-00004320: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-00004330: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-00004340: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
-00004350: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
-00004360: 0000 0000 0009 ab0e 171c 2125 2a2f 3439  ..........!%*/49
-00004370: 3e43 d40f 1011 1213 140c 0c5a 6964 656e  >C.........Ziden
-00004380: 7469 6669 6572 5577 6964 7468 5961 7363  tifierUwidthYasc
-00004390: 656e 6469 6e67 5776 6973 6962 6c65 546e  endingWvisibleTn
-000043a0: 616d 6511 01c7 0909 d40f 1011 1218 191a  ame.............
-000043b0: 1a58 7562 6971 7569 7479 1023 0808 d40f  .Xubiquity.#....
-000043c0: 1011 121d 1e1a 0c5c 6461 7465 4d6f 6469  .......\dateModi
-000043d0: 6669 6564 10b5 0809 d40f 1011 1222 1e1a  fied........."..
-000043e0: 1a5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
-000043f0: 0f10 1112 2627 1a0c 5473 697a 6510 6108  ....&'..Tsize.a.
-00004400: 09d4 0f10 1112 2b2c 0c0c 546b 696e 6410  ......+,..Tkind.
-00004410: 7309 09d4 0f10 1112 3031 0c1a 556c 6162  s.......01..Ulab
-00004420: 656c 1064 0908 d40f 1011 1235 360c 1a57  el.d.......56..W
-00004430: 7665 7273 696f 6e10 4b09 08d4 0f10 1112  version.K.......
-00004440: 3a3b 0c1a 5863 6f6d 6d65 6e74 7311 012c  :;..Xcomments..,
-00004450: 0908 d40f 1011 123f 401a 1a5e 6461 7465  .......?@..^date
-00004460: 4c61 7374 4f70 656e 6564 10c8 0808 d40f  LastOpened......
-00004470: 1011 1244 1e1a 1a59 6461 7465 4164 6465  ...D...YdateAdde
-00004480: 6408 0808 2300 0000 0000 0000 0023 4028  d...#........#@(
-00004490: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
-000044a0: 001d 0026 0038 0040 0054 0066 006f 0081  ...&.8.@.T.f.o..
-000044b0: 008c 009f 00b4 00bd 00be 00ca 00d3 00de  ................
-000044c0: 00e4 00ee 00f6 00fb 00fe 00ff 0100 0109  ................
-000044d0: 0112 0114 0115 0116 011f 012c 012e 012f  ...........,.../
-000044e0: 0130 0139 0145 0146 0147 0150 0155 0157  .0.9.E.F.G.P.U.W
-000044f0: 0158 0159 0162 0167 0169 016a 016b 0174  .X.Y.b.g.i.j.k.t
-00004500: 017a 017c 017d 017e 0187 018f 0191 0192  .z.|.}.~........
-00004510: 0193 019c 01a5 01a8 01a9 01aa 01b3 01c2  ................
-00004520: 01c4 01c5 01c6 01cf 01d9 01da 01db 01dc  ................
-00004530: 01e5 01ee 01f3 01f4 0000 0000 0000 0201  ................
-00004540: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-00004550: 0000 0000 0000 01f6 0000 0006 0061 0073  .............a.s
-00004560: 0073 0065 0074 0073 6c73 7670 626c 6f62  .s.e.t.slsvpblob
-00004570: 0000 0295 6270 6c69 7374 3030 da01 0203  ....bplist00....
-00004580: 0405 0607 0809 0a0b 0c0d 1c48 4948 4a0c  ...........HIHJ.
-00004590: 2958 6963 6f6e 5369 7a65 5f10 0f73 686f  )XiconSize_..sho
-000045a0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-000045b0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-000045c0: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-000045d0: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-000045e0: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-000045f0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00004600: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00004610: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00004620: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00004630: 0009 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
-00004640: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
-00004650: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-00004660: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-00004670: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00004680: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00004690: 616d 65d4 1819 1a1b 1c1d 0c1f 5776 6973  ame.........Wvis
-000046a0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-000046b0: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-000046c0: 07d4 1819 1a1b 1c22 1c24 0810 c808 1008  .......".$......
-000046d0: d418 191a 1b0c 271c 2909 10b5 0810 01d4  ......'.).......
-000046e0: 1819 1a1b 1c27 1c2d 0808 1002 d418 191a  .....'.-........
-000046f0: 1b0c 301c 3209 1061 0810 03d4 1819 1a1b  ..0.2..a........
-00004700: 1c35 0c37 0810 6409 1005 d418 191a 1b0c  .5.7..d.........
-00004710: 3a0c 3c09 1073 0910 04d4 1819 1a1b 1c3f  :.<..s.........?
-00004720: 0c41 0810 4b09 1006 d418 191a 1b0c 440c  .A..K.........D.
-00004730: 4609 1101 c709 1000 0823 0000 0000 0000  F........#......
-00004740: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
-00004750: 0900 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
-00004760: 6f00 8100 8c00 9f00 b400 bd00 be00 d100  o...............
-00004770: da00 e900 f601 0201 0701 0d01 1201 1a01  ................
-00004780: 1f01 2801 3001 3601 4001 4601 4701 4a01  ..(.0.6.@.F.G.J.
-00004790: 4b01 4d01 5601 5701 5901 5a01 5c01 6501  K.M.V.W.Y.Z.\.e.
-000047a0: 6601 6801 6901 6b01 7401 7501 7601 7801  f.h.i.k.t.u.v.x.
-000047b0: 8101 8201 8401 8501 8701 9001 9101 9301  ................
-000047c0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
-000047d0: af01 b101 b201 b401 bd01 be01 c101 c201  ................
-000047e0: c401 c501 ce01 d701 dc00 0000 0000 0002  ................
-000047f0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
-00004800: 0000 0000 0000 0001 dd00 0000 0600 6100  ..............a.
-00004810: 7300 7300 6500 7400 736d 6f44 4462 6c6f  s.s.e.t.smoDDblo
-00004820: 6200 0000 08cf 958c e8d0 e1c4 4100 0000  b...........A...
-00004830: 0600 6100 7300 7300 6500 7400 736d 6f64  ..a.s.s.e.t.smod
-00004840: 4462 6c6f 6200 0000 08cf 958c e8d0 e1c4  Dblob...........
-00004850: 4100 0000 0600 6100 7300 7300 6500 7400  A.....a.s.s.e.t.
-00004860: 7370 6831 5363 6f6d 7000 0000 0000 81a0  sph1Scomp.......
-00004870: 0000 0000 0600 6100 7300 7300 6500 7400  ......a.s.s.e.t.
-00004880: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
-00004890: 0c00 6200 6c00 6f00 6200 5f00 7300 7400  ..b.l.o.b._.s.t.
-000048a0: 6f00 7200 6100 6700 6562 7773 7062 6c6f  o.r.a.g.ebwspblo
-000048b0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
-000048c0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-000048d0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-000048e0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-000048f0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00004900: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00004910: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-00004920: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00004930: 0908 095f 1018 7b7b 3333 352c 2031 3938  ..._..{{335, 198
-00004940: 7d2c 207b 3932 372c 2035 3638 7d7d 0908  }, {927, 568}}..
-00004950: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
-00004960: 0000 0000 0101 0000 0000 0000 000f 0000  ................
-00004970: 0000 0000 0000 0000 0000 0000 009a 0000  ................
-00004980: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
-00004990: 006f 0072 0061 0067 0065 6c67 3153 636f  .o.r.a.g.elg1Sco
-000049a0: 6d70 0000 0000 0000 1804 0000 000c 0062  mp.............b
-000049b0: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
-000049c0: 0061 0067 0065 6d6f 4444 626c 6f62 0000  .a.g.emoDDblob..
-000049d0: 0008 3f3c 3f74 e2dd c441 0000 000c 0062  ..?<?t...A.....b
-000049e0: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
-000049f0: 0061 0067 0065 6d6f 6444 626c 6f62 0000  .a.g.emodDblob..
-00004a00: 0008 3f3c 3f74 e2dd c441 0000 000c 0062  ..?<?t...A.....b
-00004a10: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
-00004a20: 0061 0067 0065 7068 3153 636f 6d70 0000  .a.g.eph1Scomp..
-00004a30: 0000 0000 2000 0000 000c 0062 006c 006f  .... ......b.l.o
-00004a40: 0062 005f 0073 0074 006f 0072 0061 0067  .b._.s.t.o.r.a.g
-00004a50: 0065 7653 726e 6c6f 6e67 0000 0001 0000  .evSrnlong......
-00004a60: 0012 0062 006f 0075 006e 0064 0069 006e  ...b.o.u.n.d.i.n
-00004a70: 0067 005f 0062 006f 0078 005f 0074 006f  .g._.b.o.x._.t.o
-00004a80: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
-00004a90: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00004aa0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00004ab0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00004ac0: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00004ad0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00004ae0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00004af0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00004b00: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-00004b10: 5f10 197b 7b33 3534 2c20 3132 347d 2c20  _..{{354, 124}, 
-00004b20: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
-00004b30: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
-00004b40: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00004b50: 0000 0000 0000 0000 0000 009b 0000 0012  ................
-00004b60: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
-00004b70: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
-00004b80: 006c 0073 6473 636c 626f 6f6c 0000 0000  .l.sdsclbool....
-00004b90: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
-00004ba0: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
-00004bb0: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
-00004bc0: 0000 02e8 8d00 0000 1200 6200 6f00 7500  ..........b.o.u.
-00004bd0: 6e00 6400 6900 6e00 6700 5f00 6200 6f00  n.d.i.n.g._.b.o.
-00004be0: 7800 5f00 7400 6f00 6f00 6c00 736c 7376  x._.t.o.o.l.slsv
-00004bf0: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
-00004c00: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
-00004c10: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
-00004c20: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00004c30: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00004c40: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00004c50: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00004c60: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-00004c70: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-00004c80: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
-00004c90: 3237 3c41 d40d 0e0f 100a 120a 1457 7669  27<A.........Wvi
-00004ca0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-00004cb0: 6e64 696e 675a 6964 656e 7469 6669 6572  ndingZidentifier
-00004cc0: 0911 01c7 0954 6e61 6d65 d40d 0e0f 1016  .....Tname......
-00004cd0: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
-00004ce0: d40d 0e0f 100a 1c16 1e09 10b5 085c 6461  .............\da
-00004cf0: 7465 4d6f 6469 6669 6564 d40d 0e0f 1016  teModified......
-00004d00: 1c16 2208 085b 6461 7465 4372 6561 7465  .."..[dateCreate
-00004d10: 64d4 0d0e 0f10 0a25 1627 0910 6108 5473  d......%.'..a.Ts
-00004d20: 697a 65d4 0d0e 0f10 0a2a 0a2c 0910 7309  ize......*.,..s.
-00004d30: 546b 696e 64d4 0d0e 0f10 162f 0a31 0810  Tkind....../.1..
-00004d40: 6409 556c 6162 656c d40d 0e0f 1016 340a  d.Ulabel......4.
-00004d50: 3608 104b 0957 7665 7273 696f 6ed4 0d0e  6..K.Wversion...
-00004d60: 0f10 1639 0a3b 0811 012c 0958 636f 6d6d  ...9.;...,.Xcomm
-00004d70: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
-00004d80: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00004d90: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
-00004da0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-00004db0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00004dc0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
-00004dd0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
-00004de0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
-00004df0: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
-00004e00: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
-00004e10: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
-00004e20: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00004e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00004e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00004e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
-00004e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00004e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00004220: 0908 095f 1015 7b7b 302c 2035 7d2c 207b  ..._..{{0, 5}, {
+00004230: 3134 3237 2c20 3837 307d 7d09 0815 232f  1427, 870}}...#/
+00004240: 3b52 5f6b 6c6d 6e6f 8700 0000 0000 0001  ;R_klmno........
+00004250: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00004260: 0000 0000 0000 0000 8800 0000 0600 6100  ..............a.
+00004270: 7300 7300 6500 7400 736c 6731 5363 6f6d  s.s.e.t.slg1Scom
+00004280: 7000 0000 0000 7ddb 9300 0000 0600 6100  p.....}.......a.
+00004290: 7300 7300 6500 7400 736c 7376 4362 6c6f  s.s.e.t.slsvCblo
+000042a0: 6200 0002 b062 706c 6973 7430 30da 0102  b....bplist00...
+000042b0: 0304 0506 0708 090a 0b0c 0d1a 4849 484a  ............HIHJ
+000042c0: 0c4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
+000042d0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+000042e0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+000042f0: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
+00004300: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+00004310: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00004320: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00004330: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
+00004340: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
+00004350: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
+00004360: 0000 09ab 0e17 1c21 252a 2f34 393e 43d4  .......!%*/49>C.
+00004370: 0f10 1112 1314 0c0c 5a69 6465 6e74 6966  ........Zidentif
+00004380: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
+00004390: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
+000043a0: 1101 c709 09d4 0f10 1112 1819 1a1a 5875  ..............Xu
+000043b0: 6269 7175 6974 7910 2308 08d4 0f10 1112  biquity.#.......
+000043c0: 1d1e 1a0c 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+000043d0: 6410 b508 09d4 0f10 1112 221e 1a1a 5b64  d........."...[d
+000043e0: 6174 6543 7265 6174 6564 0808 d40f 1011  ateCreated......
+000043f0: 1226 271a 0c54 7369 7a65 1061 0809 d40f  .&'..Tsize.a....
+00004400: 1011 122b 2c0c 0c54 6b69 6e64 1073 0909  ...+,..Tkind.s..
+00004410: d40f 1011 1230 310c 1a55 6c61 6265 6c10  .....01..Ulabel.
+00004420: 6409 08d4 0f10 1112 3536 0c1a 5776 6572  d.......56..Wver
+00004430: 7369 6f6e 104b 0908 d40f 1011 123a 3b0c  sion.K.......:;.
+00004440: 1a58 636f 6d6d 656e 7473 1101 2c09 08d4  .Xcomments..,...
+00004450: 0f10 1112 3f40 1a1a 5e64 6174 654c 6173  ....?@..^dateLas
+00004460: 744f 7065 6e65 6410 c808 08d4 0f10 1112  tOpened.........
+00004470: 441e 1a1a 5964 6174 6541 6464 6564 0808  D...YdateAdded..
+00004480: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
+00004490: 0000 0054 6e61 6d65 0910 0100 0800 1d00  ...Tname........
+000044a0: 2600 3800 4000 5400 6600 6f00 8100 8c00  &.8.@.T.f.o.....
+000044b0: 9f00 b400 bd00 be00 ca00 d300 de00 e400  ................
+000044c0: ee00 f600 fb00 fe00 ff01 0001 0901 1201  ................
+000044d0: 1401 1501 1601 1f01 2c01 2e01 2f01 3001  ........,.../.0.
+000044e0: 3901 4501 4601 4701 5001 5501 5701 5801  9.E.F.G.P.U.W.X.
+000044f0: 5901 6201 6701 6901 6a01 6b01 7401 7a01  Y.b.g.i.j.k.t.z.
+00004500: 7c01 7d01 7e01 8701 8f01 9101 9201 9301  |.}.~...........
+00004510: 9c01 a501 a801 a901 aa01 b301 c201 c401  ................
+00004520: c501 c601 cf01 d901 da01 db01 dc01 e501  ................
+00004530: ee01 f301 f400 0000 0000 0002 0100 0000  ................
+00004540: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
+00004550: 0000 0001 f600 0000 0600 6100 7300 7300  ..........a.s.s.
+00004560: 6500 7400 736c 7376 7062 6c6f 6200 0002  e.t.slsvpblob...
+00004570: 9562 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
+00004580: 0708 090a 0b0c 0d1c 4849 484a 0c29 5869  ........HIHJ.)Xi
+00004590: 636f 6e53 697a 655f 100f 7368 6f77 4963  conSize_..showIc
+000045a0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+000045b0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+000045c0: 5369 7a65 735f 100f 7363 726f 6c6c 506f  Sizes_..scrollPo
+000045d0: 7369 7469 6f6e 5958 7465 7874 5369 7a65  sitionYXtextSize
+000045e0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000045f0: 6e58 5a73 6f72 7443 6f6c 756d 6e5f 1010  nXZsortColumn_..
+00004600: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00004610: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00004620: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
+00004630: 0e0f 1011 1213 1415 1617 2025 2a2e 3338  .......... %*.38
+00004640: 3d42 5863 6f6d 6d65 6e74 735e 6461 7465  =BXcomments^date
+00004650: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
+00004660: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
+00004670: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
+00004680: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
+00004690: d418 191a 1b1c 1d0c 1f57 7669 7369 626c  .........Wvisibl
+000046a0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+000046b0: 6755 696e 6465 7808 1101 2c09 1007 d418  gUindex...,.....
+000046c0: 191a 1b1c 221c 2408 10c8 0810 08d4 1819  ....".$.........
+000046d0: 1a1b 0c27 1c29 0910 b508 1001 d418 191a  ...'.)..........
+000046e0: 1b1c 271c 2d08 0810 02d4 1819 1a1b 0c30  ..'.-..........0
+000046f0: 1c32 0910 6108 1003 d418 191a 1b1c 350c  .2..a.........5.
+00004700: 3708 1064 0910 05d4 1819 1a1b 0c3a 0c3c  7..d.........:.<
+00004710: 0910 7309 1004 d418 191a 1b1c 3f0c 4108  ..s.........?.A.
+00004720: 104b 0910 06d4 1819 1a1b 0c44 0c46 0911  .K.........D.F..
+00004730: 01c7 0910 0008 2300 0000 0000 0000 0023  ......#........#
+00004740: 4028 0000 0000 0000 546e 616d 6509 0008  @(......Tname...
+00004750: 001d 0026 0038 0040 0054 0066 006f 0081  ...&.8.@.T.f.o..
+00004760: 008c 009f 00b4 00bd 00be 00d1 00da 00e9  ................
+00004770: 00f6 0102 0107 010d 0112 011a 011f 0128  ...............(
+00004780: 0130 0136 0140 0146 0147 014a 014b 014d  .0.6.@.F.G.J.K.M
+00004790: 0156 0157 0159 015a 015c 0165 0166 0168  .V.W.Y.Z.\.e.f.h
+000047a0: 0169 016b 0174 0175 0176 0178 0181 0182  .i.k.t.u.v.x....
+000047b0: 0184 0185 0187 0190 0191 0193 0194 0196  ................
+000047c0: 019f 01a0 01a2 01a3 01a5 01ae 01af 01b1  ................
+000047d0: 01b2 01b4 01bd 01be 01c1 01c2 01c4 01c5  ................
+000047e0: 01ce 01d7 01dc 0000 0000 0000 0201 0000  ................
+000047f0: 0000 0000 004c 0000 0000 0000 0000 0000  .....L..........
+00004800: 0000 0000 01dd 0000 0006 0061 0073 0073  ...........a.s.s
+00004810: 0065 0074 0073 6d6f 4444 626c 6f62 0000  .e.t.smoDDblob..
+00004820: 0008 cf95 8ce8 d0e1 c441 0000 0006 0061  .........A.....a
+00004830: 0073 0073 0065 0074 0073 6d6f 6444 626c  .s.s.e.t.smodDbl
+00004840: 6f62 0000 0008 cf95 8ce8 d0e1 c441 0000  ob...........A..
+00004850: 0006 0061 0073 0073 0065 0074 0073 7068  ...a.s.s.e.t.sph
+00004860: 3153 636f 6d70 0000 0000 0081 a000 0000  1Scomp..........
+00004870: 0006 0061 0073 0073 0065 0074 0073 7653  ...a.s.s.e.t.svS
+00004880: 726e 6c6f 6e67 0000 0001 0000 000c 0062  rnlong.........b
+00004890: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
+000048a0: 0061 0067 0065 6277 7370 626c 6f62 0000  .a.g.ebwspblob..
+000048b0: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+000048c0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+000048d0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+000048e0: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+000048f0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00004900: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00004910: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00004920: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+00004930: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
+00004940: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
+00004950: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
+00004960: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
+00004970: 0000 0000 0000 0000 0000 9a00 0000 0c00  ................
+00004980: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
+00004990: 7200 6100 6700 656c 6731 5363 6f6d 7000  r.a.g.elg1Scomp.
+000049a0: 0000 0000 0018 0400 0000 0c00 6200 6c00  ............b.l.
+000049b0: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
+000049c0: 6700 656d 6f44 4462 6c6f 6200 0000 083f  g.emoDDblob....?
+000049d0: 3c3f 74e2 ddc4 4100 0000 0c00 6200 6c00  <?t...A.....b.l.
+000049e0: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
+000049f0: 6700 656d 6f64 4462 6c6f 6200 0000 083f  g.emodDblob....?
+00004a00: 3c3f 74e2 ddc4 4100 0000 0c00 6200 6c00  <?t...A.....b.l.
+00004a10: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
+00004a20: 6700 6570 6831 5363 6f6d 7000 0000 0000  g.eph1Scomp.....
+00004a30: 0020 0000 0000 0c00 6200 6c00 6f00 6200  . ......b.l.o.b.
+00004a40: 5f00 7300 7400 6f00 7200 6100 6700 6576  _.s.t.o.r.a.g.ev
+00004a50: 5372 6e6c 6f6e 6700 0000 0100 0000 1200  Srnlong.........
+00004a60: 6200 6f00 7500 6e00 6400 6900 6e00 6700  b.o.u.n.d.i.n.g.
+00004a70: 5f00 6200 6f00 7800 5f00 7400 6f00 6f00  _.b.o.x._.t.o.o.
+00004a80: 6c00 7362 7773 7062 6c6f 6200 0000 ca62  l.sbwspblob....b
+00004a90: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00004aa0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00004ab0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00004ac0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00004ad0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00004ae0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00004af0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00004b00: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00004b10: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00004b20: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+00004b30: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+00004b40: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+00004b50: 0000 0000 0000 0000 9b00 0000 1200 6200  ..............b.
+00004b60: 6f00 7500 6e00 6400 6900 6e00 6700 5f00  o.u.n.d.i.n.g._.
+00004b70: 6200 6f00 7800 5f00 7400 6f00 6f00 6c00  b.o.x._.t.o.o.l.
+00004b80: 7364 7363 6c62 6f6f 6c00 0000 0012 0062  sdsclbool......b
+00004b90: 006f 0075 006e 0064 0069 006e 0067 005f  .o.u.n.d.i.n.g._
+00004ba0: 0062 006f 0078 005f 0074 006f 006f 006c  .b.o.x._.t.o.o.l
+00004bb0: 0073 6c67 3153 636f 6d70 0000 0000 0002  .slg1Scomp......
+00004bc0: e88d 0000 0012 0062 006f 0075 006e 0064  .......b.o.u.n.d
+00004bd0: 0069 006e 0067 005f 0062 006f 0078 005f  .i.n.g._.b.o.x._
+00004be0: 0074 006f 006f 006c 0073 6c73 7643 626c  .t.o.o.l.slsvCbl
+00004bf0: 6f62 0000 0279 6270 6c69 7374 3030 d801  ob...ybplist00..
+00004c00: 0203 0405 0607 0809 0a0b 1646 4748 0a5f  ...........FGH._
+00004c10: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00004c20: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+00004c30: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00004c40: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00004c50: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+00004c60: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+00004c70: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00004c80: 6573 1001 09ab 0c15 1a1f 2328 2d32 373c  es........#(-27<
+00004c90: 41d4 0d0e 0f10 0a12 0a14 5776 6973 6962  A.........Wvisib
+00004ca0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00004cb0: 6e67 5a69 6465 6e74 6966 6965 7209 1101  ngZidentifier...
+00004cc0: c709 546e 616d 65d4 0d0e 0f10 1617 1619  ..Tname.........
+00004cd0: 0810 2308 5875 6269 7175 6974 79d4 0d0e  ..#.Xubiquity...
+00004ce0: 0f10 0a1c 161e 0910 b508 5c64 6174 654d  ..........\dateM
+00004cf0: 6f64 6966 6965 64d4 0d0e 0f10 161c 1622  odified........"
+00004d00: 0808 5b64 6174 6543 7265 6174 6564 d40d  ..[dateCreated..
+00004d10: 0e0f 100a 2516 2709 1061 0854 7369 7a65  ....%.'..a.Tsize
+00004d20: d40d 0e0f 100a 2a0a 2c09 1073 0954 6b69  ......*.,..s.Tki
+00004d30: 6e64 d40d 0e0f 1016 2f0a 3108 1064 0955  nd....../.1..d.U
+00004d40: 6c61 6265 6cd4 0d0e 0f10 1634 0a36 0810  label......4.6..
+00004d50: 4b09 5776 6572 7369 6f6e d40d 0e0f 1016  K.Wversion......
+00004d60: 390a 3b08 1101 2c09 5863 6f6d 6d65 6e74  9.;...,.Xcomment
+00004d70: 73d4 0d0e 0f10 163e 1640 0810 c808 5e64  s......>.@....^d
+00004d80: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
+00004d90: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
+00004da0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
+00004db0: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
+00004dc0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
+00004dd0: 8e00 8f00 9b00 a400 ac00 b200 bc00 c700  ................
+00004de0: c800 cb00 cc00 d100 da00 db00 dd00 de00  ................
+00004df0: e700 f000 f100 f300 f401 0101 0a01 0b01  ................
+00004e00: 0c01 1801 2101 2201 2401 2501 2a01 3301  ....!.".$.%.*.3.
+00004e10: 3401 3601 3701 3c01 4501 4601 4801 4901  4.6.7.<.E.F.H.I.
+00004e20: 4f01 5801 5901 5b01 5c01 6401 6d01 6e01  O.X.Y.[.\.d.m.n.
+00004e30: 7101 7201 7b01 8401 8501 8701 8801 9701  q.r.{...........
+00004e40: a001 a101 a201 ac01 ad01 b601 bb01 c400  ................
+00004e50: 0000 0000 0002 0100 0000 0000 0000 4a00  ..............J.
+00004e60: 0000 0000 0000 0000 0000 0000 0001 c500  ................
+00004e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1489,31 +1489,31 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0b3d ba16 4008 10c8  omp......=..@...
-00005d80: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00005d90: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
-00005da0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-00005db0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00005dc0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
-00005dd0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
-00005de0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
-00005df0: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
-00005e00: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
-00005e10: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
-00005e20: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00005e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00005e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00005e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
-00005e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00005e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00005d70: 6f6d 7000 0000 0000 0b3d ba10 c808 5e64  omp......=....^d
+00005d80: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
+00005d90: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
+00005da0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
+00005db0: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
+00005dc0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
+00005dd0: 8e00 8f00 9b00 a400 ac00 b200 bc00 c700  ................
+00005de0: c800 cb00 cc00 d100 da00 db00 dd00 de00  ................
+00005df0: e700 f000 f100 f300 f401 0101 0a01 0b01  ................
+00005e00: 0c01 1801 2101 2201 2401 2501 2a01 3301  ....!.".$.%.*.3.
+00005e10: 3401 3601 3701 3c01 4501 4601 4801 4901  4.6.7.<.E.F.H.I.
+00005e20: 4f01 5801 5901 5b01 5c01 6401 6d01 6e01  O.X.Y.[.\.d.m.n.
+00005e30: 7101 7201 7b01 8401 8501 8701 8801 9701  q.r.{...........
+00005e40: a001 a101 a201 ac01 ad01 b601 bb01 c400  ................
+00005e50: 0000 0000 0002 0100 0000 0000 0000 4a00  ..............J.
+00005e60: 0000 0000 0000 0000 0000 0000 0001 c500  ................
+00005e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1605,16 +1605,16 @@
 00006440: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
 00006450: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
 00006460: 2c20 7b39 3237 2c20 3536 387d 7d09 0815  , {927, 568}}...
 00006470: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
 00006480: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00006490: 0000 0000 0000 0000 0000 8b00 0000 0900  ................
 000064a0: 6c00 6100 6200 6500 6c00 6c00 6900 6e00  l.a.b.e.l.l.i.n.
-000064b0: 676c 6731 5363 6f6d 7000 0000 0000 031c  glg1Scomp.......
-000064c0: bc00 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
+000064b0: 676c 6731 5363 6f6d 7000 0000 0000 0321  glg1Scomp......!
+000064c0: c400 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000064d0: 6c00 6900 6e00 676c 7376 4362 6c6f 6200  l.i.n.glsvCblob.
 000064e0: 0002 7962 706c 6973 7430 30d8 0102 0304  ..ybplist00.....
 000064f0: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
 00006500: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
 00006510: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
 00006520: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
 00006530: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
@@ -1689,18 +1689,18 @@
 00006980: 0147 0150 0152 0154 0155 0156 015f 0161  .G.P.R.T.U.V._.a
 00006990: 0163 0164 0165 016e 0170 0172 0173 0174  .c.d.e.n.p.r.s.t
 000069a0: 017d 017f 0181 0182 0183 018c 018e 0191  .}..............
 000069b0: 0192 0193 0194 019d 01a2 01ab 0000 0000  ................
 000069c0: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 000069d0: 0000 0000 0000 0000 0000 01ac 0000 0009  ................
 000069e0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-000069f0: 0067 6d6f 4444 626c 6f62 0000 0008 f5a6  .gmoDDblob......
-00006a00: 3155 1321 c541 0000 0009 006c 0061 0062  1U.!.A.....l.a.b
+000069f0: 0067 6d6f 4444 626c 6f62 0000 0008 6a3a  .gmoDDblob....j:
+00006a00: 0fc2 4122 c541 0000 0009 006c 0061 0062  ..A".A.....l.a.b
 00006a10: 0065 006c 006c 0069 006e 0067 6d6f 6444  .e.l.l.i.n.gmodD
-00006a20: 626c 6f62 0000 0008 f5a6 3155 1321 c541  blob......1U.!.A
+00006a20: 626c 6f62 0000 0008 6a3a 0fc2 4122 c541  blob....j:..A".A
 00006a30: 0000 0009 006c 0061 0062 0065 006c 006c  .....l.a.b.e.l.l
 00006a40: 0069 006e 0067 7068 3153 636f 6d70 0000  .i.n.gph1Scomp..
 00006a50: 0000 0003 a000 0000 0009 006c 0061 0062  ...........l.a.b
 00006a60: 0065 006c 006c 0069 006e 0067 7653 726e  .e.l.l.i.n.gvSrn
 00006a70: 6c6f 6e67 0000 0001 0000 0006 006d 0069  long.........m.i
 00006a80: 0078 0069 006e 0073 6277 7370 626c 6f62  .x.i.n.sbwspblob
 00006a90: 0000 00c8 6270 6c69 7374 3030 d701 0203  ....bplist00....
@@ -1713,15 +1713,15 @@
 00006b00: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 00006b10: 0809 5f10 177b 7b30 2c20 3130 357d 2c20  .._..{{0, 105}, 
 00006b20: 7b31 3139 392c 2037 3639 7d7d 0908 1725  {1199, 769}}...%
 00006b30: 313d 4960 6d79 7a7b 7c7d 7e98 0000 0000  1=I`myz{|}~.....
 00006b40: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00006b50: 0000 0000 0000 0000 0000 0099 0000 0006  ................
 00006b60: 006d 0069 0078 0069 006e 0073 6c67 3153  .m.i.x.i.n.slg1S
-00006b70: 636f 6d70 0000 0000 0010 4db8 0000 0006  comp......M.....
+00006b70: 636f 6d70 0000 0000 0010 4dd8 0000 0006  comp......M.....
 00006b80: 006d 0069 0078 0069 006e 0073 6c73 7643  .m.i.x.i.n.slsvC
 00006b90: 626c 6f62 0000 0281 6270 6c69 7374 3030  blob....bplist00
 00006ba0: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
 00006bb0: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
 00006bc0: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00006bd0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00006be0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -1755,21 +1755,21 @@
 00006da0: ff01 0001 0101 0a01 1601 1701 1801 2101  ..............!.
 00006db0: 2601 2801 2901 2a01 3301 3801 3a01 3b01  &.(.).*.3.8.:.;.
 00006dc0: 3c01 4501 4b01 4d01 4e01 4f01 5801 6001  <.E.K.M.N.O.X.`.
 00006dd0: 6201 6301 6401 6d01 7601 7901 7a01 7b01  b.c.d.m.v.y.z.{.
 00006de0: 8401 9301 9501 9601 9701 a001 a101 a201  ................
 00006df0: ac01 ad01 b601 c301 cc00 0000 0000 0002  ................
 00006e00: 0100 0000 0000 0000 4a00 0000 0000 0000  ........J.......
-00006e10: 0000 0000 0000 0001 cd3c 0145 0146 0148  .........<.E.F.H
-00006e20: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00006e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00006e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00006e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
-00006e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00006e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00006e10: 0000 0000 0000 0001 cd01 4601 4801 4901  ..........F.H.I.
+00006e20: 4f01 5801 5901 5b01 5c01 6401 6d01 6e01  O.X.Y.[.\.d.m.n.
+00006e30: 7101 7201 7b01 8401 8501 8701 8801 9701  q.r.{...........
+00006e40: a001 a101 a201 ac01 ad01 b601 bb01 c400  ................
+00006e50: 0000 0000 0002 0100 0000 0000 0000 4a00  ..............J.
+00006e60: 0000 0000 0000 0000 0000 0000 0001 c500  ................
+00006e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2088,18 +2088,18 @@
 00008270: 017a 0183 0185 0187 0188 0189 0192 0194  .z..............
 00008280: 0195 0196 019f 01a1 01a3 01a4 01a5 01ae  ................
 00008290: 01b0 01b3 01b4 01b5 01be 01c0 01c2 01c3  ................
 000082a0: 01c4 01c5 01ce 01d7 01e0 01e5 0000 0000  ................
 000082b0: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
 000082c0: 0000 0000 0000 0000 0000 01e6 0000 0008  ................
 000082d0: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-000082e0: 6d6f 4444 626c 6f62 0000 0008 b0f7 c86b  moDDblob.......k
-000082f0: eb20 c541 0000 0008 0070 006c 006f 0074  . .A.....p.l.o.t
+000082e0: 6d6f 4444 626c 6f62 0000 0008 8d4a a152  moDDblob.....J.R
+000082f0: 1321 c541 0000 0008 0070 006c 006f 0074  .!.A.....p.l.o.t
 00008300: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
-00008310: 0000 0008 b0f7 c86b eb20 c541 0000 0008  .......k. .A....
+00008310: 0000 0008 8d4a a152 1321 c541 0000 0008  .....J.R.!.A....
 00008320: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00008330: 7068 3153 636f 6d70 0000 0000 0014 2000  ph1Scomp...... .
 00008340: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00008350: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
 00008360: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
 00008370: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
 00008380: 0074 0069 006f 006e 0073 6277 7370 626c  .t.i.o.n.sbwspbl
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 079c 6d00 0000 0900  omp.......m.....
+00009bb0: 6f6d 7000 0000 0000 079d 0800 0000 0900  omp.............
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2554,20 +2554,20 @@
 00009f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a000: 0000 0000 0000 0000 0000 0018 0000 0009  ................
+0000a000: 0000 0000 0000 0000 0000 001a 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
-0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 5519  .smoDDblob....U.
-0000a030: 3cb9 d51b c541 0000 0009 0072 006f 0069  <....A.....r.o.i
+0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 0230  .smoDDblob.....0
+0000a030: 3ea2 4422 c541 0000 0009 0072 006f 0069  >.D".A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-0000a050: 626c 6f62 0000 0008 5519 3cb9 d51b c541  blob....U.<....A
+0000a050: 626c 6f62 0000 0008 0230 3ea2 4422 c541  blob.....0>.D".A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
 0000a080: 0000 0009 8000 0000 0009 0072 006f 0069  ...........r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
 0000a0a0: 6c6f 6e67 0000 0001 0000 0002 0073 0074  long.........s.t
 0000a0b0: 6c67 3153 636f 6d70 0000 0000 0000 3102  lg1Scomp......1.
 0000a0c0: 0000 0002 0073 0074 6d6f 4444 626c 6f62  .....s.tmoDDblob
@@ -2697,377 +2697,377 @@
 0000a880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
 0000a890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
 0000a8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
 0000a8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000a8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000a8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000a8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
-0000a8f0: 6e6c 6f6e 6700 0000 0100 0000 0200 7500  nlong.........u.
-0000a900: 6962 7773 7062 6c6f 6200 0000 ca62 706c  ibwspblob....bpl
-0000a910: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
-0000a920: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-0000a930: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
-0000a940: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-0000a950: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-0000a960: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-0000a970: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-0000a980: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
-0000a990: 3335 342c 2031 3234 7d2c 207b 3130 3736  354, 124}, {1076
-0000a9a0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
-0000a9b0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
-0000a9c0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-0000a9d0: 0000 0000 0000 9b00 0000 0200 7500 6964  ............u.id
-0000a9e0: 7363 6c62 6f6f 6c00 0000 0002 0075 0069  sclbool......u.i
-0000a9f0: 6c67 3153 636f 6d70 0000 0000 0011 9d6b  lg1Scomp.......k
-0000aa00: 0000 0002 0075 0069 6c73 7643 626c 6f62  .....u.ilsvCblob
-0000aa10: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
-0000aa20: 0405 0607 0809 0a0b 1846 4748 0a5f 1012  .........FGH._..
-0000aa30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-0000aa40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-0000aa50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-0000aa60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-0000aa70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-0000aa80: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-0000aa90: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-0000aaa0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
-0000aab0: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
-0000aac0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-0000aad0: 5a69 6465 6e74 6966 6965 7209 1101 c709  Zidentifier.....
-0000aae0: 546e 616d 65d4 100e 0f0d 1617 1818 5875  Tname.........Xu
-0000aaf0: 6269 7175 6974 7910 2308 08d4 100f 0e0d  biquity.#.......
-0000ab00: 1b18 1d0a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-0000ab10: 6408 10b5 09d4 100f 0e0d 2018 1d18 5b64  d......... ...[d
-0000ab20: 6174 6543 7265 6174 6564 0808 d410 0f0e  ateCreated......
-0000ab30: 0d24 1826 0a54 7369 7a65 0810 6109 d410  .$.&.Tsize..a...
-0000ab40: 0f0e 0d29 0a2b 0a54 6b69 6e64 0910 7309  ...).+.Tkind..s.
-0000ab50: d410 0f0e 0d2e 0a30 1855 6c61 6265 6c09  .......0.Ulabel.
-0000ab60: 1064 08d4 100f 0e0d 330a 3518 5776 6572  .d......3.5.Wver
-0000ab70: 7369 6f6e 0910 4b08 d410 0f0e 0d38 0a3a  sion..K......8.:
-0000ab80: 1858 636f 6d6d 656e 7473 0911 012c 08d4  .Xcomments...,..
-0000ab90: 100f 0e0d 3d18 3f18 5e64 6174 654c 6173  ....=.?.^dateLas
-0000aba0: 744f 7065 6e65 6408 10c8 08d4 100e 0f0d  tOpened.........
-0000abb0: 421d 1818 5964 6174 6541 6464 6564 0808  B...YdateAdded..
-0000abc0: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
-0000abd0: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
-0000abe0: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
-0000abf0: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
-0000ac00: cb00 cc00 d100 da00 e300 e500 e600 e700  ................
-0000ac10: f000 fd00 fe01 0001 0101 0a01 1601 1701  ................
-0000ac20: 1801 2101 2601 2701 2901 2a01 3301 3801  ..!.&.'.).*.3.8.
-0000ac30: 3901 3b01 3c01 4501 4b01 4c01 4e01 4f01  9.;.<.E.K.L.N.O.
-0000ac40: 5801 6001 6101 6301 6401 6d01 7601 7701  X.`.a.c.d.m.v.w.
-0000ac50: 7a01 7b01 8401 9301 9401 9601 9701 a001  z.{.............
-0000ac60: aa01 ab01 ac01 ad01 b601 bb01 c400 0000  ................
-0000ac70: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
-0000ac80: 0000 0000 0000 0000 0000 0001 c500 0000  ................
-0000ac90: 0200 7500 696c 7376 7062 6c6f 6200 0002  ..u.ilsvpblob...
-0000aca0: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
-0000acb0: 0708 090a 0b1a 4546 470a 5f10 1276 6965  ......EFG._..vie
-0000acc0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
-0000acd0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-0000ace0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-0000acf0: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
-0000ad00: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
-0000ad10: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
-0000ad20: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
-0000ad30: d90c 0d0e 0f10 1112 1314 151e 2327 2b30  ............#'+0
-0000ad40: 353a 3f58 636f 6d6d 656e 7473 5e64 6174  5:?Xcomments^dat
-0000ad50: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
-0000ad60: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
-0000ad70: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
-0000ad80: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
-0000ad90: 65d4 1617 1819 1a0a 1c1d 5776 6973 6962  e.........Wvisib
-0000ada0: 6c65 5961 7363 656e 6469 6e67 5577 6964  leYascendingUwid
-0000adb0: 7468 5569 6e64 6578 0809 1101 2c10 07d4  thUindex....,...
-0000adc0: 1617 1819 1a1a 2122 0808 10c8 1008 d416  ......!"........
-0000add0: 1718 190a 1a26 0909 0810 b5d4 1617 1819  .....&..........
-0000ade0: 1a1a 262a 0808 1002 d416 1718 190a 1a2e  ..&*............
-0000adf0: 2f09 0810 6110 03d4 1617 1819 1a0a 3334  /...a.........34
-0000ae00: 0809 1064 1005 d416 1718 190a 0a38 3909  ...d.........89.
-0000ae10: 0910 7310 04d4 1617 1819 1a0a 3d3e 0809  ..s.........=>..
-0000ae20: 104b 1006 d419 1817 1640 410a 0a10 0011  .K.......@A.....
-0000ae30: 01c7 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
-0000ae40: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-0000ae50: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
-0000ae60: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
-0000ae70: d800 de00 e300 eb00 f000 f901 0101 0b01  ................
-0000ae80: 1101 1701 1801 1901 1c01 1e01 2701 2801  ............'.(.
-0000ae90: 2901 2b01 2d01 3601 3701 3801 3a01 4301  ).+.-.6.7.8.:.C.
-0000aea0: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
-0000aeb0: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
-0000aec0: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
-0000aed0: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
-0000aee0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-0000aef0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
-0000af00: 0000 0200 7500 696d 6f44 4462 6c6f 6200  ....u.imoDDblob.
-0000af10: 0000 087e abce 1cd0 1fc5 4100 0000 0200  ...~......A.....
-0000af20: 7500 696d 6f64 4462 6c6f 6200 0000 087e  u.imodDblob....~
-0000af30: abce 1cd0 1fc5 4100 0000 0200 7500 6970  ......A.....u.ip
-0000af40: 6831 5363 6f6d 7000 0000 0000 17c0 0000  h1Scomp.........
-0000af50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-0000af60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
-0000af70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-0000af80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
-0000af90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
-0000b010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-0000b020: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
-0000b030: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
-0000b040: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-0000b050: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-0000b060: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-0000b070: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-0000b080: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-0000b090: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-0000b0a0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000b0b0: 0809 5f10 197b 7b33 3534 2c20 3132 347d  .._..{{354, 124}
-0000b0c0: 2c20 7b31 3037 362c 2036 3231 7d7d 0908  , {1076, 621}}..
-0000b0d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
-0000b0e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
-0000b0f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
-0000b100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
-0000b110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
-0000b120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
-0000b130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
-0000b140: 6731 5363 6f6d 7000 0000 0000 03e8 6900  g1Scomp.......i.
+0000a8f0: 6e6c 6f6e 6700 0000 0100 0000 1000 7400  nlong.........t.
+0000a900: 6800 7200 6500 6500 5f00 6400 6900 6d00  h.r.e.e._.d.i.m.
+0000a910: 6500 6e00 7300 6900 6f00 6e00 736c 6731  e.n.s.i.o.n.slg1
+0000a920: 5363 6f6d 7000 0000 0000 0332 ac00 0000  Scomp......2....
+0000a930: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
+0000a940: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
+0000a950: 736d 6f44 4462 6c6f 6200 0000 08f6 8857  smoDDblob......W
+0000a960: d65e 24c5 4100 0000 1000 7400 6800 7200  .^$.A.....t.h.r.
+0000a970: 6500 6500 5f00 6400 6900 6d00 6500 6e00  e.e._.d.i.m.e.n.
+0000a980: 7300 6900 6f00 6e00 736d 6f64 4462 6c6f  s.i.o.n.smodDblo
+0000a990: 6200 0000 08f6 8857 d65e 24c5 4100 0000  b......W.^$.A...
+0000a9a0: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
+0000a9b0: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
+0000a9c0: 7370 6831 5363 6f6d 7000 0000 0000 03a0  sph1Scomp.......
+0000a9d0: 0000 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
+0000a9e0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
+0000a9f0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+0000aa00: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+0000aa10: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+0000aa20: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+0000aa30: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+0000aa40: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+0000aa50: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+0000aa60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
+0000aa70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+0000aa80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
+0000aa90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+0000aaa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
+0000aab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
+0000aac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
+0000aad0: 0000 0000 0011 9d6c 0000 0002 0075 0069  .......l.....u.i
+0000aae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
+0000aaf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+0000ab00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
+0000ab10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+0000ab20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+0000ab30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+0000ab40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
+0000ab50: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
+0000ab60: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
+0000ab70: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
+0000ab80: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
+0000ab90: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+0000aba0: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
+0000abb0: 6965 7209 1101 c709 546e 616d 65d4 100e  ier.....Tname...
+0000abc0: 0f0d 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
+0000abd0: 2308 08d4 100f 0e0d 1b18 1d0a 5c64 6174  #...........\dat
+0000abe0: 654d 6f64 6966 6965 6408 10b5 09d4 100f  eModified.......
+0000abf0: 0e0d 2018 1d18 5b64 6174 6543 7265 6174  .. ...[dateCreat
+0000ac00: 6564 0808 d410 0f0e 0d24 1826 0a54 7369  ed.......$.&.Tsi
+0000ac10: 7a65 0810 6109 d410 0f0e 0d29 0a2b 0a54  ze..a......).+.T
+0000ac20: 6b69 6e64 0910 7309 d410 0f0e 0d2e 0a30  kind..s........0
+0000ac30: 1855 6c61 6265 6c09 1064 08d4 100f 0e0d  .Ulabel..d......
+0000ac40: 330a 3518 5776 6572 7369 6f6e 0910 4b08  3.5.Wversion..K.
+0000ac50: d410 0f0e 0d38 0a3a 1858 636f 6d6d 656e  .....8.:.Xcommen
+0000ac60: 7473 0911 012c 08d4 100f 0e0d 3d18 3f18  ts...,......=.?.
+0000ac70: 5e64 6174 654c 6173 744f 7065 6e65 6408  ^dateLastOpened.
+0000ac80: 10c8 08d4 100e 0f0d 421d 1818 5964 6174  ........B...Ydat
+0000ac90: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
+0000aca0: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
+0000acb0: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+0000acc0: 7000 7900 8c00 8e00 8f00 9b00 a400 ac00  p.y.............
+0000acd0: b200 bc00 c700 c800 cb00 cc00 d100 da00  ................
+0000ace0: e300 e500 e600 e700 f000 fd00 fe01 0001  ................
+0000acf0: 0101 0a01 1601 1701 1801 2101 2601 2701  ..........!.&.'.
+0000ad00: 2901 2a01 3301 3801 3901 3b01 3c01 4501  ).*.3.8.9.;.<.E.
+0000ad10: 4b01 4c01 4e01 4f01 5801 6001 6101 6301  K.L.N.O.X.`.a.c.
+0000ad20: 6401 6d01 7601 7701 7a01 7b01 8401 9301  d.m.v.w.z.{.....
+0000ad30: 9401 9601 9701 a001 aa01 ab01 ac01 ad01  ................
+0000ad40: b601 bb01 c400 0000 0000 0002 0100 0000  ................
+0000ad50: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
+0000ad60: 0000 0001 c500 0000 0200 7500 696c 7376  ..........u.ilsv
+0000ad70: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+0000ad80: 30d8 0102 0304 0506 0708 090a 0b1a 4546  0.............EF
+0000ad90: 470a 5f10 1276 6965 774f 7074 696f 6e73  G._..viewOptions
+0000ada0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+0000adb0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+0000adc0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+0000add0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+0000ade0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+0000adf0: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+0000ae00: 4461 7465 7310 0109 d90c 0d0e 0f10 1112  Dates...........
+0000ae10: 1314 151e 2327 2b30 353a 3f58 636f 6d6d  ....#'+05:?Xcomm
+0000ae20: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+0000ae30: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
+0000ae40: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+0000ae50: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+0000ae60: 7369 6f6e 546e 616d 65d4 1617 1819 1a0a  sionTname.......
+0000ae70: 1c1d 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
+0000ae80: 6469 6e67 5577 6964 7468 5569 6e64 6578  dingUwidthUindex
+0000ae90: 0809 1101 2c10 07d4 1617 1819 1a1a 2122  ....,.........!"
+0000aea0: 0808 10c8 1008 d416 1718 190a 1a26 0909  .............&..
+0000aeb0: 0810 b5d4 1617 1819 1a1a 262a 0808 1002  ..........&*....
+0000aec0: d416 1718 190a 1a2e 2f09 0810 6110 03d4  ......../...a...
+0000aed0: 1617 1819 1a0a 3334 0809 1064 1005 d416  ......34...d....
+0000aee0: 1718 190a 0a38 3909 0910 7310 04d4 1617  .....89...s.....
+0000aef0: 1819 1a0a 3d3e 0809 104b 1006 d419 1817  ....=>...K......
+0000af00: 1640 410a 0a10 0011 01c7 0909 0823 4028  .@A..........#@(
+0000af10: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+0000af20: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
+0000af30: 5c00 6500 7000 7900 8c00 8e00 8f00 a200  \.e.p.y.........
+0000af40: ab00 ba00 c700 d300 d800 de00 e300 eb00  ................
+0000af50: f000 f901 0101 0b01 1101 1701 1801 1901  ................
+0000af60: 1c01 1e01 2701 2801 2901 2b01 2d01 3601  ....'.(.).+.-.6.
+0000af70: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
+0000af80: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
+0000af90: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
+0000afa0: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
+0000afb0: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
+0000afc0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+0000afd0: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
+0000afe0: 6f44 4462 6c6f 6200 0000 087e abce 1cd0  oDDblob....~....
+0000aff0: 1fc5 4100 0000 0000 0000 0000 0000 0000  ..A.............
+0000b000: 0000 0000 0000 0000 0000 000c 0000 0002  ................
+0000b010: 0075 0069 7068 3153 636f 6d70 0000 0000  .u.iph1Scomp....
+0000b020: 0017 c000 0000 0002 0075 0069 7653 726e  .........u.ivSrn
+0000b030: 6c6f 6e67 0000 0001 0000 000c 0075 006e  long.........u.n
+0000b040: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
+0000b050: 0065 0064 6277 7370 626c 6f62 0000 00ca  .e.dbwspblob....
+0000b060: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+0000b070: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+0000b080: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+0000b090: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+0000b0a0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+0000b0b0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+0000b0c0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+0000b0d0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+0000b0e0: 197b 7b33 3534 2c20 3132 347d 2c20 7b31  .{{354, 124}, {1
+0000b0f0: 3037 362c 2036 3231 7d7d 0908 1725 313d  076, 621}}...%1=
+0000b100: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
+0000b110: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+0000b120: 0000 0000 0000 0000 009b 0000 000c 0075  ...............u
+0000b130: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000b140: 0073 0065 0064 6473 636c 626f 6f6c 0000  .s.e.ddsclbool..
 0000b150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
-0000b160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
-0000b170: 6c6f 6200 0002 8162 706c 6973 7430 30d8  lob....bplist00.
-0000b180: 0102 0304 0506 0708 090a 0b18 4647 0a49  ............FG.I
-0000b190: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-0000b1a0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-0000b1b0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-0000b1c0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-0000b1d0: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-0000b1e0: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-0000b1f0: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-0000b200: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
-0000b210: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 1112  ..#(-27<A.......
-0000b220: 0a0a 5a69 6465 6e74 6966 6965 7255 7769  ..ZidentifierUwi
-0000b230: 6474 6859 6173 6365 6e64 696e 6757 7669  dthYascendingWvi
-0000b240: 7369 626c 6554 6e61 6d65 1101 c709 09d4  sibleTname......
-0000b250: 0d0e 0f10 1617 1818 5875 6269 7175 6974  ........Xubiquit
-0000b260: 7910 2308 08d4 100e 0f0d 0a1c 0a1e 0910  y.#.............
-0000b270: b509 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
-0000b280: 0d0e 0f10 201c 1818 5b64 6174 6543 7265  .... ...[dateCre
-0000b290: 6174 6564 0808 d40d 0e0f 1024 2518 0a54  ated.......$%..T
-0000b2a0: 7369 7a65 1061 0809 d40d 0e0f 1029 2a0a  size.a.......)*.
-0000b2b0: 0a54 6b69 6e64 1073 0909 d40d 0e0f 102e  .Tkind.s........
-0000b2c0: 2f0a 1855 6c61 6265 6c10 6409 08d4 0d0e  /..Ulabel.d.....
-0000b2d0: 0f10 3334 0a18 5776 6572 7369 6f6e 104b  ..34..Wversion.K
-0000b2e0: 0908 d40d 0e0f 1038 390a 1858 636f 6d6d  .......89..Xcomm
-0000b2f0: 656e 7473 1101 2c09 08d4 0d0e 0f10 3d3e  ents..,.......=>
-0000b300: 1818 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-0000b310: 6410 c808 08d4 0d0e 0f10 421c 1818 5964  d.........B...Yd
-0000b320: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
-0000b330: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-0000b340: 6409 1001 0008 0019 0022 0034 003c 0050  d........".4.<.P
-0000b350: 0059 0064 0077 008c 0095 0096 00a2 00ab  .Y.d.w..........
-0000b360: 00b6 00bc 00c6 00ce 00d3 00d6 00d7 00d8  ................
-0000b370: 00e1 00ea 00ec 00ed 00ee 00f7 00f8 00fa  ................
-0000b380: 00fb 0108 0111 011d 011e 011f 0128 012d  .............(.-
-0000b390: 012f 0130 0131 013a 013f 0141 0142 0143  ./.0.1.:.?.A.B.C
-0000b3a0: 014c 0152 0154 0155 0156 015f 0167 0169  .L.R.T.U.V._.g.i
-0000b3b0: 016a 016b 0174 017d 0180 0181 0182 018b  .j.k.t.}........
-0000b3c0: 019a 019c 019d 019e 01a7 01b1 01b2 01b3  ................
-0000b3d0: 01b4 01bd 01ca 01cb 0000 0000 0000 0201  ................
-0000b3e0: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
-0000b3f0: 0000 0000 0000 01cd 0000 000c 0075 006e  .............u.n
-0000b400: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
-0000b410: 0065 0064 6c73 7670 626c 6f62 0000 0266  .e.dlsvpblob...f
-0000b420: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-0000b430: 0809 0a0b 1a46 470a 2458 6963 6f6e 5369  .....FG.$XiconSi
-0000b440: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
-0000b450: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-0000b460: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-0000b470: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-0000b480: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-0000b490: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
-0000b4a0: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
-0000b4b0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
-0000b4c0: 151e 2328 2c31 363b 4058 636f 6d6d 656e  ..#(,16;@Xcommen
-0000b4d0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-0000b4e0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
-0000b4f0: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-0000b500: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-0000b510: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
-0000b520: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-0000b530: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-0000b540: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
-0000b550: c808 1008 d419 1718 1624 250a 0a10 0110  .........$%.....
-0000b560: b509 09d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
-0000b570: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
-0000b580: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
-0000b590: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
-0000b5a0: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
-0000b5b0: 190a 420a 4409 1101 c709 1000 0823 4028  ..B.D........#@(
-0000b5c0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
-0000b5d0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
-0000b5e0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
-0000b5f0: 00c1 00ce 00da 00df 00e5 00ea 00f2 00f7  ................
-0000b600: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
-0000b610: 0125 012e 012f 0131 0132 0134 013d 013f  .%.../.1.2.4.=.?
-0000b620: 0141 0142 0143 014c 014d 014e 0150 0159  .A.B.C.L.M.N.P.Y
-0000b630: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
-0000b640: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
-0000b650: 0189 018a 018c 0195 0196 0199 019a 019c  ................
-0000b660: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
-0000b670: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
-0000b680: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
-0000b690: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-0000b6a0: 0064 6d6f 4444 626c 6f62 0000 0008 cbf3  .dmoDDblob......
-0000b6b0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
-0000b6c0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-0000b6d0: 0064 6d6f 6444 626c 6f62 0000 0008 cbf3  .dmodDblob......
-0000b6e0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
-0000b6f0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-0000b700: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
-0000b710: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
-0000b720: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
-0000b730: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
-0000b740: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
-0000b750: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-0000b760: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-0000b770: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-0000b780: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-0000b790: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-0000b7a0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-0000b7b0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-0000b7c0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000b7d0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
-0000b7e0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
-0000b7f0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-0000b800: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-0000b810: 0000 0000 0000 0000 0000 0000 9a00 1b00  ................
-0000b820: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
-0000b830: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
-0000b840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
+0000b160: 7200 7600 6900 7300 6500 646c 6731 5363  r.v.i.s.e.dlg1Sc
+0000b170: 6f6d 7000 0000 0000 03e8 6900 0000 0c00  omp.......i.....
+0000b180: 7500 6e00 7300 7500 7000 6500 7200 7600  u.n.s.u.p.e.r.v.
+0000b190: 6900 7300 6500 646c 7376 4362 6c6f 6200  i.s.e.dlsvCblob.
+0000b1a0: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
+0000b1b0: 0506 0708 090a 0b18 4647 0a49 5869 636f  ........FG.IXico
+0000b1c0: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
+0000b1d0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+0000b1e0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+0000b1f0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+0000b200: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+0000b210: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
+0000b220: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
+0000b230: 4030 0000 0000 0000 09ab 0c15 1a1f 2328  @0............#(
+0000b240: 2d32 373c 41d4 0d0e 0f10 1112 0a0a 5a69  -27<A.........Zi
+0000b250: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
+0000b260: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+0000b270: 6554 6e61 6d65 1101 c709 09d4 0d0e 0f10  eTname..........
+0000b280: 1617 1818 5875 6269 7175 6974 7910 2308  ....Xubiquity.#.
+0000b290: 08d4 100e 0f0d 0a1c 0a1e 0910 b509 5c64  ..............\d
+0000b2a0: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
+0000b2b0: 201c 1818 5b64 6174 6543 7265 6174 6564   ...[dateCreated
+0000b2c0: 0808 d40d 0e0f 1024 2518 0a54 7369 7a65  .......$%..Tsize
+0000b2d0: 1061 0809 d40d 0e0f 1029 2a0a 0a54 6b69  .a.......)*..Tki
+0000b2e0: 6e64 1073 0909 d40d 0e0f 102e 2f0a 1855  nd.s......../..U
+0000b2f0: 6c61 6265 6c10 6409 08d4 0d0e 0f10 3334  label.d.......34
+0000b300: 0a18 5776 6572 7369 6f6e 104b 0908 d40d  ..Wversion.K....
+0000b310: 0e0f 1038 390a 1858 636f 6d6d 656e 7473  ...89..Xcomments
+0000b320: 1101 2c09 08d4 0d0e 0f10 3d3e 1818 5e64  ..,.......=>..^d
+0000b330: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
+0000b340: 08d4 0d0e 0f10 421c 1818 5964 6174 6541  ......B...YdateA
+0000b350: 6464 6564 0808 0823 4028 0000 0000 0000  dded...#@(......
+0000b360: 5c64 6174 654d 6f64 6966 6965 6409 1001  \dateModified...
+0000b370: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+0000b380: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
+0000b390: 00c6 00ce 00d3 00d6 00d7 00d8 00e1 00ea  ................
+0000b3a0: 00ec 00ed 00ee 00f7 00f8 00fa 00fb 0108  ................
+0000b3b0: 0111 011d 011e 011f 0128 012d 012f 0130  .........(.-./.0
+0000b3c0: 0131 013a 013f 0141 0142 0143 014c 0152  .1.:.?.A.B.C.L.R
+0000b3d0: 0154 0155 0156 015f 0167 0169 016a 016b  .T.U.V._.g.i.j.k
+0000b3e0: 0174 017d 0180 0181 0182 018b 019a 019c  .t.}............
+0000b3f0: 019d 019e 01a7 01b1 01b2 01b3 01b4 01bd  ................
+0000b400: 01ca 01cb 0000 0000 0000 0201 0000 0000  ................
+0000b410: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+0000b420: 0000 01cd 0000 000c 0075 006e 0073 0075  .........u.n.s.u
+0000b430: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
+0000b440: 6c73 7670 626c 6f62 0000 0266 6270 6c69  lsvpblob...fbpli
+0000b450: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+0000b460: 1a46 470a 2458 6963 6f6e 5369 7a65 5f10  .FG.$XiconSize_.
+0000b470: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+0000b480: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+0000b490: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+0000b4a0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+0000b4b0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+0000b4c0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+0000b4d0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+0000b4e0: 0009 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
+0000b4f0: 2c31 363b 4058 636f 6d6d 656e 7473 5e64  ,16;@Xcomments^d
+0000b500: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+0000b510: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+0000b520: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+0000b530: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+0000b540: 616d 65d4 1617 1819 1a1b 0a1d 5776 6973  ame.........Wvis
+0000b550: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+0000b560: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+0000b570: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
+0000b580: d419 1718 1624 250a 0a10 0110 b509 09d4  .....$%.........
+0000b590: 1617 1819 1a25 1a2b 0808 1002 d416 1718  .....%.+........
+0000b5a0: 190a 2e1a 3009 1061 0810 03d4 1617 1819  ....0..a........
+0000b5b0: 1a33 0a35 0810 6409 1005 d416 1718 190a  .3.5..d.........
+0000b5c0: 380a 3a09 1073 0910 04d4 1617 1819 1a3d  8.:..s.........=
+0000b5d0: 0a3f 0810 4b09 1006 d416 1718 190a 420a  .?..K.........B.
+0000b5e0: 4409 1101 c709 1000 0823 4028 0000 0000  D........#@(....
+0000b5f0: 0000 5c64 6174 654d 6f64 6966 6965 6409  ..\dateModified.
+0000b600: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+0000b610: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
+0000b620: 00da 00df 00e5 00ea 00f2 00f7 0100 0108  ................
+0000b630: 010e 0118 011e 011f 0122 0123 0125 012e  .........".#.%..
+0000b640: 012f 0131 0132 0134 013d 013f 0141 0142  ./.1.2.4.=.?.A.B
+0000b650: 0143 014c 014d 014e 0150 0159 015a 015c  .C.L.M.N.P.Y.Z.\
+0000b660: 015d 015f 0168 0169 016b 016c 016e 0177  .]._.h.i.k.l.n.w
+0000b670: 0178 017a 017b 017d 0186 0187 0189 018a  .x.z.{.}........
+0000b680: 018c 0195 0196 0199 019a 019c 019d 01a6  ................
+0000b690: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
+0000b6a0: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+0000b6b0: 01b4 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+0000b6c0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
+0000b6d0: 4444 626c 6f62 0000 0008 cbf3 6409 d917  DDblob......d...
+0000b6e0: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
+0000b6f0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
+0000b700: 6444 626c 6f62 0000 0008 cbf3 6409 d917  dDblob......d...
+0000b710: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
+0000b720: 0065 0072 0076 0069 0073 0065 0064 7068  .e.r.v.i.s.e.dph
+0000b730: 3153 636f 6d70 0000 0000 0004 d000 0000  1Scomp..........
+0000b740: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+0000b750: 0076 0069 0073 0065 0064 7653 726e 6c6f  .v.i.s.e.dvSrnlo
+0000b760: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
+0000b770: 006c 0073 6277 7370 626c 6f62 0000 00c9  .l.sbwspblob....
+0000b780: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+0000b790: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
+0000b7a0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+0000b7b0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+0000b7c0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+0000b7d0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+0000b7e0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+0000b7f0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
+0000b800: 187b 7b32 302c 2032 3336 7d2c 207b 3130  .{{20, 236}, {10
+0000b810: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+0000b820: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
+0000b830: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+0000b840: 0000 0000 0000 0000 9a00 6500 6e00 6400  ..........e.n.d.
 0000b850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
 0000b860: 086b 121b 34c6 1fc5 4100 0000 1b00 7400  .k..4...A.....t.
 0000b870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
 0000b880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
 0000b890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
 0000b8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
 0000b8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000b8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000b8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000b8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
-0000b8f0: 6e6c 6f6e 6700 0000 0100 0000 0200 7500  nlong.........u.
-0000b900: 6962 7773 7062 6c6f 6200 0000 ca62 706c  ibwspblob....bpl
-0000b910: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
-0000b920: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-0000b930: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
-0000b940: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-0000b950: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-0000b960: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-0000b970: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-0000b980: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
-0000b990: 3335 342c 2031 3234 7d2c 207b 3130 3736  354, 124}, {1076
-0000b9a0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
-0000b9b0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
-0000b9c0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-0000b9d0: 0000 0000 0000 9b00 0000 0200 7500 6964  ............u.id
-0000b9e0: 7363 6c62 6f6f 6c00 0000 0002 0075 0069  sclbool......u.i
-0000b9f0: 6c67 3153 636f 6d70 0000 0000 0011 9d6b  lg1Scomp.......k
-0000ba00: 0000 0002 0075 0069 6c73 7643 626c 6f62  .....u.ilsvCblob
-0000ba10: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
-0000ba20: 0405 0607 0809 0a0b 1846 4748 0a5f 1012  .........FGH._..
-0000ba30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-0000ba40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-0000ba50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-0000ba60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-0000ba70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-0000ba80: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-0000ba90: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-0000baa0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
-0000bab0: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
-0000bac0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-0000bad0: 5a69 6465 6e74 6966 6965 7209 1101 c709  Zidentifier.....
-0000bae0: 546e 616d 65d4 100e 0f0d 1617 1818 5875  Tname.........Xu
-0000baf0: 6269 7175 6974 7910 2308 08d4 100f 0e0d  biquity.#.......
-0000bb00: 1b18 1d0a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-0000bb10: 6408 10b5 09d4 100f 0e0d 2018 1d18 5b64  d......... ...[d
-0000bb20: 6174 6543 7265 6174 6564 0808 d410 0f0e  ateCreated......
-0000bb30: 0d24 1826 0a54 7369 7a65 0810 6109 d410  .$.&.Tsize..a...
-0000bb40: 0f0e 0d29 0a2b 0a54 6b69 6e64 0910 7309  ...).+.Tkind..s.
-0000bb50: d410 0f0e 0d2e 0a30 1855 6c61 6265 6c09  .......0.Ulabel.
-0000bb60: 1064 08d4 100f 0e0d 330a 3518 5776 6572  .d......3.5.Wver
-0000bb70: 7369 6f6e 0910 4b08 d410 0f0e 0d38 0a3a  sion..K......8.:
-0000bb80: 1858 636f 6d6d 656e 7473 0911 012c 08d4  .Xcomments...,..
-0000bb90: 100f 0e0d 3d18 3f18 5e64 6174 654c 6173  ....=.?.^dateLas
-0000bba0: 744f 7065 6e65 6408 10c8 08d4 100e 0f0d  tOpened.........
-0000bbb0: 421d 1818 5964 6174 6541 6464 6564 0808  B...YdateAdded..
-0000bbc0: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
-0000bbd0: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
-0000bbe0: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
-0000bbf0: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
-0000bc00: cb00 cc00 d100 da00 e300 e500 e600 e700  ................
-0000bc10: f000 fd00 fe01 0001 0101 0a01 1601 1701  ................
-0000bc20: 1801 2101 2601 2701 2901 2a01 3301 3801  ..!.&.'.).*.3.8.
-0000bc30: 3901 3b01 3c01 4501 4b01 4c01 4e01 4f01  9.;.<.E.K.L.N.O.
-0000bc40: 5801 6001 6101 6301 6401 6d01 7601 7701  X.`.a.c.d.m.v.w.
-0000bc50: 7a01 7b01 8401 9301 9401 9601 9701 a001  z.{.............
-0000bc60: aa01 ab01 ac01 ad01 b601 bb01 c400 0000  ................
-0000bc70: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
-0000bc80: 0000 0000 0000 0000 0000 0001 c500 0000  ................
-0000bc90: 0200 7500 696c 7376 7062 6c6f 6200 0002  ..u.ilsvpblob...
-0000bca0: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
-0000bcb0: 0708 090a 0b1a 4546 470a 5f10 1276 6965  ......EFG._..vie
-0000bcc0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
-0000bcd0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-0000bce0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-0000bcf0: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
-0000bd00: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
-0000bd10: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
-0000bd20: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
-0000bd30: d90c 0d0e 0f10 1112 1314 151e 2327 2b30  ............#'+0
-0000bd40: 353a 3f58 636f 6d6d 656e 7473 5e64 6174  5:?Xcomments^dat
-0000bd50: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
-0000bd60: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
-0000bd70: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
-0000bd80: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
-0000bd90: 65d4 1617 1819 1a0a 1c1d 5776 6973 6962  e.........Wvisib
-0000bda0: 6c65 5961 7363 656e 6469 6e67 5577 6964  leYascendingUwid
-0000bdb0: 7468 5569 6e64 6578 0809 1101 2c10 07d4  thUindex....,...
-0000bdc0: 1617 1819 1a1a 2122 0808 10c8 1008 d416  ......!"........
-0000bdd0: 1718 190a 1a26 0909 0810 b5d4 1617 1819  .....&..........
-0000bde0: 1a1a 262a 0808 1002 d416 1718 190a 1a2e  ..&*............
-0000bdf0: 2f09 0810 6110 03d4 1617 1819 1a0a 3334  /...a.........34
-0000be00: 0809 1064 1005 d416 1718 190a 0a38 3909  ...d.........89.
-0000be10: 0910 7310 04d4 1617 1819 1a0a 3d3e 0809  ..s.........=>..
-0000be20: 104b 1006 d419 1817 1640 410a 0a10 0011  .K.......@A.....
-0000be30: 01c7 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
-0000be40: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-0000be50: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
-0000be60: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
-0000be70: d800 de00 e300 eb00 f000 f901 0101 0b01  ................
-0000be80: 1101 1701 1801 1901 1c01 1e01 2701 2801  ............'.(.
-0000be90: 2901 2b01 2d01 3601 3701 3801 3a01 4301  ).+.-.6.7.8.:.C.
-0000bea0: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
-0000beb0: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
-0000bec0: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
-0000bed0: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
-0000bee0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-0000bef0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
-0000bf00: 0000 0200 7500 696d 6f44 4462 6c6f 6200  ....u.imoDDblob.
-0000bf10: 0000 087e abce 1cd0 1fc5 4100 0000 0200  ...~......A.....
-0000bf20: 7500 696d 6f64 4462 6c6f 6200 0000 087e  u.imodDblob....~
-0000bf30: abce 1cd0 1fc5 4100 0000 0200 7500 6970  ......A.....u.ip
-0000bf40: 6831 5363 6f6d 7000 0000 0000 17c0 0000  h1Scomp.........
-0000bf50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-0000bf60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
-0000bf70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-0000bf80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
-0000bf90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8f0: 6e6c 6f6e 6700 0000 0100 0000 1000 7400  nlong.........t.
+0000b900: 6800 7200 6500 6500 5f00 6400 6900 6d00  h.r.e.e._.d.i.m.
+0000b910: 6500 6e00 7300 6900 6f00 6e00 736c 6731  e.n.s.i.o.n.slg1
+0000b920: 5363 6f6d 7000 0000 0000 0332 ac00 0000  Scomp......2....
+0000b930: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
+0000b940: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
+0000b950: 736d 6f44 4462 6c6f 6200 0000 08f6 8857  smoDDblob......W
+0000b960: d65e 24c5 4100 0000 1000 7400 6800 7200  .^$.A.....t.h.r.
+0000b970: 6500 6500 5f00 6400 6900 6d00 6500 6e00  e.e._.d.i.m.e.n.
+0000b980: 7300 6900 6f00 6e00 736d 6f64 4462 6c6f  s.i.o.n.smodDblo
+0000b990: 6200 0000 08f6 8857 d65e 24c5 4100 0000  b......W.^$.A...
+0000b9a0: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
+0000b9b0: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
+0000b9c0: 7370 6831 5363 6f6d 7000 0000 0000 03a0  sph1Scomp.......
+0000b9d0: 0000 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
+0000b9e0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
+0000b9f0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+0000ba00: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+0000ba10: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+0000ba20: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+0000ba30: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+0000ba40: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+0000ba50: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+0000ba60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
+0000ba70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+0000ba80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
+0000ba90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+0000baa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
+0000bab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
+0000bac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
+0000bad0: 0000 0000 0011 9d6c 0000 0002 0075 0069  .......l.....u.i
+0000bae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
+0000baf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+0000bb00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
+0000bb10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+0000bb20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+0000bb30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+0000bb40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
+0000bb50: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
+0000bb60: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
+0000bb70: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
+0000bb80: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
+0000bb90: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+0000bba0: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
+0000bbb0: 6965 7209 1101 c709 546e 616d 65d4 100e  ier.....Tname...
+0000bbc0: 0f0d 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
+0000bbd0: 2308 08d4 100f 0e0d 1b18 1d0a 5c64 6174  #...........\dat
+0000bbe0: 654d 6f64 6966 6965 6408 10b5 09d4 100f  eModified.......
+0000bbf0: 0e0d 2018 1d18 5b64 6174 6543 7265 6174  .. ...[dateCreat
+0000bc00: 6564 0808 d410 0f0e 0d24 1826 0a54 7369  ed.......$.&.Tsi
+0000bc10: 7a65 0810 6109 d410 0f0e 0d29 0a2b 0a54  ze..a......).+.T
+0000bc20: 6b69 6e64 0910 7309 d410 0f0e 0d2e 0a30  kind..s........0
+0000bc30: 1855 6c61 6265 6c09 1064 08d4 100f 0e0d  .Ulabel..d......
+0000bc40: 330a 3518 5776 6572 7369 6f6e 0910 4b08  3.5.Wversion..K.
+0000bc50: d410 0f0e 0d38 0a3a 1858 636f 6d6d 656e  .....8.:.Xcommen
+0000bc60: 7473 0911 012c 08d4 100f 0e0d 3d18 3f18  ts...,......=.?.
+0000bc70: 5e64 6174 654c 6173 744f 7065 6e65 6408  ^dateLastOpened.
+0000bc80: 10c8 08d4 100e 0f0d 421d 1818 5964 6174  ........B...Ydat
+0000bc90: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
+0000bca0: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
+0000bcb0: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+0000bcc0: 7000 7900 8c00 8e00 8f00 9b00 a400 ac00  p.y.............
+0000bcd0: b200 bc00 c700 c800 cb00 cc00 d100 da00  ................
+0000bce0: e300 e500 e600 e700 f000 fd00 fe01 0001  ................
+0000bcf0: 0101 0a01 1601 1701 1801 2101 2601 2701  ..........!.&.'.
+0000bd00: 2901 2a01 3301 3801 3901 3b01 3c01 4501  ).*.3.8.9.;.<.E.
+0000bd10: 4b01 4c01 4e01 4f01 5801 6001 6101 6301  K.L.N.O.X.`.a.c.
+0000bd20: 6401 6d01 7601 7701 7a01 7b01 8401 9301  d.m.v.w.z.{.....
+0000bd30: 9401 9601 9701 a001 aa01 ab01 ac01 ad01  ................
+0000bd40: b601 bb01 c400 0000 0000 0002 0100 0000  ................
+0000bd50: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
+0000bd60: 0000 0001 c500 0000 0200 7500 696c 7376  ..........u.ilsv
+0000bd70: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+0000bd80: 30d8 0102 0304 0506 0708 090a 0b1a 4546  0.............EF
+0000bd90: 470a 5f10 1276 6965 774f 7074 696f 6e73  G._..viewOptions
+0000bda0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+0000bdb0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+0000bdc0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+0000bdd0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+0000bde0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+0000bdf0: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+0000be00: 4461 7465 7310 0109 d90c 0d0e 0f10 1112  Dates...........
+0000be10: 1314 151e 2327 2b30 353a 3f58 636f 6d6d  ....#'+05:?Xcomm
+0000be20: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+0000be30: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
+0000be40: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+0000be50: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+0000be60: 7369 6f6e 546e 616d 65d4 1617 1819 1a0a  sionTname.......
+0000be70: 1c1d 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
+0000be80: 6469 6e67 5577 6964 7468 5569 6e64 6578  dingUwidthUindex
+0000be90: 0809 1101 2c10 07d4 1617 1819 1a1a 2122  ....,.........!"
+0000bea0: 0808 10c8 1008 d416 1718 190a 1a26 0909  .............&..
+0000beb0: 0810 b5d4 1617 1819 1a1a 262a 0808 1002  ..........&*....
+0000bec0: d416 1718 190a 1a2e 2f09 0810 6110 03d4  ......../...a...
+0000bed0: 1617 1819 1a0a 3334 0809 1064 1005 d416  ......34...d....
+0000bee0: 1718 190a 0a38 3909 0910 7310 04d4 1617  .....89...s.....
+0000bef0: 1819 1a0a 3d3e 0809 104b 1006 d419 1817  ....=>...K......
+0000bf00: 1640 410a 0a10 0011 01c7 0909 0823 4028  .@A..........#@(
+0000bf10: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+0000bf20: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
+0000bf30: 5c00 6500 7000 7900 8c00 8e00 8f00 a200  \.e.p.y.........
+0000bf40: ab00 ba00 c700 d300 d800 de00 e300 eb00  ................
+0000bf50: f000 f901 0101 0b01 1101 1701 1801 1901  ................
+0000bf60: 1c01 1e01 2701 2801 2901 2b01 2d01 3601  ....'.(.).+.-.6.
+0000bf70: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
+0000bf80: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
+0000bf90: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
+0000bfa0: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
+0000bfb0: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
+0000bfc0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+0000bfd0: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
+0000bfe0: 6f44 4462 6c6f 6200 0000 087e abce 1cd0  oDDblob....~....
+0000bff0: 1fc5 4100 0000 0000 0000 0000 0000 0000  ..A.............
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_subsets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
 import numpy as np
-from typing import Union
+from typing import Union, Optional
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 from itertools import combinations
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.utils.enums import Formats, Options
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.checks import check_if_filepath_list_is_empty, check_file_exist_and_readable
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
+from simba.utils.errors import CountError
 
 
 class FeatureSubsetsCalculator(ConfigReader, FeatureExtractionMixin):
     """
     Computes a subset of features from pose for non-ML downstream purposes.
     E.g., returns the size of animal convex hull in each frame.
 
@@ -35,23 +36,26 @@
     ----------
     >>> _ = FeatureSubsetsCalculator(config_path='project_folder/project_config.ini', feature_family='Frame-by-frame body-parts inside ROIs (Boolean)', save_dir='data').run()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  save_dir: Union[str, os.PathLike],
-                 feature_family: Literal[Options.FEATURE_SUBSET_OPTIONS]):
+                 feature_family: Literal[Options.FEATURE_SUBSET_OPTIONS],
+                 append_to_features_extracted: Optional[bool] = False,
+                 append_to_targets_inserted: Optional[bool] = False):
 
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         ConfigReader.__init__(self, config_path=config_path)
         check_if_filepath_list_is_empty(
             filepaths=self.outlier_corrected_paths,
             error_msg=f"SIMBA ERROR: Zero data files found in {self.outlier_corrected_paths} directory",
         )
         self.feature_family, self.save_dir = feature_family, save_dir
+        self.append_to_features, self.append_to_targets = append_to_features_extracted, append_to_targets_inserted
 
     def __get_bp_combinations(self):
         self.two_point_combs = np.array(list(combinations(self.project_bps, 2)))
         self.within_animal_three_point_combs = {}
         self.within_animal_four_point_combs = {}
         self.animal_bps = {}
         for animal, animal_data in self.animal_bp_dict.items():
@@ -63,14 +67,15 @@
             self.within_animal_four_point_combs[animal] = np.array(
                 list(combinations(animal_bps, 4))
             )
 
     def run(self):
         self.__get_bp_combinations()
         for file_path in self.outlier_corrected_paths:
+            self.current_file_path = file_path
             self.video_timer = SimbaTimer(start=True)
             self.results = pd.DataFrame()
             _, self.video_name, _ = get_fn_ext(filepath=file_path)
             print(f"Analyzing {self.video_name} ({self.feature_family})...")
             _, self.pixel_per_mm, self.fps = self.read_video_info(
                 video_name=self.video_name
             )
@@ -273,23 +278,58 @@
                             self.results[
                                 f"{animal} {bp} inside polygon {shape_name} (Boolean)"
                             ] = self.framewise_inside_polygon_roi(
                                 bp_location=bp_arr, roi_coords=shape_data
                             )
 
     def __save(self):
+        if self.append_to_features:
+            file_path = os.path.join(self.features_dir, f"{self.video_name}.csv")
+            check_file_exist_and_readable(file_path=file_path)
+            features_df = read_df(file_path=file_path, file_type=self.file_type)
+            if len(features_df) != len(self.results):
+                raise CountError(f'Cannot append feature subsets to features file. The file used to create the feature subsets ({self.current_file_path}) contains data for {len(self.results)} frames, while the file representing the same video in features extracted folder ({file_path}) contains data for {len(features_df)} frames. Make sure the two files has an equal number of rows.')
+            new_features_df = pd.concat([features_df, self.results.round(2)], axis=1)
+            write_df(df=new_features_df, file_type=self.file_type, save_path=file_path)
+            del new_features_df
+            print(f'New features for video {self.video_name} saved in project_folder/csv/features_extracted directory...')
+
+        if self.append_to_targets:
+            file_path = os.path.join(self.targets_folder, f"{self.video_name}.csv")
+            check_file_exist_and_readable(file_path=file_path)
+            targets_df = read_df(file_path=file_path, file_type=self.file_type)
+            targets_clf_df = pd.DataFrame()
+
+            for clf in self.clf_names:
+                if clf in targets_df.columns:
+                    targets_clf_df[clf] = targets_df[clf]
+                    targets_df.drop(clf, axis=1, inplace=True)
+
+            new_targets_df = pd.concat([targets_df, self.results.round(2), targets_clf_df], axis=1)
+            write_df(df=new_targets_df, file_type=self.file_type, save_path=file_path)
+            del new_targets_df
+            print(f'New targets file for video {self.video_name} saved in project_folder/csv/targets_inserted directory...')
+
+
+
         save_path = os.path.join(self.save_dir, f"{self.video_name}.csv")
-        write_df(
-            df=self.results.round(2), file_type=Formats.CSV.value, save_path=save_path
-        )
+        write_df(df=self.results.round(2), file_type=Formats.CSV.value, save_path=save_path)
 
 
 # test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 feature_family='Frame-by-frame body-parts inside ROIs (Boolean)',
 #                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data')
 # test.run()
 
 
 # test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 feature_family='Frame-by-frame body-part movements (mm)',
 #                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data')
 # test.run()
+
+
+# test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                 feature_family='Frame-by-frame body-parts inside ROIs (Boolean)',
+#                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data',
+#                                 append_to_features_extracted=True,
+#                                 append_to_targets_inserted=True)
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/requirements.txt` & `Simba-UW-tf-dev-1.63.7/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 000b ead3 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0005 1733 0000 000b 005f 005f 0070  .....3....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 26a2 1753  moDDblob....&..S
-00000160: ee20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 a32a e599  moDDblob.....*..
+00000160: 8d20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 26a2 1753 ee20  dDblob....&..S. 
+00000180: 6444 626c 6f62 0000 0008 a32a e599 8d20  dDblob.....*... 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 000c f000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0006 a000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.63.7/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/enums.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/utils/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -253,20 +253,20 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0006 042d 0000 000b 005f 005f 0070  .....-....._._.p
+00001030: 0000 0006 052f 0000 000b 005f 005f 0070  ...../....._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 693d 1a27  moDDblob....i=.'
-00001060: ee20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 daad 7e57  moDDblob......~W
+00001060: 8022 c541 0000 000b 005f 005f 0070 0079  .".A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 693d 1a27 ee20  dDblob....i=.'. 
+00001080: 6444 626c 6f62 0000 0008 daad 7e57 8022  dDblob......~W."
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000010b0: 636f 6d70 0000 0000 0007 2000 0000 0003  comp...... .....
 000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
 000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/checks.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
 
 def read_df(file_path: Union[str, os.PathLike],
             file_type: Union[str, os.PathLike],
             has_index: Optional[bool] = True,
             remove_columns: Optional[List[str]] = None,
             usecols: Optional[List[str]] = None,
-            check_multiindex: bool = False) -> pd.DataFrame:
+            anipose_data: Optional[bool] = False,
+            check_multiindex: Optional[bool] = False) -> pd.DataFrame:
 
     """
     Read single tabular data file or pickle
 
     .. note::
        For improved runtime, defaults to :external:py:meth:`pyarrow.csv.write_cs` if file type is ``csv``.
 
@@ -69,15 +70,19 @@
     if file_type == Formats.CSV.value:
         try:
             df = csv.read_csv(file_path, parse_options=PARSE_OPTIONS, read_options=READ_OPTIONS)
             duplicate_headers = list(set([x for x in df.column_names if df.column_names.count(x) > 1]))
             if len(duplicate_headers) > 0:
                 new_headers = [duplicate_headers[0] + f'_{x}' for x in range(len(df.column_names))]
                 df = df.rename_columns(new_headers)
-            df = df.to_pandas().iloc[:, 1:]
+            if anipose_data:
+                df = df.to_pandas()
+                has_index = True
+            else:
+                df = df.to_pandas().iloc[:, 1:]
             if check_multiindex:
                 header_col_cnt = get_number_of_header_columns_in_df(df=df)
                 df = df.drop(df.index[list(range(0, header_col_cnt))]).apply(pd.to_numeric)
             if not has_index:
                 df = df.reset_index()
             else:
                 df = df.reset_index(drop=True)
@@ -130,15 +135,18 @@
             idx = np.arange(len(df)).astype(str)
             df.insert(0, '', idx)
             df = pa.Table.from_pandas(df=df)
             if '__index_level_0__' in df.columns:
                 df = df.drop(['__index_level_0__'])
             csv.write_csv(df, save_path)
         else:
-            df = df.drop('scorer', axis=1, errors='ignore')
+            try:
+                df = df.drop('scorer', axis=1, errors='ignore')
+            except TypeError:
+                pass
             df.to_csv(save_path)
     elif file_type == Formats.PARQUET.value:
         df.to_parquet(save_path)
     elif file_type == Formats.PICKLE.value:
         try:
             with open(save_path, 'wb') as f:
                 pickle.dump(df, f, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/errors.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/data.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/utils/printing.py` & `Simba-UW-tf-dev-1.63.7/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.63.7/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.63.7/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/st/app.py` & `Simba-UW-tf-dev-1.63.7/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/plotting/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
 00000230: 0000 000a 5a7d 0000 000b 005f 005f 0070  ....Z}....._._.p
 00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 a566 122d  moDDblob.....f.-
-00000260: ee20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
+00000250: 6d6f 4444 626c 6f62 0000 0008 71e6 4321  moDDblob....q.C!
+00000260: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
 00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 a566 122d ee20  dDblob.....f.-. 
+00000280: 6444 626c 6f62 0000 0008 71e6 4321 1721  dDblob....q.C!.!
 00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000002b0: 636f 6d70 0000 0000 000d 7000 0000 0005  comp......p.....
 000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
 000002d0: 6d70 0000 0000 0000 50f8 0000 0005 0074  mp......P......t
 000002e0: 006f 006f 006c 0073 6d6f 4444 626c 6f62  .o.o.l.smoDDblob
 000002f0: 0000 0008 1e86 d77f cc0c c541 0000 0005  ...........A....
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.63.7/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.63.7/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.63.7/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
 00000130: 0000 0004 7300 0000 000b 005f 005f 0070  ....s......_._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 1f94 bb4d  moDDblob.......M
-00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 41ed 4121  moDDblob....A.A!
+00000160: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 1f94 bb4d 7b20  dDblob.......M{ 
+00000180: 6444 626c 6f62 0000 0008 41ed 4121 1721  dDblob....A.A!.!
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000001b0: 636f 6d70 0000 0000 0005 f000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.63.7/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.63.7/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.63.7/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.63.7/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/.DS_Store`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
-00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0005 1733 0000 000b 005f 005f 0070  .....3....._._.p
-00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 a32a e599  moDDblob.....*..
-00000160: 8d20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
-00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 a32a e599 8d20  dDblob.....*... 
-00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0006 a000 0000 0000  comp............
+00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00000230: 0000 0002 3883 0000 000b 005f 005f 0070  ....8......_._.p
+00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00000250: 6d6f 4444 626c 6f62 0000 0008 fb7c 3914  moDDblob.....|9.
+00000260: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000280: 6444 626c 6f62 0000 0008 fb7c 3914 7b20  dDblob.....|9.{ 
+00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000002b0: 636f 6d70 0000 0000 0003 0000 0000 0004  comp............
+000002c0: 006d 0069 0073 0063 6473 636c 626f 6f6c  .m.i.s.cdsclbool
+000002d0: 0000 0000 0400 6d00 6900 7300 636c 6731  ......m.i.s.clg1
+000002e0: 5363 6f6d 7000 0000 0000 0037 0b00 0000  Scomp......7....
+000002f0: 0400 6d00 6900 7300 636d 6f44 4462 6c6f  ..m.i.s.cmoDDblo
+00000300: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
+00000310: 0400 6d00 6900 7300 636d 6f64 4462 6c6f  ..m.i.s.cmodDblo
+00000320: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
+00000330: 0400 6d00 6900 7300 6370 6831 5363 6f6d  ..m.i.s.cph1Scom
+00000340: 7000 0000 0000 0040 0000 0000 0000 0000  p......@........
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_define.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,14 +558,16 @@
                             'Name': self.name_box.get(),
                             'Shape_thickness': self.shape_thickness.get(),
                             'Shape_ear_tag_size': self.ear_tag_size.get(),
                             'Shape_color_name': self.color_var.get(),
                             'Shape_color_BGR': self.named_shape_colors[self.color_var.get()]}
 
         self.video_ROIs = self.image_data.initiate_draw(c_draw_settings)
+        #cv2.setWindowProperty('Define shape', cv2.WND_PROP_TOPMOST, 1)
+
         self.update_delete_ROI_menu()
 
     def update_delete_ROI_menu(self):
         self.selected_video.set(self.video_ROIs[0])
         self.roi_dropdown = OptionMenu(self.draw_frame, self.selected_video, *self.video_ROIs)
         self.roi_dropdown.grid(row=1, column=4, sticky=W, pady=10)
 
@@ -749,10 +751,10 @@
         image_data.text_size = self.text_size.get()
         image_data.text_thickness = self.text_thickness.get()
         image_data.line_type = self.line_type.get()
         image_data.duplicate_jump_size = self.duplicate_jump_size.get()
         stdout_success(msg='Saved ROI preference settings.')
 
 
-
-#test = ROI_definitions(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini',
+#
+# test = ROI_definitions(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/project_config.ini',
 #                       video_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/mouse_open_field/project_folder/videos/Video1.mp4')
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.btnset.grid(row=0,column=2)
         self.btnreset = Button(self,text='Reset',command =self.reset)
         self.btnreset.grid(row=0,column=3)
         self.btnapplyall = Button(self, text='Apply to all', command=self.applyall)
         self.btnapplyall.grid(row=0, column=4)
 
     def draw(self):
-        ROI_definitions(self.projectini,self.filename)
+        ROI_definitions(self.projectini, self.filename)
 
     def reset(self):
         reset_video_ROIs(self.projectini, self.filename)
 
     def applyall(self):
         multiply_ROIs(self.projectini, self.filename)
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.63.7/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/SimBA.py` & `Simba-UW-tf-dev-1.63.7/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/assets/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 0000 0001 4275 6431 0000 3800 0000 0800  ....Bud1..8.....
-00000010: 0000 3800 0000 100b 0000 300b 0000 200c  ..8.......0... .
-00000020: 0000 180b 0000 0000 0000 0000 0000 0800  ................
+00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
+00000010: 0000 1800 0000 100b 0000 040a 0000 200c  .............. .
+00000020: 0000 300c 0000 0000 0000 0000 0000 0800  ..0.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0003 0000 0001 0000 002c  ...............,
 00000050: 0000 0004 0000 1000 006f 006b 0075 0070  .........o.k.u.p
 00000060: 0073 6c73 0000 0000 0000 0000 0000 0000  .sls............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,79 +58,79 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
+00000400: 0000 0000 0000 0002 0000 0002 0000 0004  ................
+00000410: 0000 0007 006c 006f 006f 006b 0075 0070  .....l.o.o.k.u.p
+00000420: 0073 6c73 7643 626c 6f62 0000 0297 6270  .slsvCblob....bp
+00000430: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
+00000440: 0a0b 1949 4a0a 4c5f 1012 7669 6577 4f70  ...IJ.L_..viewOp
+00000450: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
+00000460: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00000470: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00000480: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+00000490: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
+000004a0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+000004b0: 7358 6963 6f6e 5369 7a65 1001 09ab 0c15  sXiconSize......
+000004c0: 1d22 262b 3035 3a3f 44d4 0d0e 0f10 0a0a  ."&+05:?D.......
+000004d0: 1314 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
+000004e0: 6469 6e67 5577 6964 7468 5a69 6465 6e74  dingUwidthZident
+000004f0: 6966 6965 7209 0911 01d5 546e 616d 65d4  ifier.....Tname.
+00000500: 1617 1810 191a 191c 5776 6973 6962 6c65  ........Wvisible
+00000510: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00000520: 0810 2308 5875 6269 7175 6974 79d4 0d0e  ..#.Xubiquity...
+00000530: 0f10 0a19 2021 0908 10b5 5c64 6174 654d  .... !....\dateM
+00000540: 6f64 6966 6965 64d4 0d0e 0f10 1919 2025  odified....... %
+00000550: 0808 5b64 6174 6543 7265 6174 6564 d40d  ..[dateCreated..
+00000560: 0e0f 100a 1929 2a09 0810 6154 7369 7a65  .....)*...aTsize
+00000570: d40d 0e0f 100a 0a2e 2f09 0910 7354 6b69  ......../...sTki
+00000580: 6e64 d40d 0e0f 1019 0a33 3408 0910 6455  nd.......34...dU
+00000590: 6c61 6265 6cd4 0d0e 0f10 190a 3839 0809  label.......89..
+000005a0: 104b 5776 6572 7369 6f6e d40d 0e0f 1019  .KWversion......
+000005b0: 0a3d 3e08 0911 012c 5863 6f6d 6d65 6e74  .=>....,Xcomment
+000005c0: 73d4 0d0e 0f10 1919 4243 0808 10c8 5e64  s.......BC....^d
+000005d0: 6174 654c 6173 744f 7065 6e65 64d4 1617  ateLastOpened...
+000005e0: 1810 1920 1947 0808 5964 6174 6541 6464  ... .G..YdateAdd
+000005f0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
+00000600: 6509 2340 3000 0000 0000 0000 0800 1900  e.#@0...........
+00000610: 2e00 4000 4800 5c00 6500 7000 8300 8c00  ..@.H.\.e.p.....
+00000620: 8e00 8f00 9b00 a400 ac00 b600 bc00 c700  ................
+00000630: c800 c900 cc00 d100 da00 e200 e800 f200  ................
+00000640: f300 f500 f600 ff01 0801 0901 0a01 0c01  ................
+00000650: 1901 2201 2301 2401 3001 3901 3a01 3b01  ..".#.$.0.9.:.;.
+00000660: 3d01 4201 4b01 4c01 4d01 4f01 5401 5d01  =.B.K.L.M.O.T.].
+00000670: 5e01 5f01 6101 6701 7001 7101 7201 7401  ^._.a.g.p.q.r.t.
+00000680: 7c01 8501 8601 8701 8a01 9301 9c01 9d01  |...............
+00000690: 9e01 a001 af01 b801 b901 ba01 c401 c501  ................
+000006a0: ce01 d301 d400 0000 0000 0002 0100 0000  ................
+000006b0: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
+000006c0: 0000 0001 dd00 0000 0500 0000 0400 7300  ..............s.
+000006d0: 6800 6100 706d 6f44 4462 6c6f 6200 0000  h.a.pmoDDblob...
+000006e0: 0801 843b 74e2 ddc4 4153 636f 6d70 0000  ...;t...AScomp..
+000006f0: 0000 0004 e000 0000 0007 006c 006f 006f  ...........l.o.o
+00000700: 006b 0075 0070 0073 7653 726e 6c6f 6e67  .k.u.p.svSrnlong
+00000710: 0000 0001 0000 0004 0073 0068 0061 0070  .........s.h.a.p
+00000720: 6277 7370 626c 6f62 0000 00b9 6270 6c69  bwspblob....bpli
+00000730: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00000740: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00000750: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00000760: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00000770: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00000780: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00000790: 5369 6465 6261 7208 0908 095f 1019 7b7b  Sidebar...._..{{
+000007a0: 3130 342c 2031 3632 7d2c 207b 3131 3933  104, 162}, {1193
+000007b0: 2c20 3731 337d 7d09 0815 232f 3b52 5f6b  , 713}}...#/;R_k
+000007c0: 6c6d 6e6f 8b00 0000 0000 0001 0100 0000  lmno............
+000007d0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
+000007e0: 0000 0000 8c00 0000 0400 7300 6800 6100  ..........s.h.a.
+000007f0: 706c 6731 5363 6f6d 7000 0000 0000 0927  plg1Scomp......'
+00000800: 3400 0000 0000 0001 0000 0000 0000 080b  4...............
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,222 +250,222 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0010 0000 0004  ................
-00001010: 0073 0068 0061 0070 6d6f 4444 626c 6f62  .s.h.a.pmoDDblob
+00001000: 0000 0000 0000 0000 0000 000f 0000 0004  ................
+00001010: 0073 0068 0061 0070 6d6f 6444 626c 6f62  .s.h.a.pmodDblob
 00001020: 0000 0008 0184 3b74 e2dd c441 0000 0004  ......;t...A....
-00001030: 0073 0068 0061 0070 6d6f 6444 626c 6f62  .s.h.a.pmodDblob
-00001040: 0000 0008 0184 3b74 e2dd c441 0000 0004  ......;t...A....
-00001050: 0073 0068 0061 0070 7068 3153 636f 6d70  .s.h.a.pph1Scomp
-00001060: 0000 0000 0009 d000 0000 0004 0073 0068  .............s.h
-00001070: 0061 0070 7653 726e 6c6f 6e67 0000 0001  .a.pvSrnlong....
-00001080: 0000 0003 0073 0074 006c 6277 7370 626c  .....s.t.lbwspbl
-00001090: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-000010a0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-000010b0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-000010c0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-000010d0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-000010e0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-000010f0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00001100: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00001110: 0809 0809 5f10 197b 7b31 3034 2c20 3136  ...._..{{104, 16
-00001120: 347d 2c20 7b31 3139 332c 2037 3133 7d7d  4}, {1193, 713}}
-00001130: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00001140: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00001150: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-00001160: 0000 0003 0073 0074 006c 6c67 3153 636f  .....s.t.llg1Sco
-00001170: 6d70 0000 0000 0053 7f67 0000 0003 0073  mp.....S.g.....s
-00001180: 0074 006c 6c73 7643 626c 6f62 0000 0272  .t.llsvCblob...r
-00001190: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-000011a0: 0809 0a0b 1646 1447 0a5f 1012 7669 6577  .....F.G._..view
-000011b0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-000011c0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-000011d0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-000011e0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-000011f0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00001200: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
-00001210: 656c 6174 6976 6544 6174 6573 1001 09ab  elativeDates....
-00001220: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
-00001230: 0a12 0a14 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
-00001240: 7468 5961 7363 656e 6469 6e67 5a69 6465  thYascendingZide
-00001250: 6e74 6966 6965 7209 1102 9709 546e 616d  ntifier.....Tnam
-00001260: 65d4 0d0e 0f10 1617 1619 0810 2308 5875  e...........#.Xu
-00001270: 6269 7175 6974 79d4 0d0e 0f10 0a1c 161e  biquity.........
-00001280: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00001290: 64d4 0d0e 0f10 161c 1622 0808 5b64 6174  d........"..[dat
-000012a0: 6543 7265 6174 6564 d40d 0e0f 100a 2516  eCreated......%.
-000012b0: 2709 1061 0854 7369 7a65 d40d 0e0f 100a  '..a.Tsize......
-000012c0: 2a0a 2c09 1073 0954 6b69 6e64 d40d 0e0f  *.,..s.Tkind....
-000012d0: 1016 2f0a 3108 1064 0955 6c61 6265 6cd4  ../.1..d.Ulabel.
-000012e0: 0d0e 0f10 1634 0a36 0810 4b09 5776 6572  .....4.6..K.Wver
-000012f0: 7369 6f6e d40d 0e0f 1016 390a 3b08 1101  sion......9.;...
-00001300: 2c09 5863 6f6d 6d65 6e74 73d4 0d0e 0f10  ,.Xcomments.....
-00001310: 163e 1640 0810 c808 5e64 6174 654c 6173  .>.@....^dateLas
-00001320: 744f 7065 6e65 64d4 0d0e 0f10 161c 1644  tOpened........D
-00001330: 0808 5964 6174 6541 6464 6564 0823 4028  ..YdateAdded.#@(
-00001340: 0000 0000 0000 2340 3000 0000 0000 0009  ......#@0.......
-00001350: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
-00001360: 0079 008c 008e 008f 009b 00a4 00ac 00b2  .y..............
-00001370: 00bc 00c7 00c8 00cb 00cc 00d1 00da 00db  ................
-00001380: 00dd 00de 00e7 00f0 00f1 00f3 00f4 0101  ................
-00001390: 010a 010b 010c 0118 0121 0122 0124 0125  .........!.".$.%
-000013a0: 012a 0133 0134 0136 0137 013c 0145 0146  .*.3.4.6.7.<.E.F
-000013b0: 0148 0149 014f 0158 0159 015b 015c 0164  .H.I.O.X.Y.[.\.d
-000013c0: 016d 016e 0171 0172 017b 0184 0185 0187  .m.n.q.r.{......
-000013d0: 0188 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
-000013e0: 01bf 0000 0000 0000 0201 0000 0000 0000  ................
-000013f0: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00001400: 01c0 0000 0003 0073 0074 006c 6c73 7670  .......s.t.llsvp
-00001410: 626c 6f62 0000 0257 6270 6c69 7374 3030  blob...Wbplist00
-00001420: d801 0203 0405 0607 0809 0a0b 1d45 1446  .............E.F
-00001430: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
-00001440: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-00001450: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00001460: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00001470: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00001480: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-00001490: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-000014a0: 6174 6573 1001 09d9 0c0d 0e0f 1011 1213  ates............
-000014b0: 1415 1e23 272b 3035 3a3f 5863 6f6d 6d65  ...#'+05:?Xcomme
-000014c0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-000014d0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
-000014e0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-000014f0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-00001500: 696f 6e54 6e61 6d65 d416 1718 191a 1b0a  ionTname........
-00001510: 1d55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
-00001520: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
-00001530: 0711 012c 0908 d416 1718 191f 201d 1d10  ...,........ ...
-00001540: 0810 c808 08d4 1617 1819 0924 1d0a 10b5  ...........$....
-00001550: 0809 d416 1718 1928 241d 1d10 0208 08d4  .......($.......
-00001560: 1617 1819 2c2d 1d0a 1003 1061 0809 d416  ....,-.....a....
-00001570: 1718 1931 320a 1d10 0510 6409 08d4 1617  ...12.....d.....
-00001580: 1819 3637 0a0a 1004 1073 0909 d416 1718  ..67.....s......
-00001590: 193b 3c0a 1d10 0610 4b09 08d4 1617 1819  .;<.....K.......
-000015a0: 4041 0a0a 1000 1102 9709 0908 2340 2800  @A..........#@(.
-000015b0: 0000 0000 0023 4030 0000 0000 0000 0900  .....#@0........
-000015c0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-000015d0: 7900 8c00 8e00 8f00 a200 ab00 ba00 c700  y...............
-000015e0: d300 d800 de00 e300 eb00 f000 f900 ff01  ................
-000015f0: 0501 0f01 1701 1901 1c01 1d01 1e01 2701  ..............'.
-00001600: 2901 2b01 2c01 2d01 3601 3801 3901 3a01  ).+.,.-.6.8.9.:.
-00001610: 4301 4501 4601 4701 5001 5201 5401 5501  C.E.F.G.P.R.T.U.
-00001620: 5601 5f01 6101 6301 6401 6501 6e01 7001  V._.a.c.d.e.n.p.
-00001630: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
-00001640: 8c01 8e01 9101 9201 9301 9401 9d01 a600  ................
-00001650: 0000 0000 0002 0100 0000 0000 0000 4800  ..............H.
-00001660: 0000 0000 0000 0000 0000 0000 0001 a700  ................
-00001670: 0000 0300 7300 7400 6c6d 6f44 4462 6c6f  ....s.t.lmoDDblo
-00001680: 6200 0000 0869 be3e 74e2 ddc4 4100 0000  b....i.>t...A...
-00001690: 0300 7300 7400 6c6d 6f64 4462 6c6f 6200  ..s.t.lmodDblob.
-000016a0: 0000 0869 be3e 74e2 ddc4 4100 0000 0300  ...i.>t...A.....
-000016b0: 7300 7400 6c70 6831 5363 6f6d 7000 0000  s.t.lph1Scomp...
-000016c0: 0000 53a0 0000 0000 0300 7300 7400 6c76  ..S.......s.t.lv
-000016d0: 5372 6e6c 6f6e 6700 0000 0100 0000 0c00  Srnlong.........
-000016e0: 7500 6e00 7300 7500 7000 6500 7200 7600  u.n.s.u.p.e.r.v.
-000016f0: 6900 7300 6500 646c 6731 5363 6f6d 7000  i.s.e.dlg1Scomp.
-00001700: 0000 0000 01fb 0e00 0000 0c00 7500 6e00  ............u.n.
-00001710: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
-00001720: 6500 646d 6f44 4462 6c6f 6200 0000 08d4  e.dmoDDblob.....
-00001730: e33e 74e2 ddc4 4100 0000 0c00 7500 6e00  .>t...A.....u.n.
-00001740: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
-00001750: 6500 646d 6f64 4462 6c6f 6200 0000 08d4  e.dmodDblob.....
-00001760: e33e 74e2 ddc4 4100 0000 0c00 7500 6e00  .>t...A.....u.n.
-00001770: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
-00001780: 6500 6470 6831 5363 6f6d 7000 0000 0000  e.dph1Scomp.....
-00001790: 0210 0000 0000 0000 0000 0000 0000 0000  ................
-000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001800: 0000 0000 0000 0000 0000 0008 0000 0007  ................
-00001810: 006c 006f 006f 006b 0075 0070 0073 6c73  .l.o.o.k.u.p.sls
-00001820: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
-00001830: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
-00001840: 460a 485f 1012 7669 6577 4f70 7469 6f6e  F.H_..viewOption
-00001850: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00001860: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00001870: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00001880: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00001890: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000018a0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
-000018b0: 6f6e 5369 7a65 1001 09d9 0c0d 0e0f 1011  onSize..........
-000018c0: 1213 1415 1e23 282d 3237 3c41 5863 6f6d  .....#(-27<AXcom
-000018d0: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
-000018e0: 656e 6564 5b64 6174 6543 7265 6174 6564  ened[dateCreated
-000018f0: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-00001900: 5776 6572 7369 6f6e 546e 616d 655c 6461  WversionTname\da
-00001910: 7465 4d6f 6469 6669 6564 d416 1718 191a  teModified......
-00001920: 0a1c 1d55 696e 6465 7859 6173 6365 6e64  ...UindexYascend
-00001930: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00001940: 6510 0709 1101 2c08 d416 1718 191f 1d21  e.....,........!
-00001950: 1d10 0808 10c8 08d4 1617 1819 241d 261d  ............$.&.
-00001960: 1002 0810 b508 d416 1718 1929 1d2b 0a10  ...........).+..
-00001970: 0308 1061 09d4 1617 1819 2e0a 301d 1005  ...a........0...
-00001980: 0910 6408 d416 1718 1933 0a35 0a10 0409  ..d......3.5....
-00001990: 1073 09d4 1617 1819 380a 3a1d 1006 0910  .s......8.:.....
-000019a0: 4b08 d416 1718 193d 0a3f 0a10 0009 1101  K......=.?......
-000019b0: d509 d416 1718 1909 1d26 0a08 0908 2340  .........&....#@
-000019c0: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
-000019d0: 0000 0000 0000 0008 0019 002e 0040 0048  .............@.H
-000019e0: 005c 0065 0070 0083 008c 008e 008f 00a2  .\.e.p..........
-000019f0: 00ab 00ba 00c6 00cb 00d1 00d6 00de 00e3  ................
-00001a00: 00f0 00f9 00ff 0109 010f 0117 0119 011a  ................
-00001a10: 011d 011e 0127 0129 012a 012c 012d 0136  .....'.).*.,.-.6
-00001a20: 0138 0139 013b 013c 0145 0147 0148 014a  .8.9.;.<.E.G.H.J
-00001a30: 014b 0154 0156 0157 0159 015a 0163 0165  .K.T.V.W.Y.Z.c.e
-00001a40: 0166 0168 0169 0172 0174 0175 0177 0178  .f.h.i.r.t.u.w.x
-00001a50: 0181 0183 0184 0187 0188 0191 0192 0193  ................
-00001a60: 0194 019d 01a2 01a3 0000 0000 0000 0201  ................
-00001a70: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
-00001a80: 0000 0000 0000 01ac 0000 0007 006c 006f  .............l.o
-00001a90: 006f 006b 0075 0070 0073 6d6f 4444 626c  .o.k.u.p.smoDDbl
-00001aa0: 6f62 0000 0008 1a04 dcb9 b8e5 c441 0000  ob...........A..
-00001ab0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
-00001ac0: 6d6f 6444 626c 6f62 0000 0008 1a04 dcb9  modDblob........
-00001ad0: b8e5 c441 0000 0007 006c 006f 006f 006b  ...A.....l.o.o.k
-00001ae0: 0075 0070 0073 7068 3153 636f 6d70 0000  .u.p.sph1Scomp..
-00001af0: 0000 0004 e000 0000 0007 006c 006f 006f  ...........l.o.o
-00001b00: 006b 0075 0070 0073 7653 726e 6c6f 6e67  .k.u.p.svSrnlong
-00001b10: 0000 0001 0000 0004 0073 0068 0061 0070  .........s.h.a.p
-00001b20: 6277 7370 626c 6f62 0000 00b9 6270 6c69  bwspblob....bpli
-00001b30: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
-00001b40: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001b50: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00001b60: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00001b70: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00001b80: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00001b90: 5369 6465 6261 7208 0908 095f 1019 7b7b  Sidebar...._..{{
-00001ba0: 3130 342c 2031 3632 7d2c 207b 3131 3933  104, 162}, {1193
-00001bb0: 2c20 3731 337d 7d09 0815 232f 3b52 5f6b  , 713}}...#/;R_k
-00001bc0: 6c6d 6e6f 8b00 0000 0000 0001 0100 0000  lmno............
-00001bd0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00001be0: 0000 0000 8c00 0000 0400 7300 6800 6100  ..........s.h.a.
-00001bf0: 706c 6731 5363 6f6d 7000 0000 0000 0927  plg1Scomp......'
-00001c00: 3400 0000 0400 7300 6800 6100 706c 7376  4.....s.h.a.plsv
-00001c10: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
-00001c20: 30d8 0102 0304 0506 0708 090a 0b18 4647  0.............FG
-00001c30: 0a49 5869 636f 6e53 697a 655f 100f 7368  .IXiconSize_..sh
-00001c40: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00001c50: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00001c60: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00001c70: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00001c80: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00001c90: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001ca0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
-00001cb0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
-00001cc0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00001cd0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00001ce0: 7669 7369 626c 6554 6e61 6d65 1101 2709  visibleTname..'.
-00001cf0: 09d4 0d0e 0f10 1617 1818 5875 6269 7175  ..........Xubiqu
+00001030: 0073 0068 0061 0070 7068 3153 636f 6d70  .s.h.a.pph1Scomp
+00001040: 0000 0000 0009 d000 0000 0004 0073 0068  .............s.h
+00001050: 0061 0070 7653 726e 6c6f 6e67 0000 0001  .a.pvSrnlong....
+00001060: 0000 0003 0073 0074 006c 6277 7370 626c  .....s.t.lbwspbl
+00001070: 6f62 0000 00b5 6270 6c69 7374 3030 d601  ob....bplist00..
+00001080: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00001090: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+000010a0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+000010b0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+000010c0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+000010d0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+000010e0: 7208 0908 095f 1015 7b7b 302c 2035 7d2c  r...._..{{0, 5},
+000010f0: 207b 3134 3237 2c20 3837 307d 7d09 0815   {1427, 870}}...
+00001100: 232f 3b52 5f6b 6c6d 6e6f 8700 0000 0000  #/;R_klmno......
+00001110: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
+00001120: 0000 0000 0000 0000 0000 8800 0000 0300  ................
+00001130: 7300 7400 6c6c 6731 5363 6f6d 7000 0000  s.t.llg1Scomp...
+00001140: 0000 537f 6700 0000 0300 7300 7400 6c6c  ..S.g.....s.t.ll
+00001150: 7376 4362 6c6f 6200 0003 0662 706c 6973  svCblob....bplis
+00001160: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+00001170: 5657 0a59 5869 636f 6e53 697a 655f 100f  VW.YXiconSize_..
+00001180: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00001190: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+000011a0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+000011b0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+000011c0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+000011d0: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+000011e0: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+000011f0: 09ae 0c15 1a1f 2328 2d32 373c 4145 4d51  ......#(-27<AEMQ
+00001200: d40d 0e0f 1011 120a 0a5a 6964 656e 7469  .........Zidenti
+00001210: 6669 6572 5577 6964 7468 5961 7363 656e  fierUwidthYascen
+00001220: 6469 6e67 5776 6973 6962 6c65 546e 616d  dingWvisibleTnam
+00001230: 6510 a709 09d4 0d0e 0f10 1617 1818 5875  e.............Xu
+00001240: 6269 7175 6974 7910 2308 08d4 0d0e 0f10  biquity.#.......
+00001250: 1b1c 180a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00001260: 6410 b508 09d4 0d0e 0f10 201c 1818 5b64  d......... ...[d
+00001270: 6174 6543 7265 6174 6564 0808 d40d 0e0f  ateCreated......
+00001280: 1024 2518 0a54 7369 7a65 1061 0809 d40d  .$%..Tsize.a....
+00001290: 0e0f 1029 2a0a 0a54 6b69 6e64 1073 0909  ...)*..Tkind.s..
+000012a0: d40d 0e0f 102e 2f0a 1855 6c61 6265 6c10  ....../..Ulabel.
+000012b0: 6409 08d4 0d0e 0f10 3334 0a18 5776 6572  d.......34..Wver
+000012c0: 7369 6f6e 104b 0908 d40d 0e0f 1038 390a  sion.K.......89.
+000012d0: 1858 636f 6d6d 656e 7473 1101 2c09 08d4  .Xcomments..,...
+000012e0: 0d0e 0f10 3d3e 1818 5e64 6174 654c 6173  ....=>..^dateLas
+000012f0: 744f 7065 6e65 6410 c808 08d4 0d0e 0f10  tOpened.........
+00001300: 421c 1818 5964 6174 6541 6464 6564 0808  B...YdateAdded..
+00001310: d40d 4647 4849 4a18 1855 7769 6474 6859  ..FGHIJ..UwidthY
+00001320: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+00001330: 655a 7368 6172 654f 776e 6572 10d2 0808  eZshareOwner....
+00001340: d40d 4647 484e 4a18 185f 100f 7368 6172  ..FGHNJ.._..shar
+00001350: 654c 6173 7445 6469 746f 7208 08d4 0d46  eLastEditor....F
+00001360: 4748 524a 1818 5f10 1069 6e76 6974 6174  GHRJ.._..invitat
+00001370: 696f 6e53 7461 7475 7308 0808 2340 2800  ionStatus...#@(.
+00001380: 0000 0000 0054 6e61 6d65 0910 0100 0800  .....Tname......
+00001390: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
+000013a0: 8c00 9500 9600 a500 ae00 b900 bf00 c900  ................
+000013b0: d100 d600 d800 d900 da00 e300 ec00 ee00  ................
+000013c0: ef00 f000 f901 0601 0801 0901 0a01 1301  ................
+000013d0: 1f01 2001 2101 2a01 2f01 3101 3201 3301  .. .!.*./.1.2.3.
+000013e0: 3c01 4101 4301 4401 4501 4e01 5401 5601  <.A.C.D.E.N.T.V.
+000013f0: 5701 5801 6101 6901 6b01 6c01 6d01 7601  W.X.a.i.k.l.m.v.
+00001400: 7f01 8201 8301 8401 8d01 9c01 9e01 9f01  ................
+00001410: a001 a901 b301 b401 b501 be01 c401 ce01  ................
+00001420: d601 e101 e301 e401 e501 ee02 0002 0102  ................
+00001430: 0202 0b02 1e02 1f02 2002 2102 2a02 2f02  ........ .!.*./.
+00001440: 3000 0000 0000 0002 0100 0000 0000 0000  0...............
+00001450: 5a00 0000 0000 0000 0000 0000 0000 0002  Z...............
+00001460: 3200 0000 0300 7300 7400 6c6c 7376 7062  2.....s.t.llsvpb
+00001470: 6c6f 6200 0002 5d62 706c 6973 7430 30d8  lob...]bplist00.
+00001480: 0102 0304 0506 0708 090a 0b1a 4647 0a35  ............FG.5
+00001490: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+000014a0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+000014b0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+000014c0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+000014d0: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+000014e0: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+000014f0: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00001500: 696f 6e23 4030 0000 0000 0000 09d9 0c0d  ion#@0..........
+00001510: 0e0f 1011 1213 1415 1e23 282d 3236 3b40  .........#(-26;@
+00001520: 5863 6f6d 6d65 6e74 7355 6c61 6265 6c57  XcommentsUlabelW
+00001530: 7665 7273 696f 6e5b 6461 7465 4372 6561  version[dateCrea
+00001540: 7465 6454 7369 7a65 5c64 6174 654d 6f64  tedTsize\dateMod
+00001550: 6966 6965 6454 6b69 6e64 546e 616d 655e  ifiedTkindTname^
+00001560: 6461 7465 4c61 7374 4f70 656e 6564 d416  dateLastOpened..
+00001570: 1718 191a 1b0a 1d57 7669 7369 626c 6555  .......WvisibleU
+00001580: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
+00001590: 696e 6465 7808 1101 2c09 1007 d416 1718  index...,.......
+000015a0: 191a 200a 2208 1064 0910 05d4 1617 1819  .. ."..d........
+000015b0: 1a25 0a27 0810 4b09 1006 d416 1718 191a  .%.'..K.........
+000015c0: 2a1a 2c08 10b5 0810 02d4 1617 1819 0a2f  *.,............/
+000015d0: 1a31 0910 6108 1003 d416 1718 190a 2a1a  .1..a.........*.
+000015e0: 3509 0810 01d4 1617 1819 0a38 0a3a 0910  5..........8.:..
+000015f0: 7309 1004 d416 1718 190a 3d0a 3f09 10a7  s.........=.?...
+00001600: 0910 00d4 1617 1819 1a42 1a44 0810 c808  .........B.D....
+00001610: 1008 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00001620: 6509 0008 0019 0022 0034 003c 0050 0059  e......".4.<.P.Y
+00001630: 0064 0077 008c 0095 0096 00a9 00b2 00b8  .d.w............
+00001640: 00c0 00cc 00d1 00de 00e3 00e8 00f7 0100  ................
+00001650: 0108 010e 0118 011e 011f 0122 0123 0125  ...........".#.%
+00001660: 012e 012f 0131 0132 0134 013d 013e 0140  .../.1.2.4.=.>.@
+00001670: 0141 0143 014c 014d 014f 0150 0152 015b  .A.C.L.M.O.P.R.[
+00001680: 015c 015e 015f 0161 016a 016b 016c 016e  .\.^._.a.j.k.l.n
+00001690: 0177 0178 017a 017b 017d 0186 0187 0189  .w.x.z.{.}......
+000016a0: 018a 018c 0195 0196 0198 0199 019b 019c  ................
+000016b0: 01a5 01aa 0000 0000 0000 0201 0000 0000  ................
+000016c0: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
+000016d0: 0000 01ab 0000 0003 0073 0074 006c 6d6f  .........s.t.lmo
+000016e0: 4444 626c 6f62 0000 0008 69be 3e74 e2dd  DDblob....i.>t..
+000016f0: c441 0000 0003 0073 0074 006c 6d6f 6444  .A.....s.t.lmodD
+00001700: 626c 6f62 0000 0008 69be 3e74 e2dd c441  blob....i.>t...A
+00001710: 0000 0003 0073 0074 006c 7068 3153 636f  .....s.t.lph1Sco
+00001720: 6d70 0000 0000 0053 a000 0000 0003 0073  mp.....S.......s
+00001730: 0074 006c 7653 726e 6c6f 6e67 0000 0001  .t.lvSrnlong....
+00001740: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
+00001750: 0072 0076 0069 0073 0065 0064 6c67 3153  .r.v.i.s.e.dlg1S
+00001760: 636f 6d70 0000 0000 0001 fb0e 0000 000c  comp............
+00001770: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+00001780: 0069 0073 0065 0064 6d6f 4444 626c 6f62  .i.s.e.dmoDDblob
+00001790: 0000 0008 d4e3 3e74 e2dd c441 0000 000c  ......>t...A....
+000017a0: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+000017b0: 0069 0073 0065 0064 6d6f 6444 626c 6f62  .i.s.e.dmodDblob
+000017c0: 0000 0008 d4e3 3e74 e2dd c441 0000 000c  ......>t...A....
+000017d0: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+000017e0: 0069 0073 0065 0064 7068 3153 636f 6d70  .i.s.e.dph1Scomp
+000017f0: 0000 0000 0002 1000 0000 0000 0000 0000  ................
+00001800: 0000 0000 0000 0006 0000 0000 0000 180b  ................
+00001810: 0000 0045 0000 100b 0000 040a 0000 200c  ...E.......... .
+00001820: 0000 300c 0000 0000 0000 0000 0000 0000  ..0.............
+00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00001c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00001c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001c50: 0100 0002 0000 0000 0000 0000 0100 0008  ................
+00001c60: 0000 0000 0000 0000 0000 0000 0100 0040  ...............@
+00001c70: 0000 0000 0100 0080 0000 0000 0100 0100  ................
+00001c80: 0000 0000 0100 0200 0000 0000 0100 0400  ................
+00001c90: 0000 0000 0100 0800 0000 0000 0100 1000  ................
+00001ca0: 0000 0000 0100 2000 0000 0000 0100 4000  ...... .......@.
+00001cb0: 0000 0000 0100 8000 0000 0000 0101 0000  ................
+00001cc0: 0000 0000 0102 0000 0000 0000 0104 0000  ................
+00001cd0: 0000 0000 0108 0000 0000 0000 0110 0000  ................
+00001ce0: 0000 0000 0120 0000 0000 0000 0140 0000  ..... .......@..
+00001cf0: 0000 0000 0010 1617 1818 5875 6269 7175  ..........Xubiqu
 00001d00: 6974 7910 2308 08d4 0d0e 0f10 1b1c 180a  ity.#...........
 00001d10: 5c64 6174 654d 6f64 6966 6965 6410 b508  \dateModified...
 00001d20: 09d4 0d0e 0f10 201c 1818 5b64 6174 6543  ...... ...[dateC
 00001d30: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
 00001d40: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
 00001d50: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
 00001d60: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
@@ -483,38 +483,38 @@
 00001e20: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00001e30: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00001e40: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00001e50: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00001e60: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00001e70: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00001e80: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00001e90: 01c5 6801 6901 6b01 7401 7501 7701 7801  ..h.i.k.t.u.w.x.
-00001ea0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
-00001eb0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
-00001ec0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
-00001ed0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
-00001ee0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-00001ef0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
-00001f00: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
-00001f10: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
-00001f20: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
-00001f30: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
-00001f40: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
-00001f50: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
-00001f60: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
-00001f70: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00001f80: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
-00001f90: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00001fa0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00001fb0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00001fc0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00001fd0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00001fe0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00001ff0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00002000: 7b33 3335 0000 0000 0000 0012 0000 0005  {335............
+00001e90: 01c5 0000 0004 0073 0068 0061 0070 6c73  .......s.h.a.pls
+00001ea0: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
+00001eb0: 3030 d801 0203 0405 0607 0809 0a0b 1a46  00.............F
+00001ec0: 470a 2758 6963 6f6e 5369 7a65 5f10 0f73  G.'XiconSize_..s
+00001ed0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00001ee0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00001ef0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+00001f00: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
+00001f10: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00001f20: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
+00001f30: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
+00001f40: d90c 0d0e 0f10 1112 1314 151e 2328 2c31  ............#(,1
+00001f50: 363b 4058 636f 6d6d 656e 7473 5e64 6174  6;@Xcomments^dat
+00001f60: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
+00001f70: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
+00001f80: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+00001f90: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+00001fa0: 65d4 1617 1819 1a1b 0a1d 5776 6973 6962  e.........Wvisib
+00001fb0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00001fc0: 6e67 5569 6e64 6578 0811 012c 0910 07d4  ngUindex...,....
+00001fd0: 1617 1819 1a20 1a22 0810 c808 1008 d416  ..... ."........
+00001fe0: 1718 190a 251a 2709 10b5 0810 01d4 1617  ....%.'.........
+00001ff0: 1819 1a25 1a2b 0808 1002 d416 1718 190a  ...%.+..........
+00002000: 2e1a 3009 0000 0000 0000 0012 0000 0005  ..0.............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
 00002020: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00002030: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00002040: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00002050: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00002060: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00002070: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
@@ -762,98 +762,98 @@
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003000: 0000 0000 0000 0002 0000 0002 0000 0004  ................
-00003010: 0000 0007 006c 006f 006f 006b 0075 0070  .....l.o.o.k.u.p
-00003020: 0073 6c73 7643 626c 6f62 0000 0297 6270  .slsvCblob....bp
-00003030: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
-00003040: 0a0b 1949 4a0a 4c5f 1012 7669 6577 4f70  ...IJ.L_..viewOp
-00003050: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
-00003060: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-00003070: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-00003080: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
-00003090: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
-000030a0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-000030b0: 7358 6963 6f6e 5369 7a65 1001 09ab 0c15  sXiconSize......
-000030c0: 1d22 262b 3035 3a3f 44d4 0d0e 0f10 0a0a  ."&+05:?D.......
-000030d0: 1314 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
-000030e0: 6469 6e67 5577 6964 7468 5a69 6465 6e74  dingUwidthZident
-000030f0: 6966 6965 7209 0911 01d5 546e 616d 65d4  ifier.....Tname.
-00003100: 1617 1810 191a 191c 5776 6973 6962 6c65  ........Wvisible
-00003110: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00003120: 0810 2308 5875 6269 7175 6974 79d4 0d0e  ..#.Xubiquity...
-00003130: 0f10 0a19 2021 0908 10b5 5c64 6174 654d  .... !....\dateM
-00003140: 6f64 6966 6965 64d4 0d0e 0f10 1919 2025  odified....... %
-00003150: 0808 5b64 6174 6543 7265 6174 6564 d40d  ..[dateCreated..
-00003160: 0e0f 100a 1929 2a09 0810 6154 7369 7a65  .....)*...aTsize
-00003170: d40d 0e0f 100a 0a2e 2f09 0910 7354 6b69  ......../...sTki
-00003180: 6e64 d40d 0e0f 1019 0a33 3408 0910 6455  nd.......34...dU
-00003190: 6c61 6265 6cd4 0d0e 0f10 190a 3839 0809  label.......89..
-000031a0: 104b 5776 6572 7369 6f6e d40d 0e0f 1019  .KWversion......
-000031b0: 0a3d 3e08 0911 012c 5863 6f6d 6d65 6e74  .=>....,Xcomment
-000031c0: 73d4 0d0e 0f10 1919 4243 0808 10c8 5e64  s.......BC....^d
-000031d0: 6174 654c 6173 744f 7065 6e65 64d4 1617  ateLastOpened...
-000031e0: 1810 1920 1947 0808 5964 6174 6541 6464  ... .G..YdateAdd
-000031f0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
-00003200: 6509 2340 3000 0000 0000 0000 0800 1900  e.#@0...........
-00003210: 2e00 4000 4800 5c00 6500 7000 8300 8c00  ..@.H.\.e.p.....
-00003220: 8e00 8f00 9b00 a400 ac00 b600 bc00 c700  ................
-00003230: c800 c900 cc00 d100 da00 e200 e800 f200  ................
-00003240: f300 f500 f600 ff01 0801 0901 0a01 0c01  ................
-00003250: 1901 2201 2301 2401 3001 3901 3a01 3b01  ..".#.$.0.9.:.;.
-00003260: 3d01 4201 4b01 4c01 4d01 4f01 5401 5d01  =.B.K.L.M.O.T.].
-00003270: 5e01 5f01 6101 6701 7001 7101 7201 7401  ^._.a.g.p.q.r.t.
-00003280: 7c01 8501 8601 8701 8a01 9301 9c01 9d01  |...............
-00003290: 9e01 a001 af01 b801 b901 ba01 c401 c501  ................
-000032a0: ce01 d301 d400 0000 0000 0002 0100 0000  ................
-000032b0: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
-000032c0: 0000 0001 dd00 0000 0500 0000 0400 7300  ..............s.
-000032d0: 6800 6100 706c 7376 7062 6c6f 6200 0002  h.a.plsvpblob...
-000032e0: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
-000032f0: 0708 090a 0b1a 4647 0a27 5869 636f 6e53  ......FG.'XiconS
-00003300: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
-00003310: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00003320: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00003330: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00003340: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00003350: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
-00003360: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
-00003370: 0000 0000 0000 09d9 0c0d 0e0f 1011 1213  ................
-00003380: 1415 1e23 282c 3136 3b40 5863 6f6d 6d65  ...#(,16;@Xcomme
-00003390: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-000033a0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
-000033b0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-000033c0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-000033d0: 696f 6e54 6e61 6d65 d416 1718 191a 1b0a  ionTname........
-000033e0: 1d57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-000033f0: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
-00003400: 1101 2c09 1007 d416 1718 191a 201a 2208  ..,......... .".
-00003410: 10c8 0810 08d4 1617 1819 0a25 1a27 0910  ...........%.'..
-00003420: b508 1001 d416 1718 191a 251a 2b08 0810  ..........%.+...
-00003430: 02d4 1617 1819 0a2e 1a30 0910 6108 1003  .........0..a...
-00003440: d416 1718 191a 330a 3508 1064 0910 05d4  ......3.5..d....
-00003450: 1617 1819 0a38 0a3a 0910 7309 1004 d416  .....8.:..s.....
-00003460: 1718 191a 3d0a 3f08 104b 0910 06d4 1617  ....=.?..K......
-00003470: 1819 0a42 0a44 0911 0127 0910 0008 2340  ...B.D...'....#@
-00003480: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
-00003490: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-000034a0: 8c00 9500 9600 a900 b200 c100 ce00 da00  ................
-000034b0: df00 e500 ea00 f200 f701 0001 0801 0e01  ................
-000034c0: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
-000034d0: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
-000034e0: 4c01 4d01 4e01 5001 5901 5a01 5c01 5d01  L.M.N.P.Y.Z.\.].
-000034f0: 5f01 6801 6901 6b01 6c01 6e01 7701 7801  _.h.i.k.l.n.w.x.
-00003500: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
-00003510: 9501 9601 9901 9a01 9c01 9d01 a601 ab00  ................
-00003520: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00003530: 0000 0000 0000 0000 0000 0000 0001 ac18  ................
+00003000: 0000 0000 0000 0000 0000 0009 0000 0007  ................
+00003010: 006c 006f 006f 006b 0075 0070 0073 6c73  .l.o.o.k.u.p.sls
+00003020: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
+00003030: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
+00003040: 460a 485f 1012 7669 6577 4f70 7469 6f6e  F.H_..viewOption
+00003050: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00003060: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00003070: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00003080: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00003090: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+000030a0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
+000030b0: 6f6e 5369 7a65 1001 09d9 0c0d 0e0f 1011  onSize..........
+000030c0: 1213 1415 1e23 282d 3237 3c41 5863 6f6d  .....#(-27<AXcom
+000030d0: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
+000030e0: 656e 6564 5b64 6174 6543 7265 6174 6564  ened[dateCreated
+000030f0: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
+00003100: 5776 6572 7369 6f6e 546e 616d 655c 6461  WversionTname\da
+00003110: 7465 4d6f 6469 6669 6564 d416 1718 191a  teModified......
+00003120: 0a1c 1d55 696e 6465 7859 6173 6365 6e64  ...UindexYascend
+00003130: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
+00003140: 6510 0709 1101 2c08 d416 1718 191f 1d21  e.....,........!
+00003150: 1d10 0808 10c8 08d4 1617 1819 241d 261d  ............$.&.
+00003160: 1002 0810 b508 d416 1718 1929 1d2b 0a10  ...........).+..
+00003170: 0308 1061 09d4 1617 1819 2e0a 301d 1005  ...a........0...
+00003180: 0910 6408 d416 1718 1933 0a35 0a10 0409  ..d......3.5....
+00003190: 1073 09d4 1617 1819 380a 3a1d 1006 0910  .s......8.:.....
+000031a0: 4b08 d416 1718 193d 0a3f 0a10 0009 1101  K......=.?......
+000031b0: d509 d416 1718 1909 1d26 0a08 0908 2340  .........&....#@
+000031c0: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
+000031d0: 0000 0000 0000 0008 0019 002e 0040 0048  .............@.H
+000031e0: 005c 0065 0070 0083 008c 008e 008f 00a2  .\.e.p..........
+000031f0: 00ab 00ba 00c6 00cb 00d1 00d6 00de 00e3  ................
+00003200: 00f0 00f9 00ff 0109 010f 0117 0119 011a  ................
+00003210: 011d 011e 0127 0129 012a 012c 012d 0136  .....'.).*.,.-.6
+00003220: 0138 0139 013b 013c 0145 0147 0148 014a  .8.9.;.<.E.G.H.J
+00003230: 014b 0154 0156 0157 0159 015a 0163 0165  .K.T.V.W.Y.Z.c.e
+00003240: 0166 0168 0169 0172 0174 0175 0177 0178  .f.h.i.r.t.u.w.x
+00003250: 0181 0183 0184 0187 0188 0191 0192 0193  ................
+00003260: 0194 019d 01a2 01a3 0000 0000 0000 0201  ................
+00003270: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00003280: 0000 0000 0000 01ac 0000 0007 006c 006f  .............l.o
+00003290: 006f 006b 0075 0070 0073 6d6f 4444 626c  .o.k.u.p.smoDDbl
+000032a0: 6f62 0000 0008 1a04 dcb9 b8e5 c441 0000  ob...........A..
+000032b0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
+000032c0: 6d6f 6444 626c 6f62 0000 0008 1a04 dcb9  modDblob........
+000032d0: b8e5 c441 0000 0007 006c 006f 006f 006b  ...A.....l.o.o.k
+000032e0: 0075 0070 0073 7068 3153 636f 6d70 0000  .u.p.sph1Scomp..
+000032f0: 0000 0004 e000 0000 0007 006c 006f 006f  ...........l.o.o
+00003300: 006b 0075 0070 0073 7653 726e 6c6f 6e67  .k.u.p.svSrnlong
+00003310: 0000 0001 0000 0004 0073 0068 0061 0070  .........s.h.a.p
+00003320: 6277 7370 626c 6f62 0000 00b9 6270 6c69  bwspblob....bpli
+00003330: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00003340: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00003350: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00003360: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00003370: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00003380: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00003390: 5369 6465 6261 7208 0908 095f 1019 7b7b  Sidebar...._..{{
+000033a0: 3130 342c 2031 3632 7d2c 207b 3131 3933  104, 162}, {1193
+000033b0: 2c20 3731 337d 7d09 0815 232f 3b52 5f6b  , 713}}...#/;R_k
+000033c0: 6c6d 6e6f 8b00 0000 0000 0001 0100 0000  lmno............
+000033d0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
+000033e0: 0000 0000 8c00 0000 0400 7300 6800 6100  ..........s.h.a.
+000033f0: 706c 6731 5363 6f6d 7000 0000 0000 0927  plg1Scomp......'
+00003400: 3400 0000 0400 7300 6800 6100 706c 7376  4.....s.h.a.plsv
+00003410: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
+00003420: 30d8 0102 0304 0506 0708 090a 0b18 4647  0.............FG
+00003430: 0a49 5869 636f 6e53 697a 655f 100f 7368  .IXiconSize_..sh
+00003440: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00003450: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00003460: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00003470: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+00003480: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00003490: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000034a0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
+000034b0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
+000034c0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+000034d0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+000034e0: 7669 7369 626c 6554 6e61 6d65 1101 2709  visibleTname..'.
+000034f0: 09d4 0d0e 0f10 1617 1818 5875 6269 7175  ..........Xubiqu
+00003500: 6974 7910 2308 08d4 0d0e 0f10 1b1c 180a  ity.#...........
+00003510: 5c64 6174 654d 6f64 6966 6965 6410 b508  \dateModified...
+00003520: 09d4 0d0e 0f10 201c 1818 5b64 6174 6543  ...... ...[dateC
+00003530: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
 00003540: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
 00003550: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
 00003560: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
 00003570: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
 00003580: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
 00003590: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
 000035a0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
@@ -867,159 +867,159 @@
 00003620: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003630: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003640: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003650: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003660: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003670: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003680: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00003690: 01c5 6801 6901 6b01 7401 7501 7701 7801  ..h.i.k.t.u.w.x.
-000036a0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
-000036b0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
-000036c0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
-000036d0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
-000036e0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-000036f0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
-00003700: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
-00003710: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
-00003720: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
-00003730: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
-00003740: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
-00003750: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
-00003760: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
-00003770: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00003780: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
-00003790: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-000037a0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-000037b0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-000037c0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-000037d0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-000037e0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-000037f0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00003800: 7b33 3335 0000 0006 0000 0000 0000 380b  {335..........8.
-00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
-00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
-00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00003c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
-00003c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00003c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00003c50: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-00003c60: 0100 0008 0000 0000 0000 0000 0000 0000  ................
-00003c70: 0100 0040 0000 0000 0100 0080 0000 0000  ...@............
-00003c80: 0100 0100 0000 0000 0100 0200 0000 0000  ................
-00003c90: 0100 0400 0000 0000 0100 0800 0000 0000  ................
-00003ca0: 0100 1000 0000 0000 0100 2000 0000 0000  .......... .....
-00003cb0: 0100 4000 0000 0000 0100 8000 0000 0000  ..@.............
-00003cc0: 0101 0000 0000 0000 0102 0000 0000 0000  ................
-00003cd0: 0104 0000 0000 0000 0108 0000 0000 0000  ................
-00003ce0: 0110 0000 0000 0000 0120 0000 0000 0000  ......... ......
-00003cf0: 0140 0000 0000 0000 0001 6e01 7701 7801  .@........n.w.x.
-00003d00: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
-00003d10: 9501 9601 9901 9a01 9c01 9d01 a601 ab00  ................
-00003d20: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00003d30: 0000 0000 0000 0000 0000 0000 0001 ac18  ................
-00003d40: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
-00003d50: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
-00003d60: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
-00003d70: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
-00003d80: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
-00003d90: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
-00003da0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
-00003db0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
-00003dc0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
-00003dd0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
-00003de0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
-00003df0: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
-00003e00: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
-00003e10: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
-00003e20: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
-00003e30: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
-00003e40: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
-00003e50: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
-00003e60: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
-00003e70: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
-00003e80: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00003e90: 01c5 6801 6901 6b01 7401 7501 7701 7801  ..h.i.k.t.u.w.x.
-00003ea0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
-00003eb0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
-00003ec0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
-00003ed0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
-00003ee0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-00003ef0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
-00003f00: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
-00003f10: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
-00003f20: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
-00003f30: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
-00003f40: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
-00003f50: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
-00003f60: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
-00003f70: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
-00003f80: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
-00003f90: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00003fa0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00003fb0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00003fc0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00003fd0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00003fe0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00003ff0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00004000: 7b33 3335                                {335
+00003690: 01c5 0000 0004 0073 0068 0061 0070 6c73  .......s.h.a.pls
+000036a0: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
+000036b0: 3030 d801 0203 0405 0607 0809 0a0b 1a46  00.............F
+000036c0: 470a 2758 6963 6f6e 5369 7a65 5f10 0f73  G.'XiconSize_..s
+000036d0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+000036e0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+000036f0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+00003700: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
+00003710: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00003720: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
+00003730: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
+00003740: d90c 0d0e 0f10 1112 1314 151e 2328 2c31  ............#(,1
+00003750: 363b 4058 636f 6d6d 656e 7473 5e64 6174  6;@Xcomments^dat
+00003760: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
+00003770: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
+00003780: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+00003790: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+000037a0: 65d4 1617 1819 1a1b 0a1d 5776 6973 6962  e.........Wvisib
+000037b0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+000037c0: 6e67 5569 6e64 6578 0811 012c 0910 07d4  ngUindex...,....
+000037d0: 1617 1819 1a20 1a22 0810 c808 1008 d416  ..... ."........
+000037e0: 1718 190a 251a 2709 10b5 0810 01d4 1617  ....%.'.........
+000037f0: 1819 1a25 1a2b 0808 1002 d416 1718 190a  ...%.+..........
+00003800: 2e1a 3009 1061 0810 03d4 1617 1819 1a33  ..0..a.........3
+00003810: 0a35 0810 6409 1005 d416 1718 190a 380a  .5..d.........8.
+00003820: 3a09 1073 0910 04d4 1617 1819 1a3d 0a3f  :..s.........=.?
+00003830: 0810 4b09 1006 d416 1718 190a 420a 4409  ..K.........B.D.
+00003840: 1101 2709 1000 0823 4028 0000 0000 0000  ..'....#@(......
+00003850: 546e 616d 6509 0008 0019 0022 0034 003c  Tname......".4.<
+00003860: 0050 0059 0064 0077 008c 0095 0096 00a9  .P.Y.d.w........
+00003870: 00b2 00c1 00ce 00da 00df 00e5 00ea 00f2  ................
+00003880: 00f7 0100 0108 010e 0118 011e 011f 0122  ..............."
+00003890: 0123 0125 012e 012f 0131 0132 0134 013d  .#.%.../.1.2.4.=
+000038a0: 013e 0140 0141 0143 014c 014d 014e 0150  .>.@.A.C.L.M.N.P
+000038b0: 0159 015a 015c 015d 015f 0168 0169 016b  .Y.Z.\.]._.h.i.k
+000038c0: 016c 016e 0177 0178 017a 017b 017d 0186  .l.n.w.x.z.{.}..
+000038d0: 0187 0189 018a 018c 0195 0196 0199 019a  ................
+000038e0: 019c 019d 01a6 01ab 0000 0000 0000 0201  ................
+000038f0: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00003900: 0000 0000 0000 01ac 756d 6e58 6963 6f6e  ........umnXicon
+00003910: 5369 7a65 5f10 1276 6965 774f 7074 696f  Size_..viewOptio
+00003920: 6e73 5665 7273 696f 6e09 09ab 0e17 1c21  nsVersion......!
+00003930: 252a 2f34 393e 43d4 0f10 1112 0b14 0b16  %*/49>C.........
+00003940: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00003950: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
+00003960: 6965 7209 1101 c709 546e 616d 65d4 0f10  ier.....Tname...
+00003970: 1112 1819 181b 0810 2308 5875 6269 7175  ........#.Xubiqu
+00003980: 6974 79d4 0f10 1112 0b1e 1820 0910 b508  ity........ ....
+00003990: 5c64 6174 654d 6f64 6966 6965 64d4 0f10  \dateModified...
+000039a0: 1112 181e 1824 0808 5b64 6174 6543 7265  .....$..[dateCre
+000039b0: 6174 6564 d40f 1011 120b 2718 2909 1061  ated......'.)..a
+000039c0: 0854 7369 7a65 d40f 1011 120b 2c0b 2e09  .Tsize......,...
+000039d0: 1073 0954 6b69 6e64 d40f 1011 1218 310b  .s.Tkind......1.
+000039e0: 3308 1064 0955 6c61 6265 6cd4 0f10 1112  3..d.Ulabel.....
+000039f0: 1836 0b38 0810 4b09 5776 6572 7369 6f6e  .6.8..K.Wversion
+00003a00: d40f 1011 1218 3b0b 3d08 1101 2c09 5863  ......;.=...,.Xc
+00003a10: 6f6d 6d65 6e74 73d4 0f10 1112 1840 1842  omments......@.B
+00003a20: 0810 c808 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
+00003a30: 6e65 64d4 0f10 1112 181e 1846 0808 5964  ned........F..Yd
+00003a40: 6174 6541 6464 6564 0823 0000 0000 0000  ateAdded.#......
+00003a50: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00003a60: 2340 3000 0000 0000 0010 0100 0800 1d00  #@0.............
+00003a70: 3000 4200 4a00 5e00 7000 7900 8b00 9600  0.B.J.^.p.y.....
+00003a80: 9f00 b400 b500 b600 c200 cb00 d300 d900  ................
+00003a90: e300 ee00 ef00 f200 f300 f801 0101 0201  ................
+00003aa0: 0401 0501 0e01 1701 1801 1a01 1b01 2801  ..............(.
+00003ab0: 3101 3201 3301 3f01 4801 4901 4b01 4c01  1.2.3.?.H.I.K.L.
+00003ac0: 5101 5a01 5b01 5d01 5e01 6301 6c01 6d01  Q.Z.[.].^.c.l.m.
+00003ad0: 6f01 7001 7601 7f01 8001 8201 8301 8b01  o.p.v...........
+00003ae0: 9401 9501 9801 9901 a201 ab01 ac01 ae01  ................
+00003af0: af01 be01 c701 c801 c901 d301 d401 dd01  ................
+00003b00: e601 eb01 f400 0000 0000 0002 0100 0000  ................
+00003b10: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
+00003b20: 0000 0001 f600 0000 0300 6900 6d00 676c  ..........i.m.gl
+00003b30: 7376 7062 6c6f 6200 0002 9562 706c 6973  svpblob....bplis
+00003b40: 7430 30da 0102 0304 0506 0708 090a 0b0b  t00.............
+00003b50: 0d1f 4849 484a 4b26 5f10 1075 7365 5265  ..HIHJK&_..useRe
+00003b60: 6c61 7469 7665 4461 7465 735f 100f 7368  lativeDates_..sh
+00003b70: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00003b80: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00003b90: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
+00003ba0: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+00003bb0: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00003bc0: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00003bd0: 6e58 6963 6f6e 5369 7a65 5f10 1276 6965  nXiconSize_..vie
+00003be0: 774f 7074 696f 6e73 5665 7273 696f 6e09  wOptionsVersion.
+00003bf0: 09d9 0e0f 1011 1213 1415 1617 2025 2a2e  ............ %*.
+00003c00: 3338 3d42 5863 6f6d 6d65 6e74 735e 6461  38=BXcomments^da
+00003c10: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00003c20: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+00003c30: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00003c40: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00003c50: 6d65 d418 191a 1b1c 1d0b 1f55 696e 6465  me.........Uinde
+00003c60: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
+00003c70: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
+00003c80: d418 191a 1b21 221f 1f10 0810 c808 08d4  .....!".........
+00003c90: 1819 1a1b 2627 1f0b 1001 10b5 0809 d418  ....&'..........
+00003ca0: 191a 1b2b 271f 1f10 0208 08d4 1819 1a1b  ...+'...........
+00003cb0: 2f30 1f0b 1003 1061 0809 d418 191a 1b34  /0.....a.......4
+00003cc0: 350b 1f10 0510 6409 08d4 1819 1a1b 393a  5.....d.......9:
+00003cd0: 0b0b 1004 1073 0909 d418 191a 1b3e 3f0b  .....s.......>?.
+00003ce0: 1f10 0610 4b09 08d4 1819 1a1b 4344 0b0b  ....K.......CD..
+00003cf0: 1000 1101 c709 0908 2300 0000 0000 0000  ........#.......
+00003d00: 0023 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
+00003d10: 4030 0000 0000 0000 0008 001d 0030 0042  @0...........0.B
+00003d20: 004a 005e 0070 0079 008b 0096 009f 00b4  .J.^.p.y........
+00003d30: 00b5 00b6 00c9 00d2 00e1 00ee 00fa 00ff  ................
+00003d40: 0105 010a 0112 0117 0120 0126 012c 0136  ......... .&.,.6
+00003d50: 013e 0140 0143 0144 0145 014e 0150 0152  .>.@.C.D.E.N.P.R
+00003d60: 0153 0154 015d 015f 0161 0162 0163 016c  .S.T.]._.a.b.c.l
+00003d70: 016e 016f 0170 0179 017b 017d 017e 017f  .n.o.p.y.{.}.~..
+00003d80: 0188 018a 018c 018d 018e 0197 0199 019b  ................
+00003d90: 019c 019d 01a6 01a8 01aa 01ab 01ac 01b5  ................
+00003da0: 01b7 01ba 01bb 01bc 01bd 01c6 01cf 01d4  ................
+00003db0: 0000 0000 0000 0201 0000 0000 0000 004c  ...............L
+00003dc0: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
+00003dd0: 0000 0003 0069 006d 0067 6d6f 4444 626c  .....i.m.gmoDDbl
+00003de0: 6f62 0000 0008 4551 1b75 c60b c541 0000  ob....EQ.u...A..
+00003df0: 0003 0069 006d 0067 6d6f 6444 626c 6f62  ...i.m.gmodDblob
+00003e00: 0000 0008 4551 1b75 c60b c541 0000 0003  ....EQ.u...A....
+00003e10: 0069 006d 0067 7068 3153 636f 6d70 0000  .i.m.gph1Scomp..
+00003e20: 0000 0011 3000 0000 0003 0069 006d 0067  ....0......i.m.g
+00003e30: 7653 726e 6c6f 6e67 0000 0001 0000 0007  vSrnlong........
+00003e40: 006c 006f 006f 006b 0075 0070 0073 6277  .l.o.o.k.u.p.sbw
+00003e50: 7370 626c 6f62 0000 00c8 6270 6c69 7374  spblob....bplist
+00003e60: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+00003e70: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00003e80: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00003e90: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00003ea0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00003eb0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00003ec0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00003ed0: 6261 7208 0809 0809 5f10 177b 7b32 302c  bar....._..{{20,
+00003ee0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
+00003ef0: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+00003f00: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
+00003f10: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+00003f20: 0099 0000 0007 006c 006f 006f 006b 0075  .......l.o.o.k.u
+00003f30: 0070 0073 6c67 3153 636f 6d70 0000 0000  .p.slg1Scomp....
+00003f40: 0004 b42c 0000 0000 0000 0000 0000 0000  ...,............
+00003f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.63.7/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.7/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.63.7/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.63.7/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.63.7/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.6
+Version: 1.63.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 simba/data_processors/agg_clf_calculator.py
 simba/data_processors/directing_other_animals_calculator.py
 simba/data_processors/fsttc_calculator.py
 simba/data_processors/interpolate_pose.py
 simba/data_processors/interpolation_smoothing.py
 simba/data_processors/kleinberg_calculator.py
 simba/data_processors/movement_calculator.py
+simba/data_processors/mutual_exclusivity_corrector.py
 simba/data_processors/pup_retrieval_calculator.py
 simba/data_processors/pybursts_calculator.py
 simba/data_processors/severity_bout_based_calculator.py
 simba/data_processors/severity_calculator.py
 simba/data_processors/severity_frame_based_calculator.py
 simba/data_processors/timebins_clf_calculator.py
 simba/data_processors/timebins_movement_calculator.py
@@ -353,14 +354,26 @@
 simba/third_party_label_appenders/__init__.py
 simba/third_party_label_appenders/deepethogram_importer.py
 simba/third_party_label_appenders/ethovision_import.py
 simba/third_party_label_appenders/observer_importer.py
 simba/third_party_label_appenders/solomon_importer.py
 simba/third_party_label_appenders/third_party_appender.py
 simba/third_party_label_appenders/tools.py
+simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+simba/three_dimensions/mixins/config_reader.py
+simba/three_dimensions/mixins/feature_extraction_mixin.py
+simba/three_dimensions/mixins/plotting_mixin.py
+simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+simba/three_dimensions/plotting/plot_pose_in_dir.py
+simba/three_dimensions/pose_importers/anipose_csv_import.py
+simba/three_dimensions/ui/define_px_to_mm_ui.py
 simba/ui/.DS_Store
 simba/ui/__init__.py
 simba/ui/create_project_ui.py
 simba/ui/machine_model_settings_ui.py
 simba/ui/tkinter_functions.py
 simba/ui/user_defined_pose_creator.py
 simba/ui/video_info_ui.py
@@ -387,14 +400,15 @@
 simba/ui/pop_ups/gantt_pop_up.py
 simba/ui/pop_ups/heatmap_clf_pop_up.py
 simba/ui/pop_ups/heatmap_location_pop_up.py
 simba/ui/pop_ups/kleinberg_pop_up.py
 simba/ui/pop_ups/make_path_plot_pop_up.py
 simba/ui/pop_ups/movement_analysis_pop_up.py
 simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+simba/ui/pop_ups/mutual_exclusivity_pop_up.py
 simba/ui/pop_ups/outlier_settings_pop_up.py
 simba/ui/pop_ups/path_plot_pop_up.py
 simba/ui/pop_ups/pose_bp_drop_pop_up.py
 simba/ui/pop_ups/pose_reorganizer_pop_up.py
 simba/ui/pop_ups/pup_retrieval_pop_up.py
 simba/ui/pop_ups/quick_path_plot_pop_up.py
 simba/ui/pop_ups/remove_roi_features_pop_up.py
```

### Comparing `Simba-UW-tf-dev-1.63.6/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/LICENSE.md` & `Simba-UW-tf-dev-1.63.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.63.7/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.63.7/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.63.7/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.63.7/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.7/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.63.7/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.63.7/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.63.7/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.63.7/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.63.7/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.63.7/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.63.7/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.63.7/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.63.7/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/README.md` & `Simba-UW-tf-dev-1.63.7/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.6/setup.py` & `Simba-UW-tf-dev-1.63.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.63.6",
+    version="1.63.7",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

