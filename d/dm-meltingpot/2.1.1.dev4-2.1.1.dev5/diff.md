# Comparing `tmp/dm-meltingpot-2.1.1.dev4.tar.gz` & `tmp/dm-meltingpot-2.1.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-meltingpot-2.1.1.dev4.tar", last modified: Wed Jun 28 18:38:19 2023, max compression
+gzip compressed data, was "dm-meltingpot-2.1.1.dev5.tar", last modified: Thu Jun 29 07:26:11 2023, max compression
```

## Comparing `dm-meltingpot-2.1.1.dev4.tar` & `dm-meltingpot-2.1.1.dev5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.139508 dm-meltingpot-2.1.1.dev4/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11358 2022-06-29 10:08:59.000000 dm-meltingpot-2.1.1.dev4/LICENSE
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8547 2023-06-28 18:38:19.139331 dm-meltingpot-2.1.1.dev4/PKG-INFO
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     7567 2023-06-28 09:22:13.000000 dm-meltingpot-2.1.1.dev4/README.md
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.126843 dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8547 2023-06-28 18:38:19.000000 dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/PKG-INFO
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3183 2023-06-28 18:38:19.000000 dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/SOURCES.txt
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)        1 2023-06-28 18:38:19.000000 dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/dependency_links.txt
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)      274 2023-06-28 18:38:19.000000 dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/requires.txt
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)       11 2023-06-28 18:38:19.000000 dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/top_level.txt
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.126994 dm-meltingpot-2.1.1.dev4/meltingpot/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)      595 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/__init__.py
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.125059 dm-meltingpot-2.1.1.dev4/meltingpot/lua/
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.124969 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.127673 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/allelopathic_harvest/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    32772 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/allelopathic_harvest/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1414 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/allelopathic_harvest/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.128059 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/boat_race/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    30236 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/boat_race/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2292 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/boat_race/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.128426 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/clean_up/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    17922 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/clean_up/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1402 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/clean_up/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.128761 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coins/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11909 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coins/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1399 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coins/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.129250 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/collaborative_cooking/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    18568 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/collaborative_cooking/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1411 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/collaborative_cooking/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.129655 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/commons_harvest/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8393 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/commons_harvest/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1405 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/commons_harvest/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.130103 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coop_mining/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     9293 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coop_mining/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1401 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coop_mining/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.130569 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/daycare/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    24162 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/daycare/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1387 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/daycare/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.130959 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/externality_mushrooms/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    13306 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/externality_mushrooms/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1390 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/externality_mushrooms/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.131358 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/factory_of_the_commons/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    27587 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/factory_of_the_commons/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2753 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/factory_of_the_commons/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.131699 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/gift_refinements/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    13877 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/gift_refinements/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1406 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/gift_refinements/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.132093 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/grid_land/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    28617 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/grid_land/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1503 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/grid_land/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.132511 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/hidden_agenda/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    58910 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/hidden_agenda/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1129 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/hidden_agenda/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.132669 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    15261 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball/shared_components.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.133014 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__capture_the_flag/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12969 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__capture_the_flag/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1729 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__capture_the_flag/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.133334 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__king_of_the_hill/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11357 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1729 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.133845 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/predator_prey/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    28175 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/predator_prey/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2214 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/predator_prey/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.134039 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/stamina/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    15208 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/stamina/shared_components.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.134371 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/territory/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    14438 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/territory/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1704 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/territory/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.134753 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/the_matrix/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    43847 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/the_matrix/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1396 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/the_matrix/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.135128 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/trade/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    34427 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/trade/components.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1749 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/trade/init.lua
-drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-28 18:38:19.139076 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3528 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/api_factory.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6450 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_grappling.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     9559 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_grasp.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    46382 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_library.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2765 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_library_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    22521 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/base_simulation.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4761 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/base_simulation_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4388 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/colors.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3536 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    42148 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_library.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2627 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_library_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1721 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_registry.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1904 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_registry_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     5483 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/error_handling.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2421 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/error_handling_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    21610 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/game_object.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12410 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/game_object_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2585 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/piece_movement_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6260 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/prefab_utils.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6046 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/prefab_utils_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11744 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/updater_registry.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12308 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/updater_registry_test.lua
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)      214 2023-06-28 09:22:13.000000 dm-meltingpot-2.1.1.dev4/pyproject.toml
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)       38 2023-06-28 18:38:19.139555 dm-meltingpot-2.1.1.dev4/setup.cfg
--rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4982 2023-06-28 18:10:12.000000 dm-meltingpot-2.1.1.dev4/setup.py
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.073669 dm-meltingpot-2.1.1.dev5/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11358 2022-06-29 10:08:59.000000 dm-meltingpot-2.1.1.dev5/LICENSE
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8547 2023-06-29 07:26:11.073492 dm-meltingpot-2.1.1.dev5/PKG-INFO
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     7567 2023-06-28 09:22:13.000000 dm-meltingpot-2.1.1.dev5/README.md
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.060984 dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8547 2023-06-29 07:26:11.000000 dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/PKG-INFO
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3183 2023-06-29 07:26:11.000000 dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/SOURCES.txt
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)        1 2023-06-29 07:26:11.000000 dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/dependency_links.txt
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)      294 2023-06-29 07:26:11.000000 dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/requires.txt
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)       11 2023-06-29 07:26:11.000000 dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/top_level.txt
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.061110 dm-meltingpot-2.1.1.dev5/meltingpot/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)      595 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/__init__.py
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.059390 dm-meltingpot-2.1.1.dev5/meltingpot/lua/
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.059292 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.061733 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/allelopathic_harvest/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    32772 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/allelopathic_harvest/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1414 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/allelopathic_harvest/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.062125 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/boat_race/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    30236 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/boat_race/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2292 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/boat_race/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.062496 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/clean_up/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    17922 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/clean_up/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1402 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/clean_up/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.062952 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coins/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11909 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coins/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1399 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coins/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.063522 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/collaborative_cooking/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    18568 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/collaborative_cooking/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1411 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/collaborative_cooking/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.063946 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/commons_harvest/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     8393 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/commons_harvest/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1405 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/commons_harvest/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.064274 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coop_mining/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     9293 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coop_mining/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1401 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coop_mining/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.064663 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/daycare/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    24162 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/daycare/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1387 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/daycare/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.065099 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/externality_mushrooms/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    13306 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/externality_mushrooms/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1390 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/externality_mushrooms/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.065490 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/factory_of_the_commons/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    27587 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/factory_of_the_commons/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2753 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/factory_of_the_commons/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.065822 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/gift_refinements/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    13877 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/gift_refinements/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1406 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/gift_refinements/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.066192 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/grid_land/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    28617 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/grid_land/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1503 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/grid_land/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.066590 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/hidden_agenda/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    58910 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/hidden_agenda/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1129 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/hidden_agenda/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.066744 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    15261 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball/shared_components.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.067106 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__capture_the_flag/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12969 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__capture_the_flag/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1729 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__capture_the_flag/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.067446 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__king_of_the_hill/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11357 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1729 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.067816 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/predator_prey/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    28175 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/predator_prey/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2214 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/predator_prey/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.067993 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/stamina/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    15208 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/stamina/shared_components.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.068324 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/territory/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    14438 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/territory/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1704 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/territory/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.068715 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/the_matrix/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    43847 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/the_matrix/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1396 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/the_matrix/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.069108 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/trade/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    34427 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/trade/components.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1749 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/trade/init.lua
+drwxr-xr-x   0 jagapiou (279637) primarygroup (89939)        0 2023-06-29 07:26:11.073276 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3528 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/api_factory.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6450 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_grappling.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     9559 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_grasp.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    46382 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_library.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2765 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_library_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    22521 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/base_simulation.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4761 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/base_simulation_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4388 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/colors.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     3536 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    42148 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_library.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2627 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_library_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1721 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_registry.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     1904 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_registry_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     5483 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/error_handling.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2421 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/error_handling_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    21610 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/game_object.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12410 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/game_object_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     2585 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/piece_movement_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6260 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/prefab_utils.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     6046 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/prefab_utils_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    11744 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/updater_registry.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)    12308 2023-06-22 18:01:31.000000 dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/updater_registry_test.lua
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)      214 2023-06-28 09:22:13.000000 dm-meltingpot-2.1.1.dev5/pyproject.toml
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)       38 2023-06-29 07:26:11.073715 dm-meltingpot-2.1.1.dev5/setup.cfg
+-rw-r--r--   0 jagapiou (279637) primarygroup (89939)     4748 2023-06-29 07:23:14.000000 dm-meltingpot-2.1.1.dev5/setup.py
```

### Comparing `dm-meltingpot-2.1.1.dev4/LICENSE` & `dm-meltingpot-2.1.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/PKG-INFO` & `dm-meltingpot-2.1.1.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-meltingpot
-Version: 2.1.1.dev4
+Version: 2.1.1.dev5
 Summary: A suite of test scenarios for multi-agent reinforcement learning.
 Home-page: https://github.com/deepmind/meltingpot
 Download-URL: https://github.com/deepmind/meltingpot
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Keywords: multi-agent reinforcement-learning python machine-learning
```

### Comparing `dm-meltingpot-2.1.1.dev4/README.md` & `dm-meltingpot-2.1.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/PKG-INFO` & `dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-meltingpot
-Version: 2.1.1.dev4
+Version: 2.1.1.dev5
 Summary: A suite of test scenarios for multi-agent reinforcement learning.
 Home-page: https://github.com/deepmind/meltingpot
 Download-URL: https://github.com/deepmind/meltingpot
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Keywords: multi-agent reinforcement-learning python machine-learning
```

### Comparing `dm-meltingpot-2.1.1.dev4/dm_meltingpot.egg-info/SOURCES.txt` & `dm-meltingpot-2.1.1.dev5/dm_meltingpot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/__init__.py` & `dm-meltingpot-2.1.1.dev5/meltingpot/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/allelopathic_harvest/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/allelopathic_harvest/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/allelopathic_harvest/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/allelopathic_harvest/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/boat_race/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/boat_race/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/boat_race/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/boat_race/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/clean_up/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/clean_up/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/clean_up/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/clean_up/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coins/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coins/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coins/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coins/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/collaborative_cooking/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/collaborative_cooking/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/collaborative_cooking/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/collaborative_cooking/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/commons_harvest/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/commons_harvest/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/commons_harvest/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/commons_harvest/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coop_mining/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coop_mining/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/coop_mining/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/coop_mining/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/daycare/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/daycare/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/daycare/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/daycare/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/externality_mushrooms/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/externality_mushrooms/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/externality_mushrooms/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/externality_mushrooms/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/factory_of_the_commons/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/factory_of_the_commons/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/factory_of_the_commons/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/factory_of_the_commons/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/gift_refinements/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/gift_refinements/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/gift_refinements/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/gift_refinements/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/grid_land/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/grid_land/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/grid_land/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/grid_land/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/hidden_agenda/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/hidden_agenda/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/hidden_agenda/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/hidden_agenda/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball/shared_components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball/shared_components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__capture_the_flag/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__capture_the_flag/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__capture_the_flag/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__capture_the_flag/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__king_of_the_hill/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/paintball__king_of_the_hill/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/predator_prey/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/predator_prey/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/predator_prey/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/predator_prey/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/stamina/shared_components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/stamina/shared_components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/territory/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/territory/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/territory/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/territory/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/the_matrix/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/the_matrix/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/the_matrix/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/the_matrix/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/trade/components.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/trade/components.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/levels/trade/init.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/levels/trade/init.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/api_factory.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/api_factory.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_grappling.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_grappling.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_grasp.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_grasp.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_library.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_library.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/avatar_library_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/avatar_library_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/base_simulation.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/base_simulation.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/base_simulation_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/base_simulation_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/colors.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/colors.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_library.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_library.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_library_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_library_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_registry.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_registry.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/component_registry_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/component_registry_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/error_handling.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/error_handling.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/error_handling_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/error_handling_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/game_object.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/game_object.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/game_object_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/game_object_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/piece_movement_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/piece_movement_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/prefab_utils.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/prefab_utils.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/prefab_utils_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/prefab_utils_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/updater_registry.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/updater_registry.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/meltingpot/lua/modules/updater_registry_test.lua` & `dm-meltingpot-2.1.1.dev5/meltingpot/lua/modules/updater_registry_test.lua`

 * *Files identical despite different names*

### Comparing `dm-meltingpot-2.1.1.dev4/setup.py` & `dm-meltingpot-2.1.1.dev5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 import shutil
 import tarfile
 import urllib.request
 
 import setuptools
 from setuptools.command import build_py
 
