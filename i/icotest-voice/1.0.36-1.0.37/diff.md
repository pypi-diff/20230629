# Comparing `tmp/icotest-voice-1.0.36.tar.gz` & `tmp/icotest-voice-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icotest-voice-1.0.36.tar", last modified: Tue Jun 20 10:09:04 2023, max compression
+gzip compressed data, was "icotest-voice-1.0.37.tar", last modified: Thu Jun 29 12:28:14 2023, max compression
```

## Comparing `icotest-voice-1.0.36.tar` & `icotest-voice-1.0.37.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.36/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.36/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8431 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6843 2023-06-20 10:07:36.000000 icotest-voice-1.0.36/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      858 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Controller.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/ControllersApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    36998 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/HostConfig.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineObject.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineObject1.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineResponse200.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineResponse200Files.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Message.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Request.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/RequestsApi.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/icotest_voice/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/icotest_voice/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   101320 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/requests_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/icotest_voice/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10518 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14635 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/icotest_voice.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8431 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-06-20 10:04:27.000000 icotest-voice-1.0.36/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/setup.cfg
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/test/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_requests_api.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.934635 icotest-voice-1.0.37/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2023-06-29 12:23:54.000000 icotest-voice-1.0.37/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.37/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8432 2023-06-29 12:28:14.934635 icotest-voice-1.0.37/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6844 2023-06-29 12:26:44.000000 icotest-voice-1.0.37/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.926634 icotest-voice-1.0.37/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      858 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/Controller.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/ControllersApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    36980 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/InlineObject.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/InlineObject1.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/InlineResponse200.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/InlineResponse200Files.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/Message.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/Request.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/docs/RequestsApi.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.926634 icotest-voice-1.0.37/icotest_voice/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.930634 icotest-voice-1.0.37/icotest_voice/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/api/controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   101320 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/api/requests_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.930634 icotest-voice-1.0.37/icotest_voice/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10518 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14635 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/models/request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/icotest_voice/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.930634 icotest-voice-1.0.37/icotest_voice.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8432 2023-06-29 12:28:14.000000 icotest-voice-1.0.37/icotest_voice.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-06-29 12:28:14.000000 icotest-voice-1.0.37/icotest_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-06-29 12:28:14.000000 icotest-voice-1.0.37/icotest_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-06-29 12:28:14.000000 icotest-voice-1.0.37/icotest_voice.egg-info/requires.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-06-29 12:28:14.000000 icotest-voice-1.0.37/icotest_voice.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-06-29 12:27:35.000000 icotest-voice-1.0.37/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-06-29 12:28:14.934635 icotest-voice-1.0.37/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-29 12:28:14.934635 icotest-voice-1.0.37/test/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-06-29 11:45:15.000000 icotest-voice-1.0.37/test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.36/LICENSE` & `icotest-voice-1.0.37/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 3ADesign Limited
+Copyright © 2023 3ADesign Limited
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `icotest-voice-1.0.36/PKG-INFO` & `icotest-voice-1.0.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.36
+Version: 1.0.37
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
-License: Copyright © 2022 3ADesign Limited
+License: Copyright © 2023 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.36
-- Package version: 1.0.36
+- API version: 1.0.37
+- Package version: 1.0.37
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -64,15 +64,15 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c" # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
```

### Comparing `icotest-voice-1.0.36/README.md` & `icotest-voice-1.0.37/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.36
-- Package version: 1.0.36
+- API version: 1.0.37
+- Package version: 1.0.37
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -43,15 +43,15 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c" # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
```

### Comparing `icotest-voice-1.0.36/docs/Controller.md` & `icotest-voice-1.0.37/docs/Controller.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.36/docs/ControllersApi.md` & `icotest-voice-1.0.37/docs/ControllersApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.36/docs/Device.md` & `icotest-voice-1.0.37/docs/Device.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.36/docs/DevicesApi.md` & `icotest-voice-1.0.37/docs/DevicesApi.md`

 * *Files 1% similar despite different names*

```diff
@@ -179,18 +179,18 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient() as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.DevicesApi(api_client)
-    controller_id = '10cda64a-0dce-4663-8b47-6ec1867f9568' # str | the unique id of the controller (optional)
-device_id = '5ad25725-8be0-489d-9b26-c0299a76e136' # str | the unique id of the device (optional)
-device_type = 'handset' # str | type of device (optional)
-serial_no = 'serial-123456' # str | serial number (optional)
+    controller_id = 'controller_id_example' # str | the unique id of the controller (optional)
+device_id = 'device_id_example' # str | the unique id of the device (optional)
+device_type = 'device_type_example' # str | type of device (optional)
+serial_no = 'serial_no_example' # str | serial number (optional)
 management_status = True # bool | management status (optional)
 
     try:
         # GET devices
         api_response = api_instance.get_devices(controller_id=controller_id, device_id=device_id, device_type=device_type, serial_no=serial_no, management_status=management_status)
         pprint(api_response)
     except ApiException as e:
```

### Comparing `icotest-voice-1.0.36/docs/Request.md` & `icotest-voice-1.0.37/docs/Request.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.36/docs/RequestsApi.md` & `icotest-voice-1.0.37/docs/RequestsApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.36/icotest_voice/__init__.py` & `icotest-voice-1.0.37/icotest_voice/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.36"
+__version__ = "1.0.37"
 
 # import apis into sdk package
 from icotest_voice.api.controllers_api import ControllersApi
 from icotest_voice.api.devices_api import DevicesApi
 from icotest_voice.api.requests_api import RequestsApi
 
 # import ApiClient
```

### Comparing `icotest-voice-1.0.36/icotest_voice/api/controllers_api.py` & `icotest-voice-1.0.37/icotest_voice/api/controllers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/icotest_voice/api/devices_api.py` & `icotest-voice-1.0.37/icotest_voice/api/devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/icotest_voice/api/requests_api.py` & `icotest-voice-1.0.37/icotest_voice/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/icotest_voice/api_client.py` & `icotest-voice-1.0.37/icotest_voice/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.36/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.37/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `icotest-voice-1.0.36/icotest_voice/configuration.py` & `icotest-voice-1.0.37/icotest_voice/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -251,16 +251,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.36\n"\
-               "SDK Package Version: 1.0.36".\
+               "Version of the API: 1.0.37\n"\
+               "SDK Package Version: 1.0.37".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `icotest-voice-1.0.36/icotest_voice/exceptions.py` & `icotest-voice-1.0.37/icotest_voice/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/__init__.py` & `icotest-voice-1.0.37/icotest_voice/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/controller.py` & `icotest-voice-1.0.37/icotest_voice/models/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/device.py` & `icotest-voice-1.0.37/icotest_voice/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/host_config.py` & `icotest-voice-1.0.37/icotest_voice/models/host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/inline_object.py` & `icotest-voice-1.0.37/icotest_voice/models/inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/inline_object1.py` & `icotest-voice-1.0.37/icotest_voice/models/inline_object1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/inline_response200.py` & `icotest-voice-1.0.37/icotest_voice/models/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/inline_response200_files.py` & `icotest-voice-1.0.37/icotest_voice/models/inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/message.py` & `icotest-voice-1.0.37/icotest_voice/models/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/models/request.py` & `icotest-voice-1.0.37/icotest_voice/models/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.36/icotest_voice/rest.py` & `icotest-voice-1.0.37/icotest_voice/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/icotest_voice.egg-info/PKG-INFO` & `icotest-voice-1.0.37/icotest_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.36
+Version: 1.0.37
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
-License: Copyright © 2022 3ADesign Limited
+License: Copyright © 2023 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.36
-- Package version: 1.0.36
+- API version: 1.0.37
+- Package version: 1.0.37
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -64,15 +64,15 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c" # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
```

### Comparing `icotest-voice-1.0.36/icotest_voice.egg-info/SOURCES.txt` & `icotest-voice-1.0.37/icotest_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.36/pyproject.toml` & `icotest-voice-1.0.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icotest-voice"
-version = "1.0.36"
+version = "1.0.37"
 description = "Icotest Voice API"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Icotest Voice"]
 authors = [
     { name = "Shaun Hirst", email =  "shaun.hirst@3adesign.co.uk" },
     { name = "Ivo Shipkaliev", email = "ivo@3adesign.co.uk" }
 ]
```

### Comparing `icotest-voice-1.0.36/test/test_controller.py` & `icotest-voice-1.0.37/test/test_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_controllers_api.py` & `icotest-voice-1.0.37/test/test_controllers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_device.py` & `icotest-voice-1.0.37/test/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_devices_api.py` & `icotest-voice-1.0.37/test/test_devices_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_host_config.py` & `icotest-voice-1.0.37/test/test_host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_inline_object.py` & `icotest-voice-1.0.37/test/test_inline_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_inline_object1.py` & `icotest-voice-1.0.37/test/test_inline_object1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_inline_response200.py` & `icotest-voice-1.0.37/test/test_inline_response200.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_inline_response200_files.py` & `icotest-voice-1.0.37/test/test_inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_message.py` & `icotest-voice-1.0.37/test/test_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_request.py` & `icotest-voice-1.0.37/test/test_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.36/test/test_requests_api.py` & `icotest-voice-1.0.37/test/test_requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.36
+    The version of the OpenAPI document: 1.0.37
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

