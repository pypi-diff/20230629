# Comparing `tmp/pedal-2.5.2.tar.gz` & `tmp/pedal-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.5.2.tar", last modified: Wed Jun 14 16:24:51 2023, max compression
+gzip compressed data, was "pedal-2.5.3.tar", last modified: Thu Jun 29 18:03:45 2023, max compression
```

## Comparing `pedal-2.5.2.tar` & `pedal-2.5.3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.045547 pedal-2.5.2/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.2/LICENSE
--rw-rw-rw-   0        0        0     2981 2023-06-14 16:24:51.046546 pedal-2.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.862276 pedal-2.5.2/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.858280 pedal-2.5.2/pedal/
--rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.5.2/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.878274 pedal-2.5.2/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.2/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.5.2/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.2/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.2/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.5.2/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.2/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3254 2023-05-26 21:11:25.000000 pedal-2.5.2/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.2/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.889302 pedal-2.5.2/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.2/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.2/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.5.2/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.5.2/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.2/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.2/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.899304 pedal-2.5.2/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7971 2023-06-14 15:23:15.000000 pedal-2.5.2/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.2/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    24546 2023-06-14 15:43:56.000000 pedal-2.5.2/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.2/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.5.2/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.920224 pedal-2.5.2/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     9342 2023-05-26 21:10:34.000000 pedal-2.5.2/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/errors.py
--rw-rw-rw-   0        0        0    21081 2023-06-09 14:02:52.000000 pedal-2.5.2/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.2/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     8008 2023-06-10 15:13:23.000000 pedal-2.5.2/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.2/pedal/core/location.py
--rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.5.2/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.2/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.2/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.2/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.935551 pedal-2.5.2/pedal/environments/
--rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.2/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3060 2023-05-26 21:12:20.000000 pedal-2.5.2/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9587 2023-05-26 21:13:02.000000 pedal-2.5.2/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.2/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.2/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.2/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3684 2023-05-26 21:13:56.000000 pedal-2.5.2/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     3201 2023-06-14 16:08:09.000000 pedal-2.5.2/pedal/environments/terminal.py
--rw-rw-rw-   0        0        0     6423 2023-06-08 18:48:18.000000 pedal-2.5.2/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.941546 pedal-2.5.2/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.2/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.2/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.2/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.953545 pedal-2.5.2/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.2/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.2/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.2/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.2/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.2/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.2/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.2/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.966547 pedal-2.5.2/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.2/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.2/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     1504 2023-05-26 21:58:00.000000 pedal-2.5.2/pedal/resolvers/export.py
--rw-rw-rw-   0        0        0     1753 2023-05-26 21:21:28.000000 pedal-2.5.2/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.2/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.2/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.2/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.2/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.982547 pedal-2.5.2/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.2/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.5.2/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.2/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.2/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10695 2023-06-10 15:55:30.000000 pedal-2.5.2/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.989546 pedal-2.5.2/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.2/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.2/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.2/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.2/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.2/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    10128 2023-05-27 15:46:15.000000 pedal-2.5.2/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.2/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.2/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.2/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.2/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.997547 pedal-2.5.2/pedal/source/
--rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.2/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/source/constants.py
--rw-rw-rw-   0        0        0     5913 2023-06-10 16:42:17.000000 pedal-2.5.2/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.2/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.011547 pedal-2.5.2/pedal/tifa/
--rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.2/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.5.2/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.2/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.2/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.2/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.2/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.5.2/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42475 2023-06-08 18:43:14.000000 pedal-2.5.2/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.018548 pedal-2.5.2/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.2/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.2/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.026546 pedal-2.5.2/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.2/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.2/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.2/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.2/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.2/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.2/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51761 2023-05-27 15:40:45.000000 pedal-2.5.2/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    14912 2023-06-08 18:43:02.000000 pedal-2.5.2/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.2/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.044546 pedal-2.5.2/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.2/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.5.2/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0     9918 2023-06-10 16:39:35.000000 pedal-2.5.2/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.2/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.5.2/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.2/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.2/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-06-14 16:24:51.047546 pedal-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-06-14 16:22:25.000000 pedal-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.967597 pedal-2.5.3/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-06-29 18:03:45.967597 pedal-2.5.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.680593 pedal-2.5.3/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3759 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-29 18:03:45.000000 pedal-2.5.3/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.675594 pedal-2.5.3/pedal/
+-rw-rw-rw-   0        0        0      382 2023-06-28 02:39:12.000000 pedal-2.5.3/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.698594 pedal-2.5.3/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.3/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13562 2023-06-23 17:14:33.000000 pedal-2.5.3/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.3/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.3/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:54.000000 pedal-2.5.3/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.3/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3316 2023-06-23 17:04:45.000000 pedal-2.5.3/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.3/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.712595 pedal-2.5.3/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.3/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.3/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:06.000000 pedal-2.5.3/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:21.000000 pedal-2.5.3/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    22520 2023-06-20 15:55:10.000000 pedal-2.5.3/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.3/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.3/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.722594 pedal-2.5.3/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     7971 2023-06-14 15:23:15.000000 pedal-2.5.3/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.3/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    24755 2023-06-28 02:41:46.000000 pedal-2.5.3/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.3/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:14.000000 pedal-2.5.3/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.790594 pedal-2.5.3/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     9411 2023-06-23 17:10:49.000000 pedal-2.5.3/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    21541 2023-06-29 17:23:52.000000 pedal-2.5.3/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.3/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     8147 2023-06-29 16:44:20.000000 pedal-2.5.3/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.3/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13819 2023-06-29 17:23:24.000000 pedal-2.5.3/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.3/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.3/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.3/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.813635 pedal-2.5.3/pedal/environments/
+-rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.3/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:06.000000 pedal-2.5.3/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9910 2023-06-23 17:16:42.000000 pedal-2.5.3/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.3/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.3/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.3/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:25.000000 pedal-2.5.3/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     4941 2023-06-29 17:29:51.000000 pedal-2.5.3/pedal/environments/terminal.py
+-rw-rw-rw-   0        0        0     6673 2023-06-23 16:04:44.000000 pedal-2.5.3/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.820623 pedal-2.5.3/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.3/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.3/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.3/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.836627 pedal-2.5.3/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.3/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.3/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.3/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.3/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.3/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.3/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.3/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.851619 pedal-2.5.3/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.3/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.3/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:54.000000 pedal-2.5.3/pedal/resolvers/export.py
+-rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:54.000000 pedal-2.5.3/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.3/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.3/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.3/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.3/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.871620 pedal-2.5.3/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.3/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    18299 2023-06-28 02:55:07.000000 pedal-2.5.3/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.3/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.3/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:28.000000 pedal-2.5.3/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.880620 pedal-2.5.3/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.3/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.3/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.3/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.3/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.3/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10132 2023-06-20 15:21:24.000000 pedal-2.5.3/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.3/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.3/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.3/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.3/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.891593 pedal-2.5.3/pedal/source/
+-rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.3/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     6539 2023-06-29 16:45:23.000000 pedal-2.5.3/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.3/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.911599 pedal-2.5.3/pedal/tifa/
+-rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.3/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-06-23 17:11:58.000000 pedal-2.5.3/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.3/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.3/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.3/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.3/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:23.000000 pedal-2.5.3/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42742 2023-06-23 17:17:45.000000 pedal-2.5.3/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.925599 pedal-2.5.3/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.3/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.3/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.938593 pedal-2.5.3/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.3/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.3/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.3/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.3/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.3/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.3/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51452 2023-06-23 17:23:01.000000 pedal-2.5.3/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    15022 2023-06-23 16:26:55.000000 pedal-2.5.3/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.3/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:03:45.965594 pedal-2.5.3/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.3/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:40.000000 pedal-2.5.3/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0    10068 2023-06-23 16:57:49.000000 pedal-2.5.3/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.3/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:07.000000 pedal-2.5.3/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.3/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.3/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.3/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-06-29 18:03:45.969594 pedal-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-06-23 16:27:25.000000 pedal-2.5.3/setup.py
```

### Comparing `pedal-2.5.2/LICENSE` & `pedal-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/PKG-INFO` & `pedal-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.2
+Version: 2.5.3
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.5.2/Pedal.egg-info/PKG-INFO` & `pedal-2.5.3/Pedal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.2
+Version: 2.5.3
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.5.2/Pedal.egg-info/SOURCES.txt` & `pedal-2.5.3/Pedal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/README.rst` & `pedal-2.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/__init__.py` & `pedal-2.5.3/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/classes.py` & `pedal-2.5.3/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/commands.py` & `pedal-2.5.3/pedal/assertions/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,26 @@
     * Specify exact score for each test case, individually | list[str]
     * Specify exact score for each test case, with single value | str
     * Specify total score for all test cases, no partial credit | False, using `score`
     * Specify total score for all test cases, divide by # of cases passed | True, using `score`
 
     Args:
         assert_function: Override the assert function (defaults to assert_equal)
