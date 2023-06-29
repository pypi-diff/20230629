# Comparing `tmp/rips-2023.6.0.1.tar.gz` & `tmp/rips-2023.6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rips-2023.6.0.1.tar", last modified: Mon Jun 19 12:49:47 2023, max compression
+gzip compressed data, was "rips-2023.6.0.2.tar", last modified: Thu Jun 29 09:56:09 2023, max compression
```

## Comparing `rips-2023.6.0.1.tar` & `rips-2023.6.0.2.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/
--rw-rw-rw-   0        0        0      560 2021-03-03 12:14:39.000000 rips-2023.6.0.1/LICENSE
--rw-rw-rw-   0        0        0       75 2021-03-03 12:14:39.000000 rips-2023.6.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1039 2023-06-19 12:49:47.000000 rips-2023.6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      190 2021-03-03 12:14:39.000000 rips-2023.6.0.1/README.md
--rw-rw-rw-   0        0        0      201 2021-03-03 12:14:39.000000 rips-2023.6.0.1/autoformat_pep8.txt
--rw-rw-rw-   0        0        0     1164 2021-03-03 12:14:39.000000 rips-2023.6.0.1/create_pip_package.txt
--rw-rw-rw-   0        0        0       37 2021-03-03 12:14:39.000000 rips-2023.6.0.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/PythonExamples/
--rw-rw-rw-   0        0        0     1495 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/all_cases.py
--rw-rw-rw-   0        0        0     1267 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/all_simulation_wells.py
--rw-rw-rw-   0        0        0      606 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/all_wells.py
--rw-rw-rw-   0        0        0      801 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/alter_wbs_plot.py
--rw-rw-rw-   0        0        0      685 2023-02-10 10:50:44.000000 rips-2023.6.0.1/rips/PythonExamples/case_grid_group.py
--rw-rw-rw-   0        0        0     1016 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/case_info_streaming_example.py
--rw-rw-rw-   0        0        0      509 2021-11-18 07:34:03.000000 rips-2023.6.0.1/rips/PythonExamples/cell_result_data.py
--rw-rw-rw-   0        0        0     1785 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/command_example.py
--rw-rw-rw-   0        0        0     4227 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/create_and_export_stim_plan_model.py
--rw-rw-rw-   0        0        0     2433 2022-04-05 06:32:53.000000 rips-2023.6.0.1/rips/PythonExamples/create_intersection.py
--rw-rw-rw-   0        0        0     3735 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/create_surface_from_thermal_fracture.py
--rw-rw-rw-   0        0        0     1433 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/create_wbs_plot.py
--rw-rw-rw-   0        0        0     3230 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/error_handling.py
--rw-rw-rw-   0        0        0     1171 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/export_contour_maps.py
--rw-rw-rw-   0        0        0      654 2021-08-17 13:58:38.000000 rips-2023.6.0.1/rips/PythonExamples/export_plots.py
--rw-rw-rw-   0        0        0     1598 2021-09-02 13:22:54.000000 rips-2023.6.0.1/rips/PythonExamples/export_snapshots.py
--rw-rw-rw-   0        0        0      701 2023-02-10 14:16:08.000000 rips-2023.6.0.1/rips/PythonExamples/export_well_path_completions.py
--rw-rw-rw-   0        0        0     2671 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_of_well_logs.py
--rw-rw-rw-   0        0        0     2056 2021-08-23 10:48:10.000000 rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface.py
--rw-rw-rw-   0        0        0     1149 2021-08-31 13:17:57.000000 rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface_optimized.py
--rw-rw-rw-   0        0        0      590 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/grid_information.py
--rw-rw-rw-   0        0        0     1073 2022-03-22 10:18:39.000000 rips-2023.6.0.1/rips/PythonExamples/headless_plot_export.py
--rw-rw-rw-   0        0        0     1617 2023-06-19 06:39:04.000000 rips-2023.6.0.1/rips/PythonExamples/import_case_properties.py
--rw-rw-rw-   0        0        0     2370 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/import_fractures_on_well.py
--rw-rw-rw-   0        0        0     1403 2022-10-25 08:32:28.000000 rips-2023.6.0.1/rips/PythonExamples/import_thermal_fracture_on_well.py
--rw-rw-rw-   0        0        0     1327 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/import_well_paths_and_logs.py
--rw-rw-rw-   0        0        0     1997 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/input_prop_test_async.py
--rw-rw-rw-   0        0        0     1223 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/input_prop_test_sync.py
--rw-rw-rw-   0        0        0      302 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/instance_example.py
--rw-rw-rw-   0        0        0     1315 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/launch_load_case_snapshot_exit.py
--rw-rw-rw-   0        0        0      465 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/launch_with_commandline_options.py
--rw-rw-rw-   0        0        0     1131 2021-09-01 05:50:56.000000 rips-2023.6.0.1/rips/PythonExamples/load_case.py
--rw-rw-rw-   0        0        0     1057 2021-08-16 06:21:02.000000 rips-2023.6.0.1/rips/PythonExamples/modeled_well_path.py
--rw-rw-rw-   0        0        0     1725 2021-08-16 06:21:02.000000 rips-2023.6.0.1/rips/PythonExamples/modeled_well_path_lateral.py
--rw-rw-rw-   0        0        0      467 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/new_summary_plot.py
--rw-rw-rw-   0        0        0      692 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/open_project.py
--rw-rw-rw-   0        0        0      393 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/replace_case.py
--rw-rw-rw-   0        0        0      894 2021-09-29 06:17:01.000000 rips-2023.6.0.1/rips/PythonExamples/save_project.py
--rw-rw-rw-   0        0        0      768 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/selected_cases.py
--rw-rw-rw-   0        0        0     2536 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/selected_cells.py
--rw-rw-rw-   0        0        0      379 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/set_cell_result.py
--rw-rw-rw-   0        0        0      861 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/set_flow_diagnostics_result.py
--rw-rw-rw-   0        0        0     1444 2021-11-18 11:24:26.000000 rips-2023.6.0.1/rips/PythonExamples/set_grid_properties.py
--rw-rw-rw-   0        0        0     1279 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/soil_average_async.py
--rw-rw-rw-   0        0        0      845 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/soil_average_sync.py
--rw-rw-rw-   0        0        0     2110 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/soil_porv_async.py
--rw-rw-rw-   0        0        0     1120 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/PythonExamples/soil_porv_sync.py
--rw-rw-rw-   0        0        0      460 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/summary_cases.py
--rw-rw-rw-   0        0        0     1710 2022-03-28 07:02:00.000000 rips-2023.6.0.1/rips/PythonExamples/summary_vectors.py
--rw-rw-rw-   0        0        0     1256 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/PythonExamples/surface_import.py
--rw-rw-rw-   0        0        0     1056 2021-08-31 13:16:54.000000 rips-2023.6.0.1/rips/PythonExamples/view_example.py
--rw-rw-rw-   0        0        0      679 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/__init__.py
--rw-rw-rw-   0        0        0    45546 2021-11-18 06:43:06.000000 rips-2023.6.0.1/rips/case.py
--rw-rw-rw-   0        0        0     2118 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/contour_map.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/generated/
--rw-rw-rw-   0        0        0     7280 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/App_pb2.py
--rw-rw-rw-   0        0        0     6724 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/App_pb2_grpc.py
--rw-rw-rw-   0        0        0    40186 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/Case_pb2.py
--rw-rw-rw-   0        0        0    19104 2023-06-12 07:10:55.000000 rips-2023.6.0.1/rips/generated/Case_pb2_grpc.py
--rw-rw-rw-   0        0        0   154980 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Commands_pb2.py
--rw-rw-rw-   0        0        0     3360 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Commands_pb2_grpc.py
--rw-rw-rw-   0        0        0    14439 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Definitions_pb2.py
--rw-rw-rw-   0        0        0      159 2023-06-12 07:10:56.000000 rips-2023.6.0.1/rips/generated/Definitions_pb2_grpc.py
--rw-rw-rw-   0        0        0     5614 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/Grid_pb2.py
--rw-rw-rw-   0        0        0     5401 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/Grid_pb2_grpc.py
--rw-rw-rw-   0        0        0    21334 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/NNCProperties_pb2.py
--rw-rw-rw-   0        0        0     7334 2023-06-12 07:10:57.000000 rips-2023.6.0.1/rips/generated/NNCProperties_pb2_grpc.py
--rw-rw-rw-   0        0        0    37075 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/PdmObject_pb2.py
--rw-rw-rw-   0        0        0    13870 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/PdmObject_pb2_grpc.py
--rw-rw-rw-   0        0        0     3755 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Project_pb2.py
--rw-rw-rw-   0        0        0     9869 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Project_pb2_grpc.py
--rw-rw-rw-   0        0        0    19898 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Properties_pb2.py
--rw-rw-rw-   0        0        0    10631 2023-06-12 07:10:58.000000 rips-2023.6.0.1/rips/generated/Properties_pb2_grpc.py
--rw-rw-rw-   0        0        0      775 2023-06-12 10:05:22.000000 rips-2023.6.0.1/rips/generated/RiaVersionInfo.py
--rw-rw-rw-   0        0        0    11113 2023-06-12 07:10:59.000000 rips-2023.6.0.1/rips/generated/SimulationWell_pb2.py
--rw-rw-rw-   0        0        0     4307 2023-06-12 07:10:59.000000 rips-2023.6.0.1/rips/generated/SimulationWell_pb2_grpc.py
--rw-rw-rw-   0        0        0    80324 2023-06-12 07:16:16.000000 rips-2023.6.0.1/rips/generated/generated_classes.py
--rw-rw-rw-   0        0        0     3647 2021-11-18 11:24:26.000000 rips-2023.6.0.1/rips/grid.py
--rw-rw-rw-   0        0        0     2368 2023-02-10 10:50:44.000000 rips-2023.6.0.1/rips/gridcasegroup.py
--rw-rw-rw-   0        0        0     1511 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/grpc_retry_interceptor.py
--rw-rw-rw-   0        0        0    14846 2022-10-04 12:14:47.000000 rips-2023.6.0.1/rips/instance.py
--rw-rw-rw-   0        0        0    17137 2022-02-08 18:45:33.000000 rips-2023.6.0.1/rips/pdmobject.py
--rw-rw-rw-   0        0        0      832 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/plot.py
--rw-rw-rw-   0        0        0    11987 2021-09-29 07:44:28.000000 rips-2023.6.0.1/rips/project.py
--rw-rw-rw-   0        0        0       59 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/resinsight_classes.py
--rw-rw-rw-   0        0        0     2508 2022-02-08 18:45:33.000000 rips-2023.6.0.1/rips/retry_policy.py
--rw-rw-rw-   0        0        0     2515 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/simulation_well.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips/tests/
--rw-rw-rw-   0        0        0     1428 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/conftest.py
--rw-rw-rw-   0        0        0      207 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/dataroot.py
--rw-rw-rw-   0        0        0     8964 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_cases.py
--rw-rw-rw-   0        0        0      875 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/test_commands.py
--rw-rw-rw-   0        0        0     2317 2022-02-21 12:46:35.000000 rips-2023.6.0.1/rips/tests/test_create_well_path.py
--rw-rw-rw-   0        0        0     5755 2023-06-19 06:39:04.000000 rips-2023.6.0.1/rips/tests/test_grids.py
--rw-rw-rw-   0        0        0     1198 2022-09-28 06:53:25.000000 rips-2023.6.0.1/rips/tests/test_launch.py
--rw-rw-rw-   0        0        0     2596 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_nnc_properties.py
--rw-rw-rw-   0        0        0     3042 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/tests/test_project.py
--rw-rw-rw-   0        0        0     4516 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_properties.py
--rw-rw-rw-   0        0        0     1816 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_simulation_wells.py
--rw-rw-rw-   0        0        0     4574 2023-01-24 09:05:18.000000 rips-2023.6.0.1/rips/tests/test_summary_cases.py
--rw-rw-rw-   0        0        0     1019 2021-08-17 12:15:16.000000 rips-2023.6.0.1/rips/tests/test_surfaces.py
--rw-rw-rw-   0        0        0     1522 2023-02-01 07:57:21.000000 rips-2023.6.0.1/rips/tests/test_well_log_extraction.py
--rw-rw-rw-   0        0        0     3343 2022-02-08 18:45:33.000000 rips-2023.6.0.1/rips/tests/test_wells.py
--rw-rw-rw-   0        0        0      678 2021-10-14 08:34:07.000000 rips-2023.6.0.1/rips/tests/test_wells_path_completions.py
--rw-rw-rw-   0        0        0     7612 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/view.py
--rw-rw-rw-   0        0        0     2356 2021-03-03 12:14:39.000000 rips-2023.6.0.1/rips/well_log_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:49:47.000000 rips-2023.6.0.1/rips.egg-info/
--rw-rw-rw-   0        0        0     1039 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3947 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-19 12:49:46.000000 rips-2023.6.0.1/rips.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 12:49:47.000000 rips-2023.6.0.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-06-12 06:26:22.000000 rips-2023.6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:56:09.746183 rips-2023.6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-29 09:11:21.000000 rips-2023.6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-29 09:11:21.000000 rips-2023.6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-29 09:56:09.746183 rips-2023.6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-29 09:11:21.000000 rips-2023.6.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-06-29 09:11:21.000000 rips-2023.6.0.2/autoformat_pep8.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-29 09:11:21.000000 rips-2023.6.0.2/create_pip_package.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-29 09:11:21.000000 rips-2023.6.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:56:09.714183 rips-2023.6.0.2/rips/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:56:09.730183 rips-2023.6.0.2/rips/PythonExamples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/all_cases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/all_simulation_wells.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/all_wells.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/alter_wbs_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/case_grid_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/case_info_streaming_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/cell_result_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/command_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/create_and_export_stim_plan_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/create_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/create_surface_from_thermal_fracture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/create_wbs_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/export_contour_maps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/export_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/export_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/export_well_path_completions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2584 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/generate_ensemble_of_well_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/generate_ensemble_surface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/generate_ensemble_surface_optimized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/grid_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/headless_plot_export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/import_case_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/import_fractures_on_well.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/import_thermal_fracture_on_well.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/import_well_paths_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/input_prop_test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/input_prop_test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/instance_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/launch_load_case_snapshot_exit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/launch_with_commandline_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/load_case.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/modeled_well_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/modeled_well_path_lateral.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/new_summary_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/open_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/replace_case.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/save_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/selected_cases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/selected_cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/set_cell_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/set_flow_diagnostics_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/set_grid_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/soil_average_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/soil_average_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/soil_porv_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/soil_porv_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/summary_cases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/summary_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/surface_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/PythonExamples/view_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44236 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/case.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2056 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/contour_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:56:09.738184 rips-2023.6.0.2/rips/generated/
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/App_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/App_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Case_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19104 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Case_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20336 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Commands_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Commands_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Definitions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Definitions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Grid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Grid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/NNCProperties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7334 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/NNCProperties_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5988 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/PdmObject_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13870 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/PdmObject_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9869 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3843 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10631 2023-06-29 09:55:09.000000 rips-2023.6.0.2/rips/generated/Properties_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-29 09:16:19.000000 rips-2023.6.0.2/rips/generated/RiaVersionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-29 09:55:10.000000 rips-2023.6.0.2/rips/generated/SimulationWell_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4307 2023-06-29 09:55:10.000000 rips-2023.6.0.2/rips/generated/SimulationWell_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78140 2023-06-29 09:56:04.000000 rips-2023.6.0.2/rips/generated/generated_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2280 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/gridcasegroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/grpc_retry_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14434 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16681 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/pdmobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11563 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/resinsight_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/simulation_well.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:56:09.746183 rips-2023.6.0.2/rips/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/dataroot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8734 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_create_well_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5606 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_grids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_nnc_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4402 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_simulation_wells.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4449 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_summary_cases.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_well_log_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_wells.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/tests/test_wells_path_completions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2282 2023-06-29 09:11:21.000000 rips-2023.6.0.2/rips/well_log_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 09:56:09.714183 rips-2023.6.0.2/rips.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-29 09:56:09.000000 rips-2023.6.0.2/rips.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-29 09:56:09.000000 rips-2023.6.0.2/rips.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 09:56:09.000000 rips-2023.6.0.2/rips.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-29 09:56:09.000000 rips-2023.6.0.2/rips.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 09:56:09.000000 rips-2023.6.0.2/rips.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 09:56:09.746183 rips-2023.6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-29 09:16:19.000000 rips-2023.6.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rips-2023.6.0.1/LICENSE` & `rips-2023.6.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Copyright (C) 2019-     Equinor ASA
-
-ResInsight is free software: you can redistribute it andor modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-ResInsight is distributed in the hope that it will be useful, but WITHOUT ANY
-WARRANTY; without even the implied warranty of MERCHANTABILITY or
-FITNESS FOR A PARTICULAR PURPOSE.
-
-See the GNU General Public License at <http:www.gnu.orglicensesgpl.html>
-for more details.
-
+Copyright (C) 2019-     Equinor ASA
+
+ResInsight is free software: you can redistribute it andor modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+ResInsight is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or
+FITNESS FOR A PARTICULAR PURPOSE.
+
+See the GNU General Public License at <http:www.gnu.orglicensesgpl.html>
+for more details.
+
```

### Comparing `rips-2023.6.0.1/create_pip_package.txt` & `rips-2023.6.0.2/create_pip_package.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-######################################################################
-# All this is based on the MANIFEST.in and setup.py in Python-folder
-######################################################################
-
-# 1. Make sure dist folder is clear
-del dist/*
- 
-# 2. Update rips-version tag in setup.py (".N after ResInsight version"). This is generated from setup.py.cmake
-#    So that you for instance have version 2019.08.1 of rips.
- 
-# 3. Build source distribution
-python setup.py sdist
- 
-# 4. Test upload to test.pypi.org. This requires a ResInsight testpypi-user and you will be prompted for username and password
-python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
- 
-# 5. Test install rips module.
-pip install --index-url https://test.pypi.org/simple/ rips
-
-# 6. Test the newly installed module
-
-# 8. If anything is wrong, start again from 1. with an incremented rips-version (ResInsightVersion.2+)
-# These incremented versions are just for testpypi and you can reset back to the wanted version before real upload
-
-# 9. Upload to real Pypi. This requires a ResInsight pypi-user.
+######################################################################
+# All this is based on the MANIFEST.in and setup.py in Python-folder
+######################################################################
+
+# 1. Make sure dist folder is clear
+del dist/*
+ 
+# 2. Update rips-version tag in setup.py (".N after ResInsight version"). This is generated from setup.py.cmake
+#    So that you for instance have version 2019.08.1 of rips.
+ 
+# 3. Build source distribution
+python setup.py sdist
+ 
+# 4. Test upload to test.pypi.org. This requires a ResInsight testpypi-user and you will be prompted for username and password
+python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+ 
+# 5. Test install rips module.
+pip install --index-url https://test.pypi.org/simple/ rips
+
+# 6. Test the newly installed module
+
+# 8. If anything is wrong, start again from 1. with an incremented rips-version (ResInsightVersion.2+)
+# These incremented versions are just for testpypi and you can reset back to the wanted version before real upload
+
+# 9. Upload to real Pypi. This requires a ResInsight pypi-user.
 python -m twine upload dist/*
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/all_cases.py` & `rips-2023.6.0.2/rips/PythonExamples/all_cases.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-###################################################################################
-# This example will connect to ResInsight, retrieve a list of cases and print info
-#
-###################################################################################
-
-# Import the ResInsight Processing Server Module
-import rips
-
-# Connect to ResInsight
-resinsight = rips.Instance.find()
-if resinsight is not None:
-    # Get a list of all cases
-    cases = resinsight.project.cases()
-
-    print("Got " + str(len(cases)) + " cases: ")
-    for case in cases:
-        print("Case id: " + str(case.id))
-        print("Case name: " + case.name)
-        print("Case type: " + case.__class__.__name__)
-        print("Case file name: " + case.file_path)
-        print("Case reservoir bounding box:", case.reservoir_boundingbox())
-
-        timesteps = case.time_steps()
-        for t in timesteps:
-            print("Year: " + str(t.year))
-            print("Month: " + str(t.month))
-
-        if isinstance(case, rips.EclipseCase):
-            print("Getting coarsening info for case: ", case.name, case.id)
-            coarsening_info = case.coarsening_info()
-            if coarsening_info:
-                print("Coarsening information:")
-
-            for c in coarsening_info:
-                print(
-                    "[{}, {}, {}] - [{}, {}, {}]".format(
-                        c.min.x, c.min.y, c.min.z, c.max.x, c.max.y, c.max.z
-                    )
-                )
+###################################################################################
+# This example will connect to ResInsight, retrieve a list of cases and print info
+#
+###################################################################################
+
+# Import the ResInsight Processing Server Module
+import rips
+
+# Connect to ResInsight
+resinsight = rips.Instance.find()
+if resinsight is not None:
+    # Get a list of all cases
+    cases = resinsight.project.cases()
+
+    print("Got " + str(len(cases)) + " cases: ")
+    for case in cases:
+        print("Case id: " + str(case.id))
+        print("Case name: " + case.name)
+        print("Case type: " + case.__class__.__name__)
+        print("Case file name: " + case.file_path)
+        print("Case reservoir bounding box:", case.reservoir_boundingbox())
+
+        timesteps = case.time_steps()
+        for t in timesteps:
+            print("Year: " + str(t.year))
+            print("Month: " + str(t.month))
+
+        if isinstance(case, rips.EclipseCase):
+            print("Getting coarsening info for case: ", case.name, case.id)
+            coarsening_info = case.coarsening_info()
+            if coarsening_info:
+                print("Coarsening information:")
+
+            for c in coarsening_info:
+                print(
+                    "[{}, {}, {}] - [{}, {}, {}]".format(
+                        c.min.x, c.min.y, c.min.z, c.max.x, c.max.y, c.max.z
+                    )
+                )
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/all_simulation_wells.py` & `rips-2023.6.0.2/rips/PythonExamples/all_simulation_wells.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-###################################################################################
-# This example will connect to ResInsight, retrieve a list of
-# simulation wells and print info
-###################################################################################
-
-# Import the ResInsight Processing Server Module
-import rips
-
-# Connect to ResInsight
-resinsight = rips.Instance.find()
-if resinsight is not None:
-    # Get a list of all wells
-    cases = resinsight.project.cases()
-
-    for case in cases:
-        print("Case id: " + str(case.id))
-        print("Case name: " + case.name)
-
-        timesteps = case.time_steps()
-        sim_wells = case.simulation_wells()
-        for sim_well in sim_wells:
-            print("Simulation well: " + sim_well.name)
-
-            for tidx, timestep in enumerate(timesteps):
-                status = sim_well.status(tidx)
-                cells = sim_well.cells(tidx)
-                print(
-                    "timestep: "
-                    + str(tidx)
-                    + " type: "
-                    + status.well_type
-                    + " open: "
-                    + str(status.is_open)
-                    + " cells:"
-                    + str(len(cells))
-                )
+###################################################################################
+# This example will connect to ResInsight, retrieve a list of
+# simulation wells and print info
+###################################################################################
+
+# Import the ResInsight Processing Server Module
+import rips
+
+# Connect to ResInsight
+resinsight = rips.Instance.find()
+if resinsight is not None:
+    # Get a list of all wells
+    cases = resinsight.project.cases()
+
+    for case in cases:
+        print("Case id: " + str(case.id))
+        print("Case name: " + case.name)
+
+        timesteps = case.time_steps()
+        sim_wells = case.simulation_wells()
+        for sim_well in sim_wells:
+            print("Simulation well: " + sim_well.name)
+
+            for tidx, timestep in enumerate(timesteps):
+                status = sim_well.status(tidx)
+                cells = sim_well.cells(tidx)
+                print(
+                    "timestep: "
+                    + str(tidx)
+                    + " type: "
+                    + status.well_type
+                    + " open: "
+                    + str(status.is_open)
+                    + " cells:"
+                    + str(len(cells))
+                )
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/alter_wbs_plot.py` & `rips-2023.6.0.2/rips/PythonExamples/alter_wbs_plot.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-# Get the project
-project = resinsight.project
-
-# Find all the well bore stability plots in the project
-wbsplots = project.descendants(rips.WellBoreStabilityPlot)
-
-# Chose a sensible output folder
-dirname = tempfile.gettempdir()
-
-# Loop through all Well Bore Stability plots
-for wbsplot in wbsplots:
-    # Set depth type a parameter and export snapshot
-    wbsplot.depth_type = "TRUE_VERTICAL_DEPTH_RKB"
-
-    # Example of setting parameters for existing plots
-    params = wbsplot.parameters()
-    params.user_poisson_ratio = 0.12345
-    params.update()
-    wbsplot.update()
-    wbsplot.export_snapshot(export_folder=dirname)
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+# Get the project
+project = resinsight.project
+
+# Find all the well bore stability plots in the project
+wbsplots = project.descendants(rips.WellBoreStabilityPlot)
+
+# Chose a sensible output folder
+dirname = tempfile.gettempdir()
+
+# Loop through all Well Bore Stability plots
+for wbsplot in wbsplots:
+    # Set depth type a parameter and export snapshot
+    wbsplot.depth_type = "TRUE_VERTICAL_DEPTH_RKB"
+
+    # Example of setting parameters for existing plots
+    params = wbsplot.parameters()
+    params.user_poisson_ratio = 0.12345
+    params.update()
+    wbsplot.update()
+    wbsplot.export_snapshot(export_folder=dirname)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/case_grid_group.py` & `rips-2023.6.0.2/rips/PythonExamples/case_grid_group.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import os
-import rips
-
-resinsight = rips.Instance.find()
-
-case_paths = []
-case_paths.append(
-    "C:/Users/lindk/source/repos/ResInsight/TestModels/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
-)
-case_paths.append(
-    "C:/Users/lindk/source/repos/ResInsight/TestModels/Case_with_10_timesteps/Real10/BRUGGE_0010.EGRID"
-)
-for case_path in case_paths:
-    assert os.path.exists(
-        case_path
-    ), "You need to set valid case paths for this script to work"
-
-case_group = resinsight.project.create_grid_case_group(case_paths=case_paths)
-
-case_group.compute_statistics()
-
-view = case_group.views()[0]
-view.apply_cell_result("DYNAMIC_NATIVE", "PRESSURE_DEV")
+import os
+import rips
+
+resinsight = rips.Instance.find()
+
+case_paths = []
+case_paths.append(
+    "C:/Users/lindk/source/repos/ResInsight/TestModels/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
+)
+case_paths.append(
+    "C:/Users/lindk/source/repos/ResInsight/TestModels/Case_with_10_timesteps/Real10/BRUGGE_0010.EGRID"
+)
+for case_path in case_paths:
+    assert os.path.exists(
+        case_path
+    ), "You need to set valid case paths for this script to work"
+
+case_group = resinsight.project.create_grid_case_group(case_paths=case_paths)
+
+case_group.compute_statistics()
+
+view = case_group.views()[0]
+view.apply_cell_result("DYNAMIC_NATIVE", "PRESSURE_DEV")
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/case_info_streaming_example.py` & `rips-2023.6.0.2/rips/PythonExamples/case_info_streaming_example.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-###############################################################################
-# This example will get the cell info for the active cells for the first case
-###############################################################################
-
-# Import the ResInsight Processing Server Module
-import rips
-
-# Connect to ResInsight
-resinsight = rips.Instance.find()
-
-# Get the first case. This will fail if you haven't loaded any cases
-case = resinsight.project.cases()[0]
-
-# Get the cell count object
-cell_counts = case.cell_count()
-print("Number of active cells: " + str(cell_counts.active_cell_count))
-print("Total number of reservoir cells: " + str(cell_counts.reservoir_cell_count))
-
-# Get information for all active cells
-active_cell_infos = case.cell_info_for_active_cells()
-
-# A simple check on the size of the cell info
-assert cell_counts.active_cell_count == len(active_cell_infos)
-
-# Print information for the first active cell
-print("First active cell: ")
-print(active_cell_infos[0])
+###############################################################################
+# This example will get the cell info for the active cells for the first case
+###############################################################################
+
+# Import the ResInsight Processing Server Module
+import rips
+
+# Connect to ResInsight
+resinsight = rips.Instance.find()
+
+# Get the first case. This will fail if you haven't loaded any cases
+case = resinsight.project.cases()[0]
+
+# Get the cell count object
+cell_counts = case.cell_count()
+print("Number of active cells: " + str(cell_counts.active_cell_count))
+print("Total number of reservoir cells: " + str(cell_counts.reservoir_cell_count))
+
+# Get information for all active cells
+active_cell_infos = case.cell_info_for_active_cells()
+
+# A simple check on the size of the cell info
+assert cell_counts.active_cell_count == len(active_cell_infos)
+
+# Print information for the first active cell
+print("First active cell: ")
+print(active_cell_infos[0])
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/command_example.py` & `rips-2023.6.0.2/rips/PythonExamples/command_example.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-###############################################################################
-# This example will show setting time step, window size and export snapshots and properties
-###############################################################################
-import os
-import tempfile
-import rips
-
-# Load instance
-resinsight = rips.Instance.find()
-
-# Set window sizes
-resinsight.set_main_window_size(width=800, height=500)
-resinsight.set_plot_window_size(width=1000, height=1000)
-
-
-# Retrieve first case
-case = resinsight.project.cases()[0]
-
-# Get a view
-view1 = case.views()[0]
-
-# Clone the view
-view2 = view1.clone()
-
-# Set the time step for view1 only
-view1.set_time_step(time_step=2)
-
-# Set cell result to SOIL
-view1.apply_cell_result(result_type="DYNAMIC_NATIVE", result_variable="SOIL")
-
-
-# Create a temporary directory which will disappear at the end of this script
-# If you want to keep the files, provide a good path name instead of tmpdirname
-with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
-    print("Temporary folder: ", tmpdirname)
-
-    # Set export folder for snapshots and properties
-    resinsight.set_export_folder(export_type="SNAPSHOTS", path=tmpdirname)
-    resinsight.set_export_folder(export_type="PROPERTIES", path=tmpdirname)
-
-    # Export all snapshots
-    resinsight.project.export_snapshots()
-
-    assert len(os.listdir(tmpdirname)) > 0
-
-    # Export properties in the view
-    view1.export_property()
-
-    # Check that the exported file exists
-    expected_file_name = case.name + "-" + str("3D_View") + "-" + "T2" + "-SOIL"
-    full_path = tmpdirname + "/" + expected_file_name
-
-    # Print contents of temporary folder
-    print(os.listdir(tmpdirname))
-
-    assert os.path.exists(full_path)
+###############################################################################
+# This example will show setting time step, window size and export snapshots and properties
+###############################################################################
+import os
+import tempfile
+import rips
+
+# Load instance
+resinsight = rips.Instance.find()
+
+# Set window sizes
+resinsight.set_main_window_size(width=800, height=500)
+resinsight.set_plot_window_size(width=1000, height=1000)
+
+
+# Retrieve first case
+case = resinsight.project.cases()[0]
+
+# Get a view
+view1 = case.views()[0]
+
+# Clone the view
+view2 = view1.clone()
+
+# Set the time step for view1 only
+view1.set_time_step(time_step=2)
+
+# Set cell result to SOIL
+view1.apply_cell_result(result_type="DYNAMIC_NATIVE", result_variable="SOIL")
+
+
+# Create a temporary directory which will disappear at the end of this script
+# If you want to keep the files, provide a good path name instead of tmpdirname
+with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
+    print("Temporary folder: ", tmpdirname)
+
+    # Set export folder for snapshots and properties
+    resinsight.set_export_folder(export_type="SNAPSHOTS", path=tmpdirname)
+    resinsight.set_export_folder(export_type="PROPERTIES", path=tmpdirname)
+
+    # Export all snapshots
+    resinsight.project.export_snapshots()
+
+    assert len(os.listdir(tmpdirname)) > 0
+
+    # Export properties in the view
+    view1.export_property()
+
+    # Check that the exported file exists
+    expected_file_name = case.name + "-" + str("3D_View") + "-" + "T2" + "-SOIL"
+    full_path = tmpdirname + "/" + expected_file_name
+
+    # Print contents of temporary folder
+    print(os.listdir(tmpdirname))
+
+    assert os.path.exists(full_path)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/create_and_export_stim_plan_model.py` & `rips-2023.6.0.2/rips/PythonExamples/create_and_export_stim_plan_model.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-# Example code
-project = resinsight.project
-
-# Look for input files in the home directory of the user
-home_dir = expanduser("~")
-elastic_properties_file_path = (Path(home_dir) / "elastic_properties.csv").as_posix()
-print("Elastic properties file path:", elastic_properties_file_path)
-
-facies_properties_file_path = (Path(home_dir) / "facies_id.roff").as_posix()
-print("Facies properties file path:", facies_properties_file_path)
-
-# Find a case
-cases = resinsight.project.cases()
-case = cases[1]
-
-# Use the last time step
-time_steps = case.time_steps()
-time_step = time_steps[len(time_steps) - 1]
-
-
-# Create stim plan model template
-fmt_collection = project.descendants(rips.StimPlanModelTemplateCollection)[0]
-stim_plan_model_template = fmt_collection.append_stim_plan_model_template(
-    eclipse_case=case,
-    time_step=time_step,
-    elastic_properties_file_path=elastic_properties_file_path,
-    facies_properties_file_path=facies_properties_file_path,
-)
-stim_plan_model_template.overburden_formation = "Garn"
-stim_plan_model_template.overburden_facies = "Shale"
-stim_plan_model_template.underburden_formation = "Garn"
-stim_plan_model_template.underburden_facies = "Shale"
-stim_plan_model_template.overburden_height = 68
-stim_plan_model_template.update()
-print("Overburden: ", stim_plan_model_template.overburden_formation)
-
-
-# Set eclipse result for facies definition
-eclipse_result = stim_plan_model_template.facies_properties().facies_definition()
-eclipse_result.result_type = "INPUT_PROPERTY"
-eclipse_result.result_variable = "OPERNUM_1"
-eclipse_result.update()
-
-# Set eclipse result for non-net layers
-non_net_layers = stim_plan_model_template.non_net_layers()
-non_net_layers_result = non_net_layers.facies_definition()
-non_net_layers_result.result_type = "STATIC_NATIVE"
-non_net_layers_result.result_variable = "NTG"
-non_net_layers_result.update()
-non_net_layers.formation = "Not"
-non_net_layers.facies = "Shale"
-non_net_layers.update()
-
-
-# Add some scaling factors
-elastic_properties = stim_plan_model_template.elastic_properties()
-elastic_properties.add_property_scaling(
-    formation="Garn", facies="Calcite", property="YOUNGS_MODULUS", scale=1.44
-)
-
-
-well_name = "B-2 H"
-
-# Find a well
-well_path = project.well_path_by_name(well_name)
-print("well path:", well_path)
-stim_plan_model_collection = project.descendants(rips.StimPlanModelCollection)[0]
-
-
-export_folder = tempfile.gettempdir()
-
-stim_plan_models = []
-
-# Create and export a StimPlan model for each depth
-measured_depths = [3200.0, 3400.0, 3600.0]
-for measured_depth in measured_depths:
-    # Create stim plan model at a give measured depth
-    stim_plan_model = stim_plan_model_collection.append_stim_plan_model(
-        well_path=well_path,
-        measured_depth=measured_depth,
-        stim_plan_model_template=stim_plan_model_template,
-    )
-    stim_plan_models.append(stim_plan_model)
-
-    # Make the well name safer to use as a directory path
-    well_name_part = well_name.replace(" ", "_")
-    directory_path = Path(export_folder) / "{}_{}".format(
-        well_name_part, int(measured_depth)
-    )
-
-    # Create the folder
-    directory_path.mkdir(parents=True, exist_ok=True)
-
-    print("Exporting fracture model to: ", directory_path)
-    stim_plan_model.export_to_file(directory_path=directory_path.as_posix())
-
-    # Create a fracture mode plot
-    stim_plan_model_plot_collection = project.descendants(
-        rips.StimPlanModelPlotCollection
-    )[0]
-    stim_plan_model_plot = stim_plan_model_plot_collection.append_stim_plan_model_plot(
-        stim_plan_model=stim_plan_model
-    )
-
-    print("Exporting fracture model plot to: ", directory_path)
-    stim_plan_model_plot.export_snapshot(export_folder=directory_path.as_posix())
-
-
-print("Setting measured depth and perforation length.")
-stim_plan_models[0].measured_depth = 3300.0
-stim_plan_models[0].perforation_length = 123.445
-stim_plan_models[0].update()
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+# Example code
+project = resinsight.project
+
+# Look for input files in the home directory of the user
+home_dir = expanduser("~")
+elastic_properties_file_path = (Path(home_dir) / "elastic_properties.csv").as_posix()
+print("Elastic properties file path:", elastic_properties_file_path)
+
+facies_properties_file_path = (Path(home_dir) / "facies_id.roff").as_posix()
+print("Facies properties file path:", facies_properties_file_path)
+
+# Find a case
+cases = resinsight.project.cases()
+case = cases[1]
+
+# Use the last time step
+time_steps = case.time_steps()
+time_step = time_steps[len(time_steps) - 1]
+
+
+# Create stim plan model template
+fmt_collection = project.descendants(rips.StimPlanModelTemplateCollection)[0]
+stim_plan_model_template = fmt_collection.append_stim_plan_model_template(
+    eclipse_case=case,
+    time_step=time_step,
+    elastic_properties_file_path=elastic_properties_file_path,
+    facies_properties_file_path=facies_properties_file_path,
+)
+stim_plan_model_template.overburden_formation = "Garn"
+stim_plan_model_template.overburden_facies = "Shale"
+stim_plan_model_template.underburden_formation = "Garn"
+stim_plan_model_template.underburden_facies = "Shale"
+stim_plan_model_template.overburden_height = 68
+stim_plan_model_template.update()
+print("Overburden: ", stim_plan_model_template.overburden_formation)
+
+
+# Set eclipse result for facies definition
+eclipse_result = stim_plan_model_template.facies_properties().facies_definition()
+eclipse_result.result_type = "INPUT_PROPERTY"
+eclipse_result.result_variable = "OPERNUM_1"
+eclipse_result.update()
+
+# Set eclipse result for non-net layers
+non_net_layers = stim_plan_model_template.non_net_layers()
+non_net_layers_result = non_net_layers.facies_definition()
+non_net_layers_result.result_type = "STATIC_NATIVE"
+non_net_layers_result.result_variable = "NTG"
+non_net_layers_result.update()
+non_net_layers.formation = "Not"
+non_net_layers.facies = "Shale"
+non_net_layers.update()
+
+
+# Add some scaling factors
+elastic_properties = stim_plan_model_template.elastic_properties()
+elastic_properties.add_property_scaling(
+    formation="Garn", facies="Calcite", property="YOUNGS_MODULUS", scale=1.44
+)
+
+
+well_name = "B-2 H"
+
+# Find a well
+well_path = project.well_path_by_name(well_name)
+print("well path:", well_path)
+stim_plan_model_collection = project.descendants(rips.StimPlanModelCollection)[0]
+
+
+export_folder = tempfile.gettempdir()
+
+stim_plan_models = []
+
+# Create and export a StimPlan model for each depth
+measured_depths = [3200.0, 3400.0, 3600.0]
+for measured_depth in measured_depths:
+    # Create stim plan model at a give measured depth
+    stim_plan_model = stim_plan_model_collection.append_stim_plan_model(
+        well_path=well_path,
+        measured_depth=measured_depth,
+        stim_plan_model_template=stim_plan_model_template,
+    )
+    stim_plan_models.append(stim_plan_model)
+
+    # Make the well name safer to use as a directory path
+    well_name_part = well_name.replace(" ", "_")
+    directory_path = Path(export_folder) / "{}_{}".format(
+        well_name_part, int(measured_depth)
+    )
+
+    # Create the folder
+    directory_path.mkdir(parents=True, exist_ok=True)
+
+    print("Exporting fracture model to: ", directory_path)
+    stim_plan_model.export_to_file(directory_path=directory_path.as_posix())
+
+    # Create a fracture mode plot
+    stim_plan_model_plot_collection = project.descendants(
+        rips.StimPlanModelPlotCollection
+    )[0]
+    stim_plan_model_plot = stim_plan_model_plot_collection.append_stim_plan_model_plot(
+        stim_plan_model=stim_plan_model
+    )
+
+    print("Exporting fracture model plot to: ", directory_path)
+    stim_plan_model_plot.export_snapshot(export_folder=directory_path.as_posix())
+
+
+print("Setting measured depth and perforation length.")
+stim_plan_models[0].measured_depth = 3300.0
+stim_plan_models[0].perforation_length = 123.445
+stim_plan_models[0].update()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/create_intersection.py` & `rips-2023.6.0.2/rips/PythonExamples/create_intersection.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# Load ResInsight Processing Server Client Library
-import math, time
-import rips
-
-resinsight = rips.Instance.find()
-
-# The coordinates in this example is based on the Drogon test case from Equinor
-file_path = "e:/models/from_equinor_sftp/drogon-real0-iter3/DROGON-0.EGRID"
-
-case = resinsight.project.load_case(file_path)
-
-view = case.create_view()
-view.set_time_step(2)
-
-intersection_coll = resinsight.project.descendants(rips.IntersectionCollection)[0]
-
-# Add a CurveIntersection and set coordinates for the polyline
-intersection = intersection_coll.add_new_object(rips.CurveIntersection)
-intersection.points = [
-    [45854, 595757, 1500],
-    [46493, 534259.1, 1500],
-    [46598, 590044.1, 1500],
-]
-intersection.update()
-
-# Add a new modeled well path
-well_path_coll = resinsight.project.descendants(rips.WellPathCollection)[0]
-well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
-well_path.name = "Test Well-1"
-well_path.update()
-
-# Set reference coordinate
-geometry = well_path.well_path_geometry()
-reference_point = geometry.reference_point
-reference_point[0] = 458580
-reference_point[1] = 5935514
-reference_point[2] = 1742
-geometry.update()  # Commit updates back to ResInsight
-
-# Create the first well target at the reference point
-coord = [0, 0, 0]
-geometry.append_well_target(coord)
-
-# Append well target with fixed azimuth
-coord = [2229.10, -833.74, -74.70]
-target = geometry.append_well_target(
-    coord, use_fixed_azimuth=True, fixed_azimuth_value=45.1
-)
-
-# Append well target with fixed inclination
-coord = [3403.15, -1938.61, -80.93]
-target = geometry.append_well_target(
-    coord, use_fixed_inclination=True, fixed_inclination_value=115.2
-)
-
-coord = [4577.21, -3043.47, -87.15]
-target = geometry.append_well_target(coord)
-geometry.update()
-
-# Read out estimated dogleg and azimuth/inclination for well targets
-for w in geometry.well_path_targets():
-    print(
-        "DL1:{}   DL2:{}   Azi: {}   Incl: {}".format(
-            w.estimated_dogleg1,
-            w.estimated_dogleg2,
-            w.estimated_azimuth,
-            w.estimated_inclination,
-        )
-    )
-
-# Add a curve intersection based on the modeled well path
-well_path_intersection = intersection_coll.add_new_object(rips.CurveIntersection)
-well_path_intersection.type = "CS_WELL_PATH"
-well_path_intersection.well_path = well_path
-well_path_intersection.update()
+# Load ResInsight Processing Server Client Library
+import math, time
+import rips
+
+resinsight = rips.Instance.find()
+
+# The coordinates in this example is based on the Drogon test case from Equinor
+file_path = "e:/models/from_equinor_sftp/drogon-real0-iter3/DROGON-0.EGRID"
+
+case = resinsight.project.load_case(file_path)
+
+view = case.create_view()
+view.set_time_step(2)
+
+intersection_coll = resinsight.project.descendants(rips.IntersectionCollection)[0]
+
+# Add a CurveIntersection and set coordinates for the polyline
+intersection = intersection_coll.add_new_object(rips.CurveIntersection)
+intersection.points = [
+    [45854, 595757, 1500],
+    [46493, 534259.1, 1500],
+    [46598, 590044.1, 1500],
+]
+intersection.update()
+
+# Add a new modeled well path
+well_path_coll = resinsight.project.descendants(rips.WellPathCollection)[0]
+well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
+well_path.name = "Test Well-1"
+well_path.update()
+
+# Set reference coordinate
+geometry = well_path.well_path_geometry()
+reference_point = geometry.reference_point
+reference_point[0] = 458580
+reference_point[1] = 5935514
+reference_point[2] = 1742
+geometry.update()  # Commit updates back to ResInsight
+
+# Create the first well target at the reference point
+coord = [0, 0, 0]
+geometry.append_well_target(coord)
+
+# Append well target with fixed azimuth
+coord = [2229.10, -833.74, -74.70]
+target = geometry.append_well_target(
+    coord, use_fixed_azimuth=True, fixed_azimuth_value=45.1
+)
+
+# Append well target with fixed inclination
+coord = [3403.15, -1938.61, -80.93]
+target = geometry.append_well_target(
+    coord, use_fixed_inclination=True, fixed_inclination_value=115.2
+)
+
+coord = [4577.21, -3043.47, -87.15]
+target = geometry.append_well_target(coord)
+geometry.update()
+
+# Read out estimated dogleg and azimuth/inclination for well targets
+for w in geometry.well_path_targets():
+    print(
+        "DL1:{}   DL2:{}   Azi: {}   Incl: {}".format(
+            w.estimated_dogleg1,
+            w.estimated_dogleg2,
+            w.estimated_azimuth,
+            w.estimated_inclination,
+        )
+    )
+
+# Add a curve intersection based on the modeled well path
+well_path_intersection = intersection_coll.add_new_object(rips.CurveIntersection)
+well_path_intersection.type = "CS_WELL_PATH"
+well_path_intersection.well_path = well_path
+well_path_intersection.update()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/create_surface_from_thermal_fracture.py` & `rips-2023.6.0.2/rips/PythonExamples/create_surface_from_thermal_fracture.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-import numpy as np
-import pyvista as pv
-
-
-def generate_surface_from_file(path):
-    point_cloud_data = np.loadtxt(path, delimiter=" ", skiprows=1)
-
-    # Get [x, y, z] components in separate matrix
-    num_rows = point_cloud_data.shape[0]
-    xyz = point_cloud_data[0:num_rows, 0:3]
-
-    # Generate surface
-    cloud = pv.PolyData(xyz)
-    surf = cloud.delaunay_2d()
-
-    # Read properties names from header data
-    f = open(path)
-    header = f.readline()
-    properties = header.strip().split(" ")
-
-    return (surf, point_cloud_data, properties)
-
-
-def export_surface_as_ts_file(surf, point_cloud, properties, path):
-    # open text file
-    text_file = open(path, "w")
-
-    # write GOCAD header
-    top_header = """GOCAD TSurf 1
-HEADER {
-name:MF_027_SU
-}
-"""
-
-    properties_str = "PROPERTIES " + " ".join(properties)
-
-    bottom_header = """
-GOCAD_ORIGINAL_COORDINATE_SYSTEM
-NAME Default
-AXIS_NAME "X" "Y" "Z"
-AXIS_UNIT "m" "m" "m"
-ZPOSITIVE Depth
-END_ORIGINAL_COORDINATE_SYSTEM
-TFACE
-"""
-
-    text_file.write(top_header)
-    text_file.write(properties_str)
-    text_file.write(bottom_header)
-
-    i = 1
-    (num_rows, num_props) = point_cloud.shape
-    for row in range(0, num_rows):
-        x = point_cloud[row, 0]
-        y = point_cloud[row, 1]
-        z = point_cloud[row, 2]
-        txt = "PVRTX {} {:.3f} {:.3f} {:.3f} ".format(i, x, y, z)
-        for property_index in range(0, num_props):
-            txt += "{:.3f} ".format(point_cloud[row, property_index])
-        txt += "\n"
-        text_file.write(txt)
-        i += 1
-
-    mysurface = surf.faces.reshape(-1, 4)
-    for p in mysurface:
-        txt = "TRGL {} {} {}\n".format(p[1] + 1, p[2] + 1, p[3] + 1)
-        text_file.write(txt)
-
-    text_file.write("END")
-    text_file.close()
-
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-project = resinsight.project
-
-
-fractures = project.descendants(rips.ThermalFractureTemplate)
-print("Number of thermal fractures: ", len(fractures))
-
-
-temp_folder = tempfile.gettempdir()
-
-# Write results to a suitable directory
-home_dir = expanduser("~")
-
-for fracture in fractures:
-    fracture_name = fracture.user_description
-
-    # Create the ouput directory
-    output_directory = (
-        Path(home_dir) / "thermal_fracture_surfaces" / "{}".format(fracture_name)
-    )
-
-    output_directory.mkdir(parents=True, exist_ok=True)
-    print("Creating result directory: ", output_directory.as_posix())
-
-    time_steps = fracture.time_steps().values
-    for time_step_index, time_step in enumerate(time_steps):
-        print(
-            "Generating surface for time step #{}: {}".format(
-                time_step_index, time_step
-            )
-        )
-        temp_file_path = Path(temp_folder) / "output.xyz"
-        fracture.export_to_file(
-            file_path=temp_file_path.as_posix(), time_step=time_step_index
-        )
-
-        # Reconstruct a surface from the exported values file
-        (surface, point_cloud, properties) = generate_surface_from_file(
-            temp_file_path.as_posix()
-        )
-
-        # Export surface ts file from the surface data
-        output_file_path = output_directory / "time_step_{:03d}.ts".format(
-            time_step_index
-        )
-        export_surface_as_ts_file(
-            surface, point_cloud, properties, output_file_path.as_posix()
-        )
-        print(
-            "Wrote surface for time step #{} to {}".format(
-                time_step, output_file_path.as_posix()
-            )
-        )
+#!/usr/bin/env python
+# coding: utf-8
+
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+import numpy as np
+import pyvista as pv
+
+
+def generate_surface_from_file(path):
+    point_cloud_data = np.loadtxt(path, delimiter=" ", skiprows=1)
+
+    # Get [x, y, z] components in separate matrix
+    num_rows = point_cloud_data.shape[0]
+    xyz = point_cloud_data[0:num_rows, 0:3]
+
+    # Generate surface
+    cloud = pv.PolyData(xyz)
+    surf = cloud.delaunay_2d()
+
+    # Read properties names from header data
+    f = open(path)
+    header = f.readline()
+    properties = header.strip().split(" ")
+
+    return (surf, point_cloud_data, properties)
+
+
+def export_surface_as_ts_file(surf, point_cloud, properties, path):
+    # open text file
+    text_file = open(path, "w")
+
+    # write GOCAD header
+    top_header = """GOCAD TSurf 1
+HEADER {
+name:MF_027_SU
+}
+"""
+
+    properties_str = "PROPERTIES " + " ".join(properties)
+
+    bottom_header = """
+GOCAD_ORIGINAL_COORDINATE_SYSTEM
+NAME Default
+AXIS_NAME "X" "Y" "Z"
+AXIS_UNIT "m" "m" "m"
+ZPOSITIVE Depth
+END_ORIGINAL_COORDINATE_SYSTEM
+TFACE
+"""
+
+    text_file.write(top_header)
+    text_file.write(properties_str)
+    text_file.write(bottom_header)
+
+    i = 1
+    (num_rows, num_props) = point_cloud.shape
+    for row in range(0, num_rows):
+        x = point_cloud[row, 0]
+        y = point_cloud[row, 1]
+        z = point_cloud[row, 2]
+        txt = "PVRTX {} {:.3f} {:.3f} {:.3f} ".format(i, x, y, z)
+        for property_index in range(0, num_props):
+            txt += "{:.3f} ".format(point_cloud[row, property_index])
+        txt += "\n"
+        text_file.write(txt)
+        i += 1
+
+    mysurface = surf.faces.reshape(-1, 4)
+    for p in mysurface:
+        txt = "TRGL {} {} {}\n".format(p[1] + 1, p[2] + 1, p[3] + 1)
+        text_file.write(txt)
+
+    text_file.write("END")
+    text_file.close()
+
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+project = resinsight.project
+
+
+fractures = project.descendants(rips.ThermalFractureTemplate)
+print("Number of thermal fractures: ", len(fractures))
+
+
+temp_folder = tempfile.gettempdir()
+
+# Write results to a suitable directory
+home_dir = expanduser("~")
+
+for fracture in fractures:
+    fracture_name = fracture.user_description
+
+    # Create the ouput directory
+    output_directory = (
+        Path(home_dir) / "thermal_fracture_surfaces" / "{}".format(fracture_name)
+    )
+
+    output_directory.mkdir(parents=True, exist_ok=True)
+    print("Creating result directory: ", output_directory.as_posix())
+
+    time_steps = fracture.time_steps().values
+    for time_step_index, time_step in enumerate(time_steps):
+        print(
+            "Generating surface for time step #{}: {}".format(
+                time_step_index, time_step
+            )
+        )
+        temp_file_path = Path(temp_folder) / "output.xyz"
+        fracture.export_to_file(
+            file_path=temp_file_path.as_posix(), time_step=time_step_index
+        )
+
+        # Reconstruct a surface from the exported values file
+        (surface, point_cloud, properties) = generate_surface_from_file(
+            temp_file_path.as_posix()
+        )
+
+        # Export surface ts file from the surface data
+        output_file_path = output_directory / "time_step_{:03d}.ts".format(
+            time_step_index
+        )
+        export_surface_as_ts_file(
+            surface, point_cloud, properties, output_file_path.as_posix()
+        )
+        print(
+            "Wrote surface for time step #{} to {}".format(
+                time_step, output_file_path.as_posix()
+            )
+        )
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/create_wbs_plot.py` & `rips-2023.6.0.2/rips/PythonExamples/create_wbs_plot.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import os
-import grpc
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resInsight = rips.Instance.find()
-
-# Get all GeoMech cases
-cases = resInsight.project.descendants(rips.GeoMechCase)
-
-# Get all well paths
-well_paths = resInsight.project.well_paths()
-
-# Ensure there's at least one well path
-if len(well_paths) < 1:
-    print("No well paths in project")
-    exit(1)
-
-# Create a set of WbsParameters
-params = rips.WbsParameters()
-params.user_poisson_ratio = 0.23456
-params.user_ucs = 123
-
-# Loop through all cases
-for case in cases:
-    assert isinstance(case, rips.GeoMechCase)
-    min_res_depth, max_res_depth = case.reservoir_depth_range()
-
-    # Find a good output path
-    case_path = case.file_path
-    folder_name = os.path.dirname(case_path)
-
-    # Import formation names
-    case.import_formation_names(
-        formation_files=[
-            "D:/Projects/ResInsight-regression-test/ModelData/norne/Norne_ATW2013.lyr"
-        ]
-    )
-
-    # create a folder to hold the snapshots
-    dirname = os.path.join(folder_name, "snapshots")
-    print("Exporting to: " + dirname)
-
-    for well_path in well_paths[0:4]:  # Loop through the first five well paths
-        # Create plot with parameters
-        wbsplot = case.create_well_bore_stability_plot(
-            well_path=well_path.name, time_step=0, parameters=params
-        )
+import os
+import grpc
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resInsight = rips.Instance.find()
+
+# Get all GeoMech cases
+cases = resInsight.project.descendants(rips.GeoMechCase)
+
+# Get all well paths
+well_paths = resInsight.project.well_paths()
+
+# Ensure there's at least one well path
+if len(well_paths) < 1:
+    print("No well paths in project")
+    exit(1)
+
+# Create a set of WbsParameters
+params = rips.WbsParameters()
+params.user_poisson_ratio = 0.23456
+params.user_ucs = 123
+
+# Loop through all cases
+for case in cases:
+    assert isinstance(case, rips.GeoMechCase)
+    min_res_depth, max_res_depth = case.reservoir_depth_range()
+
+    # Find a good output path
+    case_path = case.file_path
+    folder_name = os.path.dirname(case_path)
+
+    # Import formation names
+    case.import_formation_names(
+        formation_files=[
+            "D:/Projects/ResInsight-regression-test/ModelData/norne/Norne_ATW2013.lyr"
+        ]
+    )
+
+    # create a folder to hold the snapshots
+    dirname = os.path.join(folder_name, "snapshots")
+    print("Exporting to: " + dirname)
+
+    for well_path in well_paths[0:4]:  # Loop through the first five well paths
+        # Create plot with parameters
+        wbsplot = case.create_well_bore_stability_plot(
+            well_path=well_path.name, time_step=0, parameters=params
+        )
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/error_handling.py` & `rips-2023.6.0.2/rips/PythonExamples/error_handling.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-###################################################################
-# This example demonstrates the use of ResInsight exceptions
-# for proper error handling
-###################################################################
-
-import rips
-import grpc
-import tempfile
-
-resinsight = rips.Instance.find()
-
-case = None
-
-# Try loading a non-existing case. We should get a grpc.RpcError exception from the server
-try:
-    case = resinsight.project.load_case("Nonsense")
-except grpc.RpcError as e:
-    print(
-        "Expected Server Exception Received while loading case: ", e.code(), e.details()
-    )
-
-# Try loading well paths from a non-existing folder.  We should get a grpc.RpcError exception from the server
-try:
-    well_path_files = resinsight.project.import_well_paths(
-        well_path_folder="NONSENSE/NONSENSE"
-    )
-except grpc.RpcError as e:
-    print(
-        "Expected Server Exception Received while loading wellpaths: ",
-        e.code(),
-        e.details(),
-    )
-
-# Try loading well paths from an existing but empty folder. We should get a warning.
-try:
-    with tempfile.TemporaryDirectory() as tmpdirname:
-        well_path_files = resinsight.project.import_well_paths(
-            well_path_folder=tmpdirname
-        )
-        assert len(well_path_files) == 0
-        assert resinsight.project.has_warnings()
-        print("Should get warnings below")
-        for warning in resinsight.project.warnings():
-            print(warning)
-except grpc.RpcError as e:
-    print("Unexpected Server Exception caught!!!", e)
-
-case = resinsight.project.case(case_id=0)
-if case is not None:
-    results = case.active_cell_property("STATIC_NATIVE", "PORO", 0)
-    active_cell_count = len(results)
-
-    # Send the results back to ResInsight inside try / except construct
-    try:
-        case.set_active_cell_property(results, "GENERATED", "POROAPPENDED", 0)
-        print("Everything went well as expected")
-    except:  # Match any exception, but it should not happen
-        print("Ooops!")
-
-    # Add another value, so this is outside the bounds of the active cell result storage
-    results.append(1.0)
-
-    # This time we should get a grpc.RpcError exception, which is a server side error.
-    try:
-        case.set_active_cell_property(results, "GENERATED", "POROAPPENDED", 0)
-        print("Everything went well??")
-    except grpc.RpcError as e:
-        print("Expected Server Exception Received: ", e)
-    except IndexError:
-        print("Got index out of bounds error. This shouldn't happen here")
-
-    # With a chunk size exactly matching the active cell count the server will not
-    # be able to see any error as it will successfully close the stream after receiving
-    # the correct number of values, even if the python client has more chunks to send
-    case.chunk_size = active_cell_count
-
-    try:
-        case.set_active_cell_property(results, "GENERATED", "POROAPPENDED", 0)
-        print("Everything went well??")
-    except grpc.RpcError as e:
-        print("Got unexpected server exception", e, "This should not happen now")
-    except IndexError:
-        print("Got expected index out of bounds error on client side")
+###################################################################
+# This example demonstrates the use of ResInsight exceptions
+# for proper error handling
+###################################################################
+
+import rips
+import grpc
+import tempfile
+
+resinsight = rips.Instance.find()
+
+case = None
+
+# Try loading a non-existing case. We should get a grpc.RpcError exception from the server
+try:
+    case = resinsight.project.load_case("Nonsense")
+except grpc.RpcError as e:
+    print(
+        "Expected Server Exception Received while loading case: ", e.code(), e.details()
+    )
+
+# Try loading well paths from a non-existing folder.  We should get a grpc.RpcError exception from the server
+try:
+    well_path_files = resinsight.project.import_well_paths(
+        well_path_folder="NONSENSE/NONSENSE"
+    )
+except grpc.RpcError as e:
+    print(
+        "Expected Server Exception Received while loading wellpaths: ",
+        e.code(),
+        e.details(),
+    )
+
+# Try loading well paths from an existing but empty folder. We should get a warning.
+try:
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        well_path_files = resinsight.project.import_well_paths(
+            well_path_folder=tmpdirname
+        )
+        assert len(well_path_files) == 0
+        assert resinsight.project.has_warnings()
+        print("Should get warnings below")
+        for warning in resinsight.project.warnings():
+            print(warning)
+except grpc.RpcError as e:
+    print("Unexpected Server Exception caught!!!", e)
+
+case = resinsight.project.case(case_id=0)
+if case is not None:
+    results = case.active_cell_property("STATIC_NATIVE", "PORO", 0)
+    active_cell_count = len(results)
+
+    # Send the results back to ResInsight inside try / except construct
+    try:
+        case.set_active_cell_property(results, "GENERATED", "POROAPPENDED", 0)
+        print("Everything went well as expected")
+    except:  # Match any exception, but it should not happen
+        print("Ooops!")
+
+    # Add another value, so this is outside the bounds of the active cell result storage
+    results.append(1.0)
+
+    # This time we should get a grpc.RpcError exception, which is a server side error.
+    try:
+        case.set_active_cell_property(results, "GENERATED", "POROAPPENDED", 0)
+        print("Everything went well??")
+    except grpc.RpcError as e:
+        print("Expected Server Exception Received: ", e)
+    except IndexError:
+        print("Got index out of bounds error. This shouldn't happen here")
+
+    # With a chunk size exactly matching the active cell count the server will not
+    # be able to see any error as it will successfully close the stream after receiving
+    # the correct number of values, even if the python client has more chunks to send
+    case.chunk_size = active_cell_count
+
+    try:
+        case.set_active_cell_property(results, "GENERATED", "POROAPPENDED", 0)
+        print("Everything went well??")
+    except grpc.RpcError as e:
+        print("Got unexpected server exception", e, "This should not happen now")
+    except IndexError:
+        print("Got expected index out of bounds error on client side")
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/export_plots.py` & `rips-2023.6.0.2/rips/PythonExamples/export_plots.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Import the tempfile module
-import tempfile
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resInsight = rips.Instance.find()
-
-# Get a list of all plots
-plots = resInsight.project.plots()
-
-export_folder = tempfile.mkdtemp()
-
-print("Exporting to: " + export_folder)
-
-for plot in plots:
-    plot.export_snapshot(export_folder=export_folder)
-    plot.export_snapshot(export_folder=export_folder, output_format="PDF")
-    if isinstance(plot, rips.WellLogPlot):
-        plot.export_data_as_las(export_folder=export_folder)
-        plot.export_data_as_ascii(export_folder=export_folder)
+# Import the tempfile module
+import tempfile
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resInsight = rips.Instance.find()
+
+# Get a list of all plots
+plots = resInsight.project.plots()
+
+export_folder = tempfile.mkdtemp()
+
+print("Exporting to: " + export_folder)
+
+for plot in plots:
+    plot.export_snapshot(export_folder=export_folder)
+    plot.export_snapshot(export_folder=export_folder, output_format="PDF")
+    if isinstance(plot, rips.WellLogPlot):
+        plot.export_data_as_las(export_folder=export_folder)
+        plot.export_data_as_ascii(export_folder=export_folder)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/export_snapshots.py` & `rips-2023.6.0.2/rips/PythonExamples/export_snapshots.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-############################################################################
-# This script will export snapshots for two properties in every loaded case
-# And put them in a snapshots folder in the same folder as the case grid
-############################################################################
-import os
-import rips
-
-# Load instance
-resinsight = rips.Instance.find()
-cases = resinsight.project.cases()
-
-# Set main window size
-resinsight.set_main_window_size(width=800, height=500)
-
-n = 5  # every n-th time_step for snapshot
-property_list = ["SOIL", "PRESSURE"]  # list of parameter for snapshot
-
-print("Looping through cases")
-for case in cases:
-    print("Case name: ", case.name)
-    print("Case id: ", case.id)
-    # Get grid path and its folder name
-    case_path = case.file_path
-    folder_name = os.path.dirname(case_path)
-
-    # create a folder to hold the snapshots
-    dirname = os.path.join(folder_name, "snapshots")
-
-    if os.path.exists(dirname) is False:
-        os.mkdir(dirname)
-
-    print("Exporting to folder: " + dirname)
-    resinsight.set_export_folder(export_type="SNAPSHOTS", path=dirname)
-
-    time_steps = case.time_steps()
-    print("Number of time_steps: " + str(len(time_steps)))
-
-    for view in case.views():
-        for property in property_list:
-            view.apply_cell_result(
-                result_type="DYNAMIC_NATIVE", result_variable=property
-            )
-        for time_step in range(0, len(time_steps), 10):
-            view.set_time_step(time_step=time_step)
-            view.export_snapshot()
+############################################################################
+# This script will export snapshots for two properties in every loaded case
+# And put them in a snapshots folder in the same folder as the case grid
+############################################################################
+import os
+import rips
+
+# Load instance
+resinsight = rips.Instance.find()
+cases = resinsight.project.cases()
+
+# Set main window size
+resinsight.set_main_window_size(width=800, height=500)
+
+n = 5  # every n-th time_step for snapshot
+property_list = ["SOIL", "PRESSURE"]  # list of parameter for snapshot
+
+print("Looping through cases")
+for case in cases:
+    print("Case name: ", case.name)
+    print("Case id: ", case.id)
+    # Get grid path and its folder name
+    case_path = case.file_path
+    folder_name = os.path.dirname(case_path)
+
+    # create a folder to hold the snapshots
+    dirname = os.path.join(folder_name, "snapshots")
+
+    if os.path.exists(dirname) is False:
+        os.mkdir(dirname)
+
+    print("Exporting to folder: " + dirname)
+    resinsight.set_export_folder(export_type="SNAPSHOTS", path=dirname)
+
+    time_steps = case.time_steps()
+    print("Number of time_steps: " + str(len(time_steps)))
+
+    for view in case.views():
+        for property in property_list:
+            view.apply_cell_result(
+                result_type="DYNAMIC_NATIVE", result_variable=property
+            )
+        for time_step in range(0, len(time_steps), 10):
+            view.set_time_step(time_step=time_step)
+            view.export_snapshot()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_of_well_logs.py` & `rips-2023.6.0.2/rips/PythonExamples/generate_ensemble_of_well_logs.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-
-home_dir = expanduser("~")
-
-
-properties = [
-    ("STATIC_NATIVE", "INDEX_K", 0),
-    ("STATIC_NATIVE", "PORO", 0),
-    ("STATIC_NATIVE", "PERMX", 0),
-    ("DYNAMIC_NATIVE", "PRESSURE", 0),
-]
-
-export_folder = tempfile.mkdtemp()
-
-directory_path = "resprojects/webviz-subsurface-testdata/reek_history_match/"
-
-
-case_file_paths = []
-num_realizations = 9
-num_iterations = 4
-
-
-for realization in range(0, num_realizations):
-    for iteration in range(0, num_iterations):
-        realization_dir = "realization-" + str(realization)
-        iteration_dir = "iter-" + str(iteration)
-        egrid_name = "eclipse/model/5_R001_REEK-" + str(realization) + ".EGRID"
-        path = Path(
-            home_dir, directory_path, realization_dir, iteration_dir, egrid_name
-        )
-        case_file_paths.append(path)
-
-for path in case_file_paths:
-    # Load a case
-    path_name = path.as_posix()
-    grid_only = True
-    case = resinsight.project.load_case(path_name, grid_only)
-
-    # Load some wells
-    well_paths = resinsight.project.import_well_paths(
-        well_path_files=[
-            Path(home_dir, directory_path, "wellpaths", "Well-1.dev").as_posix(),
-            Path(home_dir, directory_path, "wellpaths", "Well-2.dev").as_posix(),
-        ]
-    )
-
-    if resinsight.project.has_warnings():
-        for warning in resinsight.project.warnings():
-            print(warning)
-
-    well_log_plot_collection = resinsight.project.descendants(
-        rips.WellLogPlotCollection
-    )[0]
-
-    for well_path in well_paths:
-        print(
-            "Generating las file for well: " + well_path.name + " in case: " + path_name
-        )
-
-        well_log_plot = well_log_plot_collection.new_well_log_plot(case, well_path)
-
-        # Create a track for each property
-        for prop_type, prop_name, time_step in properties:
-            track = well_log_plot.new_well_log_track(
-                "Track: " + prop_name, case, well_path
-            )
-
-            c = track.add_extraction_curve(
-                case, well_path, prop_type, prop_name, time_step
-            )
-
-        parent_path = path.parent
-        export_folder_path = Path(parent_path, "lasexport")
-        export_folder_path.mkdir(parents=True, exist_ok=True)
-
-        export_folder = export_folder_path.as_posix()
-        well_log_plot.export_data_as_las(export_folder=export_folder)
-
-    resinsight.project.close()
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+
+home_dir = expanduser("~")
+
+
+properties = [
+    ("STATIC_NATIVE", "INDEX_K", 0),
+    ("STATIC_NATIVE", "PORO", 0),
+    ("STATIC_NATIVE", "PERMX", 0),
+    ("DYNAMIC_NATIVE", "PRESSURE", 0),
+]
+
+export_folder = tempfile.mkdtemp()
+
+directory_path = "resprojects/webviz-subsurface-testdata/reek_history_match/"
+
+
+case_file_paths = []
+num_realizations = 9
+num_iterations = 4
+
+
+for realization in range(0, num_realizations):
+    for iteration in range(0, num_iterations):
+        realization_dir = "realization-" + str(realization)
+        iteration_dir = "iter-" + str(iteration)
+        egrid_name = "eclipse/model/5_R001_REEK-" + str(realization) + ".EGRID"
+        path = Path(
+            home_dir, directory_path, realization_dir, iteration_dir, egrid_name
+        )
+        case_file_paths.append(path)
+
+for path in case_file_paths:
+    # Load a case
+    path_name = path.as_posix()
+    grid_only = True
+    case = resinsight.project.load_case(path_name, grid_only)
+
+    # Load some wells
+    well_paths = resinsight.project.import_well_paths(
+        well_path_files=[
+            Path(home_dir, directory_path, "wellpaths", "Well-1.dev").as_posix(),
+            Path(home_dir, directory_path, "wellpaths", "Well-2.dev").as_posix(),
+        ]
+    )
+
+    if resinsight.project.has_warnings():
+        for warning in resinsight.project.warnings():
+            print(warning)
+
+    well_log_plot_collection = resinsight.project.descendants(
+        rips.WellLogPlotCollection
+    )[0]
+
+    for well_path in well_paths:
+        print(
+            "Generating las file for well: " + well_path.name + " in case: " + path_name
+        )
+
+        well_log_plot = well_log_plot_collection.new_well_log_plot(case, well_path)
+
+        # Create a track for each property
+        for prop_type, prop_name, time_step in properties:
+            track = well_log_plot.new_well_log_track(
+                "Track: " + prop_name, case, well_path
+            )
+
+            c = track.add_extraction_curve(
+                case, well_path, prop_type, prop_name, time_step
+            )
+
+        parent_path = path.parent
+        export_folder_path = Path(parent_path, "lasexport")
+        export_folder_path.mkdir(parents=True, exist_ok=True)
+
+        export_folder = export_folder_path.as_posix()
+        well_log_plot.export_data_as_las(export_folder=export_folder)
+
+    resinsight.project.close()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface.py` & `rips-2023.6.0.2/rips/PythonExamples/generate_ensemble_surface.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-
-home_dir = expanduser("~")
-
-export_folder = tempfile.mkdtemp()
-
-directory_path = "resprojects/webviz-subsurface-testdata/reek_history_match/"
-# directory_path = "e:/gitroot/webviz-subsurface-testdata/reek_history_match"
-
-
-case_file_paths = []
-num_realizations = 9
-num_iterations = 4
-
-
-for realization in range(0, num_realizations):
-    for iteration in range(0, num_iterations):
-        realization_dir = "realization-" + str(realization)
-        iteration_dir = "iter-" + str(iteration)
-        egrid_name = "eclipse/model/5_R001_REEK-" + str(realization) + ".EGRID"
-        path = Path(
-            home_dir, directory_path, realization_dir, iteration_dir, egrid_name
-        )
-        case_file_paths.append(path)
-
-k_indexes = [4, 10]
-
-for path in case_file_paths:
-    # Load a case
-    path_name = path.as_posix()
-    case = resinsight.project.load_case(path_name)
-
-    if resinsight.project.has_warnings():
-        for warning in resinsight.project.warnings():
-            print(warning)
-
-    surface_collection = resinsight.project.descendants(rips.SurfaceCollection)[0]
-
-    for k_index in k_indexes:
-        print("Generating surface K layer " + str(k_index) + " for case " + path_name)
-
-        surface = surface_collection.new_surface(case, k_index)
-        print("Surface: ", surface)
-
-        parent_path = path.parent
-        export_folder_path = Path(parent_path, "surfaceexport")
-        export_folder_path.mkdir(parents=True, exist_ok=True)
-
-        export_file = Path(export_folder_path, "surf_" + str(k_index) + ".ts")
-        print("Exporting to " + export_file.as_posix())
-        surface.export_to_file(export_file.as_posix())
-
-    # Close project to avoid aggregated memory usage
-    # Can be replaced when case.close() is implemented
-    resinsight.project.close()
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+
+home_dir = expanduser("~")
+
+export_folder = tempfile.mkdtemp()
+
+directory_path = "resprojects/webviz-subsurface-testdata/reek_history_match/"
+# directory_path = "e:/gitroot/webviz-subsurface-testdata/reek_history_match"
+
+
+case_file_paths = []
+num_realizations = 9
+num_iterations = 4
+
+
+for realization in range(0, num_realizations):
+    for iteration in range(0, num_iterations):
+        realization_dir = "realization-" + str(realization)
+        iteration_dir = "iter-" + str(iteration)
+        egrid_name = "eclipse/model/5_R001_REEK-" + str(realization) + ".EGRID"
+        path = Path(
+            home_dir, directory_path, realization_dir, iteration_dir, egrid_name
+        )
+        case_file_paths.append(path)
+
+k_indexes = [4, 10]
+
+for path in case_file_paths:
+    # Load a case
+    path_name = path.as_posix()
+    case = resinsight.project.load_case(path_name)
+
+    if resinsight.project.has_warnings():
+        for warning in resinsight.project.warnings():
+            print(warning)
+
+    surface_collection = resinsight.project.descendants(rips.SurfaceCollection)[0]
+
+    for k_index in k_indexes:
+        print("Generating surface K layer " + str(k_index) + " for case " + path_name)
+
+        surface = surface_collection.new_surface(case, k_index)
+        print("Surface: ", surface)
+
+        parent_path = path.parent
+        export_folder_path = Path(parent_path, "surfaceexport")
+        export_folder_path.mkdir(parents=True, exist_ok=True)
+
+        export_file = Path(export_folder_path, "surf_" + str(k_index) + ".ts")
+        print("Exporting to " + export_file.as_posix())
+        surface.export_to_file(export_file.as_posix())
+
+    # Close project to avoid aggregated memory usage
+    # Can be replaced when case.close() is implemented
+    resinsight.project.close()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/generate_ensemble_surface_optimized.py` & `rips-2023.6.0.2/rips/PythonExamples/generate_ensemble_surface_optimized.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-
-home_dir = expanduser("~")
-
-export_folder = tempfile.mkdtemp()
-
-directory_path = "resprojects/webviz-subsurface-testdata/reek_history_match/"
-# directory_path = "e:/gitroot/webviz-subsurface-testdata/reek_history_match"
-
-
-case_file_paths = []
-num_realizations = 9
-num_iterations = 4
-
-
-for realization in range(0, num_realizations):
-    for iteration in range(0, num_iterations):
-        realization_dir = "realization-" + str(realization)
-        iteration_dir = "iter-" + str(iteration)
-        egrid_name = "eclipse/model/5_R001_REEK-" + str(realization) + ".EGRID"
-        path = Path(
-            home_dir, directory_path, realization_dir, iteration_dir, egrid_name
-        )
-        case_file_paths.append(path)
-
-k_indexes = [4, 10]
-
-command_router = resinsight.command_router
-
-for path in case_file_paths:
-    path_name = path.as_posix()
-
-    command_router.extract_surfaces(path_name, k_indexes)
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+
+home_dir = expanduser("~")
+
+export_folder = tempfile.mkdtemp()
+
+directory_path = "resprojects/webviz-subsurface-testdata/reek_history_match/"
+# directory_path = "e:/gitroot/webviz-subsurface-testdata/reek_history_match"
+
+
+case_file_paths = []
+num_realizations = 9
+num_iterations = 4
+
+
+for realization in range(0, num_realizations):
+    for iteration in range(0, num_iterations):
+        realization_dir = "realization-" + str(realization)
+        iteration_dir = "iter-" + str(iteration)
+        egrid_name = "eclipse/model/5_R001_REEK-" + str(realization) + ".EGRID"
+        path = Path(
+            home_dir, directory_path, realization_dir, iteration_dir, egrid_name
+        )
+        case_file_paths.append(path)
+
+k_indexes = [4, 10]
+
+command_router = resinsight.command_router
+
+for path in case_file_paths:
+    path_name = path.as_posix()
+
+    command_router.extract_surfaces(path_name, k_indexes)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/grid_information.py` & `rips-2023.6.0.2/rips/PythonExamples/grid_information.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-######################################################################################
-# This example prints information about the grids of all cases in the current project
-######################################################################################
-
-import rips
-
-resinsight = rips.Instance.find()
-
-cases = resinsight.project.cases()
-print("Number of cases found: ", len(cases))
-for case in cases:
-    print(case.name)
-    grids = case.grids()
-    print("Number of grids: ", len(grids))
-    for grid in grids:
-        print("Grid dimensions: ", grid.dimensions())
+######################################################################################
+# This example prints information about the grids of all cases in the current project
+######################################################################################
+
+import rips
+
+resinsight = rips.Instance.find()
+
+cases = resinsight.project.cases()
+print("Number of cases found: ", len(cases))
+for case in cases:
+    print(case.name)
+    grids = case.grids()
+    print("Number of grids: ", len(grids))
+    for grid in grids:
+        print("Grid dimensions: ", grid.dimensions())
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/headless_plot_export.py` & `rips-2023.6.0.2/rips/PythonExamples/headless_plot_export.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import sys
-import os
-
-import rips
-
-use_platform_offscreen = True
-if use_platform_offscreen:
-    # To use offscreen, the path to fonts must be specified in the environment variable QT_QPA_FONTDIR="C:/windows/fonts"
-    resinsight = rips.Instance.launch(
-        command_line_parameters=["-platform", "offscreen", "--size", 1200, 1000]
-    )
-
-    qpa_fontdir = os.environ["QT_QPA_FONTDIR"]
-    print("Environment var QT_QPA_FONTDIR : " + qpa_fontdir)
-else:
-    resinsight = rips.Instance.find()
-
-summary_filename = "NORNE.SMSPEC"
-
-project = resinsight.project
-summary_case = project.import_summary_case(summary_filename)
-
-summary_plot_collection = project.descendants(rips.SummaryPlotCollection)[0]
-
-summary_plot_collection.new_summary_plot(summary_cases=[summary_case], address="FOPR")
-summary_plot_collection.new_summary_plot(
-    summary_cases=[summary_case], address="WOPR:A*;WOPR:B*"
-)
-
-plots = resinsight.project.plots()
-for plot in plots:
-    plot.export_snapshot()
-    # plot.export_snapshot(output_format="PDF")
-
-resinsight.exit()
+import sys
+import os
+
+import rips
+
+use_platform_offscreen = True
+if use_platform_offscreen:
+    # To use offscreen, the path to fonts must be specified in the environment variable QT_QPA_FONTDIR="C:/windows/fonts"
+    resinsight = rips.Instance.launch(
+        command_line_parameters=["-platform", "offscreen", "--size", 1200, 1000]
+    )
+
+    qpa_fontdir = os.environ["QT_QPA_FONTDIR"]
+    print("Environment var QT_QPA_FONTDIR : " + qpa_fontdir)
+else:
+    resinsight = rips.Instance.find()
+
+summary_filename = "NORNE.SMSPEC"
+
+project = resinsight.project
+summary_case = project.import_summary_case(summary_filename)
+
+summary_plot_collection = project.descendants(rips.SummaryPlotCollection)[0]
+
+summary_plot_collection.new_summary_plot(summary_cases=[summary_case], address="FOPR")
+summary_plot_collection.new_summary_plot(
+    summary_cases=[summary_case], address="WOPR:A*;WOPR:B*"
+)
+
+plots = resinsight.project.plots()
+for plot in plots:
+    plot.export_snapshot()
+    # plot.export_snapshot(output_format="PDF")
+
+resinsight.exit()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/import_fractures_on_well.py` & `rips-2023.6.0.2/rips/PythonExamples/import_fractures_on_well.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-project = resinsight.project
-
-# Look for input files in the home directory of the user
-home_dir = expanduser("~")
-stim_plan_file_path = (Path(home_dir) / "contour.xml").as_posix()
-print("StimPlan contour file path:", stim_plan_file_path)
-
-# Find a case
-cases = resinsight.project.cases()
-case = cases[0]
-
-# Create stim plan template
-fmt_collection = project.descendants(rips.FractureTemplateCollection)[0]
-fracture_template = fmt_collection.append_fracture_template(
-    file_path=stim_plan_file_path
-)
-
-well_name = "B-2 H"
-
-# Find a well
-well_path = project.well_path_by_name(well_name)
-print("well path:", well_path.name)
-
-# Place fracture at given depths
-measured_depths = [3200.0, 3400.0, 3600.0]
-for measured_depth in measured_depths:
-    print("Placing fracture at {} depth (MD)".format(measured_depth))
-    # Create stim plan  at a give measured depth
-    fracture = well_path.add_fracture(
-        measured_depth=measured_depth,
-        stim_plan_fracture_template=fracture_template,
-        align_dip=True,
-        eclipse_case=case,
-    )
-
-# Update the orientation of the fracture
-# Call update() to propagate changes from the Python object back to ResInsight
-fracture_template.orientation = "Azimuth"
-fracture_template.azimuth_angle = 60.0
-fracture_template.user_defined_perforation_length = True
-fracture_template.conductivity_type = "InfiniteConductivity"
-fracture_template.perforation_length = 12.3
-fracture_template.update()
-
-# Scale the template
-fracture_template.set_scale_factors(
-    half_length=2.0, height=2.0, d_factor=1.1, conductivity=1.2
-)
-
-# Output scale factors for all fracture templates
-fmt_collection = project.descendants(rips.FractureTemplate)
-for fracture_template in fmt_collection:
-    print(
-        "Fracture: '{}' Scale factors: Height={} Half Length={} D Factor={} Conductivity={}".format(
-            fracture_template.user_description,
-            fracture_template.height_scale_factor,
-            fracture_template.width_scale_factor,
-            fracture_template.d_factor_scale_factor,
-            fracture_template.conductivity_factor,
-        )
-    )
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+project = resinsight.project
+
+# Look for input files in the home directory of the user
+home_dir = expanduser("~")
+stim_plan_file_path = (Path(home_dir) / "contour.xml").as_posix()
+print("StimPlan contour file path:", stim_plan_file_path)
+
+# Find a case
+cases = resinsight.project.cases()
+case = cases[0]
+
+# Create stim plan template
+fmt_collection = project.descendants(rips.FractureTemplateCollection)[0]
+fracture_template = fmt_collection.append_fracture_template(
+    file_path=stim_plan_file_path
+)
+
+well_name = "B-2 H"
+
+# Find a well
+well_path = project.well_path_by_name(well_name)
+print("well path:", well_path.name)
+
+# Place fracture at given depths
+measured_depths = [3200.0, 3400.0, 3600.0]
+for measured_depth in measured_depths:
+    print("Placing fracture at {} depth (MD)".format(measured_depth))
+    # Create stim plan  at a give measured depth
+    fracture = well_path.add_fracture(
+        measured_depth=measured_depth,
+        stim_plan_fracture_template=fracture_template,
+        align_dip=True,
+        eclipse_case=case,
+    )
+
+# Update the orientation of the fracture
+# Call update() to propagate changes from the Python object back to ResInsight
+fracture_template.orientation = "Azimuth"
+fracture_template.azimuth_angle = 60.0
+fracture_template.user_defined_perforation_length = True
+fracture_template.conductivity_type = "InfiniteConductivity"
+fracture_template.perforation_length = 12.3
+fracture_template.update()
+
+# Scale the template
+fracture_template.set_scale_factors(
+    half_length=2.0, height=2.0, d_factor=1.1, conductivity=1.2
+)
+
+# Output scale factors for all fracture templates
+fmt_collection = project.descendants(rips.FractureTemplate)
+for fracture_template in fmt_collection:
+    print(
+        "Fracture: '{}' Scale factors: Height={} Half Length={} D Factor={} Conductivity={}".format(
+            fracture_template.user_description,
+            fracture_template.height_scale_factor,
+            fracture_template.width_scale_factor,
+            fracture_template.d_factor_scale_factor,
+            fracture_template.conductivity_factor,
+        )
+    )
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/import_thermal_fracture_on_well.py` & `rips-2023.6.0.2/rips/PythonExamples/import_thermal_fracture_on_well.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# Load ResInsight Processing Server Client Library
-import rips
-import tempfile
-from os.path import expanduser
-from pathlib import Path
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-project = resinsight.project
-
-# Look for input files in the home directory of the user
-home_dir = expanduser("~")
-fracture_file_path = (Path(home_dir) / "fracture.csv").as_posix()
-print("Thermal fracture file path:", fracture_file_path)
-
-# Find a case
-cases = resinsight.project.cases()
-case = cases[0]
-
-# Create thermal template
-fmt_collection = project.descendants(rips.FractureTemplateCollection)[0]
-fracture_template = fmt_collection.append_thermal_fracture_template(
-    file_path=fracture_file_path
-)
-
-well_name = "F-1 H"
-
-# Find a well
-well_path = project.well_path_by_name(well_name)
-print("Well path:", well_path.name)
-
-# Create fracture and place it using data from the fracture template
-fracture = well_path.add_thermal_fracture(
-    fracture_template=fracture_template,
-    place_using_template_data=True,
-)
-
-
-time_steps = fracture_template.time_steps().values
-for time_step_index, time_stamp in enumerate(time_steps):
-    print("Time step #{}: {}".format(time_step_index, time_stamp))
-    fracture_template.active_time_step_index = time_step_index
-    fracture_template.conductivity_result_name = "Conductivity"
-    fracture_template.update()
+# Load ResInsight Processing Server Client Library
+import rips
+import tempfile
+from os.path import expanduser
+from pathlib import Path
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+project = resinsight.project
+
+# Look for input files in the home directory of the user
+home_dir = expanduser("~")
+fracture_file_path = (Path(home_dir) / "fracture.csv").as_posix()
+print("Thermal fracture file path:", fracture_file_path)
+
+# Find a case
+cases = resinsight.project.cases()
+case = cases[0]
+
+# Create thermal template
+fmt_collection = project.descendants(rips.FractureTemplateCollection)[0]
+fracture_template = fmt_collection.append_thermal_fracture_template(
+    file_path=fracture_file_path
+)
+
+well_name = "F-1 H"
+
+# Find a well
+well_path = project.well_path_by_name(well_name)
+print("Well path:", well_path.name)
+
+# Create fracture and place it using data from the fracture template
+fracture = well_path.add_thermal_fracture(
+    fracture_template=fracture_template,
+    place_using_template_data=True,
+)
+
+
+time_steps = fracture_template.time_steps().values
+for time_step_index, time_stamp in enumerate(time_steps):
+    print("Time step #{}: {}".format(time_step_index, time_stamp))
+    fracture_template.active_time_step_index = time_step_index
+    fracture_template.conductivity_result_name = "Conductivity"
+    fracture_template.update()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/input_prop_test_async.py` & `rips-2023.6.0.2/rips/PythonExamples/input_prop_test_async.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-########################################################################################
-# This example generates a derived property in an asynchronous manner
-# Meaning it does not wait for all the data for each stage to be read before proceeding
-########################################################################################
-import rips
-import time
-
-
-# Internal function for creating a result from a small chunk of poro and permx results
-# The return value of the function is a generator for the results rather than the result itself.
-def create_result(poro_chunks, permx_chunks):
-    # Loop through all the chunks of poro and permx in order
-    for poroChunk, permxChunk in zip(poro_chunks, permx_chunks):
-        resultChunk = []
-        # Loop through all the values inside the chunks, in order
-        for poro, permx in zip(poroChunk.values, permxChunk.values):
-            resultChunk.append(poro * permx)
-        # Return a generator object that behaves like a Python iterator
-        yield resultChunk
-
-
-resinsight = rips.Instance.find()
-start = time.time()
-case = resinsight.project.cases()[0]
-
-# Get a generator for the poro results. The generator will provide a chunk each time it is iterated
-poro_chunks = case.active_cell_property_async("STATIC_NATIVE", "PORO", 0)
-# Get a generator for the permx results. The generator will provide a chunk each time it is iterated
-permx_chunks = case.active_cell_property_async("STATIC_NATIVE", "PERMX", 0)
-
-# Send back the result with the result provided by a generator object.
-# Iterating the result generator will cause the script to read from the poro and permx generators
-# And return the result of each iteration
-case.set_active_cell_property_async(
-    create_result(poro_chunks, permx_chunks), "GENERATED", "POROPERMXAS", 0
-)
-
-end = time.time()
-print("Time elapsed: ", end - start)
-print("Transferred all results back")
-view = case.views()[0].apply_cell_result("GENERATED", "POROPERMXAS")
+########################################################################################
+# This example generates a derived property in an asynchronous manner
+# Meaning it does not wait for all the data for each stage to be read before proceeding
+########################################################################################
+import rips
+import time
+
+
+# Internal function for creating a result from a small chunk of poro and permx results
+# The return value of the function is a generator for the results rather than the result itself.
+def create_result(poro_chunks, permx_chunks):
+    # Loop through all the chunks of poro and permx in order
+    for poroChunk, permxChunk in zip(poro_chunks, permx_chunks):
+        resultChunk = []
+        # Loop through all the values inside the chunks, in order
+        for poro, permx in zip(poroChunk.values, permxChunk.values):
+            resultChunk.append(poro * permx)
+        # Return a generator object that behaves like a Python iterator
+        yield resultChunk
+
+
+resinsight = rips.Instance.find()
+start = time.time()
+case = resinsight.project.cases()[0]
+
+# Get a generator for the poro results. The generator will provide a chunk each time it is iterated
+poro_chunks = case.active_cell_property_async("STATIC_NATIVE", "PORO", 0)
+# Get a generator for the permx results. The generator will provide a chunk each time it is iterated
+permx_chunks = case.active_cell_property_async("STATIC_NATIVE", "PERMX", 0)
+
+# Send back the result with the result provided by a generator object.
+# Iterating the result generator will cause the script to read from the poro and permx generators
+# And return the result of each iteration
+case.set_active_cell_property_async(
+    create_result(poro_chunks, permx_chunks), "GENERATED", "POROPERMXAS", 0
+)
+
+end = time.time()
+print("Time elapsed: ", end - start)
+print("Transferred all results back")
+view = case.views()[0].apply_cell_result("GENERATED", "POROPERMXAS")
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/input_prop_test_sync.py` & `rips-2023.6.0.2/rips/PythonExamples/input_prop_test_sync.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-########################################################################################
-# This example generates a derived property in an synchronous manner
-# Meaning it completes reading each result before calculating the derived result
-# See InputPropTestAsync for how to do this asynchronously instead.
-########################################################################################
-import rips
-import time
-import grpc
-
-resinsight = rips.Instance.find()
-start = time.time()
-case = resinsight.project.cases()[0]
-
-# Read poro result into list
-poro_results = case.active_cell_property("STATIC_NATIVE", "PORO", 0)
-# Read permx result into list
-permx_results = case.active_cell_property("STATIC_NATIVE", "PERMX", 0)
-
-# Generate output result
-results = []
-for poro, permx in zip(poro_results, permx_results):
-    results.append(poro * permx)
-
-try:
-    # Send back output result
-    case.set_active_cell_property(results, "GENERATED", "POROPERMXSY", 0)
-except grpc.RpcError as e:
-    print("Exception Received: ", e)
-
-
-end = time.time()
-print("Time elapsed: ", end - start)
-print("Transferred all results back")
-
-view = case.views()[0].apply_cell_result("GENERATED", "POROPERMXSY")
+########################################################################################
+# This example generates a derived property in an synchronous manner
+# Meaning it completes reading each result before calculating the derived result
+# See InputPropTestAsync for how to do this asynchronously instead.
+########################################################################################
+import rips
+import time
+import grpc
+
+resinsight = rips.Instance.find()
+start = time.time()
+case = resinsight.project.cases()[0]
+
+# Read poro result into list
+poro_results = case.active_cell_property("STATIC_NATIVE", "PORO", 0)
+# Read permx result into list
+permx_results = case.active_cell_property("STATIC_NATIVE", "PERMX", 0)
+
+# Generate output result
+results = []
+for poro, permx in zip(poro_results, permx_results):
+    results.append(poro * permx)
+
+try:
+    # Send back output result
+    case.set_active_cell_property(results, "GENERATED", "POROPERMXSY", 0)
+except grpc.RpcError as e:
+    print("Exception Received: ", e)
+
+
+end = time.time()
+print("Time elapsed: ", end - start)
+print("Transferred all results back")
+
+view = case.views()[0].apply_cell_result("GENERATED", "POROPERMXSY")
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/launch_load_case_snapshot_exit.py` & `rips-2023.6.0.2/rips/PythonExamples/launch_load_case_snapshot_exit.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Access to environment variables
-import os
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.launch()
-
-# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
-resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
-
-# Get the TestModels path from the executable path
-resinsight_install_path = os.path.dirname(resinsight_exe_path)
-test_models_path = os.path.join(resinsight_install_path, "TestModels")
-path_name = os.path.join(
-    test_models_path, "TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-)
-
-# Load an example case. Needs to be replaced with a valid path!
-case = resinsight.project.load_case(path_name)
-
-# Get a view
-view1 = case.views()[0]
-
-# Set the time step for view1 only
-view1.set_time_step(time_step=2)
-
-# Set cell result to SOIL
-view1.apply_cell_result(result_type="DYNAMIC_NATIVE", result_variable="SOIL")
-
-# Set export folder for snapshots and properties
-resinsight.set_export_folder(export_type="SNAPSHOTS", path="e:/temp")
-resinsight.set_export_folder(export_type="PROPERTIES", path="e:/temp")
-
-# Export all snapshots
-resinsight.project.export_snapshots()
-
-# Export properties in the view
-view1.export_property()
-
-resinsight.exit()
+# Access to environment variables
+import os
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.launch()
+
+# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
+resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
+
+# Get the TestModels path from the executable path
+resinsight_install_path = os.path.dirname(resinsight_exe_path)
+test_models_path = os.path.join(resinsight_install_path, "TestModels")
+path_name = os.path.join(
+    test_models_path, "TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+)
+
+# Load an example case. Needs to be replaced with a valid path!
+case = resinsight.project.load_case(path_name)
+
+# Get a view
+view1 = case.views()[0]
+
+# Set the time step for view1 only
+view1.set_time_step(time_step=2)
+
+# Set cell result to SOIL
+view1.apply_cell_result(result_type="DYNAMIC_NATIVE", result_variable="SOIL")
+
+# Set export folder for snapshots and properties
+resinsight.set_export_folder(export_type="SNAPSHOTS", path="e:/temp")
+resinsight.set_export_folder(export_type="PROPERTIES", path="e:/temp")
+
+# Export all snapshots
+resinsight.project.export_snapshots()
+
+# Export properties in the view
+view1.export_property()
+
+resinsight.exit()
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/load_case.py` & `rips-2023.6.0.2/rips/PythonExamples/load_case.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Access to environment variables and path tools
-import os
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
-resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
-
-# Get the TestModels path from the executable path
-resinsight_install_path = os.path.dirname(resinsight_exe_path)
-test_models_path = os.path.join(resinsight_install_path, "TestModels")
-path_name = os.path.join(
-    test_models_path, "TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-)
-case = resinsight.project.load_case(path_name)
-case.create_view()
-
-# Print out lots of information from the case object
-print("Case id: " + str(case.id))
-print("Case name: " + case.name)
-print("Case type: " + case.__class__.__name__)
-print("Case file name: " + case.file_path)
-print("Case reservoir bounding box:", case.reservoir_boundingbox())
-
-timesteps = case.time_steps()
-for t in timesteps:
-    print("Year: " + str(t.year))
-    print("Month: " + str(t.month))
+# Access to environment variables and path tools
+import os
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
+resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
+
+# Get the TestModels path from the executable path
+resinsight_install_path = os.path.dirname(resinsight_exe_path)
+test_models_path = os.path.join(resinsight_install_path, "TestModels")
+path_name = os.path.join(
+    test_models_path, "TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+)
+case = resinsight.project.load_case(path_name)
+case.create_view()
+
+# Print out lots of information from the case object
+print("Case id: " + str(case.id))
+print("Case name: " + case.name)
+print("Case type: " + case.__class__.__name__)
+print("Case file name: " + case.file_path)
+print("Case reservoir bounding box:", case.reservoir_boundingbox())
+
+timesteps = case.time_steps()
+for t in timesteps:
+    print("Year: " + str(t.year))
+    print("Month: " + str(t.month))
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/modeled_well_path.py` & `rips-2023.6.0.2/rips/PythonExamples/modeled_well_path.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-# Create a modeled well path and add well path targets
-# The coordinates are based on the Norne case
-
-well_path_coll = resinsight.project.descendants(rips.WellPathCollection)[0]
-well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
-well_path.name = "Test Well-1"
-well_path.update()
-
-geometry = well_path.well_path_geometry()
-
-reference_point = geometry.reference_point
-reference_point[0] = 457196
-reference_point[1] = 7322270
-reference_point[2] = 2742
-geometry.update()  # Commit updates back to ResInsight
-
-# Create the first well target at the reference point
-coord = [0, 0, 0]
-geometry.append_well_target(coord)
-
-# Append new well targets relative the the reference point
-coord = [454.28, 250, -10]
-target = geometry.append_well_target(coord)
-
-coord = [1054.28, 250, -50]
-target = geometry.append_well_target(coord)
-
-well_path.append_perforation_interval(3300, 3350, 0.2, 0.76)
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+# Create a modeled well path and add well path targets
+# The coordinates are based on the Norne case
+
+well_path_coll = resinsight.project.descendants(rips.WellPathCollection)[0]
+well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
+well_path.name = "Test Well-1"
+well_path.update()
+
+geometry = well_path.well_path_geometry()
+
+reference_point = geometry.reference_point
+reference_point[0] = 457196
+reference_point[1] = 7322270
+reference_point[2] = 2742
+geometry.update()  # Commit updates back to ResInsight
+
+# Create the first well target at the reference point
+coord = [0, 0, 0]
+geometry.append_well_target(coord)
+
+# Append new well targets relative the the reference point
+coord = [454.28, 250, -10]
+target = geometry.append_well_target(coord)
+
+coord = [1054.28, 250, -50]
+target = geometry.append_well_target(coord)
+
+well_path.append_perforation_interval(3300, 3350, 0.2, 0.76)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/open_project.py` & `rips-2023.6.0.2/rips/PythonExamples/open_project.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Access to environment variables and path tools
-import os
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
-resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
-
-# Get the TestModels path from the executable path
-resinsight_install_path = os.path.dirname(resinsight_exe_path)
-test_models_path = os.path.join(resinsight_install_path, "TestModels")
-path_name = os.path.join(test_models_path, "TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp")
-
-# Open a project
-resinsight.project.open(path_name)
+# Access to environment variables and path tools
+import os
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
+resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
+
+# Get the TestModels path from the executable path
+resinsight_install_path = os.path.dirname(resinsight_exe_path)
+test_models_path = os.path.join(resinsight_install_path, "TestModels")
+path_name = os.path.join(test_models_path, "TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp")
+
+# Open a project
+resinsight.project.open(path_name)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/save_project.py` & `rips-2023.6.0.2/rips/PythonExamples/save_project.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Access to environment variables and path tools
-import os
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
-resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
-
-# Get the TestModels path from the executable path
-resinsight_install_path = os.path.dirname(resinsight_exe_path)
-test_models_path = os.path.join(resinsight_install_path, "TestModels")
-path_name = os.path.join(
-    test_models_path, "TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-)
-case = resinsight.project.load_case(path_name)
-
-# Save the project to file
-home_dir = os.path.expanduser("~")
-project_path = home_dir + "/new-project.rsp"
-print("Saving project to: ", project_path)
-resinsight.project.save(project_path)
+# Access to environment variables and path tools
+import os
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+# This requires the TestModels to be installed with ResInsight (RESINSIGHT_BUNDLE_TESTMODELS):
+resinsight_exe_path = os.environ.get("RESINSIGHT_EXECUTABLE")
+
+# Get the TestModels path from the executable path
+resinsight_install_path = os.path.dirname(resinsight_exe_path)
+test_models_path = os.path.join(resinsight_install_path, "TestModels")
+path_name = os.path.join(
+    test_models_path, "TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+)
+case = resinsight.project.load_case(path_name)
+
+# Save the project to file
+home_dir = os.path.expanduser("~")
+project_path = home_dir + "/new-project.rsp"
+print("Saving project to: ", project_path)
+resinsight.project.save(project_path)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/selected_cases.py` & `rips-2023.6.0.2/rips/PythonExamples/selected_cases.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-############################################################################
-# This example returns the currently selected cases in ResInsight
-# Because running this script in the GUI takes away the selection
-# This script does not run successfully from within the ResInsight GUI
-# And will need to be run from the command line separately from ResInsight
-############################################################################
-
-import rips
-
-resinsight = rips.Instance.find()
-if resinsight is not None:
-    cases = resinsight.project.selected_cases()
-
-    print("Got " + str(len(cases)) + " cases: ")
-    for case in cases:
-        print(case.name)
-        for property in case.available_properties("DYNAMIC_NATIVE"):
-            print(property)
+############################################################################
+# This example returns the currently selected cases in ResInsight
+# Because running this script in the GUI takes away the selection
+# This script does not run successfully from within the ResInsight GUI
+# And will need to be run from the command line separately from ResInsight
+############################################################################
+
+import rips
+
+resinsight = rips.Instance.find()
+if resinsight is not None:
+    cases = resinsight.project.selected_cases()
+
+    print("Got " + str(len(cases)) + " cases: ")
+    for case in cases:
+        print(case.name)
+        for property in case.available_properties("DYNAMIC_NATIVE"):
+            print(property)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/selected_cells.py` & `rips-2023.6.0.2/rips/PythonExamples/selected_cells.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-############################################################################
-# This example prints center and corners for the currently selected cells
-# in ResInsight
-############################################################################
-
-import rips
-
-resinsight = rips.Instance.find()
-if resinsight is not None:
-    cases = resinsight.project.cases()
-
-    print("Got " + str(len(cases)) + " cases: ")
-    for case in cases:
-        print(case.name)
-        cells = case.selected_cells()
-        print("Found " + str(len(cells)) + " selected cells")
-
-        time_step_info = case.time_steps()
-
-        for idx, cell in enumerate(cells):
-            print(
-                "Selected cell: [{}, {}, {}] grid: {}".format(
-                    cell.ijk.i + 1, cell.ijk.j + 1, cell.ijk.k + 1, cell.grid_index
-                )
-            )
-
-            # Get the grid and dimensions
-            grid = case.grids()[cell.grid_index]
-            dimensions = grid.dimensions()
-
-            # Map ijk to cell index
-            cell_index = (
-                dimensions.i * dimensions.j * cell.ijk.k
-                + dimensions.i * cell.ijk.j
-                + cell.ijk.i
-            )
-
-            # Print the cell center
-            cell_centers = grid.cell_centers()
-            cell_center = cell_centers[cell_index]
-            print(
-                "Cell center: [{}, {}, {}]".format(
-                    cell_center.x, cell_center.y, cell_center.z
-                )
-            )
-
-            # Print the cell corners
-            cell_corners = grid.cell_corners()[cell_index]
-            print("Cell corners:")
-            print("c0:\n" + str(cell_corners.c0))
-            print("c1:\n" + str(cell_corners.c1))
-            print("c2:\n" + str(cell_corners.c2))
-            print("c3:\n" + str(cell_corners.c3))
-            print("c4:\n" + str(cell_corners.c4))
-            print("c5:\n" + str(cell_corners.c5))
-            print("c6:\n" + str(cell_corners.c6))
-            print("c7:\n" + str(cell_corners.c7))
-
-            for tidx, timestep in enumerate(time_step_info):
-                # Read the full SOIL result for time step
-                soil_results = case.selected_cell_property(
-                    "DYNAMIC_NATIVE", "SOIL", tidx
-                )
-                print(
-                    "SOIL: {} ({}.{}.{})".format(
-                        soil_results[idx], timestep.year, timestep.month, timestep.day
-                    )
-                )
+############################################################################
+# This example prints center and corners for the currently selected cells
+# in ResInsight
+############################################################################
+
+import rips
+
+resinsight = rips.Instance.find()
+if resinsight is not None:
+    cases = resinsight.project.cases()
+
+    print("Got " + str(len(cases)) + " cases: ")
+    for case in cases:
+        print(case.name)
+        cells = case.selected_cells()
+        print("Found " + str(len(cells)) + " selected cells")
+
+        time_step_info = case.time_steps()
+
+        for idx, cell in enumerate(cells):
+            print(
+                "Selected cell: [{}, {}, {}] grid: {}".format(
+                    cell.ijk.i + 1, cell.ijk.j + 1, cell.ijk.k + 1, cell.grid_index
+                )
+            )
+
+            # Get the grid and dimensions
+            grid = case.grids()[cell.grid_index]
+            dimensions = grid.dimensions()
+
+            # Map ijk to cell index
+            cell_index = (
+                dimensions.i * dimensions.j * cell.ijk.k
+                + dimensions.i * cell.ijk.j
+                + cell.ijk.i
+            )
+
+            # Print the cell center
+            cell_centers = grid.cell_centers()
+            cell_center = cell_centers[cell_index]
+            print(
+                "Cell center: [{}, {}, {}]".format(
+                    cell_center.x, cell_center.y, cell_center.z
+                )
+            )
+
+            # Print the cell corners
+            cell_corners = grid.cell_corners()[cell_index]
+            print("Cell corners:")
+            print("c0:\n" + str(cell_corners.c0))
+            print("c1:\n" + str(cell_corners.c1))
+            print("c2:\n" + str(cell_corners.c2))
+            print("c3:\n" + str(cell_corners.c3))
+            print("c4:\n" + str(cell_corners.c4))
+            print("c5:\n" + str(cell_corners.c5))
+            print("c6:\n" + str(cell_corners.c6))
+            print("c7:\n" + str(cell_corners.c7))
+
+            for tidx, timestep in enumerate(time_step_info):
+                # Read the full SOIL result for time step
+                soil_results = case.selected_cell_property(
+                    "DYNAMIC_NATIVE", "SOIL", tidx
+                )
+                print(
+                    "SOIL: {} ({}.{}.{})".format(
+                        soil_results[idx], timestep.year, timestep.month, timestep.day
+                    )
+                )
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/set_flow_diagnostics_result.py` & `rips-2023.6.0.2/rips/PythonExamples/set_flow_diagnostics_result.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-######################################################################
-# This script applies a flow diagnostics cell result to the first view in the project
-######################################################################
-
-# Load ResInsight Processing Server Client Library
-import rips
-
-# Connect to ResInsight instance
-resinsight = rips.Instance.find()
-
-view = resinsight.project.view(view_id=1)
-# view.apply_flow_diagnostics_cell_result(result_variable='Fraction',
-#                                    selection_mode='FLOW_TR_INJ_AND_PROD')
-
-# Example of setting individual wells. Commented out because well names are case specific.
-view.apply_flow_diagnostics_cell_result(
-    result_variable="Fraction",
-    selection_mode="FLOW_TR_BY_SELECTION",
-    injectors=["C-1H", "C-2H", "F-2H"],
-    producers=["B-1AH", "B-3H", "D-1H"],
-)
+######################################################################
+# This script applies a flow diagnostics cell result to the first view in the project
+######################################################################
+
+# Load ResInsight Processing Server Client Library
+import rips
+
+# Connect to ResInsight instance
+resinsight = rips.Instance.find()
+
+view = resinsight.project.view(view_id=1)
+# view.apply_flow_diagnostics_cell_result(result_variable='Fraction',
+#                                    selection_mode='FLOW_TR_INJ_AND_PROD')
+
+# Example of setting individual wells. Commented out because well names are case specific.
+view.apply_flow_diagnostics_cell_result(
+    result_variable="Fraction",
+    selection_mode="FLOW_TR_BY_SELECTION",
+    injectors=["C-1H", "C-2H", "F-2H"],
+    producers=["B-1AH", "B-3H", "D-1H"],
+)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/set_grid_properties.py` & `rips-2023.6.0.2/rips/PythonExamples/set_grid_properties.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-######################################################################
-# This script sets values for all grid cells in the first case in the project
-# The script is intended to be used for TEST10K_FLT_LGR_NNC.EGRID
-# This grid case contains one LGR
-######################################################################
-import rips
-
-resinsight = rips.Instance.find()
-
-case = resinsight.project.case(case_id=0)
-grid = case.grid()
-grid_cell_count = grid.cell_count()
-print("total cell count : " + str(grid_cell_count))
-
-values = []
-for i in range(0, grid_cell_count):
-    values.append(i % 2 * 0.75)
-
-# Assign value to IJK grid cell at (31, 53, 21)
-grid = case.grid()
-property_data_index = grid.property_data_index_from_ijk(31, 53, 21)
-values[property_data_index] = 1.5
-
-print("Applying values to main grid")
-case.set_grid_property(values, "STATIC_NATIVE", "MY_DATA", 0)
-
-values_from_ri = case.grid_property("STATIC_NATIVE", "MY_DATA", 0)
-assert values[property_data_index] == values_from_ri[property_data_index]
-
-# Get LGR grid as grid index 1
-grid = case.grid(1)
-grid_cell_count = grid.cell_count()
-print("lgr cell count : " + str(grid_cell_count))
-
-values = []
-for i in range(0, grid_cell_count):
-    values.append(i % 3 * 0.75)
-
-print("Applying values to LGR grid")
-case.set_grid_property(values, "STATIC_NATIVE", "MY_DATA", 0, 1)
-values_from_ri = case.grid_property("STATIC_NATIVE", "MY_DATA", 0, 1)
+######################################################################
+# This script sets values for all grid cells in the first case in the project
+# The script is intended to be used for TEST10K_FLT_LGR_NNC.EGRID
+# This grid case contains one LGR
+######################################################################
+import rips
+
+resinsight = rips.Instance.find()
+
+case = resinsight.project.case(case_id=0)
+grid = case.grid()
+grid_cell_count = grid.cell_count()
+print("total cell count : " + str(grid_cell_count))
+
+values = []
+for i in range(0, grid_cell_count):
+    values.append(i % 2 * 0.75)
+
+# Assign value to IJK grid cell at (31, 53, 21)
+grid = case.grid()
+property_data_index = grid.property_data_index_from_ijk(31, 53, 21)
+values[property_data_index] = 1.5
+
+print("Applying values to main grid")
+case.set_grid_property(values, "STATIC_NATIVE", "MY_DATA", 0)
+
+values_from_ri = case.grid_property("STATIC_NATIVE", "MY_DATA", 0)
+assert values[property_data_index] == values_from_ri[property_data_index]
+
+# Get LGR grid as grid index 1
+grid = case.grid(1)
+grid_cell_count = grid.cell_count()
+print("lgr cell count : " + str(grid_cell_count))
+
+values = []
+for i in range(0, grid_cell_count):
+    values.append(i % 3 * 0.75)
+
+print("Applying values to LGR grid")
+case.set_grid_property(values, "STATIC_NATIVE", "MY_DATA", 0, 1)
+values_from_ri = case.grid_property("STATIC_NATIVE", "MY_DATA", 0, 1)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/soil_average_async.py` & `rips-2023.6.0.2/rips/PythonExamples/soil_average_async.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-###########################################################################################
-# This example will asynchronously calculate the average value for SOIL for all time steps
-###########################################################################################
-
-import rips
-import itertools
-import time
-
-resinsight = rips.Instance.find()
-
-start = time.time()
-
-# Get the case with case id 0
-case = resinsight.project.case(case_id=0)
-
-# Get a list of all time steps
-timeSteps = case.time_steps()
-
-averages = []
-for i in range(0, len(timeSteps)):
-    # Get the results from time step i asynchronously
-    # It actually returns a generator object almost immediately
-    result_chunks = case.active_cell_property_async("DYNAMIC_NATIVE", "SOIL", i)
-    mysum = 0.0
-    count = 0
-    # Loop through and append the average. each time we loop resultChunks
-    # We will trigger a read of the input data, meaning the script will start
-    # Calculating averages before the whole resultValue for this time step has been received
-    for chunk in result_chunks:
-        mysum += sum(chunk.values)
-        count += len(chunk.values)
-
-    averages.append(mysum / count)
-
-end = time.time()
-print("Time elapsed: ", end - start)
-print(averages)
+###########################################################################################
+# This example will asynchronously calculate the average value for SOIL for all time steps
+###########################################################################################
+
+import rips
+import itertools
+import time
+
+resinsight = rips.Instance.find()
+
+start = time.time()
+
+# Get the case with case id 0
+case = resinsight.project.case(case_id=0)
+
+# Get a list of all time steps
+timeSteps = case.time_steps()
+
+averages = []
+for i in range(0, len(timeSteps)):
+    # Get the results from time step i asynchronously
+    # It actually returns a generator object almost immediately
+    result_chunks = case.active_cell_property_async("DYNAMIC_NATIVE", "SOIL", i)
+    mysum = 0.0
+    count = 0
+    # Loop through and append the average. each time we loop resultChunks
+    # We will trigger a read of the input data, meaning the script will start
+    # Calculating averages before the whole resultValue for this time step has been received
+    for chunk in result_chunks:
+        mysum += sum(chunk.values)
+        count += len(chunk.values)
+
+    averages.append(mysum / count)
+
+end = time.time()
+print("Time elapsed: ", end - start)
+print(averages)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/soil_average_sync.py` & `rips-2023.6.0.2/rips/PythonExamples/soil_average_sync.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-###########################################################################################
-# This example will synchronously calculate the average value for SOIL for all time steps
-###########################################################################################
-import rips
-import itertools
-import time
-
-resinsight = rips.Instance.find()
-
-start = time.time()
-
-# Get the case with case id 0
-case = resinsight.project.case(case_id=0)
-
-# Get a list of all time steps
-time_steps = case.time_steps()
-
-averages = []
-for i in range(0, len(time_steps)):
-    # Get a list of all the results for time step i
-    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", i)
-    mysum = sum(results)
-    averages.append(mysum / len(results))
-
-end = time.time()
-print("Time elapsed: ", end - start)
-print(averages)
+###########################################################################################
+# This example will synchronously calculate the average value for SOIL for all time steps
+###########################################################################################
+import rips
+import itertools
+import time
+
+resinsight = rips.Instance.find()
+
+start = time.time()
+
+# Get the case with case id 0
+case = resinsight.project.case(case_id=0)
+
+# Get a list of all time steps
+time_steps = case.time_steps()
+
+averages = []
+for i in range(0, len(time_steps)):
+    # Get a list of all the results for time step i
+    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", i)
+    mysum = sum(results)
+    averages.append(mysum / len(results))
+
+end = time.time()
+print("Time elapsed: ", end - start)
+print(averages)
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/soil_porv_async.py` & `rips-2023.6.0.2/rips/PythonExamples/soil_porv_async.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-##############################################################################
-# This example will create a derived result for each time step asynchronously
-##############################################################################
-
-import rips
-import time
-
-
-# Internal function for creating a result from a small chunk of soil and porv results
-# The return value of the function is a generator for the results rather than the result itself.
-def create_result(soil_chunks, porv_chunks):
-    for soil_chunk, porv_chunk in zip(soil_chunks, porv_chunks):
-        resultChunk = []
-        number = 0
-        for soil_value, porv_value in zip(soil_chunk.values, porv_chunk.values):
-            resultChunk.append(soil_value * porv_value)
-        # Return a Python generator
-        yield resultChunk
-
-
-resinsight = rips.Instance.find()
-start = time.time()
-case = resinsight.project.cases()[0]
-timeStepInfo = case.time_steps()
-
-# Get a generator for the porv results. The generator will provide a chunk each time it is iterated
-porv_chunks = case.active_cell_property_async("STATIC_NATIVE", "PORV", 0)
-
-# Read the static result into an array, so we don't have to transfer it for each iteration
-# Note we use the async method even if we synchronise here, because we need the values chunked
-# ... to match the soil chunks
-porv_array = []
-for porv_chunk in porv_chunks:
-    porv_array.append(porv_chunk)
-
-for i in range(0, len(timeStepInfo)):
-    # Get a generator object for the SOIL property for time step i
-    soil_chunks = case.active_cell_property_async("DYNAMIC_NATIVE", "SOIL", i)
-    # Create the generator object for the SOIL * PORV derived result
-    result_generator = create_result(soil_chunks, iter(porv_array))
-    # Send back the result asynchronously with a generator object
-    case.set_active_cell_property_async(
-        result_generator, "GENERATED", "SOILPORVAsync", i
-    )
-
-end = time.time()
-print("Time elapsed: ", end - start)
-
-print("Transferred all results back")
-
-view = case.views()[0].apply_cell_result("GENERATED", "SOILPORVAsync")
+##############################################################################
+# This example will create a derived result for each time step asynchronously
+##############################################################################
+
+import rips
+import time
+
+
+# Internal function for creating a result from a small chunk of soil and porv results
+# The return value of the function is a generator for the results rather than the result itself.
+def create_result(soil_chunks, porv_chunks):
+    for soil_chunk, porv_chunk in zip(soil_chunks, porv_chunks):
+        resultChunk = []
+        number = 0
+        for soil_value, porv_value in zip(soil_chunk.values, porv_chunk.values):
+            resultChunk.append(soil_value * porv_value)
+        # Return a Python generator
+        yield resultChunk
+
+
+resinsight = rips.Instance.find()
+start = time.time()
+case = resinsight.project.cases()[0]
+timeStepInfo = case.time_steps()
+
+# Get a generator for the porv results. The generator will provide a chunk each time it is iterated
+porv_chunks = case.active_cell_property_async("STATIC_NATIVE", "PORV", 0)
+
+# Read the static result into an array, so we don't have to transfer it for each iteration
+# Note we use the async method even if we synchronise here, because we need the values chunked
+# ... to match the soil chunks
+porv_array = []
+for porv_chunk in porv_chunks:
+    porv_array.append(porv_chunk)
+
+for i in range(0, len(timeStepInfo)):
+    # Get a generator object for the SOIL property for time step i
+    soil_chunks = case.active_cell_property_async("DYNAMIC_NATIVE", "SOIL", i)
+    # Create the generator object for the SOIL * PORV derived result
+    result_generator = create_result(soil_chunks, iter(porv_array))
+    # Send back the result asynchronously with a generator object
+    case.set_active_cell_property_async(
+        result_generator, "GENERATED", "SOILPORVAsync", i
+    )
+
+end = time.time()
+print("Time elapsed: ", end - start)
+
+print("Transferred all results back")
+
+view = case.views()[0].apply_cell_result("GENERATED", "SOILPORVAsync")
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/soil_porv_sync.py` & `rips-2023.6.0.2/rips/PythonExamples/soil_porv_sync.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-##############################################################################
-# This example will create a derived result for each time step synchronously
-##############################################################################
-
-import rips
-import time
-
-resinsight = rips.Instance.find()
-start = time.time()
-case = resinsight.project.cases()[0]
-
-# Read the full porv result
-porv_results = case.active_cell_property("STATIC_NATIVE", "PORV", 0)
-time_step_info = case.time_steps()
-
-for i in range(0, len(time_step_info)):
-    # Read the full SOIl result for time step i
-    soil_results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", i)
-
-    # Generate the result by looping through both lists in order
-    results = []
-    for soil, porv in zip(soil_results, porv_results):
-        results.append(soil * porv)
-
-    # Send back result
-    case.set_active_cell_property(results, "GENERATED", "SOILPORVSync", i)
-
-end = time.time()
-print("Time elapsed: ", end - start)
-
-print("Transferred all results back")
-
-view = case.views()[0].apply_cell_result("GENERATED", "SOILPORVSync")
+##############################################################################
+# This example will create a derived result for each time step synchronously
+##############################################################################
+
+import rips
+import time
+
+resinsight = rips.Instance.find()
+start = time.time()
+case = resinsight.project.cases()[0]
+
+# Read the full porv result
+porv_results = case.active_cell_property("STATIC_NATIVE", "PORV", 0)
+time_step_info = case.time_steps()
+
+for i in range(0, len(time_step_info)):
+    # Read the full SOIl result for time step i
+    soil_results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", i)
+
+    # Generate the result by looping through both lists in order
+    results = []
+    for soil, porv in zip(soil_results, porv_results):
+        results.append(soil * porv)
+
+    # Send back result
+    case.set_active_cell_property(results, "GENERATED", "SOILPORVSync", i)
+
+end = time.time()
+print("Time elapsed: ", end - start)
+
+print("Transferred all results back")
+
+view = case.views()[0].apply_cell_result("GENERATED", "SOILPORVSync")
```

### Comparing `rips-2023.6.0.1/rips/PythonExamples/summary_vectors.py` & `rips-2023.6.0.2/rips/PythonExamples/summary_vectors.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import rips
-import time
-
-resinsight = rips.Instance.find()
-
-project = resinsight.project
-
-# Use the following commented lines to import a file from disk
-# filename = "path/to/file/1_R001_REEK-0.SMSPEC"
-# summary_case = project.import_summary_case(filename)
-
-# Assumes at least one summery case loaded with case_id 1
-summary_case = project.summary_case(1)
-if summary_case is None:
-    print("No summary case found")
-    exit()
-
-vector_name = "FOPT"
-summary_data = summary_case.summary_vector_values(vector_name)
-
-print("Data for summary vector " + vector_name)
-print(summary_data.values)
-
-time_steps = summary_case.available_time_steps()
-print(time_steps.values)
-
-summary_data_sampled = summary_case.resample_values("FOPT", "QUARTER")
-print("\nResampled data")
-
-for t, value in zip(summary_data_sampled.time_steps, summary_data_sampled.values):
-    print(time.strftime("%a, %d %b %Y ", time.gmtime(t)) + " | " + str(value))
-
-test_values = summary_data.values
-offset = test_values[len(test_values) - 1] / 10
-
-for index, item in enumerate(test_values):
-    test_values[index] = test_values[index] + offset
-
-summary_case.set_summary_values("FOPT_M1", "myUnit", test_values)
-
-for index, item in enumerate(test_values):
-    test_values[index] = test_values[index] + offset
-summary_case.set_summary_values("FOPT_M2", "myUnit", test_values)
-
-for index, item in enumerate(test_values):
-    test_values[index] = test_values[index] + offset
-summary_case.set_summary_values("FOPT_M3", "myUnit", test_values)
-
-for index, item in enumerate(test_values):
-    test_values[index] = test_values[index] + offset
-summary_case.set_summary_values("FOPT_M4", "myUnit", test_values)
+import rips
+import time
+
+resinsight = rips.Instance.find()
+
+project = resinsight.project
+
+# Use the following commented lines to import a file from disk
+# filename = "path/to/file/1_R001_REEK-0.SMSPEC"
+# summary_case = project.import_summary_case(filename)
+
+# Assumes at least one summery case loaded with case_id 1
+summary_case = project.summary_case(1)
+if summary_case is None:
+    print("No summary case found")
+    exit()
+
+vector_name = "FOPT"
+summary_data = summary_case.summary_vector_values(vector_name)
+
+print("Data for summary vector " + vector_name)
+print(summary_data.values)
+
+time_steps = summary_case.available_time_steps()
+print(time_steps.values)
+
+summary_data_sampled = summary_case.resample_values("FOPT", "QUARTER")
+print("\nResampled data")
+
+for t, value in zip(summary_data_sampled.time_steps, summary_data_sampled.values):
+    print(time.strftime("%a, %d %b %Y ", time.gmtime(t)) + " | " + str(value))
+
+test_values = summary_data.values
+offset = test_values[len(test_values) - 1] / 10
+
+for index, item in enumerate(test_values):
+    test_values[index] = test_values[index] + offset
+
+summary_case.set_summary_values("FOPT_M1", "myUnit", test_values)
+
+for index, item in enumerate(test_values):
+    test_values[index] = test_values[index] + offset
+summary_case.set_summary_values("FOPT_M2", "myUnit", test_values)
+
+for index, item in enumerate(test_values):
+    test_values[index] = test_values[index] + offset
+summary_case.set_summary_values("FOPT_M3", "myUnit", test_values)
+
+for index, item in enumerate(test_values):
+    test_values[index] = test_values[index] + offset
+summary_case.set_summary_values("FOPT_M4", "myUnit", test_values)
```

### Comparing `rips-2023.6.0.1/rips/__init__.py` & `rips-2023.6.0.2/rips/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-name = "rips"
-
-import os
-import sys
-
-sys.path.insert(0, os.path.join(os.path.dirname(__file__), "generated"))
-
-from .resinsight_classes import *
-
-from .case import Case, EclipseCase, GeoMechCase
-from .grid import Grid
-from .instance import Instance
-from .view import View
-from .project import Project
-from .plot import Plot, PlotWindow
-from .contour_map import EclipseContourMap, GeoMechContourMap
-from .well_log_plot import WellLogPlot
-from .simulation_well import SimulationWell
-
-__all__ = []
-for key in class_dict():
-    __all__.append(key)
-
-# Add classes not in resinsight_classes
-__all__.append("Grid")
-__all__.append("Instance")
-
-__all__.sort()
+name = "rips"
+
+import os
+import sys
+
+sys.path.insert(0, os.path.join(os.path.dirname(__file__), "generated"))
+
+from .resinsight_classes import *
+
+from .case import Case, EclipseCase, GeoMechCase
+from .grid import Grid
+from .instance import Instance
+from .view import View
+from .project import Project
+from .plot import Plot, PlotWindow
+from .contour_map import EclipseContourMap, GeoMechContourMap
+from .well_log_plot import WellLogPlot
+from .simulation_well import SimulationWell
+
+__all__ = []
+for key in class_dict():
+    __all__.append(key)
+
+# Add classes not in resinsight_classes
+__all__.append("Grid")
+__all__.append("Instance")
+
+__all__.sort()
```

### Comparing `rips-2023.6.0.1/rips/case.py` & `rips-2023.6.0.2/rips/case.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1310 +1,1310 @@
-# pylint: disable=no-member
-# pylint: disable=too-many-arguments
-# pylint: disable=too-many-public-methods
-# pylint: disable=no-self-use
-
-"""
-Module containing the Case class
-
-ResInsight Case class
-
-Operate on a ResInsight case specified by a Case Id integer.
-Not meant to be constructed separately but created by one of the following
-methods in Project: loadCase, case, allCases, selectedCases
-
-.. _result-definition-label:
-
-Result Definition
------------------
-When working with grid case results, the following two arguments are used in many functions to identify a
-result
-
-**Result Definition enums**::
-    
-    property_type           |       | porosity_model
-    (str enum)              |       | (str enum)
-    ----------------------- | ----- | --------------
-    DYNAMIC_NATIVE          |       | MATRIX_MODEL
-    STATIC_NATIVE           |       | FRACTURE_MODEL
-    SOURSIMRL               |       |
-    GENERATED               |       |
-    INPUT_PROPERTY          |       |
-    FORMATION_NAMES         |       |
-    FLOW_DIAGNOSTICS        |       |
-    INJECTION_FLOODING      |       |
-
-"""
-
-import builtins
-import grpc
-
-import Case_pb2
-import Case_pb2_grpc
-import Commands_pb2 as Cmd
-import PdmObject_pb2 as PdmObject_pb2
-
-import Properties_pb2
-import Properties_pb2_grpc
-import NNCProperties_pb2
-import NNCProperties_pb2_grpc
-from .resinsight_classes import (
-    Case,
-    EclipseCase,
-    GeoMechCase,
-    WellBoreStabilityPlot,
-    WbsParameters,
-)
-
-from .grid import Grid
-from .pdmobject import add_method
-from .view import View
-from .simulation_well import SimulationWell
-import rips.project  # full name import due to circular dependency
-
-
-@add_method(Case)
-def __custom_init__(self, pb2_object, channel):
-    self.__case_stub = Case_pb2_grpc.CaseStub(self._channel)
-
-    self.__properties_stub = Properties_pb2_grpc.PropertiesStub(self._channel)
-    self.__nnc_properties_stub = NNCProperties_pb2_grpc.NNCPropertiesStub(self._channel)
-
-    # Public properties
-    self.chunk_size = 8160
-
-
-@add_method(Case)
-def __grid_count(self):
-    """Get number of grids in the case"""
-    try:
-        return self.__case_stub.GetGridCount(self.__request()).count
-    except grpc.RpcError as exception:
-        if exception.code() == grpc.StatusCode.NOT_FOUND:
-            return 0
-        return 0
-
-
-@add_method(Case)
-def __request(self):
-    return Case_pb2.CaseRequest(id=self.id)
-
-
-@add_method(Case)
-def __generate_property_input_iterator(self, values_iterator, parameters):
-    chunk = Properties_pb2.PropertyInputChunk()
-    chunk.params.CopyFrom(parameters)
-    yield chunk
-
-    for values in values_iterator:
-        valmsg = Properties_pb2.PropertyChunk(values=values)
-        chunk.values.CopyFrom(valmsg)
-        yield chunk
-
-
-@add_method(Case)
-def __generate_property_input_chunks(self, array, parameters):
-    index = -1
-    while index < len(array):
-        chunk = Properties_pb2.PropertyInputChunk()
-        if index == -1:
-            chunk.params.CopyFrom(parameters)
-            index += 1
-        else:
-            actual_chunk_size = min(len(array) - index + 1, self.chunk_size)
-            chunk.values.CopyFrom(
-                Properties_pb2.PropertyChunk(
-                    values=array[index : index + actual_chunk_size]
-                )
-            )
-            index += actual_chunk_size
-
-        yield chunk
-    # Final empty message to signal completion
-    chunk = Properties_pb2.PropertyInputChunk()
-    yield chunk
-
-
-@add_method(Case)
-def grid(self, index=0):
-    """Get Grid of a given index
-
-    Arguments:
-        index (int): The grid index
-
-    Returns:
-        :class:`rips.grid.Grid`
-    """
-    return Grid(index, self, self.channel())
-
-
-@add_method(Case)
-def grids(self):
-    """Get a list of all rips Grid objects in the case
-
-    Returns:
-        List of :class:`rips.grid.Grid`
-    """
-    grid_list = []
-    for i in range(0, self.__grid_count()):
-        grid_list.append(Grid(i, self, self.channel()))
-    return grid_list
-
-
-@add_method(Case)
-def replace(self, new_grid_file):
-    """Replace the current case grid with a new grid loaded from file
-
-    Arguments:
-        new_egrid_file (str): Path to EGRID file
-    """
-    project = self.ancestor(rips.project.Project)
-    self._execute_command(
-        replaceCase=Cmd.ReplaceCaseRequest(newGridFile=new_grid_file, caseId=self.id)
-    )
-    new_case = project.case(self.id)
-    self.copy_from(new_case)
-
-
-@add_method(Case)
-def cell_count(self, porosity_model="MATRIX_MODEL"):
-    """Get a cell count object containing number of active cells and total number of cells
-
-    Arguments:
-        porosity_model (str): String representing an enum.
-            must be 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
-    Returns:
-        Cell Count object with the following integer attributes:
-            active_cell_count: number of active cells
-            reservoir_cell_count: total number of reservoir cells
-
-    **CellCount class description**::
-
-        Parameter               | Description               | Type
-        ----------------------- | ------------------------- | -----
-        active_cell_count       | Number of active cells    | Integer
-        reservoir_cell_count    | Total number of cells     | Integer
-
-    """
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Case_pb2.CellInfoRequest(
-        case_request=self.__request(), porosity_model=porosity_model_enum
-    )
-    return self.__case_stub.GetCellCount(request)
-
-
-@add_method(Case)
-def cell_info_for_active_cells_async(self, porosity_model="MATRIX_MODEL"):
-    """Get Stream of cell info objects for current case
-
-    Arguments:
-        porosity_model(str): String representing an enum.
-            must be 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
-
-    Returns:
-        Stream of **CellInfo** objects
-
-    See :meth:`rips.case.cell_info_for_active_cells()` for detalis on the **CellInfo** class.
-    """
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Case_pb2.CellInfoRequest(
-        case_request=self.__request(), porosity_model=porosity_model_enum
-    )
-    return self.__case_stub.GetCellInfoForActiveCells(request)
-
-
-@add_method(Case)
-def cell_info_for_active_cells(self, porosity_model="MATRIX_MODEL"):
-    """Get list of cell info objects for current case
-
-    Arguments:
-        porosity_model(str): String representing an enum.
-            must be 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
-
-    Returns:
-        List of **CellInfo** objects
-
-    **CellInfo class description**::
-
-        Parameter                 | Description                                   | Type
-        ------------------------- | --------------------------------------------- | -----
-        grid_index                | Index to grid                                 | Integer
-        parent_grid_index         | Index to parent grid                          | Integer
-        coarsening_box_index      | Index to coarsening box                       | Integer
-        local_ijk                 | Cell index in IJK directions of local grid    | Vec3i
-        parent_ijk                | Cell index in IJK directions of parent grid   | Vec3i
-
-    **Vec3i class description**::
-
-        Parameter        | Description                                  | Type
-        ---------------- | -------------------------------------------- | -----
-        i                | I grid index                                 | Integer
-        j                | J grid index                                 | Integer
-        k                | K grid index                                 | Integer
-
-    """
-    active_cell_info_chunks = self.cell_info_for_active_cells_async(
-        porosity_model=porosity_model
-    )
-    received_active_cells = []
-    for active_cell_chunk in active_cell_info_chunks:
-        for active_cell in active_cell_chunk.data:
-            received_active_cells.append(active_cell)
-    return received_active_cells
-
-
-@add_method(Case)
-def time_steps(self):
-    """Get a list containing all time steps
-
-    The time steps are defined by the class **TimeStepDate**
-
-    **TimeStepDate class description**::
-
-        Type      | Name
-        --------- | ----------
-        int       | year
-        int       | month
-        int       | day
-        int       | hour
-        int       | minute
-        int       | second
-
-
-    """
-    return self.__case_stub.GetTimeSteps(self.__request()).dates
-
-
-@add_method(Case)
-def reservoir_boundingbox(self):
-    """Get the reservoir bounding box
-
-    Returns:
-        BoundingBox
-
-    **BoundingBox class description**::
-
-        Type      | Name
-        --------- | ----------
-        int       | min_x
-        int       | max_x
-        int       | min_y
-        int       | max_y
-        int       | min_z
-        int       | max_z
-
-
-    """
-    return self.__case_stub.GetReservoirBoundingBox(self.__request())
-
-
-@add_method(Case)
-def reservoir_depth_range(self):
-    """Get the reservoir depth range
-
-    Returns:
-        A tuple with two members. The first is the minimum depth, the second is the maximum depth
-    """
-    bbox = self.reservoir_boundingbox()
-    return -bbox.max_z, -bbox.min_z
-
-
-@add_method(Case)
-def days_since_start(self):
-    """Get a list of decimal values representing days since the start of the simulation"""
-    return self.__case_stub.GetDaysSinceStart(self.__request()).day_decimals
-
-
-@add_method(Case)
-def view(self, view_id):
-    """Get a particular view belonging to a case by providing view id
-
-    Arguments:
-        view_id(int): view id
-
-    Returns:
-        :class:`rips.generated.generated_classes.View`
-    """
-    views = self.views()
-    for view_object in views:
-        if view_object.id == view_id:
-            return view_object
-    return None
-
-
-@add_method(Case)
-def create_view(self):
-    """Create a new view in the current case
-
-    Returns:
-        :class:`rips.generated.generated_classes.View`
-    """
-    return self.view(
-        self._execute_command(
-            createView=Cmd.CreateViewRequest(caseId=self.id)
-        ).createViewResult.viewId
-    )
-
-
-@add_method(Case)
-def export_snapshots_of_all_views(self, prefix="", export_folder=""):
-    """Export snapshots for all views in the case
-
-    Arguments:
-        prefix (str): Exported file name prefix
-        export_folder(str): The path to export to. By default will use the global export folder
-
-    """
-    return self._execute_command(
-        exportSnapshots=Cmd.ExportSnapshotsRequest(
-            type="VIEWS",
-            prefix=prefix,
-            caseId=self.id,
-            viewId=-1,
-            exportFolder=export_folder,
-        )
-    )
-
-
-@add_method(Case)
-def export_well_path_completions(
-    self,
-    time_step,
-    well_path_names,
-    file_split,
-    compdat_export="TRANSMISSIBILITIES",
-    include_perforations=True,
-    include_fishbones=True,
-    fishbones_exclude_main_bore=True,
-    combination_mode="INDIVIDUALLY",
-    export_welspec=True,
-    export_comments=True,
-    custom_file_name="",
-):
-    """
-    Export well path completions for the current case to file
-
-    **Parameters**::
-
-        Parameter                   | Description                                      | Type
-        ----------------------------| ------------------------------------------------ | -----
-        time_step                   | Time step to export for                          | Integer
-        well_path_names             | List of well path names                          | List
-        file_split                  | Controls how export data is split into files     | String enum
-        compdat_export              | Compdat export type                              | String enum
-        include_perforations        | Export perforations?                             | bool
-        include_fishbones           | Export fishbones?                                | bool
-        fishbones_exclude_main_bore | Exclude main bore when exporting fishbones?      | bool
-        combination_mode            | Settings for multiple completions in same cell   | String Enum
-        export_welspec              | Export WELSPEC keyword                           | bool
-        export_comments             | Export completion data source as comment         | bool
-        custom_file_name            | Custom filename when file_split is "UNIFIED_FILE"| String
-
-    **Enum file_split**::
-
-        Option                              | Description
-        ----------------------------------- | ------------
-        "UNIFIED_FILE"                      | A single file with all combined transmissibilities
-        "SPLIT_ON_WELL"                     | One file for each well with combined transmissibilities
-        "SPLIT_ON_WELL_AND_COMPLETION_TYPE" | One file for each completion type for each well
-
-    **Enum compdat_export**::
-
-        Option                                      | Description
-        ------------------------------------------- | ------------
-        "TRANSMISSIBILITIES"                        | Direct export of transmissibilities
-        "WPIMULT_AND_DEFAULT_CONNECTION_FACTORS"    | Include WPIMULT in addition to transmissibilities
-
-    **Enum combination_mode**::
-
-        Option              | Description
-        ------------------- | ------------
-        "INDIVIDUALLY"      | Exports the different completion types into separate sections
-        "COMBINED"          | Export one combined transmissibility for each cell
-
-    """
-    if isinstance(well_path_names, str):
-        well_path_names = [well_path_names]
-    return self._execute_command(
-        exportWellPathCompletions=Cmd.ExportWellPathCompRequest(
-            caseId=self.id,
-            timeStep=time_step,
-            wellPathNames=well_path_names,
-            fileSplit=file_split,
-            compdatExport=compdat_export,
-            includePerforations=include_perforations,
-            includeFishbones=include_fishbones,
-            excludeMainBoreForFishbones=fishbones_exclude_main_bore,
-            combinationMode=combination_mode,
-            exportWelspec=export_welspec,
-            exportComments=export_comments,
-            customFileName=custom_file_name,
-        )
-    )
-
-
-@add_method(Case)
-def export_msw(self, well_path):
-    """
-    Export Eclipse Multi-segment-well model to file
-
-    Arguments:
-        well_path(str): Well path name
-    """
-    return self._execute_command(
-        exportMsw=Cmd.ExportMswRequest(caseId=self.id, wellPath=well_path)
-    )
-
-
-@add_method(Case)
-def create_multiple_fractures(
-    self,
-    template_id,
-    well_path_names,
-    min_dist_from_well_td,
-    max_fractures_per_well,
-    top_layer,
-    base_layer,
-    spacing,
-    action,
-):
-    """
-    Create Multiple Fractures in one go
-
-    **Parameters**::
-
-        Parameter              | Description                               | Type
-        -----------------------| ----------------------------------------- | -----
-        template_id            | Id of the template                        | Integer
-        well_path_names        | List of well path names                   | List of Strings
-        min_dist_from_well_td  | Minimum distance from well TD             | Double
-        max_fractures_per_well | Max number of fractures per well          | Integer
-        top_layer              | Top grid k-level for fractures            | Integer
-        base_layer             | Base grid k-level for fractures           | Integer
-        spacing                | Spacing between fractures                 | Double
-        action                 | 'APPEND_FRACTURES' or 'REPLACE_FRACTURES' | String enum
-
-    """
-    if isinstance(well_path_names, str):
-        well_path_names = [well_path_names]
-    return self._execute_command(
-        createMultipleFractures=Cmd.MultipleFracRequest(
-            caseId=self.id,
-            templateId=template_id,
-            wellPathNames=well_path_names,
-            minDistFromWellTd=min_dist_from_well_td,
-            maxFracturesPerWell=max_fractures_per_well,
-            topLayer=top_layer,
-            baseLayer=base_layer,
-            spacing=spacing,
-            action=action,
-        )
-    )
-
-
-@add_method(Case)
-def create_lgr_for_completion(
-    self,
-    time_step,
-    well_path_names,
-    refinement_i,
-    refinement_j,
-    refinement_k,
-    split_type,
-):
-    """
-    Create a local grid refinement for the completions on the given well paths
-
-    **Parameters**::
-
-        Parameter       | Description                            | Type
-        --------------- | -------------------------------------- | -----
-        time_steps      | Time step index                        | Integer
-        well_path_names | List of well path names                | List of Strings
-        refinement_i    | Refinment in x-direction               | Integer
-        refinement_j    | Refinment in y-direction               | Integer
-        refinement_k    | Refinment in z-direction               | Integer
-        split_type      | Defines how to split LGRS              | String enum
-
-    **Enum split_type**::
-
-        Option                  | Description
-        ------------------------| ------------
-        "LGR_PER_CELL"          | One LGR for each completed cell
-        "LGR_PER_COMPLETION"    | One LGR for each completion (fracture, perforation, ...)
-        "LGR_PER_WELL"          | One LGR for each well
-
-    """
-    if isinstance(well_path_names, str):
-        well_path_names = [well_path_names]
-    return self._execute_command(
-        createLgrForCompletions=Cmd.CreateLgrForCompRequest(
-            caseId=self.id,
-            timeStep=time_step,
-            wellPathNames=well_path_names,
-            refinementI=refinement_i,
-            refinementJ=refinement_j,
-            refinementK=refinement_k,
-            splitType=split_type,
-        )
-    )
-
-
-@add_method(Case)
-def create_saturation_pressure_plots(self):
-    """
-    Create saturation pressure plots for the current case
-    """
-    case_ids = [self.id]
-    return self._execute_command(
-        createSaturationPressurePlots=Cmd.CreateSatPressPlotRequest(caseIds=case_ids)
-    )
-
-
-@add_method(Case)
-def export_flow_characteristics(
-    self,
-    time_steps,
-    injectors,
-    producers,
-    file_name,
-    minimum_communication=0.0,
-    aquifer_cell_threshold=0.1,
-):
-    """Export Flow Characteristics data to text file in CSV format
-
-    **Parameters**::
-
-        Parameter                 | Description                                   | Type
-        ------------------------- | --------------------------------------------- | -----
-        time_steps                | Time step indices                             | List of Integer
-        injectors                 | Injector names                                | List of Strings
-        producers                 | Producer names                                | List of Strings
-        file_name                 | Export file name                              | Integer
-        minimum_communication     | Minimum Communication, defaults to 0.0        | Integer
-        aquifer_cell_threshold    | Aquifer Cell Threshold, defaults to 0.1       | Integer
-
-    """
-    if isinstance(time_steps, int):
-        time_steps = [time_steps]
-    if isinstance(injectors, str):
-        injectors = [injectors]
-    if isinstance(producers, str):
-        producers = [producers]
-    return self._execute_command(
-        exportFlowCharacteristics=Cmd.ExportFlowInfoRequest(
-            caseId=self.id,
-            timeSteps=time_steps,
-            injectors=injectors,
-            producers=producers,
-            fileName=file_name,
-            minimumCommunication=minimum_communication,
-            aquiferCellThreshold=aquifer_cell_threshold,
-        )
-    )
-
-
-@add_method(Case)
-def available_properties(self, property_type, porosity_model="MATRIX_MODEL"):
-    """Get a list of available properties
-
-    For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type (str): string corresponding to property_type enum.
-        porosity_model(str): 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
-    """
-
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.AvailablePropertiesRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        porosity_model=porosity_model_enum,
-    )
-    return self.__properties_stub.GetAvailableProperties(request).property_names
-
-
-@add_method(Case)
-def active_cell_property_async(
-    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
-):
-    """Get a cell property for all active cells. Async, so returns an iterator. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum
-
-    Returns:
-        An iterator to a chunk object containing an array of double values
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.PropertyRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        property_name=property_name,
-        time_step=time_step,
-        porosity_model=porosity_model_enum,
-    )
-    for chunk in self.__properties_stub.GetActiveCellProperty(request):
-        yield chunk
-
-
-@add_method(Case)
-def active_cell_property(
-    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
-):
-    """Get a cell property for all active cells. Sync, so returns a list. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum
-
-    Returns:
-        A list containing double values
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    all_values = []
-    generator = self.active_cell_property_async(
-        property_type, property_name, time_step, porosity_model
-    )
-    for chunk in generator:
-        for value in chunk.values:
-            all_values.append(value)
-    return all_values
-
-
-@add_method(Case)
-def selected_cell_property_async(
-    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
-):
-    """Get a cell property for all selected cells. Async, so returns an iterator. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum
-
-    Returns:
-        An iterator to a chunk object containing an array of double values
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.PropertyRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        property_name=property_name,
-        time_step=time_step,
-        porosity_model=porosity_model_enum,
-    )
-    for chunk in self.__properties_stub.GetSelectedCellProperty(request):
-        yield chunk
-
-
-@add_method(Case)
-def selected_cell_property(
-    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
-):
-    """Get a cell property for all selected cells. Sync, so returns a list. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum
-
-    Returns:
-        A list containing double values
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    all_values = []
-    generator = self.selected_cell_property_async(
-        property_type, property_name, time_step, porosity_model
-    )
-    for chunk in generator:
-        for value in chunk.values:
-            all_values.append(value)
-    return all_values
-
-
-@add_method(Case)
-def grid_property_async(
-    self,
-    property_type,
-    property_name,
-    time_step,
-    grid_index=0,
-    porosity_model="MATRIX_MODEL",
-):
-    """Get a cell property for all grid cells. Async, so returns an iterator. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        gridIndex(int): index to the grid we're getting values for
-        porosity_model(str): string enum
-
-    Returns:
-        An iterator to a chunk object containing an array of double values
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.PropertyRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        property_name=property_name,
-        time_step=time_step,
-        grid_index=grid_index,
-        porosity_model=porosity_model_enum,
-    )
-    for chunk in self.__properties_stub.GetGridProperty(request):
-        yield chunk
-
-
-@add_method(Case)
-def grid_property(
-    self,
-    property_type,
-    property_name,
-    time_step,
-    grid_index=0,
-    porosity_model="MATRIX_MODEL",
-):
-    """Get a cell property for all grid cells. Synchronous, so returns a list. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        grid_index(int): index to the grid we're getting values for
-        porosity_model(str): string enum
-
-    Returns:
-        A list of double values
-    """
-    all_values = []
-    generator = self.grid_property_async(
-        property_type, property_name, time_step, grid_index, porosity_model
-    )
-    for chunk in generator:
-        for value in chunk.values:
-            all_values.append(value)
-    return all_values
-
-
-@add_method(Case)
-def set_active_cell_property_async(
-    self,
-    values_iterator,
-    property_type,
-    property_name,
-    time_step,
-    porosity_model="MATRIX_MODEL",
-):
-    """Set cell property for all active cells Async. Takes an iterator to the input values. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        values_iterator(iterator): an iterator to the properties to be set
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum
-    """
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.PropertyRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        property_name=property_name,
-        time_step=time_step,
-        porosity_model=porosity_model_enum,
-    )
-
-    request_iterator = self.__generate_property_input_iterator(values_iterator, request)
-    self.__properties_stub.SetActiveCellProperty(request_iterator)
-
-
-@add_method(Case)
-def set_active_cell_property(
-    self, values, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
-):
-    """Set a cell property for all active cells. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        values(list): a list of double precision floating point numbers
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum
-    """
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.PropertyRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        property_name=property_name,
-        time_step=time_step,
-        porosity_model=porosity_model_enum,
-    )
-    request_iterator = self.__generate_property_input_chunks(values, request)
-    reply = self.__properties_stub.SetActiveCellProperty(request_iterator)
-    if reply.accepted_value_count < len(values):
-        raise IndexError
-
-
-@add_method(Case)
-def set_grid_property(
-    self,
-    values,
-    property_type,
-    property_name,
-    time_step,
-    grid_index=0,
-    porosity_model="MATRIX_MODEL",
-):
-    """Set a cell property for all grid cells. For argument details, see :ref:`Result Definition <result-definition-label>`
-
-    Arguments:
-        values(list): a list of double precision floating point numbers
-        property_type(str): string enum
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        grid_index(int): index to the grid we're setting values for
-        porosity_model(str): string enum
-    """
-    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Properties_pb2.PropertyRequest(
-        case_request=self.__request(),
-        property_type=property_type_enum,
-        property_name=property_name,
-        time_step=time_step,
-        grid_index=grid_index,
-        porosity_model=porosity_model_enum,
-    )
-    request_iterator = self.__generate_property_input_chunks(values, request)
-    reply = self.__properties_stub.SetGridProperty(request_iterator)
-    if reply.accepted_value_count < len(values):
-        raise IndexError
-
-
-@add_method(Case)
-def export_property(
-    self,
-    time_step,
-    property_name,
-    eclipse_keyword=property,
-    undefined_value=0.0,
-    export_file=property,
-):
-    """Export an Eclipse property
-
-    Arguments:
-        time_step (int): time step index
-        property_name (str): property to export
-        eclipse_keyword (str): Keyword used in export header. Defaults: value of property
-        undefined_value (double): Value to use for undefined values. Defaults to 0.0
-        export_file (str): File name for export. Defaults to the value of property parameter
-    """
-    return self._execute_command(
-        exportProperty=Cmd.ExportPropertyRequest(
-            caseId=self.id,
-            timeStep=time_step,
-            property=property_name,
-            eclipseKeyword=eclipse_keyword,
-            undefinedValue=undefined_value,
-            exportFile=export_file,
-        )
-    )
-
-
-@add_method(Case)
-def create_well_bore_stability_plot(self, well_path, time_step, parameters=None):
-    """Create a new well bore stability plot
-
-    Arguments:
-        well_path(str): well path name
-        time_step(int): time step
-
-    Returns:
-        :class:`rips.generated.generated_classes.WellBoreStabilityPlot`
-    """
-    pb2_parameters = None
-    if parameters is not None:
-        assert isinstance(parameters, WbsParameters)
-        pb2_parameters = parameters.pb2_object()
-
-    plot_result = self._execute_command(
-        createWellBoreStabilityPlot=Cmd.CreateWbsPlotRequest(
-            caseId=self.id,
-            wellPath=well_path,
-            timeStep=time_step,
-            wbsParameters=pb2_parameters,
-        )
-    )
-    project = self.ancestor(rips.project.Project)
-    plot = project.plot(view_id=plot_result.createWbsPlotResult.viewId)
-    return plot
-
-
-@add_method(Case)
-def import_formation_names(self, formation_files=None):
-    """Import formation names into project and apply it to the current case
-
-    Arguments:
-        formation_files(list): list of files to import
-
-    """
-    if formation_files is None:
-        formation_files = []
-    elif isinstance(formation_files, str):
-        formation_files = [formation_files]
-
-    self._execute_command(
-        importFormationNames=Cmd.ImportFormationNamesRequest(
-            formationFiles=formation_files, applyToCaseId=self.id
-        )
-    )
-
-
-@add_method(Case)
-def simulation_wells(self):
-    """Get a list of all simulation wells for a case
-
-    Returns:
-        :class:`rips.generated.generated_classes.SimulationWell`
-
-    """
-    wells = self.descendants(SimulationWell)
-    return wells
-
-
-@add_method(Case)
-def active_cell_centers_async(self, porosity_model="MATRIX_MODEL"):
-    """Get a cell centers for all active cells. Async, so returns an iterator
-
-    Arguments:
-        porosity_model(str): string enum. See available()
-
-    Returns:
-        An iterator to a chunk object containing an array of Vec3d values.
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Case_pb2.CellInfoRequest(
-        case_request=self.__request(), porosity_model=porosity_model_enum
-    )
-    return self.__case_stub.GetCellCenterForActiveCells(request)
-
-
-@add_method(Case)
-def active_cell_centers(self, porosity_model="MATRIX_MODEL"):
-    """Get a cell centers for all active cells. Synchronous, so returns a list.
-
-    Arguments:
-        porosity_model(str): string enum. See available()
-
-    Returns:
-        A list of Vec3d
-    """
-    cell_centers = []
-    generator = self.active_cell_centers_async(porosity_model)
-    for chunk in generator:
-        for value in chunk.centers:
-            cell_centers.append(value)
-    return cell_centers
-
-
-@add_method(Case)
-def active_cell_corners_async(self, porosity_model="MATRIX_MODEL"):
-    """Get a cell corners for all active cells. Async, so returns an iterator
-
-    Arguments:
-        porosity_model(str): string enum. See available()
-
-    Returns:
-        An iterator to a chunk object containing an array of CellCorners (which is eight Vec3d values).
-        Loop through the chunks and then the values within the chunk to get all values.
-    """
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = Case_pb2.CellInfoRequest(
-        case_request=self.__request(), porosity_model=porosity_model_enum
-    )
-    return self.__case_stub.GetCellCornersForActiveCells(request)
-
-
-@add_method(Case)
-def active_cell_corners(self, porosity_model="MATRIX_MODEL"):
-    """Get a cell corners for all active cells. Synchronous, so returns a list.
-
-        Arguments:
-            porosity_model(str): string enum. See available()
-
-    **CellCorner class description**::
-
-        Parameter   | Description   | Type
-        ----------- | ------------  | -----
-        c0          |               | Vec3d
-        c1          |               | Vec3d
-        c2          |               | Vec3d
-        c3          |               | Vec3d
-        c4          |               | Vec3d
-        c5          |               | Vec3d
-        c6          |               | Vec3d
-        c7          |               | Vec3d
-
-
-    """
-    cell_corners = []
-    generator = self.active_cell_corners_async(porosity_model)
-    for chunk in generator:
-        for value in chunk.cells:
-            cell_corners.append(value)
-    return cell_corners
-
-
-@add_method(Case)
-def selected_cells_async(self):
-    """Get the selected cells. Async, so returns an iterator.
-
-    Returns:
-        An iterator to a chunk object containing an array of cells.
-        Loop through the chunks and then the cells within the chunk to get all cells.
-    """
-    return self.__case_stub.GetSelectedCells(self.__request())
-
-
-@add_method(Case)
-def selected_cells(self):
-    """Get the selected cells. Synchronous, so returns a list.
-
-    Returns:
-        A list of Cells.
-    """
-    cells = []
-    generator = self.selected_cells_async()
-    for chunk in generator:
-        for value in chunk.cells:
-            cells.append(value)
-    return cells
-
-
-@add_method(Case)
-def coarsening_info(self):
-    """Get a coarsening information for all grids in the case.
-
-    Returns:
-        A list of CoarseningInfo objects with two Vec3i min and max objects
-        for each entry.
-    """
-    return self.__case_stub.GetCoarseningInfoArray(self.__request()).data
-
-
-@add_method(Case)
-def available_nnc_properties(self):
-    """Get a list of available NNC properties
-
-    **NNCConnection class description**::
-
-          Parameter               | Description                                   | Type
-          ------------------------| --------------------------------------------- | -----
-          cell_grid_index1        | Reservoir Cell Index to cell 1                | int32
-          cell_grid_index2        | Reservoir Cell Index to cell 2                | int32
-          cell1                   | Reservoir Cell IJK to cell 1                  | Vec3i
-          cell2                   | Reservoir Cell IJK to cell 1                  | Vec3i
-
-    """
-    return self.__nnc_properties_stub.GetAvailableNNCProperties(
-        self.__request()
-    ).properties
-
-
-@add_method(Case)
-def nnc_connections_async(self):
-    """Get the NNC connections. Async, so returns an iterator.
-
-    Returns:
-        An iterator to a chunk object containing an array NNCConnection objects.
-        Loop through the chunks and then the connection within the chunk to get all connections.
-    """
-    return self.__nnc_properties_stub.GetNNCConnections(self.__request())
-
-
-@add_method(Case)
-def nnc_connections(self):
-    """Get the NNC connection. Synchronous, so returns a list.
-
-    Returns:
-        A list of NNCConnection objects.
-    """
-    connections = []
-    generator = self.nnc_connections_async()
-    for chunk in generator:
-        for value in chunk.connections:
-            connections.append(value)
-    return connections
-
-
-@add_method(Case)
-def __nnc_connections_values_async(self, property_name, property_type, time_step):
-    request = NNCProperties_pb2.NNCValuesRequest(
-        case_id=self.id,
-        property_name=property_name,
-        property_type=property_type,
-        time_step=time_step,
-    )
-    return self.__nnc_properties_stub.GetNNCValues(request)
-
-
-@add_method(Case)
-def __nnc_values_generator_to_list(self, generator):
-    """Converts a NNC values generator to a list."""
-    vals = []
-    for chunk in generator:
-        for value in chunk.values:
-            vals.append(value)
-    return vals
-
-
-@add_method(Case)
-def nnc_connections_static_values_async(self, property_name):
-    """Get the static NNC values. Async, so returns an iterator.
-
-    Returns:
-        An iterator to a chunk object containing an list of doubles.
-        Loop through the chunks and then the values within the chunk to get values
-        for all the connections. The order of the list matches the list from
-        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
-        value in this list.
-    """
-    return self.__nnc_connections_values_async(
-        property_name, NNCProperties_pb2.NNC_STATIC, 0
-    )
-
-
-@add_method(Case)
-def nnc_connections_static_values(self, property_name):
-    """Get the static NNC values.
-
-    Returns:
-        A list of doubles. The order of the list matches the list from
-        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
-        value in this list.
-    """
-    generator = self.nnc_connections_static_values_async(property_name)
-    return self.__nnc_values_generator_to_list(generator)
-
-
-@add_method(Case)
-def nnc_connections_dynamic_values_async(self, property_name, time_step):
-    """Get the dynamic NNC values. Async, so returns an iterator.
-
-    Returns:
-        An iterator to a chunk object containing an list of doubles.
-        Loop through the chunks and then the values within the chunk to get values
-        for all the connections. The order of the list matches the list from
-        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
-        value in this list.
-    """
-    return self.__nnc_connections_values_async(
-        property_name, NNCProperties_pb2.NNC_DYNAMIC, time_step
-    )
-
-
-@add_method(Case)
-def nnc_connections_dynamic_values(self, property_name, time_step):
-    """Get the dynamic NNC values.
-
-    Returns:
-        A list of doubles. The order of the list matches the list from
-        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
-        value in this list.
-    """
-    generator = self.nnc_connections_dynamic_values_async(property_name, time_step)
-    return self.__nnc_values_generator_to_list(generator)
-
-
-@add_method(Case)
-def nnc_connections_generated_values_async(self, property_name, time_step):
-    """Get the generated NNC values. Async, so returns an iterator.
-
-    Returns:
-        An iterator to a chunk object containing an list of doubles.
-        Loop through the chunks and then the values within the chunk to get values
-        for all the connections. The order of the list matches the list from
-        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
-        value in this list.
-    """
-    return self.__nnc_connections_values_async(
-        property_name, NNCProperties_pb2.NNC_GENERATED, time_step
-    )
-
-
-@add_method(Case)
-def nnc_connections_generated_values(self, property_name, time_step):
-    """Get the generated NNC values.
-
-    Returns:
-        A list of doubles. The order of the list matches the list from
-        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
-        value in this list.
-    """
-    generator = self.nnc_connections_generated_values_async(property_name, time_step)
-    return self.__nnc_values_generator_to_list(generator)
-
-
-@add_method(Case)
-def __generate_nnc_property_input_chunks(self, array, parameters):
-    index = -1
-    while index < len(array):
-        chunk = NNCProperties_pb2.NNCValuesChunk()
-        if index == -1:
-            chunk.params.CopyFrom(parameters)
-            index += 1
-        else:
-            actual_chunk_size = min(len(array) - index + 1, self.chunk_size)
-            chunk.values.CopyFrom(
-                NNCProperties_pb2.NNCValues(
-                    values=array[index : index + actual_chunk_size]
-                )
-            )
-            index += actual_chunk_size
-
-        yield chunk
-    # Final empty message to signal completion
-    chunk = NNCProperties_pb2.NNCValuesChunk()
-    yield chunk
-
-
-@add_method(Case)
-def set_nnc_connections_values(
-    self, values, property_name, time_step, porosity_model="MATRIX_MODEL"
-):
-    """Set nnc connection values for all connections..
-
-    Arguments:
-        values(list): a list of double precision floating point numbers
-        property_name(str): name of an Eclipse property
-        time_step(int): the time step for which to get the property for
-        porosity_model(str): string enum. See available()
-    """
-    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
-    request = NNCProperties_pb2.NNCValuesInputRequest(
-        case_id=self.id,
-        property_name=property_name,
-        time_step=time_step,
-        porosity_model=porosity_model_enum,
-    )
-    request_iterator = self.__generate_nnc_property_input_chunks(values, request)
-    reply = self.__nnc_properties_stub.SetNNCValues(request_iterator)
-    if reply.accepted_value_count < len(values):
-        raise IndexError
+# pylint: disable=no-member
+# pylint: disable=too-many-arguments
+# pylint: disable=too-many-public-methods
+# pylint: disable=no-self-use
+
+"""
+Module containing the Case class
+
+ResInsight Case class
+
+Operate on a ResInsight case specified by a Case Id integer.
+Not meant to be constructed separately but created by one of the following
+methods in Project: loadCase, case, allCases, selectedCases
+
+.. _result-definition-label:
+
+Result Definition
+-----------------
+When working with grid case results, the following two arguments are used in many functions to identify a
+result
+
+**Result Definition enums**::
+    
+    property_type           |       | porosity_model
+    (str enum)              |       | (str enum)
+    ----------------------- | ----- | --------------
+    DYNAMIC_NATIVE          |       | MATRIX_MODEL
+    STATIC_NATIVE           |       | FRACTURE_MODEL
+    SOURSIMRL               |       |
+    GENERATED               |       |
+    INPUT_PROPERTY          |       |
+    FORMATION_NAMES         |       |
+    FLOW_DIAGNOSTICS        |       |
+    INJECTION_FLOODING      |       |
+
+"""
+
+import builtins
+import grpc
+
+import Case_pb2
+import Case_pb2_grpc
+import Commands_pb2 as Cmd
+import PdmObject_pb2 as PdmObject_pb2
+
+import Properties_pb2
+import Properties_pb2_grpc
+import NNCProperties_pb2
+import NNCProperties_pb2_grpc
+from .resinsight_classes import (
+    Case,
+    EclipseCase,
+    GeoMechCase,
+    WellBoreStabilityPlot,
+    WbsParameters,
+)
+
+from .grid import Grid
+from .pdmobject import add_method
+from .view import View
+from .simulation_well import SimulationWell
+import rips.project  # full name import due to circular dependency
+
+
+@add_method(Case)
+def __custom_init__(self, pb2_object, channel):
+    self.__case_stub = Case_pb2_grpc.CaseStub(self._channel)
+
+    self.__properties_stub = Properties_pb2_grpc.PropertiesStub(self._channel)
+    self.__nnc_properties_stub = NNCProperties_pb2_grpc.NNCPropertiesStub(self._channel)
+
+    # Public properties
+    self.chunk_size = 8160
+
+
+@add_method(Case)
+def __grid_count(self):
+    """Get number of grids in the case"""
+    try:
+        return self.__case_stub.GetGridCount(self.__request()).count
+    except grpc.RpcError as exception:
+        if exception.code() == grpc.StatusCode.NOT_FOUND:
+            return 0
+        return 0
+
+
+@add_method(Case)
+def __request(self):
+    return Case_pb2.CaseRequest(id=self.id)
+
+
+@add_method(Case)
+def __generate_property_input_iterator(self, values_iterator, parameters):
+    chunk = Properties_pb2.PropertyInputChunk()
+    chunk.params.CopyFrom(parameters)
+    yield chunk
+
+    for values in values_iterator:
+        valmsg = Properties_pb2.PropertyChunk(values=values)
+        chunk.values.CopyFrom(valmsg)
+        yield chunk
+
+
+@add_method(Case)
+def __generate_property_input_chunks(self, array, parameters):
+    index = -1
+    while index < len(array):
+        chunk = Properties_pb2.PropertyInputChunk()
+        if index == -1:
+            chunk.params.CopyFrom(parameters)
+            index += 1
+        else:
+            actual_chunk_size = min(len(array) - index + 1, self.chunk_size)
+            chunk.values.CopyFrom(
+                Properties_pb2.PropertyChunk(
+                    values=array[index : index + actual_chunk_size]
+                )
+            )
+            index += actual_chunk_size
+
+        yield chunk
+    # Final empty message to signal completion
+    chunk = Properties_pb2.PropertyInputChunk()
+    yield chunk
+
+
+@add_method(Case)
+def grid(self, index=0):
+    """Get Grid of a given index
+
+    Arguments:
+        index (int): The grid index
+
+    Returns:
+        :class:`rips.grid.Grid`
+    """
+    return Grid(index, self, self.channel())
+
+
+@add_method(Case)
+def grids(self):
+    """Get a list of all rips Grid objects in the case
+
+    Returns:
+        List of :class:`rips.grid.Grid`
+    """
+    grid_list = []
+    for i in range(0, self.__grid_count()):
+        grid_list.append(Grid(i, self, self.channel()))
+    return grid_list
+
+
+@add_method(Case)
+def replace(self, new_grid_file):
+    """Replace the current case grid with a new grid loaded from file
+
+    Arguments:
+        new_egrid_file (str): Path to EGRID file
+    """
+    project = self.ancestor(rips.project.Project)
+    self._execute_command(
+        replaceCase=Cmd.ReplaceCaseRequest(newGridFile=new_grid_file, caseId=self.id)
+    )
+    new_case = project.case(self.id)
+    self.copy_from(new_case)
+
+
+@add_method(Case)
+def cell_count(self, porosity_model="MATRIX_MODEL"):
+    """Get a cell count object containing number of active cells and total number of cells
+
+    Arguments:
+        porosity_model (str): String representing an enum.
+            must be 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
+    Returns:
+        Cell Count object with the following integer attributes:
+            active_cell_count: number of active cells
+            reservoir_cell_count: total number of reservoir cells
+
+    **CellCount class description**::
+
+        Parameter               | Description               | Type
+        ----------------------- | ------------------------- | -----
+        active_cell_count       | Number of active cells    | Integer
+        reservoir_cell_count    | Total number of cells     | Integer
+
+    """
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Case_pb2.CellInfoRequest(
+        case_request=self.__request(), porosity_model=porosity_model_enum
+    )
+    return self.__case_stub.GetCellCount(request)
+
+
+@add_method(Case)
+def cell_info_for_active_cells_async(self, porosity_model="MATRIX_MODEL"):
+    """Get Stream of cell info objects for current case
+
+    Arguments:
+        porosity_model(str): String representing an enum.
+            must be 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
+
+    Returns:
+        Stream of **CellInfo** objects
+
+    See :meth:`rips.case.cell_info_for_active_cells()` for detalis on the **CellInfo** class.
+    """
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Case_pb2.CellInfoRequest(
+        case_request=self.__request(), porosity_model=porosity_model_enum
+    )
+    return self.__case_stub.GetCellInfoForActiveCells(request)
+
+
+@add_method(Case)
+def cell_info_for_active_cells(self, porosity_model="MATRIX_MODEL"):
+    """Get list of cell info objects for current case
+
+    Arguments:
+        porosity_model(str): String representing an enum.
+            must be 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
+
+    Returns:
+        List of **CellInfo** objects
+
+    **CellInfo class description**::
+
+        Parameter                 | Description                                   | Type
+        ------------------------- | --------------------------------------------- | -----
+        grid_index                | Index to grid                                 | Integer
+        parent_grid_index         | Index to parent grid                          | Integer
+        coarsening_box_index      | Index to coarsening box                       | Integer
+        local_ijk                 | Cell index in IJK directions of local grid    | Vec3i
+        parent_ijk                | Cell index in IJK directions of parent grid   | Vec3i
+
+    **Vec3i class description**::
+
+        Parameter        | Description                                  | Type
+        ---------------- | -------------------------------------------- | -----
+        i                | I grid index                                 | Integer
+        j                | J grid index                                 | Integer
+        k                | K grid index                                 | Integer
+
+    """
+    active_cell_info_chunks = self.cell_info_for_active_cells_async(
+        porosity_model=porosity_model
+    )
+    received_active_cells = []
+    for active_cell_chunk in active_cell_info_chunks:
+        for active_cell in active_cell_chunk.data:
+            received_active_cells.append(active_cell)
+    return received_active_cells
+
+
+@add_method(Case)
+def time_steps(self):
+    """Get a list containing all time steps
+
+    The time steps are defined by the class **TimeStepDate**
+
+    **TimeStepDate class description**::
+
+        Type      | Name
+        --------- | ----------
+        int       | year
+        int       | month
+        int       | day
+        int       | hour
+        int       | minute
+        int       | second
+
+
+    """
+    return self.__case_stub.GetTimeSteps(self.__request()).dates
+
+
+@add_method(Case)
+def reservoir_boundingbox(self):
+    """Get the reservoir bounding box
+
+    Returns:
+        BoundingBox
+
+    **BoundingBox class description**::
+
+        Type      | Name
+        --------- | ----------
+        int       | min_x
+        int       | max_x
+        int       | min_y
+        int       | max_y
+        int       | min_z
+        int       | max_z
+
+
+    """
+    return self.__case_stub.GetReservoirBoundingBox(self.__request())
+
+
+@add_method(Case)
+def reservoir_depth_range(self):
+    """Get the reservoir depth range
+
+    Returns:
+        A tuple with two members. The first is the minimum depth, the second is the maximum depth
+    """
+    bbox = self.reservoir_boundingbox()
+    return -bbox.max_z, -bbox.min_z
+
+
+@add_method(Case)
+def days_since_start(self):
+    """Get a list of decimal values representing days since the start of the simulation"""
+    return self.__case_stub.GetDaysSinceStart(self.__request()).day_decimals
+
+
+@add_method(Case)
+def view(self, view_id):
+    """Get a particular view belonging to a case by providing view id
+
+    Arguments:
+        view_id(int): view id
+
+    Returns:
+        :class:`rips.generated.generated_classes.View`
+    """
+    views = self.views()
+    for view_object in views:
+        if view_object.id == view_id:
+            return view_object
+    return None
+
+
+@add_method(Case)
+def create_view(self):
+    """Create a new view in the current case
+
+    Returns:
+        :class:`rips.generated.generated_classes.View`
+    """
+    return self.view(
+        self._execute_command(
+            createView=Cmd.CreateViewRequest(caseId=self.id)
+        ).createViewResult.viewId
+    )
+
+
+@add_method(Case)
+def export_snapshots_of_all_views(self, prefix="", export_folder=""):
+    """Export snapshots for all views in the case
+
+    Arguments:
+        prefix (str): Exported file name prefix
+        export_folder(str): The path to export to. By default will use the global export folder
+
+    """
+    return self._execute_command(
+        exportSnapshots=Cmd.ExportSnapshotsRequest(
+            type="VIEWS",
+            prefix=prefix,
+            caseId=self.id,
+            viewId=-1,
+            exportFolder=export_folder,
+        )
+    )
+
+
+@add_method(Case)
+def export_well_path_completions(
+    self,
+    time_step,
+    well_path_names,
+    file_split,
+    compdat_export="TRANSMISSIBILITIES",
+    include_perforations=True,
+    include_fishbones=True,
+    fishbones_exclude_main_bore=True,
+    combination_mode="INDIVIDUALLY",
+    export_welspec=True,
+    export_comments=True,
+    custom_file_name="",
+):
+    """
+    Export well path completions for the current case to file
+
+    **Parameters**::
+
+        Parameter                   | Description                                      | Type
+        ----------------------------| ------------------------------------------------ | -----
+        time_step                   | Time step to export for                          | Integer
+        well_path_names             | List of well path names                          | List
+        file_split                  | Controls how export data is split into files     | String enum
+        compdat_export              | Compdat export type                              | String enum
+        include_perforations        | Export perforations?                             | bool
+        include_fishbones           | Export fishbones?                                | bool
+        fishbones_exclude_main_bore | Exclude main bore when exporting fishbones?      | bool
+        combination_mode            | Settings for multiple completions in same cell   | String Enum
+        export_welspec              | Export WELSPEC keyword                           | bool
+        export_comments             | Export completion data source as comment         | bool
+        custom_file_name            | Custom filename when file_split is "UNIFIED_FILE"| String
+
+    **Enum file_split**::
+
+        Option                              | Description
+        ----------------------------------- | ------------
+        "UNIFIED_FILE"                      | A single file with all combined transmissibilities
+        "SPLIT_ON_WELL"                     | One file for each well with combined transmissibilities
+        "SPLIT_ON_WELL_AND_COMPLETION_TYPE" | One file for each completion type for each well
+
+    **Enum compdat_export**::
+
+        Option                                      | Description
+        ------------------------------------------- | ------------
+        "TRANSMISSIBILITIES"                        | Direct export of transmissibilities
+        "WPIMULT_AND_DEFAULT_CONNECTION_FACTORS"    | Include WPIMULT in addition to transmissibilities
+
+    **Enum combination_mode**::
+
+        Option              | Description
+        ------------------- | ------------
+        "INDIVIDUALLY"      | Exports the different completion types into separate sections
+        "COMBINED"          | Export one combined transmissibility for each cell
+
+    """
+    if isinstance(well_path_names, str):
+        well_path_names = [well_path_names]
+    return self._execute_command(
+        exportWellPathCompletions=Cmd.ExportWellPathCompRequest(
+            caseId=self.id,
+            timeStep=time_step,
+            wellPathNames=well_path_names,
+            fileSplit=file_split,
+            compdatExport=compdat_export,
+            includePerforations=include_perforations,
+            includeFishbones=include_fishbones,
+            excludeMainBoreForFishbones=fishbones_exclude_main_bore,
+            combinationMode=combination_mode,
+            exportWelspec=export_welspec,
+            exportComments=export_comments,
+            customFileName=custom_file_name,
+        )
+    )
+
+
+@add_method(Case)
+def export_msw(self, well_path):
+    """
+    Export Eclipse Multi-segment-well model to file
+
+    Arguments:
+        well_path(str): Well path name
+    """
+    return self._execute_command(
+        exportMsw=Cmd.ExportMswRequest(caseId=self.id, wellPath=well_path)
+    )
+
+
+@add_method(Case)
+def create_multiple_fractures(
+    self,
+    template_id,
+    well_path_names,
+    min_dist_from_well_td,
+    max_fractures_per_well,
+    top_layer,
+    base_layer,
+    spacing,
+    action,
+):
+    """
+    Create Multiple Fractures in one go
+
+    **Parameters**::
+
+        Parameter              | Description                               | Type
+        -----------------------| ----------------------------------------- | -----
+        template_id            | Id of the template                        | Integer
+        well_path_names        | List of well path names                   | List of Strings
+        min_dist_from_well_td  | Minimum distance from well TD             | Double
+        max_fractures_per_well | Max number of fractures per well          | Integer
+        top_layer              | Top grid k-level for fractures            | Integer
+        base_layer             | Base grid k-level for fractures           | Integer
+        spacing                | Spacing between fractures                 | Double
+        action                 | 'APPEND_FRACTURES' or 'REPLACE_FRACTURES' | String enum
+
+    """
+    if isinstance(well_path_names, str):
+        well_path_names = [well_path_names]
+    return self._execute_command(
+        createMultipleFractures=Cmd.MultipleFracRequest(
+            caseId=self.id,
+            templateId=template_id,
+            wellPathNames=well_path_names,
+            minDistFromWellTd=min_dist_from_well_td,
+            maxFracturesPerWell=max_fractures_per_well,
+            topLayer=top_layer,
+            baseLayer=base_layer,
+            spacing=spacing,
+            action=action,
+        )
+    )
+
+
+@add_method(Case)
+def create_lgr_for_completion(
+    self,
+    time_step,
+    well_path_names,
+    refinement_i,
+    refinement_j,
+    refinement_k,
+    split_type,
+):
+    """
+    Create a local grid refinement for the completions on the given well paths
+
+    **Parameters**::
+
+        Parameter       | Description                            | Type
+        --------------- | -------------------------------------- | -----
+        time_steps      | Time step index                        | Integer
+        well_path_names | List of well path names                | List of Strings
+        refinement_i    | Refinment in x-direction               | Integer
+        refinement_j    | Refinment in y-direction               | Integer
+        refinement_k    | Refinment in z-direction               | Integer
+        split_type      | Defines how to split LGRS              | String enum
+
+    **Enum split_type**::
+
+        Option                  | Description
+        ------------------------| ------------
+        "LGR_PER_CELL"          | One LGR for each completed cell
+        "LGR_PER_COMPLETION"    | One LGR for each completion (fracture, perforation, ...)
+        "LGR_PER_WELL"          | One LGR for each well
+
+    """
+    if isinstance(well_path_names, str):
+        well_path_names = [well_path_names]
+    return self._execute_command(
+        createLgrForCompletions=Cmd.CreateLgrForCompRequest(
+            caseId=self.id,
+            timeStep=time_step,
+            wellPathNames=well_path_names,
+            refinementI=refinement_i,
+            refinementJ=refinement_j,
+            refinementK=refinement_k,
+            splitType=split_type,
+        )
+    )
+
+
+@add_method(Case)
+def create_saturation_pressure_plots(self):
+    """
+    Create saturation pressure plots for the current case
+    """
+    case_ids = [self.id]
+    return self._execute_command(
+        createSaturationPressurePlots=Cmd.CreateSatPressPlotRequest(caseIds=case_ids)
+    )
+
+
+@add_method(Case)
+def export_flow_characteristics(
+    self,
+    time_steps,
+    injectors,
+    producers,
+    file_name,
+    minimum_communication=0.0,
+    aquifer_cell_threshold=0.1,
+):
+    """Export Flow Characteristics data to text file in CSV format
+
+    **Parameters**::
+
+        Parameter                 | Description                                   | Type
+        ------------------------- | --------------------------------------------- | -----
+        time_steps                | Time step indices                             | List of Integer
+        injectors                 | Injector names                                | List of Strings
+        producers                 | Producer names                                | List of Strings
+        file_name                 | Export file name                              | Integer
+        minimum_communication     | Minimum Communication, defaults to 0.0        | Integer
+        aquifer_cell_threshold    | Aquifer Cell Threshold, defaults to 0.1       | Integer
+
+    """
+    if isinstance(time_steps, int):
+        time_steps = [time_steps]
+    if isinstance(injectors, str):
+        injectors = [injectors]
+    if isinstance(producers, str):
+        producers = [producers]
+    return self._execute_command(
+        exportFlowCharacteristics=Cmd.ExportFlowInfoRequest(
+            caseId=self.id,
+            timeSteps=time_steps,
+            injectors=injectors,
+            producers=producers,
+            fileName=file_name,
+            minimumCommunication=minimum_communication,
+            aquiferCellThreshold=aquifer_cell_threshold,
+        )
+    )
+
+
+@add_method(Case)
+def available_properties(self, property_type, porosity_model="MATRIX_MODEL"):
+    """Get a list of available properties
+
+    For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type (str): string corresponding to property_type enum.
+        porosity_model(str): 'MATRIX_MODEL' or 'FRACTURE_MODEL'.
+    """
+
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.AvailablePropertiesRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        porosity_model=porosity_model_enum,
+    )
+    return self.__properties_stub.GetAvailableProperties(request).property_names
+
+
+@add_method(Case)
+def active_cell_property_async(
+    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
+):
+    """Get a cell property for all active cells. Async, so returns an iterator. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum
+
+    Returns:
+        An iterator to a chunk object containing an array of double values
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.PropertyRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        property_name=property_name,
+        time_step=time_step,
+        porosity_model=porosity_model_enum,
+    )
+    for chunk in self.__properties_stub.GetActiveCellProperty(request):
+        yield chunk
+
+
+@add_method(Case)
+def active_cell_property(
+    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
+):
+    """Get a cell property for all active cells. Sync, so returns a list. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum
+
+    Returns:
+        A list containing double values
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    all_values = []
+    generator = self.active_cell_property_async(
+        property_type, property_name, time_step, porosity_model
+    )
+    for chunk in generator:
+        for value in chunk.values:
+            all_values.append(value)
+    return all_values
+
+
+@add_method(Case)
+def selected_cell_property_async(
+    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
+):
+    """Get a cell property for all selected cells. Async, so returns an iterator. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum
+
+    Returns:
+        An iterator to a chunk object containing an array of double values
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.PropertyRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        property_name=property_name,
+        time_step=time_step,
+        porosity_model=porosity_model_enum,
+    )
+    for chunk in self.__properties_stub.GetSelectedCellProperty(request):
+        yield chunk
+
+
+@add_method(Case)
+def selected_cell_property(
+    self, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
+):
+    """Get a cell property for all selected cells. Sync, so returns a list. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum
+
+    Returns:
+        A list containing double values
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    all_values = []
+    generator = self.selected_cell_property_async(
+        property_type, property_name, time_step, porosity_model
+    )
+    for chunk in generator:
+        for value in chunk.values:
+            all_values.append(value)
+    return all_values
+
+
+@add_method(Case)
+def grid_property_async(
+    self,
+    property_type,
+    property_name,
+    time_step,
+    grid_index=0,
+    porosity_model="MATRIX_MODEL",
+):
+    """Get a cell property for all grid cells. Async, so returns an iterator. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        gridIndex(int): index to the grid we're getting values for
+        porosity_model(str): string enum
+
+    Returns:
+        An iterator to a chunk object containing an array of double values
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.PropertyRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        property_name=property_name,
+        time_step=time_step,
+        grid_index=grid_index,
+        porosity_model=porosity_model_enum,
+    )
+    for chunk in self.__properties_stub.GetGridProperty(request):
+        yield chunk
+
+
+@add_method(Case)
+def grid_property(
+    self,
+    property_type,
+    property_name,
+    time_step,
+    grid_index=0,
+    porosity_model="MATRIX_MODEL",
+):
+    """Get a cell property for all grid cells. Synchronous, so returns a list. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        grid_index(int): index to the grid we're getting values for
+        porosity_model(str): string enum
+
+    Returns:
+        A list of double values
+    """
+    all_values = []
+    generator = self.grid_property_async(
+        property_type, property_name, time_step, grid_index, porosity_model
+    )
+    for chunk in generator:
+        for value in chunk.values:
+            all_values.append(value)
+    return all_values
+
+
+@add_method(Case)
+def set_active_cell_property_async(
+    self,
+    values_iterator,
+    property_type,
+    property_name,
+    time_step,
+    porosity_model="MATRIX_MODEL",
+):
+    """Set cell property for all active cells Async. Takes an iterator to the input values. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        values_iterator(iterator): an iterator to the properties to be set
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum
+    """
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.PropertyRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        property_name=property_name,
+        time_step=time_step,
+        porosity_model=porosity_model_enum,
+    )
+
+    request_iterator = self.__generate_property_input_iterator(values_iterator, request)
+    self.__properties_stub.SetActiveCellProperty(request_iterator)
+
+
+@add_method(Case)
+def set_active_cell_property(
+    self, values, property_type, property_name, time_step, porosity_model="MATRIX_MODEL"
+):
+    """Set a cell property for all active cells. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        values(list): a list of double precision floating point numbers
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum
+    """
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.PropertyRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        property_name=property_name,
+        time_step=time_step,
+        porosity_model=porosity_model_enum,
+    )
+    request_iterator = self.__generate_property_input_chunks(values, request)
+    reply = self.__properties_stub.SetActiveCellProperty(request_iterator)
+    if reply.accepted_value_count < len(values):
+        raise IndexError
+
+
+@add_method(Case)
+def set_grid_property(
+    self,
+    values,
+    property_type,
+    property_name,
+    time_step,
+    grid_index=0,
+    porosity_model="MATRIX_MODEL",
+):
+    """Set a cell property for all grid cells. For argument details, see :ref:`Result Definition <result-definition-label>`
+
+    Arguments:
+        values(list): a list of double precision floating point numbers
+        property_type(str): string enum
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        grid_index(int): index to the grid we're setting values for
+        porosity_model(str): string enum
+    """
+    property_type_enum = Properties_pb2.PropertyType.Value(property_type)
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Properties_pb2.PropertyRequest(
+        case_request=self.__request(),
+        property_type=property_type_enum,
+        property_name=property_name,
+        time_step=time_step,
+        grid_index=grid_index,
+        porosity_model=porosity_model_enum,
+    )
+    request_iterator = self.__generate_property_input_chunks(values, request)
+    reply = self.__properties_stub.SetGridProperty(request_iterator)
+    if reply.accepted_value_count < len(values):
+        raise IndexError
+
+
+@add_method(Case)
+def export_property(
+    self,
+    time_step,
+    property_name,
+    eclipse_keyword=property,
+    undefined_value=0.0,
+    export_file=property,
+):
+    """Export an Eclipse property
+
+    Arguments:
+        time_step (int): time step index
+        property_name (str): property to export
+        eclipse_keyword (str): Keyword used in export header. Defaults: value of property
+        undefined_value (double): Value to use for undefined values. Defaults to 0.0
+        export_file (str): File name for export. Defaults to the value of property parameter
+    """
+    return self._execute_command(
+        exportProperty=Cmd.ExportPropertyRequest(
+            caseId=self.id,
+            timeStep=time_step,
+            property=property_name,
+            eclipseKeyword=eclipse_keyword,
+            undefinedValue=undefined_value,
+            exportFile=export_file,
+        )
+    )
+
+
+@add_method(Case)
+def create_well_bore_stability_plot(self, well_path, time_step, parameters=None):
+    """Create a new well bore stability plot
+
+    Arguments:
+        well_path(str): well path name
+        time_step(int): time step
+
+    Returns:
+        :class:`rips.generated.generated_classes.WellBoreStabilityPlot`
+    """
+    pb2_parameters = None
+    if parameters is not None:
+        assert isinstance(parameters, WbsParameters)
+        pb2_parameters = parameters.pb2_object()
+
+    plot_result = self._execute_command(
+        createWellBoreStabilityPlot=Cmd.CreateWbsPlotRequest(
+            caseId=self.id,
+            wellPath=well_path,
+            timeStep=time_step,
+            wbsParameters=pb2_parameters,
+        )
+    )
+    project = self.ancestor(rips.project.Project)
+    plot = project.plot(view_id=plot_result.createWbsPlotResult.viewId)
+    return plot
+
+
+@add_method(Case)
+def import_formation_names(self, formation_files=None):
+    """Import formation names into project and apply it to the current case
+
+    Arguments:
+        formation_files(list): list of files to import
+
+    """
+    if formation_files is None:
+        formation_files = []
+    elif isinstance(formation_files, str):
+        formation_files = [formation_files]
+
+    self._execute_command(
+        importFormationNames=Cmd.ImportFormationNamesRequest(
+            formationFiles=formation_files, applyToCaseId=self.id
+        )
+    )
+
+
+@add_method(Case)
+def simulation_wells(self):
+    """Get a list of all simulation wells for a case
+
+    Returns:
+        :class:`rips.generated.generated_classes.SimulationWell`
+
+    """
+    wells = self.descendants(SimulationWell)
+    return wells
+
+
+@add_method(Case)
+def active_cell_centers_async(self, porosity_model="MATRIX_MODEL"):
+    """Get a cell centers for all active cells. Async, so returns an iterator
+
+    Arguments:
+        porosity_model(str): string enum. See available()
+
+    Returns:
+        An iterator to a chunk object containing an array of Vec3d values.
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Case_pb2.CellInfoRequest(
+        case_request=self.__request(), porosity_model=porosity_model_enum
+    )
+    return self.__case_stub.GetCellCenterForActiveCells(request)
+
+
+@add_method(Case)
+def active_cell_centers(self, porosity_model="MATRIX_MODEL"):
+    """Get a cell centers for all active cells. Synchronous, so returns a list.
+
+    Arguments:
+        porosity_model(str): string enum. See available()
+
+    Returns:
+        A list of Vec3d
+    """
+    cell_centers = []
+    generator = self.active_cell_centers_async(porosity_model)
+    for chunk in generator:
+        for value in chunk.centers:
+            cell_centers.append(value)
+    return cell_centers
+
+
+@add_method(Case)
+def active_cell_corners_async(self, porosity_model="MATRIX_MODEL"):
+    """Get a cell corners for all active cells. Async, so returns an iterator
+
+    Arguments:
+        porosity_model(str): string enum. See available()
+
+    Returns:
+        An iterator to a chunk object containing an array of CellCorners (which is eight Vec3d values).
+        Loop through the chunks and then the values within the chunk to get all values.
+    """
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = Case_pb2.CellInfoRequest(
+        case_request=self.__request(), porosity_model=porosity_model_enum
+    )
+    return self.__case_stub.GetCellCornersForActiveCells(request)
+
+
+@add_method(Case)
+def active_cell_corners(self, porosity_model="MATRIX_MODEL"):
+    """Get a cell corners for all active cells. Synchronous, so returns a list.
+
+        Arguments:
+            porosity_model(str): string enum. See available()
+
+    **CellCorner class description**::
+
+        Parameter   | Description   | Type
+        ----------- | ------------  | -----
+        c0          |               | Vec3d
+        c1          |               | Vec3d
+        c2          |               | Vec3d
+        c3          |               | Vec3d
+        c4          |               | Vec3d
+        c5          |               | Vec3d
+        c6          |               | Vec3d
+        c7          |               | Vec3d
+
+
+    """
+    cell_corners = []
+    generator = self.active_cell_corners_async(porosity_model)
+    for chunk in generator:
+        for value in chunk.cells:
+            cell_corners.append(value)
+    return cell_corners
+
+
+@add_method(Case)
+def selected_cells_async(self):
+    """Get the selected cells. Async, so returns an iterator.
+
+    Returns:
+        An iterator to a chunk object containing an array of cells.
+        Loop through the chunks and then the cells within the chunk to get all cells.
+    """
+    return self.__case_stub.GetSelectedCells(self.__request())
+
+
+@add_method(Case)
+def selected_cells(self):
+    """Get the selected cells. Synchronous, so returns a list.
+
+    Returns:
+        A list of Cells.
+    """
+    cells = []
+    generator = self.selected_cells_async()
+    for chunk in generator:
+        for value in chunk.cells:
+            cells.append(value)
+    return cells
+
+
+@add_method(Case)
+def coarsening_info(self):
+    """Get a coarsening information for all grids in the case.
+
+    Returns:
+        A list of CoarseningInfo objects with two Vec3i min and max objects
+        for each entry.
+    """
+    return self.__case_stub.GetCoarseningInfoArray(self.__request()).data
+
+
+@add_method(Case)
+def available_nnc_properties(self):
+    """Get a list of available NNC properties
+
+    **NNCConnection class description**::
+
+          Parameter               | Description                                   | Type
+          ------------------------| --------------------------------------------- | -----
+          cell_grid_index1        | Reservoir Cell Index to cell 1                | int32
+          cell_grid_index2        | Reservoir Cell Index to cell 2                | int32
+          cell1                   | Reservoir Cell IJK to cell 1                  | Vec3i
+          cell2                   | Reservoir Cell IJK to cell 1                  | Vec3i
+
+    """
+    return self.__nnc_properties_stub.GetAvailableNNCProperties(
+        self.__request()
+    ).properties
+
+
+@add_method(Case)
+def nnc_connections_async(self):
+    """Get the NNC connections. Async, so returns an iterator.
+
+    Returns:
+        An iterator to a chunk object containing an array NNCConnection objects.
+        Loop through the chunks and then the connection within the chunk to get all connections.
+    """
+    return self.__nnc_properties_stub.GetNNCConnections(self.__request())
+
+
+@add_method(Case)
+def nnc_connections(self):
+    """Get the NNC connection. Synchronous, so returns a list.
+
+    Returns:
+        A list of NNCConnection objects.
+    """
+    connections = []
+    generator = self.nnc_connections_async()
+    for chunk in generator:
+        for value in chunk.connections:
+            connections.append(value)
+    return connections
+
+
+@add_method(Case)
+def __nnc_connections_values_async(self, property_name, property_type, time_step):
+    request = NNCProperties_pb2.NNCValuesRequest(
+        case_id=self.id,
+        property_name=property_name,
+        property_type=property_type,
+        time_step=time_step,
+    )
+    return self.__nnc_properties_stub.GetNNCValues(request)
+
+
+@add_method(Case)
+def __nnc_values_generator_to_list(self, generator):
+    """Converts a NNC values generator to a list."""
+    vals = []
+    for chunk in generator:
+        for value in chunk.values:
+            vals.append(value)
+    return vals
+
+
+@add_method(Case)
+def nnc_connections_static_values_async(self, property_name):
+    """Get the static NNC values. Async, so returns an iterator.
+
+    Returns:
+        An iterator to a chunk object containing an list of doubles.
+        Loop through the chunks and then the values within the chunk to get values
+        for all the connections. The order of the list matches the list from
+        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
+        value in this list.
+    """
+    return self.__nnc_connections_values_async(
+        property_name, NNCProperties_pb2.NNC_STATIC, 0
+    )
+
+
+@add_method(Case)
+def nnc_connections_static_values(self, property_name):
+    """Get the static NNC values.
+
+    Returns:
+        A list of doubles. The order of the list matches the list from
+        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
+        value in this list.
+    """
+    generator = self.nnc_connections_static_values_async(property_name)
+    return self.__nnc_values_generator_to_list(generator)
+
+
+@add_method(Case)
+def nnc_connections_dynamic_values_async(self, property_name, time_step):
+    """Get the dynamic NNC values. Async, so returns an iterator.
+
+    Returns:
+        An iterator to a chunk object containing an list of doubles.
+        Loop through the chunks and then the values within the chunk to get values
+        for all the connections. The order of the list matches the list from
+        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
+        value in this list.
+    """
+    return self.__nnc_connections_values_async(
+        property_name, NNCProperties_pb2.NNC_DYNAMIC, time_step
+    )
+
+
+@add_method(Case)
+def nnc_connections_dynamic_values(self, property_name, time_step):
+    """Get the dynamic NNC values.
+
+    Returns:
+        A list of doubles. The order of the list matches the list from
+        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
+        value in this list.
+    """
+    generator = self.nnc_connections_dynamic_values_async(property_name, time_step)
+    return self.__nnc_values_generator_to_list(generator)
+
+
+@add_method(Case)
+def nnc_connections_generated_values_async(self, property_name, time_step):
+    """Get the generated NNC values. Async, so returns an iterator.
+
+    Returns:
+        An iterator to a chunk object containing an list of doubles.
+        Loop through the chunks and then the values within the chunk to get values
+        for all the connections. The order of the list matches the list from
+        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
+        value in this list.
+    """
+    return self.__nnc_connections_values_async(
+        property_name, NNCProperties_pb2.NNC_GENERATED, time_step
+    )
+
+
+@add_method(Case)
+def nnc_connections_generated_values(self, property_name, time_step):
+    """Get the generated NNC values.
+
+    Returns:
+        A list of doubles. The order of the list matches the list from
+        nnc_connections, i.e. the nth object of nnc_connections() refers to nth
+        value in this list.
+    """
+    generator = self.nnc_connections_generated_values_async(property_name, time_step)
+    return self.__nnc_values_generator_to_list(generator)
+
+
+@add_method(Case)
+def __generate_nnc_property_input_chunks(self, array, parameters):
+    index = -1
+    while index < len(array):
+        chunk = NNCProperties_pb2.NNCValuesChunk()
+        if index == -1:
+            chunk.params.CopyFrom(parameters)
+            index += 1
+        else:
+            actual_chunk_size = min(len(array) - index + 1, self.chunk_size)
+            chunk.values.CopyFrom(
+                NNCProperties_pb2.NNCValues(
+                    values=array[index : index + actual_chunk_size]
+                )
+            )
+            index += actual_chunk_size
+
+        yield chunk
+    # Final empty message to signal completion
+    chunk = NNCProperties_pb2.NNCValuesChunk()
+    yield chunk
+
+
+@add_method(Case)
+def set_nnc_connections_values(
+    self, values, property_name, time_step, porosity_model="MATRIX_MODEL"
+):
+    """Set nnc connection values for all connections..
+
+    Arguments:
+        values(list): a list of double precision floating point numbers
+        property_name(str): name of an Eclipse property
+        time_step(int): the time step for which to get the property for
+        porosity_model(str): string enum. See available()
+    """
+    porosity_model_enum = Case_pb2.PorosityModelType.Value(porosity_model)
+    request = NNCProperties_pb2.NNCValuesInputRequest(
+        case_id=self.id,
+        property_name=property_name,
+        time_step=time_step,
+        porosity_model=porosity_model_enum,
+    )
+    request_iterator = self.__generate_nnc_property_input_chunks(values, request)
+    reply = self.__nnc_properties_stub.SetNNCValues(request_iterator)
+    if reply.accepted_value_count < len(values):
+        raise IndexError
```

### Comparing `rips-2023.6.0.1/rips/contour_map.py` & `rips-2023.6.0.2/rips/contour_map.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""
-ResInsight 3d contour map module
-"""
-import Commands_pb2
-
-from .pdmobject import add_method
-from .view import View
-from .resinsight_classes import EclipseContourMap, GeoMechContourMap
-
-
-@add_method(EclipseContourMap)
-def export_to_text(
-    self,
-    export_file_name="",
-    export_local_coordinates=False,
-    undefined_value_label="NaN",
-    exclude_undefined_values=False,
-):
-    """Export snapshot for the current view
-
-    Arguments:
-        export_file_name(str): The file location to store results in.
-        export_local_coordinates(bool): Should we export local coordinates, or UTM.
-        undefined_value_label(str): Replace undefined values with this label.
-        exclude_undefined_values(bool): Skip undefined values.
-    """
-    return self._execute_command(
-        exportContourMapToText=Commands_pb2.ExportContourMapToTextRequest(
-            exportFileName=export_file_name,
-            exportLocalCoordinates=export_local_coordinates,
-            undefinedValueLabel=undefined_value_label,
-            excludeUndefinedValues=exclude_undefined_values,
-            viewId=self.id,
-        )
-    )
-
-
-@add_method(GeoMechContourMap)
-def export_to_text(
-    self,
-    export_file_name="",
-    export_local_coordinates=False,
-    undefined_value_label="NaN",
-    exclude_undefined_values=False,
-):
-    """Export snapshot for the current view
-
-    Arguments:
-        export_file_name(str): The file location to store results in.
-        export_local_coordinates(bool): Should we export local coordinates, or UTM.
-        undefined_value_label(str): Replace undefined values with this label.
-        exclude_undefined_values(bool): Skip undefined values.
-    """
-    return self._execute_command(
-        exportContourMapToText=Commands_pb2.ExportContourMapToTextRequest(
-            exportFileName=export_file_name,
-            exportLocalCoordinates=export_local_coordinates,
-            undefinedValueLabel=undefined_value_label,
-            excludeUndefinedValues=exclude_undefined_values,
-            viewId=self.id,
-        )
-    )
+"""
+ResInsight 3d contour map module
+"""
+import Commands_pb2
+
+from .pdmobject import add_method
+from .view import View
+from .resinsight_classes import EclipseContourMap, GeoMechContourMap
+
+
+@add_method(EclipseContourMap)
+def export_to_text(
+    self,
+    export_file_name="",
+    export_local_coordinates=False,
+    undefined_value_label="NaN",
+    exclude_undefined_values=False,
+):
+    """Export snapshot for the current view
+
+    Arguments:
+        export_file_name(str): The file location to store results in.
+        export_local_coordinates(bool): Should we export local coordinates, or UTM.
+        undefined_value_label(str): Replace undefined values with this label.
+        exclude_undefined_values(bool): Skip undefined values.
+    """
+    return self._execute_command(
+        exportContourMapToText=Commands_pb2.ExportContourMapToTextRequest(
+            exportFileName=export_file_name,
+            exportLocalCoordinates=export_local_coordinates,
+            undefinedValueLabel=undefined_value_label,
+            excludeUndefinedValues=exclude_undefined_values,
+            viewId=self.id,
+        )
+    )
+
+
+@add_method(GeoMechContourMap)
+def export_to_text(
+    self,
+    export_file_name="",
+    export_local_coordinates=False,
+    undefined_value_label="NaN",
+    exclude_undefined_values=False,
+):
+    """Export snapshot for the current view
+
+    Arguments:
+        export_file_name(str): The file location to store results in.
+        export_local_coordinates(bool): Should we export local coordinates, or UTM.
+        undefined_value_label(str): Replace undefined values with this label.
+        exclude_undefined_values(bool): Skip undefined values.
+    """
+    return self._execute_command(
+        exportContourMapToText=Commands_pb2.ExportContourMapToTextRequest(
+            exportFileName=export_file_name,
+            exportLocalCoordinates=export_local_coordinates,
+            undefinedValueLabel=undefined_value_label,
+            excludeUndefinedValues=exclude_undefined_values,
+            viewId=self.id,
+        )
+    )
```

### Comparing `rips-2023.6.0.1/rips/generated/App_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/App_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/Case_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/Case_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/Commands_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/Commands_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/Grid_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/Grid_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/NNCProperties_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/NNCProperties_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/PdmObject_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/PdmObject_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/Project_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/Project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/Properties_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/Properties_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/RiaVersionInfo.py` & `rips-2023.6.0.2/rips/generated/RiaVersionInfo.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#
-#  Copyright (C) 2019- Equinor ASA
-# 
-#  ResInsight is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-# 
-#  ResInsight is distributed in the hope that it will be useful, but WITHOUT ANY
-#  WARRANTY; without even the implied warranty of MERCHANTABILITY or
-#  FITNESS FOR A PARTICULAR PURPOSE.
-# 
-#  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html> 
-#  for more details.
-#
-#  Python version of RiaVersionInfo.h
-#  Just sets version constants
-
-RESINSIGHT_MAJOR_VERSION = "2023"
-RESINSIGHT_MINOR_VERSION = "06"
-RESINSIGHT_PATCH_VERSION = "0"
+#
+#  Copyright (C) 2019- Equinor ASA
+# 
+#  ResInsight is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+# 
+#  ResInsight is distributed in the hope that it will be useful, but WITHOUT ANY
+#  WARRANTY; without even the implied warranty of MERCHANTABILITY or
+#  FITNESS FOR A PARTICULAR PURPOSE.
+# 
+#  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html> 
+#  for more details.
+#
+#  Python version of RiaVersionInfo.h
+#  Just sets version constants
+
+RESINSIGHT_MAJOR_VERSION = "2023"
+RESINSIGHT_MINOR_VERSION = "06"
+RESINSIGHT_PATCH_VERSION = "0"
```

### Comparing `rips-2023.6.0.1/rips/generated/SimulationWell_pb2_grpc.py` & `rips-2023.6.0.2/rips/generated/SimulationWell_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/rips/generated/generated_classes.py` & `rips-2023.6.0.2/rips/generated/generated_classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,2087 +1,2085 @@
-from rips.pdmobject import PdmObjectBase
-class CellFilterCollection(PdmObjectBase):
-    """
-    Attributes:
-        active (bool): Active
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.active = True
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if CellFilterCollection.__custom_init__ is not None:
-            CellFilterCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class CurveIntersection(PdmObjectBase):
-    """
-    Attributes:
-        name (str): Name
-        points (List of str): Points
-        simulation_well (str): Simulation Well
-        type (str): One of [CS_WELL_PATH, CS_SIMULATION_WELL, CS_POLYLINE, CS_AZIMUTHLINE]
-        well_path (str): Well Path        
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.name = "Intersection Name"
-        self.points = []
-        self.simulation_well = ""
-        self.type = "CS_POLYLINE"
-        self.well_path = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if CurveIntersection.__custom_init__ is not None:
-            CurveIntersection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def geometry(self, geometry_type="FULL_3D"):
-        """
-        
-
-        Arguments:
-            geometry_type (str): One of [FULL_3D, PROJECTED_TO_PLANE]
-        Returns:
-            TriangleGeometry
-        """
-        return self._call_pdm_method("geometry", geometry_type=geometry_type)
-
-
-    def geometry_result(self, geometry_type="FULL_3D"):
-        """
-        
-
-        Arguments:
-            geometry_type (str): One of [FULL_3D, PROJECTED_TO_PLANE]
-        Returns:
-            DataContainerFloat
-        """
-        return self._call_pdm_method("geometryResult", geometry_type=geometry_type)
-
-
-class DataContainerFloat(PdmObjectBase):
-    """
-    Attributes:
-        values (List of float): Float Values
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.values = []
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if DataContainerFloat.__custom_init__ is not None:
-            DataContainerFloat.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class DataContainerString(PdmObjectBase):
-    """
-    Attributes:
-        values (List of str): String Values
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.values = []
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if DataContainerString.__custom_init__ is not None:
-            DataContainerString.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class DataContainerTime(PdmObjectBase):
-    """
-    Attributes:
-        values (List of time): Time Values
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.values = []
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if DataContainerTime.__custom_init__ is not None:
-            DataContainerTime.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class Case(PdmObjectBase):
-    """
-    The ResInsight base class for Cases
-
-    Attributes:
-        file_path (str): Case File Name
-        id (int): Case ID
-        name (str): Case Name
-        name_setting (str): One of [FULL_CASE_NAME, SHORT_CASE_NAME, CUSTOM_NAME]
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.file_path = ""
-        self.id = -1
-        self.name = ""
-        self.name_setting = "FULL_CASE_NAME"
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if Case.__custom_init__ is not None:
-            Case.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class Reservoir(Case):
-    """
-    Abstract base class for Eclipse Cases
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        Case.__init__(self, pb2_object, channel)
-        if Reservoir.__custom_init__ is not None:
-            Reservoir.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def import_properties(self, file_names=[]):
-        """
-        Import Properties
-
-        Arguments:
-            file_names (List of str): 
-        Returns:
-            
-        """
-        return self._call_pdm_method("import_properties", file_names=file_names)
-
-
-    def views(self):
-        """All Eclipse Views in the case
-
-        Returns:
-             List of EclipseView
-        """
-        return self.children("Views", EclipseView)
-
-
-class EclipseCase(Reservoir):
-    """
-    The Regular Eclipse Results Case
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        Reservoir.__init__(self, pb2_object, channel)
-        if EclipseCase.__custom_init__ is not None:
-            EclipseCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class ElasticProperties(PdmObjectBase):
-    """
-    Attributes:
-        file_path (str): File Path
-        properties_table (str): Properties Table
-        show_scaled_properties (bool): Show Scaled Properties
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.file_path = ""
-        self.properties_table = ""
-        self.show_scaled_properties = True
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if ElasticProperties.__custom_init__ is not None:
-            ElasticProperties.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def add_property_scaling(self, formation="", facies="", property="", scale=1):
-        """
-        Add Elastic Property Scaling
-
-        Arguments:
-            formation (str): Formation
-            facies (str): Facies
-            property (str): Property
-            scale (float): Scale
-        Returns:
-            ElasticPropertyScaling
-        """
-        return self._call_pdm_method("AddPropertyScaling", formation=formation, facies=facies, property=property, scale=scale)
-
-
-    def property_scaling_collection(self):
-        """PropertyScalingCollection
-
-        Returns:
-             ElasticPropertyScalingCollection
-        """
-        children = self.children("PropertyScalingCollection", ElasticPropertyScalingCollection)
-        return children[0] if len(children) > 0 else None
-
-
-class NamedObject(PdmObjectBase):
-    """
-    Attributes:
-        name (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.name = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if NamedObject.__custom_init__ is not None:
-            NamedObject.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class CheckableNamedObject(NamedObject):
-    """
-    Attributes:
-        is_checked (bool): Active
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.is_checked = True
-        NamedObject.__init__(self, pb2_object, channel)
-        if CheckableNamedObject.__custom_init__ is not None:
-            CheckableNamedObject.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class ElasticPropertyScaling(CheckableNamedObject):
-    """
-    Attributes:
-        facies (str): Facies
-        formation (str): Formation
-        property (str): One of [UNDEFINED, FACIES, LAYERS, POROSITY, PERMEABILITY_X, PERMEABILITY_Z, INITIAL_PRESSURE, PRESSURE, STRESS, INITIAL_STRESS, STRESS_GRADIENT, YOUNGS_MODULUS, POISSONS_RATIO, K_IC, PROPPANT_EMBEDMENT, BIOT_COEFFICIENT, K0, FLUID_LOSS_COEFFICIENT, SPURT_LOSS, TEMPERATURE, RELATIVE_PERMEABILITY_FACTOR, PORO_ELASTIC_CONSTANT, THERMAL_EXPANSION_COEFFICIENT, IMMOBILE_FLUID_SATURATION, NET_TO_GROSS, POROSITY_UNSCALED, EQLNUM, PRESSURE_GRADIENT, FORMATIONS]
-        scale (float): Scale
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.facies = ""
-        self.formation = ""
-        self.property = "YOUNGS_MODULUS"
-        self.scale = 1
-        CheckableNamedObject.__init__(self, pb2_object, channel)
-        if ElasticPropertyScaling.__custom_init__ is not None:
-            ElasticPropertyScaling.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class ElasticPropertyScalingCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if ElasticPropertyScalingCollection.__custom_init__ is not None:
-            ElasticPropertyScalingCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def elastic_property_scalings(self):
-        """Elastic Property Scalings
-
-        Returns:
-             List of ElasticPropertyScaling
-        """
-        return self.children("ElasticPropertyScalings", ElasticPropertyScaling)
-
-
-class SurfaceInterface(PdmObjectBase):
-    """
-    Attributes:
-        depth_offset (float): Depth Offset
-        surface_user_decription (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.depth_offset = 0
-        self.surface_user_decription = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if SurfaceInterface.__custom_init__ is not None:
-            SurfaceInterface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def export_to_file(self, file_name=""):
-        """
-        Export a surface to file
-
-        Arguments:
-            file_name (str): Filename to export surface to
-        Returns:
-            DataContainerString
-        """
-        return self._call_pdm_method("ExportToFile", file_name=file_name)
-
-
-class EnsembleStatisticsSurface(SurfaceInterface):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        SurfaceInterface.__init__(self, pb2_object, channel)
-        if EnsembleStatisticsSurface.__custom_init__ is not None:
-            EnsembleStatisticsSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class SurfaceCollection(PdmObjectBase):
-    """
-    Attributes:
-        surface_user_decription (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.surface_user_decription = "Surfaces"
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if SurfaceCollection.__custom_init__ is not None:
-            SurfaceCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def add_folder(self, folder_name="Surfaces"):
-        """
-        Add a new surface folder
-
-        Arguments:
-            folder_name (str): New surface folder name
-        Returns:
-            SurfaceCollection
-        """
-        return self._call_pdm_method("AddFolder", folder_name=folder_name)
-
-
-    def import_surface(self, file_name=""):
-        """
-        Import a new surface from file
-
-        Arguments:
-            file_name (str): Filename to import surface from
-        Returns:
-            Surface
-        """
-        return self._call_pdm_method("ImportSurface", file_name=file_name)
-
-
-    def new_surface(self, case="", k_index=0):
-        """
-        Create a new surface
-
-        Arguments:
-            case (Case): 
-            k_index (int): 
-        Returns:
-            GridCaseSurface
-        """
-        return self._call_pdm_method("NewSurface", case=case, k_index=k_index)
-
-
-    def sub_collections(self):
-        """Surfaces
-
-        Returns:
-             List of SurfaceCollection
-        """
-        return self.children("SubCollections", SurfaceCollection)
-
-
-    def surfaces_field(self):
-        """Surfaces
-
-        Returns:
-             List of SurfaceInterface
-        """
-        return self.children("SurfacesField", SurfaceInterface)
-
-
-class EnsembleSurface(SurfaceCollection):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        SurfaceCollection.__init__(self, pb2_object, channel)
-        if EnsembleSurface.__custom_init__ is not None:
-            EnsembleSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class EnsembleWellLogs(NamedObject):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        NamedObject.__init__(self, pb2_object, channel)
-        if EnsembleWellLogs.__custom_init__ is not None:
-            EnsembleWellLogs.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class FaciesInitialPressureConfig(PdmObjectBase):
-    """
-    Attributes:
-        facies_name (str): Facies
-        facies_value (int): Value
-        fraction (float): ? Pressure Fraction
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.facies_name = ""
-        self.facies_value = -1
-        self.fraction = 0
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if FaciesInitialPressureConfig.__custom_init__ is not None:
-            FaciesInitialPressureConfig.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class FaciesProperties(PdmObjectBase):
-    """
-    Attributes:
-        color_legend (str): Colors
-        file_path (str): File Path
-        properties_table (str): Properties Table
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.color_legend = ""
-        self.file_path = ""
-        self.properties_table = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if FaciesProperties.__custom_init__ is not None:
-            FaciesProperties.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def facies_definition(self):
-        """
-
-        Returns:
-             EclipseResult
-        """
-        children = self.children("FaciesDefinition", EclipseResult)
-        return children[0] if len(children) > 0 else None
-
-
-class SummaryCase(PdmObjectBase):
-    """
-    The Base Class for all Summary Cases
-
-    Attributes:
-        auto_shorty_name (bool): Use Auto Display Name
-        id (int): Case ID
-        name_setting (str): One of [FULL_CASE_NAME, SHORT_CASE_NAME, CUSTOM_NAME]
-        short_name (str): Display Name
-        show_sub_nodes_in_tree (bool): Show Summary Data Sub-Tree
-        summary_header_filename (str): Summary Header File
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.auto_shorty_name = False
-        self.id = -1
-        self.name_setting = "FULL_CASE_NAME"
-        self.short_name = ""
-        self.show_sub_nodes_in_tree = False
-        self.summary_header_filename = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if SummaryCase.__custom_init__ is not None:
-            SummaryCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def available_addresses(self, ):
-        """
-        
-
-        Arguments:
-            
-        Returns:
-            DataContainerString
-        """
-        return self._call_pdm_method("availableAddresses")
-
-
-    def available_time_steps(self, ):
-        """
-        
-
-        Arguments:
-            
-        Returns:
-            DataContainerTime
-        """
-        return self._call_pdm_method("availableTimeSteps")
-
-
-    def resample_values(self, address="", resampling_period=""):
-        """
-        
-
-        Arguments:
-            address (str): Formatted address specifying the summary vector
-            resampling_period (str): Resampling Period
-        Returns:
-            ResampleData
-        """
-        return self._call_pdm_method("resampleValues", address=address, resampling_period=resampling_period)
-
-
-    def set_summary_values(self, address="", unit="", values=[]):
-        """
-        
-
-        Arguments:
-            address (str): Formatted address specifying the summary vector
-            unit (str): Unit
-            values (List of float): Values
-        Returns:
-            
-        """
-        return self._call_pdm_method("setSummaryValues", address=address, unit=unit, values=values)
-
-
-    def summary_vector_values(self, address=""):
-        """
-        Get all values for a summary vector
-
-        Arguments:
-            address (str): Formatted address specifying the summary vector
-        Returns:
-            DataContainerFloat
-        """
-        return self._call_pdm_method("summaryVectorValues", address=address)
-
-
-class FileSummaryCase(SummaryCase):
-    """
-    A Summary Case based on SMSPEC files
-
-    Attributes:
-        include_restart_files (bool): Include Restart Files
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.include_restart_files = False
-        SummaryCase.__init__(self, pb2_object, channel)
-        if FileSummaryCase.__custom_init__ is not None:
-            FileSummaryCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class FractureTemplateCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if FractureTemplateCollection.__custom_init__ is not None:
-            FractureTemplateCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def append_fracture_template(self, file_path=""):
-        """
-        Create a new StimPlan Fracture Template
-
-        Arguments:
-            file_path (str): File Path to StimPlan Countour File
-        Returns:
-            StimPlanFractureTemplate
-        """
-        return self._call_pdm_method("AppendFractureTemplate", file_path=file_path)
-
-
-    def append_thermal_fracture_template(self, file_path=""):
-        """
-        Create a new Thermal Fracture Template
-
-        Arguments:
-            file_path (str): File Path to Thermal Fracture CSV File
-        Returns:
-            ThermalFractureTemplate
-        """
-        return self._call_pdm_method("AppendThermalFractureTemplate", file_path=file_path)
-
-
-class GeoMechPart(CheckableNamedObject):
-    """
-    Attributes:
-        part_id (int): Part Id
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.part_id = -1
-        CheckableNamedObject.__init__(self, pb2_object, channel)
-        if GeoMechPart.__custom_init__ is not None:
-            GeoMechPart.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GeoMechPartCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if GeoMechPartCollection.__custom_init__ is not None:
-            GeoMechPartCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def parts(self):
-        """Parts
-
-        Returns:
-             List of GeoMechPart
-        """
-        return self.children("Parts", GeoMechPart)
-
-
-class ViewWindow(PdmObjectBase):
-    """
-    The Base Class for all Views and Plots in ResInsight
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if ViewWindow.__custom_init__ is not None:
-            ViewWindow.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class View(ViewWindow):
-    """
-    Attributes:
-        background_color (str): Background
-        current_time_step (int): Current Time Step
-        disable_lighting (bool): Disable Results Lighting
-        grid_z_scale (float): Z Scale
-        id (int): View ID
-        perspective_projection (bool): Perspective Projection
-        show_grid_box (bool): Show Grid Box
-        show_z_scale (bool): Show Z Scale Label
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.background_color = "#3b3b3b"
-        self.current_time_step = 0
-        self.disable_lighting = False
-        self.grid_z_scale = 5
-        self.id = -1
-        self.perspective_projection = True
-        self.show_grid_box = True
-        self.show_z_scale = True
-        ViewWindow.__init__(self, pb2_object, channel)
-        if View.__custom_init__ is not None:
-            View.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GeoMechView(View):
-    """
-    The Geomechanical 3d View
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        View.__init__(self, pb2_object, channel)
-        if GeoMechView.__custom_init__ is not None:
-            GeoMechView.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GridCaseSurface(SurfaceInterface):
-    """
-    Attributes:
-        include_inactive_cells (bool): Include Inactive Cells
-        slice_index (int): Slice Index (K)
-        source_case (str): Source Case
-        watertight (bool): Watertight Surface (fill gaps)
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.include_inactive_cells = False
-        self.slice_index = 1
-        self.source_case = ""
-        self.watertight = False
-        SurfaceInterface.__init__(self, pb2_object, channel)
-        if GridCaseSurface.__custom_init__ is not None:
-            GridCaseSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GridSummaryCase(SummaryCase):
-    """
-    A Summary Case based on extracting grid data.
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        SummaryCase.__init__(self, pb2_object, channel)
-        if GridSummaryCase.__custom_init__ is not None:
-            GridSummaryCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class IntersectionCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if IntersectionCollection.__custom_init__ is not None:
-            IntersectionCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellPath(PdmObjectBase):
-    """
-    A ResInsight Well Path
-
-    Attributes:
-        name (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.name = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if WellPath.__custom_init__ is not None:
-            WellPath.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def add_fracture(self, measured_depth=0, stim_plan_fracture_template="", align_dip=False, eclipse_case=""):
-        """
-        Add StimPlan Fracture
-
-        Arguments:
-            measured_depth (float): 
-            stim_plan_fracture_template (StimPlanFractureTemplate): StimPlan Fracture Template
-            align_dip (bool): 
-            eclipse_case (RimReservoir): Eclipse Case
-        Returns:
-            WellPathFracture
-        """
-        return self._call_pdm_method("AddFracture", measured_depth=measured_depth, stim_plan_fracture_template=stim_plan_fracture_template, align_dip=align_dip, eclipse_case=eclipse_case)
-
-
-    def add_thermal_fracture(self, measured_depth=0, fracture_template="", place_using_template_data=True):
-        """
-        Add Thermal Fracture
-
-        Arguments:
-            measured_depth (float): 
-            fracture_template (ThermalFractureTemplate): Thermal Fracture Template
-            place_using_template_data (bool): 
-        Returns:
-            WellPathFracture
-        """
-        return self._call_pdm_method("AddThermalFracture", measured_depth=measured_depth, fracture_template=fracture_template, place_using_template_data=place_using_template_data)
-
-
-    def append_perforation_interval(self, start_md=0, end_md=0, diameter=0, skin_factor=0):
-        """
-        Append Perforation Interval
-
-        Arguments:
-            start_md (float): Start Measured Depth
-            end_md (float): End Measured Depth
-            diameter (float): Diameter
-            skin_factor (float): Skin Factor
-        Returns:
-            Perforation
-        """
-        return self._call_pdm_method("AppendPerforationInterval", start_md=start_md, end_md=end_md, diameter=diameter, skin_factor=skin_factor)
-
-
-class ModeledWellPath(WellPath):
-    """
-    A Well Path created interactively in ResInsight
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        WellPath.__init__(self, pb2_object, channel)
-        if ModeledWellPath.__custom_init__ is not None:
-            ModeledWellPath.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def append_lateral(self, tie_in_depth=0, lateral_name=""):
-        """
-        Append Well Path Lateral
-
-        Arguments:
-            tie_in_depth (float): Measured Depth on the Parent Well Path
-            lateral_name (str): Lateral Name
-        Returns:
-            ModeledWellPath
-        """
-        return self._call_pdm_method("AppendLateral", tie_in_depth=tie_in_depth, lateral_name=lateral_name)
-
-
-    def well_path_geometry(self):
-        """Trajectory
-
-        Returns:
-             WellPathGeometry
-        """
-        children = self.children("WellPathGeometry", WellPathGeometry)
-        return children[0] if len(children) > 0 else None
-
-
-class NonNetLayers(PdmObjectBase):
-    """
-    Attributes:
-        cutoff (float): Cutoff
-        facies (str): Facies
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.cutoff = 0
-        self.facies = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if NonNetLayers.__custom_init__ is not None:
-            NonNetLayers.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def facies_definition(self):
-        """
-
-        Returns:
-             EclipseResult
-        """
-        children = self.children("FaciesDefinition", EclipseResult)
-        return children[0] if len(children) > 0 else None
-
-
-class PressureTable(PdmObjectBase):
-    """
-    Attributes:
-        pressure_date (str): Pressure Date
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.pressure_date = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if PressureTable.__custom_init__ is not None:
-            PressureTable.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def items(self):
-        """Pressure Table Items
-
-        Returns:
-             List of PressureTableItem
-        """
-        return self.children("Items", PressureTableItem)
-
-
-class PressureTableItem(PdmObjectBase):
-    """
-    Attributes:
-        depth (float): Depth TVDMSL [m]
-        initial_pressure (float): Initial Pressure [Bar]
-        pressure (float): Pressure [Bar]
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.depth = 0
-        self.initial_pressure = 0
-        self.pressure = 0
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if PressureTableItem.__custom_init__ is not None:
-            PressureTableItem.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GeoMechCase(Case):
-    """
-    The Abaqus Based GeoMech Case
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        Case.__init__(self, pb2_object, channel)
-        if GeoMechCase.__custom_init__ is not None:
-            GeoMechCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def views(self):
-        """All GeoMech Views in the Case
-
-        Returns:
-             List of GeoMechView
-        """
-        return self.children("Views", GeoMechView)
-
-
-class Project(PdmObjectBase):
-    """
-    The ResInsight Project
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if Project.__custom_init__ is not None:
-            Project.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def import_summary_case(self, file_name=""):
-        """
-        Import Summary Case
-
-        Arguments:
-            file_name (str): 
-        Returns:
-            FileSummaryCase
-        """
-        return self._call_pdm_method("importSummaryCase", file_name=file_name)
-
-
-    def summary_case(self, case_id=-1):
-        """
-        Find Summary Case
-
-        Arguments:
-            case_id (int): 
-        Returns:
-            FileSummaryCase
-        """
-        return self._call_pdm_method("summaryCase", case_id=case_id)
-
-
-    def surface_folder(self, folder_name=""):
-        """
-        Get Surface Folder
-
-        Arguments:
-            folder_name (str): 
-        Returns:
-            SurfaceCollection
-        """
-        return self._call_pdm_method("surfaceFolder", folder_name=folder_name)
-
-
-class ResampleData(PdmObjectBase):
-    """
-    Attributes:
-        time_steps (List of time): Time Steps
-        values (List of float): Values
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.time_steps = []
-        self.values = []
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if ResampleData.__custom_init__ is not None:
-            ResampleData.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class EclipseView(View):
-    """
-    The Eclipse 3d Reservoir View
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        View.__init__(self, pb2_object, channel)
-        if EclipseView.__custom_init__ is not None:
-            EclipseView.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def cell_result(self):
-        """Cell Result
-
-        Returns:
-             CellColors
-        """
-        children = self.children("CellResult", CellColors)
-        return children[0] if len(children) > 0 else None
-
-
-    def cell_result_data(self):
-        """Current Eclipse Cell Result
-
-        Returns:
-             str
-        """
-        return self._call_get_method("CellResultData")
-
-
-    def set_cell_result_data(self, values):
-        """Set Current Eclipse Cell Result
-
-        Arguments:
-            values (str): data
-        """
-        self._call_set_method("CellResultData", values)
-
-
-class EclipseResult(PdmObjectBase):
-    """
-    An eclipse result definition
-
-    Attributes:
-        flow_tracer_selection_mode (str): One of [FLOW_TR_INJ_AND_PROD, FLOW_TR_PRODUCERS, FLOW_TR_INJECTORS, FLOW_TR_BY_SELECTION]
-        phase_selection (str): One of [PHASE_ALL, PHASE_OIL, PHASE_GAS, PHASE_WAT]
-        porosity_model_type (str): One of [MATRIX_MODEL, FRACTURE_MODEL]
-        result_type (str): One of [DYNAMIC_NATIVE, STATIC_NATIVE, SOURSIMRL, GENERATED, INPUT_PROPERTY, FORMATION_NAMES, ALLAN_DIAGRAMS, FLOW_DIAGNOSTICS, INJECTION_FLOODING]
-        result_variable (str): Variable
-        selected_injector_tracers (List of str): Injector Tracers
-        selected_producer_tracers (List of str): Producer Tracers
-        selected_souring_tracers (List of str): Tracers
-        show_only_visible_categories_in_legend (bool): Show Only Visible Categories In Legend
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.flow_tracer_selection_mode = "FLOW_TR_INJ_AND_PROD"
-        self.phase_selection = "PHASE_ALL"
-        self.porosity_model_type = "MATRIX_MODEL"
-        self.result_type = "DYNAMIC_NATIVE"
-        self.result_variable = "None"
-        self.selected_injector_tracers = []
-        self.selected_producer_tracers = []
-        self.selected_souring_tracers = []
-        self.show_only_visible_categories_in_legend = True
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if EclipseResult.__custom_init__ is not None:
-            EclipseResult.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class CellColors(EclipseResult):
-    """
-    Eclipse Cell Colors class
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        EclipseResult.__init__(self, pb2_object, channel)
-        if CellColors.__custom_init__ is not None:
-            CellColors.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class CommandRouter(PdmObjectBase):
-    """
-    The CommandRouter is used to call code independent to the project
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if CommandRouter.__custom_init__ is not None:
-            CommandRouter.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def extract_surfaces(self, grid_model_filename="", layers=[], minimum_i=-1, maximum_i=-1, minimum_j=-1, maximum_j=-1):
-        """
-        Extract Layer Surface
-
-        Arguments:
-            grid_model_filename (str): 
-            layers (List of int): 
-            minimum_i (int): 
-            maximum_i (int): 
-            minimum_j (int): 
-            maximum_j (int): 
-        Returns:
-            
-        """
-        return self._call_pdm_method("ExtractSurfaces", grid_model_filename=grid_model_filename, layers=layers, minimum_i=minimum_i, maximum_i=maximum_i, minimum_j=minimum_j, maximum_j=maximum_j)
-
-
-class EclipseContourMap(EclipseView):
-    """
-    A contour map for Eclipse cases
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        EclipseView.__init__(self, pb2_object, channel)
-        if EclipseContourMap.__custom_init__ is not None:
-            EclipseContourMap.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GeoMechContourMap(GeoMechView):
-    """
-    A contour map for GeoMech cases
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        GeoMechView.__init__(self, pb2_object, channel)
-        if GeoMechContourMap.__custom_init__ is not None:
-            GeoMechContourMap.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class GridCaseGroup(PdmObjectBase):
-    """
-    A statistics case group
-
-    Attributes:
-        group_id (int): Case Group ID
-        user_description (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.group_id = -1
-        self.user_description = "Grid Case Group"
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if GridCaseGroup.__custom_init__ is not None:
-            GridCaseGroup.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class MudWeightWindowParameters(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if MudWeightWindowParameters.__custom_init__ is not None:
-            MudWeightWindowParameters.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class FractureTemplate(PdmObjectBase):
-    """
-    Attributes:
-        azimuth_angle (float): Azimuth Angle
-        conductivity_factor (float): Conductivity
-        conductivity_type (str): One of [InfiniteConductivity, FiniteConductivity]
-        d_factor_scale_factor (float): D-factor
-        height_scale_factor (float): Height
-        orientation (str): One of [Azimuth, Longitudinal, Transverse]
-        perforation_length (float): Perforation Length
-        user_defined_perforation_length (bool): User-defined Perforation Length
-        user_description (str): Name
-        width_scale_factor (float): Half Length
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.azimuth_angle = 0
-        self.conductivity_factor = 1
-        self.conductivity_type = "FiniteConductivity"
-        self.d_factor_scale_factor = 1
-        self.height_scale_factor = 1
-        self.orientation = "Transverse"
-        self.perforation_length = 1
-        self.user_defined_perforation_length = False
-        self.user_description = "Fracture Template"
-        self.width_scale_factor = 1
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if FractureTemplate.__custom_init__ is not None:
-            FractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def set_scale_factors(self, half_length=1, height=1, d_factor=1, conductivity=1):
-        """
-        Set Fracture Template Scale Factors.
-
-        Arguments:
-            half_length (float): 
-            height (float): 
-            d_factor (float): 
-            conductivity (float): 
-        Returns:
-            
-        """
-        return self._call_pdm_method("SetScaleFactors", half_length=half_length, height=height, d_factor=d_factor, conductivity=conductivity)
-
-
-class MeshFractureTemplate(FractureTemplate):
-    """
-    Attributes:
-        active_time_step_index (int): Active TimeStep Index
-        conductivity_result_name (str): Active Conductivity Result Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.active_time_step_index = 0
-        self.conductivity_result_name = ""
-        FractureTemplate.__init__(self, pb2_object, channel)
-        if MeshFractureTemplate.__custom_init__ is not None:
-            MeshFractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class StimPlanFractureTemplate(MeshFractureTemplate):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        MeshFractureTemplate.__init__(self, pb2_object, channel)
-        if StimPlanFractureTemplate.__custom_init__ is not None:
-            StimPlanFractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class StimPlanModel(CheckableNamedObject):
-    """
-    Attributes:
-        anchor_position (str): Anchor Position
-        auto_compute_barrier (bool): Auto Compute Barrier
-        azimuth_angle (float): Azimuth Angle
-        barrier (bool): Barrier
-        barrier_dip (float): Barrier Dip
-        barrier_fault_name (str): Barrier Fault
-        barrier_text_annotation (str): Barrier Text Annotation
-        bounding_box_horizontal (float): Bounding Box Horizontal
-        bounding_box_vertical (float): Bounding Box Vertical
-        distance_to_barrier (float): Distance To Barrier [m]
-        eclipse_case (str): Dynamic Case
-        extraction_depth_bottom (float): Depth
-        extraction_depth_top (float): Depth
-        extraction_offset_bottom (float): Bottom Offset
-        extraction_offset_top (float): Top Offset
-        extraction_type (str): One of [TVT, TST]
-        formation_dip (float): Formation Dip
-        fracture_orientation (str): One of [Longitudinal, Transverse, Azimuth]
-        initial_pressure_eclipse_case (str): Initial Pressure Case
-        measured_depth (float): Measured Depth
-        original_thickness_direction (str): Original Thickness Direction
-        perforation_interval (str): Perforation Interval
-        perforation_length (float): Perforation Length [m]
-        poro_elastic_constant (float): Poro-Elastic Constant
-        relative_permeability_factor (float): Relative Permeability Factor
-        show_all_faults (bool): Show All Faults
-        show_only_barrier_fault (bool): Show Only Barrier Fault
-        static_eclipse_case (str): Static Case
-        thermal_expansion_coefficient (float): Thermal Expansion Coefficient [1/C]
-        thickness_direction (str): Thickness Direction
-        thickness_direction_well_path (str): Thickness Direction Well Path
-        time_step (int): Time Step
-        use_detailed_fluid_loss (bool): Use Detailed Fluid Loss
-        well_penetration_layer (int): Well Penetration Layer
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.anchor_position = [0, 0, 0]
-        self.auto_compute_barrier = True
-        self.azimuth_angle = 0
-        self.barrier = True
-        self.barrier_dip = 0
-        self.barrier_fault_name = ""
-        self.barrier_text_annotation = ""
-        self.bounding_box_horizontal = 50
-        self.bounding_box_vertical = 100
-        self.distance_to_barrier = 0
-        self.eclipse_case = ""
-        self.extraction_depth_bottom = -1
-        self.extraction_depth_top = -1
-        self.extraction_offset_bottom = -1
-        self.extraction_offset_top = -1
-        self.extraction_type = "TST"
-        self.formation_dip = 0
-        self.fracture_orientation = "Longitudinal"
-        self.initial_pressure_eclipse_case = ""
-        self.measured_depth = 0
-        self.original_thickness_direction = [0, 0, 0]
-        self.perforation_interval = ""
-        self.perforation_length = 10
-        self.poro_elastic_constant = 0
-        self.relative_permeability_factor = 0.5
-        self.show_all_faults = False
-        self.show_only_barrier_fault = False
-        self.static_eclipse_case = ""
-        self.thermal_expansion_coefficient = 0
-        self.thickness_direction = [0, 0, 0]
-        self.thickness_direction_well_path = ""
-        self.time_step = 0
-        self.use_detailed_fluid_loss = True
-        self.well_penetration_layer = 2
-        CheckableNamedObject.__init__(self, pb2_object, channel)
-        if StimPlanModel.__custom_init__ is not None:
-            StimPlanModel.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def export_to_file(self, directory_path=""):
-        """
-        Export StimPlan Model Plot to File
-
-        Arguments:
-            directory_path (str): Directory Path
-        Returns:
-            StimPlanModel
-        """
-        return self._call_pdm_method("ExportToFile", directory_path=directory_path)
-
-
-class StimPlanModelCollection(CheckableNamedObject):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        CheckableNamedObject.__init__(self, pb2_object, channel)
-        if StimPlanModelCollection.__custom_init__ is not None:
-            StimPlanModelCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def append_stim_plan_model(self, well_path="", measured_depth=0, stim_plan_model_template=""):
-        """
-        Create a new StimPlan Model
-
-        Arguments:
-            well_path (WellPathBase): Well Path
-            measured_depth (float): 
-            stim_plan_model_template (StimPlanModelTemplate): StimPlan Model Template
-        Returns:
-            StimPlanModel
-        """
-        return self._call_pdm_method("AppendStimPlanModel", well_path=well_path, measured_depth=measured_depth, stim_plan_model_template=stim_plan_model_template)
-
-
-    def stim_plan_models(self):
-        """
-
-        Returns:
-             List of StimPlanModel
-        """
-        return self.children("StimPlanModels", StimPlanModel)
-
-
-class PlotWindow(ViewWindow):
-    """
-    The Abstract base class for all MDI Windows in the Plot Window
-
-    Attributes:
-        id (int): View ID
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.id = -1
-        ViewWindow.__init__(self, pb2_object, channel)
-        if PlotWindow.__custom_init__ is not None:
-            PlotWindow.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class DepthTrackPlot(PlotWindow):
-    """
-    Attributes:
-        auto_scale_depth_enabled (bool): Auto Scale
-        auto_zoom_max_depth_factor (float): Auto Zoom Maximum Factor
-        auto_zoom_min_depth_factor (float): Auto Zoom Minimum Factor
-        axis_title_font_size (str): One of [XX_Small, X_Small, Small, Medium, Large, X_Large, XX_Large]
-        axis_value_font_size (str): One of [XX_Small, X_Small, Small, Medium, Large, X_Large, XX_Large]
-        depth_type (str): One of [MEASURED_DEPTH, TRUE_VERTICAL_DEPTH, PSEUDO_LENGTH, CONNECTION_NUMBER, TRUE_VERTICAL_DEPTH_RKB]
-        depth_unit (str): One of [UNIT_METER, UNIT_FEET, UNIT_NONE]
-        maximum_depth (float): Max
-        minimum_depth (float): Min
-        show_depth_grid_lines (str): One of [GRID_X_NONE, GRID_X_MAJOR, GRID_X_MAJOR_AND_MINOR]
-        show_depth_marker_line (bool): Show Depth Marker Line
-        sub_title_font_size (str): One of [XX_Small, X_Small, Small, Medium, Large, X_Large, XX_Large]
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.auto_scale_depth_enabled = True
-        self.auto_zoom_max_depth_factor = 0
-        self.auto_zoom_min_depth_factor = 0
-        self.axis_title_font_size = "Medium"
-        self.axis_value_font_size = "Medium"
-        self.depth_type = "MEASURED_DEPTH"
-        self.depth_unit = "UNIT_METER"
-        self.maximum_depth = 1000
-        self.minimum_depth = 0
-        self.show_depth_grid_lines = "GRID_X_MAJOR"
-        self.show_depth_marker_line = False
-        self.sub_title_font_size = "Medium"
-        PlotWindow.__init__(self, pb2_object, channel)
-        if DepthTrackPlot.__custom_init__ is not None:
-            DepthTrackPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class StimPlanModelPlot(DepthTrackPlot):
-    """
-    A fracture model plot
-
-    Attributes:
-        eclipse_case (str): Case
-        stim_plan_model (str): StimPlan Model
-        time_step (int): Time Step
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.eclipse_case = ""
-        self.stim_plan_model = ""
-        self.time_step = 0
-        DepthTrackPlot.__init__(self, pb2_object, channel)
-        if StimPlanModelPlot.__custom_init__ is not None:
-            StimPlanModelPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class StimPlanModelPlotCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if StimPlanModelPlotCollection.__custom_init__ is not None:
-            StimPlanModelPlotCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def append_stim_plan_model_plot(self, stim_plan_model=""):
-        """
-        Create a new StimPlan Model
-
-        Arguments:
-            stim_plan_model (StimPlanModel): StimPlan Model
-        Returns:
-            StimPlanModelPlot
-        """
-        return self._call_pdm_method("AppendStimPlanModelPlot", stim_plan_model=stim_plan_model)
-
-
-    def stim_plan_model_plots(self):
-        """
-
-        Returns:
-             List of StimPlanModelPlot
-        """
-        return self.children("StimPlanModelPlots", StimPlanModelPlot)
-
-
-class StimPlanModelTemplate(NamedObject):
-    """
-    Attributes:
-        default_facies (str): Default Facies
-        default_permeability (float): Default Permeability
-        default_porosity (float): Default Porosity
-        dynamic_eclipse_case (str): Dynamic Case
-        id (int): ID
-        initial_pressure_eclipse_case (str): Initial Pressure Case
-        overburden_facies (str): Overburden Facies
-        overburden_fluid_density (float): Overburden Fluid Density [g/cm^3]
-        overburden_formation (str): Overburden Formation
-        overburden_height (float): Overburden Height
-        overburden_permeability (float): Overburden Permeability
-        overburden_porosity (float): Overburden Porosity
-        reference_temperature (float): Temperature [C]
-        reference_temperature_depth (float): Temperature Depth [m]
-        reference_temperature_gradient (float): Temperature Gradient [C/m]
-        static_eclipse_case (str): Static Case
-        stress_depth (float): Stress Depth
-        time_step (int): Time Step
-        underburden_facies (str): Underburden Facies
-        underburden_fluid_density (float): Underburden Fluid Density [g/cm^3]
-        underburden_formation (str): Underburden Formation
-        underburden_height (float): Underburden Height
-        underburden_permeability (float): Underburden Permeability
-        underburden_porosity (float): Underburden Porosity
-        vertical_stress (float): Vertical Stress
-        vertical_stress_gradient (float): Vertical Stress Gradient
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.default_facies = ""
-        self.default_permeability = 0.0001
-        self.default_porosity = 0.01
-        self.dynamic_eclipse_case = ""
-        self.id = -1
-        self.initial_pressure_eclipse_case = ""
-        self.overburden_facies = ""
-        self.overburden_fluid_density = 1.03
-        self.overburden_formation = ""
-        self.overburden_height = 50
-        self.overburden_permeability = 1e-05
-        self.overburden_porosity = 0
-        self.reference_temperature = 70
-        self.reference_temperature_depth = 2500
-        self.reference_temperature_gradient = 0.025
-        self.static_eclipse_case = ""
-        self.stress_depth = 1000
-        self.time_step = 0
-        self.underburden_facies = ""
-        self.underburden_fluid_density = 1.03
-        self.underburden_formation = ""
-        self.underburden_height = 50
-        self.underburden_permeability = 1e-05
-        self.underburden_porosity = 0
-        self.vertical_stress = 238
-        self.vertical_stress_gradient = 0.238
-        NamedObject.__init__(self, pb2_object, channel)
-        if StimPlanModelTemplate.__custom_init__ is not None:
-            StimPlanModelTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def elastic_properties(self):
-        """Elastic Properties
-
-        Returns:
-             ElasticProperties
-        """
-        children = self.children("ElasticProperties", ElasticProperties)
-        return children[0] if len(children) > 0 else None
-
-
-    def facies_initial_pressure_configs(self):
-        """Facies Initial Pressure Configs
-
-        Returns:
-             List of FaciesInitialPressureConfig
-        """
-        return self.children("FaciesInitialPressureConfigs", FaciesInitialPressureConfig)
-
-
-    def facies_properties(self):
-        """Facies Properties
-
-        Returns:
-             FaciesProperties
-        """
-        children = self.children("FaciesProperties", FaciesProperties)
-        return children[0] if len(children) > 0 else None
-
-
-    def non_net_layers(self):
-        """Non-Net Layers
-
-        Returns:
-             NonNetLayers
-        """
-        children = self.children("NonNetLayers", NonNetLayers)
-        return children[0] if len(children) > 0 else None
-
-
-    def pressure_table(self):
-        """Pressure Table
-
-        Returns:
-             PressureTable
-        """
-        children = self.children("PressureTable", PressureTable)
-        return children[0] if len(children) > 0 else None
-
-
-class StimPlanModelTemplateCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if StimPlanModelTemplateCollection.__custom_init__ is not None:
-            StimPlanModelTemplateCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def append_stim_plan_model_template(self, eclipse_case="", time_step=0, facies_properties_file_path="", elastic_properties_file_path=""):
-        """
-        Create a new StimPlan Model Template
-
-        Arguments:
-            eclipse_case (RimReservoir): Eclipse Case
-            time_step (int): Time Step
-            facies_properties_file_path (str): Facies Properties File Path
-            elastic_properties_file_path (str): Elastic Properties File Path
-        Returns:
-            StimPlanModelTemplate
-        """
-        return self._call_pdm_method("AppendStimPlanModelTemplate", eclipse_case=eclipse_case, time_step=time_step, facies_properties_file_path=facies_properties_file_path, elastic_properties_file_path=elastic_properties_file_path)
-
-
-    def stim_plan_model_templates(self):
-        """StimPlan Model Templates
-
-        Returns:
-             List of StimPlanModelTemplate
-        """
-        return self.children("StimPlanModelTemplates", StimPlanModelTemplate)
-
-
-class SummaryCaseSubCollection(PdmObjectBase):
-    """
-    Attributes:
-        create_auto_name (bool): Auto Name
-        id (int): Ensemble ID
-        is_ensemble (bool): Is Ensemble
-        name_count (str): Name
-        summary_collection_name (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.create_auto_name = True
-        self.id = -1
-        self.is_ensemble = False
-        self.name_count = "Group"
-        self.summary_collection_name = "Group"
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if SummaryCaseSubCollection.__custom_init__ is not None:
-            SummaryCaseSubCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class Plot(PlotWindow):
-    """
-    The Abstract Base Class for all Plot Objects
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PlotWindow.__init__(self, pb2_object, channel)
-        if Plot.__custom_init__ is not None:
-            Plot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class SummaryPlot(Plot):
-    """
-    A Summary Plot
-
-    Attributes:
-        is_using_auto_name (bool): Auto Title
-        normalize_curve_y_values (bool): Normalize all curves
-        plot_description (str): Name
-        use_qt_charts_plot (bool): Use Qt Charts
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.is_using_auto_name = True
-        self.normalize_curve_y_values = False
-        self.plot_description = "Summary Plot"
-        self.use_qt_charts_plot = False
-        Plot.__init__(self, pb2_object, channel)
-        if SummaryPlot.__custom_init__ is not None:
-            SummaryPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class SummaryPlotCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if SummaryPlotCollection.__custom_init__ is not None:
-            SummaryPlotCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def new_summary_plot(self, summary_cases=[], ensemble="", address=""):
-        """
-        Create a new Summary Plot
-
-        Arguments:
-            summary_cases (List of SummaryCase): Summary Cases
-            ensemble (SummaryCaseSubCollection): Ensemble
-            address (str): Formatted address string specifying the plot options
-        Returns:
-            SummaryPlot
-        """
-        return self._call_pdm_method("NewSummaryPlot", summary_cases=summary_cases, ensemble=ensemble, address=address)
-
-
-class Surface(SurfaceInterface):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        SurfaceInterface.__init__(self, pb2_object, channel)
-        if Surface.__custom_init__ is not None:
-            Surface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class ThermalFractureTemplate(MeshFractureTemplate):
-    """
-    Attributes:
-        filter_cake_pressure_drop (str): One of [None, Relative, Absolute]
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.filter_cake_pressure_drop = "Relative"
-        MeshFractureTemplate.__init__(self, pb2_object, channel)
-        if ThermalFractureTemplate.__custom_init__ is not None:
-            ThermalFractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def export_to_file(self, file_path="", time_step=0):
-        """
-        Export Thermal Fracture Template to File
-
-        Arguments:
-            file_path (str): File Path
-            time_step (int): 
-        Returns:
-            ThermalFractureTemplate
-        """
-        return self._call_pdm_method("ExportToFile", file_path=file_path, time_step=time_step)
-
-
-    def time_steps(self, ):
-        """
-        Get Thermal Fracture Template Time Steps
-
-        Arguments:
-            
-        Returns:
-            DataContainerString
-        """
-        return self._call_pdm_method("TimeSteps")
-
-
-class TriangleGeometry(PdmObjectBase):
-    """
-    Attributes:
-        connections (List of int): Indices to triangle vertices
-        display_model_offset (str): Display Model Offset
-        fault_mesh_x_coords (List of float): Fault Mesh X coords
-        fault_mesh_y_coords (List of float): Fault Mesh Y coords
-        fault_mesh_z_coords (List of float): Fault Mesh Z coords
-        mesh_x_coords (List of float): Mesh X coords
-        mesh_y_coords (List of float): Mesh Y coords
-        mesh_z_coords (List of float): Mesh Z coords
-        x_coords (List of float): X coords
-        y_coords (List of float): Y coords
-        z_coords (List of float): Z coords
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.connections = []
-        self.display_model_offset = [0, 0, 0]
-        self.fault_mesh_x_coords = []
-        self.fault_mesh_y_coords = []
-        self.fault_mesh_z_coords = []
-        self.mesh_x_coords = []
-        self.mesh_y_coords = []
-        self.mesh_z_coords = []
-        self.x_coords = []
-        self.y_coords = []
-        self.z_coords = []
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if TriangleGeometry.__custom_init__ is not None:
-            TriangleGeometry.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WbsParameters(PdmObjectBase):
-    """
-    Attributes:
-        df_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        fg_multiplier (float): SH Multiplier for FG in Shale
-        fg_shale_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        k0_fg_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        k0_sh_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        obg0_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        poission_ratio_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        pore_pressure_non_reservoir_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        pore_pressure_reservoir_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        ucs_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
-        user_df (float): User Defined DF
-        user_k0_fg (float): User Defined K0_FG
-        user_k0_sh (float): User Defined K0_SH
-        user_poisson_ratio (float): User Defined Poisson Ratio
-        user_pp_non_reservoir (float):   Multiplier of hydrostatic PP
-        user_ucs (float): User Defined UCS [bar]
-        water_density (float): Density of Sea Water [g/cm^3]
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.df_source = "LAS_FILE"
-        self.fg_multiplier = 1.05
-        self.fg_shale_source = "DERIVED_FROM_K0FG"
-        self.k0_fg_source = "LAS_FILE"
-        self.k0_sh_source = "LAS_FILE"
-        self.obg0_source = "GRID"
-        self.poission_ratio_source = "LAS_FILE"
-        self.pore_pressure_non_reservoir_source = "LAS_FILE"
-        self.pore_pressure_reservoir_source = "GRID"
-        self.ucs_source = "LAS_FILE"
-        self.user_df = 0.7
-        self.user_k0_fg = 0.75
-        self.user_k0_sh = 0.65
-        self.user_poisson_ratio = 0.35
-        self.user_pp_non_reservoir = 1
-        self.user_ucs = 100
-        self.water_density = 1.03
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if WbsParameters.__custom_init__ is not None:
-            WbsParameters.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class SimulationWell(PdmObjectBase):
-    """
-    An Eclipse Simulation Well
-
-    Attributes:
-        name (str): Name
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.name = ""
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if SimulationWell.__custom_init__ is not None:
-            SimulationWell.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellLogPlot(DepthTrackPlot):
-    """
-    A Well Log Plot With a shared Depth Axis and Multiple Tracks
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        DepthTrackPlot.__init__(self, pb2_object, channel)
-        if WellLogPlot.__custom_init__ is not None:
-            WellLogPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def new_well_log_track(self, title="", case="", well_path=""):
-        """
-        Create a new well log track
-
-        Arguments:
-            title (str): Title
-            case (RimReservoir): Case
-            well_path (WellPathBase): Well Path
-        Returns:
-            WellLogPlotTrack
-        """
-        return self._call_pdm_method("NewWellLogTrack", title=title, case=case, well_path=well_path)
-
-
-class WellBoreStabilityPlot(WellLogPlot):
-    """
-    A GeoMechanical Well Bore Stability Plot
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        WellLogPlot.__init__(self, pb2_object, channel)
-        if WellBoreStabilityPlot.__custom_init__ is not None:
-            WellBoreStabilityPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def parameters(self):
-        """Well Bore Stability Parameters
-
-        Returns:
-             WbsParameters
-        """
-        children = self.children("Parameters", WbsParameters)
-        return children[0] if len(children) > 0 else None
-
-
-class PlotCurve(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if PlotCurve.__custom_init__ is not None:
-            PlotCurve.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellLogPlotCurve(PlotCurve):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PlotCurve.__init__(self, pb2_object, channel)
-        if WellLogPlotCurve.__custom_init__ is not None:
-            WellLogPlotCurve.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellLogExtractionCurve(WellLogPlotCurve):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        WellLogPlotCurve.__init__(self, pb2_object, channel)
-        if WellLogExtractionCurve.__custom_init__ is not None:
-            WellLogExtractionCurve.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellLogPlotCollection(PdmObjectBase):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if WellLogPlotCollection.__custom_init__ is not None:
-            WellLogPlotCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def new_well_log_plot(self, case="", well_path="", property_type="", property_name="", time_step=0):
-        """
-        Create a new well log plot
-
-        Arguments:
-            case (RimReservoir): Case
-            well_path (WellPathBase): Well Path
-            property_type (str): Property Type
-            property_name (str): Property Name
-            time_step (int): Time Step
-        Returns:
-            WellLogPlot
-        """
-        return self._call_pdm_method("NewWellLogPlot", case=case, well_path=well_path, property_type=property_type, property_name=property_name, time_step=time_step)
-
-
-    def well_log_plots(self):
-        """
-
-        Returns:
-             List of WellLogPlot
-        """
-        return self.children("WellLogPlots", WellLogPlot)
-
-
-class WellLogPlotTrack(Plot):
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        Plot.__init__(self, pb2_object, channel)
-        if WellLogPlotTrack.__custom_init__ is not None:
-            WellLogPlotTrack.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def add_extraction_curve(self, case="", well_path="", property_type="", property_name="", time_step=0):
-        """
-        Create a well log extraction curve
-
-        Arguments:
-            case (RimReservoir): Case
-            well_path (WellPathBase): Well Path
-            property_type (str): Property Type
-            property_name (str): Property Name
-            time_step (int): Time Step
-        Returns:
-            WellLogExtractionCurve
-        """
-        return self._call_pdm_method("AddExtractionCurve", case=case, well_path=well_path, property_type=property_type, property_name=property_name, time_step=time_step)
-
-
-class FileWellPath(WellPath):
-    """
-    Well Paths Loaded From File
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        WellPath.__init__(self, pb2_object, channel)
-        if FileWellPath.__custom_init__ is not None:
-            FileWellPath.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellPathGeometry(PdmObjectBase):
-    """
-    Class containing the geometry of a modeled Well Path
-
-    Attributes:
-        air_gap (float): Air Gap
-        attached_to_parent_well (bool): Attached to Parent Well
-        link_reference_point_updates (bool): Link Reference Point
-        md_at_first_target (float): MD at First Target
-        reference_point (str): UTM Reference Point
-        show_spheres (bool): Spheres
-        use_auto_generated_target_at_sea_level (bool): Generate Target at Sea Level
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.air_gap = 0
-        self.attached_to_parent_well = False
-        self.link_reference_point_updates = False
-        self.md_at_first_target = 0
-        self.reference_point = [0, 0, 0]
-        self.show_spheres = True
-        self.use_auto_generated_target_at_sea_level = True
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if WellPathGeometry.__custom_init__ is not None:
-            WellPathGeometry.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def append_well_target(self, coordinate=[0, 0, 0], absolute=False, use_fixed_azimuth=False, use_fixed_inclination=False, fixed_azimuth_value=0, fixed_inclination_value=0):
-        """
-        Create and Add New Well Target
-
-        Arguments:
-            coordinate (class cvf::Vector3<double>): Coordinate
-            absolute (bool): Relative or Absolute Coordinate
-            use_fixed_azimuth (bool): 
-            use_fixed_inclination (bool): 
-            fixed_azimuth_value (float): [Degrees]
-            fixed_inclination_value (float): [Degrees]
-        Returns:
-            WellPathTarget
-        """
-        return self._call_pdm_method("AppendWellTarget", coordinate=coordinate, absolute=absolute, use_fixed_azimuth=use_fixed_azimuth, use_fixed_inclination=use_fixed_inclination, fixed_azimuth_value=fixed_azimuth_value, fixed_inclination_value=fixed_inclination_value)
-
-
-    def auto_generated_target(self):
-        """Auto Generated Target
-
-        Returns:
-             WellPathTarget
-        """
-        children = self.children("AutoGeneratedTarget", WellPathTarget)
-        return children[0] if len(children) > 0 else None
-
-
-    def well_path_targets(self):
-        """Well Targets
-
-        Returns:
-             List of WellPathTarget
-        """
-        return self.children("WellPathTargets", WellPathTarget)
-
-
-class WellPathTarget(PdmObjectBase):
-    """
-    Class containing the Well Target definition
-
-    Attributes:
-        azimuth (float): Azi(deg)
-        dogleg1 (float): DL in
-        dogleg2 (float): DL out
-        estimated_azimuth (float): Est Azi(deg)
-        estimated_dogleg1 (float): Est DL in
-        estimated_dogleg2 (float): Est DL out
-        estimated_inclination (float): Est Inc(deg)
-        inclination (float): Inc(deg)
-        target_measured_depth (float): MD
-        target_point (str): Relative Coord
-        use_fixed_azimuth (bool): Azi
-        use_fixed_inclination (bool): Inc
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        self.azimuth = 0
-        self.dogleg1 = 3
-        self.dogleg2 = 3
-        self.estimated_azimuth = 0
-        self.estimated_dogleg1 = 0
-        self.estimated_dogleg2 = 0
-        self.estimated_inclination = 0
-        self.inclination = 0
-        self.target_measured_depth = 0
-        self.target_point = [0, 0, 0]
-        self.use_fixed_azimuth = False
-        self.use_fixed_inclination = False
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if WellPathTarget.__custom_init__ is not None:
-            WellPathTarget.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-class WellPathCollection(PdmObjectBase):
-    """
-    Collection of Well Paths
-
-    """
-    __custom_init__ = None #: Assign a custom init routine to be run at __init__
-
-    def __init__(self, pb2_object=None, channel=None):
-        PdmObjectBase.__init__(self, pb2_object, channel)
-        if WellPathCollection.__custom_init__ is not None:
-            WellPathCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
-
-    def well_paths(self):
-        """Well Paths
-
-        Returns:
-             List of WellPath
-        """
-        return self.children("WellPaths", WellPath)
-
-
-def class_dict():
-    classes = {}
-    classes['Case'] = Case
-    classes['CellColors'] = CellColors
-    classes['CellFilterCollection'] = CellFilterCollection
-    classes['CheckableNamedObject'] = CheckableNamedObject
-    classes['CommandRouter'] = CommandRouter
-    classes['CurveIntersection'] = CurveIntersection
-    classes['DataContainerFloat'] = DataContainerFloat
-    classes['DataContainerString'] = DataContainerString
-    classes['DataContainerTime'] = DataContainerTime
-    classes['DepthTrackPlot'] = DepthTrackPlot
-    classes['EclipseCase'] = EclipseCase
-    classes['EclipseContourMap'] = EclipseContourMap
-    classes['EclipseResult'] = EclipseResult
-    classes['EclipseView'] = EclipseView
-    classes['ElasticProperties'] = ElasticProperties
-    classes['ElasticPropertyScaling'] = ElasticPropertyScaling
-    classes['ElasticPropertyScalingCollection'] = ElasticPropertyScalingCollection
-    classes['EnsembleStatisticsSurface'] = EnsembleStatisticsSurface
-    classes['EnsembleSurface'] = EnsembleSurface
-    classes['EnsembleWellLogs'] = EnsembleWellLogs
-    classes['FaciesInitialPressureConfig'] = FaciesInitialPressureConfig
-    classes['FaciesProperties'] = FaciesProperties
-    classes['FileSummaryCase'] = FileSummaryCase
-    classes['FileWellPath'] = FileWellPath
-    classes['FractureTemplate'] = FractureTemplate
-    classes['FractureTemplateCollection'] = FractureTemplateCollection
-    classes['GeoMechCase'] = GeoMechCase
-    classes['GeoMechContourMap'] = GeoMechContourMap
-    classes['GeoMechPart'] = GeoMechPart
-    classes['GeoMechPartCollection'] = GeoMechPartCollection
-    classes['GeoMechView'] = GeoMechView
-    classes['GridCaseGroup'] = GridCaseGroup
-    classes['GridCaseSurface'] = GridCaseSurface
-    classes['GridSummaryCase'] = GridSummaryCase
-    classes['IntersectionCollection'] = IntersectionCollection
-    classes['MeshFractureTemplate'] = MeshFractureTemplate
-    classes['ModeledWellPath'] = ModeledWellPath
-    classes['MudWeightWindowParameters'] = MudWeightWindowParameters
-    classes['NamedObject'] = NamedObject
-    classes['NonNetLayers'] = NonNetLayers
-    classes['PdmObjectBase'] = PdmObjectBase
-    classes['Plot'] = Plot
-    classes['PlotCurve'] = PlotCurve
-    classes['PlotWindow'] = PlotWindow
-    classes['PressureTable'] = PressureTable
-    classes['PressureTableItem'] = PressureTableItem
-    classes['Project'] = Project
-    classes['ResampleData'] = ResampleData
-    classes['Reservoir'] = Reservoir
-    classes['SimulationWell'] = SimulationWell
-    classes['StimPlanFractureTemplate'] = StimPlanFractureTemplate
-    classes['StimPlanModel'] = StimPlanModel
-    classes['StimPlanModelCollection'] = StimPlanModelCollection
-    classes['StimPlanModelPlot'] = StimPlanModelPlot
-    classes['StimPlanModelPlotCollection'] = StimPlanModelPlotCollection
-    classes['StimPlanModelTemplate'] = StimPlanModelTemplate
-    classes['StimPlanModelTemplateCollection'] = StimPlanModelTemplateCollection
-    classes['SummaryCase'] = SummaryCase
-    classes['SummaryCaseSubCollection'] = SummaryCaseSubCollection
-    classes['SummaryPlot'] = SummaryPlot
-    classes['SummaryPlotCollection'] = SummaryPlotCollection
-    classes['Surface'] = Surface
-    classes['SurfaceCollection'] = SurfaceCollection
-    classes['SurfaceInterface'] = SurfaceInterface
-    classes['ThermalFractureTemplate'] = ThermalFractureTemplate
-    classes['TriangleGeometry'] = TriangleGeometry
-    classes['View'] = View
-    classes['ViewWindow'] = ViewWindow
-    classes['WbsParameters'] = WbsParameters
-    classes['WellBoreStabilityPlot'] = WellBoreStabilityPlot
-    classes['WellLogExtractionCurve'] = WellLogExtractionCurve
-    classes['WellLogPlot'] = WellLogPlot
-    classes['WellLogPlotCollection'] = WellLogPlotCollection
-    classes['WellLogPlotCurve'] = WellLogPlotCurve
-    classes['WellLogPlotTrack'] = WellLogPlotTrack
-    classes['WellPath'] = WellPath
-    classes['WellPathCollection'] = WellPathCollection
-    classes['WellPathGeometry'] = WellPathGeometry
-    classes['WellPathTarget'] = WellPathTarget
-    return classes
-
-def class_from_keyword(class_keyword):
-    all_classes = class_dict()
-    if class_keyword in all_classes.keys():
-        return all_classes[class_keyword]
-    return None
+from rips.pdmobject import PdmObjectBase
+class CellFilterCollection(PdmObjectBase):
+    """
+    Attributes:
+        active (bool): Active
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.active = True
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if CellFilterCollection.__custom_init__ is not None:
+            CellFilterCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class CurveIntersection(PdmObjectBase):
+    """
+    Attributes:
+        name (str): Name
+        points (List of str): Points
+        simulation_well (str): Simulation Well
+        type (str): One of [CS_WELL_PATH, CS_SIMULATION_WELL, CS_POLYLINE, CS_AZIMUTHLINE]
+        well_path (str): Well Path        
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.name = "Intersection Name"
+        self.points = []
+        self.simulation_well = ""
+        self.type = "CS_POLYLINE"
+        self.well_path = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if CurveIntersection.__custom_init__ is not None:
+            CurveIntersection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def geometry(self, geometry_type="FULL_3D"):
+        """
+        
+
+        Arguments:
+            geometry_type (str): One of [FULL_3D, PROJECTED_TO_PLANE]
+        Returns:
+            TriangleGeometry
+        """
+        return self._call_pdm_method("geometry", geometry_type=geometry_type)
+
+
+    def geometry_result(self, geometry_type="FULL_3D"):
+        """
+        
+
+        Arguments:
+            geometry_type (str): One of [FULL_3D, PROJECTED_TO_PLANE]
+        Returns:
+            DataContainerFloat
+        """
+        return self._call_pdm_method("geometryResult", geometry_type=geometry_type)
+
+
+class DataContainerFloat(PdmObjectBase):
+    """
+    Attributes:
+        values (List of float): Float Values
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.values = []
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if DataContainerFloat.__custom_init__ is not None:
+            DataContainerFloat.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class DataContainerString(PdmObjectBase):
+    """
+    Attributes:
+        values (List of str): String Values
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.values = []
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if DataContainerString.__custom_init__ is not None:
+            DataContainerString.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class DataContainerTime(PdmObjectBase):
+    """
+    Attributes:
+        values (List of time): Time Values
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.values = []
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if DataContainerTime.__custom_init__ is not None:
+            DataContainerTime.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class Case(PdmObjectBase):
+    """
+    The ResInsight base class for Cases
+
+    Attributes:
+        file_path (str): Case File Name
+        id (int): Case ID
+        name (str): Case Name
+        name_setting (str): One of [FULL_CASE_NAME, SHORT_CASE_NAME, CUSTOM_NAME]
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.file_path = ""
+        self.id = -1
+        self.name = ""
+        self.name_setting = "FULL_CASE_NAME"
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if Case.__custom_init__ is not None:
+            Case.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class Reservoir(Case):
+    """
+    Abstract base class for Eclipse Cases
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        Case.__init__(self, pb2_object, channel)
+        if Reservoir.__custom_init__ is not None:
+            Reservoir.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def import_properties(self, file_names=[]):
+        """
+        Import Properties
+
+        Arguments:
+            file_names (List of str): 
+        Returns:
+            
+        """
+        return self._call_pdm_method("import_properties", file_names=file_names)
+
+
+    def views(self):
+        """All Eclipse Views in the case
+
+        Returns:
+             List of EclipseView
+        """
+        return self.children("Views", EclipseView)
+
+
+class EclipseCase(Reservoir):
+    """
+    The Regular Eclipse Results Case
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        Reservoir.__init__(self, pb2_object, channel)
+        if EclipseCase.__custom_init__ is not None:
+            EclipseCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class ElasticProperties(PdmObjectBase):
+    """
+    Attributes:
+        file_path (str): File Path
+        properties_table (str): Properties Table
+        show_scaled_properties (bool): Show Scaled Properties
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.file_path = ""
+        self.properties_table = ""
+        self.show_scaled_properties = True
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if ElasticProperties.__custom_init__ is not None:
+            ElasticProperties.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def add_property_scaling(self, formation="", facies="", property="", scale=1):
+        """
+        Add Elastic Property Scaling
+
+        Arguments:
+            formation (str): Formation
+            facies (str): Facies
+            property (str): Property
+            scale (float): Scale
+        Returns:
+            ElasticPropertyScaling
+        """
+        return self._call_pdm_method("AddPropertyScaling", formation=formation, facies=facies, property=property, scale=scale)
+
+
+    def property_scaling_collection(self):
+        """PropertyScalingCollection
+
+        Returns:
+             ElasticPropertyScalingCollection
+        """
+        children = self.children("PropertyScalingCollection", ElasticPropertyScalingCollection)
+        return children[0] if len(children) > 0 else None
+
+
+class NamedObject(PdmObjectBase):
+    """
+    Attributes:
+        name (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.name = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if NamedObject.__custom_init__ is not None:
+            NamedObject.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class CheckableNamedObject(NamedObject):
+    """
+    Attributes:
+        is_checked (bool): Active
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.is_checked = True
+        NamedObject.__init__(self, pb2_object, channel)
+        if CheckableNamedObject.__custom_init__ is not None:
+            CheckableNamedObject.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class ElasticPropertyScaling(CheckableNamedObject):
+    """
+    Attributes:
+        facies (str): Facies
+        formation (str): Formation
+        property (str): One of [UNDEFINED, FACIES, LAYERS, POROSITY, PERMEABILITY_X, PERMEABILITY_Z, INITIAL_PRESSURE, PRESSURE, STRESS, INITIAL_STRESS, STRESS_GRADIENT, YOUNGS_MODULUS, POISSONS_RATIO, K_IC, PROPPANT_EMBEDMENT, BIOT_COEFFICIENT, K0, FLUID_LOSS_COEFFICIENT, SPURT_LOSS, TEMPERATURE, RELATIVE_PERMEABILITY_FACTOR, PORO_ELASTIC_CONSTANT, THERMAL_EXPANSION_COEFFICIENT, IMMOBILE_FLUID_SATURATION, NET_TO_GROSS, POROSITY_UNSCALED, EQLNUM, PRESSURE_GRADIENT, FORMATIONS]
+        scale (float): Scale
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.facies = ""
+        self.formation = ""
+        self.property = "YOUNGS_MODULUS"
+        self.scale = 1
+        CheckableNamedObject.__init__(self, pb2_object, channel)
+        if ElasticPropertyScaling.__custom_init__ is not None:
+            ElasticPropertyScaling.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class ElasticPropertyScalingCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if ElasticPropertyScalingCollection.__custom_init__ is not None:
+            ElasticPropertyScalingCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def elastic_property_scalings(self):
+        """Elastic Property Scalings
+
+        Returns:
+             List of ElasticPropertyScaling
+        """
+        return self.children("ElasticPropertyScalings", ElasticPropertyScaling)
+
+
+class SurfaceInterface(PdmObjectBase):
+    """
+    Attributes:
+        depth_offset (float): Depth Offset
+        surface_user_decription (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.depth_offset = 0
+        self.surface_user_decription = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if SurfaceInterface.__custom_init__ is not None:
+            SurfaceInterface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def export_to_file(self, file_name=""):
+        """
+        Export a surface to file
+
+        Arguments:
+            file_name (str): Filename to export surface to
+        Returns:
+            DataContainerString
+        """
+        return self._call_pdm_method("ExportToFile", file_name=file_name)
+
+
+class EnsembleStatisticsSurface(SurfaceInterface):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        SurfaceInterface.__init__(self, pb2_object, channel)
+        if EnsembleStatisticsSurface.__custom_init__ is not None:
+            EnsembleStatisticsSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class SurfaceCollection(PdmObjectBase):
+    """
+    Attributes:
+        surface_user_decription (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.surface_user_decription = "Surfaces"
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if SurfaceCollection.__custom_init__ is not None:
+            SurfaceCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def add_folder(self, folder_name="Surfaces"):
+        """
+        Add a new surface folder
+
+        Arguments:
+            folder_name (str): New surface folder name
+        Returns:
+            SurfaceCollection
+        """
+        return self._call_pdm_method("AddFolder", folder_name=folder_name)
+
+
+    def import_surface(self, file_name=""):
+        """
+        Import a new surface from file
+
+        Arguments:
+            file_name (str): Filename to import surface from
+        Returns:
+            Surface
+        """
+        return self._call_pdm_method("ImportSurface", file_name=file_name)
+
+
+    def new_surface(self, case="", k_index=0):
+        """
+        Create a new surface
+
+        Arguments:
+            case (Case): 
+            k_index (int): 
+        Returns:
+            GridCaseSurface
+        """
+        return self._call_pdm_method("NewSurface", case=case, k_index=k_index)
+
+
+    def sub_collections(self):
+        """Surfaces
+
+        Returns:
+             List of SurfaceCollection
+        """
+        return self.children("SubCollections", SurfaceCollection)
+
+
+    def surfaces_field(self):
+        """Surfaces
+
+        Returns:
+             List of SurfaceInterface
+        """
+        return self.children("SurfacesField", SurfaceInterface)
+
+
+class EnsembleSurface(SurfaceCollection):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        SurfaceCollection.__init__(self, pb2_object, channel)
+        if EnsembleSurface.__custom_init__ is not None:
+            EnsembleSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class EnsembleWellLogs(NamedObject):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        NamedObject.__init__(self, pb2_object, channel)
+        if EnsembleWellLogs.__custom_init__ is not None:
+            EnsembleWellLogs.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class FaciesInitialPressureConfig(PdmObjectBase):
+    """
+    Attributes:
+        facies_name (str): Facies
+        facies_value (int): Value
+        fraction (float): Δ Pressure Fraction
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.facies_name = ""
+        self.facies_value = -1
+        self.fraction = 0
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if FaciesInitialPressureConfig.__custom_init__ is not None:
+            FaciesInitialPressureConfig.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class FaciesProperties(PdmObjectBase):
+    """
+    Attributes:
+        color_legend (str): Colors
+        file_path (str): File Path
+        properties_table (str): Properties Table
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.color_legend = ""
+        self.file_path = ""
+        self.properties_table = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if FaciesProperties.__custom_init__ is not None:
+            FaciesProperties.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def facies_definition(self):
+        """
+
+        Returns:
+             EclipseResult
+        """
+        children = self.children("FaciesDefinition", EclipseResult)
+        return children[0] if len(children) > 0 else None
+
+
+class SummaryCase(PdmObjectBase):
+    """
+    The Base Class for all Summary Cases
+
+    Attributes:
+        auto_shorty_name (bool): Use Auto Display Name
+        id (int): Case ID
+        name_setting (str): One of [FULL_CASE_NAME, SHORT_CASE_NAME, CUSTOM_NAME]
+        short_name (str): Display Name
+        show_sub_nodes_in_tree (bool): Show Summary Data Sub-Tree
+        summary_header_filename (str): Summary Header File
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.auto_shorty_name = False
+        self.id = -1
+        self.name_setting = "FULL_CASE_NAME"
+        self.short_name = ""
+        self.show_sub_nodes_in_tree = False
+        self.summary_header_filename = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if SummaryCase.__custom_init__ is not None:
+            SummaryCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def available_addresses(self, ):
+        """
+        
+
+        Arguments:
+            
+        Returns:
+            DataContainerString
+        """
+        return self._call_pdm_method("availableAddresses")
+
+
+    def available_time_steps(self, ):
+        """
+        
+
+        Arguments:
+            
+        Returns:
+            DataContainerTime
+        """
+        return self._call_pdm_method("availableTimeSteps")
+
+
+    def resample_values(self, address="", resampling_period=""):
+        """
+        
+
+        Arguments:
+            address (str): Formatted address specifying the summary vector
+            resampling_period (str): Resampling Period
+        Returns:
+            ResampleData
+        """
+        return self._call_pdm_method("resampleValues", address=address, resampling_period=resampling_period)
+
+
+    def set_summary_values(self, address="", unit="", values=[]):
+        """
+        
+
+        Arguments:
+            address (str): Formatted address specifying the summary vector
+            unit (str): Unit
+            values (List of float): Values
+        Returns:
+            
+        """
+        return self._call_pdm_method("setSummaryValues", address=address, unit=unit, values=values)
+
+
+    def summary_vector_values(self, address=""):
+        """
+        Get all values for a summary vector
+
+        Arguments:
+            address (str): Formatted address specifying the summary vector
+        Returns:
+            DataContainerFloat
+        """
+        return self._call_pdm_method("summaryVectorValues", address=address)
+
+
+class FileSummaryCase(SummaryCase):
+    """
+    A Summary Case based on SMSPEC files
+
+    Attributes:
+        include_restart_files (bool): Include Restart Files
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.include_restart_files = False
+        SummaryCase.__init__(self, pb2_object, channel)
+        if FileSummaryCase.__custom_init__ is not None:
+            FileSummaryCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class FractureTemplateCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if FractureTemplateCollection.__custom_init__ is not None:
+            FractureTemplateCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def append_fracture_template(self, file_path=""):
+        """
+        Create a new StimPlan Fracture Template
+
+        Arguments:
+            file_path (str): File Path to StimPlan Countour File
+        Returns:
+            StimPlanFractureTemplate
+        """
+        return self._call_pdm_method("AppendFractureTemplate", file_path=file_path)
+
+
+    def append_thermal_fracture_template(self, file_path=""):
+        """
+        Create a new Thermal Fracture Template
+
+        Arguments:
+            file_path (str): File Path to Thermal Fracture CSV File
+        Returns:
+            ThermalFractureTemplate
+        """
+        return self._call_pdm_method("AppendThermalFractureTemplate", file_path=file_path)
+
+
+class GeoMechPart(CheckableNamedObject):
+    """
+    Attributes:
+        part_id (int): Part Id
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.part_id = -1
+        CheckableNamedObject.__init__(self, pb2_object, channel)
+        if GeoMechPart.__custom_init__ is not None:
+            GeoMechPart.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GeoMechPartCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if GeoMechPartCollection.__custom_init__ is not None:
+            GeoMechPartCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def parts(self):
+        """Parts
+
+        Returns:
+             List of GeoMechPart
+        """
+        return self.children("Parts", GeoMechPart)
+
+
+class ViewWindow(PdmObjectBase):
+    """
+    The Base Class for all Views and Plots in ResInsight
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if ViewWindow.__custom_init__ is not None:
+            ViewWindow.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class View(ViewWindow):
+    """
+    Attributes:
+        background_color (str): Background
+        current_time_step (int): Current Time Step
+        disable_lighting (bool): Disable Results Lighting
+        grid_z_scale (float): Z Scale
+        id (int): View ID
+        perspective_projection (bool): Perspective Projection
+        show_grid_box (bool): Show Grid Box
+        show_z_scale (bool): Show Z Scale Label
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.background_color = "#b0c4de"
+        self.current_time_step = 0
+        self.disable_lighting = False
+        self.grid_z_scale = 5
+        self.id = -1
+        self.perspective_projection = True
+        self.show_grid_box = True
+        self.show_z_scale = True
+        ViewWindow.__init__(self, pb2_object, channel)
+        if View.__custom_init__ is not None:
+            View.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GeoMechView(View):
+    """
+    The Geomechanical 3d View
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        View.__init__(self, pb2_object, channel)
+        if GeoMechView.__custom_init__ is not None:
+            GeoMechView.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GridCaseSurface(SurfaceInterface):
+    """
+    Attributes:
+        include_inactive_cells (bool): Include Inactive Cells
+        slice_index (int): Slice Index (K)
+        source_case (str): Source Case
+        watertight (bool): Watertight Surface (fill gaps)
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.include_inactive_cells = False
+        self.slice_index = 1
+        self.source_case = ""
+        self.watertight = False
+        SurfaceInterface.__init__(self, pb2_object, channel)
+        if GridCaseSurface.__custom_init__ is not None:
+            GridCaseSurface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GridSummaryCase(SummaryCase):
+    """
+    A Summary Case based on extracting grid data.
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        SummaryCase.__init__(self, pb2_object, channel)
+        if GridSummaryCase.__custom_init__ is not None:
+            GridSummaryCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class IntersectionCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if IntersectionCollection.__custom_init__ is not None:
+            IntersectionCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellPath(PdmObjectBase):
+    """
+    A ResInsight Well Path
+
+    Attributes:
+        name (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.name = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if WellPath.__custom_init__ is not None:
+            WellPath.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def add_fracture(self, measured_depth=0, stim_plan_fracture_template="", align_dip=False, eclipse_case=""):
+        """
+        Add StimPlan Fracture
+
+        Arguments:
+            measured_depth (float): 
+            stim_plan_fracture_template (StimPlanFractureTemplate): StimPlan Fracture Template
+            align_dip (bool): 
+            eclipse_case (RimReservoir): Eclipse Case
+        Returns:
+            WellPathFracture
+        """
+        return self._call_pdm_method("AddFracture", measured_depth=measured_depth, stim_plan_fracture_template=stim_plan_fracture_template, align_dip=align_dip, eclipse_case=eclipse_case)
+
+
+    def add_thermal_fracture(self, measured_depth=0, fracture_template="", place_using_template_data=True):
+        """
+        Add Thermal Fracture
+
+        Arguments:
+            measured_depth (float): 
+            fracture_template (ThermalFractureTemplate): Thermal Fracture Template
+            place_using_template_data (bool): 
+        Returns:
+            WellPathFracture
+        """
+        return self._call_pdm_method("AddThermalFracture", measured_depth=measured_depth, fracture_template=fracture_template, place_using_template_data=place_using_template_data)
+
+
+    def append_perforation_interval(self, start_md=0, end_md=0, diameter=0, skin_factor=0):
+        """
+        Append Perforation Interval
+
+        Arguments:
+            start_md (float): Start Measured Depth
+            end_md (float): End Measured Depth
+            diameter (float): Diameter
+            skin_factor (float): Skin Factor
+        Returns:
+            Perforation
+        """
+        return self._call_pdm_method("AppendPerforationInterval", start_md=start_md, end_md=end_md, diameter=diameter, skin_factor=skin_factor)
+
+
+class ModeledWellPath(WellPath):
+    """
+    A Well Path created interactively in ResInsight
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        WellPath.__init__(self, pb2_object, channel)
+        if ModeledWellPath.__custom_init__ is not None:
+            ModeledWellPath.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def append_lateral(self, tie_in_depth=0, lateral_name=""):
+        """
+        Append Well Path Lateral
+
+        Arguments:
+            tie_in_depth (float): Measured Depth on the Parent Well Path
+            lateral_name (str): Lateral Name
+        Returns:
+            ModeledWellPath
+        """
+        return self._call_pdm_method("AppendLateral", tie_in_depth=tie_in_depth, lateral_name=lateral_name)
+
+
+    def well_path_geometry(self):
+        """Trajectory
+
+        Returns:
+             WellPathGeometry
+        """
+        children = self.children("WellPathGeometry", WellPathGeometry)
+        return children[0] if len(children) > 0 else None
+
+
+class NonNetLayers(PdmObjectBase):
+    """
+    Attributes:
+        cutoff (float): Cutoff
+        facies (str): Facies
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.cutoff = 0
+        self.facies = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if NonNetLayers.__custom_init__ is not None:
+            NonNetLayers.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def facies_definition(self):
+        """
+
+        Returns:
+             EclipseResult
+        """
+        children = self.children("FaciesDefinition", EclipseResult)
+        return children[0] if len(children) > 0 else None
+
+
+class PressureTable(PdmObjectBase):
+    """
+    Attributes:
+        pressure_date (str): Pressure Date
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.pressure_date = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if PressureTable.__custom_init__ is not None:
+            PressureTable.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def items(self):
+        """Pressure Table Items
+
+        Returns:
+             List of PressureTableItem
+        """
+        return self.children("Items", PressureTableItem)
+
+
+class PressureTableItem(PdmObjectBase):
+    """
+    Attributes:
+        depth (float): Depth TVDMSL [m]
+        initial_pressure (float): Initial Pressure [Bar]
+        pressure (float): Pressure [Bar]
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.depth = 0
+        self.initial_pressure = 0
+        self.pressure = 0
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if PressureTableItem.__custom_init__ is not None:
+            PressureTableItem.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GeoMechCase(Case):
+    """
+    The Abaqus Based GeoMech Case
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        Case.__init__(self, pb2_object, channel)
+        if GeoMechCase.__custom_init__ is not None:
+            GeoMechCase.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def views(self):
+        """All GeoMech Views in the Case
+
+        Returns:
+             List of GeoMechView
+        """
+        return self.children("Views", GeoMechView)
+
+
+class Project(PdmObjectBase):
+    """
+    The ResInsight Project
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if Project.__custom_init__ is not None:
+            Project.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def import_summary_case(self, file_name=""):
+        """
+        Import Summary Case
+
+        Arguments:
+            file_name (str): 
+        Returns:
+            FileSummaryCase
+        """
+        return self._call_pdm_method("importSummaryCase", file_name=file_name)
+
+
+    def summary_case(self, case_id=-1):
+        """
+        Find Summary Case
+
+        Arguments:
+            case_id (int): 
+        Returns:
+            FileSummaryCase
+        """
+        return self._call_pdm_method("summaryCase", case_id=case_id)
+
+
+    def surface_folder(self, folder_name=""):
+        """
+        Get Surface Folder
+
+        Arguments:
+            folder_name (str): 
+        Returns:
+            SurfaceCollection
+        """
+        return self._call_pdm_method("surfaceFolder", folder_name=folder_name)
+
+
+class ResampleData(PdmObjectBase):
+    """
+    Attributes:
+        time_steps (List of time): Time Steps
+        values (List of float): Values
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.time_steps = []
+        self.values = []
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if ResampleData.__custom_init__ is not None:
+            ResampleData.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class EclipseView(View):
+    """
+    The Eclipse 3d Reservoir View
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        View.__init__(self, pb2_object, channel)
+        if EclipseView.__custom_init__ is not None:
+            EclipseView.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def cell_result(self):
+        """Cell Result
+
+        Returns:
+             CellColors
+        """
+        children = self.children("CellResult", CellColors)
+        return children[0] if len(children) > 0 else None
+
+
+    def cell_result_data(self):
+        """Current Eclipse Cell Result
+
+        Returns:
+             str
+        """
+        return self._call_get_method("CellResultData")
+
+
+    def set_cell_result_data(self, values):
+        """Set Current Eclipse Cell Result
+
+        Arguments:
+            values (str): data
+        """
+        self._call_set_method("CellResultData", values)
+
+
+class EclipseResult(PdmObjectBase):
+    """
+    An eclipse result definition
+
+    Attributes:
+        flow_tracer_selection_mode (str): One of [FLOW_TR_INJ_AND_PROD, FLOW_TR_PRODUCERS, FLOW_TR_INJECTORS, FLOW_TR_BY_SELECTION]
+        phase_selection (str): One of [PHASE_ALL, PHASE_OIL, PHASE_GAS, PHASE_WAT]
+        porosity_model_type (str): One of [MATRIX_MODEL, FRACTURE_MODEL]
+        result_type (str): One of [DYNAMIC_NATIVE, STATIC_NATIVE, SOURSIMRL, GENERATED, INPUT_PROPERTY, FORMATION_NAMES, ALLAN_DIAGRAMS, FLOW_DIAGNOSTICS, INJECTION_FLOODING]
+        result_variable (str): Variable
+        selected_injector_tracers (List of str): Injector Tracers
+        selected_producer_tracers (List of str): Producer Tracers
+        selected_souring_tracers (List of str): Tracers
+        show_only_visible_categories_in_legend (bool): Show Only Visible Categories In Legend
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.flow_tracer_selection_mode = "FLOW_TR_INJ_AND_PROD"
+        self.phase_selection = "PHASE_ALL"
+        self.porosity_model_type = "MATRIX_MODEL"
+        self.result_type = "DYNAMIC_NATIVE"
+        self.result_variable = "None"
+        self.selected_injector_tracers = []
+        self.selected_producer_tracers = []
+        self.selected_souring_tracers = []
+        self.show_only_visible_categories_in_legend = True
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if EclipseResult.__custom_init__ is not None:
+            EclipseResult.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class CellColors(EclipseResult):
+    """
+    Eclipse Cell Colors class
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        EclipseResult.__init__(self, pb2_object, channel)
+        if CellColors.__custom_init__ is not None:
+            CellColors.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class CommandRouter(PdmObjectBase):
+    """
+    The CommandRouter is used to call code independent to the project
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if CommandRouter.__custom_init__ is not None:
+            CommandRouter.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def extract_surfaces(self, grid_model_filename="", layers=[], minimum_i=-1, maximum_i=-1, minimum_j=-1, maximum_j=-1):
+        """
+        Extract Layer Surface
+
+        Arguments:
+            grid_model_filename (str): 
+            layers (List of int): 
+            minimum_i (int): 
+            maximum_i (int): 
+            minimum_j (int): 
+            maximum_j (int): 
+        Returns:
+            
+        """
+        return self._call_pdm_method("ExtractSurfaces", grid_model_filename=grid_model_filename, layers=layers, minimum_i=minimum_i, maximum_i=maximum_i, minimum_j=minimum_j, maximum_j=maximum_j)
+
+
+class EclipseContourMap(EclipseView):
+    """
+    A contour map for Eclipse cases
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        EclipseView.__init__(self, pb2_object, channel)
+        if EclipseContourMap.__custom_init__ is not None:
+            EclipseContourMap.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GeoMechContourMap(GeoMechView):
+    """
+    A contour map for GeoMech cases
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        GeoMechView.__init__(self, pb2_object, channel)
+        if GeoMechContourMap.__custom_init__ is not None:
+            GeoMechContourMap.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class GridCaseGroup(PdmObjectBase):
+    """
+    A statistics case group
+
+    Attributes:
+        group_id (int): Case Group ID
+        user_description (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.group_id = -1
+        self.user_description = "Grid Case Group"
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if GridCaseGroup.__custom_init__ is not None:
+            GridCaseGroup.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class MudWeightWindowParameters(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if MudWeightWindowParameters.__custom_init__ is not None:
+            MudWeightWindowParameters.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class FractureTemplate(PdmObjectBase):
+    """
+    Attributes:
+        azimuth_angle (float): Azimuth Angle
+        conductivity_factor (float): Conductivity
+        conductivity_type (str): One of [InfiniteConductivity, FiniteConductivity]
+        d_factor_scale_factor (float): D-factor
+        height_scale_factor (float): Height
+        orientation (str): One of [Azimuth, Longitudinal, Transverse]
+        perforation_length (float): Perforation Length
+        user_defined_perforation_length (bool): User-defined Perforation Length
+        user_description (str): Name
+        width_scale_factor (float): Half Length
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.azimuth_angle = 0
+        self.conductivity_factor = 1
+        self.conductivity_type = "FiniteConductivity"
+        self.d_factor_scale_factor = 1
+        self.height_scale_factor = 1
+        self.orientation = "Transverse"
+        self.perforation_length = 1
+        self.user_defined_perforation_length = False
+        self.user_description = "Fracture Template"
+        self.width_scale_factor = 1
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if FractureTemplate.__custom_init__ is not None:
+            FractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def set_scale_factors(self, half_length=1, height=1, d_factor=1, conductivity=1):
+        """
+        Set Fracture Template Scale Factors.
+
+        Arguments:
+            half_length (float): 
+            height (float): 
+            d_factor (float): 
+            conductivity (float): 
+        Returns:
+            
+        """
+        return self._call_pdm_method("SetScaleFactors", half_length=half_length, height=height, d_factor=d_factor, conductivity=conductivity)
+
+
+class MeshFractureTemplate(FractureTemplate):
+    """
+    Attributes:
+        active_time_step_index (int): Active TimeStep Index
+        conductivity_result_name (str): Active Conductivity Result Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.active_time_step_index = 0
+        self.conductivity_result_name = ""
+        FractureTemplate.__init__(self, pb2_object, channel)
+        if MeshFractureTemplate.__custom_init__ is not None:
+            MeshFractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class StimPlanFractureTemplate(MeshFractureTemplate):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        MeshFractureTemplate.__init__(self, pb2_object, channel)
+        if StimPlanFractureTemplate.__custom_init__ is not None:
+            StimPlanFractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class StimPlanModel(CheckableNamedObject):
+    """
+    Attributes:
+        anchor_position (str): Anchor Position
+        auto_compute_barrier (bool): Auto Compute Barrier
+        azimuth_angle (float): Azimuth Angle
+        barrier (bool): Barrier
+        barrier_dip (float): Barrier Dip
+        barrier_fault_name (str): Barrier Fault
+        barrier_text_annotation (str): Barrier Text Annotation
+        bounding_box_horizontal (float): Bounding Box Horizontal
+        bounding_box_vertical (float): Bounding Box Vertical
+        distance_to_barrier (float): Distance To Barrier [m]
+        eclipse_case (str): Dynamic Case
+        extraction_depth_bottom (float): Depth
+        extraction_depth_top (float): Depth
+        extraction_offset_bottom (float): Bottom Offset
+        extraction_offset_top (float): Top Offset
+        extraction_type (str): One of [TVT, TST]
+        formation_dip (float): Formation Dip
+        fracture_orientation (str): One of [Longitudinal, Transverse, Azimuth]
+        initial_pressure_eclipse_case (str): Initial Pressure Case
+        measured_depth (float): Measured Depth
+        original_thickness_direction (str): Original Thickness Direction
+        perforation_interval (str): Perforation Interval
+        perforation_length (float): Perforation Length [m]
+        poro_elastic_constant (float): Poro-Elastic Constant
+        relative_permeability_factor (float): Relative Permeability Factor
+        show_all_faults (bool): Show All Faults
+        show_only_barrier_fault (bool): Show Only Barrier Fault
+        static_eclipse_case (str): Static Case
+        thermal_expansion_coefficient (float): Thermal Expansion Coefficient [1/C]
+        thickness_direction (str): Thickness Direction
+        thickness_direction_well_path (str): Thickness Direction Well Path
+        time_step (int): Time Step
+        use_detailed_fluid_loss (bool): Use Detailed Fluid Loss
+        well_penetration_layer (int): Well Penetration Layer
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.anchor_position = [0, 0, 0]
+        self.auto_compute_barrier = True
+        self.azimuth_angle = 0
+        self.barrier = True
+        self.barrier_dip = 0
+        self.barrier_fault_name = ""
+        self.barrier_text_annotation = ""
+        self.bounding_box_horizontal = 50
+        self.bounding_box_vertical = 100
+        self.distance_to_barrier = 0
+        self.eclipse_case = ""
+        self.extraction_depth_bottom = -1
+        self.extraction_depth_top = -1
+        self.extraction_offset_bottom = -1
+        self.extraction_offset_top = -1
+        self.extraction_type = "TST"
+        self.formation_dip = 0
+        self.fracture_orientation = "Longitudinal"
+        self.initial_pressure_eclipse_case = ""
+        self.measured_depth = 0
+        self.original_thickness_direction = [0, 0, 0]
+        self.perforation_interval = ""
+        self.perforation_length = 10
+        self.poro_elastic_constant = 0
+        self.relative_permeability_factor = 0.5
+        self.show_all_faults = False
+        self.show_only_barrier_fault = False
+        self.static_eclipse_case = ""
+        self.thermal_expansion_coefficient = 0
+        self.thickness_direction = [0, 0, 0]
+        self.thickness_direction_well_path = ""
+        self.time_step = 0
+        self.use_detailed_fluid_loss = True
+        self.well_penetration_layer = 2
+        CheckableNamedObject.__init__(self, pb2_object, channel)
+        if StimPlanModel.__custom_init__ is not None:
+            StimPlanModel.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def export_to_file(self, directory_path=""):
+        """
+        Export StimPlan Model Plot to File
+
+        Arguments:
+            directory_path (str): Directory Path
+        Returns:
+            StimPlanModel
+        """
+        return self._call_pdm_method("ExportToFile", directory_path=directory_path)
+
+
+class StimPlanModelCollection(CheckableNamedObject):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        CheckableNamedObject.__init__(self, pb2_object, channel)
+        if StimPlanModelCollection.__custom_init__ is not None:
+            StimPlanModelCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def append_stim_plan_model(self, well_path="", measured_depth=0, stim_plan_model_template=""):
+        """
+        Create a new StimPlan Model
+
+        Arguments:
+            well_path (WellPathBase): Well Path
+            measured_depth (float): 
+            stim_plan_model_template (StimPlanModelTemplate): StimPlan Model Template
+        Returns:
+            StimPlanModel
+        """
+        return self._call_pdm_method("AppendStimPlanModel", well_path=well_path, measured_depth=measured_depth, stim_plan_model_template=stim_plan_model_template)
+
+
+    def stim_plan_models(self):
+        """
+
+        Returns:
+             List of StimPlanModel
+        """
+        return self.children("StimPlanModels", StimPlanModel)
+
+
+class PlotWindow(ViewWindow):
+    """
+    The Abstract base class for all MDI Windows in the Plot Window
+
+    Attributes:
+        id (int): View ID
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.id = -1
+        ViewWindow.__init__(self, pb2_object, channel)
+        if PlotWindow.__custom_init__ is not None:
+            PlotWindow.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class DepthTrackPlot(PlotWindow):
+    """
+    Attributes:
+        auto_scale_depth_enabled (bool): Auto Scale
+        auto_zoom_max_depth_factor (float): Auto Zoom Maximum Factor
+        auto_zoom_min_depth_factor (float): Auto Zoom Minimum Factor
+        axis_title_font_size (str): One of [XX_Small, X_Small, Small, Medium, Large, X_Large, XX_Large]
+        axis_value_font_size (str): One of [XX_Small, X_Small, Small, Medium, Large, X_Large, XX_Large]
+        depth_type (str): One of [MEASURED_DEPTH, TRUE_VERTICAL_DEPTH, PSEUDO_LENGTH, CONNECTION_NUMBER, TRUE_VERTICAL_DEPTH_RKB]
+        depth_unit (str): One of [UNIT_METER, UNIT_FEET, UNIT_NONE]
+        maximum_depth (float): Max
+        minimum_depth (float): Min
+        show_depth_grid_lines (str): One of [GRID_X_NONE, GRID_X_MAJOR, GRID_X_MAJOR_AND_MINOR]
+        show_depth_marker_line (bool): Show Depth Marker Line
+        sub_title_font_size (str): One of [XX_Small, X_Small, Small, Medium, Large, X_Large, XX_Large]
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.auto_scale_depth_enabled = True
+        self.auto_zoom_max_depth_factor = 0
+        self.auto_zoom_min_depth_factor = 0
+        self.axis_title_font_size = "Medium"
+        self.axis_value_font_size = "Medium"
+        self.depth_type = "MEASURED_DEPTH"
+        self.depth_unit = "UNIT_METER"
+        self.maximum_depth = 1000
+        self.minimum_depth = 0
+        self.show_depth_grid_lines = "GRID_X_MAJOR"
+        self.show_depth_marker_line = False
+        self.sub_title_font_size = "Medium"
+        PlotWindow.__init__(self, pb2_object, channel)
+        if DepthTrackPlot.__custom_init__ is not None:
+            DepthTrackPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class StimPlanModelPlot(DepthTrackPlot):
+    """
+    A fracture model plot
+
+    Attributes:
+        eclipse_case (str): Case
+        stim_plan_model (str): StimPlan Model
+        time_step (int): Time Step
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.eclipse_case = ""
+        self.stim_plan_model = ""
+        self.time_step = 0
+        DepthTrackPlot.__init__(self, pb2_object, channel)
+        if StimPlanModelPlot.__custom_init__ is not None:
+            StimPlanModelPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class StimPlanModelPlotCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if StimPlanModelPlotCollection.__custom_init__ is not None:
+            StimPlanModelPlotCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def append_stim_plan_model_plot(self, stim_plan_model=""):
+        """
+        Create a new StimPlan Model
+
+        Arguments:
+            stim_plan_model (StimPlanModel): StimPlan Model
+        Returns:
+            StimPlanModelPlot
+        """
+        return self._call_pdm_method("AppendStimPlanModelPlot", stim_plan_model=stim_plan_model)
+
+
+    def stim_plan_model_plots(self):
+        """
+
+        Returns:
+             List of StimPlanModelPlot
+        """
+        return self.children("StimPlanModelPlots", StimPlanModelPlot)
+
+
+class StimPlanModelTemplate(NamedObject):
+    """
+    Attributes:
+        default_facies (str): Default Facies
+        default_permeability (float): Default Permeability
+        default_porosity (float): Default Porosity
+        dynamic_eclipse_case (str): Dynamic Case
+        id (int): ID
+        initial_pressure_eclipse_case (str): Initial Pressure Case
+        overburden_facies (str): Overburden Facies
+        overburden_fluid_density (float): Overburden Fluid Density [g/cm^3]
+        overburden_formation (str): Overburden Formation
+        overburden_height (float): Overburden Height
+        overburden_permeability (float): Overburden Permeability
+        overburden_porosity (float): Overburden Porosity
+        reference_temperature (float): Temperature [C]
+        reference_temperature_depth (float): Temperature Depth [m]
+        reference_temperature_gradient (float): Temperature Gradient [C/m]
+        static_eclipse_case (str): Static Case
+        stress_depth (float): Stress Depth
+        time_step (int): Time Step
+        underburden_facies (str): Underburden Facies
+        underburden_fluid_density (float): Underburden Fluid Density [g/cm^3]
+        underburden_formation (str): Underburden Formation
+        underburden_height (float): Underburden Height
+        underburden_permeability (float): Underburden Permeability
+        underburden_porosity (float): Underburden Porosity
+        vertical_stress (float): Vertical Stress
+        vertical_stress_gradient (float): Vertical Stress Gradient
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.default_facies = ""
+        self.default_permeability = 0.0001
+        self.default_porosity = 0.01
+        self.dynamic_eclipse_case = ""
+        self.id = -1
+        self.initial_pressure_eclipse_case = ""
+        self.overburden_facies = ""
+        self.overburden_fluid_density = 1.03
+        self.overburden_formation = ""
+        self.overburden_height = 50
+        self.overburden_permeability = 1e-05
+        self.overburden_porosity = 0
+        self.reference_temperature = 70
+        self.reference_temperature_depth = 2500
+        self.reference_temperature_gradient = 0.025
+        self.static_eclipse_case = ""
+        self.stress_depth = 1000
+        self.time_step = 0
+        self.underburden_facies = ""
+        self.underburden_fluid_density = 1.03
+        self.underburden_formation = ""
+        self.underburden_height = 50
+        self.underburden_permeability = 1e-05
+        self.underburden_porosity = 0
+        self.vertical_stress = 238
+        self.vertical_stress_gradient = 0.238
+        NamedObject.__init__(self, pb2_object, channel)
+        if StimPlanModelTemplate.__custom_init__ is not None:
+            StimPlanModelTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def elastic_properties(self):
+        """Elastic Properties
+
+        Returns:
+             ElasticProperties
+        """
+        children = self.children("ElasticProperties", ElasticProperties)
+        return children[0] if len(children) > 0 else None
+
+
+    def facies_initial_pressure_configs(self):
+        """Facies Initial Pressure Configs
+
+        Returns:
+             List of FaciesInitialPressureConfig
+        """
+        return self.children("FaciesInitialPressureConfigs", FaciesInitialPressureConfig)
+
+
+    def facies_properties(self):
+        """Facies Properties
+
+        Returns:
+             FaciesProperties
+        """
+        children = self.children("FaciesProperties", FaciesProperties)
+        return children[0] if len(children) > 0 else None
+
+
+    def non_net_layers(self):
+        """Non-Net Layers
+
+        Returns:
+             NonNetLayers
+        """
+        children = self.children("NonNetLayers", NonNetLayers)
+        return children[0] if len(children) > 0 else None
+
+
+    def pressure_table(self):
+        """Pressure Table
+
+        Returns:
+             PressureTable
+        """
+        children = self.children("PressureTable", PressureTable)
+        return children[0] if len(children) > 0 else None
+
+
+class StimPlanModelTemplateCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if StimPlanModelTemplateCollection.__custom_init__ is not None:
+            StimPlanModelTemplateCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def append_stim_plan_model_template(self, eclipse_case="", time_step=0, facies_properties_file_path="", elastic_properties_file_path=""):
+        """
+        Create a new StimPlan Model Template
+
+        Arguments:
+            eclipse_case (RimReservoir): Eclipse Case
+            time_step (int): Time Step
+            facies_properties_file_path (str): Facies Properties File Path
+            elastic_properties_file_path (str): Elastic Properties File Path
+        Returns:
+            StimPlanModelTemplate
+        """
+        return self._call_pdm_method("AppendStimPlanModelTemplate", eclipse_case=eclipse_case, time_step=time_step, facies_properties_file_path=facies_properties_file_path, elastic_properties_file_path=elastic_properties_file_path)
+
+
+    def stim_plan_model_templates(self):
+        """StimPlan Model Templates
+
+        Returns:
+             List of StimPlanModelTemplate
+        """
+        return self.children("StimPlanModelTemplates", StimPlanModelTemplate)
+
+
+class SummaryCaseSubCollection(PdmObjectBase):
+    """
+    Attributes:
+        create_auto_name (bool): Auto Name
+        id (int): Ensemble ID
+        is_ensemble (bool): Is Ensemble
+        name_count (str): Name
+        summary_collection_name (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.create_auto_name = True
+        self.id = -1
+        self.is_ensemble = False
+        self.name_count = "Group"
+        self.summary_collection_name = "Group"
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if SummaryCaseSubCollection.__custom_init__ is not None:
+            SummaryCaseSubCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class Plot(PlotWindow):
+    """
+    The Abstract Base Class for all Plot Objects
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PlotWindow.__init__(self, pb2_object, channel)
+        if Plot.__custom_init__ is not None:
+            Plot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class SummaryPlot(Plot):
+    """
+    A Summary Plot
+
+    Attributes:
+        is_using_auto_name (bool): Auto Title
+        normalize_curve_y_values (bool): Normalize all curves
+        plot_description (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.is_using_auto_name = True
+        self.normalize_curve_y_values = False
+        self.plot_description = "Summary Plot"
+        Plot.__init__(self, pb2_object, channel)
+        if SummaryPlot.__custom_init__ is not None:
+            SummaryPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class SummaryPlotCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if SummaryPlotCollection.__custom_init__ is not None:
+            SummaryPlotCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def new_summary_plot(self, summary_cases=[], ensemble="", address=""):
+        """
+        Create a new Summary Plot
+
+        Arguments:
+            summary_cases (List of SummaryCase): Summary Cases
+            ensemble (SummaryCaseSubCollection): Ensemble
+            address (str): Formatted address string specifying the plot options
+        Returns:
+            SummaryPlot
+        """
+        return self._call_pdm_method("NewSummaryPlot", summary_cases=summary_cases, ensemble=ensemble, address=address)
+
+
+class Surface(SurfaceInterface):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        SurfaceInterface.__init__(self, pb2_object, channel)
+        if Surface.__custom_init__ is not None:
+            Surface.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class ThermalFractureTemplate(MeshFractureTemplate):
+    """
+    Attributes:
+        filter_cake_pressure_drop (str): One of [None, Relative, Absolute]
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.filter_cake_pressure_drop = "Relative"
+        MeshFractureTemplate.__init__(self, pb2_object, channel)
+        if ThermalFractureTemplate.__custom_init__ is not None:
+            ThermalFractureTemplate.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def export_to_file(self, file_path="", time_step=0):
+        """
+        Export Thermal Fracture Template to File
+
+        Arguments:
+            file_path (str): File Path
+            time_step (int): 
+        Returns:
+            ThermalFractureTemplate
+        """
+        return self._call_pdm_method("ExportToFile", file_path=file_path, time_step=time_step)
+
+
+    def time_steps(self, ):
+        """
+        Get Thermal Fracture Template Time Steps
+
+        Arguments:
+            
+        Returns:
+            DataContainerString
+        """
+        return self._call_pdm_method("TimeSteps")
+
+
+class TriangleGeometry(PdmObjectBase):
+    """
+    Attributes:
+        connections (List of int): Indices to triangle vertices
+        display_model_offset (str): Display Model Offset
+        fault_mesh_x_coords (List of float): Fault Mesh X coords
+        fault_mesh_y_coords (List of float): Fault Mesh Y coords
+        fault_mesh_z_coords (List of float): Fault Mesh Z coords
+        mesh_x_coords (List of float): Mesh X coords
+        mesh_y_coords (List of float): Mesh Y coords
+        mesh_z_coords (List of float): Mesh Z coords
+        x_coords (List of float): X coords
+        y_coords (List of float): Y coords
+        z_coords (List of float): Z coords
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.connections = []
+        self.display_model_offset = [0, 0, 0]
+        self.fault_mesh_x_coords = []
+        self.fault_mesh_y_coords = []
+        self.fault_mesh_z_coords = []
+        self.mesh_x_coords = []
+        self.mesh_y_coords = []
+        self.mesh_z_coords = []
+        self.x_coords = []
+        self.y_coords = []
+        self.z_coords = []
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if TriangleGeometry.__custom_init__ is not None:
+            TriangleGeometry.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WbsParameters(PdmObjectBase):
+    """
+    Attributes:
+        df_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        fg_multiplier (float): SH Multiplier for FG in Shale
+        fg_shale_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        k0_fg_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        k0_sh_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        obg0_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        poission_ratio_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        pore_pressure_non_reservoir_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        pore_pressure_reservoir_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        ucs_source (str): One of [GRID, LAS_FILE, ELEMENT_PROPERTY_TABLE, USER_DEFINED, HYDROSTATIC, DERIVED_FROM_K0FG, PROPORTIONAL_TO_SH, UNDEFINED]
+        user_df (float): User Defined DF
+        user_k0_fg (float): User Defined K0_FG
+        user_k0_sh (float): User Defined K0_SH
+        user_poisson_ratio (float): User Defined Poisson Ratio
+        user_pp_non_reservoir (float):   Multiplier of hydrostatic PP
+        user_ucs (float): User Defined UCS [bar]
+        water_density (float): Density of Sea Water [g/cm^3]
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.df_source = "LAS_FILE"
+        self.fg_multiplier = 1.05
+        self.fg_shale_source = "DERIVED_FROM_K0FG"
+        self.k0_fg_source = "LAS_FILE"
+        self.k0_sh_source = "LAS_FILE"
+        self.obg0_source = "GRID"
+        self.poission_ratio_source = "LAS_FILE"
+        self.pore_pressure_non_reservoir_source = "LAS_FILE"
+        self.pore_pressure_reservoir_source = "GRID"
+        self.ucs_source = "LAS_FILE"
+        self.user_df = 0.7
+        self.user_k0_fg = 0.75
+        self.user_k0_sh = 0.65
+        self.user_poisson_ratio = 0.35
+        self.user_pp_non_reservoir = 1
+        self.user_ucs = 100
+        self.water_density = 1.03
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if WbsParameters.__custom_init__ is not None:
+            WbsParameters.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class SimulationWell(PdmObjectBase):
+    """
+    An Eclipse Simulation Well
+
+    Attributes:
+        name (str): Name
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.name = ""
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if SimulationWell.__custom_init__ is not None:
+            SimulationWell.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellLogPlot(DepthTrackPlot):
+    """
+    A Well Log Plot With a shared Depth Axis and Multiple Tracks
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        DepthTrackPlot.__init__(self, pb2_object, channel)
+        if WellLogPlot.__custom_init__ is not None:
+            WellLogPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def new_well_log_track(self, title="", case="", well_path=""):
+        """
+        Create a new well log track
+
+        Arguments:
+            title (str): Title
+            case (RimReservoir): Case
+            well_path (WellPathBase): Well Path
+        Returns:
+            WellLogPlotTrack
+        """
+        return self._call_pdm_method("NewWellLogTrack", title=title, case=case, well_path=well_path)
+
+
+class WellBoreStabilityPlot(WellLogPlot):
+    """
+    A GeoMechanical Well Bore Stability Plot
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        WellLogPlot.__init__(self, pb2_object, channel)
+        if WellBoreStabilityPlot.__custom_init__ is not None:
+            WellBoreStabilityPlot.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def parameters(self):
+        """Well Bore Stability Parameters
+
+        Returns:
+             WbsParameters
+        """
+        children = self.children("Parameters", WbsParameters)
+        return children[0] if len(children) > 0 else None
+
+
+class PlotCurve(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if PlotCurve.__custom_init__ is not None:
+            PlotCurve.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellLogPlotCurve(PlotCurve):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PlotCurve.__init__(self, pb2_object, channel)
+        if WellLogPlotCurve.__custom_init__ is not None:
+            WellLogPlotCurve.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellLogExtractionCurve(WellLogPlotCurve):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        WellLogPlotCurve.__init__(self, pb2_object, channel)
+        if WellLogExtractionCurve.__custom_init__ is not None:
+            WellLogExtractionCurve.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellLogPlotCollection(PdmObjectBase):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if WellLogPlotCollection.__custom_init__ is not None:
+            WellLogPlotCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def new_well_log_plot(self, case="", well_path="", property_type="", property_name="", time_step=0):
+        """
+        Create a new well log plot
+
+        Arguments:
+            case (RimReservoir): Case
+            well_path (WellPathBase): Well Path
+            property_type (str): Property Type
+            property_name (str): Property Name
+            time_step (int): Time Step
+        Returns:
+            WellLogPlot
+        """
+        return self._call_pdm_method("NewWellLogPlot", case=case, well_path=well_path, property_type=property_type, property_name=property_name, time_step=time_step)
+
+
+    def well_log_plots(self):
+        """
+
+        Returns:
+             List of WellLogPlot
+        """
+        return self.children("WellLogPlots", WellLogPlot)
+
+
+class WellLogPlotTrack(Plot):
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        Plot.__init__(self, pb2_object, channel)
+        if WellLogPlotTrack.__custom_init__ is not None:
+            WellLogPlotTrack.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def add_extraction_curve(self, case="", well_path="", property_type="", property_name="", time_step=0):
+        """
+        Create a well log extraction curve
+
+        Arguments:
+            case (RimReservoir): Case
+            well_path (WellPathBase): Well Path
+            property_type (str): Property Type
+            property_name (str): Property Name
+            time_step (int): Time Step
+        Returns:
+            WellLogExtractionCurve
+        """
+        return self._call_pdm_method("AddExtractionCurve", case=case, well_path=well_path, property_type=property_type, property_name=property_name, time_step=time_step)
+
+
+class FileWellPath(WellPath):
+    """
+    Well Paths Loaded From File
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        WellPath.__init__(self, pb2_object, channel)
+        if FileWellPath.__custom_init__ is not None:
+            FileWellPath.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellPathGeometry(PdmObjectBase):
+    """
+    Class containing the geometry of a modeled Well Path
+
+    Attributes:
+        air_gap (float): Air Gap
+        attached_to_parent_well (bool): Attached to Parent Well
+        link_reference_point_updates (bool): Link Reference Point
+        md_at_first_target (float): MD at First Target
+        reference_point (str): UTM Reference Point
+        show_spheres (bool): Spheres
+        use_auto_generated_target_at_sea_level (bool): Generate Target at Sea Level
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.air_gap = 0
+        self.attached_to_parent_well = False
+        self.link_reference_point_updates = False
+        self.md_at_first_target = 0
+        self.reference_point = [0, 0, 0]
+        self.show_spheres = True
+        self.use_auto_generated_target_at_sea_level = True
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if WellPathGeometry.__custom_init__ is not None:
+            WellPathGeometry.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def append_well_target(self, coordinate=[0, 0, 0], absolute=False, use_fixed_azimuth=False, use_fixed_inclination=False, fixed_azimuth_value=0, fixed_inclination_value=0):
+        """
+        Create and Add New Well Target
+
+        Arguments:
+            coordinate (N3cvf7Vector3IdEE): Coordinate
+            absolute (bool): Relative or Absolute Coordinate
+            use_fixed_azimuth (bool): 
+            use_fixed_inclination (bool): 
+            fixed_azimuth_value (float): [Degrees]
+            fixed_inclination_value (float): [Degrees]
+        Returns:
+            WellPathTarget
+        """
+        return self._call_pdm_method("AppendWellTarget", coordinate=coordinate, absolute=absolute, use_fixed_azimuth=use_fixed_azimuth, use_fixed_inclination=use_fixed_inclination, fixed_azimuth_value=fixed_azimuth_value, fixed_inclination_value=fixed_inclination_value)
+
+
+    def auto_generated_target(self):
+        """Auto Generated Target
+
+        Returns:
+             WellPathTarget
+        """
+        children = self.children("AutoGeneratedTarget", WellPathTarget)
+        return children[0] if len(children) > 0 else None
+
+
+    def well_path_targets(self):
+        """Well Targets
+
+        Returns:
+             List of WellPathTarget
+        """
+        return self.children("WellPathTargets", WellPathTarget)
+
+
+class WellPathTarget(PdmObjectBase):
+    """
+    Class containing the Well Target definition
+
+    Attributes:
+        azimuth (float): Azi(deg)
+        dogleg1 (float): DL in
+        dogleg2 (float): DL out
+        estimated_azimuth (float): Est Azi(deg)
+        estimated_dogleg1 (float): Est DL in
+        estimated_dogleg2 (float): Est DL out
+        estimated_inclination (float): Est Inc(deg)
+        inclination (float): Inc(deg)
+        target_measured_depth (float): MD
+        target_point (str): Relative Coord
+        use_fixed_azimuth (bool): Azi
+        use_fixed_inclination (bool): Inc
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        self.azimuth = 0
+        self.dogleg1 = 3
+        self.dogleg2 = 3
+        self.estimated_azimuth = 0
+        self.estimated_dogleg1 = 0
+        self.estimated_dogleg2 = 0
+        self.estimated_inclination = 0
+        self.inclination = 0
+        self.target_measured_depth = 0
+        self.target_point = [0, 0, 0]
+        self.use_fixed_azimuth = False
+        self.use_fixed_inclination = False
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if WellPathTarget.__custom_init__ is not None:
+            WellPathTarget.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+class WellPathCollection(PdmObjectBase):
+    """
+    Collection of Well Paths
+
+    """
+    __custom_init__ = None #: Assign a custom init routine to be run at __init__
+
+    def __init__(self, pb2_object=None, channel=None):
+        PdmObjectBase.__init__(self, pb2_object, channel)
+        if WellPathCollection.__custom_init__ is not None:
+            WellPathCollection.__custom_init__(self, pb2_object=pb2_object, channel=channel)
+
+    def well_paths(self):
+        """Well Paths
+
+        Returns:
+             List of WellPath
+        """
+        return self.children("WellPaths", WellPath)
+
+
+def class_dict():
+    classes = {}
+    classes['Case'] = Case
+    classes['CellColors'] = CellColors
+    classes['CellFilterCollection'] = CellFilterCollection
+    classes['CheckableNamedObject'] = CheckableNamedObject
+    classes['CommandRouter'] = CommandRouter
+    classes['CurveIntersection'] = CurveIntersection
+    classes['DataContainerFloat'] = DataContainerFloat
+    classes['DataContainerString'] = DataContainerString
+    classes['DataContainerTime'] = DataContainerTime
+    classes['DepthTrackPlot'] = DepthTrackPlot
+    classes['EclipseCase'] = EclipseCase
+    classes['EclipseContourMap'] = EclipseContourMap
+    classes['EclipseResult'] = EclipseResult
+    classes['EclipseView'] = EclipseView
+    classes['ElasticProperties'] = ElasticProperties
+    classes['ElasticPropertyScaling'] = ElasticPropertyScaling
+    classes['ElasticPropertyScalingCollection'] = ElasticPropertyScalingCollection
+    classes['EnsembleStatisticsSurface'] = EnsembleStatisticsSurface
+    classes['EnsembleSurface'] = EnsembleSurface
+    classes['EnsembleWellLogs'] = EnsembleWellLogs
+    classes['FaciesInitialPressureConfig'] = FaciesInitialPressureConfig
+    classes['FaciesProperties'] = FaciesProperties
+    classes['FileSummaryCase'] = FileSummaryCase
+    classes['FileWellPath'] = FileWellPath
+    classes['FractureTemplate'] = FractureTemplate
+    classes['FractureTemplateCollection'] = FractureTemplateCollection
+    classes['GeoMechCase'] = GeoMechCase
+    classes['GeoMechContourMap'] = GeoMechContourMap
+    classes['GeoMechPart'] = GeoMechPart
+    classes['GeoMechPartCollection'] = GeoMechPartCollection
+    classes['GeoMechView'] = GeoMechView
+    classes['GridCaseGroup'] = GridCaseGroup
+    classes['GridCaseSurface'] = GridCaseSurface
+    classes['GridSummaryCase'] = GridSummaryCase
+    classes['IntersectionCollection'] = IntersectionCollection
+    classes['MeshFractureTemplate'] = MeshFractureTemplate
+    classes['ModeledWellPath'] = ModeledWellPath
+    classes['MudWeightWindowParameters'] = MudWeightWindowParameters
+    classes['NamedObject'] = NamedObject
+    classes['NonNetLayers'] = NonNetLayers
+    classes['PdmObjectBase'] = PdmObjectBase
+    classes['Plot'] = Plot
+    classes['PlotCurve'] = PlotCurve
+    classes['PlotWindow'] = PlotWindow
+    classes['PressureTable'] = PressureTable
+    classes['PressureTableItem'] = PressureTableItem
+    classes['Project'] = Project
+    classes['ResampleData'] = ResampleData
+    classes['Reservoir'] = Reservoir
+    classes['SimulationWell'] = SimulationWell
+    classes['StimPlanFractureTemplate'] = StimPlanFractureTemplate
+    classes['StimPlanModel'] = StimPlanModel
+    classes['StimPlanModelCollection'] = StimPlanModelCollection
+    classes['StimPlanModelPlot'] = StimPlanModelPlot
+    classes['StimPlanModelPlotCollection'] = StimPlanModelPlotCollection
+    classes['StimPlanModelTemplate'] = StimPlanModelTemplate
+    classes['StimPlanModelTemplateCollection'] = StimPlanModelTemplateCollection
+    classes['SummaryCase'] = SummaryCase
+    classes['SummaryCaseSubCollection'] = SummaryCaseSubCollection
+    classes['SummaryPlot'] = SummaryPlot
+    classes['SummaryPlotCollection'] = SummaryPlotCollection
+    classes['Surface'] = Surface
+    classes['SurfaceCollection'] = SurfaceCollection
+    classes['SurfaceInterface'] = SurfaceInterface
+    classes['ThermalFractureTemplate'] = ThermalFractureTemplate
+    classes['TriangleGeometry'] = TriangleGeometry
+    classes['View'] = View
+    classes['ViewWindow'] = ViewWindow
+    classes['WbsParameters'] = WbsParameters
+    classes['WellBoreStabilityPlot'] = WellBoreStabilityPlot
+    classes['WellLogExtractionCurve'] = WellLogExtractionCurve
+    classes['WellLogPlot'] = WellLogPlot
+    classes['WellLogPlotCollection'] = WellLogPlotCollection
+    classes['WellLogPlotCurve'] = WellLogPlotCurve
+    classes['WellLogPlotTrack'] = WellLogPlotTrack
+    classes['WellPath'] = WellPath
+    classes['WellPathCollection'] = WellPathCollection
+    classes['WellPathGeometry'] = WellPathGeometry
+    classes['WellPathTarget'] = WellPathTarget
+    return classes
+
+def class_from_keyword(class_keyword):
+    all_classes = class_dict()
+    if class_keyword in all_classes.keys():
+        return all_classes[class_keyword]
+    return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rips-2023.6.0.1/rips/grid.py` & `rips-2023.6.0.2/rips/grid.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# pylint: disable=too-few-public-methods
-
-"""
-Module containing the Grid class, containing information
-about Case grids.
-"""
-
-import Case_pb2
-import Grid_pb2
-import Grid_pb2_grpc
-
-
-class Grid:
-    """Grid Information. Created by methods in Case
-    :meth:`rips.case.grid()`
-    :meth:`rips.case.grids()`
-    """
-
-    def __init__(self, index, case, channel):
-        self.__channel = channel
-        self.__stub = Grid_pb2_grpc.GridStub(self.__channel)
-
-        self.case = case
-        self.index = index
-        self.cached_dimensions = None
-
-    def dimensions(self):
-        """The dimensions in i, j, k direction
-
-        Returns:
-            Vec3i: class with integer attributes i, j, k giving extent in all three dimensions.
-        """
-        case_request = Case_pb2.CaseRequest(id=self.case.id)
-
-        if self.cached_dimensions is None:
-            self.cached_dimensions = self.__stub.GetDimensions(
-                Grid_pb2.GridRequest(case_request=case_request, grid_index=self.index)
-            ).dimensions
-
-        return self.cached_dimensions
-
-    def cell_centers_async(self):
-        """The cells center for all cells in given grid async.
-
-        Returns:
-            Iterator to a list of Vec3d: class with double attributes x, y, x giving cell centers
-        """
-        case_request = Case_pb2.CaseRequest(id=self.case.id)
-        chunks = self.__stub.GetCellCenters(
-            Grid_pb2.GridRequest(case_request=case_request, grid_index=self.index)
-        )
-        for chunk in chunks:
-            yield chunk
-
-    def cell_centers(self):
-        """The cell center for all cells in given grid
-
-        Returns:
-            List of Vec3d: class with double attributes x, y, x giving cell centers
-        """
-        centers = []
-        chunks = self.cell_centers_async()
-        for chunk in chunks:
-            for center in chunk.centers:
-                centers.append(center)
-        return centers
-
-    def cell_corners_async(self):
-        """The cell corners for all cells in given grid, async.
-
-        Returns:
-            iterator to a list of CellCorners: a class with Vec3d for each corner (c0, c1.., c7)
-        """
-        case_request = Case_pb2.CaseRequest(id=self.case.id)
-        chunks = self.__stub.GetCellCorners(
-            Grid_pb2.GridRequest(case_request=case_request, grid_index=self.index)
-        )
-
-        for chunk in chunks:
-            yield chunk
-
-    def cell_corners(self):
-        """The cell corners for all cells in given grid
-
-        Returns:
-            list of CellCorners: a class with Vec3d for each corner (c0, c1.., c7)
-        """
-        corners = []
-        chunks = self.cell_corners_async()
-        for chunk in chunks:
-            for center in chunk.cells:
-                corners.append(center)
-        return corners
-
-    def property_data_index_from_ijk(self, i, j, k):
-        """Compute property index from 1-based IJK cell address. Cell Property Result data is organized by I, J and K.
-
-        property_data_index = dims.i * dims.j * (k - 1) + dims.i * (j - 1) + (i - 1)
-
-        Returns:
-            int: Cell property result index from IJK
-        """
-
-        dims = self.dimensions()
-
-        property_data_index = dims.i * dims.j * (k - 1) + dims.i * (j - 1) + (i - 1)
-
-        return property_data_index
-
-    def cell_count(self):
-        """Cell count in grid
-
-        Returns:
-            int: Cell count in grid
-        """
-
-        dims = self.dimensions()
-
-        count = dims.i * dims.j * dims.k
-
-        return count
+# pylint: disable=too-few-public-methods
+
+"""
+Module containing the Grid class, containing information
+about Case grids.
+"""
+
+import Case_pb2
+import Grid_pb2
+import Grid_pb2_grpc
+
+
+class Grid:
+    """Grid Information. Created by methods in Case
+    :meth:`rips.case.grid()`
+    :meth:`rips.case.grids()`
+    """
+
+    def __init__(self, index, case, channel):
+        self.__channel = channel
+        self.__stub = Grid_pb2_grpc.GridStub(self.__channel)
+
+        self.case = case
+        self.index = index
+        self.cached_dimensions = None
+
+    def dimensions(self):
+        """The dimensions in i, j, k direction
+
+        Returns:
+            Vec3i: class with integer attributes i, j, k giving extent in all three dimensions.
+        """
+        case_request = Case_pb2.CaseRequest(id=self.case.id)
+
+        if self.cached_dimensions is None:
+            self.cached_dimensions = self.__stub.GetDimensions(
+                Grid_pb2.GridRequest(case_request=case_request, grid_index=self.index)
+            ).dimensions
+
+        return self.cached_dimensions
+
+    def cell_centers_async(self):
+        """The cells center for all cells in given grid async.
+
+        Returns:
+            Iterator to a list of Vec3d: class with double attributes x, y, x giving cell centers
+        """
+        case_request = Case_pb2.CaseRequest(id=self.case.id)
+        chunks = self.__stub.GetCellCenters(
+            Grid_pb2.GridRequest(case_request=case_request, grid_index=self.index)
+        )
+        for chunk in chunks:
+            yield chunk
+
+    def cell_centers(self):
+        """The cell center for all cells in given grid
+
+        Returns:
+            List of Vec3d: class with double attributes x, y, x giving cell centers
+        """
+        centers = []
+        chunks = self.cell_centers_async()
+        for chunk in chunks:
+            for center in chunk.centers:
+                centers.append(center)
+        return centers
+
+    def cell_corners_async(self):
+        """The cell corners for all cells in given grid, async.
+
+        Returns:
+            iterator to a list of CellCorners: a class with Vec3d for each corner (c0, c1.., c7)
+        """
+        case_request = Case_pb2.CaseRequest(id=self.case.id)
+        chunks = self.__stub.GetCellCorners(
+            Grid_pb2.GridRequest(case_request=case_request, grid_index=self.index)
+        )
+
+        for chunk in chunks:
+            yield chunk
+
+    def cell_corners(self):
+        """The cell corners for all cells in given grid
+
+        Returns:
+            list of CellCorners: a class with Vec3d for each corner (c0, c1.., c7)
+        """
+        corners = []
+        chunks = self.cell_corners_async()
+        for chunk in chunks:
+            for center in chunk.cells:
+                corners.append(center)
+        return corners
+
+    def property_data_index_from_ijk(self, i, j, k):
+        """Compute property index from 1-based IJK cell address. Cell Property Result data is organized by I, J and K.
+
+        property_data_index = dims.i * dims.j * (k - 1) + dims.i * (j - 1) + (i - 1)
+
+        Returns:
+            int: Cell property result index from IJK
+        """
+
+        dims = self.dimensions()
+
+        property_data_index = dims.i * dims.j * (k - 1) + dims.i * (j - 1) + (i - 1)
+
+        return property_data_index
+
+    def cell_count(self):
+        """Cell count in grid
+
+        Returns:
+            int: Cell count in grid
+        """
+
+        dims = self.dimensions()
+
+        count = dims.i * dims.j * dims.k
+
+        return count
```

### Comparing `rips-2023.6.0.1/rips/gridcasegroup.py` & `rips-2023.6.0.2/rips/gridcasegroup.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-"""
-Grid Case Group statistics module
-"""
-
-from .pdmobject import add_method
-from .view import View
-from .case import Case
-
-import Commands_pb2
-from .resinsight_classes import GridCaseGroup
-from .resinsight_classes import EclipseView
-
-
-@add_method(GridCaseGroup)
-def create_statistics_case(self):
-    """Create a Statistics case in the Grid Case Group
-
-    Returns:
-        :class:`rips.generated.generated_classes.EclipseCase`
-    """
-    command_reply = self._execute_command(
-        createStatisticsCase=Commands_pb2.CreateStatisticsCaseRequest(
-            caseGroupId=self.group_id
-        )
-    )
-    return Case(self.channel, command_reply.createStatisticsCaseResult.caseId)
-
-
-@add_method(GridCaseGroup)
-def statistics_cases(self):
-    """Get a list of all statistics cases in the Grid Case Group
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.EclipseCase`
-
-    """
-    stat_case_collection = self.children("StatisticsCaseCollection")[0]
-    return stat_case_collection.children("Reservoirs")
-
-
-@add_method(GridCaseGroup)
-def views(self):
-    """Get a list of views belonging to a grid case group
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.EclipseView`
-
-    """
-    resinsight_classes = self.descendants(EclipseView)
-    view_list = []
-    for pdm_object in resinsight_classes:
-        view_list.append(pdm_object)
-    return view_list
-
-
-@add_method(GridCaseGroup)
-def view(self, view_id):
-    """Get a particular view belonging to a case group by providing view id
-
-    Arguments:
-        id(int): view id
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.EclipseView`
-
-    """
-    views = self.views()
-    for view_object in views:
-        if view_object.id == view_id:
-            return view_object
-    return None
-
-
-@add_method(GridCaseGroup)
-def compute_statistics(self, case_ids=None):
-    """Compute statistics for the given case ids
-
-    Arguments:
-        case_ids(list of integers): List of case ids. If this is None all cases in group are included
-
-    """
-    if case_ids is None:
-        case_ids = []
-    return self._execute_command(
-        computeCaseGroupStatistics=Commands_pb2.ComputeCaseGroupStatRequest(
-            caseIds=case_ids, caseGroupId=self.group_id
-        )
-    )
+"""
+Grid Case Group statistics module
+"""
+
+from .pdmobject import add_method
+from .view import View
+from .case import Case
+
+import Commands_pb2
+from .resinsight_classes import GridCaseGroup
+from .resinsight_classes import EclipseView
+
+
+@add_method(GridCaseGroup)
+def create_statistics_case(self):
+    """Create a Statistics case in the Grid Case Group
+
+    Returns:
+        :class:`rips.generated.generated_classes.EclipseCase`
+    """
+    command_reply = self._execute_command(
+        createStatisticsCase=Commands_pb2.CreateStatisticsCaseRequest(
+            caseGroupId=self.group_id
+        )
+    )
+    return Case(self.channel, command_reply.createStatisticsCaseResult.caseId)
+
+
+@add_method(GridCaseGroup)
+def statistics_cases(self):
+    """Get a list of all statistics cases in the Grid Case Group
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.EclipseCase`
+
+    """
+    stat_case_collection = self.children("StatisticsCaseCollection")[0]
+    return stat_case_collection.children("Reservoirs")
+
+
+@add_method(GridCaseGroup)
+def views(self):
+    """Get a list of views belonging to a grid case group
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.EclipseView`
+
+    """
+    resinsight_classes = self.descendants(EclipseView)
+    view_list = []
+    for pdm_object in resinsight_classes:
+        view_list.append(pdm_object)
+    return view_list
+
+
+@add_method(GridCaseGroup)
+def view(self, view_id):
+    """Get a particular view belonging to a case group by providing view id
+
+    Arguments:
+        id(int): view id
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.EclipseView`
+
+    """
+    views = self.views()
+    for view_object in views:
+        if view_object.id == view_id:
+            return view_object
+    return None
+
+
+@add_method(GridCaseGroup)
+def compute_statistics(self, case_ids=None):
+    """Compute statistics for the given case ids
+
+    Arguments:
+        case_ids(list of integers): List of case ids. If this is None all cases in group are included
+
+    """
+    if case_ids is None:
+        case_ids = []
+    return self._execute_command(
+        computeCaseGroupStatistics=Commands_pb2.ComputeCaseGroupStatRequest(
+            caseIds=case_ids, caseGroupId=self.group_id
+        )
+    )
```

### Comparing `rips-2023.6.0.1/rips/grpc_retry_interceptor.py` & `rips-2023.6.0.2/rips/grpc_retry_interceptor.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import grpc
-
-
-class RetryOnRpcErrorClientInterceptor(
-    grpc.UnaryUnaryClientInterceptor, grpc.StreamUnaryClientInterceptor
-):
-    def __init__(
-        self,
-        *,
-        retry_policy,
-        status_for_retry,
-    ):
-        self.retry_policy = retry_policy
-        self.status_for_retry = status_for_retry
-
-    def _intercept_call(self, continuation, client_call_details, request_or_iterator):
-        for retry_num in range(self.retry_policy.num_retries()):
-            response = continuation(client_call_details, request_or_iterator)
-
-            if isinstance(response, grpc.RpcError):
-                # Return if it was last attempt
-                if retry_num == (self.retry_policy.num_retries() - 1):
-                    return response
-
-                # If status code is not in retryable status codes
-                if (
-                    self.status_for_retry
-                    and response.code() not in self.status_for_retry
-                ):
-                    return response
-
-                self.retry_policy.sleep(retry_num)
-            else:
-                return response
-
-    def intercept_unary_unary(self, continuation, client_call_details, request):
-        return self._intercept_call(continuation, client_call_details, request)
-
-    def intercept_stream_unary(
-        self, continuation, client_call_details, request_iterator
-    ):
-        return self._intercept_call(continuation, client_call_details, request_iterator)
+import grpc
+
+
+class RetryOnRpcErrorClientInterceptor(
+    grpc.UnaryUnaryClientInterceptor, grpc.StreamUnaryClientInterceptor
+):
+    def __init__(
+        self,
+        *,
+        retry_policy,
+        status_for_retry,
+    ):
+        self.retry_policy = retry_policy
+        self.status_for_retry = status_for_retry
+
+    def _intercept_call(self, continuation, client_call_details, request_or_iterator):
+        for retry_num in range(self.retry_policy.num_retries()):
+            response = continuation(client_call_details, request_or_iterator)
+
+            if isinstance(response, grpc.RpcError):
+                # Return if it was last attempt
+                if retry_num == (self.retry_policy.num_retries() - 1):
+                    return response
+
+                # If status code is not in retryable status codes
+                if (
+                    self.status_for_retry
+                    and response.code() not in self.status_for_retry
+                ):
+                    return response
+
+                self.retry_policy.sleep(retry_num)
+            else:
+                return response
+
+    def intercept_unary_unary(self, continuation, client_call_details, request):
+        return self._intercept_call(continuation, client_call_details, request)
+
+    def intercept_stream_unary(
+        self, continuation, client_call_details, request_iterator
+    ):
+        return self._intercept_call(continuation, client_call_details, request_iterator)
```

### Comparing `rips-2023.6.0.1/rips/instance.py` & `rips-2023.6.0.2/rips/instance.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,412 +1,412 @@
-# pylint: disable=no-self-use
-"""
-The main entry point for ResInsight connections
-The Instance class contained have static methods launch and find for
-creating connections to ResInsight
-"""
-
-import os
-import socket
-import logging
-import time
-import tempfile
-import signal
-
-import grpc
-
-import App_pb2
-import App_pb2_grpc
-import Commands_pb2
-import Commands_pb2_grpc
-from Definitions_pb2 import Empty
-
-import RiaVersionInfo
-
-from .project import Project
-from .retry_policy import ExponentialBackoffRetryPolicy
-from .grpc_retry_interceptor import RetryOnRpcErrorClientInterceptor
-from .generated.generated_classes import CommandRouter
-
-
-class Instance:
-    """The ResInsight Instance class. Use to launch or find existing ResInsight instances
-
-    Attributes:
-        launched (bool): Tells us whether the application was launched as a new process.
-            If the application was launched we may need to close it when exiting the script.
-        commands (Commands): Command executor. Set when creating an instance.
-        project (Project): Current project in ResInsight.
-            Set when creating an instance and updated when opening/closing projects.
-    """
-
-    @staticmethod
-    def __is_port_in_use(port):
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as my_socket:
-            my_socket.settimeout(0.2)
-            return my_socket.connect_ex(("localhost", port)) == 0
-
-    @staticmethod
-    def __is_valid_port(port):
-        location = "localhost:" + str(port)
-        channel = grpc.insecure_channel(
-            location, options=[("grpc.enable_http_proxy", False)]
-        )
-        app = App_pb2_grpc.AppStub(channel)
-        try:
-            app.GetVersion(Empty(), timeout=1)
-        except grpc.RpcError:
-            return False
-        return True
-
-    @staticmethod
-    def __read_port_number_from_file(file_path):
-        retry_count = 0
-        while not os.path.exists(file_path) and retry_count < 60:
-            time.sleep(1)
-            retry_count = retry_count + 1
-
-        print("Portnumber file retry count : ", retry_count)
-
-        if os.path.isfile(file_path):
-            with open(file_path) as f:
-                value = f.readline()
-                return int(value)
-        else:
-            return -1
-
-    @staticmethod
-    def __kill_process(pid):
-        """
-        Kill the process with a given pid.
-        """
-        if hasattr(signal, "CTRL_C_EVENT"):
-            # windows does not have kill
-            os.kill(pid, signal.CTRL_C_EVENT)
-        else:
-            # linux/unix
-            os.kill(pid, signal.SIGKILL)
-
-    @staticmethod
-    def launch(
-        resinsight_executable="",
-        console=False,
-        launch_port=-1,
-        command_line_parameters=None,
-    ):
-        """Launch a new Instance of ResInsight. This requires the environment variable
-        RESINSIGHT_EXECUTABLE to be set or the parameter resinsight_executable to be provided.
-        The RESINSIGHT_GRPC_PORT environment variable can be set to an alternative port number.
-
-        Args:
-            resinsight_executable (str): Path to a valid ResInsight executable. If set
-                will take precedence over what is provided in the RESINSIGHT_EXECUTABLE
-                environment variable.
-            console (bool): If True, launch as console application, without GUI.
-            launch_port(int): If -1 will use the default port 50051 or RESINSIGHT_GRPC_PORT
-                             if anything else, ResInsight will try to launch with this port.
-                             If 0 a random port will be used.
-            command_line_parameters(list): Additional parameters as string entries in the list.
-        Returns:
-            Instance: an instance object if it worked. None if not.
-        """
-
-        requested_port = 50051
-        port_env = os.environ.get("RESINSIGHT_GRPC_PORT")
-        if port_env:
-            requested_port = int(port_env)
-        if launch_port != -1:
-            requested_port = launch_port
-
-        if not resinsight_executable:
-            resinsight_executable = os.environ.get("RESINSIGHT_EXECUTABLE")
-            if not resinsight_executable:
-                print(
-                    "ERROR: Could not launch ResInsight because the environment variable"
-                    " RESINSIGHT_EXECUTABLE is not set"
-                )
-                return None
-
-        print("Trying to launch", resinsight_executable)
-
-        if command_line_parameters is None:
-            command_line_parameters = []
-        elif isinstance(command_line_parameters, str):
-            command_line_parameters = [str]
-
-        with tempfile.TemporaryDirectory() as tmp_dir_path:
-            port_number_file = tmp_dir_path + "/portnumber.txt"
-            parameters = [
-                "ResInsight",
-                "--server",
-                requested_port,
-                "--portnumberfile",
-                port_number_file,
-            ] + command_line_parameters
-            if console:
-                print("Launching as console app")
-                parameters.append("--console")
-
-            # Stringify all parameters
-            for i in range(0, len(parameters)):
-                parameters[i] = str(parameters[i])
-
-            pid = os.spawnv(os.P_NOWAIT, resinsight_executable, parameters)
-            if pid:
-                port = Instance.__read_port_number_from_file(port_number_file)
-                if port == -1:
-                    print("Unable to read port number. Launch failed.")
-                    # Need to kill the process using PID since there is no  GRPC connection to use.
-                    Instance.__kill_process(pid)
-                else:
-                    instance = Instance(port=port, launched=True)
-                    return instance
-        return None
-
-    @staticmethod
-    def find(start_port=50051, end_port=50071):
-        """Search for an existing Instance of ResInsight by testing ports.
-
-        By default we search from port 50051 to 50071 or if the environment
-        variable RESINSIGHT_GRPC_PORT is set we search
-        RESINSIGHT_GRPC_PORT to RESINSIGHT_GRPC_PORT+20
-
-        Args:
-            start_port (int): start searching from this port
-            end_port (int): search up to but not including this port
-        """
-        port_env = os.environ.get("RESINSIGHT_GRPC_PORT")
-        if port_env:
-            print("Got port " + port_env + " from environment")
-            start_port = int(port_env)
-            end_port = start_port + 20
-
-        for try_port in range(start_port, end_port):
-            print("Trying port " + str(try_port))
-            if Instance.__is_port_in_use(try_port) and Instance.__is_valid_port(
-                try_port
-            ):
-                return Instance(port=try_port)
-
-        print(
-            "Error: Could not find any ResInsight instances responding between ports "
-            + str(start_port)
-            + " and "
-            + str(end_port)
-        )
-        return None
-
-    def __execute_command(self, **command_params):
-        return self.commands.Execute(Commands_pb2.CommandParams(**command_params))
-
-    def __check_version(self):
-        try:
-            major_version_ok = self.major_version() == int(
-                RiaVersionInfo.RESINSIGHT_MAJOR_VERSION
-            )
-            minor_version_ok = self.minor_version() == int(
-                RiaVersionInfo.RESINSIGHT_MINOR_VERSION
-            )
-            return True, major_version_ok and minor_version_ok
-        except grpc.RpcError:
-            return False, False
-
-    def __init__(self, port=50051, launched=False):
-        """Attempts to connect to ResInsight at aa specific port on localhost
-
-        Args:
-            port(int): port number
-        """
-        logging.basicConfig()
-        self.location = "localhost:" + str(port)
-
-        self.channel = grpc.insecure_channel(
-            self.location, options=[("grpc.enable_http_proxy", False)]
-        )
-        self.launched = launched
-        self.commands = Commands_pb2_grpc.CommandsStub(self.channel)
-
-        # Main version check package
-        self.app = App_pb2_grpc.AppStub(self.channel)
-
-        self._check_connection_and_version(self.channel, launched, self.location)
-
-        # Intercept UNAVAILABLE errors and retry on failures
-        interceptors = (
-            RetryOnRpcErrorClientInterceptor(
-                retry_policy=ExponentialBackoffRetryPolicy(
-                    min_backoff=100, max_backoff=5000, max_num_retries=20
-                ),
-                status_for_retry=(grpc.StatusCode.UNAVAILABLE,),
-            ),
-        )
-
-        intercepted_channel = grpc.intercept_channel(self.channel, *interceptors)
-
-        # Recreate command stubs with the retry policy
-        self.commands = Commands_pb2_grpc.CommandsStub(intercepted_channel)
-
-        # Service packages
-        self.project = Project.create(intercepted_channel)
-
-        # Command Router object used as entry point for independent processing functions
-        self.command_router = CommandRouter(
-            self.app.GetPdmObject(Empty()), intercepted_channel
-        )
-
-        path = os.getcwd()
-        self.set_start_dir(path=path)
-
-    def _check_connection_and_version(self, channel, launched, location):
-        connection_ok = False
-        version_ok = False
-
-        retry_policy = ExponentialBackoffRetryPolicy()
-        if self.launched:
-            for num_tries in range(0, retry_policy.num_retries()):
-                connection_ok, version_ok = self.__check_version()
-                if connection_ok:
-                    break
-                retry_policy.sleep(num_tries)
-        else:
-            connection_ok, version_ok = self.__check_version()
-
-        if not connection_ok:
-            if self.launched:
-                raise Exception(
-                    "Error: Could not connect to resinsight at ",
-                    location,
-                    ".",
-                    retry_policy.time_out_message(),
-                )
-            raise Exception("Error: Could not connect to resinsight at ", location)
-        if not version_ok:
-            raise Exception(
-                "Error: Wrong Version of ResInsight at ",
-                location,
-                self.version_string(),
-                " ",
-                self.client_version_string(),
-            )
-
-    def __version_message(self):
-        return self.app.GetVersion(Empty())
-
-    def set_start_dir(self, path):
-        """Set current start directory
-
-        Arguments:
-            path (str): path to directory
-
-        """
-        return self.__execute_command(
-            setStartDir=Commands_pb2.FilePathRequest(path=path)
-        )
-
-    def set_export_folder(self, export_type, path, create_folder=False):
-        """
-        Set the export folder used for all export functions
-
-        **Parameters**::
-
-            Parameter        | Description                                  | Type
-            ---------------- | -------------------------------------------- | -----
-            export_type      | String specifying what to export             | String
-            path             | Path to folder                               | String
-            create_folder    | Create folder if it doesn't exist?           | Boolean
-
-        **Enum export_type**::
-
-            Option          | Description
-            --------------- | ------------
-            "COMPLETIONS"   |
-            "SNAPSHOTS"     |
-            "PROPERTIES"    |
-            "STATISTICS"    |
-
-        """
-        return self.__execute_command(
-            setExportFolder=Commands_pb2.SetExportFolderRequest(
-                type=export_type, path=path, createFolder=create_folder
-            )
-        )
-
-    def set_main_window_size(self, width, height):
-        """
-        Set the main window size in pixels
-
-        **Parameters**::
-
-            Parameter | Description      | Type
-            --------- | ---------------- | -----
-            width     | Width in pixels  | Integer
-            height    | Height in pixels | Integer
-
-        """
-        return self.__execute_command(
-            setMainWindowSize=Commands_pb2.SetWindowSizeParams(
-                width=width, height=height
-            )
-        )
-
-    def set_plot_window_size(self, width, height):
-        """
-        Set the plot window size in pixels
-
-        **Parameters**::
-
-            Parameter | Description      | Type
-            --------- | ---------------- | -----
-            width     | Width in pixels  | Integer
-            height    | Height in pixels | Integer
-        """
-        return self.__execute_command(
-            setPlotWindowSize=Commands_pb2.SetWindowSizeParams(
-                width=width, height=height
-            )
-        )
-
-    def major_version(self):
-        """Get an integer with the major version number"""
-        return self.__version_message().major_version
-
-    def minor_version(self):
-        """Get an integer with the minor version number"""
-        return self.__version_message().minor_version
-
-    def patch_version(self):
-        """Get an integer with the patch version number"""
-        return self.__version_message().patch_version
-
-    def version_string(self):
-        """Get a full version string, i.e. 2019.04.01"""
-        return (
-            str(self.major_version())
-            + "."
-            + str(self.minor_version())
-            + "."
-            + str(self.patch_version())
-        )
-
-    def client_version_string(self):
-        """Get a full version string, i.e. 2019.04.01"""
-        version_string = RiaVersionInfo.RESINSIGHT_MAJOR_VERSION + "."
-        version_string += RiaVersionInfo.RESINSIGHT_MINOR_VERSION + "."
-        version_string += RiaVersionInfo.RESINSIGHT_PATCH_VERSION
-        return version_string
-
-    def exit(self):
-        """Tell ResInsight instance to quit"""
-        print("Telling ResInsight to Exit")
-        return self.app.Exit(Empty())
-
-    def is_console(self):
-        """Returns true if the connected ResInsight instance is a console app"""
-        return self.app.GetRuntimeInfo(
-            Empty()
-        ).app_type == App_pb2.ApplicationTypeEnum.Value("CONSOLE_APPLICATION")
-
-    def is_gui(self):
-        """Returns true if the connected ResInsight instance is a GUI app"""
-        return self.app.GetRuntimeInfo(
-            Empty()
-        ).app_type == App_pb2.ApplicationTypeEnum.Value("GUI_APPLICATION")
+# pylint: disable=no-self-use
+"""
+The main entry point for ResInsight connections
+The Instance class contained have static methods launch and find for
+creating connections to ResInsight
+"""
+
+import os
+import socket
+import logging
+import time
+import tempfile
+import signal
+
+import grpc
+
+import App_pb2
+import App_pb2_grpc
+import Commands_pb2
+import Commands_pb2_grpc
+from Definitions_pb2 import Empty
+
+import RiaVersionInfo
+
+from .project import Project
+from .retry_policy import ExponentialBackoffRetryPolicy
+from .grpc_retry_interceptor import RetryOnRpcErrorClientInterceptor
+from .generated.generated_classes import CommandRouter
+
+
+class Instance:
+    """The ResInsight Instance class. Use to launch or find existing ResInsight instances
+
+    Attributes:
+        launched (bool): Tells us whether the application was launched as a new process.
+            If the application was launched we may need to close it when exiting the script.
+        commands (Commands): Command executor. Set when creating an instance.
+        project (Project): Current project in ResInsight.
+            Set when creating an instance and updated when opening/closing projects.
+    """
+
+    @staticmethod
+    def __is_port_in_use(port):
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as my_socket:
+            my_socket.settimeout(0.2)
+            return my_socket.connect_ex(("localhost", port)) == 0
+
+    @staticmethod
+    def __is_valid_port(port):
+        location = "localhost:" + str(port)
+        channel = grpc.insecure_channel(
+            location, options=[("grpc.enable_http_proxy", False)]
+        )
+        app = App_pb2_grpc.AppStub(channel)
+        try:
+            app.GetVersion(Empty(), timeout=1)
+        except grpc.RpcError:
+            return False
+        return True
+
+    @staticmethod
+    def __read_port_number_from_file(file_path):
+        retry_count = 0
+        while not os.path.exists(file_path) and retry_count < 60:
+            time.sleep(1)
+            retry_count = retry_count + 1
+
+        print("Portnumber file retry count : ", retry_count)
+
+        if os.path.isfile(file_path):
+            with open(file_path) as f:
+                value = f.readline()
+                return int(value)
+        else:
+            return -1
+
+    @staticmethod
+    def __kill_process(pid):
+        """
+        Kill the process with a given pid.
+        """
+        if hasattr(signal, "CTRL_C_EVENT"):
+            # windows does not have kill
+            os.kill(pid, signal.CTRL_C_EVENT)
+        else:
+            # linux/unix
+            os.kill(pid, signal.SIGKILL)
+
+    @staticmethod
+    def launch(
+        resinsight_executable="",
+        console=False,
+        launch_port=-1,
+        command_line_parameters=None,
+    ):
+        """Launch a new Instance of ResInsight. This requires the environment variable
+        RESINSIGHT_EXECUTABLE to be set or the parameter resinsight_executable to be provided.
+        The RESINSIGHT_GRPC_PORT environment variable can be set to an alternative port number.
+
+        Args:
+            resinsight_executable (str): Path to a valid ResInsight executable. If set
+                will take precedence over what is provided in the RESINSIGHT_EXECUTABLE
+                environment variable.
+            console (bool): If True, launch as console application, without GUI.
+            launch_port(int): If -1 will use the default port 50051 or RESINSIGHT_GRPC_PORT
+                             if anything else, ResInsight will try to launch with this port.
+                             If 0 a random port will be used.
+            command_line_parameters(list): Additional parameters as string entries in the list.
+        Returns:
+            Instance: an instance object if it worked. None if not.
+        """
+
+        requested_port = 50051
+        port_env = os.environ.get("RESINSIGHT_GRPC_PORT")
+        if port_env:
+            requested_port = int(port_env)
+        if launch_port != -1:
+            requested_port = launch_port
+
+        if not resinsight_executable:
+            resinsight_executable = os.environ.get("RESINSIGHT_EXECUTABLE")
+            if not resinsight_executable:
+                print(
+                    "ERROR: Could not launch ResInsight because the environment variable"
+                    " RESINSIGHT_EXECUTABLE is not set"
+                )
+                return None
+
+        print("Trying to launch", resinsight_executable)
+
+        if command_line_parameters is None:
+            command_line_parameters = []
+        elif isinstance(command_line_parameters, str):
+            command_line_parameters = [str]
+
+        with tempfile.TemporaryDirectory() as tmp_dir_path:
+            port_number_file = tmp_dir_path + "/portnumber.txt"
+            parameters = [
+                "ResInsight",
+                "--server",
+                requested_port,
+                "--portnumberfile",
+                port_number_file,
+            ] + command_line_parameters
+            if console:
+                print("Launching as console app")
+                parameters.append("--console")
+
+            # Stringify all parameters
+            for i in range(0, len(parameters)):
+                parameters[i] = str(parameters[i])
+
+            pid = os.spawnv(os.P_NOWAIT, resinsight_executable, parameters)
+            if pid:
+                port = Instance.__read_port_number_from_file(port_number_file)
+                if port == -1:
+                    print("Unable to read port number. Launch failed.")
+                    # Need to kill the process using PID since there is no  GRPC connection to use.
+                    Instance.__kill_process(pid)
+                else:
+                    instance = Instance(port=port, launched=True)
+                    return instance
+        return None
+
+    @staticmethod
+    def find(start_port=50051, end_port=50071):
+        """Search for an existing Instance of ResInsight by testing ports.
+
+        By default we search from port 50051 to 50071 or if the environment
+        variable RESINSIGHT_GRPC_PORT is set we search
+        RESINSIGHT_GRPC_PORT to RESINSIGHT_GRPC_PORT+20
+
+        Args:
+            start_port (int): start searching from this port
+            end_port (int): search up to but not including this port
+        """
+        port_env = os.environ.get("RESINSIGHT_GRPC_PORT")
+        if port_env:
+            print("Got port " + port_env + " from environment")
+            start_port = int(port_env)
+            end_port = start_port + 20
+
+        for try_port in range(start_port, end_port):
+            print("Trying port " + str(try_port))
+            if Instance.__is_port_in_use(try_port) and Instance.__is_valid_port(
+                try_port
+            ):
+                return Instance(port=try_port)
+
+        print(
+            "Error: Could not find any ResInsight instances responding between ports "
+            + str(start_port)
+            + " and "
+            + str(end_port)
+        )
+        return None
+
+    def __execute_command(self, **command_params):
+        return self.commands.Execute(Commands_pb2.CommandParams(**command_params))
+
+    def __check_version(self):
+        try:
+            major_version_ok = self.major_version() == int(
+                RiaVersionInfo.RESINSIGHT_MAJOR_VERSION
+            )
+            minor_version_ok = self.minor_version() == int(
+                RiaVersionInfo.RESINSIGHT_MINOR_VERSION
+            )
+            return True, major_version_ok and minor_version_ok
+        except grpc.RpcError:
+            return False, False
+
+    def __init__(self, port=50051, launched=False):
+        """Attempts to connect to ResInsight at aa specific port on localhost
+
+        Args:
+            port(int): port number
+        """
+        logging.basicConfig()
+        self.location = "localhost:" + str(port)
+
+        self.channel = grpc.insecure_channel(
+            self.location, options=[("grpc.enable_http_proxy", False)]
+        )
+        self.launched = launched
+        self.commands = Commands_pb2_grpc.CommandsStub(self.channel)
+
+        # Main version check package
+        self.app = App_pb2_grpc.AppStub(self.channel)
+
+        self._check_connection_and_version(self.channel, launched, self.location)
+
+        # Intercept UNAVAILABLE errors and retry on failures
+        interceptors = (
+            RetryOnRpcErrorClientInterceptor(
+                retry_policy=ExponentialBackoffRetryPolicy(
+                    min_backoff=100, max_backoff=5000, max_num_retries=20
+                ),
+                status_for_retry=(grpc.StatusCode.UNAVAILABLE,),
+            ),
+        )
+
+        intercepted_channel = grpc.intercept_channel(self.channel, *interceptors)
+
+        # Recreate command stubs with the retry policy
+        self.commands = Commands_pb2_grpc.CommandsStub(intercepted_channel)
+
+        # Service packages
+        self.project = Project.create(intercepted_channel)
+
+        # Command Router object used as entry point for independent processing functions
+        self.command_router = CommandRouter(
+            self.app.GetPdmObject(Empty()), intercepted_channel
+        )
+
+        path = os.getcwd()
+        self.set_start_dir(path=path)
+
+    def _check_connection_and_version(self, channel, launched, location):
+        connection_ok = False
+        version_ok = False
+
+        retry_policy = ExponentialBackoffRetryPolicy()
+        if self.launched:
+            for num_tries in range(0, retry_policy.num_retries()):
+                connection_ok, version_ok = self.__check_version()
+                if connection_ok:
+                    break
+                retry_policy.sleep(num_tries)
+        else:
+            connection_ok, version_ok = self.__check_version()
+
+        if not connection_ok:
+            if self.launched:
+                raise Exception(
+                    "Error: Could not connect to resinsight at ",
+                    location,
+                    ".",
+                    retry_policy.time_out_message(),
+                )
+            raise Exception("Error: Could not connect to resinsight at ", location)
+        if not version_ok:
+            raise Exception(
+                "Error: Wrong Version of ResInsight at ",
+                location,
+                self.version_string(),
+                " ",
+                self.client_version_string(),
+            )
+
+    def __version_message(self):
+        return self.app.GetVersion(Empty())
+
+    def set_start_dir(self, path):
+        """Set current start directory
+
+        Arguments:
+            path (str): path to directory
+
+        """
+        return self.__execute_command(
+            setStartDir=Commands_pb2.FilePathRequest(path=path)
+        )
+
+    def set_export_folder(self, export_type, path, create_folder=False):
+        """
+        Set the export folder used for all export functions
+
+        **Parameters**::
+
+            Parameter        | Description                                  | Type
+            ---------------- | -------------------------------------------- | -----
+            export_type      | String specifying what to export             | String
+            path             | Path to folder                               | String
+            create_folder    | Create folder if it doesn't exist?           | Boolean
+
+        **Enum export_type**::
+
+            Option          | Description
+            --------------- | ------------
+            "COMPLETIONS"   |
+            "SNAPSHOTS"     |
+            "PROPERTIES"    |
+            "STATISTICS"    |
+
+        """
+        return self.__execute_command(
+            setExportFolder=Commands_pb2.SetExportFolderRequest(
+                type=export_type, path=path, createFolder=create_folder
+            )
+        )
+
+    def set_main_window_size(self, width, height):
+        """
+        Set the main window size in pixels
+
+        **Parameters**::
+
+            Parameter | Description      | Type
+            --------- | ---------------- | -----
+            width     | Width in pixels  | Integer
+            height    | Height in pixels | Integer
+
+        """
+        return self.__execute_command(
+            setMainWindowSize=Commands_pb2.SetWindowSizeParams(
+                width=width, height=height
+            )
+        )
+
+    def set_plot_window_size(self, width, height):
+        """
+        Set the plot window size in pixels
+
+        **Parameters**::
+
+            Parameter | Description      | Type
+            --------- | ---------------- | -----
+            width     | Width in pixels  | Integer
+            height    | Height in pixels | Integer
+        """
+        return self.__execute_command(
+            setPlotWindowSize=Commands_pb2.SetWindowSizeParams(
+                width=width, height=height
+            )
+        )
+
+    def major_version(self):
+        """Get an integer with the major version number"""
+        return self.__version_message().major_version
+
+    def minor_version(self):
+        """Get an integer with the minor version number"""
+        return self.__version_message().minor_version
+
+    def patch_version(self):
+        """Get an integer with the patch version number"""
+        return self.__version_message().patch_version
+
+    def version_string(self):
+        """Get a full version string, i.e. 2019.04.01"""
+        return (
+            str(self.major_version())
+            + "."
+            + str(self.minor_version())
+            + "."
+            + str(self.patch_version())
+        )
+
+    def client_version_string(self):
+        """Get a full version string, i.e. 2019.04.01"""
+        version_string = RiaVersionInfo.RESINSIGHT_MAJOR_VERSION + "."
+        version_string += RiaVersionInfo.RESINSIGHT_MINOR_VERSION + "."
+        version_string += RiaVersionInfo.RESINSIGHT_PATCH_VERSION
+        return version_string
+
+    def exit(self):
+        """Tell ResInsight instance to quit"""
+        print("Telling ResInsight to Exit")
+        return self.app.Exit(Empty())
+
+    def is_console(self):
+        """Returns true if the connected ResInsight instance is a console app"""
+        return self.app.GetRuntimeInfo(
+            Empty()
+        ).app_type == App_pb2.ApplicationTypeEnum.Value("CONSOLE_APPLICATION")
+
+    def is_gui(self):
+        """Returns true if the connected ResInsight instance is a GUI app"""
+        return self.app.GetRuntimeInfo(
+            Empty()
+        ).app_type == App_pb2.ApplicationTypeEnum.Value("GUI_APPLICATION")
```

### Comparing `rips-2023.6.0.1/rips/plot.py` & `rips-2023.6.0.2/rips/plot.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""
-ResInsight 2d plot module
-"""
-import Commands_pb2
-
-from .pdmobject import add_method
-from .resinsight_classes import PlotWindow, Plot
-
-
-@add_method(PlotWindow)
-def export_snapshot(self, export_folder="", file_prefix="", output_format="PNG"):
-    """Export snapshot for the current plot
-
-    Arguments:
-        export_folder(str): The path to export to. By default will use the global export folder
-        prefix (str): Exported file name prefix
-        output_format(str): Enum string. Can be 'PNG' or 'PDF'.
-
-    """
-    return self._execute_command(
-        exportSnapshots=Commands_pb2.ExportSnapshotsRequest(
-            type="PLOTS",
-            prefix=file_prefix,
-            viewId=self.id,
-            exportFolder=export_folder,
-            plotOutputFormat=output_format,
-        )
-    )
+"""
+ResInsight 2d plot module
+"""
+import Commands_pb2
+
+from .pdmobject import add_method
+from .resinsight_classes import PlotWindow, Plot
+
+
+@add_method(PlotWindow)
+def export_snapshot(self, export_folder="", file_prefix="", output_format="PNG"):
+    """Export snapshot for the current plot
+
+    Arguments:
+        export_folder(str): The path to export to. By default will use the global export folder
+        prefix (str): Exported file name prefix
+        output_format(str): Enum string. Can be 'PNG' or 'PDF'.
+
+    """
+    return self._execute_command(
+        exportSnapshots=Commands_pb2.ExportSnapshotsRequest(
+            type="PLOTS",
+            prefix=file_prefix,
+            viewId=self.id,
+            exportFolder=export_folder,
+            plotOutputFormat=output_format,
+        )
+    )
```

### Comparing `rips-2023.6.0.1/rips/project.py` & `rips-2023.6.0.2/rips/project.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,424 +1,424 @@
-# pylint: disable=too-many-arguments
-# pylint: disable=no-member
-"""
-The ResInsight project module
-"""
-import builtins
-import grpc
-
-from .case import Case
-from .gridcasegroup import GridCaseGroup
-from .pdmobject import PdmObjectBase, add_method, add_static_method
-from .plot import Plot
-from .view import View
-
-import Commands_pb2
-from Definitions_pb2 import Empty
-import Project_pb2_grpc
-import Project_pb2
-import PdmObject_pb2
-from .resinsight_classes import Project, PlotWindow, WellPath, SummaryCase
-
-
-@add_method(Project)
-def __custom_init__(self, pb2_object, channel):
-    self._project_stub = Project_pb2_grpc.ProjectStub(self._channel)
-
-
-@add_static_method(Project)
-def create(channel):
-    project_stub = Project_pb2_grpc.ProjectStub(channel)
-    pb2_object = project_stub.GetPdmObject(Empty())
-    return Project(pb2_object, channel)
-
-
-@add_method(Project)
-def open(self, path):
-    """Open a new project from the given path
-
-    Arguments:
-        path(str): path to project file
-
-    """
-    self._execute_command(openProject=Commands_pb2.FilePathRequest(path=path))
-    return self
-
-
-@add_method(Project)
-def save(self, path=""):
-    """Save the project to the existing project file, or to a new file
-
-    Arguments:
-        path(str): File path to the file to save the project to. If empty, saves to the active project file
-    """
-    self._execute_command(saveProject=Commands_pb2.SaveProjectRequest(filePath=path))
-    return self
-
-
-@add_method(Project)
-def close(self):
-    """Close the current project (and open new blank project)"""
-    self._execute_command(closeProject=Empty())
-
-
-@add_method(Project)
-def load_case(self, path, grid_only=False):
-    """Load a new grid case from the given file path
-
-    Arguments:
-        path(str): file path to case
-    Returns:
-        :class:`rips.generated.generated_classes.Case`
-    """
-    command_reply = self._execute_command(
-        loadCase=Commands_pb2.FilePathRequest(path=path, gridOnly=grid_only)
-    )
-    return self.case(command_reply.loadCaseResult.id)
-
-
-@add_method(Project)
-def selected_cases(self):
-    """Get a list of all grid cases selected in the project tree
-
-    Returns:
-        A list of :class:`rips.generated.generated_classes.Case`
-    """
-    case_infos = self._project_stub.GetSelectedCases(Empty())
-    cases = []
-    for case_info in case_infos.data:
-        cases.append(self.case(case_info.id))
-    return cases
-
-
-@add_method(Project)
-def cases(self):
-    """Get a list of all grid cases in the project
-
-    Returns:
-        A list of :class:`rips.generated.generated_classes.Case`
-    """
-    return self.descendants(Case)
-
-
-@add_method(Project)
-def case(self, case_id):
-    """Get a specific grid case from the provided case Id
-
-    Arguments:
-        id(int): case id
-    Returns:
-        :class:`rips.generated.resinsight_classes.Case`
-    """
-    allCases = self.cases()
-    for case in allCases:
-        if case.id == case_id:
-            return case
-    return None
-
-
-@add_method(Project)
-def replace_source_cases(self, grid_list_file, case_group_id=0):
-    """Replace all source grid cases within a case group
-
-    Arguments:
-        grid_list_file (str): path to file containing a list of cases
-        case_group_id (int): id of the case group to replace
-    """
-    return self._execute_command(
-        replaceSourceCases=Commands_pb2.ReplaceSourceCasesRequest(
-            gridListFile=grid_list_file, caseGroupId=case_group_id
-        )
-    )
-
-
-@add_method(Project)
-def create_grid_case_group(self, case_paths):
-    """Create a Grid Case Group from a list of cases
-
-    Arguments:
-        case_paths (list): list of file path strings
-    Returns:
-        :class:`rips.generated.resinsight_classes.GridCaseGroup`
-    """
-    command_reply = self._execute_command(
-        createGridCaseGroup=Commands_pb2.CreateGridCaseGroupRequest(
-            casePaths=case_paths
-        )
-    )
-    return self.grid_case_group(command_reply.createGridCaseGroupResult.groupId)
-
-
-@add_method(Project)
-def summary_cases(self):
-    """Get a list of all summary cases in the Project
-
-    Returns: A list of :class:`rips.generated.resinsight_classes.SummaryCase`
-    """
-    return self.descendants(SummaryCase)
-
-
-@add_method(Project)
-def views(self):
-    """Get a list of views belonging to a project"""
-    return self.descendants(View)
-
-
-@add_method(Project)
-def view(self, view_id):
-    """Get a particular view belonging to a case by providing view id
-
-    Arguments:
-        view_id(int): view id
-    Returns:
-        :class:`rips.generated.generated_classes.View`
-    """
-    views = self.views()
-    for view_object in views:
-        if view_object.id == view_id:
-            return view_object
-    return None
-
-
-@add_method(Project)
-def plots(self):
-    """Get a list of all plots belonging to a project
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.Plot`
-    """
-    resinsight_classes = self.descendants(PlotWindow)
-    plot_list = []
-    for pdm_object in resinsight_classes:
-        if pdm_object.id != -1:
-            plot_list.append(pdm_object)
-    return plot_list
-
-
-@add_method(Project)
-def plot(self, view_id):
-    """Get a particular plot by providing view id
-
-    Arguments:
-        view_id(int): view id
-
-    Returns:
-        :class:`rips.generated.generated_classes.Plot`
-    """
-    plots = self.plots()
-    for plot_object in plots:
-        if plot_object.id == view_id:
-            return plot_object
-    return None
-
-
-@add_method(Project)
-def grid_case_groups(self):
-    """Get a list of all grid case groups in the project
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.GridCaseGroup`
-
-    """
-    case_groups = self.descendants(GridCaseGroup)
-    return case_groups
-
-
-@add_method(Project)
-def grid_case_group(self, group_id):
-    """Get a particular grid case group belonging to a project
-
-    Arguments:
-        groupId(int): group id
-
-    Returns:
-        :class:`rips.generated.generated_classes.GridCaseGroup`
-    """
-    case_groups = self.grid_case_groups()
-    for case_group in case_groups:
-        if case_group.group_id == group_id:
-            return case_group
-    return None
-
-
-@add_method(Project)
-def export_multi_case_snapshots(self, grid_list_file):
-    """Export snapshots for a set of cases
-
-    Arguments:
-        grid_list_file (str): Path to a file containing a list of grids to export snapshot for
-    """
-    return self._execute_command(
-        exportMultiCaseSnapshot=Commands_pb2.ExportMultiCaseRequest(
-            gridListFile=grid_list_file
-        )
-    )
-
-
-@add_method(Project)
-def export_snapshots(self, snapshot_type="ALL", prefix="", plot_format="PNG"):
-    """Export all snapshots of a given type
-
-    Arguments:
-        snapshot_type (str): Enum string ('ALL', 'VIEWS' or 'PLOTS')
-        prefix (str): Exported file name prefix
-        plot_format(str): Enum string, 'PNG' or 'PDF'
-    """
-    return self._execute_command(
-        exportSnapshots=Commands_pb2.ExportSnapshotsRequest(
-            type=snapshot_type,
-            prefix=prefix,
-            caseId=-1,
-            viewId=-1,
-            plotOutputFormat=plot_format,
-        )
-    )
-
-
-@add_method(Project)
-def export_well_paths(self, well_paths=None, md_step_size=5.0):
-    """Export a set of well paths
-
-    Arguments:
-        well_paths(list): List of strings of well paths. If none, export all.
-        md_step_size(double): resolution of the exported well path
-    """
-    if well_paths is None:
-        well_paths = []
-    elif isinstance(well_paths, str):
-        well_paths = [well_paths]
-    return self._execute_command(
-        exportWellPaths=Commands_pb2.ExportWellPathRequest(
-            wellPathNames=well_paths, mdStepSize=md_step_size
-        )
-    )
-
-
-@add_method(Project)
-def scale_fracture_template(
-    self, template_id, half_length, height, d_factor, conductivity
-):
-    """Scale fracture template parameters
-
-    Arguments:
-        template_id(int): ID of fracture template
-        half_length (double): Half Length scale factor
-        height (double): Height scale factor
-        d_factor (double): D-factor scale factor
-        conductivity (double): Conductivity scale factor
-    """
-    return self._execute_command(
-        scaleFractureTemplate=Commands_pb2.ScaleFractureTemplateRequest(
-            id=template_id,
-            halfLength=half_length,
-            height=height,
-            dFactor=d_factor,
-            conductivity=conductivity,
-        )
-    )
-
-
-@add_method(Project)
-def set_fracture_containment(self, template_id, top_layer, base_layer):
-    """Set fracture template containment parameters
-
-    Arguments:
-        template_id(int): ID of fracture template
-        top_layer (int): Top layer containment
-        base_layer (int): Base layer containment
-    """
-    return self._execute_command(
-        setFractureContainment=Commands_pb2.SetFracContainmentRequest(
-            id=template_id, topLayer=top_layer, baseLayer=base_layer
-        )
-    )
-
-
-@add_method(Project)
-def import_well_paths(self, well_path_files=None, well_path_folder=""):
-    """Import well paths into project
-
-    Arguments:
-        well_path_files(list): List of file paths to import
-        well_path_folder(str): A folder path containing files to import
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.WellPath`
-    """
-    if well_path_files is None:
-        well_path_files = []
-
-    res = self._execute_command(
-        importWellPaths=Commands_pb2.ImportWellPathsRequest(
-            wellPathFolder=well_path_folder, wellPathFiles=well_path_files
-        )
-    )
-    well_paths = []
-    for well_path_name in res.importWellPathsResult.wellPathNames:
-        well_paths.append(self.well_path_by_name(well_path_name))
-    return well_paths
-
-
-@add_method(Project)
-def well_paths(self):
-    """Get a list of all well paths in the project
-
-    Returns:
-        List of :class:`rips.generated.generated_classes.WellPath`
-    """
-    return self.descendants(WellPath)
-
-
-@add_method(Project)
-def well_path_by_name(self, well_path_name):
-    """Get a specific well path by name from the project
-
-    Returns:
-        :class:`rips.generated.generated_classes.WellPath`
-    """
-    all_well_paths = self.well_paths()
-    for well_path in all_well_paths:
-        if well_path.name == well_path_name:
-            return well_path
-    return None
-
-
-@add_method(Project)
-def import_well_log_files(self, well_log_files=None, well_log_folder=""):
-    """Import well log files into project
-
-    Arguments:
-        well_log_files(list): List of file paths to import
-        well_log_folder(str): A folder path containing files to import
-
-    Returns:
-        A list of well path names (strings) that had logs imported
-    """
-
-    if well_log_files is None:
-        well_log_files = []
-    res = self._execute_command(
-        importWellLogFiles=Commands_pb2.ImportWellLogFilesRequest(
-            wellLogFolder=well_log_folder, wellLogFiles=well_log_files
-        )
-    )
-    return res.importWellLogFilesResult.wellPathNames
-
-
-@add_method(Project)
-def import_formation_names(self, formation_files=None):
-    """Import formation names into project
-
-    Arguments:
-        formation_files(list): list of files to import
-
-    """
-    if formation_files is None:
-        formation_files = []
-    elif isinstance(formation_files, str):
-        formation_files = [formation_files]
-
-    self._execute_command(
-        importFormationNames=Commands_pb2.ImportFormationNamesRequest(
-            formationFiles=formation_files, applyToCaseId=-1
-        )
-    )
+# pylint: disable=too-many-arguments
+# pylint: disable=no-member
+"""
+The ResInsight project module
+"""
+import builtins
+import grpc
+
+from .case import Case
+from .gridcasegroup import GridCaseGroup
+from .pdmobject import PdmObjectBase, add_method, add_static_method
+from .plot import Plot
+from .view import View
+
+import Commands_pb2
+from Definitions_pb2 import Empty
+import Project_pb2_grpc
+import Project_pb2
+import PdmObject_pb2
+from .resinsight_classes import Project, PlotWindow, WellPath, SummaryCase
+
+
+@add_method(Project)
+def __custom_init__(self, pb2_object, channel):
+    self._project_stub = Project_pb2_grpc.ProjectStub(self._channel)
+
+
+@add_static_method(Project)
+def create(channel):
+    project_stub = Project_pb2_grpc.ProjectStub(channel)
+    pb2_object = project_stub.GetPdmObject(Empty())
+    return Project(pb2_object, channel)
+
+
+@add_method(Project)
+def open(self, path):
+    """Open a new project from the given path
+
+    Arguments:
+        path(str): path to project file
+
+    """
+    self._execute_command(openProject=Commands_pb2.FilePathRequest(path=path))
+    return self
+
+
+@add_method(Project)
+def save(self, path=""):
+    """Save the project to the existing project file, or to a new file
+
+    Arguments:
+        path(str): File path to the file to save the project to. If empty, saves to the active project file
+    """
+    self._execute_command(saveProject=Commands_pb2.SaveProjectRequest(filePath=path))
+    return self
+
+
+@add_method(Project)
+def close(self):
+    """Close the current project (and open new blank project)"""
+    self._execute_command(closeProject=Empty())
+
+
+@add_method(Project)
+def load_case(self, path, grid_only=False):
+    """Load a new grid case from the given file path
+
+    Arguments:
+        path(str): file path to case
+    Returns:
+        :class:`rips.generated.generated_classes.Case`
+    """
+    command_reply = self._execute_command(
+        loadCase=Commands_pb2.FilePathRequest(path=path, gridOnly=grid_only)
+    )
+    return self.case(command_reply.loadCaseResult.id)
+
+
+@add_method(Project)
+def selected_cases(self):
+    """Get a list of all grid cases selected in the project tree
+
+    Returns:
+        A list of :class:`rips.generated.generated_classes.Case`
+    """
+    case_infos = self._project_stub.GetSelectedCases(Empty())
+    cases = []
+    for case_info in case_infos.data:
+        cases.append(self.case(case_info.id))
+    return cases
+
+
+@add_method(Project)
+def cases(self):
+    """Get a list of all grid cases in the project
+
+    Returns:
+        A list of :class:`rips.generated.generated_classes.Case`
+    """
+    return self.descendants(Case)
+
+
+@add_method(Project)
+def case(self, case_id):
+    """Get a specific grid case from the provided case Id
+
+    Arguments:
+        id(int): case id
+    Returns:
+        :class:`rips.generated.resinsight_classes.Case`
+    """
+    allCases = self.cases()
+    for case in allCases:
+        if case.id == case_id:
+            return case
+    return None
+
+
+@add_method(Project)
+def replace_source_cases(self, grid_list_file, case_group_id=0):
+    """Replace all source grid cases within a case group
+
+    Arguments:
+        grid_list_file (str): path to file containing a list of cases
+        case_group_id (int): id of the case group to replace
+    """
+    return self._execute_command(
+        replaceSourceCases=Commands_pb2.ReplaceSourceCasesRequest(
+            gridListFile=grid_list_file, caseGroupId=case_group_id
+        )
+    )
+
+
+@add_method(Project)
+def create_grid_case_group(self, case_paths):
+    """Create a Grid Case Group from a list of cases
+
+    Arguments:
+        case_paths (list): list of file path strings
+    Returns:
+        :class:`rips.generated.resinsight_classes.GridCaseGroup`
+    """
+    command_reply = self._execute_command(
+        createGridCaseGroup=Commands_pb2.CreateGridCaseGroupRequest(
+            casePaths=case_paths
+        )
+    )
+    return self.grid_case_group(command_reply.createGridCaseGroupResult.groupId)
+
+
+@add_method(Project)
+def summary_cases(self):
+    """Get a list of all summary cases in the Project
+
+    Returns: A list of :class:`rips.generated.resinsight_classes.SummaryCase`
+    """
+    return self.descendants(SummaryCase)
+
+
+@add_method(Project)
+def views(self):
+    """Get a list of views belonging to a project"""
+    return self.descendants(View)
+
+
+@add_method(Project)
+def view(self, view_id):
+    """Get a particular view belonging to a case by providing view id
+
+    Arguments:
+        view_id(int): view id
+    Returns:
+        :class:`rips.generated.generated_classes.View`
+    """
+    views = self.views()
+    for view_object in views:
+        if view_object.id == view_id:
+            return view_object
+    return None
+
+
+@add_method(Project)
+def plots(self):
+    """Get a list of all plots belonging to a project
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.Plot`
+    """
+    resinsight_classes = self.descendants(PlotWindow)
+    plot_list = []
+    for pdm_object in resinsight_classes:
+        if pdm_object.id != -1:
+            plot_list.append(pdm_object)
+    return plot_list
+
+
+@add_method(Project)
+def plot(self, view_id):
+    """Get a particular plot by providing view id
+
+    Arguments:
+        view_id(int): view id
+
+    Returns:
+        :class:`rips.generated.generated_classes.Plot`
+    """
+    plots = self.plots()
+    for plot_object in plots:
+        if plot_object.id == view_id:
+            return plot_object
+    return None
+
+
+@add_method(Project)
+def grid_case_groups(self):
+    """Get a list of all grid case groups in the project
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.GridCaseGroup`
+
+    """
+    case_groups = self.descendants(GridCaseGroup)
+    return case_groups
+
+
+@add_method(Project)
+def grid_case_group(self, group_id):
+    """Get a particular grid case group belonging to a project
+
+    Arguments:
+        groupId(int): group id
+
+    Returns:
+        :class:`rips.generated.generated_classes.GridCaseGroup`
+    """
+    case_groups = self.grid_case_groups()
+    for case_group in case_groups:
+        if case_group.group_id == group_id:
+            return case_group
+    return None
+
+
+@add_method(Project)
+def export_multi_case_snapshots(self, grid_list_file):
+    """Export snapshots for a set of cases
+
+    Arguments:
+        grid_list_file (str): Path to a file containing a list of grids to export snapshot for
+    """
+    return self._execute_command(
+        exportMultiCaseSnapshot=Commands_pb2.ExportMultiCaseRequest(
+            gridListFile=grid_list_file
+        )
+    )
+
+
+@add_method(Project)
+def export_snapshots(self, snapshot_type="ALL", prefix="", plot_format="PNG"):
+    """Export all snapshots of a given type
+
+    Arguments:
+        snapshot_type (str): Enum string ('ALL', 'VIEWS' or 'PLOTS')
+        prefix (str): Exported file name prefix
+        plot_format(str): Enum string, 'PNG' or 'PDF'
+    """
+    return self._execute_command(
+        exportSnapshots=Commands_pb2.ExportSnapshotsRequest(
+            type=snapshot_type,
+            prefix=prefix,
+            caseId=-1,
+            viewId=-1,
+            plotOutputFormat=plot_format,
+        )
+    )
+
+
+@add_method(Project)
+def export_well_paths(self, well_paths=None, md_step_size=5.0):
+    """Export a set of well paths
+
+    Arguments:
+        well_paths(list): List of strings of well paths. If none, export all.
+        md_step_size(double): resolution of the exported well path
+    """
+    if well_paths is None:
+        well_paths = []
+    elif isinstance(well_paths, str):
+        well_paths = [well_paths]
+    return self._execute_command(
+        exportWellPaths=Commands_pb2.ExportWellPathRequest(
+            wellPathNames=well_paths, mdStepSize=md_step_size
+        )
+    )
+
+
+@add_method(Project)
+def scale_fracture_template(
+    self, template_id, half_length, height, d_factor, conductivity
+):
+    """Scale fracture template parameters
+
+    Arguments:
+        template_id(int): ID of fracture template
+        half_length (double): Half Length scale factor
+        height (double): Height scale factor
+        d_factor (double): D-factor scale factor
+        conductivity (double): Conductivity scale factor
+    """
+    return self._execute_command(
+        scaleFractureTemplate=Commands_pb2.ScaleFractureTemplateRequest(
+            id=template_id,
+            halfLength=half_length,
+            height=height,
+            dFactor=d_factor,
+            conductivity=conductivity,
+        )
+    )
+
+
+@add_method(Project)
+def set_fracture_containment(self, template_id, top_layer, base_layer):
+    """Set fracture template containment parameters
+
+    Arguments:
+        template_id(int): ID of fracture template
+        top_layer (int): Top layer containment
+        base_layer (int): Base layer containment
+    """
+    return self._execute_command(
+        setFractureContainment=Commands_pb2.SetFracContainmentRequest(
+            id=template_id, topLayer=top_layer, baseLayer=base_layer
+        )
+    )
+
+
+@add_method(Project)
+def import_well_paths(self, well_path_files=None, well_path_folder=""):
+    """Import well paths into project
+
+    Arguments:
+        well_path_files(list): List of file paths to import
+        well_path_folder(str): A folder path containing files to import
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.WellPath`
+    """
+    if well_path_files is None:
+        well_path_files = []
+
+    res = self._execute_command(
+        importWellPaths=Commands_pb2.ImportWellPathsRequest(
+            wellPathFolder=well_path_folder, wellPathFiles=well_path_files
+        )
+    )
+    well_paths = []
+    for well_path_name in res.importWellPathsResult.wellPathNames:
+        well_paths.append(self.well_path_by_name(well_path_name))
+    return well_paths
+
+
+@add_method(Project)
+def well_paths(self):
+    """Get a list of all well paths in the project
+
+    Returns:
+        List of :class:`rips.generated.generated_classes.WellPath`
+    """
+    return self.descendants(WellPath)
+
+
+@add_method(Project)
+def well_path_by_name(self, well_path_name):
+    """Get a specific well path by name from the project
+
+    Returns:
+        :class:`rips.generated.generated_classes.WellPath`
+    """
+    all_well_paths = self.well_paths()
+    for well_path in all_well_paths:
+        if well_path.name == well_path_name:
+            return well_path
+    return None
+
+
+@add_method(Project)
+def import_well_log_files(self, well_log_files=None, well_log_folder=""):
+    """Import well log files into project
+
+    Arguments:
+        well_log_files(list): List of file paths to import
+        well_log_folder(str): A folder path containing files to import
+
+    Returns:
+        A list of well path names (strings) that had logs imported
+    """
+
+    if well_log_files is None:
+        well_log_files = []
+    res = self._execute_command(
+        importWellLogFiles=Commands_pb2.ImportWellLogFilesRequest(
+            wellLogFolder=well_log_folder, wellLogFiles=well_log_files
+        )
+    )
+    return res.importWellLogFilesResult.wellPathNames
+
+
+@add_method(Project)
+def import_formation_names(self, formation_files=None):
+    """Import formation names into project
+
+    Arguments:
+        formation_files(list): list of files to import
+
+    """
+    if formation_files is None:
+        formation_files = []
+    elif isinstance(formation_files, str):
+        formation_files = [formation_files]
+
+    self._execute_command(
+        importFormationNames=Commands_pb2.ImportFormationNamesRequest(
+            formationFiles=formation_files, applyToCaseId=-1
+        )
+    )
```

### Comparing `rips-2023.6.0.1/rips/retry_policy.py` & `rips-2023.6.0.2/rips/retry_policy.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import abc
-
-import time
-import random
-
-
-class RetryPolicy(abc.ABC):
-    @abc.abstractmethod
-    def sleep(self, retry_num):
-        """
-        How long to sleep in milliseconds.
-        :param retry_num: the number of retry (starting from zero)
-        """
-        assert retry_num >= 0
-
-    @abc.abstractmethod
-    def time_out_message(self):
-        """
-        Generate a error message for user on time out.
-        """
-        pass
-
-    @abc.abstractmethod
-    def num_retries(self):
-        """
-        Max number retries.
-        """
-        pass
-
-
-class FixedRetryPolicy(RetryPolicy):
-    def __init__(self, sleep_time=1000, max_num_retries=10):
-        """
-        Create a fixed time retry policy.
-        :param sleep_time: time to sleep in milliseconds.
-        :param max_num_retries: max number of retries.
-        """
-        self.sleep_time = sleep_time
-        self.max_num_retries = max_num_retries
-
-    def sleep(self, retry_num):
-        time.sleep(self.sleep_time / 1000)
-
-    def time_out_message(self):
-        return "Tried {} times with {} milliseconds apart.".format(
-            self.max_num_retries, self.sleep_time
-        )
-
-    def num_retries(self):
-        return self.max_num_retries
-
-
-class ExponentialBackoffRetryPolicy(RetryPolicy):
-    def __init__(self, min_backoff=200, max_backoff=10000, max_num_retries=20):
-        """
-        Create a truncated exponential backoff policy.
-        See: https://en.wikipedia.org/wiki/Exponential_backoff
-        :param min_backoff: minimum time to sleep in milliseconds.
-        :param max_backoff: maximum time to sleep in milliseconds.
-        :param max_num_retries: max number of retries.
-        """
-        self.min_backoff = min_backoff
-        self.max_backoff = max_backoff
-        self.max_num_retries = max_num_retries
-        self.multiplier = 2
-
-    def sleep(self, retry_num):
-        # Add a random component to avoid synchronized retries
-        wiggle = random.randint(0, 100)
-        sleep_ms = min(
-            self.min_backoff + self.multiplier**retry_num + wiggle, self.max_backoff
-        )
-        time.sleep(sleep_ms / 1000)
-
-    def time_out_message(self):
-        return (
-            "Tried {} times with increasing delay (from {} to {} milliseconds).".format(
-                self.max_num_retries, self.min_backoff, self.max_backoff
-            )
-        )
-
-    def num_retries(self):
-        return self.max_num_retries
+import abc
+
+import time
+import random
+
+
+class RetryPolicy(abc.ABC):
+    @abc.abstractmethod
+    def sleep(self, retry_num):
+        """
+        How long to sleep in milliseconds.
+        :param retry_num: the number of retry (starting from zero)
+        """
+        assert retry_num >= 0
+
+    @abc.abstractmethod
+    def time_out_message(self):
+        """
+        Generate a error message for user on time out.
+        """
+        pass
+
+    @abc.abstractmethod
+    def num_retries(self):
+        """
+        Max number retries.
+        """
+        pass
+
+
+class FixedRetryPolicy(RetryPolicy):
+    def __init__(self, sleep_time=1000, max_num_retries=10):
+        """
+        Create a fixed time retry policy.
+        :param sleep_time: time to sleep in milliseconds.
+        :param max_num_retries: max number of retries.
+        """
+        self.sleep_time = sleep_time
+        self.max_num_retries = max_num_retries
+
+    def sleep(self, retry_num):
+        time.sleep(self.sleep_time / 1000)
+
+    def time_out_message(self):
+        return "Tried {} times with {} milliseconds apart.".format(
+            self.max_num_retries, self.sleep_time
+        )
+
+    def num_retries(self):
+        return self.max_num_retries
+
+
+class ExponentialBackoffRetryPolicy(RetryPolicy):
+    def __init__(self, min_backoff=200, max_backoff=10000, max_num_retries=20):
+        """
+        Create a truncated exponential backoff policy.
+        See: https://en.wikipedia.org/wiki/Exponential_backoff
+        :param min_backoff: minimum time to sleep in milliseconds.
+        :param max_backoff: maximum time to sleep in milliseconds.
+        :param max_num_retries: max number of retries.
+        """
+        self.min_backoff = min_backoff
+        self.max_backoff = max_backoff
+        self.max_num_retries = max_num_retries
+        self.multiplier = 2
+
+    def sleep(self, retry_num):
+        # Add a random component to avoid synchronized retries
+        wiggle = random.randint(0, 100)
+        sleep_ms = min(
+            self.min_backoff + self.multiplier**retry_num + wiggle, self.max_backoff
+        )
+        time.sleep(sleep_ms / 1000)
+
+    def time_out_message(self):
+        return (
+            "Tried {} times with increasing delay (from {} to {} milliseconds).".format(
+                self.max_num_retries, self.min_backoff, self.max_backoff
+            )
+        )
+
+    def num_retries(self):
+        return self.max_num_retries
```

### Comparing `rips-2023.6.0.1/rips/simulation_well.py` & `rips-2023.6.0.2/rips/simulation_well.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""
-ResInsight SimulationWell
-"""
-import grpc
-
-import SimulationWell_pb2
-import SimulationWell_pb2_grpc
-
-import Properties_pb2
-import Properties_pb2_grpc
-
-from .resinsight_classes import SimulationWell
-
-from .pdmobject import PdmObjectBase, add_method
-
-import rips.case
-
-
-@add_method(SimulationWell)
-def __custom_init__(self, pb2_object, channel):
-    self._simulation_well_stub = SimulationWell_pb2_grpc.SimulationWellStub(channel)
-
-
-@add_method(SimulationWell)
-def status(self, timestep):
-    """Get simulation well status
-
-     **SimulationWellStatus class description**::
-
-        Parameter   | Description                                                   | Type
-        ----------- | ------------------------------------------------------------- | -----
-        well_type   | Well type as string                                           | string
-        is_open     | True if simulation well is open at the specified time step    | bool
-
-    Arguments:
-        timestep(int): Time step index
-
-    """
-    sim_well_request = SimulationWell_pb2.SimulationWellRequest(
-        case_id=self.case().id, well_name=self.name, timestep=timestep
-    )
-    return self._simulation_well_stub.GetSimulationWellStatus(sim_well_request)
-
-
-@add_method(SimulationWell)
-def cells(self, timestep):
-    """Get reservoir cells the simulation well is defined for
-
-     **SimulationWellCellInfo class description**::
-
-        Parameter   | Description                                               | Type
-        ----------- | --------------------------------------------------------- | -----
-        ijk         | Cell IJK location                                         | Vec3i
-        grid_index  | Grid index                                                | int
-        is_open     | True if connection to is open at the specified time step  | bool
-        branch_id   |                                                           | int
-        segment_id  |                                                           | int
-
-    Arguments:
-        timestep(int): Time step index
-
-    Returns:
-        List of SimulationWellCellInfo
-
-    """
-    sim_well_request = SimulationWell_pb2.SimulationWellRequest(
-        case_id=self.case().id, well_name=self.name, timestep=timestep
-    )
-    return self._simulation_well_stub.GetSimulationWellCells(sim_well_request).data
-
-
-@add_method(SimulationWell)
-def case(self):
-    return self.ancestor(rips.case.Case)
+"""
+ResInsight SimulationWell
+"""
+import grpc
+
+import SimulationWell_pb2
+import SimulationWell_pb2_grpc
+
+import Properties_pb2
+import Properties_pb2_grpc
+
+from .resinsight_classes import SimulationWell
+
+from .pdmobject import PdmObjectBase, add_method
+
+import rips.case
+
+
+@add_method(SimulationWell)
+def __custom_init__(self, pb2_object, channel):
+    self._simulation_well_stub = SimulationWell_pb2_grpc.SimulationWellStub(channel)
+
+
+@add_method(SimulationWell)
+def status(self, timestep):
+    """Get simulation well status
+
+     **SimulationWellStatus class description**::
+
+        Parameter   | Description                                                   | Type
+        ----------- | ------------------------------------------------------------- | -----
+        well_type   | Well type as string                                           | string
+        is_open     | True if simulation well is open at the specified time step    | bool
+
+    Arguments:
+        timestep(int): Time step index
+
+    """
+    sim_well_request = SimulationWell_pb2.SimulationWellRequest(
+        case_id=self.case().id, well_name=self.name, timestep=timestep
+    )
+    return self._simulation_well_stub.GetSimulationWellStatus(sim_well_request)
+
+
+@add_method(SimulationWell)
+def cells(self, timestep):
+    """Get reservoir cells the simulation well is defined for
+
+     **SimulationWellCellInfo class description**::
+
+        Parameter   | Description                                               | Type
+        ----------- | --------------------------------------------------------- | -----
+        ijk         | Cell IJK location                                         | Vec3i
+        grid_index  | Grid index                                                | int
+        is_open     | True if connection to is open at the specified time step  | bool
+        branch_id   |                                                           | int
+        segment_id  |                                                           | int
+
+    Arguments:
+        timestep(int): Time step index
+
+    Returns:
+        List of SimulationWellCellInfo
+
+    """
+    sim_well_request = SimulationWell_pb2.SimulationWellRequest(
+        case_id=self.case().id, well_name=self.name, timestep=timestep
+    )
+    return self._simulation_well_stub.GetSimulationWellCells(sim_well_request).data
+
+
+@add_method(SimulationWell)
+def case(self):
+    return self.ancestor(rips.case.Case)
```

### Comparing `rips-2023.6.0.1/rips/tests/test_cases.py` & `rips-2023.6.0.2/rips/tests/test_cases.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-import sys
-import os
-import math
-import pytest
-import grpc
-import tempfile
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_Launch(rips_instance, initialize_test):
-    assert rips_instance is not None
-
-
-def test_EmptyProject(rips_instance, initialize_test):
-    cases = rips_instance.project.cases()
-    assert len(cases) is 0
-
-
-def test_OneCase(rips_instance, initialize_test):
-    case = rips_instance.project.load_case(
-        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    )
-    assert case.name == "TEST10K_FLT_LGR_NNC"
-    assert case.id == 0
-    cases = rips_instance.project.cases()
-    assert len(cases) is 1
-
-
-def test_BoundingBox(rips_instance, initialize_test):
-    case = rips_instance.project.load_case(
-        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    )
-    assert case.name == "TEST10K_FLT_LGR_NNC"
-    boundingbox = case.reservoir_boundingbox()
-    assert math.isclose(3382.90, boundingbox.min_x, abs_tol=1.0e-1)
-    assert math.isclose(5850.48, boundingbox.max_x, abs_tol=1.0e-1)
-    assert math.isclose(4157.45, boundingbox.min_y, abs_tol=1.0e-1)
-    assert math.isclose(7354.93, boundingbox.max_y, abs_tol=1.0e-1)
-    assert math.isclose(-4252.61, boundingbox.min_z, abs_tol=1.0e-1)
-    assert math.isclose(-4103.60, boundingbox.max_z, abs_tol=1.0e-1)
-
-    min_depth, max_depth = case.reservoir_depth_range()
-    assert math.isclose(4103.60, min_depth, abs_tol=1.0e-1)
-    assert math.isclose(4252.61, max_depth, abs_tol=1.0e-1)
-
-
-def test_MultipleCases(rips_instance, initialize_test):
-    case_paths = []
-    case_paths.append(dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID")
-    case_paths.append(dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID")
-    case_paths.append(dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID")
-
-    case_names = []
-    for case_path in case_paths:
-        case_name = os.path.splitext(os.path.basename(case_path))[0]
-        case_names.append(case_name)
-        rips_instance.project.load_case(path=case_path)
-
-    cases = rips_instance.project.cases()
-    assert len(cases) == len(case_names)
-    for i, case_name in enumerate(case_names):
-        assert case_name == cases[i].name
-
-
-def get_cell_index_with_ijk(cell_info, i, j, k):
-    for idx, cell in enumerate(cell_info):
-        if cell.local_ijk.i == i and cell.local_ijk.j == j and cell.local_ijk.k == k:
-            return idx
-    return -1
-
-
-def check_corner(actual, expected):
-    assert math.isclose(actual.x, expected[0], abs_tol=0.1)
-    assert math.isclose(actual.y, expected[1], abs_tol=0.1)
-    assert math.isclose(actual.z, expected[2], abs_tol=0.1)
-
-
-def test_10k(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    assert len(case.grids()) == 2
-    cell_count_info = case.cell_count()
-    assert cell_count_info.active_cell_count == 11125
-    assert cell_count_info.reservoir_cell_count == 316224
-    time_steps = case.time_steps()
-    assert len(time_steps) == 9
-    days_since_start = case.days_since_start()
-    assert len(days_since_start) == 9
-    cell_info = case.cell_info_for_active_cells()
-    assert len(cell_info) == cell_count_info.active_cell_count
-
-    # Check an active cell (found in resinsight ui)
-    cell_index = get_cell_index_with_ijk(cell_info, 23, 44, 19)
-    assert cell_index != -1
-
-    cell_centers = case.active_cell_centers()
-    assert len(cell_centers) == cell_count_info.active_cell_count
-
-    # Check the cell center for the specific cell
-    assert math.isclose(3627.17, cell_centers[cell_index].x, abs_tol=0.1)
-    assert math.isclose(5209.75, cell_centers[cell_index].y, abs_tol=0.1)
-    assert math.isclose(4179.6, cell_centers[cell_index].z, abs_tol=0.1)
-
-    cell_corners = case.active_cell_corners()
-    assert len(cell_corners) == cell_count_info.active_cell_count
-    # Expected values from ResInsight UI
-    expected_corners = [
-        [3565.22, 5179.02, 4177.18],
-        [3655.67, 5145.34, 4176.63],
-        [3690.07, 5240.69, 4180.02],
-        [3599.87, 5275.16, 4179.32],
-        [3564.13, 5178.61, 4179.75],
-        [3654.78, 5144.79, 4179.23],
-        [3688.99, 5239.88, 4182.7],
-        [3598.62, 5274.48, 4181.96],
-    ]
-    check_corner(cell_corners[cell_index].c0, expected_corners[0])
-    check_corner(cell_corners[cell_index].c1, expected_corners[1])
-    check_corner(cell_corners[cell_index].c2, expected_corners[2])
-    check_corner(cell_corners[cell_index].c3, expected_corners[3])
-    check_corner(cell_corners[cell_index].c4, expected_corners[4])
-    check_corner(cell_corners[cell_index].c5, expected_corners[5])
-    check_corner(cell_corners[cell_index].c6, expected_corners[6])
-    check_corner(cell_corners[cell_index].c7, expected_corners[7])
-
-    # No coarsening info for this case
-    coarsening_info = case.coarsening_info()
-    assert len(coarsening_info) == 0
-
-
-def test_PdmObject(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    assert case.id == 0
-    assert case.address() is not 0
-    assert case.__class__.__name__ == "EclipseCase"
-
-
-@pytest.mark.skipif(
-    sys.platform.startswith("linux"),
-    reason="Brugge is currently exceptionally slow on Linux",
-)
-def test_brugge_0010(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real10/BRUGGE_0010.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    assert len(case.grids()) == 1
-    cellCountInfo = case.cell_count()
-    assert cellCountInfo.active_cell_count == 43374
-    assert cellCountInfo.reservoir_cell_count == 60048
-    time_steps = case.time_steps()
-    assert len(time_steps) == 11
-    days_since_start = case.days_since_start()
-    assert len(days_since_start) == 11
-
-
-@pytest.mark.skipif(
-    sys.platform.startswith("linux"),
-    reason="Brugge is currently exceptionally slow on Linux",
-)
-def test_replaceCase(rips_instance, initialize_test):
-    project = rips_instance.project.open(
-        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp"
-    )
-    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
-    case = project.case(case_id=0)
-    assert case is not None
-    assert case.name == "TEST10K_FLT_LGR_NNC"
-    assert case.id == 0
-    cases = rips_instance.project.cases()
-    assert len(cases) is 1
-
-    case.replace(new_grid_file=case_path)
-    # Check that the case object has been changed
-    assert case.name == "BRUGGE_0000"
-    assert case.id == 0
-
-    cases = rips_instance.project.cases()
-    assert len(cases) is 1
-    # Check that retrieving the case object again will yield the changed object
-    case = project.case(case_id=0)
-    assert case.name == "BRUGGE_0000"
-    assert case.id == 0
-
-
-def test_loadNonExistingCase(rips_instance, initialize_test):
-    case_path = "Nonsense/Nonsense/Nonsense"
-    with pytest.raises(grpc.RpcError):
-        assert rips_instance.project.load_case(case_path)
-
-
-@pytest.mark.skipif(
-    sys.platform.startswith("linux"),
-    reason="Brugge is currently exceptionally slow on Linux",
-)
-def test_exportFlowCharacteristics(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
-    case = rips_instance.project.load_case(case_path)
-    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
-        print("Temporary folder: ", tmpdirname)
-        file_name = tmpdirname + "/exportFlowChar.txt"
-        case.export_flow_characteristics(
-            time_steps=8, producers=[], injectors="I01", file_name=file_name
-        )
-
-
-def test_selected_cells(rips_instance, initialize_test):
-    case = rips_instance.project.load_case(
-        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    )
-    assert case.name == "TEST10K_FLT_LGR_NNC"
-    selected_cells = case.selected_cells()
-    assert len(selected_cells) == 0
-
-    time_step_info = case.time_steps()
-    for tidx, timestep in enumerate(time_step_info):
-        # Try to read for SOIL the time step (will be empty since nothing is selected)
-        soil_results = case.selected_cell_property("DYNAMIC_NATIVE", "SOIL", tidx)
-        assert len(soil_results) == 0
-
-
-def test_multiple_load_of_same_case(rips_instance, initialize_test):
-    # Test related to issue https://github.com/OPM/ResInsight/issues/9332
-    path_name = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.EGRID"
-    case_count = 3
-    for i in range(case_count):
-        case = rips_instance.project.load_case(path_name)
+import sys
+import os
+import math
+import pytest
+import grpc
+import tempfile
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_Launch(rips_instance, initialize_test):
+    assert rips_instance is not None
+
+
+def test_EmptyProject(rips_instance, initialize_test):
+    cases = rips_instance.project.cases()
+    assert len(cases) is 0
+
+
+def test_OneCase(rips_instance, initialize_test):
+    case = rips_instance.project.load_case(
+        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    )
+    assert case.name == "TEST10K_FLT_LGR_NNC"
+    assert case.id == 0
+    cases = rips_instance.project.cases()
+    assert len(cases) is 1
+
+
+def test_BoundingBox(rips_instance, initialize_test):
+    case = rips_instance.project.load_case(
+        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    )
+    assert case.name == "TEST10K_FLT_LGR_NNC"
+    boundingbox = case.reservoir_boundingbox()
+    assert math.isclose(3382.90, boundingbox.min_x, abs_tol=1.0e-1)
+    assert math.isclose(5850.48, boundingbox.max_x, abs_tol=1.0e-1)
+    assert math.isclose(4157.45, boundingbox.min_y, abs_tol=1.0e-1)
+    assert math.isclose(7354.93, boundingbox.max_y, abs_tol=1.0e-1)
+    assert math.isclose(-4252.61, boundingbox.min_z, abs_tol=1.0e-1)
+    assert math.isclose(-4103.60, boundingbox.max_z, abs_tol=1.0e-1)
+
+    min_depth, max_depth = case.reservoir_depth_range()
+    assert math.isclose(4103.60, min_depth, abs_tol=1.0e-1)
+    assert math.isclose(4252.61, max_depth, abs_tol=1.0e-1)
+
+
+def test_MultipleCases(rips_instance, initialize_test):
+    case_paths = []
+    case_paths.append(dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID")
+    case_paths.append(dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID")
+    case_paths.append(dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID")
+
+    case_names = []
+    for case_path in case_paths:
+        case_name = os.path.splitext(os.path.basename(case_path))[0]
+        case_names.append(case_name)
+        rips_instance.project.load_case(path=case_path)
+
+    cases = rips_instance.project.cases()
+    assert len(cases) == len(case_names)
+    for i, case_name in enumerate(case_names):
+        assert case_name == cases[i].name
+
+
+def get_cell_index_with_ijk(cell_info, i, j, k):
+    for idx, cell in enumerate(cell_info):
+        if cell.local_ijk.i == i and cell.local_ijk.j == j and cell.local_ijk.k == k:
+            return idx
+    return -1
+
+
+def check_corner(actual, expected):
+    assert math.isclose(actual.x, expected[0], abs_tol=0.1)
+    assert math.isclose(actual.y, expected[1], abs_tol=0.1)
+    assert math.isclose(actual.z, expected[2], abs_tol=0.1)
+
+
+def test_10k(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    assert len(case.grids()) == 2
+    cell_count_info = case.cell_count()
+    assert cell_count_info.active_cell_count == 11125
+    assert cell_count_info.reservoir_cell_count == 316224
+    time_steps = case.time_steps()
+    assert len(time_steps) == 9
+    days_since_start = case.days_since_start()
+    assert len(days_since_start) == 9
+    cell_info = case.cell_info_for_active_cells()
+    assert len(cell_info) == cell_count_info.active_cell_count
+
+    # Check an active cell (found in resinsight ui)
+    cell_index = get_cell_index_with_ijk(cell_info, 23, 44, 19)
+    assert cell_index != -1
+
+    cell_centers = case.active_cell_centers()
+    assert len(cell_centers) == cell_count_info.active_cell_count
+
+    # Check the cell center for the specific cell
+    assert math.isclose(3627.17, cell_centers[cell_index].x, abs_tol=0.1)
+    assert math.isclose(5209.75, cell_centers[cell_index].y, abs_tol=0.1)
+    assert math.isclose(4179.6, cell_centers[cell_index].z, abs_tol=0.1)
+
+    cell_corners = case.active_cell_corners()
+    assert len(cell_corners) == cell_count_info.active_cell_count
+    # Expected values from ResInsight UI
+    expected_corners = [
+        [3565.22, 5179.02, 4177.18],
+        [3655.67, 5145.34, 4176.63],
+        [3690.07, 5240.69, 4180.02],
+        [3599.87, 5275.16, 4179.32],
+        [3564.13, 5178.61, 4179.75],
+        [3654.78, 5144.79, 4179.23],
+        [3688.99, 5239.88, 4182.7],
+        [3598.62, 5274.48, 4181.96],
+    ]
+    check_corner(cell_corners[cell_index].c0, expected_corners[0])
+    check_corner(cell_corners[cell_index].c1, expected_corners[1])
+    check_corner(cell_corners[cell_index].c2, expected_corners[2])
+    check_corner(cell_corners[cell_index].c3, expected_corners[3])
+    check_corner(cell_corners[cell_index].c4, expected_corners[4])
+    check_corner(cell_corners[cell_index].c5, expected_corners[5])
+    check_corner(cell_corners[cell_index].c6, expected_corners[6])
+    check_corner(cell_corners[cell_index].c7, expected_corners[7])
+
+    # No coarsening info for this case
+    coarsening_info = case.coarsening_info()
+    assert len(coarsening_info) == 0
+
+
+def test_PdmObject(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    assert case.id == 0
+    assert case.address() is not 0
+    assert case.__class__.__name__ == "EclipseCase"
+
+
+@pytest.mark.skipif(
+    sys.platform.startswith("linux"),
+    reason="Brugge is currently exceptionally slow on Linux",
+)
+def test_brugge_0010(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real10/BRUGGE_0010.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    assert len(case.grids()) == 1
+    cellCountInfo = case.cell_count()
+    assert cellCountInfo.active_cell_count == 43374
+    assert cellCountInfo.reservoir_cell_count == 60048
+    time_steps = case.time_steps()
+    assert len(time_steps) == 11
+    days_since_start = case.days_since_start()
+    assert len(days_since_start) == 11
+
+
+@pytest.mark.skipif(
+    sys.platform.startswith("linux"),
+    reason="Brugge is currently exceptionally slow on Linux",
+)
+def test_replaceCase(rips_instance, initialize_test):
+    project = rips_instance.project.open(
+        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp"
+    )
+    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
+    case = project.case(case_id=0)
+    assert case is not None
+    assert case.name == "TEST10K_FLT_LGR_NNC"
+    assert case.id == 0
+    cases = rips_instance.project.cases()
+    assert len(cases) is 1
+
+    case.replace(new_grid_file=case_path)
+    # Check that the case object has been changed
+    assert case.name == "BRUGGE_0000"
+    assert case.id == 0
+
+    cases = rips_instance.project.cases()
+    assert len(cases) is 1
+    # Check that retrieving the case object again will yield the changed object
+    case = project.case(case_id=0)
+    assert case.name == "BRUGGE_0000"
+    assert case.id == 0
+
+
+def test_loadNonExistingCase(rips_instance, initialize_test):
+    case_path = "Nonsense/Nonsense/Nonsense"
+    with pytest.raises(grpc.RpcError):
+        assert rips_instance.project.load_case(case_path)
+
+
+@pytest.mark.skipif(
+    sys.platform.startswith("linux"),
+    reason="Brugge is currently exceptionally slow on Linux",
+)
+def test_exportFlowCharacteristics(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
+    case = rips_instance.project.load_case(case_path)
+    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
+        print("Temporary folder: ", tmpdirname)
+        file_name = tmpdirname + "/exportFlowChar.txt"
+        case.export_flow_characteristics(
+            time_steps=8, producers=[], injectors="I01", file_name=file_name
+        )
+
+
+def test_selected_cells(rips_instance, initialize_test):
+    case = rips_instance.project.load_case(
+        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    )
+    assert case.name == "TEST10K_FLT_LGR_NNC"
+    selected_cells = case.selected_cells()
+    assert len(selected_cells) == 0
+
+    time_step_info = case.time_steps()
+    for tidx, timestep in enumerate(time_step_info):
+        # Try to read for SOIL the time step (will be empty since nothing is selected)
+        soil_results = case.selected_cell_property("DYNAMIC_NATIVE", "SOIL", tidx)
+        assert len(soil_results) == 0
+
+
+def test_multiple_load_of_same_case(rips_instance, initialize_test):
+    # Test related to issue https://github.com/OPM/ResInsight/issues/9332
+    path_name = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.EGRID"
+    case_count = 3
+    for i in range(case_count):
+        case = rips_instance.project.load_case(path_name)
```

### Comparing `rips-2023.6.0.1/rips/tests/test_create_well_path.py` & `rips-2023.6.0.2/rips/tests/test_create_well_path.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from rips.generated.generated_classes import (
-    ModeledWellPath,
-    StimPlanModel,
-    WellPathGeometry,
-    WellPathTarget,
-)
-import sys
-import os
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-
-def test_add_new_object_for_well_paths(rips_instance, initialize_test):
-    well_path_coll = rips_instance.project.descendants(rips.WellPathCollection)[0]
-
-    my_well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
-    my_well_path.name = "test"
-    my_well_path.update()
-
-    geometry = my_well_path.well_path_geometry()
-    geometry.add_new_object(rips.WellPathTarget)
-    geometry.add_new_object(rips.WellPathTarget)
-    geometry.add_new_object(rips.WellPathTarget)
-    assert len(geometry.well_path_targets()) == 3
-
-    assert len(well_path_coll.well_paths()) == 1
-    my_well_path_duplicate = well_path_coll.well_paths()[0]
-    assert my_well_path_duplicate.name == "test"
-    geometry_duplicate = my_well_path_duplicate.well_path_geometry()
-    assert len(geometry_duplicate.well_path_targets()) == 3
-
-    # Not allowed to add object of unrelated type
-    invalid_object = geometry.add_new_object(rips.WellPath)
-    assert invalid_object is None
-
-
-def test_add_well_path_targets(rips_instance, initialize_test):
-    well_path_coll = rips_instance.project.descendants(rips.WellPathCollection)[0]
-
-    my_well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
-    my_well_path.name = "test"
-    my_well_path.update()
-
-    geometry = my_well_path.well_path_geometry()
-
-    # Append well target with fixed azimuth
-    coord = [2229.10, -833.74, -74.70]
-    target = geometry.append_well_target(
-        coord, use_fixed_azimuth=True, fixed_azimuth_value=110.1
-    )
-    assert target.use_fixed_inclination == False
-    assert target.use_fixed_azimuth == True
-    assert target.azimuth == 110.1
-    assert target.inclination == 0.0
-
-    # Append well target with fixed inclination
-    coord = [4577.21, -3043.47, -87.15]
-    target = geometry.append_well_target(
-        coord, use_fixed_inclination=True, fixed_inclination_value=25.6
-    )
-
-    assert target.use_fixed_inclination == True
-    assert target.use_fixed_azimuth == False
-    assert target.azimuth == 0.0
-    assert target.inclination == 25.6
+from rips.generated.generated_classes import (
+    ModeledWellPath,
+    StimPlanModel,
+    WellPathGeometry,
+    WellPathTarget,
+)
+import sys
+import os
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+
+def test_add_new_object_for_well_paths(rips_instance, initialize_test):
+    well_path_coll = rips_instance.project.descendants(rips.WellPathCollection)[0]
+
+    my_well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
+    my_well_path.name = "test"
+    my_well_path.update()
+
+    geometry = my_well_path.well_path_geometry()
+    geometry.add_new_object(rips.WellPathTarget)
+    geometry.add_new_object(rips.WellPathTarget)
+    geometry.add_new_object(rips.WellPathTarget)
+    assert len(geometry.well_path_targets()) == 3
+
+    assert len(well_path_coll.well_paths()) == 1
+    my_well_path_duplicate = well_path_coll.well_paths()[0]
+    assert my_well_path_duplicate.name == "test"
+    geometry_duplicate = my_well_path_duplicate.well_path_geometry()
+    assert len(geometry_duplicate.well_path_targets()) == 3
+
+    # Not allowed to add object of unrelated type
+    invalid_object = geometry.add_new_object(rips.WellPath)
+    assert invalid_object is None
+
+
+def test_add_well_path_targets(rips_instance, initialize_test):
+    well_path_coll = rips_instance.project.descendants(rips.WellPathCollection)[0]
+
+    my_well_path = well_path_coll.add_new_object(rips.ModeledWellPath)
+    my_well_path.name = "test"
+    my_well_path.update()
+
+    geometry = my_well_path.well_path_geometry()
+
+    # Append well target with fixed azimuth
+    coord = [2229.10, -833.74, -74.70]
+    target = geometry.append_well_target(
+        coord, use_fixed_azimuth=True, fixed_azimuth_value=110.1
+    )
+    assert target.use_fixed_inclination == False
+    assert target.use_fixed_azimuth == True
+    assert target.azimuth == 110.1
+    assert target.inclination == 0.0
+
+    # Append well target with fixed inclination
+    coord = [4577.21, -3043.47, -87.15]
+    target = geometry.append_well_target(
+        coord, use_fixed_inclination=True, fixed_inclination_value=25.6
+    )
+
+    assert target.use_fixed_inclination == True
+    assert target.use_fixed_azimuth == False
+    assert target.azimuth == 0.0
+    assert target.inclination == 25.6
```

### Comparing `rips-2023.6.0.1/rips/tests/test_nnc_properties.py` & `rips-2023.6.0.2/rips/tests/test_nnc_properties.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import sys
-import os
-import grpc
-import pytest
-
-import rips.generated.NNCProperties_pb2 as NNCProperties_pb2
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_10kSync(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    properties = case.available_nnc_properties()
-    assert len(properties) == 1
-
-    assert "TRAN" == properties[0].name
-    assert (
-        NNCProperties_pb2.NNCPropertyType.Value("NNC_STATIC")
-        == properties[0].property_type
-    )
-
-    nnc_connections = case.nnc_connections()
-    assert len(nnc_connections) == 3416
-
-    connection = nnc_connections[0]
-    assert connection.cell1.i == 33
-    assert connection.cell1.j == 40
-    assert connection.cell1.k == 14
-    assert connection.cell_grid_index1 == 0
-
-    tran_vals = case.nnc_connections_static_values("TRAN")
-    assert len(tran_vals) == len(nnc_connections)
-
-    for t in tran_vals:
-        assert isinstance(t, float)
-
-    # Generate some data
-    new_data = []
-    for c, _ in enumerate(nnc_connections):
-        new_data.append(float(c))
-
-    property_name = "NEW_PROP"
-    case.set_nnc_connections_values(new_data, property_name, 0)
-    new_prop_vals = case.nnc_connections_generated_values(property_name, 0)
-    assert len(new_prop_vals) == len(new_data)
-    for i in range(0, len(new_data)):
-        assert new_data[i] == new_prop_vals[i]
-
-    # Set some other data for second time step
-    for i in range(0, len(new_data)):
-        new_data[i] = new_data[i] * 2.0
-
-    case.set_nnc_connections_values(new_data, property_name, 1)
-    new_prop_vals = case.nnc_connections_generated_values(property_name, 1)
-    assert len(new_prop_vals) == len(nnc_connections)
-    for i in range(0, len(new_data)):
-        assert new_data[i] == new_prop_vals[i]
-
-
-def test_non_existing_dynamic_values(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    with pytest.raises(grpc.RpcError):
-        case.nnc_connections_dynamic_values("x", 0)
-
-
-def test_invalid_time_steps(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-    with pytest.raises(grpc.RpcError):
-        case.nnc_connections_generated_values("Formation Allan", 9999)
+import sys
+import os
+import grpc
+import pytest
+
+import rips.generated.NNCProperties_pb2 as NNCProperties_pb2
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_10kSync(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    properties = case.available_nnc_properties()
+    assert len(properties) == 1
+
+    assert "TRAN" == properties[0].name
+    assert (
+        NNCProperties_pb2.NNCPropertyType.Value("NNC_STATIC")
+        == properties[0].property_type
+    )
+
+    nnc_connections = case.nnc_connections()
+    assert len(nnc_connections) == 3416
+
+    connection = nnc_connections[0]
+    assert connection.cell1.i == 33
+    assert connection.cell1.j == 40
+    assert connection.cell1.k == 14
+    assert connection.cell_grid_index1 == 0
+
+    tran_vals = case.nnc_connections_static_values("TRAN")
+    assert len(tran_vals) == len(nnc_connections)
+
+    for t in tran_vals:
+        assert isinstance(t, float)
+
+    # Generate some data
+    new_data = []
+    for c, _ in enumerate(nnc_connections):
+        new_data.append(float(c))
+
+    property_name = "NEW_PROP"
+    case.set_nnc_connections_values(new_data, property_name, 0)
+    new_prop_vals = case.nnc_connections_generated_values(property_name, 0)
+    assert len(new_prop_vals) == len(new_data)
+    for i in range(0, len(new_data)):
+        assert new_data[i] == new_prop_vals[i]
+
+    # Set some other data for second time step
+    for i in range(0, len(new_data)):
+        new_data[i] = new_data[i] * 2.0
+
+    case.set_nnc_connections_values(new_data, property_name, 1)
+    new_prop_vals = case.nnc_connections_generated_values(property_name, 1)
+    assert len(new_prop_vals) == len(nnc_connections)
+    for i in range(0, len(new_data)):
+        assert new_data[i] == new_prop_vals[i]
+
+
+def test_non_existing_dynamic_values(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    with pytest.raises(grpc.RpcError):
+        case.nnc_connections_dynamic_values("x", 0)
+
+
+def test_invalid_time_steps(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+    with pytest.raises(grpc.RpcError):
+        case.nnc_connections_generated_values("Formation Allan", 9999)
```

### Comparing `rips-2023.6.0.1/rips/tests/test_project.py` & `rips-2023.6.0.2/rips/tests/test_project.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import sys
-import os
-import pytest
-import grpc
-import tempfile
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_loadProject(rips_instance, initialize_test):
-    project = rips_instance.project.open(
-        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp"
-    )
-    case = project.cases()[0]
-    assert case is not None
-    assert case.name == "TEST10K_FLT_LGR_NNC"
-    assert case.id == 0
-    cases = rips_instance.project.cases()
-    assert len(cases) is 1
-
-
-def test_well_log_plots(rips_instance, initialize_test):
-    project = rips_instance.project.open(
-        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp"
-    )
-    plots = project.plots()
-    well_log_plots = []
-    for plot in plots:
-        if isinstance(plot, rips.WellLogPlot):
-            assert plot.depth_type == "MEASURED_DEPTH"
-            well_log_plots.append(plot)
-    assert len(well_log_plots) == 2
-
-    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
-        for well_log_plot in well_log_plots:
-            well_log_plot.depth_type = "TRUE_VERTICAL_DEPTH_RKB"
-            well_log_plot.update()
-            if rips_instance.is_gui():
-                well_log_plot.export_snapshot(tmpdirname)
-            well_log_plot.export_data_as_las(tmpdirname)
-        files = os.listdir(tmpdirname)
-        print(files)
-        if rips_instance.is_gui():
-            assert len(files) == 4
-        else:
-            assert len(files) == 2
-
-    plots2 = project.plots()
-    for plot2 in plots2:
-        if isinstance(plot2, rips.WellLogPlot):
-            assert plot2.depth_type == "TRUE_VERTICAL_DEPTH_RKB"
-
-
-@pytest.mark.skipif(
-    sys.platform.startswith("linux"),
-    reason="Brugge is currently exceptionally slow on Linux",
-)
-def test_loadGridCaseGroup(rips_instance, initialize_test):
-    case_paths = []
-    case_paths.append(dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID")
-    case_paths.append(
-        dataroot.PATH + "/Case_with_10_timesteps/Real10/BRUGGE_0010.EGRID"
-    )
-    grid_case_group = rips_instance.project.create_grid_case_group(
-        case_paths=case_paths
-    )
-    assert grid_case_group is not None and grid_case_group.group_id == 0
-
-
-def test_exportSnapshots(rips_instance, initialize_test):
-    if not rips_instance.is_gui():
-        pytest.skip("Cannot run test without a GUI")
-
-    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    rips_instance.project.load_case(case_path)
-    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
-        print("Temporary folder: ", tmpdirname)
-        rips_instance.set_export_folder(export_type="SNAPSHOTS", path=tmpdirname)
-        rips_instance.project.export_snapshots()
-        print(os.listdir(tmpdirname))
-        #        assert(len(os.listdir(tmpdirname)) > 0)
-        for fileName in os.listdir(tmpdirname):
-            assert os.path.splitext(fileName)[1] == ".png"
+import sys
+import os
+import pytest
+import grpc
+import tempfile
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_loadProject(rips_instance, initialize_test):
+    project = rips_instance.project.open(
+        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp"
+    )
+    case = project.cases()[0]
+    assert case is not None
+    assert case.name == "TEST10K_FLT_LGR_NNC"
+    assert case.id == 0
+    cases = rips_instance.project.cases()
+    assert len(cases) is 1
+
+
+def test_well_log_plots(rips_instance, initialize_test):
+    project = rips_instance.project.open(
+        dataroot.PATH + "/TEST10K_FLT_LGR_NNC/10KWithWellLog.rsp"
+    )
+    plots = project.plots()
+    well_log_plots = []
+    for plot in plots:
+        if isinstance(plot, rips.WellLogPlot):
+            assert plot.depth_type == "MEASURED_DEPTH"
+            well_log_plots.append(plot)
+    assert len(well_log_plots) == 2
+
+    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
+        for well_log_plot in well_log_plots:
+            well_log_plot.depth_type = "TRUE_VERTICAL_DEPTH_RKB"
+            well_log_plot.update()
+            if rips_instance.is_gui():
+                well_log_plot.export_snapshot(tmpdirname)
+            well_log_plot.export_data_as_las(tmpdirname)
+        files = os.listdir(tmpdirname)
+        print(files)
+        if rips_instance.is_gui():
+            assert len(files) == 4
+        else:
+            assert len(files) == 2
+
+    plots2 = project.plots()
+    for plot2 in plots2:
+        if isinstance(plot2, rips.WellLogPlot):
+            assert plot2.depth_type == "TRUE_VERTICAL_DEPTH_RKB"
+
+
+@pytest.mark.skipif(
+    sys.platform.startswith("linux"),
+    reason="Brugge is currently exceptionally slow on Linux",
+)
+def test_loadGridCaseGroup(rips_instance, initialize_test):
+    case_paths = []
+    case_paths.append(dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID")
+    case_paths.append(
+        dataroot.PATH + "/Case_with_10_timesteps/Real10/BRUGGE_0010.EGRID"
+    )
+    grid_case_group = rips_instance.project.create_grid_case_group(
+        case_paths=case_paths
+    )
+    assert grid_case_group is not None and grid_case_group.group_id == 0
+
+
+def test_exportSnapshots(rips_instance, initialize_test):
+    if not rips_instance.is_gui():
+        pytest.skip("Cannot run test without a GUI")
+
+    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    rips_instance.project.load_case(case_path)
+    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
+        print("Temporary folder: ", tmpdirname)
+        rips_instance.set_export_folder(export_type="SNAPSHOTS", path=tmpdirname)
+        rips_instance.project.export_snapshots()
+        print(os.listdir(tmpdirname))
+        #        assert(len(os.listdir(tmpdirname)) > 0)
+        for fileName in os.listdir(tmpdirname):
+            assert os.path.splitext(fileName)[1] == ".png"
```

### Comparing `rips-2023.6.0.1/rips/tests/test_properties.py` & `rips-2023.6.0.2/rips/tests/test_properties.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import sys
-import os
-import grpc
-import pytest
-import tempfile
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_10kAsync(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    resultChunks = case.active_cell_property_async("DYNAMIC_NATIVE", "SOIL", 1)
-    mysum = 0.0
-    count = 0
-    for chunk in resultChunks:
-        mysum += sum(chunk.values)
-        count += len(chunk.values)
-    average = mysum / count
-    assert mysum == pytest.approx(621.768, abs=0.001)
-    assert average != pytest.approx(0.0158893, abs=0.0000001)
-    assert average == pytest.approx(0.0558893, abs=0.0000001)
-
-
-def test_10kSync(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
-    mysum = sum(results)
-    average = mysum / len(results)
-    assert mysum == pytest.approx(621.768, abs=0.001)
-    assert average != pytest.approx(0.0158893, abs=0.0000001)
-    assert average == pytest.approx(0.0558893, abs=0.0000001)
-
-
-def test_10k_set(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
-    case.set_active_cell_property(results, "GENERATED", "SOIL", 1)
-
-
-def test_10k_set_out_of_bounds(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
-    results.append(5.0)
-    with pytest.raises(grpc.RpcError):
-        assert case.set_active_cell_property(results, "GENERATED", "SOIL", 1)
-
-
-def test_10k_set_out_of_bounds_client(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
-    case.chunk_size = len(results)
-    results.append(5.0)
-    with pytest.raises(IndexError):
-        assert case.set_active_cell_property(results, "GENERATED", "SOIL", 1)
-
-
-def createResult(poroChunks, permxChunks):
-    for poroChunk, permxChunk in zip(poroChunks, permxChunks):
-        resultChunk = []
-        for poro, permx in zip(poroChunk.values, permxChunk.values):
-            resultChunk.append(poro * permx)
-        yield resultChunk
-
-
-def checkResults(poroValues, permxValues, poropermxValues):
-    for poro, permx, poropermx in zip(poroValues, permxValues, poropermxValues):
-        recalc = poro * permx
-        assert recalc == pytest.approx(poropermx, rel=1.0e-10)
-
-
-def test_10k_PoroPermX(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=casePath)
-
-    poroChunks = case.active_cell_property_async("STATIC_NATIVE", "PORO", 0)
-    permxChunks = case.active_cell_property_async("STATIC_NATIVE", "PERMX", 0)
-
-    case.set_active_cell_property_async(
-        createResult(poroChunks, permxChunks), "GENERATED", "POROPERMXAS", 0
-    )
-
-    poro = case.active_cell_property("STATIC_NATIVE", "PORO", 0)
-    permx = case.active_cell_property("STATIC_NATIVE", "PERMX", 0)
-    poroPermX = case.active_cell_property("GENERATED", "POROPERMXAS", 0)
-
-    checkResults(poro, permx, poroPermX)
-
-
-def test_exportPropertyInView(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(case_path)
-    case.create_view()
-    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
-        print("Temporary folder: ", tmpdirname)
-        rips_instance.set_export_folder(export_type="PROPERTIES", path=tmpdirname)
-        case = rips_instance.project.cases()[0]
-        view = case.views()[0]
-        view.export_property()
-        expected_file_name = case.name + "-" + str("3D_View") + "-" + "T0" + "-SOIL"
-        full_path = tmpdirname + "/" + expected_file_name
-        assert os.path.exists(full_path)
+import sys
+import os
+import grpc
+import pytest
+import tempfile
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_10kAsync(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    resultChunks = case.active_cell_property_async("DYNAMIC_NATIVE", "SOIL", 1)
+    mysum = 0.0
+    count = 0
+    for chunk in resultChunks:
+        mysum += sum(chunk.values)
+        count += len(chunk.values)
+    average = mysum / count
+    assert mysum == pytest.approx(621.768, abs=0.001)
+    assert average != pytest.approx(0.0158893, abs=0.0000001)
+    assert average == pytest.approx(0.0558893, abs=0.0000001)
+
+
+def test_10kSync(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
+    mysum = sum(results)
+    average = mysum / len(results)
+    assert mysum == pytest.approx(621.768, abs=0.001)
+    assert average != pytest.approx(0.0158893, abs=0.0000001)
+    assert average == pytest.approx(0.0558893, abs=0.0000001)
+
+
+def test_10k_set(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
+    case.set_active_cell_property(results, "GENERATED", "SOIL", 1)
+
+
+def test_10k_set_out_of_bounds(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
+    results.append(5.0)
+    with pytest.raises(grpc.RpcError):
+        assert case.set_active_cell_property(results, "GENERATED", "SOIL", 1)
+
+
+def test_10k_set_out_of_bounds_client(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    results = case.active_cell_property("DYNAMIC_NATIVE", "SOIL", 1)
+    case.chunk_size = len(results)
+    results.append(5.0)
+    with pytest.raises(IndexError):
+        assert case.set_active_cell_property(results, "GENERATED", "SOIL", 1)
+
+
+def createResult(poroChunks, permxChunks):
+    for poroChunk, permxChunk in zip(poroChunks, permxChunks):
+        resultChunk = []
+        for poro, permx in zip(poroChunk.values, permxChunk.values):
+            resultChunk.append(poro * permx)
+        yield resultChunk
+
+
+def checkResults(poroValues, permxValues, poropermxValues):
+    for poro, permx, poropermx in zip(poroValues, permxValues, poropermxValues):
+        recalc = poro * permx
+        assert recalc == pytest.approx(poropermx, rel=1.0e-10)
+
+
+def test_10k_PoroPermX(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=casePath)
+
+    poroChunks = case.active_cell_property_async("STATIC_NATIVE", "PORO", 0)
+    permxChunks = case.active_cell_property_async("STATIC_NATIVE", "PERMX", 0)
+
+    case.set_active_cell_property_async(
+        createResult(poroChunks, permxChunks), "GENERATED", "POROPERMXAS", 0
+    )
+
+    poro = case.active_cell_property("STATIC_NATIVE", "PORO", 0)
+    permx = case.active_cell_property("STATIC_NATIVE", "PERMX", 0)
+    poroPermX = case.active_cell_property("GENERATED", "POROPERMXAS", 0)
+
+    checkResults(poro, permx, poroPermX)
+
+
+def test_exportPropertyInView(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(case_path)
+    case.create_view()
+    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
+        print("Temporary folder: ", tmpdirname)
+        rips_instance.set_export_folder(export_type="PROPERTIES", path=tmpdirname)
+        case = rips_instance.project.cases()[0]
+        view = case.views()[0]
+        view.export_property()
+        expected_file_name = case.name + "-" + str("3D_View") + "-" + "T0" + "-SOIL"
+        full_path = tmpdirname + "/" + expected_file_name
+        assert os.path.exists(full_path)
```

### Comparing `rips-2023.6.0.1/rips/tests/test_simulation_wells.py` & `rips-2023.6.0.2/rips/tests/test_simulation_wells.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import sys
-import os
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_10k(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    case.create_view()
-    assert len(case.grids()) == 2
-    cell_count_info = case.cell_count()
-
-    sim_wells = case.simulation_wells()
-    assert len(sim_wells) == 3
-
-    assert sim_wells[0].name == "GI1"
-    assert sim_wells[1].name == "GP1"
-    assert sim_wells[2].name == "GP2"
-
-    timesteps = case.time_steps()
-
-    # On time step 0 all simulation wells are undefined
-    for sim_well in sim_wells:
-        status = sim_well.status(0)
-        assert status.well_type == "NotDefined"
-
-    # On time step 3 all wells are producing
-    for sim_well in sim_wells:
-        status = sim_well.status(3)
-        assert status.well_type == "Producer"
-
-    # On time step 0 all simulation wells have no cells
-    for sim_well in sim_wells:
-        cells = sim_well.cells(0)
-        assert len(cells) == 0
-
-    # On the other time steps there should be cells
-    expected_cell_count = {}
-    expected_cell_count["GP1"] = 105
-    expected_cell_count["GI1"] = 38
-    expected_cell_count["GP2"] = 18
-    for sim_well in sim_wells:
-        for tidx, timestep in enumerate(timesteps):
-            if tidx > 0:
-                cells = sim_well.cells(tidx)
-                print(
-                    "well: "
-                    + sim_well.name
-                    + " timestep: "
-                    + str(tidx)
-                    + " cells:"
-                    + str(len(cells))
-                )
-                assert len(cells) == expected_cell_count[sim_well.name]
+import sys
+import os
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_10k(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    case.create_view()
+    assert len(case.grids()) == 2
+    cell_count_info = case.cell_count()
+
+    sim_wells = case.simulation_wells()
+    assert len(sim_wells) == 3
+
+    assert sim_wells[0].name == "GI1"
+    assert sim_wells[1].name == "GP1"
+    assert sim_wells[2].name == "GP2"
+
+    timesteps = case.time_steps()
+
+    # On time step 0 all simulation wells are undefined
+    for sim_well in sim_wells:
+        status = sim_well.status(0)
+        assert status.well_type == "NotDefined"
+
+    # On time step 3 all wells are producing
+    for sim_well in sim_wells:
+        status = sim_well.status(3)
+        assert status.well_type == "Producer"
+
+    # On time step 0 all simulation wells have no cells
+    for sim_well in sim_wells:
+        cells = sim_well.cells(0)
+        assert len(cells) == 0
+
+    # On the other time steps there should be cells
+    expected_cell_count = {}
+    expected_cell_count["GP1"] = 105
+    expected_cell_count["GI1"] = 38
+    expected_cell_count["GP2"] = 18
+    for sim_well in sim_wells:
+        for tidx, timestep in enumerate(timesteps):
+            if tidx > 0:
+                cells = sim_well.cells(tidx)
+                print(
+                    "well: "
+                    + sim_well.name
+                    + " timestep: "
+                    + str(tidx)
+                    + " cells:"
+                    + str(len(cells))
+                )
+                assert len(cells) == expected_cell_count[sim_well.name]
```

### Comparing `rips-2023.6.0.1/rips/tests/test_summary_cases.py` & `rips-2023.6.0.2/rips/tests/test_summary_cases.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import sys
-import os
-import math
-import contextlib
-import os
-import shutil
-import tempfile
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_summary_import_and_find(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
-    summary_case = rips_instance.project.import_summary_case(casePath)
-    assert summary_case.id == 1
-
-    case_id = 234
-    found_summary_case = rips_instance.project.summary_case(case_id)
-    assert found_summary_case is None
-
-    correct_case_id = 1
-    found_summary_case = rips_instance.project.summary_case(correct_case_id)
-    assert found_summary_case is not None
-
-    rips_instance.project.close()
-    correct_case_id = 1
-    found_summary_case = rips_instance.project.summary_case(correct_case_id)
-    assert found_summary_case is None
-
-
-def test_summary_data(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
-    summary_case = rips_instance.project.import_summary_case(casePath)
-    assert summary_case.id == 1
-
-    addresses = summary_case.available_addresses()
-    # Summary reader type is controlled from Preferences. libecl reports 343 vectors, opm_common (ESMRY) reports 339.
-    # As this configuration can be different, allow both variants
-    assert len(addresses.values) == 335 or len(addresses.values) == 339
-
-    summary_data = summary_case.summary_vector_values("FOPT")
-    assert len(summary_data.values) == 60
-
-
-def test_summary_resample(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
-    summary_case = rips_instance.project.import_summary_case(casePath)
-    assert summary_case.id == 1
-
-    summary_data_sampled = summary_case.resample_values("FOPT", "NONE")
-    assert len(summary_data_sampled.values) == 60
-    assert len(summary_data_sampled.time_steps) == 60
-
-    summary_data_sampled = summary_case.resample_values("FOPT", "DAY")
-    assert len(summary_data_sampled.values) == 721
-    assert len(summary_data_sampled.time_steps) == 721
-
-    summary_data_sampled = summary_case.resample_values("FOPT", "MONTH")
-    assert len(summary_data_sampled.values) == 24
-    assert len(summary_data_sampled.time_steps) == 24
-
-    summary_data_sampled = summary_case.resample_values("FOPT", "QUARTER")
-    assert len(summary_data_sampled.values) == 8
-    assert len(summary_data_sampled.time_steps) == 8
-
-    summary_data_sampled = summary_case.resample_values("FOPT", "YEAR")
-    assert len(summary_data_sampled.values) == 3
-    assert len(summary_data_sampled.time_steps) == 3
-
-
-@contextlib.contextmanager
-def cd(newdir, cleanup=lambda: True):
-    prevdir = os.getcwd()
-    os.chdir(os.path.expanduser(newdir))
-    try:
-        yield
-    finally:
-        os.chdir(prevdir)
-        cleanup()
-
-
-@contextlib.contextmanager
-def tempdir():
-    dirpath = tempfile.mkdtemp()
-
-    def cleanup():
-        shutil.rmtree(dirpath)
-
-    with cd(dirpath, cleanup):
-        yield dirpath
-
-
-def test_summary_set_values(rips_instance, initialize_test):
-    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
-    summary_case = rips_instance.project.import_summary_case(casePath)
-    assert summary_case.id == 1
-
-    addresses = summary_case.available_addresses()
-    original_keyword_count = len(addresses.values)
-
-    summary_data = summary_case.summary_vector_values("FOPT")
-    assert len(summary_data.values) == 60
-
-    summary_case.set_summary_values("FOPT_1", "", summary_data.values)
-    generated_summary_data = summary_case.summary_vector_values("FOPT_1")
-    assert len(generated_summary_data.values) == 60
-
-    addresses = summary_case.available_addresses()
-    current_keyword_count = len(addresses.values)
-    assert current_keyword_count == original_keyword_count + 1
-
-    # Using existing keyword will overwrite existing data
-    summary_case.set_summary_values("FOPT_1", "", summary_data.values)
-    addresses = summary_case.available_addresses()
-    current_keyword_count = len(addresses.values)
-    assert current_keyword_count == original_keyword_count + 1
-
-    # invalid value count, check that available addresses are unchanged
-    summary_case.set_summary_values("FOPT_2", "", [])
-    addresses = summary_case.available_addresses()
-    current_keyword_count = len(addresses.values)
-    assert current_keyword_count == original_keyword_count + 1
+import sys
+import os
+import math
+import contextlib
+import os
+import shutil
+import tempfile
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_summary_import_and_find(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
+    summary_case = rips_instance.project.import_summary_case(casePath)
+    assert summary_case.id == 1
+
+    case_id = 234
+    found_summary_case = rips_instance.project.summary_case(case_id)
+    assert found_summary_case is None
+
+    correct_case_id = 1
+    found_summary_case = rips_instance.project.summary_case(correct_case_id)
+    assert found_summary_case is not None
+
+    rips_instance.project.close()
+    correct_case_id = 1
+    found_summary_case = rips_instance.project.summary_case(correct_case_id)
+    assert found_summary_case is None
+
+
+def test_summary_data(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
+    summary_case = rips_instance.project.import_summary_case(casePath)
+    assert summary_case.id == 1
+
+    addresses = summary_case.available_addresses()
+    # Summary reader type is controlled from Preferences. libecl reports 343 vectors, opm_common (ESMRY) reports 339.
+    # As this configuration can be different, allow both variants
+    assert len(addresses.values) == 335 or len(addresses.values) == 339
+
+    summary_data = summary_case.summary_vector_values("FOPT")
+    assert len(summary_data.values) == 60
+
+
+def test_summary_resample(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
+    summary_case = rips_instance.project.import_summary_case(casePath)
+    assert summary_case.id == 1
+
+    summary_data_sampled = summary_case.resample_values("FOPT", "NONE")
+    assert len(summary_data_sampled.values) == 60
+    assert len(summary_data_sampled.time_steps) == 60
+
+    summary_data_sampled = summary_case.resample_values("FOPT", "DAY")
+    assert len(summary_data_sampled.values) == 721
+    assert len(summary_data_sampled.time_steps) == 721
+
+    summary_data_sampled = summary_case.resample_values("FOPT", "MONTH")
+    assert len(summary_data_sampled.values) == 24
+    assert len(summary_data_sampled.time_steps) == 24
+
+    summary_data_sampled = summary_case.resample_values("FOPT", "QUARTER")
+    assert len(summary_data_sampled.values) == 8
+    assert len(summary_data_sampled.time_steps) == 8
+
+    summary_data_sampled = summary_case.resample_values("FOPT", "YEAR")
+    assert len(summary_data_sampled.values) == 3
+    assert len(summary_data_sampled.time_steps) == 3
+
+
+@contextlib.contextmanager
+def cd(newdir, cleanup=lambda: True):
+    prevdir = os.getcwd()
+    os.chdir(os.path.expanduser(newdir))
+    try:
+        yield
+    finally:
+        os.chdir(prevdir)
+        cleanup()
+
+
+@contextlib.contextmanager
+def tempdir():
+    dirpath = tempfile.mkdtemp()
+
+    def cleanup():
+        shutil.rmtree(dirpath)
+
+    with cd(dirpath, cleanup):
+        yield dirpath
+
+
+def test_summary_set_values(rips_instance, initialize_test):
+    casePath = dataroot.PATH + "/flow_diagnostics_test/SIMPLE_SUMMARY2.SMSPEC"
+    summary_case = rips_instance.project.import_summary_case(casePath)
+    assert summary_case.id == 1
+
+    addresses = summary_case.available_addresses()
+    original_keyword_count = len(addresses.values)
+
+    summary_data = summary_case.summary_vector_values("FOPT")
+    assert len(summary_data.values) == 60
+
+    summary_case.set_summary_values("FOPT_1", "", summary_data.values)
+    generated_summary_data = summary_case.summary_vector_values("FOPT_1")
+    assert len(generated_summary_data.values) == 60
+
+    addresses = summary_case.available_addresses()
+    current_keyword_count = len(addresses.values)
+    assert current_keyword_count == original_keyword_count + 1
+
+    # Using existing keyword will overwrite existing data
+    summary_case.set_summary_values("FOPT_1", "", summary_data.values)
+    addresses = summary_case.available_addresses()
+    current_keyword_count = len(addresses.values)
+    assert current_keyword_count == original_keyword_count + 1
+
+    # invalid value count, check that available addresses are unchanged
+    summary_case.set_summary_values("FOPT_2", "", [])
+    addresses = summary_case.available_addresses()
+    current_keyword_count = len(addresses.values)
+    assert current_keyword_count == original_keyword_count + 1
```

### Comparing `rips-2023.6.0.1/rips/tests/test_surfaces.py` & `rips-2023.6.0.2/rips/tests/test_surfaces.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import sys
-import os
-import tempfile
-from pathlib import Path
-import pytest
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-@pytest.mark.skipif(
-    sys.platform.startswith("linux"),
-    reason="Brugge is currently exceptionally slow on Linux",
-)
-def test_create_and_export_surface(rips_instance, initialize_test):
-    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    assert len(case.grids()) == 1
-
-    surface_collection = rips_instance.project.descendants(rips.SurfaceCollection)[0]
-
-    surface = surface_collection.new_surface(case, 5)
-    assert surface
-
-    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
-        path = Path(tmpdirname, "mysurface.ts")
-        print("Temporary folder: ", path.as_posix())
-
-        fname = surface.export_to_file(path.as_posix())
-        assert len(fname.values) == 1
-
-        assert path.exists()
+import sys
+import os
+import tempfile
+from pathlib import Path
+import pytest
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+@pytest.mark.skipif(
+    sys.platform.startswith("linux"),
+    reason="Brugge is currently exceptionally slow on Linux",
+)
+def test_create_and_export_surface(rips_instance, initialize_test):
+    case_path = dataroot.PATH + "/Case_with_10_timesteps/Real0/BRUGGE_0000.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    assert len(case.grids()) == 1
+
+    surface_collection = rips_instance.project.descendants(rips.SurfaceCollection)[0]
+
+    surface = surface_collection.new_surface(case, 5)
+    assert surface
+
+    with tempfile.TemporaryDirectory(prefix="rips") as tmpdirname:
+        path = Path(tmpdirname, "mysurface.ts")
+        print("Temporary folder: ", path.as_posix())
+
+        fname = surface.export_to_file(path.as_posix())
+        assert len(fname.values) == 1
+
+        assert path.exists()
```

### Comparing `rips-2023.6.0.1/rips/tests/test_wells.py` & `rips-2023.6.0.2/rips/tests/test_wells.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import sys
-import os
-
-sys.path.insert(1, os.path.join(sys.path[0], "../../"))
-import rips
-
-import dataroot
-
-
-def test_10k(rips_instance, initialize_test):
-    case_root_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC"
-    case_path = case_root_path + "/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    assert len(case.grids()) == 2
-    well_path_files = [
-        case_root_path + "/wellpath_a.dev",
-        case_root_path + "/wellpath_b.dev",
-    ]
-    well_path_names = rips_instance.project.import_well_paths(well_path_files)
-    wells = rips_instance.project.well_paths()
-    assert len(wells) == 2
-    assert wells[0].name == "Well Path A"
-    assert wells[1].name == "Well Path B"
-
-
-def test_10k_intersection(rips_instance, initialize_test):
-    case_root_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC"
-    case_path = case_root_path + "/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-    assert len(case.grids()) == 2
-    well_path_files = [
-        case_root_path + "/wellpath_a.dev",
-    ]
-
-    view = case.create_view()
-    view.set_time_step(1)
-
-    well_path_names = rips_instance.project.import_well_paths(well_path_files)
-    wells = rips_instance.project.well_paths()
-    well_path = wells[0]
-
-    # Add a curve intersection based on the well path
-    intersection_coll = rips_instance.project.descendants(rips.IntersectionCollection)[
-        0
-    ]
-    well_path_intersection = intersection_coll.add_new_object(rips.CurveIntersection)
-    well_path_intersection.type = "CS_WELL_PATH"
-    well_path_intersection.well_path = well_path
-    well_path_intersection.update()
-
-    # Three coords per triangle
-    geometry = well_path_intersection.geometry()
-    coord_count = len(geometry.x_coords)
-    assert coord_count == 13254
-
-    # One value per triangle
-    geometry_result_values = well_path_intersection.geometry_result()
-    result_count = len(geometry_result_values.values)
-    assert result_count == 4418
-
-    # Three coords per triangle, one result value per triangle
-    assert (result_count * 3) == coord_count
-
-
-def test_empty_well_intersection(rips_instance, initialize_test):
-    case_root_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC"
-    case_path = case_root_path + "/TEST10K_FLT_LGR_NNC.EGRID"
-    case = rips_instance.project.load_case(path=case_path)
-
-    view = case.create_view()
-    view.set_time_step(1)
-
-    # Add a curve intersection based on the well path
-    intersection_coll = rips_instance.project.descendants(rips.IntersectionCollection)[
-        0
-    ]
-
-    well_path_intersection = intersection_coll.add_new_object(rips.CurveIntersection)
-    well_path_intersection.type = "CS_WELL_PATH"
-    well_path_intersection.well_path = None
-    well_path_intersection.update()
-
-    # Test with empty geometry. This will also test that an empty list in CAF is converted to an empty list in Python
-    # See __makelist in pdmobject.py
-    geometry = well_path_intersection.geometry()
-    coord_count = len(geometry.x_coords)
-    assert coord_count == 0
-
-    # One value per triangle
-    geometry_result_values = well_path_intersection.geometry_result()
-    result_count = len(geometry_result_values.values)
-    assert result_count == 0
+import sys
+import os
+
+sys.path.insert(1, os.path.join(sys.path[0], "../../"))
+import rips
+
+import dataroot
+
+
+def test_10k(rips_instance, initialize_test):
+    case_root_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC"
+    case_path = case_root_path + "/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    assert len(case.grids()) == 2
+    well_path_files = [
+        case_root_path + "/wellpath_a.dev",
+        case_root_path + "/wellpath_b.dev",
+    ]
+    well_path_names = rips_instance.project.import_well_paths(well_path_files)
+    wells = rips_instance.project.well_paths()
+    assert len(wells) == 2
+    assert wells[0].name == "Well Path A"
+    assert wells[1].name == "Well Path B"
+
+
+def test_10k_intersection(rips_instance, initialize_test):
+    case_root_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC"
+    case_path = case_root_path + "/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+    assert len(case.grids()) == 2
+    well_path_files = [
+        case_root_path + "/wellpath_a.dev",
+    ]
+
+    view = case.create_view()
+    view.set_time_step(1)
+
+    well_path_names = rips_instance.project.import_well_paths(well_path_files)
+    wells = rips_instance.project.well_paths()
+    well_path = wells[0]
+
+    # Add a curve intersection based on the well path
+    intersection_coll = rips_instance.project.descendants(rips.IntersectionCollection)[
+        0
+    ]
+    well_path_intersection = intersection_coll.add_new_object(rips.CurveIntersection)
+    well_path_intersection.type = "CS_WELL_PATH"
+    well_path_intersection.well_path = well_path
+    well_path_intersection.update()
+
+    # Three coords per triangle
+    geometry = well_path_intersection.geometry()
+    coord_count = len(geometry.x_coords)
+    assert coord_count == 13254
+
+    # One value per triangle
+    geometry_result_values = well_path_intersection.geometry_result()
+    result_count = len(geometry_result_values.values)
+    assert result_count == 4418
+
+    # Three coords per triangle, one result value per triangle
+    assert (result_count * 3) == coord_count
+
+
+def test_empty_well_intersection(rips_instance, initialize_test):
+    case_root_path = dataroot.PATH + "/TEST10K_FLT_LGR_NNC"
+    case_path = case_root_path + "/TEST10K_FLT_LGR_NNC.EGRID"
+    case = rips_instance.project.load_case(path=case_path)
+
+    view = case.create_view()
+    view.set_time_step(1)
+
+    # Add a curve intersection based on the well path
+    intersection_coll = rips_instance.project.descendants(rips.IntersectionCollection)[
+        0
+    ]
+
+    well_path_intersection = intersection_coll.add_new_object(rips.CurveIntersection)
+    well_path_intersection.type = "CS_WELL_PATH"
+    well_path_intersection.well_path = None
+    well_path_intersection.update()
+
+    # Test with empty geometry. This will also test that an empty list in CAF is converted to an empty list in Python
+    # See __makelist in pdmobject.py
+    geometry = well_path_intersection.geometry()
+    coord_count = len(geometry.x_coords)
+    assert coord_count == 0
+
+    # One value per triangle
+    geometry_result_values = well_path_intersection.geometry_result()
+    result_count = len(geometry_result_values.values)
+    assert result_count == 0
```

### Comparing `rips-2023.6.0.1/rips/view.py` & `rips-2023.6.0.2/rips/view.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-"""
-ResInsight 3d view module
-"""
-
-import builtins
-import Commands_pb2 as Cmd
-
-import rips.case  # Circular import of Case, which already imports View. Use full name.
-from .pdmobject import add_method
-from .resinsight_classes import View, ViewWindow, EclipseView, GeoMechView
-
-
-@add_method(View)
-def apply_cell_result(self, result_type, result_variable):
-    """Apply a regular cell result
-
-    Arguments:
-        result_type (str): String representing the result category. The valid values are::
-            - DYNAMIC_NATIVE
-            - STATIC_NATIVE
-            - SOURSIMRL
-            - GENERATED
-            - INPUT_PROPERTY
-            - FORMATION_NAMES
-            - FLOW_DIAGNOSTICS
-            - INJECTION_FLOODING
-        result_variable (str): String representing the result variable.
-    """
-    cell_result = self.cell_result()
-    cell_result.result_type = result_type
-    cell_result.result_variable = result_variable
-    cell_result.update()
-
-
-@add_method(View)
-def apply_flow_diagnostics_cell_result(
-    self,
-    result_variable="TOF",
-    selection_mode="FLOW_TR_BY_SELECTION",
-    injectors=None,
-    producers=None,
-):
-    """Apply a flow diagnostics cell result
-
-    **Parameters**::
-
-        Parameter           | Description                                            | Type
-        ------------------- | ------------------------------------------------------ | -----
-        result_variable     | String representing the result value                   | String
-        selection_mode      | String specifying which tracers to select              | String
-        injectors           | List of injector names, used by 'FLOW_TR_BY_SELECTION' | String List
-        producers           | List of injector names, used by 'FLOW_TR_BY_SELECTION' | String List
-
-    **Enum compdat_export**::
-
-        Option                  | Description
-        ------------------------| ------------
-        "TOF"                   | Time of flight
-        "Fraction"              | Fraction
-        "MaxFractionTracer"     | Max Fraction Tracer
-        "Communication"         | Communication
-
-    """
-    if injectors is None:
-        injectors = []
-    if producers is None:
-        producers = []
-    cell_result = self.cell_result()
-    cell_result.result_type = "FLOW_DIAGNOSTICS"
-    cell_result.result_variable = result_variable
-    cell_result.flow_tracer_selection_mode = selection_mode
-    if selection_mode == "FLOW_TR_BY_SELECTION":
-        cell_result.selected_injector_tracers = injectors
-        cell_result.selected_producer_tracers = producers
-    cell_result.update()
-
-
-@add_method(View)
-def clone(self):
-    """Clone the current view"""
-    view_id = self._execute_command(
-        cloneView=Cmd.CloneViewRequest(viewId=self.id)
-    ).createViewResult.viewId
-    return self.case().view(view_id)
-
-
-@add_method(View)
-def set_time_step(self, time_step):
-    """Set the time step for current view"""
-    case_id = self.case().id
-    return self._execute_command(
-        setTimeStep=Cmd.SetTimeStepParams(
-            caseId=case_id, viewId=self.id, timeStep=time_step
-        )
-    )
-
-
-@add_method(View)
-def export_sim_well_fracture_completions(
-    self, time_step, simulation_well_names, file_split, compdat_export
-):
-    """Export fracture completions for simulation wells
-
-    **Parameters**::
-
-        Parameter                   | Description                                      | Type
-        ----------------------------| ------------------------------------------------ | -----
-        time_step                   | Time step to export for                          | Integer
-        simulation_well_names       | List of simulation well names                    | List
-        file_split                  | Controls how export data is split into files     | String enum
-        compdat_export              | Compdat export type                              | String enum
-
-    **Enum file_split**::
-
-        Option                              | Description
-        ----------------------------------- | ------------
-        "UNIFIED_FILE" <b>Default Option</b>| A single file with all transmissibilities
-        "SPLIT_ON_WELL"                     | One file for each well transmissibilities
-        "SPLIT_ON_WELL_AND_COMPLETION_TYPE" | One file for each completion type for each well
-
-    **Enum compdat_export**::
-
-        Option                                   | Description
-        -----------------------------------------| ------------
-        "TRANSMISSIBILITIES"<b>Default Option</b>| Direct export of transmissibilities
-        "WPIMULT_AND_DEFAULT_CONNECTION_FACTORS" | Include export of WPIMULT
-
-    """
-    if isinstance(simulation_well_names, str):
-        simulation_well_names = [simulation_well_names]
-
-    case_id = self.case().id
-    return self._execute_command(
-        exportSimWellFractureCompletions=Cmd.ExportSimWellPathFracRequest(
-            caseId=case_id,
-            viewId=self.id,
-            timeStep=time_step,
-            simulationWellNames=simulation_well_names,
-            fileSplit=file_split,
-            compdatExport=compdat_export,
-        )
-    )
-
-
-@add_method(View)
-def export_visible_cells(
-    self,
-    export_keyword="FLUXNUM",
-    visible_active_cells_value=1,
-    hidden_active_cells_value=0,
-    inactive_cells_value=0,
-):
-    """Export special properties for all visible cells.
-
-    Arguments:
-        export_keyword (string): The keyword to export.
-        Choices: 'FLUXNUM' or 'MULTNUM'. Default: 'FLUXNUM'
-        visible_active_cells_value (int): Value to export forvisible active cells. Default: 1
-        hidden_active_cells_value (int): Value to export for hidden active cells. Default: 0
-        inactive_cells_value (int): Value to export for inactive cells. Default: 0
-    """
-    case_id = self.case().id
-    return self._execute_command(
-        exportVisibleCells=Cmd.ExportVisibleCellsRequest(
-            caseId=case_id,
-            viewId=self.id,
-            exportKeyword=export_keyword,
-            visibleActiveCellsValue=visible_active_cells_value,
-            hiddenActiveCellsValue=hidden_active_cells_value,
-            inactiveCellsValue=inactive_cells_value,
-        )
-    )
-
-
-@add_method(View)
-def export_property(self, undefined_value=0.0):
-    """Export the current Eclipse property from the view
-
-    Arguments:
-        undefined_value (double): Value to use for undefined values. Defaults to 0.0
-    """
-    case_id = self.case().id
-    return self._execute_command(
-        exportPropertyInViews=Cmd.ExportPropertyInViewsRequest(
-            caseId=case_id, viewIds=[self.id], undefinedValue=undefined_value
-        )
-    )
-
-
-@add_method(ViewWindow)
-def case(self):
-    """Get the case the view belongs to"""
-    mycase = self.ancestor(rips.case.Case)
-    assert mycase is not None
-    return mycase
-
-
-@add_method(ViewWindow)
-def export_snapshot(self, prefix="", export_folder=""):
-    """Export snapshot for the current view
-
-    Arguments:
-        prefix (str): Exported file name prefix
-        export_folder(str): The path to export to. By default will use the global export folder
-    """
-    case_id = self.case().id
-    return self._execute_command(
-        exportSnapshots=Cmd.ExportSnapshotsRequest(
-            type="VIEWS",
-            prefix=prefix,
-            caseId=case_id,
-            viewId=self.id,
-            exportFolder=export_folder,
-        )
-    )
+"""
+ResInsight 3d view module
+"""
+
+import builtins
+import Commands_pb2 as Cmd
+
+import rips.case  # Circular import of Case, which already imports View. Use full name.
+from .pdmobject import add_method
+from .resinsight_classes import View, ViewWindow, EclipseView, GeoMechView
+
+
+@add_method(View)
+def apply_cell_result(self, result_type, result_variable):
+    """Apply a regular cell result
+
+    Arguments:
+        result_type (str): String representing the result category. The valid values are::
+            - DYNAMIC_NATIVE
+            - STATIC_NATIVE
+            - SOURSIMRL
+            - GENERATED
+            - INPUT_PROPERTY
+            - FORMATION_NAMES
+            - FLOW_DIAGNOSTICS
+            - INJECTION_FLOODING
+        result_variable (str): String representing the result variable.
+    """
+    cell_result = self.cell_result()
+    cell_result.result_type = result_type
+    cell_result.result_variable = result_variable
+    cell_result.update()
+
+
+@add_method(View)
+def apply_flow_diagnostics_cell_result(
+    self,
+    result_variable="TOF",
+    selection_mode="FLOW_TR_BY_SELECTION",
+    injectors=None,
+    producers=None,
+):
+    """Apply a flow diagnostics cell result
+
+    **Parameters**::
+
+        Parameter           | Description                                            | Type
+        ------------------- | ------------------------------------------------------ | -----
+        result_variable     | String representing the result value                   | String
+        selection_mode      | String specifying which tracers to select              | String
+        injectors           | List of injector names, used by 'FLOW_TR_BY_SELECTION' | String List
+        producers           | List of injector names, used by 'FLOW_TR_BY_SELECTION' | String List
+
+    **Enum compdat_export**::
+
+        Option                  | Description
+        ------------------------| ------------
+        "TOF"                   | Time of flight
+        "Fraction"              | Fraction
+        "MaxFractionTracer"     | Max Fraction Tracer
+        "Communication"         | Communication
+
+    """
+    if injectors is None:
+        injectors = []
+    if producers is None:
+        producers = []
+    cell_result = self.cell_result()
+    cell_result.result_type = "FLOW_DIAGNOSTICS"
+    cell_result.result_variable = result_variable
+    cell_result.flow_tracer_selection_mode = selection_mode
+    if selection_mode == "FLOW_TR_BY_SELECTION":
+        cell_result.selected_injector_tracers = injectors
+        cell_result.selected_producer_tracers = producers
+    cell_result.update()
+
+
+@add_method(View)
+def clone(self):
+    """Clone the current view"""
+    view_id = self._execute_command(
+        cloneView=Cmd.CloneViewRequest(viewId=self.id)
+    ).createViewResult.viewId
+    return self.case().view(view_id)
+
+
+@add_method(View)
+def set_time_step(self, time_step):
+    """Set the time step for current view"""
+    case_id = self.case().id
+    return self._execute_command(
+        setTimeStep=Cmd.SetTimeStepParams(
+            caseId=case_id, viewId=self.id, timeStep=time_step
+        )
+    )
+
+
+@add_method(View)
+def export_sim_well_fracture_completions(
+    self, time_step, simulation_well_names, file_split, compdat_export
+):
+    """Export fracture completions for simulation wells
+
+    **Parameters**::
+
+        Parameter                   | Description                                      | Type
+        ----------------------------| ------------------------------------------------ | -----
+        time_step                   | Time step to export for                          | Integer
+        simulation_well_names       | List of simulation well names                    | List
+        file_split                  | Controls how export data is split into files     | String enum
+        compdat_export              | Compdat export type                              | String enum
+
+    **Enum file_split**::
+
+        Option                              | Description
+        ----------------------------------- | ------------
+        "UNIFIED_FILE" <b>Default Option</b>| A single file with all transmissibilities
+        "SPLIT_ON_WELL"                     | One file for each well transmissibilities
+        "SPLIT_ON_WELL_AND_COMPLETION_TYPE" | One file for each completion type for each well
+
+    **Enum compdat_export**::
+
+        Option                                   | Description
+        -----------------------------------------| ------------
+        "TRANSMISSIBILITIES"<b>Default Option</b>| Direct export of transmissibilities
+        "WPIMULT_AND_DEFAULT_CONNECTION_FACTORS" | Include export of WPIMULT
+
+    """
+    if isinstance(simulation_well_names, str):
+        simulation_well_names = [simulation_well_names]
+
+    case_id = self.case().id
+    return self._execute_command(
+        exportSimWellFractureCompletions=Cmd.ExportSimWellPathFracRequest(
+            caseId=case_id,
+            viewId=self.id,
+            timeStep=time_step,
+            simulationWellNames=simulation_well_names,
+            fileSplit=file_split,
+            compdatExport=compdat_export,
+        )
+    )
+
+
+@add_method(View)
+def export_visible_cells(
+    self,
+    export_keyword="FLUXNUM",
+    visible_active_cells_value=1,
+    hidden_active_cells_value=0,
+    inactive_cells_value=0,
+):
+    """Export special properties for all visible cells.
+
+    Arguments:
+        export_keyword (string): The keyword to export.
+        Choices: 'FLUXNUM' or 'MULTNUM'. Default: 'FLUXNUM'
+        visible_active_cells_value (int): Value to export forvisible active cells. Default: 1
+        hidden_active_cells_value (int): Value to export for hidden active cells. Default: 0
+        inactive_cells_value (int): Value to export for inactive cells. Default: 0
+    """
+    case_id = self.case().id
+    return self._execute_command(
+        exportVisibleCells=Cmd.ExportVisibleCellsRequest(
+            caseId=case_id,
+            viewId=self.id,
+            exportKeyword=export_keyword,
+            visibleActiveCellsValue=visible_active_cells_value,
+            hiddenActiveCellsValue=hidden_active_cells_value,
+            inactiveCellsValue=inactive_cells_value,
+        )
+    )
+
+
+@add_method(View)
+def export_property(self, undefined_value=0.0):
+    """Export the current Eclipse property from the view
+
+    Arguments:
+        undefined_value (double): Value to use for undefined values. Defaults to 0.0
+    """
+    case_id = self.case().id
+    return self._execute_command(
+        exportPropertyInViews=Cmd.ExportPropertyInViewsRequest(
+            caseId=case_id, viewIds=[self.id], undefinedValue=undefined_value
+        )
+    )
+
+
+@add_method(ViewWindow)
+def case(self):
+    """Get the case the view belongs to"""
+    mycase = self.ancestor(rips.case.Case)
+    assert mycase is not None
+    return mycase
+
+
+@add_method(ViewWindow)
+def export_snapshot(self, prefix="", export_folder=""):
+    """Export snapshot for the current view
+
+    Arguments:
+        prefix (str): Exported file name prefix
+        export_folder(str): The path to export to. By default will use the global export folder
+    """
+    case_id = self.case().id
+    return self._execute_command(
+        exportSnapshots=Cmd.ExportSnapshotsRequest(
+            type="VIEWS",
+            prefix=prefix,
+            caseId=case_id,
+            viewId=self.id,
+            exportFolder=export_folder,
+        )
+    )
```

### Comparing `rips-2023.6.0.1/rips/well_log_plot.py` & `rips-2023.6.0.2/rips/well_log_plot.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""
-ResInsight Well Log Plot plot module
-"""
-
-import Commands_pb2
-
-from .plot import Plot
-from .pdmobject import PdmObjectBase, add_method
-from .resinsight_classes import WellLogPlot
-
-
-@add_method(WellLogPlot)
-def export_data_as_las(
-    self,
-    export_folder,
-    file_prefix="",
-    export_tvdrkb=False,
-    capitalize_file_names=False,
-    resample_interval=0.0,
-    convert_to_standard_units=False,
-):
-    """Export LAS file(s) for the current plot
-
-    Arguments:
-        export_folder(str): The path to export to. By default will use the global export folder
-        file_prefix (str): Exported file name prefix
-        export_tvdrkb(bool): Export in TVD-RKB format
-        capitalize_file_names(bool): Make all file names upper case
-        resample_interval(double): if > 0.0 the files will be resampled
-
-    Returns:
-        A list of files exported
-    """
-    res = self._execute_command(
-        exportWellLogPlotData=Commands_pb2.ExportWellLogPlotDataRequest(
-            exportFormat="LAS",
-            viewId=self.id,
-            exportFolder=export_folder,
-            filePrefix=file_prefix,
-            exportTvdRkb=export_tvdrkb,
-            capitalizeFileNames=capitalize_file_names,
-            resampleInterval=resample_interval,
-            convertCurveUnits=convert_to_standard_units,
-        )
-    )
-    return res.exportWellLogPlotDataResult.exportedFiles
-
-
-@add_method(WellLogPlot)
-def export_data_as_ascii(
-    self, export_folder, file_prefix="", capitalize_file_names=False
-):
-    """Export LAS file(s) for the current plot
-
-    Arguments:
-        export_folder(str): The path to export to. By default will use the global export folder
-        file_prefix (str): Exported file name prefix
-        capitalize_file_names(bool): Make all file names upper case
-
-    Returns:
-        A list of files exported
-    """
-    res = self._execute_command(
-        exportWellLogPlotData=Commands_pb2.ExportWellLogPlotDataRequest(
-            exportFormat="ASCII",
-            viewId=self.id,
-            exportFolder=export_folder,
-            filePrefix=file_prefix,
-            exportTvdRkb=False,
-            capitalizeFileNames=capitalize_file_names,
-            resampleInterval=0.0,
-        )
-    )
-    return res.exportWellLogPlotDataResult.exportedFiles
+"""
+ResInsight Well Log Plot plot module
+"""
+
+import Commands_pb2
+
+from .plot import Plot
+from .pdmobject import PdmObjectBase, add_method
+from .resinsight_classes import WellLogPlot
+
+
+@add_method(WellLogPlot)
+def export_data_as_las(
+    self,
+    export_folder,
+    file_prefix="",
+    export_tvdrkb=False,
+    capitalize_file_names=False,
+    resample_interval=0.0,
+    convert_to_standard_units=False,
+):
+    """Export LAS file(s) for the current plot
+
+    Arguments:
+        export_folder(str): The path to export to. By default will use the global export folder
+        file_prefix (str): Exported file name prefix
+        export_tvdrkb(bool): Export in TVD-RKB format
+        capitalize_file_names(bool): Make all file names upper case
+        resample_interval(double): if > 0.0 the files will be resampled
+
+    Returns:
+        A list of files exported
+    """
+    res = self._execute_command(
+        exportWellLogPlotData=Commands_pb2.ExportWellLogPlotDataRequest(
+            exportFormat="LAS",
+            viewId=self.id,
+            exportFolder=export_folder,
+            filePrefix=file_prefix,
+            exportTvdRkb=export_tvdrkb,
+            capitalizeFileNames=capitalize_file_names,
+            resampleInterval=resample_interval,
+            convertCurveUnits=convert_to_standard_units,
+        )
+    )
+    return res.exportWellLogPlotDataResult.exportedFiles
+
+
+@add_method(WellLogPlot)
+def export_data_as_ascii(
+    self, export_folder, file_prefix="", capitalize_file_names=False
+):
+    """Export LAS file(s) for the current plot
+
+    Arguments:
+        export_folder(str): The path to export to. By default will use the global export folder
+        file_prefix (str): Exported file name prefix
+        capitalize_file_names(bool): Make all file names upper case
+
+    Returns:
+        A list of files exported
+    """
+    res = self._execute_command(
+        exportWellLogPlotData=Commands_pb2.ExportWellLogPlotDataRequest(
+            exportFormat="ASCII",
+            viewId=self.id,
+            exportFolder=export_folder,
+            filePrefix=file_prefix,
+            exportTvdRkb=False,
+            capitalizeFileNames=capitalize_file_names,
+            resampleInterval=0.0,
+        )
+    )
+    return res.exportWellLogPlotDataResult.exportedFiles
```

### Comparing `rips-2023.6.0.1/rips.egg-info/SOURCES.txt` & `rips-2023.6.0.2/rips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rips-2023.6.0.1/setup.py` & `rips-2023.6.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
-
-with open('README.md') as f:
-    readme = f.read()
-
-with open('LICENSE') as f:
-	license = f.read()
-
-RIPS_DIST_VERSION = '1'
-	
-setup(
-    name='rips',
-    version='2023.06.0.' + RIPS_DIST_VERSION,
-    description='Python Interface for ResInsight',
-    long_description=readme,
-    author='Ceetron Solutions',
-    author_email='info@ceetronsolutions.com',
-    url='http://www.resinsight.org',
-    license=license,
-    packages=['rips'],
-    package_data={'rips': ['*.py', 'generated/*.py', 'PythonExamples/*.py', 'tests/*.py']},
-    install_requires=['grpcio>=1.20.0', 'protobuf', 'wheel']
-)
+from setuptools import setup, find_packages
+
+with open('README.md') as f:
+    readme = f.read()
+
+with open('LICENSE') as f:
+	license = f.read()
+
+RIPS_DIST_VERSION = '2'
+	
+setup(
+    name='rips',
+    version='2023.06.0.' + RIPS_DIST_VERSION,
+    description='Python Interface for ResInsight',
+    long_description=readme,
+    author='Ceetron Solutions',
+    author_email='info@ceetronsolutions.com',
+    url='http://www.resinsight.org',
+    license=license,
+    packages=['rips'],
+    package_data={'rips': ['*.py', 'generated/*.py', 'PythonExamples/*.py', 'tests/*.py']},
+    install_requires=['grpcio>=1.20.0', 'protobuf', 'wheel']
+)
```

