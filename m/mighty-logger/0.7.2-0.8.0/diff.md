# Comparing `tmp/mighty_logger-0.7.2.tar.gz` & `tmp/mighty_logger-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.7.2.tar", last modified: Wed Jun 28 12:24:10 2023, max compression
+gzip compressed data, was "mighty_logger-0.8.0.tar", last modified: Thu Jun 29 13:38:37 2023, max compression
```

## Comparing `mighty_logger-0.7.2.tar` & `mighty_logger-0.8.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.597877 mighty_logger-0.7.2/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.7.2/LICENSE
--rw-rw-rw-   0        0        0    10892 2023-06-28 12:24:10.597877 mighty_logger-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     9949 2023-06-28 11:14:28.000000 mighty_logger-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.459263 mighty_logger-0.7.2/mighty_logger/
--rw-rw-rw-   0        0        0      861 2023-06-28 11:14:28.000000 mighty_logger-0.7.2/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.507455 mighty_logger-0.7.2/mighty_logger/basic/
--rw-rw-rw-   0        0        0      789 2023-06-26 10:51:25.000000 mighty_logger-0.7.2/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0    10109 2023-06-28 10:45:25.000000 mighty_logger-0.7.2/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1499 2023-06-26 10:49:56.000000 mighty_logger-0.7.2/mighty_logger/basic/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.541187 mighty_logger-0.7.2/mighty_logger/basic/lib_types/
--rw-rw-rw-   0        0        0      921 2023-06-27 12:43:22.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/__init__.py
--rw-rw-rw-   0        0        0     1086 2023-06-25 13:07:43.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/animation_type.py
--rw-rw-rw-   0        0        0     2030 2023-06-28 10:45:25.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/entry_type.py
--rw-rw-rw-   0        0        0     1297 2023-06-26 11:32:43.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/environment_type.py
--rw-rw-rw-   0        0        0      798 2023-06-27 12:43:22.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/sorting_key_type.py
--rw-rw-rw-   0        0        0      874 2023-06-25 13:06:36.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/status_message_type.py
--rw-rw-rw-   0        0        0     4317 2023-06-26 11:33:46.000000 mighty_logger-0.7.2/mighty_logger/basic/lib_types/text_buffer_type.py
--rw-rw-rw-   0        0        0     7087 2023-06-28 10:57:00.000000 mighty_logger-0.7.2/mighty_logger/basic/modifier.py
--rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.7.2/mighty_logger/basic/patterns.py
--rw-rw-rw-   0        0        0    28476 2023-06-28 09:48:23.000000 mighty_logger-0.7.2/mighty_logger/mighty_logger.py
--rw-rw-rw-   0        0        0     6699 2023-06-28 11:14:28.000000 mighty_logger-0.7.2/mighty_logger/simple_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.565611 mighty_logger-0.7.2/mighty_logger/src/
--rw-rw-rw-   0        0        0      956 2023-06-28 09:48:23.000000 mighty_logger-0.7.2/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     9975 2023-06-25 13:20:13.000000 mighty_logger-0.7.2/mighty_logger/src/animations.py
--rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.7.2/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.7.2/mighty_logger/src/color_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.593877 mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/
--rw-rw-rw-   0        0        0      831 2023-06-28 10:57:00.000000 mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/__init__.py
--rw-rw-rw-   0        0        0    40877 2023-06-28 11:04:00.000000 mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/entry_types.py
--rw-rw-rw-   0        0        0     1140 2023-06-25 13:20:13.000000 mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/environments.py
--rw-rw-rw-   0        0        0      873 2023-06-27 12:43:22.000000 mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/sorting_keys.py
--rw-rw-rw-   0        0        0     5473 2023-06-25 13:20:13.000000 mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/status_variables.py
--rw-rw-rw-   0        0        0    10808 2023-06-28 09:48:23.000000 mighty_logger-0.7.2/mighty_logger/src/text_buffer.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.478883 mighty_logger-0.7.2/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10892 2023-06-28 12:24:10.000000 mighty_logger-0.7.2/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1244 2023-06-28 12:24:10.000000 mighty_logger-0.7.2/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 12:24:10.000000 mighty_logger-0.7.2/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-28 12:24:10.000000 mighty_logger-0.7.2/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 12:24:10.598876 mighty_logger-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1757 2023-06-28 11:14:28.000000 mighty_logger-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:24:10.596879 mighty_logger-0.7.2/test/
--rw-rw-rw-   0        0        0     3073 2023-06-28 11:06:47.000000 mighty_logger-0.7.2/test/test.py
--rw-rw-rw-   0        0        0      924 2023-06-28 09:53:14.000000 mighty_logger-0.7.2/test/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.645940 mighty_logger-0.8.0/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0    10856 2023-06-29 13:38:37.645940 mighty_logger-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9913 2023-06-29 12:46:55.000000 mighty_logger-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.535905 mighty_logger-0.8.0/mighty_logger/
+-rw-rw-rw-   0        0        0      861 2023-06-29 12:46:55.000000 mighty_logger-0.8.0/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.572906 mighty_logger-0.8.0/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      783 2023-06-29 12:11:16.000000 mighty_logger-0.8.0/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     8311 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1712 2023-06-29 12:11:16.000000 mighty_logger-0.8.0/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0     2606 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.620938 mighty_logger-0.8.0/mighty_logger/basic/lib_types/
+-rw-rw-rw-   0        0        0      869 2023-06-28 14:21:52.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/__init__.py
+-rw-rw-rw-   0        0        0     1086 2023-06-25 13:07:43.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/animation_type.py
+-rw-rw-rw-   0        0        0     2030 2023-06-28 10:45:25.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/entry_type.py
+-rw-rw-rw-   0        0        0     1297 2023-06-26 11:32:43.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/environment_type.py
+-rw-rw-rw-   0        0        0      798 2023-06-27 12:43:22.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/sorting_key_type.py
+-rw-rw-rw-   0        0        0     4317 2023-06-26 11:33:46.000000 mighty_logger-0.8.0/mighty_logger/basic/lib_types/text_buffer_type.py
+-rw-rw-rw-   0        0        0     7061 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/modifier.py
+-rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.8.0/mighty_logger/basic/singleton.py
+-rw-rw-rw-   0        0        0    10554 2023-06-29 12:34:25.000000 mighty_logger-0.8.0/mighty_logger/basic/text_buffer.py
+-rw-rw-rw-   0        0        0    25499 2023-06-29 09:55:09.000000 mighty_logger-0.8.0/mighty_logger/mighty_logger.py
+-rw-rw-rw-   0        0        0     5953 2023-06-29 12:15:54.000000 mighty_logger-0.8.0/mighty_logger/simple_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.631752 mighty_logger-0.8.0/mighty_logger/src/
+-rw-rw-rw-   0        0        0      903 2023-06-29 08:51:20.000000 mighty_logger-0.8.0/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     9975 2023-06-25 13:20:13.000000 mighty_logger-0.8.0/mighty_logger/src/animations.py
+-rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.8.0/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.8.0/mighty_logger/src/color_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.642941 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/
+-rw-rw-rw-   0        0        0      779 2023-06-28 14:22:30.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/__init__.py
+-rw-rw-rw-   0        0        0    40877 2023-06-28 11:04:00.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/entry_types.py
+-rw-rw-rw-   0        0        0     1140 2023-06-25 13:20:13.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/environments.py
+-rw-rw-rw-   0        0        0      873 2023-06-27 12:43:22.000000 mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/sorting_keys.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.544905 mighty_logger-0.8.0/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10856 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 13:38:37.000000 mighty_logger-0.8.0/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:38:37.646940 mighty_logger-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2023-06-29 12:46:55.000000 mighty_logger-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:38:37.644940 mighty_logger-0.8.0/test/
+-rw-rw-rw-   0        0        0     3078 2023-06-29 09:02:18.000000 mighty_logger-0.8.0/test/test.py
+-rw-rw-rw-   0        0        0      924 2023-06-28 09:53:14.000000 mighty_logger-0.8.0/test/test_simple.py
```

### Comparing `mighty_logger-0.7.2/LICENSE` & `mighty_logger-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/PKG-INFO` & `mighty_logger-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mighty_logger
-Version: 0.7.2
+Version: 0.8.0
 Summary: Powerful functional logger
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -106,15 +106,15 @@
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
-- [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
+- [x] v0.8.0 - Export update (added conversion to csv)
 - [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
```

### Comparing `mighty_logger-0.7.2/README.md` & `mighty_logger-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
-- [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
+- [x] v0.8.0 - Export update (added conversion to csv)
 - [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
```

### Comparing `mighty_logger-0.7.2/mighty_logger/__init__.py` & `mighty_logger-0.8.0/mighty_logger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 limitations under the License.
 """
 
 from .mighty_logger import MightyLogger
 from .simple_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.7.2"
+__version__ = "0.8.0"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/__init__.py` & `mighty_logger-0.8.0/mighty_logger/basic/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,9 +12,12 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .exceptions import ColorException, ReCreationException, EnvironmentException, InitException
-from .patterns import Singleton
+from .exceptions import ColorException,\
+	ReCreationException,\
+	EnvironmentException,\
+	InitException,\
+	MessageException
```

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.8.0/mighty_logger/basic/basic_logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,29 +12,33 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import datetime, platform, os, random
+from random import randint
+import platform
+from os import getlogin
+from datetime import datetime
 
 from mighty_logger.basic.lib_types.entry_type import EntryType
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
-from mighty_logger.basic.patterns import Singleton
+from mighty_logger.basic.exceptions import MessageException
+from mighty_logger.basic.singleton import Singleton
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 from mighty_logger.src.ansi_format import GetAnsiFormat
 
 class BasicLogger(Singleton):
 	def __init__(
 		self,
 		program_name: str,
 		env: EnvironmentType
 	) -> None:
-		self._ID: int = random.randint(1000000, 9999999)
+		self._ID: int = randint(1000000, 9999999)
 		self._program_name: str = program_name
 		self._environment: EnvironmentType = env
 		self._settings: dict = {}
 
 	def _initialized_data(
 		self,
 		colors: list[str, str],
@@ -46,69 +50,68 @@
 		:return: a string with initialized data
 		"""
 		match self._environment.environment_name:
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					f"{colors[1]}" +
 					f"{colors[0]}-{self._program_name}?entry> " +
-					f"${platform.node()}:{os.getlogin()}" +
+					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}" +
 					f"{GetAnsiFormat('reset/on')}"
 				)
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				return (
 					f"-{self._program_name}?entry> " +
-					f"${platform.node()}:{os.getlogin()}" +
+					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}" +
 					f"{GetAnsiFormat('reset/on')}"
 				)
 			case LogEnvironments.HTML.environment_name:
 				return (
 					f"<span style='background-color: #{colors[1]};'>" +
 					f"<span style='color: #{colors[0]};'>-{self._program_name}?entry> " +
-					f"${platform.node()}:{os.getlogin()}" +
+					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}" +
 					f"</span></span>"
 				)
 			case LogEnvironments.MARKDOWN.environment_name:
 				return (
 					f"<span style='background-color: #{colors[1]};'>" +
 					f"<span style='color: #{colors[0]};'>-{self._program_name}?entry> " +
-					f"${platform.node()}:{os.getlogin()}" +
+					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}" +
 					f"</span></span>"
 				)
 			case LogEnvironments.PLAIN.environment_name:
 				return (
 					f"-{self._program_name}?entry> " +
-					f"${platform.node()}:{os.getlogin()}" +
+					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}"
 				)
 
 	def _assemble_entry(
 		self,
 		entry_type: EntryType,
 		icon_set: int,
 		animation: str,
-		status_message_text: str,
 		message_text: str,
 		entry_background: bool,
 		local_settings: dict
 	) -> str:
 		"""
 		A method that assemble an entry into a string and returns it.
 
@@ -117,82 +120,75 @@
 		:param icon: Type icon
 		:param status_message_text: Status message
 		:param message_type: Entry type
 		:param message_text: Entry message
 		:param local_settings: Settings for the string of the current entry
 		:return: the formed entry string
 		"""
