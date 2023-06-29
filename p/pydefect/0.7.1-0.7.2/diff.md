# Comparing `tmp/pydefect-0.7.1.tar.gz` & `tmp/pydefect-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydefect-0.7.1.tar", last modified: Sat May 20 00:06:15 2023, max compression
+gzip compressed data, was "dist/pydefect-0.7.2.tar", last modified: Thu Jun 29 09:06:44 2023, max compression
```

## Comparing `pydefect-0.7.1.tar` & `pydefect-0.7.2.tar`

### file list

```diff
@@ -1,272 +1,242 @@
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.152753 pydefect-0.7.1/
--rw-r--r--   0 kumagai    (501) staff       (20)       54 2021-03-12 02:40:59.000000 pydefect-0.7.1/MANIFEST.in
--rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-05-20 00:06:15.152455 pydefect-0.7.1/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     4563 2022-08-17 09:42:29.000000 pydefect-0.7.1/README.md
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.010738 pydefect-0.7.1/pydefect/
--rw-r--r--   0 kumagai    (501) staff       (20)       21 2023-05-20 00:05:58.000000 pydefect-0.7.1/pydefect/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.037593 pydefect-0.7.1/pydefect/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2840 2021-04-02 01:38:50.000000 pydefect-0.7.1/pydefect/analyzer/_defect_charge_distribution.py
--rw-r--r--   0 kumagai    (501) staff       (20)    11690 2023-02-21 04:23:52.000000 pydefect-0.7.1/pydefect/analyzer/band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1334 2021-05-01 01:17:09.000000 pydefect-0.7.1/pydefect/analyzer/calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2426 2021-05-26 07:04:12.000000 pydefect-0.7.1/pydefect/analyzer/calc_summary.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.040948 pydefect-0.7.1/pydefect/analyzer/concentration/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:15.000000 pydefect-0.7.1/pydefect/analyzer/concentration/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5631 2023-02-08 05:36:42.000000 pydefect-0.7.1/pydefect/analyzer/concentration/concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2973 2023-02-01 00:50:27.000000 pydefect-0.7.1/pydefect/analyzer/concentration/degeneracy.py
--rw-r--r--   0 kumagai    (501) staff       (20)      385 2023-01-30 01:10:12.000000 pydefect-0.7.1/pydefect/analyzer/concentration/distribution_function.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7772 2023-02-08 07:02:02.000000 pydefect-0.7.1/pydefect/analyzer/concentration/make_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2462 2023-03-09 04:26:39.000000 pydefect-0.7.1/pydefect/analyzer/concentration/plot_concentration.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.044379 pydefect-0.7.1/pydefect/analyzer/dash_components/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-21 04:26:43.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5094 2021-08-15 04:39:32.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1754 2021-05-27 10:09:51.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py
--rw-r--r--   0 kumagai    (501) staff       (20)      929 2021-05-27 09:07:43.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_plotter_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8866 2021-04-04 05:43:59.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6859 2021-04-04 05:43:59.000000 pydefect-0.7.1/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4716 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/analyzer/defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12944 2023-03-12 22:54:57.000000 pydefect-0.7.1/pydefect/analyzer/defect_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9945 2023-01-31 04:11:38.000000 pydefect-0.7.1/pydefect/analyzer/defect_energy_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1280 2022-11-15 04:48:53.000000 pydefect-0.7.1/pydefect/analyzer/defect_energy_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7741 2022-09-30 05:43:38.000000 pydefect-0.7.1/pydefect/analyzer/defect_structure_comparator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6536 2023-01-28 01:55:02.000000 pydefect-0.7.1/pydefect/analyzer/defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10186 2021-06-04 06:03:27.000000 pydefect-0.7.1/pydefect/analyzer/eigenvalue_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2420 2021-08-06 10:11:01.000000 pydefect-0.7.1/pydefect/analyzer/grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7225 2022-11-22 05:43:00.000000 pydefect-0.7.1/pydefect/analyzer/make_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1571 2021-05-26 07:04:53.000000 pydefect-0.7.1/pydefect/analyzer/make_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2270 2021-08-06 10:11:46.000000 pydefect-0.7.1/pydefect/analyzer/make_defect_energy_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1716 2023-02-11 23:51:37.000000 pydefect-0.7.1/pydefect/analyzer/make_defect_energy_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6480 2022-11-19 06:15:43.000000 pydefect-0.7.1/pydefect/analyzer/make_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)      787 2022-12-08 07:12:16.000000 pydefect-0.7.1/pydefect/analyzer/pinning_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1575 2021-04-27 05:43:07.000000 pydefect-0.7.1/pydefect/analyzer/refine_defect_structure.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2279 2022-11-16 04:21:58.000000 pydefect-0.7.1/pydefect/analyzer/transition_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2006 2022-11-16 04:21:59.000000 pydefect-0.7.1/pydefect/analyzer/transition_levels_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2128 2023-03-26 01:17:24.000000 pydefect-0.7.1/pydefect/analyzer/unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.046070 pydefect-0.7.1/pydefect/chem_pot_diag/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/chem_pot_diag/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    15678 2023-01-04 05:04:29.000000 pydefect-0.7.1/pydefect/chem_pot_diag/chem_pot_diag.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10577 2022-10-10 09:09:15.000000 pydefect-0.7.1/pydefect/chem_pot_diag/cpd_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.050461 pydefect-0.7.1/pydefect/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    15399 2023-03-05 01:50:27.000000 pydefect-0.7.1/pydefect/cli/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10546 2023-05-19 23:36:53.000000 pydefect-0.7.1/pydefect/cli/main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)      289 2022-12-13 08:11:13.000000 pydefect-0.7.1/pydefect/cli/main_print_json.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2248 2023-04-06 01:32:45.000000 pydefect-0.7.1/pydefect/cli/main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10042 2023-03-09 23:27:38.000000 pydefect-0.7.1/pydefect/cli/main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6818 2023-03-09 23:26:07.000000 pydefect-0.7.1/pydefect/cli/main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4923 2021-05-02 06:20:14.000000 pydefect-0.7.1/pydefect/cli/make_defect_vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.058388 pydefect-0.7.1/pydefect/cli/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-26 08:41:03.000000 pydefect-0.7.1/pydefect/cli/vasp/__init__.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     1017 2021-04-29 04:10:12.000000 pydefect-0.7.1/pydefect/cli/vasp/get_defect_charge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9144 2022-11-22 04:59:04.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6954 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5648 2023-03-05 02:05:12.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4282 2023-03-05 02:05:12.000000 pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4770 2022-11-22 05:00:35.000000 pydefect-0.7.1/pydefect/cli/vasp/make_band_edge_orbital_infos.py
--rw-r--r--   0 kumagai    (501) staff       (20)      690 2021-04-13 03:41:39.000000 pydefect-0.7.1/pydefect/cli/vasp/make_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2221 2021-06-04 02:29:24.000000 pydefect-0.7.1/pydefect/cli/vasp/make_composition_energies_from_mp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2754 2021-05-24 05:42:28.000000 pydefect-0.7.1/pydefect/cli/vasp/make_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3728 2023-03-24 00:21:35.000000 pydefect-0.7.1/pydefect/cli/vasp/make_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2398 2020-11-25 07:07:18.000000 pydefect-0.7.1/pydefect/cli/vasp/make_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)    18748 2022-10-24 06:34:05.000000 pydefect-0.7.1/pydefect/cli/vasp/make_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1349 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/cli/vasp/make_perfect_band_edge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2471 2023-01-04 04:53:30.000000 pydefect-0.7.1/pydefect/cli/vasp/make_poscars_from_query.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1156 2021-04-25 05:20:51.000000 pydefect-0.7.1/pydefect/cli/vasp/make_unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.059832 pydefect-0.7.1/pydefect/cli/vasp/molecules/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.060735 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.061706 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/
--rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.062542 pydefect-0.7.1/pydefect/cli/vasp/molecules/N2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/N2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/N2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.063381 pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/
--rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.064335 pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/
--rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.065353 pydefect-0.7.1/pydefect/cli/vasp/molecules/O2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/O2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/O2/prior_info.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 08:59:11.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/molecule_data.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      417 2020-05-26 08:59:40.000000 pydefect-0.7.1/pydefect/cli/vasp/molecules/molecules.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.068090 pydefect-0.7.1/pydefect/corrections/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/corrections/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      523 2021-04-26 01:51:45.000000 pydefect-0.7.1/pydefect/corrections/abstract_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2042 2023-05-10 06:23:17.000000 pydefect-0.7.1/pydefect/corrections/efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4802 2020-06-06 00:50:29.000000 pydefect-0.7.1/pydefect/corrections/ewald.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2875 2020-11-26 00:07:11.000000 pydefect-0.7.1/pydefect/corrections/gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9656 2023-03-29 07:34:00.000000 pydefect-0.7.1/pydefect/corrections/site_potential_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.070382 pydefect-0.7.1/pydefect/database/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/database/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      808 2021-04-28 23:15:40.000000 pydefect-0.7.1/pydefect/database/database.py
--rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.7.1/pydefect/database/electronegativity.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.7.1/pydefect/database/oxidation_state.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.7.1/pydefect/database/rcore.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     2982 2021-06-10 06:38:20.000000 pydefect-0.7.1/pydefect/defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)      138 2020-05-13 06:54:40.000000 pydefect-0.7.1/pydefect/error.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.077411 pydefect-0.7.1/pydefect/input_maker/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:45:24.000000 pydefect-0.7.1/pydefect/input_maker/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2252 2022-11-04 06:49:00.000000 pydefect-0.7.1/pydefect/input_maker/append_interstitial.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2011 2023-03-13 01:10:20.000000 pydefect-0.7.1/pydefect/input_maker/complex_defect_entries_make.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1178 2023-03-12 23:38:44.000000 pydefect-0.7.1/pydefect/input_maker/complex_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1509 2022-09-30 06:02:01.000000 pydefect-0.7.1/pydefect/input_maker/defect.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5794 2022-09-30 06:04:45.000000 pydefect-0.7.1/pydefect/input_maker/defect_entries_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4655 2022-09-30 06:27:37.000000 pydefect-0.7.1/pydefect/input_maker/defect_entry.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1464 2022-07-01 01:20:02.000000 pydefect-0.7.1/pydefect/input_maker/defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3918 2020-11-23 04:55:46.000000 pydefect-0.7.1/pydefect/input_maker/defect_set_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2305 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/input_maker/local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3149 2023-01-28 01:22:10.000000 pydefect-0.7.1/pydefect/input_maker/manual_supercell_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3938 2023-01-28 00:19:05.000000 pydefect-0.7.1/pydefect/input_maker/supercell.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4242 2023-01-28 01:11:46.000000 pydefect-0.7.1/pydefect/input_maker/supercell_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4727 2023-05-18 07:33:28.000000 pydefect-0.7.1/pydefect/input_maker/supercell_maker.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.078243 pydefect-0.7.1/pydefect/tests/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.1/pydefect/tests/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.094353 pydefect-0.7.1/pydefect/tests/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.7.1/pydefect/tests/analyzer/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-03 11:12:30.000000 pydefect-0.7.1/pydefect/tests/analyzer/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.097026 pydefect-0.7.1/pydefect/tests/analyzer/concentration/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:35.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3177 2023-02-02 23:17:57.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1723 2023-02-01 00:50:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_degeneracy.py
--rw-r--r--   0 kumagai    (501) staff       (20)      469 2023-01-30 01:09:25.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_distribution_function.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3239 2023-03-05 02:07:50.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_make_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)      975 2023-02-08 06:50:25.000000 pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_plot_concentration.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.003173 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.003650 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.097571 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/
--rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.098235 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/
--rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)     7450 2022-09-30 03:57:34.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1022 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2402 2021-05-26 07:04:12.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2915 2021-05-03 01:56:28.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8302 2023-03-05 02:36:13.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2466 2022-11-15 07:29:49.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1540 2022-11-15 04:49:34.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7391 2022-09-30 04:57:30.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_comparator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4373 2023-01-29 23:13:01.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2636 2021-05-02 08:25:54.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_eigenvalue_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2648 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7215 2022-11-22 05:40:58.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1786 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2067 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1609 2021-05-01 06:02:47.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1665 2022-09-30 05:50:49.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1465 2022-12-08 07:12:16.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_pinning_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4262 2022-05-20 02:54:43.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_refine_defect_structure.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1796 2022-11-16 04:14:17.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1539 2022-11-16 04:16:01.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2014 2023-05-10 06:40:55.000000 pydefect-0.7.1/pydefect/tests/analyzer/test_unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.100873 pydefect-0.7.1/pydefect/tests/chem_pot_diag/
--rw-r--r--   0 kumagai    (501) staff       (20)      169 2020-11-30 07:08:52.000000 pydefect-0.7.1/pydefect/tests/chem_pot_diag/cpd.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.106560 pydefect-0.7.1/pydefect/tests/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/tests/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10308 2023-01-28 00:50:06.000000 pydefect-0.7.1/pydefect/tests/cli/test_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    11140 2023-03-05 02:10:01.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1980 2022-10-10 09:24:54.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4986 2023-03-05 02:12:51.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5290 2023-03-09 23:26:49.000000 pydefect-0.7.1/pydefect/tests/cli/test_main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3011 2021-05-15 12:24:21.000000 pydefect-0.7.1/pydefect/tests/cli/test_make_defect_vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.122265 pydefect-0.7.1/pydefect/tests/cli/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/__init__.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     1671 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_get_defect_charge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4907 2022-11-22 04:59:59.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10280 2023-05-10 06:37:49.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2748 2021-04-30 03:32:19.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5028 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7333 2022-11-22 01:50:04.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py
--rw-r--r--   0 kumagai    (501) staff       (20)      873 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2702 2021-06-04 02:28:26.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2164 2021-08-06 10:10:20.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2385 2021-03-05 09:52:57.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1619 2021-04-12 08:07:10.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2178 2021-04-29 04:12:46.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1429 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1557 2022-05-20 02:54:43.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_poscars_from_query.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1538 2023-03-26 01:11:16.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_unitcell.py
--rw-r--r--   0 kumagai    (501) staff       (20)      216 2021-04-23 05:16:53.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/unitcell.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.005209 pydefect-0.7.1/pydefect/tests/cli/vasp/vasp_files/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.123025 pydefect-0.7.1/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/
--rw-r--r--   0 kumagai    (501) staff       (20)       18 2020-05-31 08:54:40.000000 pydefect-0.7.1/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/pydefect.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)    14382 2023-05-10 00:54:37.000000 pydefect-0.7.1/pydefect/tests/conftest.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.128009 pydefect-0.7.1/pydefect/tests/corrections/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-06-14 07:43:24.000000 pydefect-0.7.1/pydefect/tests/corrections/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1723 2021-04-26 01:56:50.000000 pydefect-0.7.1/pydefect/tests/corrections/test_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)      963 2020-06-05 00:53:04.000000 pydefect-0.7.1/pydefect/tests/corrections/test_efnv_performance.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3613 2021-03-02 02:40:28.000000 pydefect-0.7.1/pydefect/tests/corrections/test_ewald.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2549 2020-11-25 07:07:18.000000 pydefect-0.7.1/pydefect/tests/corrections/test_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2395 2020-11-25 07:22:27.000000 pydefect-0.7.1/pydefect/tests/corrections/test_site_potential_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.128445 pydefect-0.7.1/pydefect/tests/helpers/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.1/pydefect/tests/helpers/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.138244 pydefect-0.7.1/pydefect/tests/input_maker/
--rw-r--r--   0 kumagai    (501) staff       (20)      347 2020-08-05 23:35:58.000000 pydefect-0.7.1/pydefect/tests/input_maker/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:46:18.000000 pydefect-0.7.1/pydefect/tests/input_maker/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2704 2021-04-28 11:25:22.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_append_interstitial.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1923 2023-03-13 01:10:15.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_complex_defect_entries_make.py
--rw-r--r--   0 kumagai    (501) staff       (20)      810 2023-03-13 00:52:36.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_complex_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1230 2022-09-30 06:02:25.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5834 2021-08-06 10:14:07.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entries_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4367 2022-09-30 06:12:21.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entry.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1551 2022-07-01 01:20:10.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2139 2020-12-23 03:22:55.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4174 2021-08-06 10:11:01.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2368 2023-01-28 01:19:23.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_manual_supercell_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3571 2021-03-05 09:52:57.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_supercell.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4443 2023-01-27 05:27:59.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5393 2023-05-19 23:41:13.000000 pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_maker.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.007077 pydefect-0.7.1/pydefect/tests/test_data_files/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.138808 pydefect-0.7.1/pydefect/tests/test_data_files/Na3AgO2/
--rw-r--r--   0 kumagai    (501) staff       (20)     3145 2023-01-31 23:38:38.000000 pydefect-0.7.1/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.151776 pydefect-0.7.1/pydefect/util/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 03:04:22.000000 pydefect-0.7.1/pydefect/util/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      245 2021-04-06 09:47:19.000000 pydefect-0.7.1/pydefect/util/coords.py
--rw-r--r--   0 kumagai    (501) staff       (20)      287 2020-05-26 12:22:43.000000 pydefect-0.7.1/pydefect/util/error_classes.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2333 2023-01-04 05:27:12.000000 pydefect-0.7.1/pydefect/util/mp_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3052 2022-11-15 07:39:58.000000 pydefect-0.7.1/pydefect/util/prepare_names.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2727 2021-04-26 23:23:36.000000 pydefect-0.7.1/pydefect/util/structure_tools.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.993460 pydefect-0.7.1/pydefect-0.7.0/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.996014 pydefect-0.7.1/pydefect-0.7.0/pydefect/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.993732 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.993945 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.011265 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.012364 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.013419 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/
--rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.014378 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/N2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.015440 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/
--rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.016562 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/
--rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.017619 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/O2/prior_info.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/cli/vasp/molecules/molecule_data.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.019166 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/
--rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/electronegativity.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/oxidation_state.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/database/rcore.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:14.996213 pydefect-0.7.1/pydefect-0.7.0/pydefect/tests/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.019690 pydefect-0.7.1/pydefect-0.7.0/pydefect/tests/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.7.1/pydefect-0.7.0/pydefect/tests/analyzer/POSCAR
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-20 00:06:15.022575 pydefect-0.7.1/pydefect.egg-info/
--rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     9663 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/SOURCES.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/dependency_links.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      256 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/entry_points.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      164 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/requires.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        9 2023-05-20 00:06:14.000000 pydefect-0.7.1/pydefect.egg-info/top_level.txt
--rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-05-20 00:06:15.152846 pydefect-0.7.1/setup.cfg
--rw-r--r--   0 kumagai    (501) staff       (20)     1335 2021-08-06 00:13:51.000000 pydefect-0.7.1/setup.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.638026 pydefect-0.7.2/
+-rw-r--r--   0 kumagai    (501) staff       (20)       54 2021-03-12 02:40:59.000000 pydefect-0.7.2/MANIFEST.in
+-rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-06-29 09:06:44.637539 pydefect-0.7.2/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     4563 2022-08-17 09:42:29.000000 pydefect-0.7.2/README.md
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.097813 pydefect-0.7.2/pydefect/
+-rw-r--r--   0 kumagai    (501) staff       (20)       21 2023-06-29 09:06:05.000000 pydefect-0.7.2/pydefect/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.206318 pydefect-0.7.2/pydefect/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2840 2021-04-02 01:38:50.000000 pydefect-0.7.2/pydefect/analyzer/_defect_charge_distribution.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11690 2023-02-21 04:23:52.000000 pydefect-0.7.2/pydefect/analyzer/band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1334 2021-05-01 01:17:09.000000 pydefect-0.7.2/pydefect/analyzer/calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2426 2021-05-26 07:04:12.000000 pydefect-0.7.2/pydefect/analyzer/calc_summary.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.212375 pydefect-0.7.2/pydefect/analyzer/concentration/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:15.000000 pydefect-0.7.2/pydefect/analyzer/concentration/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5631 2023-02-08 05:36:42.000000 pydefect-0.7.2/pydefect/analyzer/concentration/concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2973 2023-02-01 00:50:27.000000 pydefect-0.7.2/pydefect/analyzer/concentration/degeneracy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      385 2023-01-30 01:10:12.000000 pydefect-0.7.2/pydefect/analyzer/concentration/distribution_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7772 2023-02-08 07:02:02.000000 pydefect-0.7.2/pydefect/analyzer/concentration/make_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2462 2023-03-09 04:26:39.000000 pydefect-0.7.2/pydefect/analyzer/concentration/plot_concentration.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.224266 pydefect-0.7.2/pydefect/analyzer/dash_components/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-21 04:26:43.000000 pydefect-0.7.2/pydefect/analyzer/dash_components/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5094 2021-08-15 04:39:32.000000 pydefect-0.7.2/pydefect/analyzer/dash_components/cpd_energy_dash.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1754 2021-05-27 10:09:51.000000 pydefect-0.7.2/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      929 2021-05-27 09:07:43.000000 pydefect-0.7.2/pydefect/analyzer/dash_components/cpd_plotter_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8866 2021-04-04 05:43:59.000000 pydefect-0.7.2/pydefect/analyzer/dash_components/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6859 2021-04-04 05:43:59.000000 pydefect-0.7.2/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4716 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/analyzer/defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12944 2023-03-12 22:54:57.000000 pydefect-0.7.2/pydefect/analyzer/defect_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9945 2023-01-31 04:11:38.000000 pydefect-0.7.2/pydefect/analyzer/defect_energy_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1280 2022-11-15 04:48:53.000000 pydefect-0.7.2/pydefect/analyzer/defect_energy_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7741 2022-09-30 05:43:38.000000 pydefect-0.7.2/pydefect/analyzer/defect_structure_comparator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6536 2023-01-28 01:55:02.000000 pydefect-0.7.2/pydefect/analyzer/defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10344 2023-05-28 21:48:51.000000 pydefect-0.7.2/pydefect/analyzer/eigenvalue_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2420 2021-08-06 10:11:01.000000 pydefect-0.7.2/pydefect/analyzer/grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7225 2022-11-22 05:43:00.000000 pydefect-0.7.2/pydefect/analyzer/make_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1571 2021-05-26 07:04:53.000000 pydefect-0.7.2/pydefect/analyzer/make_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2270 2021-08-06 10:11:46.000000 pydefect-0.7.2/pydefect/analyzer/make_defect_energy_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1716 2023-02-11 23:51:37.000000 pydefect-0.7.2/pydefect/analyzer/make_defect_energy_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6480 2022-11-19 06:15:43.000000 pydefect-0.7.2/pydefect/analyzer/make_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      787 2022-12-08 07:12:16.000000 pydefect-0.7.2/pydefect/analyzer/pinning_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1575 2021-04-27 05:43:07.000000 pydefect-0.7.2/pydefect/analyzer/refine_defect_structure.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2279 2022-11-16 04:21:58.000000 pydefect-0.7.2/pydefect/analyzer/transition_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2006 2022-11-16 04:21:59.000000 pydefect-0.7.2/pydefect/analyzer/transition_levels_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2128 2023-03-26 01:17:24.000000 pydefect-0.7.2/pydefect/analyzer/unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.229492 pydefect-0.7.2/pydefect/chem_pot_diag/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/chem_pot_diag/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    15678 2023-01-04 05:04:29.000000 pydefect-0.7.2/pydefect/chem_pot_diag/chem_pot_diag.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10577 2022-10-10 09:09:15.000000 pydefect-0.7.2/pydefect/chem_pot_diag/cpd_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.289697 pydefect-0.7.2/pydefect/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    15573 2023-05-25 04:54:17.000000 pydefect-0.7.2/pydefect/cli/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10832 2023-06-28 00:24:41.000000 pydefect-0.7.2/pydefect/cli/main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      289 2022-12-13 08:11:13.000000 pydefect-0.7.2/pydefect/cli/main_print_json.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2248 2023-04-06 01:32:45.000000 pydefect-0.7.2/pydefect/cli/main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10042 2023-03-09 23:27:38.000000 pydefect-0.7.2/pydefect/cli/main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6818 2023-03-09 23:26:07.000000 pydefect-0.7.2/pydefect/cli/main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4923 2021-05-02 06:20:14.000000 pydefect-0.7.2/pydefect/cli/make_defect_vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.367101 pydefect-0.7.2/pydefect/cli/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-26 08:41:03.000000 pydefect-0.7.2/pydefect/cli/vasp/__init__.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     1017 2021-04-29 04:10:12.000000 pydefect-0.7.2/pydefect/cli/vasp/get_defect_charge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9144 2022-11-22 04:59:04.000000 pydefect-0.7.2/pydefect/cli/vasp/main_vasp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6954 2023-03-26 01:11:16.000000 pydefect-0.7.2/pydefect/cli/vasp/main_vasp_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5798 2023-05-28 21:33:53.000000 pydefect-0.7.2/pydefect/cli/vasp/main_vasp_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4348 2023-05-28 21:36:20.000000 pydefect-0.7.2/pydefect/cli/vasp/main_vasp_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4770 2022-11-22 05:00:35.000000 pydefect-0.7.2/pydefect/cli/vasp/make_band_edge_orbital_infos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      690 2021-04-13 03:41:39.000000 pydefect-0.7.2/pydefect/cli/vasp/make_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2221 2021-06-04 02:29:24.000000 pydefect-0.7.2/pydefect/cli/vasp/make_composition_energies_from_mp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2754 2021-05-24 05:42:28.000000 pydefect-0.7.2/pydefect/cli/vasp/make_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3728 2023-03-24 00:21:35.000000 pydefect-0.7.2/pydefect/cli/vasp/make_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2398 2020-11-25 07:07:18.000000 pydefect-0.7.2/pydefect/cli/vasp/make_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    18748 2022-10-24 06:34:05.000000 pydefect-0.7.2/pydefect/cli/vasp/make_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1349 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/cli/vasp/make_perfect_band_edge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2471 2023-01-04 04:53:30.000000 pydefect-0.7.2/pydefect/cli/vasp/make_poscars_from_query.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1156 2021-04-25 05:20:51.000000 pydefect-0.7.2/pydefect/cli/vasp/make_unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.373165 pydefect-0.7.2/pydefect/cli/vasp/molecules/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.374853 pydefect-0.7.2/pydefect/cli/vasp/molecules/H2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/H2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/H2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.376626 pydefect-0.7.2/pydefect/cli/vasp/molecules/H2O/
+-rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/H2O/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.378120 pydefect-0.7.2/pydefect/cli/vasp/molecules/N2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/N2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/N2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.379617 pydefect-0.7.2/pydefect/cli/vasp/molecules/NH3/
+-rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/NH3/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.381532 pydefect-0.7.2/pydefect/cli/vasp/molecules/NO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/NO2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.383396 pydefect-0.7.2/pydefect/cli/vasp/molecules/O2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/O2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/O2/prior_info.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 08:59:11.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/molecule_data.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      417 2020-05-26 08:59:40.000000 pydefect-0.7.2/pydefect/cli/vasp/molecules/molecules.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.398095 pydefect-0.7.2/pydefect/corrections/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/corrections/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      700 2023-06-28 00:22:14.000000 pydefect-0.7.2/pydefect/corrections/abstract_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2042 2023-05-10 06:23:17.000000 pydefect-0.7.2/pydefect/corrections/efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4802 2020-06-06 00:50:29.000000 pydefect-0.7.2/pydefect/corrections/ewald.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2875 2020-11-26 00:07:11.000000 pydefect-0.7.2/pydefect/corrections/gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      306 2023-06-28 00:22:41.000000 pydefect-0.7.2/pydefect/corrections/no_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9656 2023-03-29 07:34:00.000000 pydefect-0.7.2/pydefect/corrections/site_potential_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.402526 pydefect-0.7.2/pydefect/database/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/database/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      808 2021-04-28 23:15:40.000000 pydefect-0.7.2/pydefect/database/database.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.7.2/pydefect/database/electronegativity.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.7.2/pydefect/database/oxidation_state.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.7.2/pydefect/database/rcore.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     2982 2021-06-10 06:38:20.000000 pydefect-0.7.2/pydefect/defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      138 2020-05-13 06:54:40.000000 pydefect-0.7.2/pydefect/error.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.423714 pydefect-0.7.2/pydefect/input_maker/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:45:24.000000 pydefect-0.7.2/pydefect/input_maker/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2252 2022-11-04 06:49:00.000000 pydefect-0.7.2/pydefect/input_maker/append_interstitial.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2011 2023-03-13 01:10:20.000000 pydefect-0.7.2/pydefect/input_maker/complex_defect_entries_make.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1178 2023-03-12 23:38:44.000000 pydefect-0.7.2/pydefect/input_maker/complex_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1509 2022-09-30 06:02:01.000000 pydefect-0.7.2/pydefect/input_maker/defect.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5794 2022-09-30 06:04:45.000000 pydefect-0.7.2/pydefect/input_maker/defect_entries_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4655 2022-09-30 06:27:37.000000 pydefect-0.7.2/pydefect/input_maker/defect_entry.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1464 2022-07-01 01:20:02.000000 pydefect-0.7.2/pydefect/input_maker/defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3918 2020-11-23 04:55:46.000000 pydefect-0.7.2/pydefect/input_maker/defect_set_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2305 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/input_maker/local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3149 2023-01-28 01:22:10.000000 pydefect-0.7.2/pydefect/input_maker/manual_supercell_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3938 2023-01-28 00:19:05.000000 pydefect-0.7.2/pydefect/input_maker/supercell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4242 2023-01-28 01:11:46.000000 pydefect-0.7.2/pydefect/input_maker/supercell_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4727 2023-05-18 07:33:28.000000 pydefect-0.7.2/pydefect/input_maker/supercell_maker.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.425281 pydefect-0.7.2/pydefect/tests/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.2/pydefect/tests/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.480762 pydefect-0.7.2/pydefect/tests/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.7.2/pydefect/tests/analyzer/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-03 11:12:30.000000 pydefect-0.7.2/pydefect/tests/analyzer/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.487010 pydefect-0.7.2/pydefect/tests/analyzer/concentration/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:35.000000 pydefect-0.7.2/pydefect/tests/analyzer/concentration/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3177 2023-02-02 23:17:57.000000 pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1723 2023-02-01 00:50:07.000000 pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_degeneracy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      469 2023-01-30 01:09:25.000000 pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_distribution_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3239 2023-03-05 02:07:50.000000 pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_make_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      975 2023-02-08 06:50:25.000000 pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_plot_concentration.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.085518 pydefect-0.7.2/pydefect/tests/analyzer/dash_components/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.086185 pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.487973 pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/
+-rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.489944 pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/
+-rw-r--r--   0 kumagai    (501) staff       (20)     7233 2020-06-26 09:34:37.000000 pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)     7450 2022-09-30 03:57:34.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1022 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2402 2021-05-26 07:04:12.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2915 2021-05-03 01:56:28.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8302 2023-03-05 02:36:13.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_defect_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2466 2022-11-15 07:29:49.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_defect_energy_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1540 2022-11-15 04:49:34.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_defect_energy_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7391 2022-09-30 04:57:30.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_defect_structure_comparator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4373 2023-01-29 23:13:01.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2688 2023-05-28 21:47:22.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_eigenvalue_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2648 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7215 2022-11-22 05:40:58.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_make_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1786 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_make_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2067 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_make_defect_energy_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1609 2021-05-01 06:02:47.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_make_defect_energy_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1665 2022-09-30 05:50:49.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_make_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1465 2022-12-08 07:12:16.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_pinning_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4262 2022-05-20 02:54:43.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_refine_defect_structure.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1796 2022-11-16 04:14:17.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_transition_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1539 2022-11-16 04:16:01.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_transition_levels_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2014 2023-05-10 06:40:55.000000 pydefect-0.7.2/pydefect/tests/analyzer/test_unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.514328 pydefect-0.7.2/pydefect/tests/chem_pot_diag/
+-rw-r--r--   0 kumagai    (501) staff       (20)      169 2020-11-30 07:08:52.000000 pydefect-0.7.2/pydefect/tests/chem_pot_diag/cpd.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.523948 pydefect-0.7.2/pydefect/tests/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/tests/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10308 2023-01-28 00:50:06.000000 pydefect-0.7.2/pydefect/tests/cli/test_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11140 2023-03-05 02:10:01.000000 pydefect-0.7.2/pydefect/tests/cli/test_main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1980 2022-10-10 09:24:54.000000 pydefect-0.7.2/pydefect/tests/cli/test_main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4986 2023-03-05 02:12:51.000000 pydefect-0.7.2/pydefect/tests/cli/test_main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5290 2023-03-09 23:26:49.000000 pydefect-0.7.2/pydefect/tests/cli/test_main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3011 2021-05-15 12:24:21.000000 pydefect-0.7.2/pydefect/tests/cli/test_make_defect_vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.570182 pydefect-0.7.2/pydefect/tests/cli/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/__init__.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     1671 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_get_defect_charge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4907 2022-11-22 04:59:59.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10280 2023-05-10 06:37:49.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2779 2023-05-28 21:34:46.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5041 2023-05-28 21:34:15.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7333 2022-11-22 01:50:04.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      873 2023-03-26 01:11:16.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2702 2021-06-04 02:28:26.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2164 2021-08-06 10:10:20.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2385 2021-03-05 09:52:57.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1619 2021-04-12 08:07:10.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2178 2021-04-29 04:12:46.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1429 2023-03-26 01:11:16.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1557 2022-05-20 02:54:43.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_poscars_from_query.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1538 2023-03-26 01:11:16.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_unitcell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      216 2021-04-23 05:16:53.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/unitcell.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.088536 pydefect-0.7.2/pydefect/tests/cli/vasp/vasp_files/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.571351 pydefect-0.7.2/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/
+-rw-r--r--   0 kumagai    (501) staff       (20)       18 2020-05-31 08:54:40.000000 pydefect-0.7.2/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/pydefect.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)    14382 2023-05-10 00:54:37.000000 pydefect-0.7.2/pydefect/tests/conftest.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.579975 pydefect-0.7.2/pydefect/tests/corrections/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-06-14 07:43:24.000000 pydefect-0.7.2/pydefect/tests/corrections/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1723 2021-04-26 01:56:50.000000 pydefect-0.7.2/pydefect/tests/corrections/test_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      963 2020-06-05 00:53:04.000000 pydefect-0.7.2/pydefect/tests/corrections/test_efnv_performance.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3613 2021-03-02 02:40:28.000000 pydefect-0.7.2/pydefect/tests/corrections/test_ewald.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2549 2020-11-25 07:07:18.000000 pydefect-0.7.2/pydefect/tests/corrections/test_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2395 2020-11-25 07:22:27.000000 pydefect-0.7.2/pydefect/tests/corrections/test_site_potential_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.581129 pydefect-0.7.2/pydefect/tests/helpers/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.7.2/pydefect/tests/helpers/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.597381 pydefect-0.7.2/pydefect/tests/input_maker/
+-rw-r--r--   0 kumagai    (501) staff       (20)      347 2020-08-05 23:35:58.000000 pydefect-0.7.2/pydefect/tests/input_maker/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:46:18.000000 pydefect-0.7.2/pydefect/tests/input_maker/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2704 2021-04-28 11:25:22.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_append_interstitial.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1923 2023-03-13 01:10:15.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_complex_defect_entries_make.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      810 2023-03-13 00:52:36.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_complex_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1230 2022-09-30 06:02:25.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_defect.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5834 2021-08-06 10:14:07.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_defect_entries_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4367 2022-09-30 06:12:21.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_defect_entry.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1551 2022-07-01 01:20:10.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2139 2020-12-23 03:22:55.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_defect_set_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4174 2021-08-06 10:11:01.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2368 2023-01-28 01:19:23.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_manual_supercell_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3571 2021-03-05 09:52:57.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_supercell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4443 2023-01-27 05:27:59.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_supercell_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5393 2023-05-19 23:41:13.000000 pydefect-0.7.2/pydefect/tests/input_maker/test_supercell_maker.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.091026 pydefect-0.7.2/pydefect/tests/test_data_files/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.598559 pydefect-0.7.2/pydefect/tests/test_data_files/Na3AgO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3145 2023-01-31 23:38:38.000000 pydefect-0.7.2/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.636184 pydefect-0.7.2/pydefect/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 03:04:22.000000 pydefect-0.7.2/pydefect/util/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      245 2021-04-06 09:47:19.000000 pydefect-0.7.2/pydefect/util/coords.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      287 2020-05-26 12:22:43.000000 pydefect-0.7.2/pydefect/util/error_classes.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2333 2023-01-04 05:27:12.000000 pydefect-0.7.2/pydefect/util/mp_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3052 2022-11-15 07:39:58.000000 pydefect-0.7.2/pydefect/util/prepare_names.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2727 2021-04-26 23:23:36.000000 pydefect-0.7.2/pydefect/util/structure_tools.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-06-29 09:06:44.102460 pydefect-0.7.2/pydefect.egg-info/
+-rw-r--r--   0 kumagai    (501) staff       (20)      397 2023-06-29 09:06:43.000000 pydefect-0.7.2/pydefect.egg-info/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     8743 2023-06-29 09:06:43.000000 pydefect-0.7.2/pydefect.egg-info/SOURCES.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-06-29 09:06:43.000000 pydefect-0.7.2/pydefect.egg-info/dependency_links.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      256 2023-06-29 09:06:43.000000 pydefect-0.7.2/pydefect.egg-info/entry_points.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      164 2023-06-29 09:06:43.000000 pydefect-0.7.2/pydefect.egg-info/requires.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        9 2023-06-29 09:06:43.000000 pydefect-0.7.2/pydefect.egg-info/top_level.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-06-29 09:06:44.638210 pydefect-0.7.2/setup.cfg
+-rw-r--r--   0 kumagai    (501) staff       (20)     1335 2021-08-06 00:13:51.000000 pydefect-0.7.2/setup.py
```

### Comparing `pydefect-0.7.1/README.md` & `pydefect-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/_defect_charge_distribution.py` & `pydefect-0.7.2/pydefect/analyzer/_defect_charge_distribution.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/band_edge_states.py` & `pydefect-0.7.2/pydefect/analyzer/band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/calc_results.py` & `pydefect-0.7.2/pydefect/analyzer/calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/calc_summary.py` & `pydefect-0.7.2/pydefect/analyzer/calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/concentration/concentration.py` & `pydefect-0.7.2/pydefect/analyzer/concentration/concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/concentration/degeneracy.py` & `pydefect-0.7.2/pydefect/analyzer/concentration/degeneracy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/concentration/make_concentration.py` & `pydefect-0.7.2/pydefect/analyzer/concentration/make_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/concentration/plot_concentration.py` & `pydefect-0.7.2/pydefect/analyzer/concentration/plot_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash.py` & `pydefect-0.7.2/pydefect/analyzer/dash_components/cpd_energy_dash.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py` & `pydefect-0.7.2/pydefect/analyzer/dash_components/cpd_energy_dash_demo.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/dash_components/cpd_plotter_main.py` & `pydefect-0.7.2/pydefect/analyzer/dash_components/cpd_plotter_main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/dash_components/main.py` & `pydefect-0.7.2/pydefect/analyzer/dash_components/main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py` & `pydefect-0.7.2/pydefect/analyzer/dash_components/scenes_from_volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/defect_charge_info.py` & `pydefect-0.7.2/pydefect/analyzer/defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/defect_energy.py` & `pydefect-0.7.2/pydefect/analyzer/defect_energy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/defect_energy_plotter.py` & `pydefect-0.7.2/pydefect/analyzer/defect_energy_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/defect_energy_util.py` & `pydefect-0.7.2/pydefect/analyzer/defect_energy_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/defect_structure_comparator.py` & `pydefect-0.7.2/pydefect/analyzer/defect_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/defect_structure_info.py` & `pydefect-0.7.2/pydefect/analyzer/defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/eigenvalue_plotter.py` & `pydefect-0.7.2/pydefect/analyzer/eigenvalue_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
             self.axs = [ax]
 
     def construct_plot(self):
         self._add_eigenvalues()
         self._add_xticks()
         self._add_band_edges()
         self._set_x_range()
