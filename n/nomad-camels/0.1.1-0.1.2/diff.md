# Comparing `tmp/nomad_camels-0.1.1.tar.gz` & `tmp/nomad_camels-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels-0.1.1.tar", last modified: Wed Jun 28 15:50:25 2023, max compression
+gzip compressed data, was "nomad_camels-0.1.2.tar", last modified: Thu Jun 29 11:53:37 2023, max compression
```

## Comparing `nomad_camels-0.1.1.tar` & `nomad_camels-0.1.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.338253 nomad_camels-0.1.1/
--rw-rw-rw-   0        0        0    26526 2023-06-28 14:51:17.000000 nomad_camels-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    26525 2023-06-28 14:51:17.000000 nomad_camels-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       27 2023-06-28 14:51:17.000000 nomad_camels-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2155 2023-06-28 15:50:25.338253 nomad_camels-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-06-28 14:51:17.000000 nomad_camels-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.138274 nomad_camels-0.1.1/nomad_camels/
--rw-rw-rw-   0        0        0     4227 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/CAMELS_start.py
--rw-rw-rw-   0        0        0    43072 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/MainApp_v2.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.188272 nomad_camels-0.1.1/nomad_camels/bluesky_handling/
--rw-rw-rw-   0        0        0     5236 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/EpicsFieldSignal.py
--rw-rw-rw-   0        0        0     1827 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/__init__.py
--rw-rw-rw-   0        0        0     6047 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/builder_helper_functions.py
--rw-rw-rw-   0        0        0     4103 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/custom_function_signal.py
--rw-rw-rw-   0        0        0     4841 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/evaluation_helper.py
--rw-rw-rw-   0        0        0    18283 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/helper_functions.py
--rw-rw-rw-   0        0        0     1666 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/make_catalog.py
--rw-rw-rw-   0        0        0    14009 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/protocol_builder.py
--rw-rw-rw-   0        0        0      786 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/special_plan_stubs.py
--rw-rw-rw-   0        0        0    10584 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/bluesky_handling/visa_signal.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.188272 nomad_camels-0.1.1/nomad_camels/commands/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/commands/__init__.py
--rw-rw-rw-   0        0        0     4635 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/commands/change_sequence.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.198270 nomad_camels-0.1.1/nomad_camels/frontpanels/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/__init__.py
--rw-rw-rw-   0        0        0     9749 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/device_add_dialog.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.208269 nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/__init__.py
--rw-rw-rw-   0        0        0     8771 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
--rw-rw-rw-   0        0        0      830 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
--rw-rw-rw-   0        0        0      236 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/pass_ask.py
--rw-rw-rw-   0        0        0    10082 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/instrument_config.py
--rw-rw-rw-   0        0        0    13171 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/instrument_installer.py
--rw-rw-rw-   0        0        0     2904 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/manage_instruments.py
--rw-rw-rw-   0        0        0    22774 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/plot_definer.py
--rw-rw-rw-   0        0        0    22381 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/protocol_config.py
--rw-rw-rw-   0        0        0     8557 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/settings_window.py
--rw-rw-rw-   0        0        0     1951 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/frontpanels/taskSelector.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.218267 nomad_camels-0.1.1/nomad_camels/graphics/
--rw-rw-rw-   0        0        0    16958 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/CAMELS.ico
--rw-rw-rw-   0        0        0     2926 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/CAMELS_Icon.png
--rw-rw-rw-   0        0        0   101760 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
--rw-rw-rw-   0        0        0   479310 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
--rw-rw-rw-   0        0        0    13283 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/camels-horizontal.svg
--rw-rw-rw-   0        0        0    13715 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/camels-vertical.svg
--rw-rw-rw-   0        0        0    12919 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/camels_horizontal.png
--rw-rw-rw-   0        0        0    19245 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/camels_vertical.png
--rw-rw-rw-   0        0        0    40043 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/dark.qss
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.238264 nomad_camels-0.1.1/nomad_camels/graphics/legacy/
--rw-rw-rw-   0        0        0    60728 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS.svg
--rw-rw-rw-   0        0        0    52644 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Icon.png
--rw-rw-rw-   0        0        0   349358 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
--rw-rw-rw-   0        0        0    34101 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
--rw-rw-rw-   0        0        0    42984 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Logo.png
--rw-rw-rw-   0        0        0    43703 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Logo.svg
--rw-rw-rw-   0        0        0    96186 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
--rw-rw-rw-   0        0        0    18507 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_V1.svg
--rw-rw-rw-   0        0        0    20058 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_v2.svg
--rw-rw-rw-   0        0        0   290607 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/camels - Kopie.png
--rw-rw-rw-   0        0        0   252699 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/camels_free.png
--rw-rw-rw-   0        0        0     7058 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/graphics/legacy/plus_sign.png
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.268261 nomad_camels-0.1.1/nomad_camels/gui/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/__init__.py
--rw-rw-rw-   0        0        0     6130 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/addDeviceDialog.py
--rw-rw-rw-   0        0        0     5535 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/device_installer.py
--rw-rw-rw-   0        0        0     2841 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/enterTextDialog.py
--rw-rw-rw-   0        0        0     4027 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/fit_definer.py
--rw-rw-rw-   0        0        0    11001 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/for_loop.py
--rw-rw-rw-   0        0        0     6623 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/general_protocol_settings.py
--rw-rw-rw-   0        0        0     8501 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/gradient_descent_step.py
--rw-rw-rw-   0        0        0     8629 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/installer_window.py
--rw-rw-rw-   0        0        0     4572 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/instrument_config.py
--rw-rw-rw-   0        0        0    22581 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/gui/mainWindow_v2.py
--rw-rw-rw-   0        0        0     2893 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/pass_ask.py
--rw-rw-rw-   0        0        0     7219 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/plot_definer.py
--rw-rw-rw-   0        0        0     6027 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/plot_definer_2d.py
--rw-rw-rw-   0        0        0     3885 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/plot_options.py
--rw-rw-rw-   0        0        0     7230 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/protocol_view.py
--rw-rw-rw-   0        0        0     2537 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/read_channels.py
--rw-rw-rw-   0        0        0     1465 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/set_channels.py
--rw-rw-rw-   0        0        0    13462 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/gui/settings_window.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.278259 nomad_camels-0.1.1/nomad_camels/loop_steps/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/__init__.py
--rw-rw-rw-   0        0        0     4250 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/change_device_config.py
--rw-rw-rw-   0        0        0    28108 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/for_while_loops.py
--rw-rw-rw-   0        0        0     8185 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/gradient_descent.py
--rw-rw-rw-   0        0        0    10586 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/if_step.py
--rw-rw-rw-   0        0        0     4905 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/make_step_of_type.py
--rw-rw-rw-   0        0        0    13322 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/nd_sweep.py
--rw-rw-rw-   0        0        0     3550 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/prompt_loop_step.py
--rw-rw-rw-   0        0        0    15156 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/read_channels.py
--rw-rw-rw-   0        0        0     7679 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/run_subprotocol.py
--rw-rw-rw-   0        0        0     4488 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/set_channels.py
--rw-rw-rw-   0        0        0     4099 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/set_value_popup.py
--rw-rw-rw-   0        0        0     2383 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/set_variables.py
--rw-rw-rw-   0        0        0    14715 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/simple_sweep.py
--rw-rw-rw-   0        0        0     2648 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/loop_steps/wait_loop_step.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.288258 nomad_camels-0.1.1/nomad_camels/main_classes/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/camels_installer.py
--rw-rw-rw-   0        0        0    28615 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/main_classes/device_class.py
--rw-rw-rw-   0        0        0     3595 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/list_plot.py
--rw-rw-rw-   0        0        0    11255 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/loop_step.py
--rw-rw-rw-   0        0        0     3993 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/manual_control.py
--rw-rw-rw-   0        0        0     1242 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/measurement_channel.py
--rw-rw-rw-   0        0        0     7869 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/plot_2D.py
--rw-rw-rw-   0        0        0    48782 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/main_classes/plot_widget.py
--rw-rw-rw-   0        0        0    21225 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/main_classes/protocol_class.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.298257 nomad_camels-0.1.1/nomad_camels/manual_controls/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/manual_controls/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/manual_controls/get_manual_controls.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.298257 nomad_camels-0.1.1/nomad_camels/manual_controls/stage_control/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/manual_controls/stage_control/__init__.py
--rw-rw-rw-   0        0        0    20282 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/manual_controls/stage_control/stage_control.py
--rw-rw-rw-   0        0        0    12048 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/manual_controls/stage_control/ui_stage_control.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.298257 nomad_camels-0.1.1/nomad_camels/tests/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/tests/__init__.py
--rw-rw-rw-   0        0        0     3182 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/tests/instrument_management_test.py
--rw-rw-rw-   0        0        0    20124 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/tests/protocol_test.py
--rw-rw-rw-   0        0        0      768 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/tests/startup_test.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.308256 nomad_camels-0.1.1/nomad_camels/tools/
--rw-rw-rw-   0        0        0     8502 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/tools/EPICS_driver_builder.py
--rw-rw-rw-   0        0        0     5627 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/tools/VISA_builder.py
--rw-rw-rw-   0        0        0    11374 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/tools/VISA_driver_builder.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/tools/__init__.py
--rw-rw-rw-   0        0        0     8548 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/tools/databroker_exporter.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.318255 nomad_camels-0.1.1/nomad_camels/ui_widgets/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/__init__.py
--rw-rw-rw-   0        0        0    20475 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/add_remove_table.py
--rw-rw-rw-   0        0        0     9089 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/channels_check_table.py
--rw-rw-rw-   0        0        0     1742 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/console_redirect.py
--rw-rw-rw-   0        0        0     1204 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/drag_drop_tree_view.py
--rw-rw-rw-   0        0        0     6522 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/options_run_button.py
--rw-rw-rw-   0        0        0     2493 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/path_button_edit.py
--rw-rw-rw-   0        0        0     3567 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/variable_tool_tip_box.py
--rw-rw-rw-   0        0        0      451 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/ui_widgets/warn_popup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.338253 nomad_camels-0.1.1/nomad_camels/utility/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/__init__.py
--rw-rw-rw-   0        0        0    15701 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/databroker_export.py
--rw-rw-rw-   0        0        0     5099 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/utility/device_handling.py
--rw-rw-rw-   0        0        0     1833 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/exception_hook.py
--rw-rw-rw-   0        0        0      788 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/fit_variable_renaming.py
--rw-rw-rw-   0        0        0    14745 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/utility/load_save_functions.py
--rw-rw-rw-   0        0        0      938 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/load_save_helper_functions.py
--rw-rw-rw-   0        0        0      867 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/number_formatting.py
--rw-rw-rw-   0        0        0     1583 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/plot_placement.py
--rw-rw-rw-   0        0        0     9893 2023-06-28 15:46:34.000000 nomad_camels-0.1.1/nomad_camels/utility/qthreads.py
--rw-rw-rw-   0        0        0     2496 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/theme_changing.py
--rw-rw-rw-   0        0        0      330 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/tqdm_progress_bar.py
--rw-rw-rw-   0        0        0     2573 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/treeView_functions.py
--rw-rw-rw-   0        0        0     2674 2023-06-28 15:48:04.000000 nomad_camels-0.1.1/nomad_camels/utility/update_camels.py
--rw-rw-rw-   0        0        0    10431 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/nomad_camels/utility/variables_handling.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:50:25.168275 nomad_camels-0.1.1/nomad_camels.egg-info/
--rw-rw-rw-   0        0        0     2155 2023-06-28 15:50:25.000000 nomad_camels-0.1.1/nomad_camels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5841 2023-06-28 15:50:25.000000 nomad_camels-0.1.1/nomad_camels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 15:50:25.000000 nomad_camels-0.1.1/nomad_camels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1340 2023-06-28 15:50:25.000000 nomad_camels-0.1.1/nomad_camels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-28 15:50:25.000000 nomad_camels-0.1.1/nomad_camels.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      973 2023-06-28 15:48:46.000000 nomad_camels-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1340 2023-06-28 14:51:20.000000 nomad_camels-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 15:50:25.338253 nomad_camels-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:37.187896 nomad_camels-0.1.2/
+-rw-rw-rw-   0        0        0    26526 2023-06-28 14:51:17.000000 nomad_camels-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    26525 2023-06-28 14:51:17.000000 nomad_camels-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       27 2023-06-28 14:51:17.000000 nomad_camels-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2101 2023-06-29 11:53:37.187896 nomad_camels-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-06-28 14:51:17.000000 nomad_camels-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.466298 nomad_camels-0.1.2/nomad_camels/
+-rw-rw-rw-   0        0        0     4227 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/CAMELS_start.py
+-rw-rw-rw-   0        0        0    43072 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/MainApp_v2.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.486297 nomad_camels-0.1.2/nomad_camels/bluesky_handling/
+-rw-rw-rw-   0        0        0     5236 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/EpicsFieldSignal.py
+-rw-rw-rw-   0        0        0     1827 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/__init__.py
+-rw-rw-rw-   0        0        0     6047 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/builder_helper_functions.py
+-rw-rw-rw-   0        0        0     4103 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/custom_function_signal.py
+-rw-rw-rw-   0        0        0     4841 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/evaluation_helper.py
+-rw-rw-rw-   0        0        0    18283 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/helper_functions.py
+-rw-rw-rw-   0        0        0     1666 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/make_catalog.py
+-rw-rw-rw-   0        0        0    14114 2023-06-29 11:51:05.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/protocol_builder.py
+-rw-rw-rw-   0        0        0      786 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/special_plan_stubs.py
+-rw-rw-rw-   0        0        0    10584 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/bluesky_handling/visa_signal.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.486297 nomad_camels-0.1.2/nomad_camels/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/commands/__init__.py
+-rw-rw-rw-   0        0        0     4635 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/commands/change_sequence.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.496303 nomad_camels-0.1.2/nomad_camels/frontpanels/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/__init__.py
+-rw-rw-rw-   0        0        0     9749 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/device_add_dialog.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.506296 nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/__init__.py
+-rw-rw-rw-   0        0        0     8771 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
+-rw-rw-rw-   0        0        0      830 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
+-rw-rw-rw-   0        0        0      236 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/pass_ask.py
+-rw-rw-rw-   0        0        0    10082 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/instrument_config.py
+-rw-rw-rw-   0        0        0    13171 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/instrument_installer.py
+-rw-rw-rw-   0        0        0     2925 2023-06-29 11:51:05.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/manage_instruments.py
+-rw-rw-rw-   0        0        0    22774 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/plot_definer.py
+-rw-rw-rw-   0        0        0    22381 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/protocol_config.py
+-rw-rw-rw-   0        0        0     8557 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/settings_window.py
+-rw-rw-rw-   0        0        0     1951 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/frontpanels/taskSelector.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.516295 nomad_camels-0.1.2/nomad_camels/graphics/
+-rw-rw-rw-   0        0        0    16958 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/CAMELS.ico
+-rw-rw-rw-   0        0        0     2926 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/CAMELS_Icon.png
+-rw-rw-rw-   0        0        0   101760 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
+-rw-rw-rw-   0        0        0   479310 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
+-rw-rw-rw-   0        0        0    13283 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/camels-horizontal.svg
+-rw-rw-rw-   0        0        0    13715 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/camels-vertical.svg
+-rw-rw-rw-   0        0        0    12919 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/camels_horizontal.png
+-rw-rw-rw-   0        0        0    19245 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/camels_vertical.png
+-rw-rw-rw-   0        0        0    40043 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/dark.qss
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.536297 nomad_camels-0.1.2/nomad_camels/graphics/legacy/
+-rw-rw-rw-   0        0        0    60728 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS.svg
+-rw-rw-rw-   0        0        0    52644 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Icon.png
+-rw-rw-rw-   0        0        0   349358 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
+-rw-rw-rw-   0        0        0    34101 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
+-rw-rw-rw-   0        0        0    42984 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Logo.png
+-rw-rw-rw-   0        0        0    43703 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Logo.svg
+-rw-rw-rw-   0        0        0    96186 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
+-rw-rw-rw-   0        0        0    18507 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_V1.svg
+-rw-rw-rw-   0        0        0    20058 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_v2.svg
+-rw-rw-rw-   0        0        0   290607 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/camels - Kopie.png
+-rw-rw-rw-   0        0        0   252699 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/camels_free.png
+-rw-rw-rw-   0        0        0     7058 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/graphics/legacy/plus_sign.png
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.566295 nomad_camels-0.1.2/nomad_camels/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/__init__.py
+-rw-rw-rw-   0        0        0     6130 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/addDeviceDialog.py
+-rw-rw-rw-   0        0        0     5535 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/device_installer.py
+-rw-rw-rw-   0        0        0     2841 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/enterTextDialog.py
+-rw-rw-rw-   0        0        0     4027 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/fit_definer.py
+-rw-rw-rw-   0        0        0    11001 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/for_loop.py
+-rw-rw-rw-   0        0        0     6623 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/general_protocol_settings.py
+-rw-rw-rw-   0        0        0     8501 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/gradient_descent_step.py
+-rw-rw-rw-   0        0        0     8629 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/installer_window.py
+-rw-rw-rw-   0        0        0     4572 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/instrument_config.py
+-rw-rw-rw-   0        0        0    22581 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/gui/mainWindow_v2.py
+-rw-rw-rw-   0        0        0     2893 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/pass_ask.py
+-rw-rw-rw-   0        0        0     7219 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/plot_definer.py
+-rw-rw-rw-   0        0        0     6027 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/plot_definer_2d.py
+-rw-rw-rw-   0        0        0     3885 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/plot_options.py
+-rw-rw-rw-   0        0        0     7230 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/protocol_view.py
+-rw-rw-rw-   0        0        0     2537 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/read_channels.py
+-rw-rw-rw-   0        0        0     1465 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/set_channels.py
+-rw-rw-rw-   0        0        0    13462 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/gui/settings_window.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.586293 nomad_camels-0.1.2/nomad_camels/loop_steps/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/__init__.py
+-rw-rw-rw-   0        0        0     4250 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/change_device_config.py
+-rw-rw-rw-   0        0        0    28108 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/for_while_loops.py
+-rw-rw-rw-   0        0        0     8185 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/gradient_descent.py
+-rw-rw-rw-   0        0        0    10586 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/if_step.py
+-rw-rw-rw-   0        0        0     4905 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/make_step_of_type.py
+-rw-rw-rw-   0        0        0    13322 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/nd_sweep.py
+-rw-rw-rw-   0        0        0     3550 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/prompt_loop_step.py
+-rw-rw-rw-   0        0        0    15156 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/read_channels.py
+-rw-rw-rw-   0        0        0     7679 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/run_subprotocol.py
+-rw-rw-rw-   0        0        0     4488 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/set_channels.py
+-rw-rw-rw-   0        0        0     4099 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/set_value_popup.py
+-rw-rw-rw-   0        0        0     2383 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/set_variables.py
+-rw-rw-rw-   0        0        0    14715 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/simple_sweep.py
+-rw-rw-rw-   0        0        0     2648 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/loop_steps/wait_loop_step.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.596291 nomad_camels-0.1.2/nomad_camels/main_classes/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/__init__.py
+-rw-rw-rw-   0        0        0     1706 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/camels_installer.py
+-rw-rw-rw-   0        0        0    28770 2023-06-29 11:51:05.000000 nomad_camels-0.1.2/nomad_camels/main_classes/device_class.py
+-rw-rw-rw-   0        0        0     3595 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/list_plot.py
+-rw-rw-rw-   0        0        0    11255 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/loop_step.py
+-rw-rw-rw-   0        0        0     3993 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/manual_control.py
+-rw-rw-rw-   0        0        0     1242 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/measurement_channel.py
+-rw-rw-rw-   0        0        0     7869 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/plot_2D.py
+-rw-rw-rw-   0        0        0    48782 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/main_classes/plot_widget.py
+-rw-rw-rw-   0        0        0    21225 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/main_classes/protocol_class.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.596291 nomad_camels-0.1.2/nomad_camels/manual_controls/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/manual_controls/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/manual_controls/get_manual_controls.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:37.086280 nomad_camels-0.1.2/nomad_camels/manual_controls/stage_control/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/manual_controls/stage_control/__init__.py
+-rw-rw-rw-   0        0        0    20282 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/manual_controls/stage_control/stage_control.py
+-rw-rw-rw-   0        0        0    12048 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/manual_controls/stage_control/ui_stage_control.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:37.096278 nomad_camels-0.1.2/nomad_camels/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/tests/__init__.py
+-rw-rw-rw-   0        0        0     3182 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/tests/instrument_management_test.py
+-rw-rw-rw-   0        0        0    20124 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/tests/protocol_test.py
+-rw-rw-rw-   0        0        0      768 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/tests/startup_test.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:37.116279 nomad_camels-0.1.2/nomad_camels/tools/
+-rw-rw-rw-   0        0        0     8502 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/tools/EPICS_driver_builder.py
+-rw-rw-rw-   0        0        0     5627 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/tools/VISA_builder.py
+-rw-rw-rw-   0        0        0    11374 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/tools/VISA_driver_builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/tools/__init__.py
+-rw-rw-rw-   0        0        0     8548 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/tools/databroker_exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:37.126280 nomad_camels-0.1.2/nomad_camels/ui_widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/__init__.py
+-rw-rw-rw-   0        0        0    20475 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/add_remove_table.py
+-rw-rw-rw-   0        0        0     9089 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/channels_check_table.py
+-rw-rw-rw-   0        0        0     1742 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/console_redirect.py
+-rw-rw-rw-   0        0        0     1204 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/drag_drop_tree_view.py
+-rw-rw-rw-   0        0        0     6522 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/options_run_button.py
+-rw-rw-rw-   0        0        0     2493 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/path_button_edit.py
+-rw-rw-rw-   0        0        0     3567 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/variable_tool_tip_box.py
+-rw-rw-rw-   0        0        0      451 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/ui_widgets/warn_popup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:37.187896 nomad_camels-0.1.2/nomad_camels/utility/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/__init__.py
+-rw-rw-rw-   0        0        0    15701 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/databroker_export.py
+-rw-rw-rw-   0        0        0     5204 2023-06-29 11:51:05.000000 nomad_camels-0.1.2/nomad_camels/utility/device_handling.py
+-rw-rw-rw-   0        0        0     1833 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/exception_hook.py
+-rw-rw-rw-   0        0        0      788 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/fit_variable_renaming.py
+-rw-rw-rw-   0        0        0    14745 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/utility/load_save_functions.py
+-rw-rw-rw-   0        0        0      938 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/load_save_helper_functions.py
+-rw-rw-rw-   0        0        0      867 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/number_formatting.py
+-rw-rw-rw-   0        0        0     1583 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/plot_placement.py
+-rw-rw-rw-   0        0        0     9893 2023-06-28 15:46:34.000000 nomad_camels-0.1.2/nomad_camels/utility/qthreads.py
+-rw-rw-rw-   0        0        0     2496 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/theme_changing.py
+-rw-rw-rw-   0        0        0      330 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/tqdm_progress_bar.py
+-rw-rw-rw-   0        0        0     2573 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/treeView_functions.py
+-rw-rw-rw-   0        0        0     2674 2023-06-28 15:48:04.000000 nomad_camels-0.1.2/nomad_camels/utility/update_camels.py
+-rw-rw-rw-   0        0        0    10431 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/nomad_camels/utility/variables_handling.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:53:36.466298 nomad_camels-0.1.2/nomad_camels.egg-info/
+-rw-rw-rw-   0        0        0     2101 2023-06-29 11:53:36.000000 nomad_camels-0.1.2/nomad_camels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5841 2023-06-29 11:53:36.000000 nomad_camels-0.1.2/nomad_camels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:53:36.000000 nomad_camels-0.1.2/nomad_camels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1340 2023-06-29 11:53:36.000000 nomad_camels-0.1.2/nomad_camels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-29 11:53:36.000000 nomad_camels-0.1.2/nomad_camels.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      925 2023-06-29 11:52:28.000000 nomad_camels-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1340 2023-06-28 14:51:20.000000 nomad_camels-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 11:53:37.187896 nomad_camels-0.1.2/setup.cfg
```

### Comparing `nomad_camels-0.1.1/LICENSE` & `nomad_camels-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/LICENSE.txt` & `nomad_camels-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/PKG-INFO` & `nomad_camels-0.1.2/nomad_camels.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: nomad_camels
-Version: 0.1.1
+Name: nomad-camels
+Version: 0.1.2
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
-Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 
 ```
```

