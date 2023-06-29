# Comparing `tmp/FESTIM-0.11.0.tar.gz` & `tmp/FESTIM-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FESTIM-0.11.0.tar", last modified: Tue Jan  3 19:30:34 2023, max compression
+gzip compressed data, was "FESTIM-0.11.1.tar", last modified: Thu Jun 29 18:48:22 2023, max compression
```

## Comparing `FESTIM-0.11.0.tar` & `FESTIM-0.11.1.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.218202 FESTIM-0.11.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.178202 FESTIM-0.11.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.178202 FESTIM-0.11.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.178202 FESTIM-0.11.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.182202 FESTIM-0.11.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.github/workflows/code_formatting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.github/workflows/test_demos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-03 19:30:12.000000 FESTIM-0.11.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-01-03 19:30:12.000000 FESTIM-0.11.0/CITATION.cff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.182202 FESTIM-0.11.0/FESTIM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-01-03 19:30:34.000000 FESTIM-0.11.0/FESTIM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-01-03 19:30:34.000000 FESTIM-0.11.0/FESTIM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 19:30:34.000000 FESTIM-0.11.0/FESTIM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-03 19:30:34.000000 FESTIM-0.11.0/FESTIM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-03 19:30:34.000000 FESTIM-0.11.0/FESTIM.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-01-03 19:30:12.000000 FESTIM-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-01-03 19:30:34.218202 FESTIM-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-01-03 19:30:12.000000 FESTIM-0.11.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.182202 FESTIM-0.11.0/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-01-03 19:30:12.000000 FESTIM-0.11.0/demos/demo_Ogorodnikova.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   600529 2023-01-03 19:30:12.000000 FESTIM-0.11.0/demos/demo_coupled_heat_transfer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   124496 2023-01-03 19:30:12.000000 FESTIM-0.11.0/demos/demo_derived_quantities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34586 2023-01-03 19:30:12.000000 FESTIM-0.11.0/demos/demo_meshes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   164442 2023-01-03 19:30:12.000000 FESTIM-0.11.0/demos/demo_multi_materials.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   234399 2023-01-03 19:30:12.000000 FESTIM-0.11.0/demos/demo_read_xdmf.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.186202 FESTIM-0.11.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.186202 FESTIM-0.11.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.190202 FESTIM-0.11.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.boundary_conditions.dirichlets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.boundary_conditions.fluxes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.boundary_conditions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.concentration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.concentration.traps.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.exports.derived_quantities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.exports.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.materials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.meshing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/api/festim.temperature.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.190202 FESTIM-0.11.0/docs/source/devguide/
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/devguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/publications.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/theory.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.190202 FESTIM-0.11.0/docs/source/userguide/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/beginners_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/boundary_conditions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/export_post_processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/materials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/simulations.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/temperature.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/traps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-03 19:30:12.000000 FESTIM-0.11.0/docs/source/userguide/units.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.194202 FESTIM-0.11.0/festim/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-03 19:30:34.000000 FESTIM-0.11.0/festim/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.194202 FESTIM-0.11.0/festim/boundary_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/boundary_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.194202 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/custom_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/dc_imp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/dirichlet_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/henrys_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/dirichlets/sieverts_bc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.194202 FESTIM-0.11.0/festim/boundary_conditions/fluxes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/fluxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/fluxes/convective_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/fluxes/flux_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/fluxes/flux_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/fluxes/mass_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/boundary_conditions/fluxes/recombination_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.198202 FESTIM-0.11.0/festim/concentration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/theta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.198202 FESTIM-0.11.0/festim/concentration/traps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/traps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/traps/extrinsic_trap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/traps/neutron_induced_trap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/traps/trap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/concentration/traps/traps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.198202 FESTIM-0.11.0/festim/exports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.202202 FESTIM-0.11.0/festim/exports/derived_quantities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/average_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/average_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/derived_quantities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/derived_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/hydrogen_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/maximum_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/maximum_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/minimum_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/minimum_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/surface_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/thermal_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/total_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/derived_quantities/total_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/trap_density_xdmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/txt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/exports/xdmf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/generic_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/h_transport_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/initial_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.202202 FESTIM-0.11.0/festim/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/materials/material.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/materials/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.202202 FESTIM-0.11.0/festim/meshing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/meshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/meshing/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/meshing/mesh_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/meshing/mesh_from_refinements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/meshing/mesh_from_vertices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/meshing/mesh_from_xdmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.202202 FESTIM-0.11.0/festim/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/sources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/sources/source_implantation_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/stepsize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.206202 FESTIM-0.11.0/festim/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/temperature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/temperature/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/temperature/temperature_from_xdmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-01-03 19:30:12.000000 FESTIM-0.11.0/festim/temperature/temperature_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-03 19:30:12.000000 FESTIM-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-03 19:30:34.218202 FESTIM-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-03 19:30:12.000000 FESTIM-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.206202 FESTIM-0.11.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.206202 FESTIM-0.11.0/test/h_transport_problem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/h_transport_problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/h_transport_problem/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/h_transport_problem/test_solving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.206202 FESTIM-0.11.0/test/heat_transfer_problem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/heat_transfer_problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/heat_transfer_problem/test_solving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.206202 FESTIM-0.11.0/test/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/simulation/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/simulation/test_initialise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/simulation/test_meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/simulation/test_postprocessing_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.210203 FESTIM-0.11.0/test/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/test_chemical_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/test_cylindrical_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/test_extrinsic_traps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/test_spherical_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    28502 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/system/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.210203 FESTIM-0.11.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_boundary_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_concentration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.210203 FESTIM-0.11.0/test/unit/test_exports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.214203 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_average_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_average_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_derived_quantities.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_hydrogen_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_maximum_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_maximum_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_minimum_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_minimum_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_surface_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_surface_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_thermal_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_total_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_total_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_volume_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_trap_density_xdmf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_txt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_txt_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_xdmf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_exports/test_xdmf_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_initial_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_stepsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_theta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:34.218202 FESTIM-0.11.0/test/unit/test_traps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_traps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_traps/test_extrinsic_trap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_traps/test_neutron_induced_trap.py
--rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_traps/test_trap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-01-03 19:30:12.000000 FESTIM-0.11.0/test/unit/test_traps/test_traps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.118049 FESTIM-0.11.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.098049 FESTIM-0.11.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.098049 FESTIM-0.11.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.098049 FESTIM-0.11.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.098049 FESTIM-0.11.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.github/workflows/code_formatting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.github/workflows/test_demos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-29 18:48:11.000000 FESTIM-0.11.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-29 18:48:11.000000 FESTIM-0.11.1/CITATION.cff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.102049 FESTIM-0.11.1/FESTIM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-29 18:48:22.000000 FESTIM-0.11.1/FESTIM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-29 18:48:22.000000 FESTIM-0.11.1/FESTIM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:48:22.000000 FESTIM-0.11.1/FESTIM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 18:48:22.000000 FESTIM-0.11.1/FESTIM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 18:48:22.000000 FESTIM-0.11.1/FESTIM.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-29 18:48:11.000000 FESTIM-0.11.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-29 18:48:22.118049 FESTIM-0.11.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-29 18:48:11.000000 FESTIM-0.11.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.102049 FESTIM-0.11.1/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-06-29 18:48:11.000000 FESTIM-0.11.1/demos/demo_Ogorodnikova.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   600529 2023-06-29 18:48:11.000000 FESTIM-0.11.1/demos/demo_coupled_heat_transfer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   124496 2023-06-29 18:48:11.000000 FESTIM-0.11.1/demos/demo_derived_quantities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34586 2023-06-29 18:48:11.000000 FESTIM-0.11.1/demos/demo_meshes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   164442 2023-06-29 18:48:11.000000 FESTIM-0.11.1/demos/demo_multi_materials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   234399 2023-06-29 18:48:11.000000 FESTIM-0.11.1/demos/demo_read_xdmf.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.102049 FESTIM-0.11.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.102049 FESTIM-0.11.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.102049 FESTIM-0.11.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.boundary_conditions.dirichlets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.boundary_conditions.fluxes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.boundary_conditions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.concentration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.concentration.traps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.exports.derived_quantities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.exports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.materials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.meshing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/api/festim.temperature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/docs/source/devguide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/devguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/publications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/theory.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/docs/source/userguide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/beginners_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/boundary_conditions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/export_post_processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/materials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/simulations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/temperature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/traps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 18:48:11.000000 FESTIM-0.11.1/docs/source/userguide/units.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/festim/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 18:48:22.000000 FESTIM-0.11.1/festim/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/festim/boundary_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/boundary_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/custom_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/dc_imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/dirichlet_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/henrys_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/dirichlets/sieverts_bc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/festim/boundary_conditions/fluxes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/fluxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/fluxes/convective_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/fluxes/flux_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/fluxes/flux_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/fluxes/mass_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/boundary_conditions/fluxes/recombination_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.106049 FESTIM-0.11.1/festim/concentration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/concentration/traps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/traps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/traps/extrinsic_trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/traps/neutron_induced_trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/traps/trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/concentration/traps/traps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/exports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/exports/derived_quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/average_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/average_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/derived_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/derived_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/hydrogen_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/maximum_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/maximum_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/minimum_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/minimum_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/surface_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/thermal_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/total_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/derived_quantities/total_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/trap_density_xdmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/txt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/exports/xdmf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/generic_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/h_transport_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/initial_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/materials/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/materials/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/meshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/meshing/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/meshing/mesh_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/meshing/mesh_from_refinements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/meshing/mesh_from_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/meshing/mesh_from_xdmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/sources/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/sources/source_implantation_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/stepsize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.110049 FESTIM-0.11.1/festim/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/temperature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/temperature/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/temperature/temperature_from_xdmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-06-29 18:48:11.000000 FESTIM-0.11.1/festim/temperature/temperature_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-29 18:48:11.000000 FESTIM-0.11.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-29 18:48:22.118049 FESTIM-0.11.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 18:48:11.000000 FESTIM-0.11.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/h_transport_problem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/h_transport_problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/h_transport_problem/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/h_transport_problem/test_solving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/heat_transfer_problem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/heat_transfer_problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/heat_transfer_problem/test_solving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/simulation/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/simulation/test_initialise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/simulation/test_meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/simulation/test_postprocessing_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/test_chemical_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/test_cylindrical_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/test_extrinsic_traps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/test_spherical_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28501 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/system/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_boundary_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_concentration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.114049 FESTIM-0.11.1/test/unit/test_exports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.118049 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_average_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_average_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_derived_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_hydrogen_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_maximum_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_maximum_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_minimum_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_minimum_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_surface_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_surface_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_thermal_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_total_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_total_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_volume_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_trap_density_xdmf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_txt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_txt_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_xdmf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_exports/test_xdmf_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_initial_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_stepsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_theta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:22.118049 FESTIM-0.11.1/test/unit/test_traps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_traps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_traps/test_extrinsic_trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_traps/test_neutron_induced_trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21306 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_traps/test_trap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-29 18:48:11.000000 FESTIM-0.11.1/test/unit/test_traps/test_traps.py
```

### Comparing `FESTIM-0.11.0/.circleci/config.yml` & `FESTIM-0.11.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/.github/pull_request_template.md` & `FESTIM-0.11.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/.github/workflows/python-publish.yml` & `FESTIM-0.11.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/.github/workflows/test_demos.yml` & `FESTIM-0.11.1/.github/workflows/test_demos.yml`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/.gitignore` & `FESTIM-0.11.1/.gitignore`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/.readthedocs.yaml` & `FESTIM-0.11.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/CITATION.cff` & `FESTIM-0.11.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/FESTIM.egg-info/PKG-INFO` & `FESTIM-0.11.1/FESTIM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FESTIM
-Version: 0.11.0
+Version: 0.11.1
 Summary: Finite element simulations of hydrogen transport
 Home-page: https://github.com/RemDelaporteMathurin/FESTIM
 Author: Remi Delaporte-Mathurin
 Author-email: rdelaportemathurin@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/RemDelaporteMathurin/FESTIM
 Project-URL: Tracker, https://github.com/RemDelaporteMathurin/FESTIM/issues
