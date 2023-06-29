# Comparing `tmp/NodeGraphQt-0.6.3.tar.gz` & `tmp/NodeGraphQt-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.6.3.tar", last modified: Fri Jun 23 05:15:11 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.4.tar", last modified: Thu Jun 29 06:24:17 2023, max compression
```

## Comparing `NodeGraphQt-0.6.3.tar` & `NodeGraphQt-0.6.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.893833 NodeGraphQt-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.885833 NodeGraphQt-0.6.3/NodeGraphQt/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.885833 NodeGraphQt-0.6.3/NodeGraphQt/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)   100336 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/base/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.885833 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.889833 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.889833 NodeGraphQt-0.6.3/NodeGraphQt/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/nodes/backdrop_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    26737 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/nodes/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/nodes/base_node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/nodes/port_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/pkg_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.889833 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_backdrop.py
--rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_port_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_port_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_text_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.889833 NodeGraphQt-0.6.3/NodeGraphQt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.889833 NodeGraphQt-0.6.3/NodeGraphQt/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/icons/node_base.png
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/node_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/node_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/tab_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    54574 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/NodeGraphQt/widgets/viewer_nav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.885833 NodeGraphQt-0.6.3/NodeGraphQt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-23 05:15:11.000000 NodeGraphQt-0.6.3/NodeGraphQt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-23 05:15:11.000000 NodeGraphQt-0.6.3/NodeGraphQt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 05:15:11.000000 NodeGraphQt-0.6.3/NodeGraphQt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 05:15:11.000000 NodeGraphQt-0.6.3/NodeGraphQt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 05:15:11.000000 NodeGraphQt-0.6.3/NodeGraphQt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-23 05:15:11.893833 NodeGraphQt-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.881833 NodeGraphQt-0.6.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.889833 NodeGraphQt-0.6.3/examples/hotkeys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/hotkeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/hotkeys/hotkey_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:11.893833 NodeGraphQt-0.6.3/examples/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/nodes/basic_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/nodes/custom_ports_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/examples/nodes/widget_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-23 05:15:11.893833 NodeGraphQt-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 05:15:04.000000 NodeGraphQt-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.643869 NodeGraphQt-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.623868 NodeGraphQt-0.6.4/NodeGraphQt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.627869 NodeGraphQt-0.6.4/NodeGraphQt/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100336 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/base/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.627869 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.631868 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.635869 NodeGraphQt-0.6.4/NodeGraphQt/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/nodes/backdrop_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/nodes/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/nodes/base_node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/nodes/port_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/pkg_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.639869 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_port_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_port_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_text_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.639869 NodeGraphQt-0.6.4/NodeGraphQt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.639869 NodeGraphQt-0.6.4/NodeGraphQt/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/icons/node_base.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/node_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/node_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/tab_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54574 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/NodeGraphQt/widgets/viewer_nav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.623868 NodeGraphQt-0.6.4/NodeGraphQt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-29 06:24:17.000000 NodeGraphQt-0.6.4/NodeGraphQt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-29 06:24:17.000000 NodeGraphQt-0.6.4/NodeGraphQt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:24:17.000000 NodeGraphQt-0.6.4/NodeGraphQt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 06:24:17.000000 NodeGraphQt-0.6.4/NodeGraphQt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 06:24:17.000000 NodeGraphQt-0.6.4/NodeGraphQt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-29 06:24:17.643869 NodeGraphQt-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.619868 NodeGraphQt-0.6.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.643869 NodeGraphQt-0.6.4/examples/hotkeys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/hotkeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/hotkeys/hotkey_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:17.643869 NodeGraphQt-0.6.4/examples/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/nodes/basic_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/nodes/custom_ports_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/examples/nodes/widget_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-29 06:24:17.643869 NodeGraphQt-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 06:24:09.000000 NodeGraphQt-0.6.4/setup.py
```

### Comparing `NodeGraphQt-0.6.3/LICENSE.md` & `NodeGraphQt-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.4/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/base/port.py` & `NodeGraphQt-0.6.4/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.4/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.4/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.4/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.4/NodeGraphQt/nodes/base_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -282,14 +282,58 @@
         )
         widget = NodeCheckBox(self.view, name, label, text, state)
         widget.value_changed.connect(lambda k, v: self.set_property(k, v))
         self.view.add_widget(widget)
         #: redraw node to address calls outside the "__init__" func.
         self.view.draw_node()
 