+        self._set_y_range()
         self._set_labels()
         self._set_title()
         self._set_formatter()
         self.plt.tight_layout()
 
     def _add_eigenvalues(self):
         for spin_idx, (eo_by_spin, ax) in \
@@ -221,14 +222,19 @@
             ax.axhline(y=self._supercell_vbm, **self._mpl_defaults.svline)
             ax.axhline(y=self._supercell_cbm, **self._mpl_defaults.svline)
 
     def _set_x_range(self):
         for ax in self.axs:
             ax.set_xlim(-0.5, len(self._kpt_coords) - 0.5)
 
+    def _set_y_range(self):
+        if self._y_range:
+            for ax in self.axs:
+                ax.set_ylim(self._y_range)
+
     def _set_labels(self):
         self.fig.text(0.5, 0, "K-point coords", ha='center',
                       size=self._mpl_defaults.label_font_size)
         self.axs[0].set_ylabel(f"Energy ({self._y_unit})",
                         size=self._mpl_defaults.label_font_size)
 
     def _set_title(self):
```

### Comparing `pydefect-0.7.1/pydefect/analyzer/grids.py` & `pydefect-0.7.2/pydefect/analyzer/grids.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/make_band_edge_states.py` & `pydefect-0.7.2/pydefect/analyzer/make_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/make_calc_summary.py` & `pydefect-0.7.2/pydefect/analyzer/make_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/make_defect_energy_info.py` & `pydefect-0.7.2/pydefect/analyzer/make_defect_energy_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/make_defect_energy_summary.py` & `pydefect-0.7.2/pydefect/analyzer/make_defect_energy_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/make_defect_structure_info.py` & `pydefect-0.7.2/pydefect/analyzer/make_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/pinning_levels.py` & `pydefect-0.7.2/pydefect/analyzer/pinning_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/refine_defect_structure.py` & `pydefect-0.7.2/pydefect/analyzer/refine_defect_structure.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/transition_levels.py` & `pydefect-0.7.2/pydefect/analyzer/transition_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/transition_levels_plotter.py` & `pydefect-0.7.2/pydefect/analyzer/transition_levels_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/analyzer/unitcell.py` & `pydefect-0.7.2/pydefect/analyzer/unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/chem_pot_diag/chem_pot_diag.py` & `pydefect-0.7.2/pydefect/chem_pot_diag/chem_pot_diag.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/chem_pot_diag/cpd_plotter.py` & `pydefect-0.7.2/pydefect/chem_pot_diag/cpd_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/main.py` & `pydefect-0.7.2/pydefect/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,24 @@
         help="Maximum number of atoms")
     parser_supercell.add_argument(
         "--no_symmetry_analysis", dest="analyze_symmetry", action="store_false",
         help="Set if symmetry is not analyzed. If set, sites.yaml file is "
              "required.")
     parser_supercell.add_argument(
         "-s", "--sites_yaml_filename", type=str,
-        help="e.g., sites.yaml")
+        help="""sites.yaml. An example is 
+Mg1:
+  site_index: 0  
+  site_symmetry: Pm-3m
+  wyckoff_letter: b
+O1:
+  site_index: 1 
+  site_symmetry: Pm-3m
+Here site_index is based on the given structure.
+""")
 
     parser_supercell.set_defaults(func=make_supercell)
 
     # -- append_interstitial ------------------------------------------------
     parser_append_interstitial = subparsers.add_parser(
         name="append_interstitial",
         description="Append interstitial information to supercell_info.yaml",
```

### Comparing `pydefect-0.7.1/pydefect/cli/main_functions.py` & `pydefect-0.7.2/pydefect/cli/main_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     MakeDefectStructureInfo
 from pydefect.chem_pot_diag.chem_pot_diag import CompositionEnergies, \
     RelativeEnergies, ChemPotDiagMaker, TargetVertices, change_element_sequence
 from pydefect.chem_pot_diag.cpd_plotter import ChemPotDiag2DMplPlotter, \
     ChemPotDiag3DMplPlotter
 from pydefect.cli.main_tools import sanitize_matrix, parse_dirs
 from pydefect.cli.vasp.make_efnv_correction import make_efnv_correction
+from pydefect.corrections.no_correction import NoCorrection
 from pydefect.corrections.site_potential_plotter import SitePotentialMplPlotter
 from pydefect.input_maker.append_interstitial import append_interstitial
 from pydefect.input_maker.defect_set_maker import DefectSetMaker
 from pydefect.input_maker.manual_supercell_maker import ManualSupercellMaker, \
     make_sites_from_yaml_file
 from pydefect.input_maker.supercell_maker import SupercellMaker
 from pymatgen.analysis.phase_diagram import PDPlotter
@@ -222,15 +223,21 @@
 
 
 def make_defect_energy_infos_main_func(args):
     file_name = "defect_energy_info.yaml"
     def _inner(_dir: Path):
         calc_results = get_calc_results(_dir, args.check_calc_results)
         defect_entry = loadfn(_dir / "defect_entry.json")
-        correction = loadfn(_dir / "correction.json")
+        try:
+            correction = loadfn(_dir / "correction.json")
+        except FileNotFoundError:
+            logger.warning(
+                "Since correction.json file does not exist, no correction is "
+                "applied.")
+            correction = NoCorrection()
         try:
             band_edge_states = loadfn(_dir / "band_edge_states.json")
         except FileNotFoundError:
             band_edge_states = None
         defect_energy_info = make_defect_energy_info(
             defect_entry=defect_entry,
             calc_results=calc_results,
```

### Comparing `pydefect-0.7.1/pydefect/cli/main_tools.py` & `pydefect-0.7.2/pydefect/cli/main_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/main_util.py` & `pydefect-0.7.2/pydefect/cli/main_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/main_util_functions.py` & `pydefect-0.7.2/pydefect/cli/main_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/make_defect_vesta_file.py` & `pydefect-0.7.2/pydefect/cli/make_defect_vesta_file.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/get_defect_charge_state.py` & `pydefect-0.7.2/pydefect/cli/vasp/get_defect_charge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/main_vasp.py` & `pydefect-0.7.2/pydefect/cli/vasp/main_vasp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/main_vasp_functions.py` & `pydefect-0.7.2/pydefect/cli/vasp/main_vasp_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util.py` & `pydefect-0.7.2/pydefect/cli/vasp/main_vasp_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         name="parchg_dir",
         description="Make parchg directory containing a set of VASP files "
                     "required for generating PARCHG files.",
         parents=[dir_parser],
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         aliases=['pd'])
 
+    parser_make_parchg_dir.add_argument(
+        "-i", "--ibands", type=int, nargs="+",
+        help="Band indices to be drawn, which start from 1.")
     parser_make_parchg_dir.set_defaults(func=make_parchg_dir)
 
     # -- make refine defect poscar ---------------------------------------------
     parser_make_refine_defect_poscar = subparsers.add_parser(
         name="refine_defect_poscar",
         description="Refine defect structure POSCAR.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
```

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/main_vasp_util_functions.py` & `pydefect-0.7.2/pydefect/cli/vasp/main_vasp_util_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,19 @@
     except FileNotFoundError:
         logger.info("Need to create calc_results.json beforehand.")
         raise
     calc_results.show_convergence_warning()
 
     # Increment index by 1 as VASP band index begins from 1.
     incar = ViseIncar.from_file("INCAR")
-    band_edge_states = loadfn("band_edge_states.json")
-    iband = [i + 1 for i in band_edge_states.band_indices_from_vbm_to_cbm]
+    if args.ibands:
+        iband = args.ibands
+    else:
+        band_edge_states = loadfn("band_edge_states.json")
+        iband = [i + 1 for i in band_edge_states.band_indices_from_vbm_to_cbm]
     incar.update({"LPARD": True, "LSEPB": True, "KPAR": 1, "IBAND": iband})
 
     parchg = Path("parchg")
     parchg.mkdir()
     os.chdir("parchg")
     incar.write_file("INCAR")
     FileLink(Path("../WAVECAR")).transfer(Path.cwd())
```

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_band_edge_orbital_infos.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_band_edge_orbital_infos.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_calc_results.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_composition_energies_from_mp.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_composition_energies_from_mp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_defect_charge_info.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_efnv_correction.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_gkfo_correction.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_local_extrema.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_perfect_band_edge_state.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_perfect_band_edge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_poscars_from_query.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_poscars_from_query.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/make_unitcell.py` & `pydefect-0.7.2/pydefect/cli/vasp/make_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/molecules/H2O/POSCAR` & `pydefect-0.7.2/pydefect/cli/vasp/molecules/H2O/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/molecules/NH3/POSCAR` & `pydefect-0.7.2/pydefect/cli/vasp/molecules/NH3/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/molecules/NO2/POSCAR` & `pydefect-0.7.2/pydefect/cli/vasp/molecules/NO2/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/cli/vasp/molecules/molecule_data.yaml` & `pydefect-0.7.2/pydefect/cli/vasp/molecules/molecule_data.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/corrections/efnv_correction.py` & `pydefect-0.7.2/pydefect/corrections/efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/corrections/ewald.py` & `pydefect-0.7.2/pydefect/corrections/ewald.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/corrections/gkfo_correction.py` & `pydefect-0.7.2/pydefect/corrections/gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/corrections/site_potential_plotter.py` & `pydefect-0.7.2/pydefect/corrections/site_potential_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/database/database.py` & `pydefect-0.7.2/pydefect/database/database.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/database/electronegativity.yaml` & `pydefect-0.7.2/pydefect/database/electronegativity.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/database/rcore.yaml` & `pydefect-0.7.2/pydefect/database/rcore.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/defaults.py` & `pydefect-0.7.2/pydefect/defaults.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/append_interstitial.py` & `pydefect-0.7.2/pydefect/input_maker/append_interstitial.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/complex_defect_entries_make.py` & `pydefect-0.7.2/pydefect/input_maker/complex_defect_entries_make.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/complex_defect_set.py` & `pydefect-0.7.2/pydefect/input_maker/complex_defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/defect.py` & `pydefect-0.7.2/pydefect/input_maker/defect.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/defect_entries_maker.py` & `pydefect-0.7.2/pydefect/input_maker/defect_entries_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/defect_entry.py` & `pydefect-0.7.2/pydefect/input_maker/defect_entry.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/defect_set.py` & `pydefect-0.7.2/pydefect/input_maker/defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/defect_set_maker.py` & `pydefect-0.7.2/pydefect/input_maker/defect_set_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/local_extrema.py` & `pydefect-0.7.2/pydefect/input_maker/local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/manual_supercell_maker.py` & `pydefect-0.7.2/pydefect/input_maker/manual_supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/supercell.py` & `pydefect-0.7.2/pydefect/input_maker/supercell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/supercell_info.py` & `pydefect-0.7.2/pydefect/input_maker/supercell_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/input_maker/supercell_maker.py` & `pydefect-0.7.2/pydefect/input_maker/supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/POSCAR` & `pydefect-0.7.2/pydefect/tests/analyzer/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_concentration.py` & `pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_degeneracy.py` & `pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_degeneracy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_make_concentration.py` & `pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_make_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/concentration/test_plot_concentration.py` & `pydefect-0.7.2/pydefect/tests/analyzer/concentration/test_plot_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR` & `pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_0/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR` & `pydefect-0.7.2/pydefect/tests/analyzer/dash_components/mgo_defects/Va_O1_2/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_band_edge_states.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_calc_results.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_calc_summary.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_charge_info.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_defect_energy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_plotter.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_defect_energy_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_energy_util.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_defect_energy_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_comparator.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_defect_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_defect_structure_info.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_eigenvalue_plotter.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_eigenvalue_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         orbital_infos=[orb],
         kpt_coords=[(0.0, 0.0, 0.0), (0.25, 0.0, 0.0)],
         kpt_weights=[0.5, 0.5],
         lowest_band_index=10,
         fermi_level=0.5)
     plotter = EigenvalueMplPlotter(title="test",
                                    band_edge_orb_infos=be_orbital_info,
-                                   supercell_vbm=0.1, supercell_cbm=0.9)
+                                   supercell_vbm=0.1, supercell_cbm=0.9,
+                                   y_range=[-1, 2])
     plotter.construct_plot()
     plotter.plt.show()
 
 # def test_plot_with_actual_file():
 #     eig = loadfn(Path(__file__).parent / "band_edge_eigenvalues.json")
 #     plotter = EigenvalueMplPlotter(title="test", band_edge_eigenvalues=eig,
 #                                    supercell_vbm=0.5, supercell_cbm=2.6)