+		if len(message_text) < 10:
+			raise MessageException("Message is too short (less than 10 characters)")
+
 		bold = local_settings['bold'] if 'bold' in local_settings else self._settings['global_bold_font']
 		italic = local_settings['italic'] if 'italic' in local_settings else self._settings['global_italic_font']
 		invert = local_settings['invert'] if 'invert' in local_settings else self._settings['global_invert_font']
-		time_entry = local_settings['time_local_entry'] if 'time_local_entry' in local_settings else self._settings['time_global_entry']
-		status_entry = local_settings['status_local_entry'] if 'status_local_entry' in local_settings else self._settings['status_global_entry']
-		status_message_entry = local_settings['status_message_local_entry'] if 'status_message_local_entry' in local_settings else self._settings['status_message_global_entry']
-		status_type_entry = local_settings['status_type_local_entry'] if 'status_type_local_entry' in local_settings else self._settings['status_type_global_entry']
-		message_entry = local_settings['message_local_entry'] if 'message_local_entry' in local_settings else self._settings['message_global_entry']
 
 		match self._environment.environment_name:
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					(f"{GetAnsiFormat('bold/on')}" if bold else "") +
 					(f"{GetAnsiFormat('italic/on')}" if italic else "") +
 					(f"{GetAnsiFormat('invert/on')}" if invert else "") +
 					f"{entry_type.background_color[self._environment.environment_code][entry_background]}" +
 					f"{entry_type.message_color[self._environment.environment_code][entry_background]}-?entry> {animation} " +
-					(f"{entry_type.time_color[self._environment.environment_code][entry_background]}*{datetime.datetime.now()} " if time_entry else "") +
+					f"{entry_type.time_color[self._environment.environment_code][entry_background]}*{datetime.now()} " +
 					f"{entry_type.icon[icon_set]} " +