-        function ():
-        *tests ():
+        function (str): The name of the function to test.
+        *tests (): The test cases to run. Each test case is a tuple of the input/output pairs.
         else_message (str): The message to present as a positive if the
              tests all pass.
+        else_message_template (str): The template for the else_message, to be formatted.
         score (str): The score to give overall/per test case, depending on
             partial_credit.
-        partial_credit (bool or str or list[str]): Whether or not to give credit for
+        partial_credit (bool or str or list[str]): Whether to give credit for
             each unit test as a percentage of the whole (True), or to only give
             points for passing all the tests (False). Defaults to False.
             If a list is passed, those scores will be used per test case.
+        context (Sandbox or CommandBlock): The context to run the function in.
         **kwargs ():
 
     Returns:
 
     """
     if assert_function is None:
         assert_function = assert_equal
```

### Comparing `pedal-2.5.2/pedal/assertions/feedbacks.py` & `pedal-2.5.3/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/functions.py` & `pedal-2.5.3/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/organizers.py` & `pedal-2.5.3/pedal/assertions/organizers.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,95 +35,19 @@
 TODO: Rename? And expand on.
 with assert_group('test_add') as test_add_group:
 
 if assert_unit_tests('function_name', FUNCTION_CASES):
 
 
 '''
-
-
+from pedal.assertions.feedbacks import AssertionBreak
 from pedal.core.report import MAIN_REPORT
-from pedal.assertions.setup import (_setup_assertions, AssertionException,
-                                    _add_relationships, _add_phase)
+from pedal.assertions.setup import (_setup_assertions, _add_relationships, _add_phase)
 from functools import wraps
 
-
-class _finish_section:
-    def __init__(self, number, *functions):
-        if isinstance(number, int):
-            self.number = number
-        else:
-            self.number = -1
-            functions = [number] + list(functions)
-        self.functions = functions
-        for function in functions:
-            self(function, False)
-
-    def __call__(self, f=None, quiet=True):
-        if f is not None:
-            f()
-        if quiet:
-            print("\tNEXT SECTION")
-
-    def __enter__(self):
-        pass
-
-    def __exit__(self, x, y, z):
-        print("\tNEXT SECTION")
-        # return wrapped_f
-
-
-def finish_section(number, *functions, next_section=False):
-    """
-
-    Args:
-        number:
-        *functions:
-        next_section:
-
-    Returns:
-
-    """
-    if len(functions) == 0:
-        x = _finish_section(number, *functions)
-        x()
-    else:
-        result = _finish_section(number, *functions)
-        if next_section:
-            print("\tNEXT SECTION")
-        return result
-
-
-def section(*args):
-    '''
-    TODO: Deprecate?
-    '''
-    _setup_assertions(MAIN_REPORT)
-    def wrap(f):
-        """
-
-        Args:
-            f:
-
-        Returns:
-
-        """
-        _add_phase(phase_name, _handle_entry)
-        MAIN_REPORT['assertions']['phases'].append((section_number, f))
-        return f
-    section_number = -1
-    if len(args) >= 1 and callable(args[0]):
-        if len(args) >= 2:
-            section_number = args[1]
-        return wrap(args[0])
-    elif len(args) >= 1:
-        section_number = args[0]
-    return wrap
-
-
 def phase(phase_name, before=None, after=None):
     '''
     
     Args:
         phase_name (str): The name of the phase this function will belong to.
         before (list[str] or str): the name(s) of any phases that this phase
                                    should be before.
@@ -176,15 +100,15 @@
 
         """
         old_exception_state = MAIN_REPORT['assertions']['exceptions']
         MAIN_REPORT['assertions']['exceptions'] = True
         value = None
         try:
             value = f(*args, **kwargs)
-        except AssertionException:
+        except AssertionBreak:
             pass
         MAIN_REPORT['assertions']['exceptions'] = old_exception_state
         return value
     return wrapped
 
 
 def try_all(f):
```

### Comparing `pedal-2.5.2/pedal/assertions/runtime.py` & `pedal-2.5.3/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/setup.py` & `pedal-2.5.3/pedal/assertions/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Helper functions and basic setup routines for the entire module.
 """
-
+from pedal.assertions.feedbacks import AssertionBreak
 from pedal.core.report import MAIN_REPORT
 from pedal.core.commands import set_correct
 from pedal.sandbox.exceptions import SandboxStudentCodeException
 from pedal.utilities.sorting import topological_sort
 
 
 def resolve_all(set_successful=False, no_phases_is_success=False, report=MAIN_REPORT):
@@ -33,15 +33,15 @@
                 phase_success = False
         if not phase_success:
             break
         
     #for f in report.feedback:
     #    print("\t", f, f.mistake, f.misconception)
     if not report['assertions']['failures'] and phase_success and set_successful:
-        set_success()
+        set_successful(report)
     
     _reset_phases(report)
 
 
 def _add_phase(phase_name, function, report=MAIN_REPORT):
     phase_functions = report['assertions']['phase_functions']
     phases = report['assertions']['phases']
```

### Comparing `pedal-2.5.2/pedal/assertions/static.py` & `pedal-2.5.3/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/assertions/unittest.py` & `pedal-2.5.3/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/cait/ast_helpers.py` & `pedal-2.5.3/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/cait/ast_map.py` & `pedal-2.5.3/pedal/cait/ast_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,17 +284,14 @@
         for key, value in other.class_table.items():
             for sub_value in value:
                 self.add_class_to_sym_table(str(key), sub_value.astNode)
 
     @property
     def match_lineno(self):
         """
-        Args:
-            first (bool): Whether to use the first found match, or the last one.
-
         Returns:
             int: the line number this match started on
         """
         values = [v.lineno for v in self.mappings.values()
                   if v.lineno is not None]
         if not values:
             return -1
```

### Comparing `pedal-2.5.2/pedal/cait/cait_api.py` & `pedal-2.5.3/pedal/cait/cait_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
 def find_asts(node_name: str, student_code=None, report=MAIN_REPORT):
     """
     Find all occurrences of the given AST node, based on the name of the AST
     node (e.g., `"For"` or `"FunctionDef"`).
 
     Args:
-        node_type: the string representing the "type" of node to look for
+        node_name: the string representing the "type" of node to look for
         student_code (str): Optionally, different code to parse and search.
         report: defaults to MAIN_REPORT unless another one is given.
 
     Returns:
         a list of Ast Nodes (cait_nodes) of self that are of the specified type (including self if self
                 meets that criteria)
```

### Comparing `pedal-2.5.2/pedal/cait/cait_node.py` & `pedal-2.5.3/pedal/cait/cait_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,10 +656,13 @@
     def locate(self):
         """
         Returns:
             pedal.core.Location: The location of this node.
         """
         return Location(self.astNode.lineno, col=self.astNode.col_offset)
 
+    def to_json(self):
+        return str(self)
+
 
 AST_SINGLE_FUNCTIONS = ["ctx_name", "op_name"]
 AST_ARRAYS_OF_FUNCTIONS = ["ops_names"]
```

### Comparing `pedal-2.5.2/pedal/cait/find_node.py` & `pedal-2.5.3/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/cait/stretchy_tree_matching.py` & `pedal-2.5.3/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/command_line/command_line.py` & `pedal-2.5.3/pedal/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/command_line/mocks.py` & `pedal-2.5.3/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/command_line/modes.py` & `pedal-2.5.3/pedal/command_line/modes.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,16 @@
                     #print(list(global_data.keys()), file=x)
                     if 'MAIN_REPORT' in global_data:
                         if not global_data['MAIN_REPORT'].resolves:
                             if resolver in global_data:
                                 resolution = global_data[resolver]()
                             # TODO: Need more elegance/configurability here
                             elif self.config.resolver == 'resolve':
