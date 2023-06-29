# Comparing `tmp/ansys-api-pyensight-0.1.0.tar.gz` & `tmp/ansys-api-pyensight-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-pyensight-0.1.0.tar", last modified: Thu Jun 22 09:15:47 2023, max compression
+gzip compressed data, was "ansys-api-pyensight-0.2.0.tar", last modified: Thu Jun 29 13:06:54 2023, max compression
```

## Comparing `ansys-api-pyensight-0.1.0.tar` & `ansys-api-pyensight-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.162565 ansys-api-pyensight-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-22 09:15:47.162565 ansys-api-pyensight-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:15:47.162565 ansys-api-pyensight-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.154565 ansys-api-pyensight-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.154565 ansys-api-pyensight-0.1.0/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.154565 ansys-api-pyensight-0.1.0/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.158565 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.158565 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/enshell.proto
--rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/ensight.proto
--rw-r--r--   0 runner    (1001) docker     (123)  2446597 2023-06-22 09:15:29.000000 ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/ensight_api.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:15:47.162565 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-22 09:15:47.000000 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 09:15:47.000000 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:15:47.000000 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 09:15:47.000000 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 09:15:47.000000 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 09:15:47.000000 ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.809730 ansys-api-pyensight-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 13:06:54.809730 ansys-api-pyensight-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:06:54.809730 ansys-api-pyensight-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.789730 ansys-api-pyensight-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.785730 ansys-api-pyensight-0.2.0/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.785730 ansys-api-pyensight-0.2.0/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.805730 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/access_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.805730 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   926642 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_animobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30169 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48180 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34554 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35302 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_lgnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35577 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30261 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_annot_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34357 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_emitterobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_flipbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214200 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_lightsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_lpart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56524 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264396 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)   195871 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_aux_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190146 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_axisymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179413 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_built_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)   289827 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202105 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186771 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_developed_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264534 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_discrete_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192486 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_elevated_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241715 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192689 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_fx_sep_att.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202494 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_fx_shock.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192681 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_fx_vortex_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192954 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_isosurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183318 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_mat_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264486 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   243979 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_particle_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181578 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187760 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198386 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_tensor_glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204686 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_vector_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)   236410 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_part_vof.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132145 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83457 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_revolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_tool_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)   211317 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ens_vport.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2000687 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/ensight_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.805730 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/enshell.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/ensight.proto
+-rw-r--r--   0 runner    (1001) docker     (123)  2446597 2023-06-29 13:06:33.000000 ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/ensight_api.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:06:54.809730 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 13:06:54.000000 ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/top_level.txt
```

### Comparing `ansys-api-pyensight-0.1.0/LICENSE` & `ansys-api-pyensight-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.0/PKG-INFO` & `ansys-api-pyensight-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-pyensight
-Version: 0.1.0
-Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:15:47 on 22 June 2023
+Version: 0.2.0
+Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 13:06:53 on 29 June 2023
 Home-page: https://github.com/ansys/ansys-api-pyensight
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ansys-api-pyensight-0.1.0/README.md` & `ansys-api-pyensight-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/enshell.proto` & `ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/enshell.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/ensight.proto` & `ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/ensight.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.0/src/ansys/api/pyensight/v0/ensight_api.xml` & `ansys-api-pyensight-0.2.0/src/ansys/api/pyensight/v0/ensight_api.xml`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.0/src/ansys_api_pyensight.egg-info/PKG-INFO` & `ansys-api-pyensight-0.2.0/src/ansys_api_pyensight.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-pyensight
-Version: 0.1.0
-Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:15:47 on 22 June 2023
+Version: 0.2.0
+Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 13:06:53 on 29 June 2023
 Home-page: https://github.com/ansys/ansys-api-pyensight
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.8
```