```

### Comparing `FESTIM-0.11.0/FESTIM.egg-info/SOURCES.txt` & `FESTIM-0.11.1/FESTIM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/LICENSE` & `FESTIM-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/PKG-INFO` & `FESTIM-0.11.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FESTIM
-Version: 0.11.0
+Version: 0.11.1
 Summary: Finite element simulations of hydrogen transport
 Home-page: https://github.com/RemDelaporteMathurin/FESTIM
 Author: Remi Delaporte-Mathurin
 Author-email: rdelaportemathurin@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/RemDelaporteMathurin/FESTIM
 Project-URL: Tracker, https://github.com/RemDelaporteMathurin/FESTIM/issues
```

### Comparing `FESTIM-0.11.0/README.md` & `FESTIM-0.11.1/README.md`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/demos/demo_Ogorodnikova.ipynb` & `FESTIM-0.11.1/demos/demo_Ogorodnikova.ipynb`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/demos/demo_coupled_heat_transfer.ipynb` & `FESTIM-0.11.1/demos/demo_coupled_heat_transfer.ipynb`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/demos/demo_derived_quantities.ipynb` & `FESTIM-0.11.1/demos/demo_derived_quantities.ipynb`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/demos/demo_meshes.ipynb` & `FESTIM-0.11.1/demos/demo_meshes.ipynb`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/demos/demo_multi_materials.ipynb` & `FESTIM-0.11.1/demos/demo_multi_materials.ipynb`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/demos/demo_read_xdmf.ipynb` & `FESTIM-0.11.1/demos/demo_read_xdmf.ipynb`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.boundary_conditions.dirichlets.rst` & `FESTIM-0.11.1/docs/source/api/festim.boundary_conditions.dirichlets.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.boundary_conditions.fluxes.rst` & `FESTIM-0.11.1/docs/source/api/festim.boundary_conditions.fluxes.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.boundary_conditions.rst` & `FESTIM-0.11.1/docs/source/api/festim.boundary_conditions.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.concentration.rst` & `FESTIM-0.11.1/docs/source/api/festim.concentration.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.concentration.traps.rst` & `FESTIM-0.11.1/docs/source/api/festim.concentration.traps.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.exports.derived_quantities.rst` & `FESTIM-0.11.1/docs/source/api/festim.exports.derived_quantities.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.exports.rst` & `FESTIM-0.11.1/docs/source/api/festim.exports.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.materials.rst` & `FESTIM-0.11.1/docs/source/api/festim.materials.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.meshing.rst` & `FESTIM-0.11.1/docs/source/api/festim.meshing.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.rst` & `FESTIM-0.11.1/docs/source/api/festim.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.sources.rst` & `FESTIM-0.11.1/docs/source/api/festim.sources.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/api/festim.temperature.rst` & `FESTIM-0.11.1/docs/source/api/festim.temperature.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/conf.py` & `FESTIM-0.11.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/devguide/index.rst` & `FESTIM-0.11.1/docs/source/devguide/index.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/getting_started.rst` & `FESTIM-0.11.1/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/index.rst` & `FESTIM-0.11.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/publications.rst` & `FESTIM-0.11.1/docs/source/publications.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/beginners_guide.rst` & `FESTIM-0.11.1/docs/source/userguide/beginners_guide.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/boundary_conditions.rst` & `FESTIM-0.11.1/docs/source/userguide/boundary_conditions.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/materials.rst` & `FESTIM-0.11.1/docs/source/userguide/materials.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/mesh.rst` & `FESTIM-0.11.1/docs/source/userguide/mesh.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/settings.rst` & `FESTIM-0.11.1/docs/source/userguide/settings.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/temperature.rst` & `FESTIM-0.11.1/docs/source/userguide/temperature.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/docs/source/userguide/traps.rst` & `FESTIM-0.11.1/docs/source/userguide/traps.rst`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/__init__.py` & `FESTIM-0.11.1/festim/__init__.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/boundary_condition.py` & `FESTIM-0.11.1/festim/boundary_conditions/boundary_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
         surfaces (list or int): the surfaces of the BC
         field (int or str): the field the boundary condition is
             applied to. 0 and "solute" stand for the mobile
             concentration, "T" for temperature
     """
 
     def __init__(self, surfaces, field) -> None:
-
         if not isinstance(surfaces, list):
             surfaces = [surfaces]
         self.surfaces = surfaces
 
         if field == "solute":
             self.field = 0
         else:
```

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/dirichlets/custom_dc.py` & `FESTIM-0.11.1/festim/boundary_conditions/dirichlets/custom_dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             function=fun,
             param1=2*festim.x + festim.t
         )
 
     """
 
     def __init__(self, surfaces, function, field=0, **prms) -> None:
-
         super().__init__(surfaces, field=field, value=None)
         self.function = function
         self.prms = prms
         self.convert_prms()
 
     def create_expression(self, T):
         value_BC = BoundaryConditionExpression(
```

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/dirichlets/dc_imp.py` & `FESTIM-0.11.1/festim/boundary_conditions/dirichlets/dc_imp.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/dirichlets/dirichlet_bc.py` & `FESTIM-0.11.1/festim/boundary_conditions/dirichlets/dirichlet_bc.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 
     Args:
         T (fenics.Function): the temperature
         eval_function ([type]): [description]
     """
 
     def __init__(self, T, eval_function, **kwargs):
-
         super().__init__()
 
         self._T = T
         self.eval_function = eval_function
         self.prms = kwargs
 
     def eval(self, value, x):
```

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/dirichlets/henrys_bc.py` & `FESTIM-0.11.1/festim/boundary_conditions/dirichlets/henrys_bc.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/dirichlets/sieverts_bc.py` & `FESTIM-0.11.1/festim/boundary_conditions/dirichlets/sieverts_bc.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/fluxes/convective_flux.py` & `FESTIM-0.11.1/festim/boundary_conditions/fluxes/convective_flux.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/fluxes/flux_bc.py` & `FESTIM-0.11.1/festim/boundary_conditions/fluxes/flux_bc.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/fluxes/flux_custom.py` & `FESTIM-0.11.1/festim/boundary_conditions/fluxes/flux_custom.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/fluxes/mass_flux.py` & `FESTIM-0.11.1/festim/boundary_conditions/fluxes/mass_flux.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/boundary_conditions/fluxes/recombination_flux.py` & `FESTIM-0.11.1/festim/boundary_conditions/fluxes/recombination_flux.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/concentration/concentration.py` & `FESTIM-0.11.1/festim/concentration/concentration.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/concentration/mobile.py` & `FESTIM-0.11.1/festim/concentration/mobile.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/concentration/theta.py` & `FESTIM-0.11.1/festim/concentration/theta.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/concentration/traps/extrinsic_trap.py` & `FESTIM-0.11.1/festim/concentration/traps/extrinsic_trap.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         eta_a,
         eta_b,
         f_a,
         f_b,
         id=None,
         **kwargs,
     ):