-					(f"{entry_type.status_color[self._environment.environment_code][entry_background]}#STATUS: " if status_entry else "") +
-					(f"{entry_type.status_message_color[self._environment.environment_code][entry_background]}{status_message_text} " if status_message_entry else "") +
-					(f"{entry_type.type_color[self._environment.environment_code][entry_background]}{entry_type.type_category}{entry_type.type_name} - " if status_type_entry else "") +
-					(f"{entry_type.message_color[self._environment.environment_code][entry_background]}{message_text}" if message_entry else "") +
+					f"{entry_type.status_color[self._environment.environment_code][entry_background]}#STATUS: " +
+					f"{entry_type.type_color[self._environment.environment_code][entry_background]}{entry_type.type_category}{entry_type.type_name} - " +
+					f"{entry_type.message_color[self._environment.environment_code][entry_background]}{message_text}" +
 					f"{GetAnsiFormat('reset/on')}"
 				)
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				return (
 					f"-?entry> {animation} " +
-					(f"*{datetime.datetime.now()} " if time_entry else "") +
+					f"*{datetime.now()} " +
 					f"{entry_type.icon[icon_set]} " +
-					(f"#STATUS: " if status_entry else "") +
-					(f"{status_message_text} " if status_message_entry else "") +
-					(f"{entry_type.type_category}{entry_type.type_name} - " if status_type_entry else "") +
-					(f"{message_text}" if message_entry else "")
+					f"#STATUS: " +
+					f"{entry_type.type_category}{entry_type.type_name} - " +
+					f"{message_text}"
 				)
 			case LogEnvironments.HTML.environment_name:
 				return (
 					(f"<b>" if bold else "") +
 					(f"<i>" if italic else "") +
 					f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][entry_background]};'>" +
 					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>-?entry> {animation} </span>" +
-					(f"<span style='color: #{entry_type.time_color[self._environment.environment_code][entry_background]};'>*{datetime.datetime.now()} </span>" if time_entry else "") +
+					f"<span style='color: #{entry_type.time_color[self._environment.environment_code][entry_background]};'>*{datetime.now()} </span>" +
 					f"{entry_type.icon[icon_set]} " +
-					(f"<span style='color: #{entry_type.status_color[self._environment.environment_code][entry_background]};'>#STATUS: </span>" if status_entry else "") +
-					(f"<span style='color: #{entry_type.status_message_color[self._environment.environment_code][entry_background]};'>{status_message_text} </span>" if status_message_entry else "") +
-					(f"<span style='color: #{entry_type.type_color[self._environment.environment_code][entry_background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" if status_type_entry else "") +
-					(f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>{message_text}</span></span>" if message_entry else "") +
+					f"<span style='color: #{entry_type.status_color[self._environment.environment_code][entry_background]};'>#STATUS: </span>" +
+					f"<span style='color: #{entry_type.type_color[self._environment.environment_code][entry_background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>{message_text}</span></span>" +
 					(f"</i>" if italic else "") +
 					(f"</b>" if bold else "")
 				)
 			case LogEnvironments.MARKDOWN.environment_name:
 				return (
-						(f"<b>" if bold else "") +
-						(f"<i>" if italic else "") +
-						f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][entry_background]};'>" +
-						f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>-?entry> {animation} </span>" +
-						(f"<span style='color: #{entry_type.time_color[self._environment.environment_code][entry_background]};'>*{datetime.datetime.now()} </span>" if time_entry else "") +
-						f"{entry_type.icon[icon_set]} " +
-						(f"<span style='color: #{entry_type.status_color[self._environment.environment_code][entry_background]};'>#STATUS: </span>" if status_entry else "") +
-						(f"<span style='color: #{entry_type.status_message_color[self._environment.environment_code][entry_background]};'>{status_message_text} </span>" if status_message_entry else "") +
-						(f"<span style='color: #{entry_type.type_color[self._environment.environment_code][entry_background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" if status_type_entry else "") +
-						(f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>{message_text}</span></span>" if message_entry else "") +
-						(f"</i>" if italic else "") +
-						(f"</b>" if bold else "")
+					(f"<b>" if bold else "") +
+					(f"<i>" if italic else "") +
+					f"<span style='background-color: #{entry_type.background_color[self._environment.environment_code][entry_background]};'>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>-?entry> {animation} </span>" +
+					f"<span style='color: #{entry_type.time_color[self._environment.environment_code][entry_background]};'>*{datetime.now()} </span>" +
+					f"{entry_type.icon[icon_set]} " +
+					f"<span style='color: #{entry_type.status_color[self._environment.environment_code][entry_background]};'>#STATUS: </span>" +
+					f"<span style='color: #{entry_type.type_color[self._environment.environment_code][entry_background]};'>{entry_type.type_category}{entry_type.type_name} - </span>" +
+					f"<span style='color: #{entry_type.message_color[self._environment.environment_code][entry_background]};'>{message_text}</span></span>" +
+					(f"</i>" if italic else "") +
+					(f"</b>" if bold else "")
 				)
 			case LogEnvironments.PLAIN.environment_name:
 				return (
 					f"-?entry> {animation} " +
-					(f"*{datetime.datetime.now()} " if time_entry else "") +
+					f"*{datetime.now()} " +
 					f"{entry_type.icon[icon_set]} " +
-					(f"#STATUS: " if status_entry else "") +
-					(f"{status_message_text} " if status_message_entry else "") +
-					(f"{entry_type.type_category}{entry_type.type_name} - " if status_type_entry else "") +
-					(f"{message_text}" if message_entry else "")
+					f"#STATUS: " if status_entry else "" +
+					f"{entry_type.type_category}{entry_type.type_name} - " +
+					f"{message_text}"
 				)