### Comparing `nomad_camels-0.1.1/README.md` & `nomad_camels-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/CAMELS_start.py` & `nomad_camels-0.1.2/nomad_camels/CAMELS_start.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/MainApp_v2.py` & `nomad_camels-0.1.2/nomad_camels/MainApp_v2.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/EpicsFieldSignal.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/EpicsFieldSignal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/builder_helper_functions.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/builder_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/custom_function_signal.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/custom_function_signal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/evaluation_helper.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/evaluation_helper.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/helper_functions.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/make_catalog.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/make_catalog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/protocol_builder.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/protocol_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,18 @@
     for dev in protocol.get_used_devices():
         device = variables_handling.devices[dev]
         classname = device.ophyd_class_name
         config = copy.deepcopy(device.get_config())
         settings = copy.deepcopy(device.get_settings())
         additional_info = copy.deepcopy(device.get_additional_info())
         if 'connection' in settings:
-            settings.pop('connection')
+            conn = settings.pop('connection')
+            if 'type' in conn:
+                conn.pop('type')
+            settings.update(conn)
         if 'idn' in settings:
             settings.pop('idn')
         extra_settings = {}
         non_strings = []
         for key in settings:
             if key.startswith('!non_string!_'):
                 extra_settings[key.replace('!non_string!_', '')] = settings[key]