-                                exec("from pedal.resolvers.simple import resolve", global_data)
-                                resolution = global_data["resolve"]()
+                                exec("from pedal.resolvers import print_resolve", global_data)
+                                resolution = global_data["print_resolve"]()
                         else:
                             resolution = global_data['MAIN_REPORT'].resolves[-1]
                 except Exception as e:
                     error = e
         actual_output = captured_output.getvalue()
         self.result = BundleResult(global_data, actual_output, error, resolution)
 
@@ -254,23 +254,26 @@
             for event in events:
                 if instructor_code is None:
                     instructor_code_for_this_run = event['on_run']
                 else:
                     instructor_code_for_this_run = instructor_code
                 link_selections = progsnap._merge('link_selections', {})
                 new_submission = Submission(
-                    main_file='answer.py', main_code=event['submission_code'].decode('utf-8'),
+                    main_file='answer.py',
+                    main_code=event['submission_code'] if isinstance(event['submission_code'], str) else
+                        event['submission_code'].decode('utf-8'),
                     instructor_file='instructor.py',
                     #files={'cisc106.py': 'from bakery import *'},
                     execution=dict(client_timestamp=event['client_timestamp'],
                                    event_id=event['event_id']),
                     #user=dict(email=event['student_email'],
                     #          first=event['student_first'],
                     #          last=event['student_last']),
-                    user={key: event[key] for key in link_selections['Subject'].values()},
+                    user={key: event[key] for key in link_selections['Subject'].values()}
+                    if 'Subject' in link_selections else {'id': event['subject_id']},
                     assignment=dict(name=event['assignment_name'],
                                     url=event['assignment_url']),
                 )
                 self.submissions.append(Bundle(self.config, instructor_code_for_this_run, new_submission))
             # raise ValueError("TODO: ProgSnap DB files not yet supported")
             # Progsnap Zip
         elif script_file_extension in ('.zip',):
@@ -486,15 +489,15 @@
             if bundle.result.error:
                 raise bundle.result.error
             # This info is not sent to the output target, just to stdout
             print(bundle.submission.instructor_file,
                   bundle.submission.main_file,
                   bundle.submission.user.get('student_email') if bundle.submission.user else 'Unknown User',
                   bundle.submission.assignment.get('name') if bundle.submission.assignment else 'Unknown Assignment',
-                  1 if bundle.result.resolution.success else
+                  1 if bundle.result.resolution.correct else
                   bundle.result.resolution.score,
                   sep=", ", end="")
 
 
 class SandboxPipeline(AbstractPipeline):
     """ Run the given script in a sandbox. """
```

### Comparing `pedal-2.5.2/pedal/command_line/report.py` & `pedal-2.5.3/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/command_line/verify.py` & `pedal-2.5.3/pedal/command_line/verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """
     Parses an out file, which is based on ``ini`` files. They have pretty
     basic syntax. The difference from what configparser is that indentation
     is preserved in multiline values. We don't support comments and a number
     of other features, but who needs 'em.
 
     Args:
-        contents (str): The contents of the out file.
+        path (str): The path to the inifile that will be read.
 
     Returns:
         dict[str, dict[str, str]]: The constructed out sections=>{fields=>data}
     """
     sections = {'default': {}}
     current_section = 'default'
     current_key = None
```

### Comparing `pedal-2.5.2/pedal/core/commands.py` & `pedal-2.5.3/pedal/core/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 
 
 def log(*items, sep=" ", **kwargs):
     """
     Attach logging information to the Report as a piece of feedback.
 
     Args:
+        sep: The separator to use between items (defaults to space).
         items (Any): Any set of values to log information about. Will be
             converted to strings using `str` if not already strings.
 
     Returns:
 
     """
     kwargs.setdefault('category', Feedback.CATEGORIES.SYSTEM)
```

### Comparing `pedal-2.5.2/pedal/core/environment.py` & `pedal-2.5.3/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/errors.py` & `pedal-2.5.3/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/feedback.py` & `pedal-2.5.3/pedal/core/feedback.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 Simple data classes for storing feedback to present to learners.
 """
 
 __all__ = ['Feedback', 'FeedbackKind', 'FeedbackCategory',
            "CompositeFeedbackFunction",
            "FeedbackResponse"]
 
-from pedal.core.formatting import FeedbackFieldWrapper
+from pedal.core.formatting import wrap_fields
 from pedal.core.location import Location
 from pedal.core.report import MAIN_REPORT
 from pedal.core.feedback_category import FeedbackKind, FeedbackCategory, FeedbackStatus
 
 PEDAL_DEVELOPERS = ["Austin Cory Bart <acbart@udel.edu>",
                     "Luke Gusukuma <lukesg08@vt.edu>"]
 
 
+class FeedbackRegistry:
+    def __init__(self):
+        self._registered_feedback = {}
+
+
 class Feedback:
     """
     A class for storing raw feedback.
 
     Attributes:
         label (str): An internal name for this specific piece of feedback. The
             label should be an underscore-separated string following the same
@@ -143,14 +148,15 @@
 
     activate: bool
     _status: str
     _exception: Exception or None
     _met_condition: bool
     _stored_args: tuple
     _stored_kwargs: dict