-
         super().__init__(
             k_0,
             E_k,
             p_0,
             E_p,
             materials,
             phi_0=phi_0,
```

### Comparing `FESTIM-0.11.0/festim/concentration/traps/neutron_induced_trap.py` & `FESTIM-0.11.1/festim/concentration/traps/neutron_induced_trap.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/concentration/traps/trap.py` & `FESTIM-0.11.1/festim/concentration/traps/trap.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
         This will act as a singular trap but with seperate properties for
         respective materials. Parameters k_0, E_k, p_0, E_p, materials and
         density MUST have the same length for this method to be valid.
     """
 
     def __init__(self, k_0, E_k, p_0, E_p, materials, density, id=None):
-
         super().__init__()
         self.id = id
         self.k_0 = k_0
         self.E_k = E_k
         self.p_0 = p_0
         self.E_p = E_p
         self.materials = materials
```

### Comparing `FESTIM-0.11.0/festim/concentration/traps/traps.py` & `FESTIM-0.11.1/festim/concentration/traps/traps.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/derived_quantities.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/derived_quantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     def __init__(
         self,
         derived_quantities: list = None,
         filename: str = None,
         nb_iterations_between_compute: int = 1,
         nb_iterations_between_exports: int = None,
     ) -> None:
-
         self.filename = filename
         self.nb_iterations_between_compute = nb_iterations_between_compute
         self.nb_iterations_between_exports = nb_iterations_between_exports
 
         self.derived_quantities = derived_quantities
         if derived_quantities is None:
             self.derived_quantities = []
@@ -78,15 +77,14 @@
         for quantity in self.derived_quantities:
             quantity.D = materials.D
             quantity.S = materials.S
             quantity.thermal_cond = materials.thermal_cond
             quantity.H = materials.H
 
     def compute(self, t):
-
         # TODO need to support for soret flag in surface flux
         row = [t]
         for quantity in self.derived_quantities:
             if isinstance(quantity, (MaximumVolume, MinimumVolume)):
                 value = quantity.compute(self.volume_markers)
             else:
                 value = quantity.compute()
@@ -178,15 +176,14 @@
         if instances is not None and not isinstance(instances, list):
             instances = [instances]
 
         quantities = []
 
         # iterate through derived_quantities
         for quantity in self.derived_quantities:
-
             # initialise flags to False
             match_surface, match_volume, match_field, match_instance = (
                 False,
                 False,
                 False,
                 False,
             )
```

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/derived_quantity.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/derived_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 class DerivedQuantity(Export):
     """
     Args:
         field (str, int):  the field ("solute", 0, 1, "T", "retention")
     """
 
     def __init__(self, field) -> None:
-
         super().__init__(field=field)
         self.dx = None
         self.ds = None
         self.n = None
         self.D = None
         self.S = None
         self.thermal_cond = None
```

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/maximum_surface.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/maximum_surface.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Args:
         field (str): the field from which the maximum
             is computed (ex: "solute", "retention", "T"...)
         surface (int): the surface id where the maximum is computed
     """
 
     def __init__(self, field, surface) -> None:
-
         super().__init__(field)
         self.surface = surface
         self.title = "Maximum {} surface {}".format(self.field, self.surface)
 
     def compute(self, surface_markers):
         """Maximum of f over subdomains facets marked with self.surface"""
         V = self.function.function_space()
```

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/maximum_volume.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/maximum_volume.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/minimum_surface.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/minimum_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Args:
         field (str): the field from which the minimum
             is computed (ex: "solute", "retention", "T"...)
         surface (int): the surface id where the minimum is computed
     """
 
     def __init__(self, field, surface) -> None:
-
         super().__init__(field)
         self.surface = surface
         self.title = "Minimum {} surface {}".format(self.field, self.surface)
 
     def compute(self, surface_markers):
         """Minimum of f over subdomains facets marked with self.surface"""
         V = self.function.function_space()
```

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/minimum_volume.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/minimum_volume.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/exports/derived_quantities/surface_flux.py` & `FESTIM-0.11.1/festim/exports/derived_quantities/surface_flux.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/exports/exports.py` & `FESTIM-0.11.1/festim/exports/exports.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         self.V_DG1 = None
         self.final_time = None
         self.nb_iterations = 0
 
     def write(self, label_to_function, dt):
         for export in self.exports:
             if isinstance(export, festim.DerivedQuantities):
-
                 # compute derived quantities
                 if export.is_compute(self.nb_iterations):
                     # check if function has to be projected
                     for quantity in export.derived_quantities:
                         if isinstance(
                             quantity, (festim.MaximumVolume, festim.MinimumVolume)
                         ):
```

### Comparing `FESTIM-0.11.0/festim/exports/trap_density_xdmf.py` & `FESTIM-0.11.1/festim/exports/trap_density_xdmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     """
     Args:
         trap (festim.Trap): the trap to export density
         kwargs (): See XDMFExport
     """
 
     def __init__(self, trap, **kwargs) -> None:
-
         super().__init__(
             field="1", **kwargs
         )  # field is "1" just to make the code not crash
 
         self.trap = trap
 
     def write(self, t):
```

### Comparing `FESTIM-0.11.0/festim/exports/txt_export.py` & `FESTIM-0.11.1/festim/exports/txt_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         times (list): times of export. The stepsize will be modified to
             ensure these timesteps are hit.
         label (str): label of the field. Will also be the filename.
         folder (str): the export folder
     """
 
     def __init__(self, field, times, label, folder) -> None:
-
         super().__init__(field=field)
         self.times = sorted(times)
         self.label = label
         self.folder = folder
 
     def is_it_time_to_export(self, current_time):
         for time in self.times:
@@ -36,15 +35,14 @@
     def when_is_next_time(self, current_time):
         for time in self.times:
             if current_time < time:
                 return time
         return None
 
     def write(self, current_time, dt):
-
         # create a DG1 functionspace
         V_DG1 = f.FunctionSpace(self.function.function_space().mesh(), "DG", 1)
 
         solution = f.project(self.function, V_DG1)
         if self.is_it_time_to_export(current_time):
             filename = "{}/{}_{}s.txt".format(self.folder, self.label, current_time)
             busy = True
```

### Comparing `FESTIM-0.11.0/festim/exports/xdmf_export.py` & `FESTIM-0.11.1/festim/exports/xdmf_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             fenics.XDMFFile.write. Defaults to True.
         folder (str, optional): path of the export folder. Defaults to None.
     """
 
     def __init__(
         self, field, label=None, filename=None, mode=1, checkpoint=True, folder=None
     ) -> None:
-
         super().__init__(field=field)
         self.label = label
         self.folder = folder
         self.filename = filename
 
         self.files = None
         self.define_xdmf_file()
@@ -119,15 +118,14 @@
 
         Args:
             t (float): current time
         """
         self.function.rename(self.label, "label")
 
         if self.checkpoint:
-
             # warn users if checkpoint is True and 1D
             dimension = self.function.function_space().mesh().topology().dim()
             if dimension == 1:
                 msg = "in 1D, checkpoint needs to be set to False to "
                 msg += "visualise the XDMF file in Paraview (see issue "
                 msg += "https://github.com/RemDelaporteMathurin/festim/issues/134)"
                 warnings.warn(msg)
```

### Comparing `FESTIM-0.11.0/festim/generic_simulation.py` & `FESTIM-0.11.1/festim/generic_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import festim
 from festim.h_transport_problem import HTransportProblem
 from fenics import *
+import numpy as np
 
 
 class Simulation:
     """
     Main festim class representing a festim model
 
     Args:
@@ -81,15 +82,14 @@
         dt=None,
         settings=None,
         temperature=None,
         initial_conditions=[],
         exports=None,
         log_level=40,
     ):