```

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/special_plan_stubs.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/special_plan_stubs.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/bluesky_handling/visa_signal.py` & `nomad_camels-0.1.2/nomad_camels/bluesky_handling/visa_signal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/commands/change_sequence.py` & `nomad_camels-0.1.2/nomad_camels/commands/change_sequence.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/device_add_dialog.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/device_add_dialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/helper_panels/enterTextDialog.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/helper_panels/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/instrument_config.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/instrument_installer.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/instrument_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/manage_instruments.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/manage_instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,23 @@
 
         self.installer = instrument_installer.Instrument_Installer()
         self.tabs.addTab(self.installer, 'Install Instruments')
 
         self.config_widget = instrument_config.Instrument_Config(active_instruments)
         self.tabs.addTab(self.config_widget, 'Configure Instruments')
 
-        settab = 1 if instrument_installer.getInstalledDevices() else 0
-        self.tabs.setCurrentIndex(settab)
         self.installer.instruments_updated.connect(self.config_widget.build_table)
 
         layout.addWidget(self.tabs, 0, 0)
         layout.addWidget(self.buttonBox, 1, 0)
 
+        self.show()
+        settab = 1 if instrument_installer.getInstalledDevices() else 0
+        self.tabs.setCurrentIndex(settab)
+
     def accept(self) -> None:
         """ """
         self.active_instruments = self.config_widget.get_config()
         super().accept()
 
     def closeEvent(self, a0: QCloseEvent) -> None:
         """
```

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/plot_definer.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/protocol_config.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/protocol_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/settings_window.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/settings_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/frontpanels/taskSelector.py` & `nomad_camels-0.1.2/nomad_camels/frontpanels/taskSelector.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/CAMELS.ico` & `nomad_camels-0.1.2/nomad_camels/graphics/CAMELS.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/CAMELS_Icon.png` & `nomad_camels-0.1.2/nomad_camels/graphics/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3` & `nomad_camels-0.1.2/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav` & `nomad_camels-0.1.2/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/camels-horizontal.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/camels-horizontal.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/camels-vertical.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/camels-vertical.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/camels_horizontal.png` & `nomad_camels-0.1.2/nomad_camels/graphics/camels_horizontal.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/camels_vertical.png` & `nomad_camels-0.1.2/nomad_camels/graphics/camels_vertical.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/dark.qss` & `nomad_camels-0.1.2/nomad_camels/graphics/dark.qss`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Icon.png` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Logo.png` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Logo.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Logo.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Logo.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_V1.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_V1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/CAMELS_v2.svg` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/CAMELS_v2.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/camels - Kopie.png` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/camels - Kopie.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/camels_free.png` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/camels_free.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/graphics/legacy/plus_sign.png` & `nomad_camels-0.1.2/nomad_camels/graphics/legacy/plus_sign.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/addDeviceDialog.py` & `nomad_camels-0.1.2/nomad_camels/gui/addDeviceDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/device_installer.py` & `nomad_camels-0.1.2/nomad_camels/gui/device_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/enterTextDialog.py` & `nomad_camels-0.1.2/nomad_camels/gui/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/fit_definer.py` & `nomad_camels-0.1.2/nomad_camels/gui/fit_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/for_loop.py` & `nomad_camels-0.1.2/nomad_camels/gui/for_loop.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/general_protocol_settings.py` & `nomad_camels-0.1.2/nomad_camels/gui/general_protocol_settings.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/gradient_descent_step.py` & `nomad_camels-0.1.2/nomad_camels/gui/gradient_descent_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/installer_window.py` & `nomad_camels-0.1.2/nomad_camels/gui/installer_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/instrument_config.py` & `nomad_camels-0.1.2/nomad_camels/gui/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/mainWindow_v2.py` & `nomad_camels-0.1.2/nomad_camels/gui/mainWindow_v2.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/pass_ask.py` & `nomad_camels-0.1.2/nomad_camels/gui/pass_ask.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/plot_definer.py` & `nomad_camels-0.1.2/nomad_camels/gui/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/plot_definer_2d.py` & `nomad_camels-0.1.2/nomad_camels/gui/plot_definer_2d.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/plot_options.py` & `nomad_camels-0.1.2/nomad_camels/gui/plot_options.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/protocol_view.py` & `nomad_camels-0.1.2/nomad_camels/gui/protocol_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/read_channels.py` & `nomad_camels-0.1.2/nomad_camels/gui/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/set_channels.py` & `nomad_camels-0.1.2/nomad_camels/gui/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/gui/settings_window.py` & `nomad_camels-0.1.2/nomad_camels/gui/settings_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/change_device_config.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/change_device_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/for_while_loops.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/for_while_loops.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/gradient_descent.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/if_step.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/if_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/make_step_of_type.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/make_step_of_type.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/nd_sweep.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/nd_sweep.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/prompt_loop_step.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/prompt_loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/read_channels.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/run_subprotocol.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/run_subprotocol.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/set_channels.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/set_value_popup.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/set_value_popup.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/set_variables.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/set_variables.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/simple_sweep.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/simple_sweep.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/loop_steps/wait_loop_step.py` & `nomad_camels-0.1.2/nomad_camels/loop_steps/wait_loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/camels_installer.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/camels_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/device_class.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/device_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,15 @@
         Returns
         -------
 
         """
         conn_old = self.connector
         if self.comboBox_connection_type.currentText() == 'Local VISA':
             self.connector = Local_VISA()
+        self.connector.load_settings(self.settings_dict)
         self.layout().replaceWidget(conn_old, self.connector)
         conn_old.deleteLater()
 
     def get_settings(self):
         """Updates the settings_dict with the current settings.
         Overwrite this function for each device to specify the settings.
         It is recommended to still call the super() method for the