+    _override_backups = None
 
     resolved_score = None
     unused_message = None
 
     #MAIN_REPORT
 
     def __init__(self, *args, label=None,
@@ -312,16 +318,15 @@
 
         Returns:
             str: The message for this feedback.
         """
         if self.message is not None:
             return self.message
         if self.message_template is not None:
-            fields = {field: FeedbackFieldWrapper(field, value, self.report.format)
-                      for field, value in self.fields.items()}
+            fields = wrap_fields(self.report.format, self.fields)
             return self.message_template.format(**fields)
         return self.DEFAULT_FEEDBACK_MESSAGE
 
     def _get_else_message(self):
         """
         Determines the appropriate value for the else_message. It will attempt
         to use this instance's else_message, but if it's not available then it will
@@ -332,16 +337,15 @@
 
         Returns:
             str: The else_message for this feedback.
         """
         if self.else_message is not None:
             return self.else_message
         if self.else_message_template is not None:
-            fields = {field: FeedbackFieldWrapper(field, value, self.report.format)
-                      for field, value in self.fields.items()}
+            fields = wrap_fields(self.report.format, self.fields)
             return self.else_message_template.format(**fields)
         return self.DEFAULT_ELSE_MESSAGE
 
     def _get_justification(self, met_condition):
         """
         Determines the appropriate value for the justification. It first checks
         if there is a `justification` already present, but if it's not available
@@ -364,16 +368,15 @@
                 return met if met_condition else unmet
         if self.justification_template is not None:
             if isinstance(self.justification_template, str):
                 template = "The following condition was not met: " + self.justification_template
             else:
                 met, unmet = self.justification_template
                 template = met if met_condition else unmet
-            fields = {field: FeedbackFieldWrapper(field, value, self.report.format)
-                      for field, value in self.fields.items()}
+            fields = wrap_fields(self.report.format, self.fields)
             return template.format(**fields)
         return self.DEFAULT_JUSTIFICATION_MESSAGE
 
     def _get_child_feedback(self, feedback, active):
         """ Callback function that Reports will call when a new piece of
         feedback is being considered. By default, does nothing. This is useful
         for :py:class:`pedal.core.group.FeedbackGroup`, most other feedbacks
@@ -461,14 +464,30 @@
             'version': self.version,
             'fields': self._fields_to_json(),
             'justification': self.justification,
             'priority': self.priority,
             'location': self.location.to_json() if self.location is not None else None
         }
 
+    @classmethod
+    def override(cls, report=MAIN_REPORT, **fields):
+        if cls._override_backups is None:
+            cls._override_backups = {}
+        for field, new_value in fields.items():
+            if field not in cls._override_backups:
+                cls._override_backups[field] = getattr(cls, field)
+            setattr(cls, field, new_value)
+        report.override_feedback(cls)
+
+    @classmethod
+    def _restore_overrides(cls):
+        for field, old_value in cls._override_backups.items():
+            setattr(cls, field, old_value)
+        cls._override_backups.clear()
+
 
 class FeedbackResponse(Feedback):
     """
     An extension of :py:class:`~pedal.core.feedback.Feedback` that is meant
     to indicate that the class should not have any condition behind its
     response.
     """
```

### Comparing `pedal-2.5.2/pedal/core/feedback_category.py` & `pedal-2.5.3/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/final_feedback.py` & `pedal-2.5.3/pedal/core/final_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/formatting.py` & `pedal-2.5.3/pedal/core/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,18 @@
                 break
         return value.__format__(format_spec)
 
 # TODO: Convert Formatter into HtmlFormatter, and then make Formatter text by
 #       default.
 
 
+def wrap_fields(formatter, fields):
+    return {field: FeedbackFieldWrapper(field, value, formatter) for field, value in fields.items()}
+
+
 class Formatter:
     """ Utility class for wrapping a feedback message with HTML or other
             extra information. Can be subclassed by a different environment and
             attached to a Report, in order to change how we create feedback. """
 
     available = ['exception', 'filename', 'frame', 'traceback',
                  # 'html_code', 'html_div', 'html_pre', 'html_span', 'html_tag',
```

### Comparing `pedal-2.5.2/pedal/core/location.py` & `pedal-2.5.3/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/report.py` & `pedal-2.5.3/pedal/core/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,19 +73,21 @@
         self.group_names = {}
         self.hooks = {}
         self.class_hooks = {}
         self.submission = None
         self.format = Formatter()
         self.result = None
         self.resolves = []
+        self.overridden_feedbacks = set()
 
     def clear(self):
         """
         Resets the entire report back to its starting form,
         including deleting any attached submissions, tool data, and feedbacks.
+        It will also reset any overridden fields of feedback classes.
         However, it will not affect class hooks.
         """
         self.feedback.clear()
         self.ignored_feedback.clear()
         self.suppressions.clear()
         self.suppressed_labels.clear()
         self.hiddens.clear()
@@ -94,20 +96,29 @@
         self.groups.clear()
         self.group_names.clear()
         self.hooks.clear()
         self.submission = None
         self.result = None
         self.resolves.clear()
         self.format = Formatter()
+        self.clear_overridden_feedback()
 
     def full_clear(self):
         """ This totally resets the report, including any class hooks. """
         self.clear()
         self.class_hooks.clear()
 
+    def clear_overridden_feedback(self):
+        for feedback in self.overridden_feedbacks:
+            feedback._restore_overrides()
+        self.overridden_feedbacks.clear()
+
+    def override_feedback(self, feedback_class):
+        self.overridden_feedbacks.add(feedback_class)
+
     def contextualize(self, submission):
         """
         Attach the given submission to this report.
 
         Args:
             submission (:py:class:`pedal.core.submission.Submission`): The
                 submission to attach to this report.
```

### Comparing `pedal-2.5.2/pedal/core/resolver.py` & `pedal-2.5.3/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/scoring.py` & `pedal-2.5.3/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/submission.py` & `pedal-2.5.3/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/core/tool.py` & `pedal-2.5.3/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/environments/__init__.py` & `pedal-2.5.3/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/environments/blockpy.py` & `pedal-2.5.3/pedal/environments/blockpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 """
 from pedal import verify
 from pedal.core.environment import Environment
 from pedal.core.formatting import HtmlFormatter
 from pedal.core.report import MAIN_REPORT
 from pedal.sandbox import run, get_sandbox, set_input, start_trace
 from pedal.tifa import tifa_analysis
-from pedal.resolvers.simple import resolve
+from pedal.resolvers import print_resolve
 from pedal.resolvers.statistics import resolve as stats_resolve
 
 
 class BlockPyEnvironment(Environment):
     """
     Configures the BlockPy programming environment.
     """
@@ -77,15 +77,15 @@
         else:
             if trace:
                 start_trace()
             student = run(report=report, threaded=threaded)
             student.threaded = threaded
         self.fields = {
             'student': student,
-            'resolve': resolve,
+            'resolve': print_resolve,
             'stats_resolve': stats_resolve
         }
 
 
 setup_environment = BlockPyEnvironment
 
 """
```

### Comparing `pedal-2.5.2/pedal/environments/gradescope.py` & `pedal-2.5.3/pedal/environments/gradescope.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,22 +134,25 @@
 @make_resolver
 def detailed_resolver(report=MAIN_REPORT, priority_key=by_priority):
     """ Group by category, provide all the non-muted activated feedback """
     pass
 
 
 @make_resolver
-def resolve(report=MAIN_REPORT, customize_failure_message= None, leaderboard=None, priority_key=by_priority):
+def resolve(report=MAIN_REPORT, customize_failure_message= None, leaderboard=None):
     """
 
     TODO: Support some hidden tests for instructors
 
     Args:
-        report:
-        custom_success_message:
+        leaderboard: A list of data for the leaderboard, or a function to generate a leaderboard.
+        customize_failure_message: A function that takes in the final feedback object in order to manipulate its
+            settings. This is useful for changing the message of a feedback object to be more specific to the
+            needs of the instructor.
+        report: The report to resolve.
     """
     final = full_resolve(report)
     tests = []
     for feedback in final.used:
         test = {"name": feedback.title}
         message = feedback.message if feedback else (feedback.else_message or "Correct")
         if feedback.title != message:
```

### Comparing `pedal-2.5.2/pedal/environments/jupyter.py` & `pedal-2.5.3/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/environments/nbgrader.py` & `pedal-2.5.3/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/environments/sandbox.py` & `pedal-2.5.3/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/environments/standard.py` & `pedal-2.5.3/pedal/environments/standard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """
 A simple environment for quickly running Pedal code.
 """
 
 import sys
 
-from pedal.assertions import resolve_all
 from pedal.core.environment import Environment
 from pedal.core.report import MAIN_REPORT
 from pedal.source import verify
 from pedal.cait import parse_program
-from pedal.sandbox.commands import run
 from pedal.resolvers import simple
 from pedal.sandbox import run, get_sandbox, set_input, start_trace
 from pedal.tifa import tifa_analysis
-from pedal.resolvers.simple import resolve
 
 
 def parse_argv():
     """ Retrieve fields from sys.argv """
     if len(sys.argv) == 2:
         main_file = sys.argv[1]
         with open(main_file) as main_file_handle:
@@ -62,15 +59,15 @@
         else:
             if trace:
                 start_trace()
             student = run(report=report, threaded=threaded)
             student.threaded = threaded
         self.fields = {
             'student': student,
-            'resolve': resolve
+            'resolve': self.print_resolve
         }
         self.set_correct = set_correct or set_success
 
     def print_resolve(self, *args, **kwargs):
         """
         Trivial formatter for resolver, just dumps the
         Title/Label/Score/Message. Any arguments are forwarded to
```

### Comparing `pedal-2.5.2/pedal/environments/vpl.py` & `pedal-2.5.3/pedal/environments/vpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pedal.core.report import MAIN_REPORT
 from pedal.sandbox import run, get_sandbox, set_input, start_trace
 from pedal.source.sections import FeedbackSourceSection
 from pedal.tifa import tifa_analysis
 from pedal.resolvers.simple import resolve as simple_resolve, by_priority
 from pedal.resolvers.sectional import resolve as original_sectional_resolve
 from pedal.core.formatting import Formatter
+from pedal.core.location import Location
+from pedal.utilities.text import inject_line
 
 try:
     import tabulate
 except ImportError:
     tabulate = None
 
 
@@ -89,15 +91,17 @@
 ## TODO: Check if file exists
 
 class VPLFormatter(Formatter):
 
     def pre(self, text):
         return "\n".join([">" + line for line in text.split("\n")])
 
-    def python_code(self, code):
+    def python_code(self, code, focus=None):
+        if isinstance(focus, Location):
+            code = inject_line(code, focus.line + 1, " " * (focus.col - 1) + "^" * (focus.end_col - focus.col))
         return self.pre(code)
 
     def python_expression(self, code):
         return code
 
     def filename(self, filename):
         return filename
```

### Comparing `pedal-2.5.2/pedal/extensions/microbit.py` & `pedal-2.5.3/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/extensions/plotting.py` & `pedal-2.5.3/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/__init__.py` & `pedal-2.5.3/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/feedbacks.py` & `pedal-2.5.3/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/graders.py` & `pedal-2.5.3/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/loader.py` & `pedal-2.5.3/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/pool.py` & `pedal-2.5.3/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/questions.py` & `pedal-2.5.3/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/questions/setup.py` & `pedal-2.5.3/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/resolvers/__init__.py` & `pedal-2.5.3/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/resolvers/core.py` & `pedal-2.5.3/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/resolvers/export.py` & `pedal-2.5.3/pedal/resolvers/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import ast
 import dataclasses
 import datetime
 
+from pedal.core.feedback import Feedback
 from pedal.sandbox.result import is_sandbox_result
-import json
-
 from pedal.types import new_types
 
+# acbart: Provide JSONEncoder for Skulpt compatibility
+try:
+    from json import JSONEncoder
+except AttributeError:
+    class JSONEncoder:
+        pass
+
 
-class PedalJSONEncoder(json.JSONEncoder):
+class PedalJSONEncoder(JSONEncoder):
     """
     Custom JSON Encoder to handle weird Pedal values nested in Feedback Functions,
     including things like SandboxResult.
     """
     def _iterencode(self, o, markers=None):
         if is_sandbox_result(o):
             return super()._iterencode(o._actual_value, markers)
         else:
             return super()._iterencode(o, markers)
 
+    def iterencode(self, o, _one_shot=False):
+        if is_sandbox_result(o):
+            return super().iterencode(o._actual_value, _one_shot)
+        else:
+            return super().iterencode(o, _one_shot)
+
     def default(self, obj):
         if hasattr(obj, 'to_json'):
             return obj.to_json()
         if isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
             return obj.isoformat()
         elif isinstance(obj, datetime.timedelta):
             return (datetime.datetime.min + obj).time().isoformat()
@@ -35,13 +47,15 @@
         except:
             return '<not serializable>'
 
 
 def clean_json(obj):
     if is_sandbox_result(obj):
         return clean_json(obj._actual_value)
+    elif isinstance(obj, Feedback):
+        return clean_json(obj.to_json())
     if isinstance(obj, dict):
         return {clean_json(key): clean_json(value) for key, value in obj.items()}
     elif isinstance(obj, (set, list, tuple)):
         return [clean_json(value) for value in obj]
     else:
         return obj
```

### Comparing `pedal-2.5.2/pedal/resolvers/full.py` & `pedal-2.5.3/pedal/resolvers/full.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 @make_resolver
 def resolve(report=MAIN_REPORT, priority_key=by_priority):
     """
     This function is used to resolve the feedback objects in the report into a FinalFeedback object.
 
     Args:
+        priority_key: The function used to sort the feedback objects.
         report: The report to resolve.
 
     Returns:
         FinalFeedback: The resolved feedback.
     """
 
     # Prepare feedbacks
```

### Comparing `pedal-2.5.2/pedal/resolvers/sectional.py` & `pedal-2.5.3/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/resolvers/simple.py` & `pedal-2.5.3/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/resolvers/statistics.py` & `pedal-2.5.3/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/__init__.py` & `pedal-2.5.3/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/commands.py` & `pedal-2.5.3/pedal/sandbox/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,14 +452,28 @@
     """ Loads the data for the given mocked module, if available (otherwise raises exception) """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     if hasattr(sandbox.modules, module_name):
         return getattr(sandbox.modules, module_name)
     raise ValueError(f"Unknown Sandbox Module: `{module_name}`")
 
 
+def get_python_errors(report=MAIN_REPORT):
+    """
+    Retrieves any runtime or syntax errors from the report.
+    Args:
+        report:
+
+    Returns:
+        list[Feedback]: A list of runtime and syntax errors that were detected
+    """
+    for feedback in report.feedback:
+        if feedback.category == 'runtime' or feedback.category == 'syntax':
+            yield feedback
+
+
 class CommandBlock:
     """
     Context Manager for creating instructor blocks of code that will
     be shown together to the student.
 
     TODO: What about named points where you can "rewind" the state to?
     """
```

### Comparing `pedal-2.5.2/pedal/sandbox/data.py` & `pedal-2.5.3/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/exceptions.py` & `pedal-2.5.3/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/feedbacks.py` & `pedal-2.5.3/pedal/sandbox/feedbacks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
 Generic runtime exception feedback class.
+
+TODO: Use the FeedbackRegistry to properly dispatch the appropriate runtime_error type, instead of reusing the base object
 """
+from pedal.core.formatting import wrap_fields
 from pedal.core.location import Location
 from pedal.core.report import MAIN_REPORT
 from pedal.sandbox.data import format_contexts
 from pedal.utilities.exceptions import KeyError, get_exception_name
 from pedal.core.feedback import FeedbackResponse
 from pedal.sandbox import TOOL_NAME
 from pedal.utilities.text import add_indefinite_article
 
-RUNTIME_ERROR_MESSAGE_HEADER = (
-    "{context_message}\n"
-    "{exception_name} occurred:\n\n"
-    "{exception_message}\n\n"
-    "{traceback_message}\n"
-)
-
 
 class runtime_error(FeedbackResponse):
     """
     Used to create all runtime errors.
 
     Attributes:
         exception (Exception): The original exception.
@@ -37,190 +33,185 @@
 
     """
     tool = TOOL_NAME
     category = FeedbackResponse.CATEGORIES.RUNTIME
     kind = FeedbackResponse.KINDS.MISTAKE
     justification = "A runtime error occurred during execution of some code."
     version = '1.1.0'
-    message_template = RUNTIME_ERROR_MESSAGE_HEADER
+    constant_fields = {"suggestion": ""}
+    message_template = (
+        "{context_message}\n"
+        "{exception_name_proper} occurred:\n\n"
+        "{exception_message}\n\n"
+        "{traceback_preamble}{traceback_message}\n"
+        "{suggestion_message}"
+    )
 
     def __init__(self, exception, context, traceback, location, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         exception_name = get_exception_name(exception)
         exception_name_proper = add_indefinite_article(exception_name)
         exception_message = str(exception)
         exception_message = exception_message[0].upper() + exception_message[1:] if exception_message else ""
         if type(exception) not in EXCEPTION_FF_MAP:
             title = exception_name
         else:
             title = EXCEPTION_FF_MAP[type(exception)].title
         location = Location(location)
         traceback_stack = traceback.build_traceback()
-        traceback_message = traceback.format_traceback(traceback_stack, report.format)
-        if not traceback_message:
-            traceback_message = ""
-        else:
-            traceback_message = f"The traceback was:\n{traceback_message}"
+        traceback_message = traceback.format_traceback(traceback_stack, report.format) or ""
+        traceback_preamble = f"The traceback was:\n" if traceback_message else ""
         context_message = format_contexts(context, report.format)
         fields = {'exception': exception,
-                  'exception_name': exception_name_proper,
+                  'exception_name': exception_name,
+                  'exception_name_proper': exception_name_proper,
                   'exception_message': report.format.exception(exception_message),
                   'location': location,
                   'traceback': traceback,
+                  'traceback_preamble': traceback_preamble,
                   'traceback_stack': traceback_stack,
                   'traceback_message': traceback_message,
                   'context': context,
                   'context_message': context_message}
+        fields['suggestion_message'] = self.constant_fields['suggestion'].format(**wrap_fields(report.format, fields))
         super().__init__(fields=fields, title=title,
                          location=location, **kwargs)
 
 
 class type_error(runtime_error):
     """ Type Error """
     title = "Type Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "Type errors occur when you use an operator or "
+    constant_fields = {'suggestion': "Type errors occur when you use an operator or "
                         "function on the wrong type of value. For example, "
                         "using `+` to add to a list (instead of `.append`), or "
                         "dividing a string by a number.\n\n"
                         "Suggestion: To fix a type error, you should trace "
                         "through your code. Make sure each expression has the "
-                        "type you expect it to have.")
+                        "type you expect it to have."}
 
 
 class name_error(runtime_error):
     """ Runtime NameError """
     title = "Name Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "A name error means you have used a variable that has "
+    constant_fields = {'suggestion': "A name error means you have used a variable that has "
                         "no value.  You may have a typo, so check the "
                         "spelling. Or, you may have forgotten to initialize a "
                         "variable.\n\n"
                         "Suggestion: Trace your code and make sure each "
-                        "variable was set before it was read.")
+                        "variable was set before it was read."}
 
 
 class value_error(runtime_error):
     """ Runtime ValueError """
     title = "Value Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "A ValueError occurs when you pass the wrong type of "