-
         self.log_level = log_level
 
         self.settings = settings
         self.dt = dt
 
         self.traps = traps
         self.materials = materials
@@ -328,26 +328,28 @@
         self.display_time()
 
         # Post processing
         self.run_post_processing()
 
         # avoid t > final_time
         next_time = self.t + float(self.dt.value)
-        if next_time > self.settings.final_time and self.t != self.settings.final_time:
+        if next_time > self.settings.final_time and not np.isclose(
+            self.t, self.settings.final_time
+        ):
             self.dt.value.assign(self.settings.final_time - self.t)
 
     def display_time(self):
         """Displays the current time"""
         simulation_percentage = round(self.t / self.settings.final_time * 100, 2)
         simulation_time = round(self.t, 1)
         elapsed_time = round(self.timer.elapsed()[0], 1)
         msg = "{:.1f} %        ".format(simulation_percentage)
         msg += "{:.1e} s".format(simulation_time)
         msg += "    Ellapsed time so far: {:.1f} s".format(elapsed_time)
-        if self.t != self.settings.final_time and self.log_level == 40:
+        if not np.isclose(self.t, self.settings.final_time) and self.log_level == 40:
             print(msg, end="\r")
         else:
             print(msg)
 
     def run_post_processing(self):
         """Create post processing functions and compute/write the exports"""
         self.update_post_processing_solutions()