@@ -629,14 +630,16 @@
         settings_dict :
             
 
         Returns
         -------
 
         """
+        if 'connection' in settings_dict:
+            settings_dict = settings_dict['connection']
         if 'resource_name' in settings_dict and settings_dict['resource_name'] in self.ports:
             self.comboBox_port.setCurrentText(settings_dict['resource_name'])
         if 'baud_rate' in settings_dict:
             self.lineEdit_baud.setText(str(settings_dict['baud_rate']))
         if 'read_termination' in settings_dict:
             self.lineEdit_in_term.setText(settings_dict['read_termination'].replace('\r', '\\r').replace('\n', '\\n'))
         if 'write_termination' in settings_dict:
```

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/list_plot.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/list_plot.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/loop_step.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/manual_control.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/manual_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/measurement_channel.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/measurement_channel.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/plot_2D.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/plot_2D.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/plot_widget.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/plot_widget.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/main_classes/protocol_class.py` & `nomad_camels-0.1.2/nomad_camels/main_classes/protocol_class.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/manual_controls/get_manual_controls.py` & `nomad_camels-0.1.2/nomad_camels/manual_controls/get_manual_controls.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/manual_controls/stage_control/stage_control.py` & `nomad_camels-0.1.2/nomad_camels/manual_controls/stage_control/stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/manual_controls/stage_control/ui_stage_control.py` & `nomad_camels-0.1.2/nomad_camels/manual_controls/stage_control/ui_stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tests/instrument_management_test.py` & `nomad_camels-0.1.2/nomad_camels/tests/instrument_management_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tests/protocol_test.py` & `nomad_camels-0.1.2/nomad_camels/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tests/startup_test.py` & `nomad_camels-0.1.2/nomad_camels/tests/startup_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tools/EPICS_driver_builder.py` & `nomad_camels-0.1.2/nomad_camels/tools/EPICS_driver_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tools/VISA_builder.py` & `nomad_camels-0.1.2/nomad_camels/tools/VISA_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tools/VISA_driver_builder.py` & `nomad_camels-0.1.2/nomad_camels/tools/VISA_driver_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/tools/databroker_exporter.py` & `nomad_camels-0.1.2/nomad_camels/tools/databroker_exporter.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/add_remove_table.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/add_remove_table.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/channels_check_table.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/channels_check_table.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/console_redirect.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/console_redirect.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/drag_drop_tree_view.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/drag_drop_tree_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/options_run_button.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/options_run_button.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/path_button_edit.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/path_button_edit.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/ui_widgets/variable_tool_tip_box.py` & `nomad_camels-0.1.2/nomad_camels/ui_widgets/variable_tool_tip_box.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/databroker_export.py` & `nomad_camels-0.1.2/nomad_camels/utility/databroker_export.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/device_handling.py` & `nomad_camels-0.1.2/nomad_camels/utility/device_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,18 @@
         # getting all the settings
         device = variables_handling.devices[dev]
         classname = device.ophyd_class_name
         config = copy.deepcopy(device.get_config())
         settings = copy.deepcopy(device.get_settings())
         additional_info = copy.deepcopy(device.get_additional_info())
         if 'connection' in settings:
-            settings.pop('connection')
+            conn = settings.pop('connection')
+            if 'type' in conn:
+                conn.pop('type')
+            settings.update(conn)
         if 'idn' in settings:
             settings.pop('idn')
         extra_settings = {}
         non_strings = []
         for key in settings:
             if key.startswith('!non_string!_'):
                 extra_settings[key.replace('!non_string!_', '')] = settings[key]
```

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/exception_hook.py` & `nomad_camels-0.1.2/nomad_camels/utility/exception_hook.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/fit_variable_renaming.py` & `nomad_camels-0.1.2/nomad_camels/utility/fit_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/load_save_functions.py` & `nomad_camels-0.1.2/nomad_camels/utility/load_save_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/load_save_helper_functions.py` & `nomad_camels-0.1.2/nomad_camels/utility/load_save_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/number_formatting.py` & `nomad_camels-0.1.2/nomad_camels/utility/number_formatting.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/plot_placement.py` & `nomad_camels-0.1.2/nomad_camels/utility/plot_placement.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/qthreads.py` & `nomad_camels-0.1.2/nomad_camels/utility/qthreads.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/theme_changing.py` & `nomad_camels-0.1.2/nomad_camels/utility/theme_changing.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/treeView_functions.py` & `nomad_camels-0.1.2/nomad_camels/utility/treeView_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/update_camels.py` & `nomad_camels-0.1.2/nomad_camels/utility/update_camels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels/utility/variables_handling.py` & `nomad_camels-0.1.2/nomad_camels/utility/variables_handling.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels.egg-info/PKG-INFO` & `nomad_camels-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: nomad-camels
-Version: 0.1.1
+Name: nomad_camels
+Version: 0.1.2
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
-Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 
 ```
```

### Comparing `nomad_camels-0.1.1/nomad_camels.egg-info/SOURCES.txt` & `nomad_camels-0.1.2/nomad_camels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/nomad_camels.egg-info/requires.txt` & `nomad_camels-0.1.2/nomad_camels.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.1/pyproject.toml` & `nomad_camels-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)",
-    "Operating System :: Microsoft :: Windows",
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies= {file = ["requirements.txt"]}
 
 [tool.setuptools.packages.find]
```

### Comparing `nomad_camels-0.1.1/requirements.txt` & `nomad_camels-0.1.2/requirements.txt`

 * *Files identical despite different names*

