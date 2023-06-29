# Comparing `tmp/mypy-boto3-chime-1.26.117.tar.gz` & `tmp/mypy-boto3-chime-1.26.164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.26.117.tar", last modified: Thu Apr 20 19:33:48 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-1.26.164.tar", last modified: Thu Jun 29 20:25:42 2023, max compression
```

## Comparing `mypy-boto3-chime-1.26.117.tar` & `mypy-boto3-chime-1.26.164.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.467264 mypy-boto3-chime-1.26.117/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-04-20 19:33:48.463264 mypy-boto3-chime-1.26.117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.463264 mypy-boto3-chime-1.26.117/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121614 2023-04-20 19:32:22.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   121414 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-20 19:32:23.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-04-20 19:32:23.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-20 19:32:22.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-20 19:32:22.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144436 2023-04-20 19:32:27.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144277 2023-04-20 19:32:25.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:32:21.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:33:48.463264 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 19:33:48.000000 mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:33:48.467264 mypy-boto3-chime-1.26.117/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-20 19:32:20.000000 mypy-boto3-chime-1.26.117/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.248377 mypy-boto3-chime-1.26.164/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144436 2023-06-29 20:24:36.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144277 2023-06-29 20:24:34.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-29 20:24:30.000000 mypy-boto3-chime-1.26.164/setup.py
```

### Comparing `mypy-boto3-chime-1.26.117/LICENSE` & `mypy-boto3-chime-1.26.164/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/PKG-INFO` & `mypy-boto3-chime-1.26.164/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.26.117
-Summary: Type annotations for boto3.Chime 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.164
+Summary: Type annotations for boto3.Chime 1.26.164 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-chime-1.26.117/README.md` & `mypy-boto3-chime-1.26.164/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/__main__.py` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Chime 1.26.117\nVersion:         1.26.117\nBuilder version:"
+        "Type annotations for boto3.Chime 1.26.164\nVersion:         1.26.164\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.117")
+    print("1.26.164")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1236,15 +1236,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_media_capture_pipeline)
         """
 
     def get_meeting(self, *, MeetingId: str) -> GetMeetingResponseTypeDef:
         """
-        Gets the Amazon Chime SDK meeting details for the specified meeting ID.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_meeting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_meeting)
         """
 
     def get_messaging_session_endpoint(self) -> GetMessagingSessionEndpointResponseTypeDef:
         """
@@ -1446,16 +1446,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_termination)
         """
 
     def get_voice_connector_termination_health(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationHealthResponseTypeDef:
         """
-        Retrieves information about the last time a SIP `OPTIONS` ping was received from
-        your SIP infrastructure for the specified Amazon Chime Voice Connector.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_termination_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_termination_health)
         """
 
     def invite_users(
         self, *, AccountId: str, UserEmailList: Sequence[str], UserType: UserTypeType = ...
@@ -1769,15 +1768,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_supported_phone_number_countries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_supported_phone_number_countries)
         """
 
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Lists the tags applied to an Amazon Chime SDK meeting resource.
+        Lists the tags applied to an Amazon Chime SDK meeting and messaging resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_tags_for_resource)
         """
 
     def list_users(
         self,
@@ -2092,15 +2091,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#stop_meeting_transcription)
         """
 
     def tag_attendee(
         self, *, MeetingId: str, AttendeeId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Applies the specified tags to the specified Amazon Chime SDK attendee.
+        Applies the specified tags to the specified Amazon Chime attendee.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.tag_attendee)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#tag_attendee)
         """
 
     def tag_meeting(
         self, *, MeetingId: str, Tags: Sequence[TagTypeDef]
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1141,15 +1141,15 @@
         Gets an existing media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_media_capture_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_media_capture_pipeline)
         """
     def get_meeting(self, *, MeetingId: str) -> GetMeetingResponseTypeDef:
         """
-        Gets the Amazon Chime SDK meeting details for the specified meeting ID.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_meeting)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_meeting)
         """
     def get_messaging_session_endpoint(self) -> GetMessagingSessionEndpointResponseTypeDef:
         """
         The details of the endpoint for the messaging session.
@@ -1330,16 +1330,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_termination)
         """
     def get_voice_connector_termination_health(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationHealthResponseTypeDef:
         """
-        Retrieves information about the last time a SIP `OPTIONS` ping was received from
-        your SIP infrastructure for the specified Amazon Chime Voice Connector.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_termination_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#get_voice_connector_termination_health)
         """
     def invite_users(
         self, *, AccountId: str, UserEmailList: Sequence[str], UserType: UserTypeType = ...
     ) -> InviteUsersResponseTypeDef:
@@ -1626,15 +1625,15 @@
         Lists supported phone number countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_supported_phone_number_countries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_supported_phone_number_countries)
         """
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Lists the tags applied to an Amazon Chime SDK meeting resource.
+        Lists the tags applied to an Amazon Chime SDK meeting and messaging resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#list_tags_for_resource)
         """
     def list_users(
         self,
         *,
@@ -1921,15 +1920,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.stop_meeting_transcription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#stop_meeting_transcription)
         """
     def tag_attendee(
         self, *, MeetingId: str, AttendeeId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Applies the specified tags to the specified Amazon Chime SDK attendee.
+        Applies the specified tags to the specified Amazon Chime attendee.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.tag_attendee)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/client/#tag_attendee)
         """
     def tag_meeting(
         self, *, MeetingId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -253,14 +254,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -402,14 +404,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -428,16 +431,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -521,14 +527,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -251,14 +252,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -400,14 +402,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -426,16 +429,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -519,14 +525,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.26.117
-Summary: Type annotations for boto3.Chime 1.26.117 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.164
+Summary: Type annotations for boto3.Chime 1.26.164 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.117](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-chime-1.26.117/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.117/setup.py` & `mypy-boto3-chime-1.26.164/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.26.117",
+    version="1.26.164",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.26.117 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Chime 1.26.164 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