```

### Comparing `FESTIM-0.11.0/festim/h_transport_problem.py` & `FESTIM-0.11.1/festim/h_transport_problem.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/helpers.py` & `FESTIM-0.11.1/festim/helpers.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/initial_condition.py` & `FESTIM-0.11.1/festim/initial_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         ValueError: if XDMF and label is None
         ValueError: if XDMF and time_step is None
     """
 
     def __init__(
         self, field=0, value=0.0, component=None, label=None, time_step=None
     ) -> None:
-
         # TODO make an inherited class InitialConditionXDMF
         self.field = field
         self.value = value
         if component is not None:
             self.field = component
             warnings.warn("components key will be deprecated", DeprecationWarning)
         self.label = label
```

### Comparing `FESTIM-0.11.0/festim/materials/material.py` & `FESTIM-0.11.1/festim/materials/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         heat_capacity=None,
         rho=None,
         borders=None,
         H=None,
         solubility_law="sievert",
         name=None,
     ) -> None:
-
         self.id = id
         self.name = name
         self.D_0 = D_0
         self.E_D = E_D
         self.S_0 = S_0
         self.E_S = E_S
         self.thermal_cond = thermal_cond
```

### Comparing `FESTIM-0.11.0/festim/materials/materials.py` & `FESTIM-0.11.1/festim/materials/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     """
     Args:
         materials (list, optional): contains festim.Material objects.
             Defaults to [].
     """
 
     def __init__(self, materials=[]):
-
         self.materials = materials
         self.D = None
         self.S = None
         self.thermal_cond = None
         self.heat_capacity = None
         self.density = None
         self.H = None
```

### Comparing `FESTIM-0.11.0/festim/meshing/mesh.py` & `FESTIM-0.11.1/festim/meshing/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         dx (fenics.Measure):
         ds (fenics.Measure):
     """
 
     def __init__(
         self, mesh=None, volume_markers=None, surface_markers=None, type="cartesian"
     ) -> None:
-
         self.mesh = mesh
         self.volume_markers = volume_markers
         self.surface_markers = surface_markers
         self.type = type
 
         self.dx = None
         self.ds = None
```

### Comparing `FESTIM-0.11.0/festim/meshing/mesh_1d.py` & `FESTIM-0.11.1/festim/meshing/mesh_1d.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/meshing/mesh_from_refinements.py` & `FESTIM-0.11.1/festim/meshing/mesh_from_refinements.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/meshing/mesh_from_vertices.py` & `FESTIM-0.11.1/festim/meshing/mesh_from_vertices.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/meshing/mesh_from_xdmf.py` & `FESTIM-0.11.1/festim/meshing/mesh_from_xdmf.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/settings.py` & `FESTIM-0.11.1/festim/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         final_time=None,
         chemical_pot=False,
         soret=False,
         traps_element_type="CG",
         update_jacobian=True,
         linear_solver=None,
     ):
-
         # TODO maybe transient and final_time are redundant
         self.transient = transient
         self.final_time = final_time
         self.chemical_pot = chemical_pot
         self.soret = soret
 
         self.absolute_tolerance = absolute_tolerance
```

### Comparing `FESTIM-0.11.0/festim/sources/source.py` & `FESTIM-0.11.1/festim/sources/source.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/sources/source_implantation_flux.py` & `FESTIM-0.11.1/festim/sources/source_implantation_flux.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/stepsize.py` & `FESTIM-0.11.1/festim/stepsize.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self,
         initial_value=0.0,
         stepsize_change_ratio=None,
         t_stop=None,
         stepsize_stop_max=None,
         dt_min=None,
     ) -> None:
-
         self.adaptive_stepsize = None
         if stepsize_change_ratio is not None:
             self.adaptive_stepsize = {
                 "stepsize_change_ratio": stepsize_change_ratio,
                 "t_stop": t_stop,
                 "stepsize_stop_max": stepsize_stop_max,
                 "dt_min": dt_min,
```

### Comparing `FESTIM-0.11.0/festim/temperature/temperature.py` & `FESTIM-0.11.1/festim/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/temperature/temperature_from_xdmf.py` & `FESTIM-0.11.1/festim/temperature/temperature_from_xdmf.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/festim/temperature/temperature_solver.py` & `FESTIM-0.11.1/festim/temperature/temperature_solver.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/setup.cfg` & `FESTIM-0.11.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/h_transport_problem/test_initialisation.py` & `FESTIM-0.11.1/test/h_transport_problem/test_initialisation.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/h_transport_problem/test_solving.py` & `FESTIM-0.11.1/test/h_transport_problem/test_solving.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/heat_transfer_problem/test_solving.py` & `FESTIM-0.11.1/test/heat_transfer_problem/test_solving.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/simulation/test_construction.py` & `FESTIM-0.11.1/test/simulation/test_construction.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/simulation/test_initialise.py` & `FESTIM-0.11.1/test/simulation/test_initialise.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/simulation/test_meshing.py` & `FESTIM-0.11.1/test/simulation/test_meshing.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/simulation/test_postprocessing_integration.py` & `FESTIM-0.11.1/test/simulation/test_postprocessing_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             assert data[i][0] == t
             assert data[i][1] == 10
             assert data[i][2] == 20
             assert data[i][3] == pytest.approx(11)
             assert data[i][4] == pytest.approx(11)
 
     def test_fluxes(self, my_sim):
-
         my_sim.T = festim.Temperature(100 * festim.x + 200)
         my_sim.T.create_functions(my_sim.mesh)
 
         my_sim.materials = festim.Materials(
             [
                 festim.Material(1, D_0=5, E_D=0.4, thermal_cond=3, borders=[0, 0.5]),
                 festim.Material(2, D_0=6, E_D=0.5, thermal_cond=5, borders=[0.5, 1]),
```

### Comparing `FESTIM-0.11.0/test/system/test_chemical_potential.py` & `FESTIM-0.11.1/test/system/test_chemical_potential.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/system/test_cylindrical_coordinates.py` & `FESTIM-0.11.1/test/system/test_cylindrical_coordinates.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/system/test_extrinsic_traps.py` & `FESTIM-0.11.1/test/system/test_extrinsic_traps.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/system/test_misc.py` & `FESTIM-0.11.1/test/system/test_misc.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/system/test_spherical_coordinates.py` & `FESTIM-0.11.1/test/system/test_spherical_coordinates.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/system/test_system.py` & `FESTIM-0.11.1/test/system/test_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,14 @@
         + sp.diff(v, festim.t)
         - D * sp.diff(u, festim.x, 2)
         - sp.diff(D, festim.x) * sp.diff(u, festim.x)
     )
     g = sp.diff(v, festim.t) + p * v - k * u * (n_trap - v)
 
     def run(h):
-
         my_materials = festim.Materials(
             [festim.Material(name="mat", id=1, D_0=D_0, E_D=E_D)]
         )
 
         my_trap = festim.Trap(k_0, E_k, p_0, E_p, ["mat"], n_trap)
 
         my_initial_conditions = [
```

### Comparing `FESTIM-0.11.0/test/unit/test_boundary_conditions.py` & `FESTIM-0.11.1/test/unit/test_boundary_conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from attr import has
-from sympy.matrices import expressions
 import festim
 import fenics
 import pytest
 import sympy as sp
 import numpy as np
 
 
@@ -422,14 +420,15 @@
     assert my_bc.expression(0) == pytest.approx(expected(0))
 
 
 def test_create_expression_dc_custom():
     """Creates a dc_custom bc and checks create_expression returns
     the correct expression
     """
+
     # build
     def func(T, prm1, prm2):
         return 2 * T + prm1 * prm2
 
     T = fenics.Expression("2 + x[0] + t", degree=1, t=0)
     expressions = [T]
     # run
@@ -451,14 +450,15 @@
 
 
 def test_create_form_flux_custom():
     """Creates a flux_custom bc and checks
     create_form returns
     the correct form
     """
+
     # build
     def func(T, c, prm1, prm2):
         return 2 * T + c + prm1 * prm2
 
     expr_prm1 = 1 + 2 * festim.t + festim.x
     expr_prm2 = 2
     expr_T = 2 + festim.x + festim.t
@@ -477,15 +477,14 @@
 
     # test
     mesh = fenics.UnitIntervalMesh(10)
     V = fenics.FunctionSpace(mesh, "P", 1)
     expected_expr = 2 * expr_T + expr_c + expr_prm1 * expr_prm2
     expected_expr = fenics.Expression(sp.printing.ccode(expected_expr), t=0, degree=1)
     for t in range(10):
-
         expected_expr.t = t
         for expr in my_BC.sub_expressions + expressions:
             expr.t = t
         expected = fenics.project(expected_expr, V)
         computed = fenics.project(value_BC, V)
         for x in [0, 0.5, 1]:
             assert computed(x) == pytest.approx(expected(x))
```

### Comparing `FESTIM-0.11.0/test/unit/test_concentration.py` & `FESTIM-0.11.1/test/unit/test_concentration.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
         for t in [1, 1.5, 6, 8]:
             comp.t = t
             for x in [2, 5, 0, 6]:
                 assert comp(x) == 1 + t - x
 
     def test_get_comp_from_xdmf(self, tmpdir):
-
         # build
         value = 1 + festim.t - festim.x
 
         u = f.Expression(sp.printing.ccode(value), degree=1, t=0)
         u = f.interpolate(u, self.V)
 
         d = tmpdir.mkdir("folder")
```

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_average_surface.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_average_surface.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_average_volume.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_average_volume.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_derived_quantities.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_derived_quantities.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_maximum_surface.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_maximum_surface.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_maximum_volume.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_maximum_volume.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_minimum_surface.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_minimum_surface.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_minimum_volume.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_minimum_volume.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_surface_flux.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_surface_flux.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_total_surface.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_total_surface.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_derived_quantities/test_total_volume.py` & `FESTIM-0.11.1/test/unit/test_exports/test_derived_quantities/test_total_volume.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_trap_density_xdmf_export.py` & `FESTIM-0.11.1/test/unit/test_exports/test_trap_density_xdmf_export.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_txt_export.py` & `FESTIM-0.11.1/test/unit/test_exports/test_txt_export.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_txt_exports.py` & `FESTIM-0.11.1/test/unit/test_exports/test_txt_exports.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_xdmf_export.py` & `FESTIM-0.11.1/test/unit/test_exports/test_xdmf_export.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_exports/test_xdmf_exports.py` & `FESTIM-0.11.1/test/unit/test_exports/test_xdmf_exports.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_helpers.py` & `FESTIM-0.11.1/test/unit/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         def eval(self, x, values):
             values[0] = x
 
     assert isinstance(as_expression(CustomExpr()), UserExpression)
 
 
 def test_as_constant_or_expression():
-
     # constants
     assert isinstance(as_constant_or_expression(3), Constant)
     assert isinstance(as_constant_or_expression(3.0), Constant)
     assert isinstance(as_constant_or_expression(-2.0), Constant)
     assert isinstance(as_constant_or_expression(Constant(2.0)), Constant)
 
     # expressions
```

### Comparing `FESTIM-0.11.0/test/unit/test_initial_condition.py` & `FESTIM-0.11.1/test/unit/test_initial_condition.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_materials.py` & `FESTIM-0.11.1/test/unit/test_materials.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_meshing.py` & `FESTIM-0.11.1/test/unit/test_meshing.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,14 @@
             if fenics.near(x0.x(), 1):
                 assert self.my_mesh.surface_markers[facet] == 1
             if fenics.near(x0.x(), 3):
                 assert self.my_mesh.surface_markers[facet] == 2
 
 
 def test_create_mesh_xdmf(tmpdir):
-
     # write xdmf file
     mesh = fenics.UnitSquareMesh(10, 10)
     file1 = tmpdir.join("mesh.xdmf")
     f = fenics.XDMFFile(str(Path(file1)))
     f.write(mesh)
 
     # write files
@@ -198,15 +197,14 @@
         for v in fenics.vertices(f):
             vertices_mesh2.append([v.point().x(), v.point().y()])
     for i in range(0, len(vertices_mesh)):
         assert vertices_mesh[i] == vertices_mesh2[i]
 
 
 def test_subdomains_from_xdmf(tmpdir):
-
     # create mesh functions
     mesh = fenics.UnitCubeMesh(6, 6, 6)
     mf_cells = fenics.MeshFunction("size_t", mesh, mesh.topology().dim())
     mf_facets = fenics.MeshFunction("size_t", mesh, mesh.topology().dim() - 1)
 
     # assign values for cells and facets
     for i, c in enumerate(fenics.cells(mesh)):
```

### Comparing `FESTIM-0.11.0/test/unit/test_mobile.py` & `FESTIM-0.11.1/test/unit/test_mobile.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_sources.py` & `FESTIM-0.11.1/test/unit/test_sources.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_stepsize.py` & `FESTIM-0.11.1/test/unit/test_stepsize.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_temperature.py` & `FESTIM-0.11.1/test/unit/test_temperature.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_theta.py` & `FESTIM-0.11.1/test/unit/test_theta.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_traps/test_extrinsic_trap.py` & `FESTIM-0.11.1/test/unit/test_traps/test_extrinsic_trap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import festim
 import fenics as f
 
 
 class TestExtrinsicTrap:
-
     my_trap = festim.ExtrinsicTrap(
         1,
         1,
         1,
         1,
         "mat_name",
         phi_0=1 + festim.t + festim.x,
```

### Comparing `FESTIM-0.11.0/test/unit/test_traps/test_neutron_induced_trap.py` & `FESTIM-0.11.1/test/unit/test_traps/test_neutron_induced_trap.py`

 * *Files identical despite different names*

### Comparing `FESTIM-0.11.0/test/unit/test_traps/test_trap.py` & `FESTIM-0.11.1/test/unit/test_traps/test_trap.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,14 +357,15 @@
         assert my_trap.F.equals(expected_form)
         assert my_trap.F_trapping.equals(expected_form)
 
     def test_user_expression_as_density(self):
         """Test that create_trapping_form creates the correct formulation when
         a fenics.UserExpression is given as density
         """
+
         # build
         class CustomExpression(f.UserExpression):
             def eval(self, value, x):
                 value[0] = x
 
         my_trap = festim.Trap(
             k_0=1,
```

### Comparing `FESTIM-0.11.0/test/unit/test_traps/test_traps.py` & `FESTIM-0.11.1/test/unit/test_traps/test_traps.py`

 * *Files identical despite different names*