```

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/exceptions.py` & `mighty_logger-0.8.0/mighty_logger/basic/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,7 +51,17 @@
 	The exception thrown on errors during initialization.
 	"""
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
+
+class MessageException(BaseException):
+	"""
+	The exception that is thrown when a write message is too short.
+	"""
+	def __init__(self, message):
+		self.message = message
+
+	def __str__(self):
+		return self.message
```

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/lib_types/__init__.py` & `mighty_logger-0.8.0/mighty_logger/basic/lib_types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 limitations under the License.
 """
 
 from .animation_type import IndefiniteAnimationType, DefiniteAnimationType
 from .entry_type import EntryType
 from .environment_type import EnvironmentType
 from .sorting_key_type import SortingKeyType
-from .status_message_type import StatusMessageType
 from .text_buffer_type import TextBufferType
```

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/lib_types/animation_type.py` & `mighty_logger-0.8.0/mighty_logger/basic/lib_types/animation_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/lib_types/entry_type.py` & `mighty_logger-0.8.0/mighty_logger/basic/lib_types/entry_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/lib_types/environment_type.py` & `mighty_logger-0.8.0/mighty_logger/basic/lib_types/environment_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/lib_types/sorting_key_type.py` & `mighty_logger-0.8.0/mighty_logger/basic/lib_types/sorting_key_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/lib_types/text_buffer_type.py` & `mighty_logger-0.8.0/mighty_logger/basic/lib_types/text_buffer_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/modifier.py` & `mighty_logger-0.8.0/mighty_logger/basic/modifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import re
+from re import sub
 
 from mighty_logger.basic.lib_types.entry_type import EntryType
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.basic.lib_types.sorting_key_type import SortingKeyType
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 from mighty_logger.src.lib_types_collection.sorting_keys import SortingKeys
 
@@ -75,21 +75,21 @@
 		cleared_entry = ""
 		sorting_entries = []
 		count_separators = 0
 
 		for index, entry in enumerate(self.__entries[1:]):
 			match self.__env.environment_name:
 				case LogEnvironments.CONSOLE.environment_name:
-					cleared_entry = re.sub(r"\033\[.*?m", "", entry)
+					cleared_entry = sub(r"\033\[.*?m", "", entry)
 				case LogEnvironments.PLAIN_CONSOLE.environment_name:
 					cleared_entry = entry
 				case LogEnvironments.HTML.environment_name:
-					cleared_entry = re.sub(r"<.*?>", "", entry)
+					cleared_entry = sub(r"<.*?>", "", entry)
 				case LogEnvironments.MARKDOWN.environment_name:
-					cleared_entry = re.sub(r"<.*?>", "", entry)
+					cleared_entry = sub(r"<.*?>", "", entry)
 				case LogEnvironments.PLAIN.environment_name:
 					cleared_entry = entry
 			if cleared_entry.startswith("-?"):
 				parts = cleared_entry.split("*")[1].split()
 				sorting_entries.append([
 					self.__entries.pop(index + 1 - len(sorting_entries) - count_separators),
 					" ".join(parts[0:2]),
@@ -115,29 +115,29 @@
 		sorted_entries = [item[0] for item in sorting_entries]
 
 		self.__entries.insert(1, "----------------------------------Ordered logs----------------------------------")
 		self.__entries.insert(2, "-----------------------------Unsorted empty entries-----------------------------")
 		self.__entries[2:2] = sorted_entries
 		self.__entries.append("--------------------------------------------------------------------------------")
 
-	def search(self, keyword: str, empty: bool = False) -> None:
+	def search(self, keyword: str, empty: bool) -> None:
 		cleared_entry = ""
 		searching_entries = []
 		count_separators = 0
 
 		for index, entry in enumerate(self.__entries[1:]):
 			match self.__env.environment_name:
 				case LogEnvironments.CONSOLE.environment_name:
-					cleared_entry = re.sub(r"\033\[.*?m", "", entry)
+					cleared_entry = sub(r"\033\[.*?m", "", entry)
 				case LogEnvironments.PLAIN_CONSOLE.environment_name:
 					cleared_entry = entry
 				case LogEnvironments.HTML.environment_name:
-					cleared_entry = re.sub(r"<.*?>", "", entry)
+					cleared_entry = sub(r"<.*?>", "", entry)
 				case LogEnvironments.MARKDOWN.environment_name:
-					cleared_entry = re.sub(r"<.*?>", "", entry)
+					cleared_entry = sub(r"<.*?>", "", entry)
 				case LogEnvironments.PLAIN.environment_name:
 					cleared_entry = entry
 			if cleared_entry.startswith("--"):
 				self.__entries.pop(index + 1 - len(searching_entries) - count_separators)
 				count_separators += 1
 				continue
 			if cleared_entry.startswith("-?"):
@@ -165,21 +165,21 @@
 		cleared_entry = ""
 		selected_entries = []
 		count_excess = 0
 
 		for index, entry in enumerate(self.__entries[1:]):
 			match self.__env.environment_name:
 				case LogEnvironments.CONSOLE.environment_name:
-					cleared_entry = re.sub(r"\033\[.*?m", "", entry)
+					cleared_entry = sub(r"\033\[.*?m", "", entry)
 				case LogEnvironments.PLAIN_CONSOLE.environment_name:
 					cleared_entry = entry
 				case LogEnvironments.HTML.environment_name:
-					cleared_entry = re.sub(r"<.*?>", "", entry)
+					cleared_entry = sub(r"<.*?>", "", entry)
 				case LogEnvironments.MARKDOWN.environment_name:
-					cleared_entry = re.sub(r"<.*?>", "", entry)
+					cleared_entry = sub(r"<.*?>", "", entry)
 				case LogEnvironments.PLAIN.environment_name:
 					cleared_entry = entry
 			if cleared_entry.startswith("-?"):
 				parts = cleared_entry.split("*")[1].split()
 				if entry_type.type_category == "":
 					if parts[4][1:] == entry_type.type_name:
 						selected_entries.append(self.__entries.pop(index + 1 - len(selected_entries) - count_excess))
```

### Comparing `mighty_logger-0.7.2/mighty_logger/basic/patterns.py` & `mighty_logger-0.8.0/mighty_logger/basic/singleton.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/mighty_logger.py` & `mighty_logger-0.8.0/mighty_logger/mighty_logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
 from mighty_logger.basic.lib_types.animation_type import BasicAnimationType,\
 	IndefiniteAnimationType,\
 	DefiniteAnimationType
 from mighty_logger.basic.lib_types.entry_type import EntryType
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.basic.lib_types.sorting_key_type import SortingKeyType
-from mighty_logger.basic.lib_types.status_message_type import StatusMessageType
 from mighty_logger.basic.lib_types.text_buffer_type import TextBufferType
 from mighty_logger.basic.basic_logger import BasicLogger
 from mighty_logger.basic.exceptions import ReCreationException, InitException
+from mighty_logger.basic.exporter import Exporter
 from mighty_logger.basic.modifier import Modifier
+from mighty_logger.basic.text_buffer import BasicTextBuffer, TextBuffer
 from mighty_logger.src.lib_types_collection.entry_types import ServiceLogger,\
 	LoggerEntryTypes,\
 	ServiceProcessEntryTypes,\
 	ServiceTimerEntryTypes
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 from mighty_logger.src.lib_types_collection.sorting_keys import SortingKeys
 from mighty_logger.src.animations import IndefiniteAnimations, DefiniteAnimations
-from mighty_logger.src.text_buffer import BasicTextBuffer, TextBuffer
 
 class MightyLogger(BasicLogger):
 	"""
 	The Logger class is a class that implements the functionality
 	of logging the work of software in different directions.\n
 	It has a color output of information, settings for the operation of the log.
 	Only one class object can be created!!!\n
@@ -59,42 +59,32 @@
 	def __init__(
 		self,
 		*,
 		program_name: str = "Unknown",
 		log_environment: EnvironmentType = LogEnvironments.PLAIN,
 		console_width: int = 60,
 		icon_set: int = 1,
-		time_global_entry: bool = True,
-		status_global_entry: bool = True,
-		status_message_global_entry: bool = True,
-		status_type_global_entry: bool = True,
-		message_global_entry: bool = True,
 		global_bold_font: bool = False,
 		global_italic_font: bool = False,
 		global_invert_font: bool = False,
 		global_background: bool = False,
 	) -> None:
 		if not hasattr(self, "_environment"):
 			super().__init__(program_name, log_environment)
 			self._animation: BasicAnimationType = BasicAnimationType([])
 			self._icon_set = icon_set if 0 < icon_set < 5 else 1
 			self._settings["global_bold_font"] = global_bold_font
 			self._settings["global_italic_font"] = global_italic_font
 			self._settings["global_invert_font"] = global_invert_font
-			self._settings["time_global_entry"] = time_global_entry
-			self._settings["status_global_entry"] = status_global_entry
-			self._settings["status_message_global_entry"] = status_message_global_entry
-			self._settings["status_type_global_entry"] = status_type_global_entry
-			self._settings["message_global_entry"] = message_global_entry
 			self._progress_rise = 0
 			self._progress_start: datetime | None = None
 			self._progress_time: str = "        "
 			self._progress_interrupt = False
 			self._start_timer_value: datetime | None = None
-			self.global_background = global_background
+			self._global_background = global_background
 			self._buffer: TextBufferType = TextBufferType(log_environment)
 			self._init_buffer(console_width)
 			self._initial_log()
 		else:
 			raise ReCreationException("Logger class object already created")
 
 	def _init_buffer(self, console_width: int):