-VERSION = '2.1.1-dev.4'
+VERSION = '2.1.1-dev.5'
 ASSETS_VERSION = '2.1.0'
 
 ASSETS_URL = f'http://storage.googleapis.com/dm-meltingpot/meltingpot-assets-{ASSETS_VERSION}.tar.gz'
 
 IS_M1_MAC = platform.system() == 'Darwin' and platform.machine() == 'arm64'
 
 
 class BuildPy(build_py.build_py):
   """Command that downloads Melting Pot assets as part of build_py."""
 
   def run(self):
-    self.editable_mode = False
     self.download_and_extract_assets()
-    super().run()
-    self.build_assets()
+    if not self.editable_mode:
+      super().run()
+      self.build_assets()
 
   def download_and_extract_assets(self):
     """Downloads and extracts assets to meltingpot/assets."""
     tar_file_path = os.path.join(
         self.get_package_dir('assets'), os.path.basename(ASSETS_URL))
     if os.path.exists(tar_file_path):
       print(f'found cached assets {tar_file_path}', flush=True)
@@ -95,27 +95,24 @@
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     cmdclass={'build_py': BuildPy},
     packages=['meltingpot'],
     package_data={
         'meltingpot': [
-            # 'assets/saved_models/**/**/saved_model.pb',
-            # 'assets/saved_models/**/**/variables/variables.data-00000-of-00001',
-            # 'assets/saved_models/**/**/variables/variables.index',
             'lua/modules/*',
             'lua/levels/**/*',
         ],
     },
     python_requires='>=3.9',
     install_requires=[
         'absl-py',
         'chex',
         'dm_env',
-        # 'dmlab2d',  # Not yet available for PIP install.
+        'dmlab2d==1.0.0.dev8',
         'immutabledict',
         'ml-collections',
         'networkx',
         'numpy',
         'opencv-python',
         'pandas',
         'pygame',
```

