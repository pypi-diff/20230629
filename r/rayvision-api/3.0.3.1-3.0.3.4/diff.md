# Comparing `tmp/rayvision_api-3.0.3.1.tar.gz` & `tmp/rayvision_api-3.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayvision_api-3.0.3.1.tar", last modified: Thu May  4 12:40:08 2023, max compression
+gzip compressed data, was "dist/rayvision_api-3.0.3.4.tar", last modified: Thu Jun 29 11:07:58 2023, max compression
```

## Comparing `rayvision_api-3.0.3.1.tar` & `rayvision_api-3.0.3.4.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      258 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1121 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      286 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/CHANGES.md
--rw-rw-rw-   0 root         (0) root         (0)    11363 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1679 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/dev_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      611 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5166 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      781 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs/rayvision_api/
--rw-rw-rw-   0 root         (0) root         (0)      274 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/core_module.rst
--rw-rw-rw-   0 root         (0) root         (0)     3925 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/first_look.rst
--rw-rw-rw-   0 root         (0) root         (0)      737 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/installation_guide.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/connect.rst
--rw-rw-rw-   0 root         (0) root         (0)     2340 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/constants.rst
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/core.rst
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/exception.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/fields.rst
--rw-rw-rw-   0 root         (0) root         (0)      161 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/main/utils.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs/rayvision_api/operators/
--rw-rw-rw-   0 root         (0) root         (0)      171 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/operators/env.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/operators/query.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/operators/tag.rst
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/operators/task.rst
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/operators/user.rst
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/rayvision_api.operators.rst
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/rayvision_api.task.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs/rayvision_api/task/
--rw-rw-rw-   0 root         (0) root         (0)      279 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/task/check.rst
--rw-rw-rw-   0 root         (0) root         (0)      230 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs/rayvision_api/task/handle.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs_en/
--rw-rw-rw-   0 root         (0) root         (0)   544618 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs_en/RAYVISION Render API V3.0.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/docs_zh/
--rw-rw-rw-   0 root         (0) root         (0)   248917 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/docs_zh/瑞云渲染APIV4.0.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/examples/
--rw-rw-rw-   0 root         (0) root         (0)     7637 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/examples/api_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/init_pycharm_setup.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api/
--rw-rw-rw-   0 root         (0) root         (0)      440 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5167 2023-04-25 08:34:12.000000 rayvision_api-3.0.3.1/rayvision_api/connect.py
--rw-rw-rw-   0 root         (0) root         (0)     2955 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.1/rayvision_api/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7419 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.1/rayvision_api/core.py
--rw-rw-rw-   0 root         (0) root         (0)     4796 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/file_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     4989 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/json_operator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api/operators/
--rw-rw-rw-   0 root         (0) root         (0)      541 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5167 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/operators/env.py
--rw-rw-rw-   0 root         (0) root         (0)    22719 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.1/rayvision_api/operators/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3044 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/operators/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     6150 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/operators/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/operators/transmit.py
--rw-rw-rw-   0 root         (0) root         (0)     6396 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/operators/user.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/abandonTask.yaml
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/add.yaml
--rw-rw-rw-   0 root         (0) root         (0)       78 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/addTaskLabel.yaml
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/addUserPluginConfig.yaml
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/createTask.yaml
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/delete.yaml
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/deleteTask.yaml
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/deleteTaskLabel.yaml
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/deleteUserPluginConfig.yaml
--rw-rw-rw-   0 root         (0) root         (0)      383 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/editUserPluginConfig.yaml
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/fullSpeedRendering.yaml
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/getOutputUserDirFile.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/getRaySyncUserKey.yaml
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/getServerInfo.yaml
--rw-rw-rw-   0 root         (0) root         (0)      110 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/getTaskList.yaml
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/getUserPluginConfig.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/list.yaml
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/loadTaskProcessImg.yaml
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/loadingFrameThumbnail.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/queryAllFrameStats.yaml
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/queryAnalyseErrorDetail.yaml
--rw-rw-rw-   0 root         (0) root         (0)       39 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/queryPlatforms.yaml
--rw-rw-rw-   0 root         (0) root         (0)      110 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/querySoftwareDetail.yaml
--rw-rw-rw-   0 root         (0) root         (0)      105 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/queryTaskFrames.yaml
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/queryTaskInfo.yaml
--rw-rw-rw-   0 root         (0) root         (0)      125 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/recommitTaskFrames.yaml
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/recommitTasks.yaml
--rw-rw-rw-   0 root         (0) root         (0)      102 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/schema_v1.yaml
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/setDefaultUserPluginConfig.yaml
--rw-rw-rw-   0 root         (0) root         (0)      116 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/setTaskOverTimeStop.yaml
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/startTask.yaml
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/stopTask.yaml
--rw-rw-rw-   0 root         (0) root         (0)      125 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/stopTaskFrames.yaml
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/task.yaml
--rw-rw-rw-   0 root         (0) root         (0)      191 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/taskJsonFile.yaml
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/updateTaskUserLevel.yaml
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/schemas/updateUserSetting.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6226 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/signature.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api/task/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13726 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.1/rayvision_api/task/check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api/tests/
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_connect.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_env.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_query.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_signature.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     3669 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/tests/test_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2023-04-25 08:34:12.000000 rayvision_api-3.0.3.1/rayvision_api/url.py
--rw-rw-rw-   0 root         (0) root         (0)    13469 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2387 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/rayvision_api/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6279 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/rayvision_api.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-04 12:40:08.000000 rayvision_api-3.0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1017 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3066 2023-05-04 12:12:01.000000 rayvision_api-3.0.3.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      258 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      187 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      286 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)      229 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/CHANGES.md
+-rw-rw-rw-   0 root         (0) root         (0)    11363 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/dev_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      611 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5166 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      781 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs/rayvision_api/
+-rw-rw-rw-   0 root         (0) root         (0)      274 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/core_module.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/first_look.rst
+-rw-rw-rw-   0 root         (0) root         (0)      737 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/installation_guide.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/connect.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)      160 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/exception.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/fields.rst
+-rw-rw-rw-   0 root         (0) root         (0)      161 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/main/utils.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs/rayvision_api/operators/
+-rw-rw-rw-   0 root         (0) root         (0)      171 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/operators/env.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/operators/query.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/operators/tag.rst
+-rw-rw-rw-   0 root         (0) root         (0)      245 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/operators/task.rst
+-rw-rw-rw-   0 root         (0) root         (0)      173 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/operators/user.rst
+-rw-rw-rw-   0 root         (0) root         (0)      374 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/rayvision_api.operators.rst
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/rayvision_api.task.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs/rayvision_api/task/
+-rw-rw-rw-   0 root         (0) root         (0)      279 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/task/check.rst
+-rw-rw-rw-   0 root         (0) root         (0)      230 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs/rayvision_api/task/handle.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs_en/
+-rw-rw-rw-   0 root         (0) root         (0)   544618 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs_en/RAYVISION Render API V3.0.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/docs_zh/
+-rw-rw-rw-   0 root         (0) root         (0)   248917 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/docs_zh/瑞云渲染APIV4.0.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     7637 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/examples/api_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/init_pycharm_setup.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5167 2023-04-25 08:34:12.000000 rayvision_api-3.0.3.4/rayvision_api/connect.py
+-rw-rw-rw-   0 root         (0) root         (0)     2955 2023-06-28 10:09:55.000000 rayvision_api-3.0.3.4/rayvision_api/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7419 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.4/rayvision_api/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     4796 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/file_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/json_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api/operators/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5167 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/operators/env.py
+-rw-rw-rw-   0 root         (0) root         (0)    22719 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.4/rayvision_api/operators/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/operators/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     6150 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/operators/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/operators/transmit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6396 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/operators/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/abandonTask.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       65 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/add.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       78 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/addTaskLabel.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/addUserPluginConfig.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      246 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/createTask.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/delete.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       72 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/deleteTask.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/deleteTaskLabel.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       42 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/deleteUserPluginConfig.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      383 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/editUserPluginConfig.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/fullSpeedRendering.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       65 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/getOutputUserDirFile.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/getRaySyncUserKey.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/getServerInfo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      110 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/getTaskList.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      119 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/getUserPluginConfig.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/list.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/loadTaskProcessImg.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       83 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/loadingFrameThumbnail.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/queryAllFrameStats.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/queryAnalyseErrorDetail.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       39 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/queryPlatforms.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      110 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/querySoftwareDetail.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      105 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/queryTaskFrames.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       72 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/queryTaskInfo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      125 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/recommitTaskFrames.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      146 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/recommitTasks.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      102 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/schema_v1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       41 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/setDefaultUserPluginConfig.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      116 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/setTaskOverTimeStop.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/startTask.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/stopTask.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      125 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/stopTaskFrames.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       49 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/task.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      191 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/taskJsonFile.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/updateTaskUserLevel.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       50 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/schemas/updateUserSetting.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/signature.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api/task/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13726 2023-01-31 03:50:03.000000 rayvision_api-3.0.3.4/rayvision_api/task/check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_connect.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_env.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     3669 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/tests/test_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2023-04-25 08:34:12.000000 rayvision_api-3.0.3.4/rayvision_api/url.py
+-rw-rw-rw-   0 root         (0) root         (0)    13469 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/rayvision_api/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6279 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/rayvision_api.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-28 07:04:33.000000 rayvision_api-3.0.3.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-29 11:07:58.000000 rayvision_api-3.0.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2022-10-25 04:08:56.000000 rayvision_api-3.0.3.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2023-05-04 12:12:01.000000 rayvision_api-3.0.3.4/tox.ini
```

### Comparing `rayvision_api-3.0.3.1/.pre-commit-config.yaml` & `rayvision_api-3.0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/LICENSE` & `rayvision_api-3.0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/README.md` & `rayvision_api-3.0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs/Makefile` & `rayvision_api-3.0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs/conf.py` & `rayvision_api-3.0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs/make.bat` & `rayvision_api-3.0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs/rayvision_api/first_look.rst` & `rayvision_api-3.0.3.4/docs/rayvision_api/first_look.rst`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs/rayvision_api/installation_guide.rst` & `rayvision_api-3.0.3.4/docs/rayvision_api/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs/rayvision_api/main/constants.rst` & `rayvision_api-3.0.3.4/docs/rayvision_api/main/constants.rst`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs_en/RAYVISION Render API V3.0.pdf` & `rayvision_api-3.0.3.4/docs_en/RAYVISION Render API V3.0.pdf`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/docs_zh/瑞云渲染APIV4.0.pdf` & `rayvision_api-3.0.3.4/docs_zh/瑞云渲染APIV4.0.pdf`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/examples/api_demo.py` & `rayvision_api-3.0.3.4/examples/api_demo.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/connect.py` & `rayvision_api-3.0.3.4/rayvision_api/connect.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/constants.py` & `rayvision_api-3.0.3.4/rayvision_api/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # The name of the package.
 PACKAGE_NAME = 'rayvision_api'
 
 # The all DCC software ID mappings, we can easily get the corresponding
 # ``cgId`` from the alias.
 DCC_ID_MAPPINGS = {
     "maya": "2000",
-    "3ds Max": "2001",
+    "3ds max": "2001",
     "lightwave": "2002",
     "arnold": "2003",
     "houdini": "2004",
     "cinema4d": "2005",
     "softimage": "2006",
     "blender": "2007",
     "vr_standalone": "2008",
@@ -35,15 +35,15 @@
     'version': '2.0.0',
     'Content-Type': 'application/json'
 }
 
 
 CG_SETTING = {
     "maya": "2000",
-    "3ds Max": "2001",
+    "3ds max": "2001",
     "lightwave": "2002",
     "arnold": "2003",
     "houdini": "2004",
     "cinema4d": "2005",
     "softimage": "2006",
     "blender": "2007",
     "vr_standalone": "2008",
```

### Comparing `rayvision_api-3.0.3.1/rayvision_api/core.py` & `rayvision_api-3.0.3.4/rayvision_api/core.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/exception.py` & `rayvision_api-3.0.3.4/rayvision_api/exception.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/file_operator.py` & `rayvision_api-3.0.3.4/rayvision_api/file_operator.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/json_operator.py` & `rayvision_api-3.0.3.4/rayvision_api/json_operator.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/__init__.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/env.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/env.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/query.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/query.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/tag.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/tag.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/task.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/task.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/transmit.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/transmit.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/operators/user.py` & `rayvision_api-3.0.3.4/rayvision_api/operators/user.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/paths.py` & `rayvision_api-3.0.3.4/rayvision_api/paths.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/signature.py` & `rayvision_api-3.0.3.4/rayvision_api/signature.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/task/check.py` & `rayvision_api-3.0.3.4/rayvision_api/task/check.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/conftest.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_connect.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_env.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_query.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_signature.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_tag.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_task.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/tests/test_user.py` & `rayvision_api-3.0.3.4/rayvision_api/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/url.py` & `rayvision_api-3.0.3.4/rayvision_api/url.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/utils.py` & `rayvision_api-3.0.3.4/rayvision_api/utils.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api/validator.py` & `rayvision_api-3.0.3.4/rayvision_api/validator.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/rayvision_api.egg-info/SOURCES.txt` & `rayvision_api-3.0.3.4/rayvision_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/setup.py` & `rayvision_api-3.0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `rayvision_api-3.0.3.1/tox.ini` & `rayvision_api-3.0.3.4/tox.ini`

 * *Files identical despite different names*