@@ -109,15 +99,14 @@
 		buffer_class, buffer_args = buffer_classes.get(self._environment.environment_name, (None, None))
 		if buffer_class:
 			if buffer_class._instance is not None:
 				self._buffer = buffer_class._instance
 				self.entry(
 					entry_type=LoggerEntryTypes.notice,
 					message_text="An existing buffer was taken into use",
-					status_message=StatusMessageType("Note"),
 					local_settings={"italic": True} if buffer_class == TextBuffer else None
 				)
 			else:
 				self._buffer = buffer_class(*buffer_args)
 		else:
 			raise InitException("Text buffer initialization error")
 
@@ -125,38 +114,29 @@
 		"""
 		Displays initialized information.
 		"""
 		if self._environment.weak_environment:
 			self._buffer << "<body style='background-color: #000000; color: #ffffff;'>"
 		self._buffer << self._initialized_data(
 			[
-				ServiceLogger.initial[0][self._environment.environment_code][self.global_background],
-				ServiceLogger.initial[1][self._environment.environment_code][self.global_background]
+				ServiceLogger.initial[0][self._environment.environment_code][self._global_background],
+				ServiceLogger.initial[1][self._environment.environment_code][self._global_background]
 			]
 		)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
 	def set_icons(self, icon_set: int) -> None:
 		"""
 		Changes the current icon set used by the Logger.
 
 		:param icon_set: Icon set to use
 		"""
 		self._icon_set = icon_set if 0 < icon_set < 5 else 1
 
-	def buffer(self) -> TextBufferType:
-		"""
-		The Text Buffer object is created in the class constructor and this
-		method is used to access it. It returns a buffer.
-
-		:return: a text buffer object
-		"""
-		return self._buffer
-
 	# ######################################################################################## #
 	#                                                                                          #
 	#                                        Publishers                                        #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def publish_id(self) -> None:
@@ -271,246 +251,227 @@
 		sorter = Modifier(self._buffer.get_data().copy(), self._environment)
 		sorter.sort(key)
 		sorted_buffer = sorter.entries
 		self.clearly()
 		for entry in sorted_buffer:
 			self.empty(entry)
 
-	def sort_with_save(self, key: SortingKeyType) -> None:
+	def sort_with_save(self, key: SortingKeyType, sort_file_name: str) -> None:
 		original = self._buffer.get_data().copy()
 		sorter = Modifier(self._buffer.get_data(), self._environment)
 		sorter.sort(key)
-		self._buffer.save("sorted_logs", False)
+		self._buffer.save(sort_file_name, False)
 		self._buffer.get_data().clear()
 		self._buffer.get_data().extend(original)
 
-	def search(self, keyword: str, empty: bool = False) -> None:
+	def search(self, keyword: str, empty: bool) -> None:
 		searcher = Modifier(self._buffer.get_data().copy(), self._environment)
 		searcher.search(keyword, empty)
 		searched_buffer = searcher.entries
 		self.clearly()
 		for entry in searched_buffer:
 			self.empty(entry)
 
-	def search_with_save(self, keyword: str, empty: bool = False) -> None:
+	def search_with_save(self, keyword: str, empty: bool, search_file_name: str) -> None:
 		original = self._buffer.get_data().copy()
 		searcher = Modifier(self._buffer.get_data(), self._environment)
 		searcher.search(keyword, empty)
-		self._buffer.save("searched_logs", False)
+		self._buffer.save(search_file_name, False)
 		self._buffer.get_data().clear()
 		self._buffer.get_data().extend(original)
 
 	def select(self, entry_type: EntryType) -> None:
 		selector = Modifier(self._buffer.get_data().copy(), self._environment)
 		selector.select(entry_type)
 		selected_buffer = selector.entries
 		self.clearly()
 		for entry in selected_buffer:
 			self.empty(entry)
 
-	def select_with_save(self, entry_type: EntryType) -> None:
+	def select_with_save(self, entry_type: EntryType, select_file_name: str) -> None:
 		original = self._buffer.get_data().copy()
 		selector = Modifier(self._buffer.get_data(), self._environment)
 		selector.select(entry_type)
-		self._buffer.save("selected_logs", False)
+		self._buffer.save(select_file_name, False)
 		self._buffer.get_data().clear()
 		self._buffer.get_data().extend(original)
 
+	def export_to_csv(self, export_file_name: str) -> None:
+		exporter = Exporter(self._buffer.get_data(), self._environment)
+		exporter.export_to_csv()
+		exporter.save(export_file_name)
+
 	# ######################################################################################## #
 	#                                                                                          #
 	#                                    Entering to Logger                                    #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def entry(
 		self,
-		*,
 		entry_type: EntryType,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		...
 
 		:param entry_type:
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		if local_settings is None:
 			local_settings = {}
-		background = local_background if local_background is not None else self.global_background
+		background = local_background if local_background is not None else self._global_background
 		self.empty(
 			self._assemble_entry(
 				entry_type,
 				self._icon_set,
 				self._progress_time,
-				status_message.current_status_message,
 				message_text,
 				background,
 				local_settings
 			)
 		)
 
 	# ######################################################################################## #
 	#                                                                                          #
 	#                                  Entering to Processes                                   #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def start_indefinite_process(
 		self,