+    constant_fields = {'suggestion': "A ValueError occurs when you pass the wrong type of "
                         "value to a function. For example, you try to convert "
                         "a string without numbers to an integer (like "
                         "`int('Five')`).\n\n"
                         "Suggestion: Read the error message to see which "
                         "function had the issue. Check what type the function "
                         "expects. Then trace your code to make sure you pass "
-                        "in that type.")
+                        "in that type."}
 
 
 class attribute_error(runtime_error):
     """ Runtime AttributeError """
     title = "Attribute Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "An AttributeError means you used an attribute or "
+    constant_fields = {'suggestion': "An AttributeError means you used an attribute or "
                         "method that does not exist. For example, you wrote "
                         "`text.delete()` even though there is no `delete` "
                         "method.\n\n"
                         "Suggestion: Make sure that you spelled the method or "
                         "attribute correctly. Then, trace your code to check "
-                        "that the dot's left expression is the correct type.")
+                        "that the dot's left expression is the correct type."}
 
 
 class index_error(runtime_error):
     """ Runtime IndexError """
     title = "Index Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "An IndexError means that you indexed past the end of "
+    constant_fields = {'suggestion': "An IndexError means that you indexed past the end of "
                         "a string or a list.  For example, if you access index "
                         "5 in a list with 3 items.\n\n"
                         "Suggestion: Remember that the first position in a "
                         "list or string is 0. Often, you will be off by just "
                         "one index position, so check your math. Also, make "
-                        "sure the list or string has the right value.")
+                        "sure the list or string has the right value."}
 
 
 class zero_division_error(runtime_error):
     """ Runtime ZeroDivisionError """
     title = "Division by Zero Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "A ZeroDivisionError means you divided by 0. The "