```

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_grids.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_grids.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_make_band_edge_states.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_make_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_make_calc_summary.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_make_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_info.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_make_defect_energy_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_energy_summary.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_make_defect_energy_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_make_defect_structure_info.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_make_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_pinning_levels.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_pinning_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_refine_defect_structure.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_refine_defect_structure.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_transition_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_transition_levels_plotter.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_transition_levels_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/analyzer/test_unitcell.py` & `pydefect-0.7.2/pydefect/tests/analyzer/test_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/test_main.py` & `pydefect-0.7.2/pydefect/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/test_main_functions.py` & `pydefect-0.7.2/pydefect/tests/cli/test_main_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/test_main_tools.py` & `pydefect-0.7.2/pydefect/tests/cli/test_main_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/test_main_util.py` & `pydefect-0.7.2/pydefect/tests/cli/test_main_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/test_main_util_functions.py` & `pydefect-0.7.2/pydefect/tests/cli/test_main_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/test_make_defect_vesta_file.py` & `pydefect-0.7.2/pydefect/tests/cli/test_make_defect_vesta_file.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_get_defect_charge_state.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_get_defect_charge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_functions.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,18 @@
         func=parsed_args.func)
     assert parsed_args == expected
     mock_structure.from_file.assert_called_once_with("POSCAR")
 
 
 def test_make_parchg_dir():
     parsed_args = parse_args_main_vasp_util(
-        ["pd", "-d", "Va_O1_0"])
+        ["pd", "-d", "Va_O1_0", "-i", "1"])
     expected = Namespace(
         dir=Path("Va_O1_0"),
+        ibands=[1],
         func=parsed_args.func)
     assert parsed_args == expected
 
 
 def test_refine_defect_poscar(mocker, simple_cubic):
     mock_structure = mocker.patch(
         "pydefect.cli.vasp.main_vasp_util.Structure")
```

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             return band_edge_states
         elif str(key) == "calc_results.json":
             return calc_results
         else:
             raise ValueError
 
     mock_loadfn = mocker.patch(f"{_filepath}.loadfn", side_effect=side_effect)