-		*,
+		message_text: str,
 		animation: IndefiniteAnimationType = IndefiniteAnimations.Line,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that starts the whole process of indefinite logging. While the process
 		is running, you cannot start other processes in the Logger and call the entering
 		methods directly. While the process is running - the last entry will play
 		the animation of the process. Before starting a process, you can specify that
 		the process Logs and configure Initiation and Progress entries.
 		\n
 		Since v0.6.0
 
 		:param animation: The name of the animation that will play in the Progress entry
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._animation = animation
 
 		self._progress_start = datetime.now()
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
-		self.entry(entry_type=ServiceProcessEntryTypes.initiation, **args)
+		self.entry(ServiceProcessEntryTypes.initiation, **args)
 
 		thread = Thread(target=self._indefinite_progress, kwargs=args)
 		thread.start()
 
 	def _indefinite_progress(
 		self,
-		*,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that creates an animation entry. Only works on the last string.
 		You need to run in a thread. Terminates when the process stop flag
 		is set by the Logger.stop_process() method.
 		\n
 		Since v0.6.0
 
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		animation_index = 0
 		self._buffer << "."
 		if self._environment.updatable:
 			self._buffer.update_console()
 		while not self._progress_interrupt:
 			animation_item = self._animation.animation[animation_index]
-			background = local_background if local_background is not None else self.global_background
+			background = local_background if local_background is not None else self._global_background
 			self._buffer.get_data()[-1] = self._assemble_entry(
 				ServiceProcessEntryTypes.process,
 				self._icon_set,
 				animation_item,
-				status_message.current_status_message,
 				message_text,
 				background,
 				local_settings
 			)
 			animation_index = (animation_index + 1) % len(self._animation.animation)
 			if self._environment.updatable:
 				self._buffer.update_entry()
 			sleep(0.1)
 		if self._environment.updatable:
 			self._buffer.update_console()
 
 	def start_definite_process(
 		self,
-		*,
+		message_text: str,
 		progress_bar: DefiniteAnimationType = DefiniteAnimations.Line,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that starts the whole process of a definite logging. While the process
 		is running, you cannot start other processes in the Logger and call the entering
 		methods directly. While the process is running - the last entry will display
 		the progress of the process. Before starting a process, you can specify that
 		the process Logs and configure Initiation and Progress entries.
 		\n
 		Since v0.6.0
 
 		:param progress_bar: The name of the progress bar that will play in the Progress entry
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._animation = progress_bar
 
 		self._progress_start = datetime.now()
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
-		self.entry(entry_type=ServiceProcessEntryTypes.initiation, **args)
+		self.entry(ServiceProcessEntryTypes.initiation, **args)
 
 		thread = Thread(target=self._definite_progress, kwargs=args)
 		thread.start()
 
 	def _definite_progress(
 		self,
 		*,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		A method that creates a progress bar entry. Only works on the last string.
 		You need to run in a thread. Terminates when the process stop flag
 		is set by the Logger.stop_process() method.
 		\n
 		Since v0.6.0
 
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		old_progress_rise = 0
@@ -519,20 +480,19 @@
 			self._buffer.update_console()
 		while not self._progress_interrupt:
 			if old_progress_rise == self._progress_rise:
 				continue
 			else:
 				old_progress_rise = self._progress_rise
 				animation_item = f"{self._animation.animation[(self._progress_rise // 15) + (2 if self._progress_rise == 100 else 1)]} - {self._progress_rise} %"
-				background = local_background if local_background is not None else self.global_background
+				background = local_background if local_background is not None else self._global_background
 				self._buffer.get_data()[-1] = self._assemble_entry(
 					ServiceProcessEntryTypes.process,
 					self._icon_set,
 					animation_item,
-					status_message.current_status_message,
 					message_text,
 					background,
 					local_settings
 				)
 				if self._environment.updatable:
 					self._buffer.update_entry()
 			sleep(0.1)
@@ -550,18 +510,16 @@
 
 		:param percent: Process completion percentage
 		"""
 		self._progress_rise = percent
 
 	def note_process(
 		self,
-		*,
 		entry_type: EntryType,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		An important method that allows you to add standard non-process entry types
 		while a process is running. It's important to note that this entry will still be
 		associated with the process, so it's best to use this entry when you want to describe
@@ -570,75 +528,63 @@
 		cannot be used outside a process: achievement and milestone.
 		\n
 		Use `from mighty_logger.src import TypesEntries` for `entry_type`.
 		\n
 		Since v0.6.0
 
 		:param entry_type: The type of entry to be entered in the progress history
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		sleep(0.001)
 		last = self._buffer.pop()
 
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
-		self.entry(entry_type=entry_type, **args)
+		self.entry(entry_type, **args)
 
 		self.empty(last)
 
 	def stop_process(
 		self,
-		*,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		The method that terminates the process. If before the end of the process
 		its execution has reached 100% - the process was completed successfully,
 		otherwise - failed. After calling this method, the Progress entry will be replaced
 		by the entry with the result of the process execution.
 		\n
 		Since v0.6.0
 
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._progress_interrupt = True
 		sleep(0.11)
 		self._buffer.remove()
 
 		progress_stop = datetime.now()
 		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		self.entry(
-			entry_type=ServiceProcessEntryTypes.success if self._progress_rise == 100 else ServiceProcessEntryTypes.fail,
+			ServiceProcessEntryTypes.success if self._progress_rise == 100 else ServiceProcessEntryTypes.fail,
 			**args
 		)
 
 		self._progress_rise = 0
 		self._progress_start = None
 		self._progress_time = "        "
 		self._progress_interrupt = False
@@ -647,102 +593,81 @@
 	#                                                                                          #
 	#                                     Entering to Timer                                    #
 	#                                                                                          #
 	# ######################################################################################## #
 
 	def start_timer(
 		self,
-		*,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		...
 
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._start_timer_value = datetime.now()
 		stop_timer_value = datetime.now()
 		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
 
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
-		self.entry(entry_type=ServiceTimerEntryTypes.start_timer, **args)
+		self.entry(ServiceTimerEntryTypes.start_timer, **args)
 
 		self._progress_time = "        "
 
 	def timer_mark(
 		self,
-		*,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		...
 
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		stop_timer_value = datetime.now()
 		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
 
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
-		self.entry(entry_type=ServiceTimerEntryTypes.timer_mark, **args)
+		self.entry(ServiceTimerEntryTypes.timer_mark, **args)
 
 		self._progress_time = "        "
 
 	def stop_timer(
 		self,
-		*,
-		status_message: StatusMessageType = StatusMessageType("..."),
-		message_text: str = "...",
+		message_text: str,
 		local_background: bool = None,
 		local_settings: dict = None
 	) -> None:
 		"""
 		...
 
-		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		stop_timer_value = datetime.now()
 		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
 
-		args = {}
-		if status_message != StatusMessageType("..."):
-			args['status_message'] = status_message
-		if message_text != "...":
-			args['message_text'] = message_text
+		args = {'message_text': message_text}
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
-		self.entry(entry_type=ServiceTimerEntryTypes.stop_timer, **args)
+		self.entry(ServiceTimerEntryTypes.stop_timer, **args)
 
 		self._start_timer_value = None
 		self._progress_time = "        "
```

### Comparing `mighty_logger-0.7.2/mighty_logger/simple_logger.py` & `mighty_logger-0.8.0/mighty_logger/simple_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,198 +36,151 @@
 			self.__logger = MightyLogger._instance
 			self.notice("An existing logger was taken into use")
 		else:
 			self.__logger = MightyLogger(
 				program_name=program_name,
 				log_environment=environment,
 				console_width=console_width,
-				status_global_entry=False,
-				status_message_global_entry=False
 			)
 
 	def might(self) -> MightyLogger:
 		return self.__logger
 
-	def debug(self, message_text: str = "...") -> None:
+	def debug(self, message_text: str) -> None:
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.debug,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.debug, message_text)
 
-	def debug_performance(self, message_text: str = "...") -> None:
+	def debug_performance(self, message_text: str) -> None:
 		"""
 		Performance debugging information logging:
 		Can be used to log entry the execution time of operations or other
 		performance information while the application is being debugged.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.debug_performance,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.debug_performance, message_text)
 
-	def performance(self, message_text: str = "...") -> None:
+	def performance(self, message_text: str) -> None:
 		"""
 		Performance information logging:
 		Can be used to log entry the execution time of operations or
 		other application performance information.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.performance,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.performance, message_text)
 
-	def event(self, message_text: str = "...") -> None:
+	def event(self, message_text: str) -> None:
 		"""
 		Event information logging:
 		Can be used to log entry specific events in the application,
 		such as button presses or mouse cursor movements.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.event,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.event, message_text)
 
-	def audit(self, message_text: str = "...") -> None:
+	def audit(self, message_text: str) -> None:
 		"""
 		Audit information logging:
 		Can be used to log entry changes in the system, such as creating or
 		deleting users, as well as changes in security settings.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.audit,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.audit, message_text)
 
-	def metrics(self, message_text: str = "...") -> None:
+	def metrics(self, message_text: str) -> None:
 		"""
 		Metrics information logging:
 		Can be used to log entry metrics to track application performance and identify issues.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.metrics,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.metrics, message_text)
 
-	def user(self, message_text: str = "...") -> None:
+	def user(self, message_text: str) -> None:
 		"""
 		User information logging:
 		Can be used to log entry custom logs to store additional information
 		that may be useful for diagnosing problems.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.user,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.user, message_text)
 
-	def message(self, message_text: str = "...") -> None:
+	def message(self, message_text: str) -> None:
 		"""
 		Message information logging:
 		Can be used for the usual output of ordinary messages about the program's operation.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.message,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.message, message_text)
 
-	def info(self, message_text: str = "...") -> None:
+	def info(self, message_text: str) -> None:
 		"""
 		Default information logging:
 		Can be used to log entry messages with specific content about the operation of the program.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.info,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.info, message_text)
 