+    constant_fields = {'suggestion': "A ZeroDivisionError means you divided by 0. The "
                         "denominator (the right side of a division expression) "
                         "cannot be 0.\n\n"
                         "Suggestion: Check that you are dividing by the "
                         "correct value. Or, you might need to add an `if` "
-                        "statement to handle the zero case.")
+                        "statement to handle the zero case."}
 
 
 class indentation_error(runtime_error):
     """ Syntax IndentationError """
     title = "Indentation Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "An IndentationError means you have not indented your "
+    constant_fields = {'suggestion': "An IndentationError means you have not indented your "
                         "code correctly. You have too many or too few spaces.\n\n"
                         "Suggestion: Check the line number, and the lines "
                         "before and after. Check the body of each function "
                         "definition, `if` statement, and `for` loop. Remember, "
                         "all the statements INSIDE of a body have the same "
-                        "indentation.")
+                        "indentation."}
 
 
 class import_error(runtime_error):
     """ Runtime ImportError """
     title = "Import Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "An ImportError means you tried to import a module "
+    constant_fields = {'suggestion': "An ImportError means you tried to import a module "
                         "that does not exist. You might have a typo or a file "
                         "might be in the wrong location.\n\n"
                         "Suggestion: Check the spelling and capitalization of "
                         "the module's name. If you are importing a file, then "
-                        "check that it is in the correct folder.")
+                        "check that it is in the correct folder."}
 
 
 class io_error(runtime_error):
     """ Runtime IOError """
     title = "Input/Output Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "An IOError means you tried to open a file that was "
+    constant_fields = {'suggestion': "An IOError means you tried to open a file that was "
                         "not available.\n\n"
                         "Suggestion: Make sure that the file is in the "
                         "correct folder. Then, make sure you spelled the "
-                        "filename correctly.")
+                        "filename correctly."}
 
 
 class key_error(runtime_error):
     """ Runtime KeyError """
     title = "Key Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "A KeyError means you accessed a non-existent key in "
+    constant_fields = {'suggestion': "A KeyError means you accessed a non-existent key in "
                         "a dictionary.\n\n"
                         "Suggestion: First, check that you spelled the key "
                         "correctly. Make sure the key has the right type and "
                         "value. Then, check that the dictionary actually has "
-                        "that key.")
+                        "that key."}
 
 
 class memory_error(runtime_error):
     """ Runtime MemoryError """
     title = "Memory Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "A MemoryError means your program ran out of mental "
+    constant_fields = {'suggestion': "A MemoryError means your program ran out of mental "
                         "space.\n\n"
                         "Suggestion: You might have an infinite loop. Or, you "
-                        "might not be filtering your data enough.")
+                        "might not be filtering your data enough."}
 
 
 class timeout_error(runtime_error):
     """ Runtime TimeoutError """
     title = "Timeout Error"