-    args = Namespace(dir=Path(tmpdir))
+    args = Namespace(dir=Path(tmpdir), ibands=None)
 
     with pytest.raises(FileNotFoundError):
         make_parchg_dir(args)
 
     Path("WAVECAR").write_text("d")
     make_parchg_dir(args)
```

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_calc_results.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_defect_charge_info.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_efnv_correction.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_gkfo_correction.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_local_extrema.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_poscars_from_query.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_poscars_from_query.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/cli/vasp/test_make_unitcell.py` & `pydefect-0.7.2/pydefect/tests/cli/vasp/test_make_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/conftest.py` & `pydefect-0.7.2/pydefect/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/corrections/test_efnv_correction.py` & `pydefect-0.7.2/pydefect/tests/corrections/test_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/corrections/test_efnv_performance.py` & `pydefect-0.7.2/pydefect/tests/corrections/test_efnv_performance.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/corrections/test_ewald.py` & `pydefect-0.7.2/pydefect/tests/corrections/test_ewald.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/corrections/test_gkfo_correction.py` & `pydefect-0.7.2/pydefect/tests/corrections/test_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/corrections/test_site_potential_plotter.py` & `pydefect-0.7.2/pydefect/tests/corrections/test_site_potential_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_append_interstitial.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_append_interstitial.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_complex_defect_entries_make.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_complex_defect_entries_make.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_complex_defect_set.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_complex_defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_defect.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_defect.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entries_maker.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_defect_entries_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_entry.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_defect_entry.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_defect_set_maker.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_defect_set_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_local_extrema.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_manual_supercell_maker.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_manual_supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_supercell.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_supercell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_info.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_supercell_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/input_maker/test_supercell_maker.py` & `pydefect-0.7.2/pydefect/tests/input_maker/test_supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml` & `pydefect-0.7.2/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/util/mp_tools.py` & `pydefect-0.7.2/pydefect/util/mp_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/util/prepare_names.py` & `pydefect-0.7.2/pydefect/util/prepare_names.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/pydefect/util/structure_tools.py` & `pydefect-0.7.2/pydefect/util/structure_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.7.1/setup.py` & `pydefect-0.7.2/setup.py`

 * *Files identical despite different names*