-	def notice(self, message_text: str = "...") -> None:
+	def notice(self, message_text: str) -> None:
 		"""
 		Notice information logging:
 		Can be used to flag important events that might be missed with a normal logging level.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.notice,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.notice, message_text)
 
-	def warning(self, message_text: str = "...") -> None:
+	def warning(self, message_text: str) -> None:
 		"""
 		Warning information logging:
 		Can be used to log entry warnings that the program may work with unpredictable results.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.warning,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.warning, message_text)
 
-	def error(self, message_text: str = "...") -> None:
+	def error(self, message_text: str) -> None:
 		"""
 		Error information logging:
 		Used to log entry errors and crashes in the program.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.error,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.error, message_text)
 
-	def critical(self, message_text: str = "...") -> None:
+	def critical(self, message_text: str) -> None:
 		"""
 		Critical error information logging:
 		Used to log entry for critical and unpredictable program failures.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=LoggerEntryTypes.critical,
-			message_text=message_text
-		)
+		self.__logger.entry(LoggerEntryTypes.critical, message_text)
 
-	def success(self, message_text: str = "...") -> None:
+	def success(self, message_text: str) -> None:
 		"""
 		Success information logging:
 		Used to log entry a message about the success of the process.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=ServiceProcessEntryTypes.success,
-			message_text=message_text
-		)
+		self.__logger.entry(ServiceProcessEntryTypes.success, message_text)
 
-	def fail(self, message_text: str = "...") -> None:
+	def fail(self, message_text: str) -> None:
 		"""
 		Fail information logging:
 		Used to log entry a message about the failed execution of the process.
 
 		:param message_text: Log entry message
 		"""
-		self.__logger.entry(
-			entry_type=ServiceProcessEntryTypes.fail,
-			message_text=message_text
-		)
+		self.__logger.entry(ServiceProcessEntryTypes.fail, message_text)
```

### Comparing `mighty_logger-0.7.2/mighty_logger/src/__init__.py` & `mighty_logger-0.8.0/mighty_logger/src/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,8 +23,7 @@
 	AnsiColor,\
 	Dec2Hex,\
 	Dec2Ansi,\
 	Hex2Dec,\
 	Hex2Ansi,\
 	Ansi2Dec,\
 	Ansi2Hex
-from .text_buffer import BasicTextBuffer, TextBuffer
```

### Comparing `mighty_logger-0.7.2/mighty_logger/src/animations.py` & `mighty_logger-0.8.0/mighty_logger/src/animations.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/src/ansi_format.py` & `mighty_logger-0.8.0/mighty_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/src/color_picker.py` & `mighty_logger-0.8.0/mighty_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/__init__.py` & `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .entry_types import LoggerEntryTypes, ProcessEntryTypes, SelectionTypes, SelectionCategories
 from .environments import LogEnvironments
 from .sorting_keys import SortingKeys
-from .status_variables import StatusMessagePatterns
```

### Comparing `mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/entry_types.py` & `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/entry_types.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/environments.py` & `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/environments.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/src/lib_types_collection/sorting_keys.py` & `mighty_logger-0.8.0/mighty_logger/src/lib_types_collection/sorting_keys.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.7.2/mighty_logger/src/text_buffer.py` & `mighty_logger-0.8.0/mighty_logger/basic/text_buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import sys, re
+from re import sub
+from sys import stdout
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.basic.lib_types.text_buffer_type import TextBufferType
 from mighty_logger.basic.exceptions import ReCreationException, EnvironmentException
-from mighty_logger.basic.patterns import Singleton
+from mighty_logger.basic.singleton import Singleton
 from mighty_logger.src.lib_types_collection.environments import LogEnvironments
 
 class BasicTextBuffer(Singleton, TextBufferType):
 	"""
 	A class with a basic implementation of a simple text buffer. It is intended
 	to be used in conjunction with HTML, but this is optional.
 	"""
@@ -68,21 +69,21 @@
 			case LogEnvironments.CONSOLE.environment_name:
 				raise EnvironmentException("This environment is not supported")
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				raise EnvironmentException("This environment is not supported")
 			case LogEnvironments.HTML.environment_name:
 				with open(f"{name_file}.html", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
-						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join([entry for entry in self._text_buffer[1:] if re.sub(r"<.*?>", "", entry).startswith("-")]) + '</body></pre>')
+						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join([entry for entry in self._text_buffer[1:] if sub(r"<.*?>", "", entry).startswith("-")]) + '</body></pre>')
 					else:
 						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join(self._text_buffer[1:]) + '</body></pre>')
 			case LogEnvironments.MARKDOWN.environment_name:
 				with open(f"{name_file}.md", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
-						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join([entry for entry in self._text_buffer[1:] if re.sub(r"<.*?>", "", entry).startswith("-")]) + '</body></pre>')
+						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join([entry for entry in self._text_buffer[1:] if sub(r"<.*?>", "", entry).startswith("-")]) + '</body></pre>')
 					else:
 						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join(self._text_buffer[1:]) + '</body></pre>')
 			case LogEnvironments.PLAIN.environment_name:
 				with open(f"{name_file}.txt", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
 						text_buffer_file.write('\n'.join([entry for entry in self._text_buffer if entry.startswith("-")]))
 					else:
@@ -138,68 +139,68 @@
 			self._cursor_string: int = 0
 			self._buffer_size: int = 0
 			self.width = console_width
 		else:
 			raise ReCreationException("TextBuffer class object already created")
 
 	def append(self, message: str) -> None:
-		excess_console_string = len(re.sub(r"\033\[.*?m", "", message)) // self.width
+		excess_console_string = len(sub(r"\033\[.*?m", "", message)) // self.width
 		self._buffer_size += 1 + excess_console_string
 		self._text_buffer.append(f"{message}")
 
 	def insert(self, number_string: int, message: str) -> None:
 		if number_string > self._cursor_string:
 			count_empty_strings = (number_string - len(self._text_buffer))
 			self._text_buffer.extend([""] * count_empty_strings)
 			self._buffer_size += count_empty_strings
 			self.append(message)
 		else:
-			excess_console_string = len(re.sub(r"\033\[.*?m", "", message)) // self.width
+			excess_console_string = len(sub(r"\033\[.*?m", "", message)) // self.width
 			self._buffer_size += 1 + excess_console_string
 			self._text_buffer.insert(number_string, f"{message}")
 
 	def replace(self, number_string: int, message: str) -> None:
 		if number_string > self._cursor_string:
 			count_empty_strings = (number_string - len(self._text_buffer))
 			self._text_buffer.extend([""] * count_empty_strings)
 			self._buffer_size += count_empty_strings
 			self.append(message)
 		else:
-			old_excess_console_strings = len(re.sub(r"\033\[.*?m", "", self._text_buffer[number_string])) // self.width
-			new_excess_console_strings = len(re.sub(r"\033\[.*?m", "", message)) // self.width
+			old_excess_console_strings = len(sub(r"\033\[.*?m", "", self._text_buffer[number_string])) // self.width
+			new_excess_console_strings = len(sub(r"\033\[.*?m", "", message)) // self.width
 			self._buffer_size += new_excess_console_strings - old_excess_console_strings
 			self._text_buffer[number_string] = f"{message}"
 
 	def pop(self, number_string: int = -1) -> str:
-		excess_console_string = len(re.sub(r"\033\[.*?m", "", self._text_buffer[-1])) // self.width
+		excess_console_string = len(sub(r"\033\[.*?m", "", self._text_buffer[-1])) // self.width
 		self._buffer_size -= 1 + excess_console_string
 		last = self._text_buffer.pop(number_string)
 		return last
 
 	def remove(self, number_string: int = -1) -> None:
-		excess_console_string = len(re.sub(r"\033\[.*?m", "", self._text_buffer[-1])) // self.width
+		excess_console_string = len(sub(r"\033\[.*?m", "", self._text_buffer[-1])) // self.width
 		self._buffer_size -= 1 + excess_console_string
 		self._text_buffer.pop(number_string)
 
 	def clear(self) -> None:
 		if self._cursor_string == 0:
-			sys.stdout.write(f'\r\033[K')
+			stdout.write(f'\r\033[K')
 		else:
-			sys.stdout.write(f'\033[{self._cursor_string}A\r\033[J')
+			stdout.write(f'\033[{self._cursor_string}A\r\033[J')
 		self._text_buffer.clear()
-		sys.stdout.flush()  # Clearing the output buffer so that the changes are displayed immediately
+		stdout.flush()
 		self._buffer_size = 0
 		self._cursor_string = 0
 
 	def save(self, name_file: str, clean: bool) -> None:
 		match self._environment.environment_name:
 			case LogEnvironments.CONSOLE.environment_name:
 				with open(f"{name_file}.contxt", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
-						text_buffer_file.write('\n'.join([entry for entry in self._text_buffer if re.sub(r"\033\[.*?m", "", entry).startswith("-")]))
+						text_buffer_file.write('\n'.join([entry for entry in self._text_buffer if sub(r"\033\[.*?m", "", entry).startswith("-")]))
 					else:
 						text_buffer_file.write('\n'.join(self._text_buffer))
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				with open(f"{name_file}.txt", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
 						text_buffer_file.write('\n'.join([entry for entry in self._text_buffer if entry.startswith("-")]))
 					else:
@@ -230,23 +231,24 @@
 			case LogEnvironments.MARKDOWN.environment_name:
 				raise EnvironmentException("This environment is not supported")
 			case LogEnvironments.PLAIN.environment_name:
 				raise EnvironmentException("This environment is not supported")
 
 	def input(self, input_text: str) -> str:
 		data = input(f"\r{input_text}")
-		sys.stdout.write(f'\033[1A')
+		stdout.write(f'\033[1A')
+		stdout.flush()
 		return data
 
 	def update_console(self) -> None:
 		if self._cursor_string == 0:
-			sys.stdout.write(f'\r\033[K')
+			stdout.write(f'\r\033[K')
 		else:
-			sys.stdout.write(f'\033[{self._cursor_string}A\r\033[J')
-		sys.stdout.write('\n'.join(self._text_buffer))
-		sys.stdout.flush()  # Clearing the output buffer so that the changes are displayed immediately
+			stdout.write(f'\033[{self._cursor_string}A\r\033[J')
+		stdout.write('\n'.join(self._text_buffer))
+		stdout.flush()
 		self._cursor_string = self._buffer_size - 1
 
 	def update_entry(self) -> None:
-		sys.stdout.write(f'\r')
-		sys.stdout.write(self._text_buffer[-1])
-		sys.stdout.flush()  # Clearing the output buffer so that the changes are displayed immediately
+		stdout.write(f'\r')
+		stdout.write(self._text_buffer[-1])
+		stdout.flush()
```

### Comparing `mighty_logger-0.7.2/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.8.0/mighty_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mighty-logger
-Version: 0.7.2
+Version: 0.8.0
 Summary: Powerful functional logger
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -106,15 +106,15 @@
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
 - [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
-- [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
+- [x] v0.8.0 - Export update (added conversion to csv)
 - [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
```

### Comparing `mighty_logger-0.7.2/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.8.0/mighty_logger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 mighty_logger.egg-info/PKG-INFO
 mighty_logger.egg-info/SOURCES.txt
 mighty_logger.egg-info/dependency_links.txt
 mighty_logger.egg-info/top_level.txt
 mighty_logger/basic/__init__.py
 mighty_logger/basic/basic_logger.py
 mighty_logger/basic/exceptions.py
+mighty_logger/basic/exporter.py
 mighty_logger/basic/modifier.py
-mighty_logger/basic/patterns.py
+mighty_logger/basic/singleton.py
+mighty_logger/basic/text_buffer.py
 mighty_logger/basic/lib_types/__init__.py
 mighty_logger/basic/lib_types/animation_type.py
 mighty_logger/basic/lib_types/entry_type.py
 mighty_logger/basic/lib_types/environment_type.py
 mighty_logger/basic/lib_types/sorting_key_type.py
-mighty_logger/basic/lib_types/status_message_type.py
 mighty_logger/basic/lib_types/text_buffer_type.py
 mighty_logger/src/__init__.py
 mighty_logger/src/animations.py
 mighty_logger/src/ansi_format.py
 mighty_logger/src/color_picker.py
-mighty_logger/src/text_buffer.py
 mighty_logger/src/lib_types_collection/__init__.py
 mighty_logger/src/lib_types_collection/entry_types.py
 mighty_logger/src/lib_types_collection/environments.py
 mighty_logger/src/lib_types_collection/sorting_keys.py
-mighty_logger/src/lib_types_collection/status_variables.py
 test/test.py
 test/test_simple.py
```

### Comparing `mighty_logger-0.7.2/setup.py` & `mighty_logger-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mighty_logger",
-    version="0.7.2",
+    version="0.8.0",
 
     author="Kalynovsky 'Nakamura Akira' Valentin",
     author_email="nakama3942@gmail.com",
 
     description="Powerful functional logger",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `mighty_logger-0.7.2/test/test.py` & `mighty_logger-0.8.0/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	ProcessEntryTypes,\
 	LogEnvironments,\
 	SortingKeys,\
 	SelectionTypes
 from mighty_logger.src import IndefiniteAnimations, DefiniteAnimations
 
 if __name__ == "__main__":
-	logger = MightyLogger(program_name="Installer", log_environment=LogEnvironments.CONSOLE, console_width=115, status_message_global_entry=False)
+	logger = MightyLogger(program_name="Installer", log_environment=LogEnvironments.CONSOLE, console_width=115)
 	logger.publish_author()
 
 	logger.start_timer(message_text="Timer started")
 	logger.entry(entry_type=LoggerEntryTypes.message, message_text="Program installation started")
 
 	sleep(1)
 	logger.start_indefinite_process(animation=IndefiniteAnimations.SuperSpace, message_text="File upload")
@@ -96,7 +96,9 @@
 	logger.sort(SortingKeys.SORT_ON_TYPE)
 	# logger.sort_with_save(SortingKeys.SORT_ON_TYPE)
 	# logger.search("o", True)
 	# logger.search_with_save("o", True)
 	# logger.select(SelectionTypes.initiation)
 	# logger.select_with_save(SelectionTypes.initiation)
 	logger.entry(entry_type=LoggerEntryTypes.info, message_text="Logger sorted")
+
+	logger.export_to_csv("export_logs")
```

### Comparing `mighty_logger-0.7.2/test/test_simple.py` & `mighty_logger-0.8.0/test/test_simple.py`

 * *Files identical despite different names*