-    message_template = (RUNTIME_ERROR_MESSAGE_HEADER + "\n" +
-                        "A TimeoutError means your program took too long to "
+    constant_fields = {'suggestion': "A TimeoutError means your program took too long to "
                         "run.\n\n"
                         "Suggestion: Check that you do not have an infinite "
-                        "loop.")
+                        "loop."}
 
 
 EXCEPTION_FF_MAP = {
     TypeError: type_error,
     NameError: name_error,
     ValueError: value_error,
     AttributeError: attribute_error,
```

### Comparing `pedal-2.5.2/pedal/sandbox/library/designer.py` & `pedal-2.5.3/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/library/matplotlib.py` & `pedal-2.5.3/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/library/microbit.py` & `pedal-2.5.3/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/library/turtles.py` & `pedal-2.5.3/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/mocked.py` & `pedal-2.5.3/pedal/sandbox/mocked.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         _default_builtins = __builtins__
 
 ORIGINAL_BUILTINS = {
     'globals': _default_builtins['globals'],
     'locals': _default_builtins['locals'],
     'open': _default_builtins['open'],
     'input': _default_builtins['input'],
-    'print': _default_builtins['print'],
+    'print': _default_builtins.get('print'),
     'exec': _default_builtins.get('exec', _disabled_exec),
     'eval': _default_builtins.get('eval', _disabled_eval),
     'compile': _default_builtins.get('compile', _disabled_compile),
     'exit': disabled_builtin('exit'),
     '__import__': _default_builtins['__import__']
 }
```

### Comparing `pedal-2.5.2/pedal/sandbox/result.py` & `pedal-2.5.3/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/sandbox.py` & `pedal-2.5.3/pedal/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/timeout.py` & `pedal-2.5.3/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/sandbox/tracer.py` & `pedal-2.5.3/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/source/__init__.py` & `pedal-2.5.3/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/source/feedbacks.py` & `pedal-2.5.3/pedal/source/feedbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 Feedback functions of the Source module
 """
 import traceback as tb
 from pedal.core.commands import feedback
 from pedal.core.feedback import FeedbackResponse
 from pedal.core.location import Location
 from pedal.core.report import MAIN_REPORT
-from pedal.utilities.exceptions import ExpandedTraceback
+from pedal.utilities.exceptions import ExpandedTraceback, get_exception_name
 from pedal.source.constants import TOOL_NAME
 from pedal.utilities.system import IS_AT_LEAST_PYTHON_310
+from pedal.utilities.text import add_indefinite_article
+from pedal.core.formatting import wrap_fields
 
 
 class SourceFeedback(FeedbackResponse):
     """ Base class of all Feedback functions for Source Tool """
     category = feedback.CATEGORIES.SYNTAX
     kind = feedback.KINDS.MISTAKE
     tool = TOOL_NAME
@@ -55,19 +57,20 @@
         super().__init__(fields=fields, group=group, **kwargs)
 
 
 class syntax_error(SourceFeedback):
     """ Generic feedback for any kind of syntax error. """
     muted = False
     title = "Syntax Error"
+    constant_fields = {"suggestion": "Suggestion: Check line {lineno:line}, the line before it, and the line "
+                                     "after it. Ignore blank lines."}
     message_template = ("Bad syntax on line {lineno:line}.\n\n"
-                        "{traceback_message}\n"
-                        "{suggestion_message}"
-                        "Suggestion: Check line {lineno:line}, the line "
-                        "before it, and the line after it. Ignore blank lines.")
+                        "{traceback_preamble}{traceback_message}\n"
+                        "{exception_message}"
+                        "{suggestion_message}")
     version = '1.0.0'
     justification = "Syntax error was triggered while calling ast.parse"
 
     def __init__(self, line, filename, code, col_offset,
                  exception, exc_info, enhance=True, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         files = report.submission.get_files_lines()
@@ -75,45 +78,47 @@
             files[filename] = code.split("\n")
         if report.submission is not None:
             lines = report.submission.get_lines()
             line_offsets = report.submission.line_offsets
         else:
             lines = code.split("\n")
             line_offsets = {}
+        exception_name = get_exception_name(exception)
+        exception_name_proper = add_indefinite_article(exception_name)
         traceback = ExpandedTraceback(exception, exc_info, False,
                                       [report.submission.instructor_file],
                                       line_offsets, [filename], lines, files)
         traceback_stack = traceback.build_traceback()
         traceback_message = traceback.format_traceback(traceback_stack, report.format)
-        if traceback_message:
-            traceback_message = f"The traceback was:\n{traceback_message}"
-        else:
-            traceback_message = ""
+        traceback_preamble = f"The traceback was:\n" if traceback_message else ""
         #if not enhance:
         #    self.message_template = "{traceback_message}\n{exception_message}"
         line_offset = line_offsets.get(filename, 0)
-        suggestion_message = self.make_suggestion_message(exception)
+        exception_message = self.make_exception_message(exception)
         fields = {'lineno': line + line_offset,
                   'filename': filename,
                   'offset': col_offset,
                   'exception': exception,
-                  'exception_message': str(exception),
+                  'exception_name': exception_name,
+                  'exception_name_proper': exception_name_proper,
+                  'exception_message': exception_message,
                   'traceback': traceback,
                   'traceback_stack': traceback_stack,
-                  'traceback_message': traceback_message,
-                  'suggestion_message': suggestion_message}
+                  'traceback_preamble': traceback_preamble,
+                  'traceback_message': traceback_message}
         location = Location(line=line + line_offset, col=col_offset, filename=filename)
+        fields['suggestion_message'] = self.constant_fields['suggestion'].format(**wrap_fields(report.format, fields))
         super().__init__(fields=fields, location=location, **kwargs)
 
-    def make_suggestion_message(self, exception):
+    def make_exception_message(self, exception):
         """ Generate a suggestion message based on the exception. """
         base_message = exception.msg
         base_message = base_message.capitalize() + "."
-        if base_message == "Invalid syntax.":
-            return ""
+        #if base_message == "Invalid syntax.":
+        #    return ""
         return base_message + "\n"
 
 
 class incorrect_number_of_sections(SourceFeedback):
     """ Incorrect number of sections """
     title = "Incorrect Number of Sections"
     message_template = ("Incorrect number of sections in your file. "
@@ -127,14 +132,16 @@
 
 # TODO: TabError
 
 
 class indentation_error(syntax_error):
     """ Generic feedback for indentation errors. """
     title = "Indentation Error"
+    constant_fields = {'suggestion': "Suggestion: Check line {lineno:line}, the line before it, and the "
+                                     "line after it. Ignore blank lines."}
     message_template = ("Bad indentation on line {lineno:line} or adjacent line.\n\n"
-                        "{traceback_message}\n"
+                        "{traceback_preamble}{traceback_message}\n"
+                        "{exception_message}"
                         "{suggestion_message}"
-                        "Suggestion: Check line {lineno:line}, the line "
-                        "before it, and the line after it. Ignore blank lines.")
+                        )
     version = '1.0.0'
     justification = "Indentation error was triggered while calling ast.parse"
```

### Comparing `pedal-2.5.2/pedal/source/sections.py` & `pedal-2.5.3/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/source/source.py` & `pedal-2.5.3/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/__init__.py` & `pedal-2.5.3/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/commands.py` & `pedal-2.5.3/pedal/tifa/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,32 +37,35 @@
 
 
 def get_issues(category, report=MAIN_REPORT):
     """
 
     Args:
         category (str or Feedback): The category of Issues to retrieve.
+        report: The report to get feedback from (defaults to the MAIN_REPORT).
 
     Returns:
         list[Feedback]: The feedback functions triggered for this issue.
     """
     if not isinstance(category, str):
         category = category.__name__
     if not report[TIFA_TOOL_NAME]['latest']:
         tifa_analysis(report=report)
     latest = report[TIFA_TOOL_NAME]['latest']
     return latest.issues.get(category, [])
 
 
 def tifa_provide_module_type(name: str, fields, report=MAIN_REPORT):
     """
+    Gives TIFA the type definition for a module.
 
     Args:
-        name:
-        fields:
+        name: The name of the module to provide a type for.
+        fields: A `ModuleType` or `dict` of fields to provide.
+        report: The report to attach this feedback to (defaults to the MAIN_REPORT).
 
     Returns:
 
     """
     if not isinstance(fields, ModuleType):
         fields = ModuleType(name, fields)
     report[TIFA_TOOL_NAME]['types']['modules'][name] = fields
```

### Comparing `pedal-2.5.2/pedal/tifa/contexts.py` & `pedal-2.5.3/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/feedbacks.py` & `pedal-2.5.3/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/identifier.py` & `pedal-2.5.3/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/settings.py` & `pedal-2.5.3/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/state.py` & `pedal-2.5.3/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/tifa/tifa_core.py` & `pedal-2.5.3/pedal/tifa/tifa_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,15 +327,16 @@
         """
         Update the variable with the given name to now have the new type.
 
         Args:
             name (str): The unqualified name of the variable. The variable will
                         be assumed to be in the current scope.
             store_type (Type): The new type of this variable.
-            position: The location that this store occurred at
+            position: The location that this store occurred at.
+            force_create: Used to force the creation of a new variable, even if the variable already exists.
         Returns:
             State: The new state of the variable.
         """
         if position is None:
             position = self.locate()
         full_name = self._scope_chain_str(name)
         current_path = self.path_chain[0]
```

### Comparing `pedal-2.5.2/pedal/tifa/tifa_visitor.py` & `pedal-2.5.3/pedal/tifa/tifa_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,15 @@
         statements, including Names, Tuples/Lists, Subscripts, and
         Attributes.
 
         Args:
             target (ast.AST): The target AST Node.
             target_type (Type): The new TIFA type.
             operation (None | ast.op): The AugAssign operation, if there is one
+            store_with_read: Whether to store the variable as a read variable, or just a write variable.
 
         Returns:
 
         """
         if isinstance(target, ast.Name):
             original_value_type = self.visit(target)
             if operation:
@@ -536,17 +537,21 @@
         self._visit_collection_loop(node)
         # Handle ifs, unless they're blank (None in Skulpt :)
         if node.ifs:
             self.visit_statements(node.ifs)
 
     def fill_in_location(self, node, source_node):
         node.lineno = source_node.lineno
-        node.end_lineno = source_node.end_lineno
         node.col_offset = source_node.col_offset
-        node.end_col_offset = source_node.end_col_offset
+        if IS_AT_LEAST_PYTHON_38:
+            node.end_lineno = source_node.end_lineno
+            node.end_col_offset = source_node.end_col_offset
+        else:
+            node.end_lineno = source_node.lineno
+            node.end_col_offset = source_node.col_offset
 
     def visit_Dict(self, node):
         """
         Three types of dictionaries
         - empty
         - uniform type
         - record
```

### Comparing `pedal-2.5.2/pedal/types/builtin.py` & `pedal-2.5.3/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/types/library/cs1_curriculum.py` & `pedal-2.5.3/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/types/library/designer.py` & `pedal-2.5.3/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/types/library/matplotlib.py` & `pedal-2.5.3/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/types/library/microbit.py` & `pedal-2.5.3/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/types/new_types.py` & `pedal-2.5.3/pedal/types/new_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1274,43 +1274,38 @@
 class LiteralValue:
     """
     Special class flag that can be used to check if the type was defined as a literal.
     """
     value: any
     parents: list
 
+    def __init__(self, value):
+        self.value = value
+
     def promote(self):
         return self.parents[0]
 
     def clone(self):
         return self.__class__(self.value)
 
 
 class LiteralBool(LiteralValue, BoolType):
     value: str
     singular_name = "a boolean"
     plural_name = "booleans"
     fields = {}
     parents = [BoolType()]
 
-    def __init__(self, value):
-        super().__init__()
-        self.value = value
-
 
 class LiteralStr(LiteralValue, StrType):
     value: str
     singular_name = "a string"
     plural_name = "strings"
     fields = {}
 
-    def __init__(self, value):
-        super().__init__(value == "")
-        self.value = value
-
     @property
     def parents(self):
         return [StrType(self.is_empty)]
 
     def promote(self):
         return StrType(self.is_empty)
 
@@ -1320,35 +1315,27 @@
     singular_name = "an integer"
     plural_name = "integers"
     immutable = True
     value: int
     fields = {}
     parents = [IntType()]
 
-    def __init__(self, value):
-        super().__init__()
-        self.value = value
-
     def __str__(self):
         return f"LiteralInteger[{self.value}]"
 
 
 class LiteralFloat(LiteralValue, Type):
     name = "LiteralFloat"
     singular_name = "a float"
     plural_name = "floats"
     immutable = True
     value: int
     fields = {}
     parents = [FloatType()]
 
-    def __init__(self, value):
-        super().__init__()
-        self.value = value
-
     def __str__(self):
         return f"LiteralFloat[{self.value}]"
 
 
 # Types that support ordering
 NUMERIC_TYPES = frozenset([
     NumType, IntType, FloatType, BoolType, LiteralInt, LiteralFloat
```

### Comparing `pedal-2.5.2/pedal/types/normalize.py` & `pedal-2.5.3/pedal/types/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,20 @@
     """
     # Already a Pedal Type
     if isinstance(type_expression, str) and type_expression in PEDAL_TYPE_NAMES:
         return PEDAL_TYPE_NAMES[type_expression]()
     if isinstance(type_expression, Type):
         return type_expression
     # What if it's a builtin type function?
-    if isinstance(type_expression, (type, dynamic_python_types.GenericAlias)):
+    if isinstance(type_expression, type) or (IS_AT_LEAST_PYTHON_39 and isinstance(type_expression, dynamic_python_types.GenericAlias)):
         if type_expression.__name__ in TYPE_STRINGS:
             return get_generic_type(type_expression, evaluate_name)
         if evaluate_name:
             type_object = unbox_sandbox_if_needed(evaluate_name(type_expression.__name__))
-            if isinstance(type_object, (type, dynamic_python_types.GenericAlias)):
+            if isinstance(type_object, type) or (IS_AT_LEAST_PYTHON_39 and isinstance(type_object, dynamic_python_types.GenericAlias)):
                 if fields and hasattr(type_object, '__dataclass_fields__'):
                     return ClassType(type_object.__name__, {
                         field.name: normalize_type(field.type, evaluate_name)
                         for field in fields(type_object)
                     })
                 # TODO: Fix this ugly ugly hack!
                 try:
```

### Comparing `pedal-2.5.2/pedal/types/operations.py` & `pedal-2.5.3/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/__init__.py` & `pedal-2.5.3/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/ast_tools.py` & `pedal-2.5.3/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/comparisons.py` & `pedal-2.5.3/pedal/utilities/comparisons.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 SET_GENERATOR_TYPES = (type({}.keys()), type({}.values()), type({}.items()))
 
 LIST_GENERATOR_TYPES = (type(map(bool, [])), type(filter(bool, [])),
                         type(range(0)), type(reversed([])), type(zip()),
                         type(enumerate([])))
 
 
-def _split_into_lolos(a_string) -> 'List[List[str]]':
+def _split_into_lolos(a_string):
     """
     Splits the given string into a list of list of strings, based on new lines.
 
     Args:
         a_string: The string to split
 
     Returns: The list of list of strings
```

### Comparing `pedal-2.5.2/pedal/utilities/dictionaries.py` & `pedal-2.5.3/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/exceptions.py` & `pedal-2.5.3/pedal/utilities/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Utilities for handling exceptions across all of Pedal.
 """
 from textwrap import indent
 import traceback
 import os
 import sys
 
-from pedal.utilities.system import IS_AT_LEAST_PYTHON_310
+from pedal.utilities.system import IS_AT_LEAST_PYTHON_310, IS_AT_LEAST_PYTHON_311
 from pedal.core.location import Location
 
 BuiltinKeyError = KeyError
 
 _backup_stdout = sys.stdout
 
 
@@ -257,14 +257,16 @@
             for frame in traceback_stack
         ])
         if not traceback_message:
             return None
         return formatter.traceback(traceback_message)
 
     def format_line(self, formatter, frame):