+    def hide_widget(self, name):
+        """
+        Hide an embedded node widget.
+
+        Warnings:
+            Undo is NOT yet supported for this function.
+
+        Args:
+            name (str): node property name for the widget.
+
+        See Also:
+            :meth:`BaseNode.add_custom_widget`,
+            :meth:`BaseNode.show_widget`,
+            :meth:`BaseNode.get_widget`
+        """
+        # TODO: implement this logic to the undo stack.
+        if not self.view.has_widget(name):
+            return
+        widget = self.view.get_widget(name)
+        widget.hide()
+        self.view.draw_node()
+
+    def show_widget(self, name):
+        """
+        Show an embedded node widget.
+
+        Warnings:
+            Undo is NOT yet supported for this function.
+
+        Args:
+            name (str): node property name for the widget.
+
+        See Also:
+            :meth:`BaseNode.add_custom_widget`,
+            :meth:`BaseNode.hide_widget`,
+            :meth:`BaseNode.get_widget`
+        """
+        # TODO: implement this logic to the undo stack.
+        if not self.view.has_widget(name):
+            return
+        widget = self.view.get_widget(name)
+        widget.show()
+        self.view.draw_node()
+
     def add_input(self, name='input', multi_input=False, display_name=True,
                   color=None, locked=False, painter_func=None):
         """
         Add input :class:`Port` to node.
 
         Warnings:
             Undo is NOT supported for this function.
```

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.4/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.4/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.4/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,14 +368,16 @@
 
         port_text_width = p_input_text_width + p_output_text_width
 
         # width, height from node embedded widgets.
         widget_width = 0.0
         widget_height = 0.0
         for widget in self._widgets.values():
+            if not widget.isVisible():
+                continue
             w_width = widget.boundingRect().width()
             w_height = widget.boundingRect().height()
             if w_width > widget_width:
                 widget_width = w_width
             widget_height += w_height
 
         side_padding = 0.0
@@ -411,14 +413,16 @@
                 p_output_width += port.boundingRect().width()
                 if not p_output_height:
                     p_output_height = port.boundingRect().height()
 
         widget_width = 0.0
         widget_height = 0.0
         for widget in self._widgets.values():
+            if not widget.isVisible():
+                continue
             if widget.boundingRect().width() > widget_width:
                 widget_width = widget.boundingRect().width()
             widget_height += widget.boundingRect().height()
 
         width = max([p_input_width, p_output_width, widget_width])
         height = p_input_height + p_output_height + widget_height
         return width, height
@@ -507,14 +511,16 @@
         if not self._widgets:
             return
         rect = self.boundingRect()
         y = rect.y() + v_offset
         inputs = [p for p in self.inputs if p.isVisible()]
         outputs = [p for p in self.outputs if p.isVisible()]
         for widget in self._widgets.values():
+            if not widget.isVisible():
+                continue
             widget_rect = widget.boundingRect()
             if not inputs:
                 x = rect.left() + 10
                 widget.widget().setTitleAlign('left')
             elif not outputs:
                 x = rect.right() - widget_rect.width() - 10
                 widget.widget().setTitleAlign('right')
@@ -527,19 +533,23 @@
     def _align_widgets_vertical(self, v_offset):
         if not self._widgets:
             return
         rect = self.boundingRect()
         y = rect.center().y() + v_offset
         widget_height = 0.0
         for widget in self._widgets.values():
+            if not widget.isVisible():
+                continue
             widget_rect = widget.boundingRect()
             widget_height += widget_rect.height()
         y -= widget_height / 2
 
         for widget in self._widgets.values():
+            if not widget.isVisible():
+                continue
             widget_rect = widget.boundingRect()
             x = rect.center().x() - (widget_rect.width() / 2)
             widget.widget().setTitleAlign('center')
             widget.setPos(x, y)
             y += widget_rect.height()
 
     def align_widgets(self, v_offset=0.0):
@@ -773,16 +783,14 @@
                 text.setVisible(port_text_visible)
 
         # output port text visibility.
         for port, text in self._output_items.items():
             if port.display_name:
                 text.setVisible(port_text_visible)
 
-
-
         self._text_item.setVisible(visible)
         self._icon_item.setVisible(visible)
 
     @property
     def icon(self):
         return self._properties['icon']
```

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.4/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.4/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.4/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.3
+Version: 0.6.4
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -28,15 +28,15 @@
 NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
 ## Install
 
-NodeGraphQt is avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
+NodeGraphQt is available on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
 ```
 pip install NodeGraphQt
 ```
 or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
 
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.3 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.4 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: PySide2 License-File:
 LICENSE.md # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
 NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented
 and re-purposed into applications. [https://raw.githubusercontent.com/jchanvfx/
 NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
-avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/
+available on The Python Package Index (PyPI) [here](https://pypi.org/project/
 NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
 you can download previous versions from the [releases](https://github.com/
 jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
 jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
 basic_example.py) script to get started or check out the API example overview
 here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
 examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
```

### Comparing `NodeGraphQt-0.6.3/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.4/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/PKG-INFO` & `NodeGraphQt-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.3
+Version: 0.6.4
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -28,15 +28,15 @@
 NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
 ## Install
 
-NodeGraphQt is avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
+NodeGraphQt is available on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
 ```
 pip install NodeGraphQt
 ```
 or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
 
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.3 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.4 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: PySide2 License-File:
 LICENSE.md # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
 NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented
 and re-purposed into applications. [https://raw.githubusercontent.com/jchanvfx/
 NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
-avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/
+available on The Python Package Index (PyPI) [here](https://pypi.org/project/
 NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
 you can download previous versions from the [releases](https://github.com/
 jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
 jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
 basic_example.py) script to get started or check out the API example overview
 here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
 examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
```

### Comparing `NodeGraphQt-0.6.3/README.md` & `NodeGraphQt-0.6.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented and re-purposed into 
 applications.
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
 
 ## Install
 
-NodeGraphQt is avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
+NodeGraphQt is available on The Python Package Index (PyPI) [here](https://pypi.org/project/NodeGraphQt) so it can be installed with:
 ```
 pip install NodeGraphQt
 ```
 or you can download previous versions from the [releases](https://github.com/jchanvfx/NodeGraphQt/releases) page.
 
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
  # NodeGraphQt
   [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
                                    logo.png]
 NodeGraphQt is a node graph UI framework for `PySide2` that can be implemented
 and re-purposed into applications. [https://raw.githubusercontent.com/jchanvfx/
 NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
-avaliable on The Python Package Index (PyPI) [here](https://pypi.org/project/
+available on The Python Package Index (PyPI) [here](https://pypi.org/project/
 NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
 you can download previous versions from the [releases](https://github.com/
 jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
 jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
 basic_example.py) script to get started or check out the API example overview
 here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
 examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
```

### Comparing `NodeGraphQt-0.6.3/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.4/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.4/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.4/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.4/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.3/setup.cfg` & `NodeGraphQt-0.6.4/setup.cfg`

 * *Files identical despite different names*