-        if IS_AT_LEAST_PYTHON_310:
+        if IS_AT_LEAST_PYTHON_311:
             end_offset = frame.end_colno+1 if frame.lineno == frame.end_lineno else len(frame._line)
             # Note: Need to use _line because in 3.10 and above, the line gets stripped.
             # https://github.com/python/cpython/commit/5644c7b3ffd49bed58dc095be6e6148e0bb4431e
             line = frame._line if frame._line is not None else ''
             return formatter.python_code(line, focus=Location(0, frame.colno+1, 0, end_offset))
+        elif IS_AT_LEAST_PYTHON_310:
+            return formatter.python_code(frame._line if frame._line is not None else '')
         return formatter.python_code(frame.line if frame.line is not None else '')
```

### Comparing `pedal-2.5.2/pedal/utilities/files.py` & `pedal-2.5.3/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/operators.py` & `pedal-2.5.3/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/progsnap.py` & `pedal-2.5.3/pedal/utilities/progsnap.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,32 @@
                     'X-Code.OnRun': 'on_run'
                 }
             },
             link_primary={
                 'user': 'student_email'
             },
         ),
+        'blockpy_consenting': dict(
+            link_filters={
+                # '': [
+                #     ("LinkAssignment.`X-URL` LIKE ?", "%read%"),
+                #     ("LinkAssignment.`X-URL` LIKE ?", "%quiz%"),
+                # ]
+            },
+            link_selections={
+                'Assignment': {
+                    'X-Name': 'assignment_name',
+                    'X-URL': 'assignment_url',
+                    'X-Code.OnRun': 'on_run'
+                }
+            },
+            link_primary={
+                'user': 'SubjectID'
+            },
+        ),
     }
 
     def set_profile(self, profile):
         if profile not in self.PROFILES:
             raise ValueError(f"Unknown ProgSnap Profile specified: {profile}")
         self.profile = profile
 
@@ -131,40 +149,53 @@
         link_selections = self._merge('link_selections', link_selections)
         link_filters = self._merge('link_filters', link_filters)
         # Setup data
         tables = ['MainTable']
         filters = []  # "MainTable.EventType=?"
         selections = ['MainTable.EventID', 'MainTable.ClientTimestamp']
         fields = ['event_id', 'client_timestamp']
+        if 'Subject' not in link_selections:
+            selections.append('MainTable.SubjectID')
+            fields.append('subject_id')
         data = []
         # Add in event filters
         for column, value_filter in event_filter.items():
             if isinstance(value_filter, str):
                 filters.append(f"MainTable.`{column}`=?")
                 data.append(value_filter)
         # Add in code
         if with_code:
             tables.append("CodeState")
             filters.append(f"MainTable.CodeStateID=CodeState.ID")
             selections.append("CodeState.Contents as submission_code")
             fields.append("submission_code")
         # Add in all needed link tables
         for table in (link_filters.keys() | link_selections.keys()):
-            tables.append('Link' + table)
-            filters.append(f"MainTable.`{table}ID`=Link{table}.`{table}Id`")
+            if table:
+                tables.append('Link' + table)
+                filters.append(f"MainTable.`{table}ID`=Link{table}.`{table}Id`")
         # Add in link table filters
         for table, table_filters in link_filters.items():
-            for column, value_filter in table_filters.items():
-                if isinstance(value_filter, str):
-                    # TODO: Make this more robust
-                    if "%" in value_filter:
-                        filters.append(f"Link{table}.`{column}` LIKE ?")
-                    else:
-                        filters.append(f"Link{table}.`{column}`=?")
-                    data.append(value_filter)
+            # Blank string is generic filters
+            if table == "":
+                if isinstance(table_filters, str):
+                    table_filters = [table_filters]
+                for value_filter, v in table_filters:
+                    filters.append(value_filter)
+                    data.append(v)
+            else:
+                # Otherwise, assume link table -> column filter
+                for column, value_filter in table_filters.items():
+                    if isinstance(value_filter, str):
+                        # TODO: Make this more robust
+                        if "%" in value_filter:
+                            filters.append(f"Link{table}.`{column}` LIKE ?")
+                        else:
+                            filters.append(f"Link{table}.`{column}`=?")
+                        data.append(value_filter)
         # Add in Contextual tables
         for table, table_selections in link_selections.items():
             for column, alias in table_selections.items():
                 selections.append(f"Link{table}.`{column}` AS {alias}")
                 fields.append(alias)
         # Prepare actual filter query string
         if filters:
```

### Comparing `pedal-2.5.2/pedal/utilities/sorting.py` & `pedal-2.5.3/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/text.py` & `pedal-2.5.3/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/pedal/utilities/types.py` & `pedal-2.5.3/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.2/setup.py` & `pedal-2.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.5.2',
+    version='2.5.3',
     python_requires='>=3.7',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

