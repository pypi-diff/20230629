# Comparing `tmp/rtfparse-0.7.8.tar.gz` & `tmp/rtfparse-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtfparse-0.7.8.tar", last modified: Wed Jan  6 04:47:48 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `rtfparse-0.7.8.tar` & `rtfparse-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,21 @@
-drwxrwxrwx   0        0        0        0 2021-01-06 04:47:48.334867 rtfparse-0.7.8/
--rw-rw-rw-   0        0        0     5350 2021-01-06 04:47:48.331875 rtfparse-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     3699 2021-01-06 04:22:51.000000 rtfparse-0.7.8/README.md
--rw-rw-rw-   0        0        0       42 2021-01-06 04:47:48.334867 rtfparse-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     2914 2021-01-05 08:36:11.000000 rtfparse-0.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-06 04:47:48.266860 rtfparse-0.7.8/src/
-drwxrwxrwx   0        0        0        0 2021-01-06 04:47:48.306896 rtfparse-0.7.8/src/rtfparse/
--rw-rw-rw-   0        0        0      245 2021-01-05 08:24:11.000000 rtfparse-0.7.8/src/rtfparse/__init__.py
--rw-rw-rw-   0        0        0      214 2020-12-24 04:53:39.000000 rtfparse-0.7.8/src/rtfparse/__main__.py
--rw-rw-rw-   0        0        0    10285 2021-01-01 16:38:55.000000 rtfparse-0.7.8/src/rtfparse/config_loader.py
--rw-rw-rw-   0        0        0     8911 2021-01-04 16:07:51.000000 rtfparse-0.7.8/src/rtfparse/entities.py
--rw-rw-rw-   0        0        0     4759 2021-01-06 04:47:36.000000 rtfparse-0.7.8/src/rtfparse/entry.py
--rw-rw-rw-   0        0        0      280 2020-12-24 10:08:50.000000 rtfparse-0.7.8/src/rtfparse/enums.py
--rw-rw-rw-   0        0        0      409 2020-12-26 06:18:34.000000 rtfparse-0.7.8/src/rtfparse/errors.py
--rw-rw-rw-   0        0        0     3520 2020-12-27 13:42:35.000000 rtfparse-0.7.8/src/rtfparse/logging_conf.py
--rw-rw-rw-   0        0        0     3125 2020-12-24 04:10:02.000000 rtfparse-0.7.8/src/rtfparse/menu.py
--rw-rw-rw-   0        0        0      511 2021-01-06 04:47:36.000000 rtfparse-0.7.8/src/rtfparse/minimal.py
--rw-rw-rw-   0        0        0     3217 2021-01-05 08:24:11.000000 rtfparse-0.7.8/src/rtfparse/parser.py
--rw-rw-rw-   0        0        0     3898 2021-01-06 04:22:51.000000 rtfparse-0.7.8/src/rtfparse/re_patterns.py
-drwxrwxrwx   0        0        0        0 2021-01-06 04:47:48.328866 rtfparse-0.7.8/src/rtfparse/renderers/
--rw-rw-rw-   0        0        0       96 2020-12-27 18:23:01.000000 rtfparse-0.7.8/src/rtfparse/renderers/__init__.py
--rw-rw-rw-   0        0        0     3520 2021-01-04 16:07:51.000000 rtfparse-0.7.8/src/rtfparse/renderers/de_encapsulate_html.py
--rw-rw-rw-   0        0        0     2046 2021-01-02 11:42:05.000000 rtfparse-0.7.8/src/rtfparse/utils.py
--rw-rw-rw-   0        0        0       46 2021-01-06 04:47:36.000000 rtfparse-0.7.8/src/rtfparse/version.py
-drwxrwxrwx   0        0        0        0 2021-01-06 04:47:48.324874 rtfparse-0.7.8/src/rtfparse.egg-info/
--rw-rw-rw-   0        0        0     5350 2021-01-06 04:47:48.000000 rtfparse-0.7.8/src/rtfparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      660 2021-01-06 04:47:48.000000 rtfparse-0.7.8/src/rtfparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-06 04:47:48.000000 rtfparse-0.7.8/src/rtfparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2021-01-06 04:47:48.000000 rtfparse-0.7.8/src/rtfparse.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2021-01-06 04:47:48.000000 rtfparse-0.7.8/src/rtfparse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-01-06 04:47:48.000000 rtfparse-0.7.8/src/rtfparse.egg-info/top_level.txt
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 rtfparse-0.8.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 rtfparse-0.8.0/release.cmd
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 rtfparse-0.8.0/requirements.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 rtfparse-0.8.0/changelog.d/changelog_template.jinja
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/__about__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/__init__.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/cli.py
+-rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/entities.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/enums.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/logging_conf.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/minimal.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/parser.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/re_patterns.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/utils.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/renderers/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/renderers/de_encapsulate_html.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 rtfparse-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 rtfparse-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 rtfparse-0.8.0/README.md
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 rtfparse-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 rtfparse-0.8.0/PKG-INFO
```

### Comparing `rtfparse-0.7.8/src/rtfparse/entities.py` & `rtfparse-0.8.0/src/rtfparse/entities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,198 +1,210 @@
-#!/usr/bin/env python
-
-
-import io
-import logging
-import re
-# Own modules
-from rtfparse import re_patterns
-from rtfparse import utils
-from rtfparse import errors
-from rtfparse.enums import Bytestring_Type
-
-
-# Setup logging
-logger = logging.getLogger(__name__)
-
-
-# Constants, number of bytes to read when creating entities
-CHARACTER = BACKSLASH = DELIMITER = MINUS = GROUP_END = len(b"\\")
-SYMBOL = IGNORABLE = BACKSLASH + CHARACTER
-GROUP_START = BACKSLASH + IGNORABLE
-MAX_CW_LETTERS = 32 # As specified in RTF Spec
-INTEGER_MAGNITUDE = 32 # As specified in RTF Spec
-PLAIN_TEXT = CONTROL_WORD = BACKSLASH + MAX_CW_LETTERS + MINUS + len(str((1 << INTEGER_MAGNITUDE) // 2)) + DELIMITER
-
-
-class Entity:
-    def __init__(self) -> None:
-        self.text = ""
-    @classmethod
-    def probe(cls, pattern: re_patterns.Bytes_Regex, file: io.BufferedReader) -> Bytestring_Type:
-        logger.debug(f"Probing file at position {file.tell()}")
-        original_position = file.tell()
-        while True:
-            probed = file.read(len(re_patterns.probe_pattern))
-            logger.debug(f"{probed = }")
-            file.seek(original_position)
-            logger.debug(f"Probe returned to position {file.tell()}")
-            if (match := re_patterns.group_start.match(probed)):
-                result = Bytestring_Type.GROUP_START
-            elif (match := re_patterns.group_end.match(probed)):
-                result = Bytestring_Type.GROUP_END
-            elif (match := re_patterns.control_word.match(probed)):
-                result = Bytestring_Type.CONTROL_WORD
-            elif (match := re_patterns.control_symbol.match(probed)):
-                result = Bytestring_Type.CONTROL_SYMBOL
-            elif (match := re_patterns.plain_text.match(probed)):
-                result = Bytestring_Type.PLAIN_TEXT
-            else:
-                logger.debug(f"This does not match anything, it's probably a newline, moving on")
-                original_position += 1
-                file.seek(original_position)
-                logger.debug(f"Probe moved to position {file.tell()}")
-                if not probed:
-                    logger.debug(f"Reached unexpected end of file.")
-                    result = Bytestring_Type.GROUP_END
-                    break
-                    # raise errors.UnexpectedEndOfFileError(f"at position {file.tell()}")
-                continue
-            break
-        logger.debug(f"Probe {result = }")
-        logger.debug(f"Probe leaving file at position {file.tell()}")
-        return result
-
-
-class Control_Word(Entity):
-    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
-        super().__init__()
-        self.encoding = encoding
-        logger.debug(f"Reading Control Word at file position {file.tell()}")
-        self.control_name = "missing"
-        self.parameter = ""
-        self.bindata = b""
-        self.start_position = file.tell()
-        logger.debug(f"Starting at file position {self.start_position}")
-        probe = file.read(CONTROL_WORD)
-        if (match := re_patterns.control_word.match(probe)):
-            self.control_name = match.group("control_name").decode(self.encoding)
-            logger.debug(f"Preliminary {self.control_name = }")
-            parameter = match.group("parameter")
-            if parameter is not None:
-                self.parameter = int(parameter.decode(self.encoding))
-                logger.debug(f"{self.parameter = }")
-                self.control_name = self.control_name.removesuffix(str(self.parameter))
-                logger.debug(f"Final {self.control_name = }")
-            target_position = self.start_position + match.span()[1]
-            if match.group("other"):
-                logger.debug(f"Delimiter is {match.group('other').decode(self.encoding)}, len: {len(match.group('delimiter'))}")
-                target_position -= len(match.group("delimiter"))
-            file.seek(target_position)
-            # handle \binN:
-            if self.control_name == "bin":
-               self.bindata = file.read(utils.twos_complement(self.parameter, INTEGER_MAGNITUDE))
-        else:
-            logger.warning(f"Missing Control Word")
-            file.seek(self.start_position)
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}: {self.control_name}{self.parameter}>"
-
-
-class Control_Symbol(Entity):
-    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
-        super().__init__()
-        self.encoding = encoding
-        self.start_position = file.tell()
-        logger.debug(f"Reading Symbol at file position {self.start_position}")
-        self.char = ""
-        self.text = chr(file.read(SYMBOL)[-1])
-        if self.text == "'":
-            self.char = file.read(SYMBOL).decode(self.encoding)
-            self.text = bytes((int(self.char, base=16), )).decode(self.encoding)
-            logger.debug(f"Encountered escaped ANSI character, read two more bytes: {self.char}, character: {self.text}")
-            if self.text in "\\{}":
-                file.seek(file.tell() - SYMBOL)
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}: {self.text}>"
-
-
-class Plain_Text(Entity):
-    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
-        super().__init__()
-        self.encoding = encoding
-        self.text = ""
-        logger.debug(f"Constructing Plain_Text")
-        while True:
-            self.start_position = file.tell()
-            read = file.read(PLAIN_TEXT)
-            logger.debug(f"Read file from {self.start_position} to position {file.tell()}, read: {read}")
-            # see if we have read all the plain text there is:
-            if (match := re_patterns.plain_text.match(read)):
-                logger.debug(f"This matches the plain text pattern")
-                _text = match.group("text").decode(self.encoding)
-                logger.debug(f"{_text = }")
-                self.text = "".join((self.text, _text))
-                logger.debug(f"{self.text = }")
-                if len(_text) == PLAIN_TEXT:
-                    continue
-                else:
-                    file.seek(self.start_position + len(_text))
-                    break
-            else:
-                file.seek(self.start_position)
-                break
-        logger.debug(f"Returned to position {file.tell()}")
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}: {self.text}>"
-
-
-class Group(Entity):
-    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
-        super().__init__()
-        logger.debug(f"Group.__init__")
-        self.encoding = encoding
-        self.known = False
-        self.name = "unknown"
-        self.ignorable = False
-        self.structure = list()
-        parsed_object = utils.what_is_being_parsed(file)
-        logger.debug(f"Creating destination group from {parsed_object}")
-        self.start_position = file.tell()
-        logger.debug(f"Starting at file position {self.start_position}")
-        probe = file.read(GROUP_START)
-        logger.debug(f"Read file up to position {file.tell()}, read {probe = }")
-        if (match := re_patterns.group_start.match(probe)):
-            self.known = bool(match.group("group_start"))
-            self.ignorable = bool(match.group("ignorable"))
-            if not self.ignorable:
-                file.seek(self.start_position + GROUP_START - IGNORABLE)
-                logger.debug(f"Returned to position {file.tell()}")
-        else:
-            logger.warning(utils.warn(f"Expected a group but found no group start. Creating unknown group"))
-            file.seek(self.start_position)
-        while True:
-            probed = self.probe(re_patterns.probe, file)
-            if probed is Bytestring_Type.CONTROL_WORD:
-                self.structure.append(Control_Word(self.encoding, file))
-            elif probed is Bytestring_Type.GROUP_END:
-                file.read(GROUP_END)
-                break
-            elif probed is Bytestring_Type.GROUP_START:
-                self.structure.append(Group(self.encoding, file))
-            elif probed is Bytestring_Type.CONTROL_SYMBOL:
-                self.structure.append(Control_Symbol(self.encoding, file))
-            else:
-                self.structure.append(Plain_Text(self.encoding, file))
-        # name the group like its first Control Word
-        # this way the renderer will be able to ignore entire groups based on their first control word
-        try:
-            if isinstance(self.structure[0], Control_Word):
-                self.name = self.structure[0].control_name
-        except IndexError:
-            pass
-    def __repr__(self) -> str:
-        return f"<Group {self.name}>"
-
-
-if __name__ == "__main__":
-    pass
+#!/usr/bin/env python
+
+
+import io
+import logging
+import re
+
+# Own modules
+from rtfparse import re_patterns, utils
+from rtfparse.enums import Bytestring_Type
+
+# Setup logging
+logger = logging.getLogger(__name__)
+
+
+# Constants, number of bytes to read when creating entities
+CHARACTER = BACKSLASH = DELIMITER = MINUS = GROUP_END = len(b"\\")
+SYMBOL = IGNORABLE = BACKSLASH + CHARACTER
+GROUP_START = BACKSLASH + IGNORABLE
+MAX_CW_LETTERS = 32  # As specified in RTF Spec
+INTEGER_MAGNITUDE = 32  # As specified in RTF Spec
+PLAIN_TEXT = CONTROL_WORD = (
+    BACKSLASH + MAX_CW_LETTERS + MINUS + len(str((1 << INTEGER_MAGNITUDE) // 2)) + DELIMITER
+)
+
+
+class Entity:
+    def __init__(self) -> None:
+        self.text = ""
+
+    @classmethod
+    def probe(cls, pattern: re_patterns.Bytes_Regex, file: io.BufferedReader) -> Bytestring_Type:
+        logger.debug(f"Probing file at position {file.tell()}")
+        original_position = file.tell()
+        while True:
+            probed = file.read(len(re_patterns.probe_pattern))
+            logger.debug(f"{probed = }")
+            file.seek(original_position)
+            logger.debug(f"Probe returned to position {file.tell()}")
+            if match := re_patterns.group_start.match(probed):
+                result = Bytestring_Type.GROUP_START
+            elif match := re_patterns.group_end.match(probed):
+                result = Bytestring_Type.GROUP_END
+            elif match := re_patterns.control_word.match(probed):
+                result = Bytestring_Type.CONTROL_WORD
+            elif match := re_patterns.control_symbol.match(probed):
+                result = Bytestring_Type.CONTROL_SYMBOL
+            elif match := re_patterns.plain_text.match(probed):
+                result = Bytestring_Type.PLAIN_TEXT
+            else:
+                logger.debug(f"This does not match anything, it's probably a newline, moving on")
+                original_position += 1
+                file.seek(original_position)
+                logger.debug(f"Probe moved to position {file.tell()}")
+                if not probed:
+                    logger.debug(f"Reached unexpected end of file.")
+                    result = Bytestring_Type.GROUP_END
+                    break
+                continue
+            break
+        logger.debug(f"Probe {result = }")
+        logger.debug(f"Probe leaving file at position {file.tell()}")
+        return result
+
+
+class Control_Word(Entity):
+    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
+        super().__init__()
+        self.encoding = encoding
+        logger.debug(f"Reading Control Word at file position {file.tell()}")
+        self.control_name = "missing"
+        self.parameter = ""
+        self.bindata = b""
+        self.start_position = file.tell()
+        logger.debug(f"Starting at file position {self.start_position}")
+        probe = file.read(CONTROL_WORD)
+        if match := re_patterns.control_word.match(probe):
+            self.control_name = match.group("control_name").decode(self.encoding)
+            logger.debug(f"Preliminary {self.control_name = }")
+            parameter = match.group("parameter")
+            if parameter is not None:
+                self.parameter = int(parameter.decode(self.encoding))
+                logger.debug(f"{self.parameter = }")
+                self.control_name = self.control_name.removesuffix(str(self.parameter))
+                logger.debug(f"Final {self.control_name = }")
+            target_position = self.start_position + match.span()[1]
+            if match.group("other"):
+                logger.debug(
+                    f"Delimiter is {match.group('other').decode(self.encoding)}, len: {len(match.group('delimiter'))}"
+                )
+                target_position -= len(match.group("delimiter"))
+            file.seek(target_position)
+            # handle \binN:
+            if self.control_name == "bin":
+                self.bindata = file.read(utils.twos_complement(self.parameter, INTEGER_MAGNITUDE))
+        else:
+            logger.warning(f"Missing Control Word")
+            file.seek(self.start_position)
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}: {self.control_name}{self.parameter}>"
+
+
+class Control_Symbol(Entity):
+    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
+        super().__init__()
+        self.encoding = encoding
+        self.start_position = file.tell()
+        logger.debug(f"Reading Symbol at file position {self.start_position}")
+        self.char = ""
+        self.text = chr(file.read(SYMBOL)[-1])
+        if self.text == "'":
+            self.char = file.read(SYMBOL).decode(self.encoding)
+            self.text = bytes((int(self.char, base=16),)).decode(self.encoding)
+            logger.debug(
+                f"Encountered escaped ANSI character, read two more bytes: {self.char}, character: {self.text}"
+            )
+            if self.text in "\\{}":
+                file.seek(file.tell() - SYMBOL)
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}: {self.text}>"
+
+
+class Plain_Text(Entity):
+    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
+        super().__init__()
+        self.encoding = encoding
+        self.text = ""
+        logger.debug(f"Constructing Plain_Text")
+        while True:
+            self.start_position = file.tell()
+            read = file.read(PLAIN_TEXT)
+            logger.debug(
+                f"Read file from {self.start_position} to position {file.tell()}, read: {read}"
+            )
+            # see if we have read all the plain text there is:
+            if match := re_patterns.plain_text.match(read):
+                logger.debug(f"This matches the plain text pattern")
+                _text = match.group("text").decode(self.encoding)
+                logger.debug(f"{_text = }")
+                self.text = "".join((self.text, _text))
+                logger.debug(f"{self.text = }")
+                if len(_text) == PLAIN_TEXT:
+                    continue
+                else:
+                    file.seek(self.start_position + len(_text))
+                    break
+            else:
+                file.seek(self.start_position)
+                break
+        logger.debug(f"Returned to position {file.tell()}")
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}: {self.text}>"
+
+
+class Group(Entity):
+    def __init__(self, encoding: str, file: io.BufferedReader) -> None:
+        super().__init__()
+        logger.debug(f"Group.__init__")
+        self.encoding = encoding
+        self.known = False
+        self.name = "unknown"
+        self.ignorable = False
+        self.structure = list()
+        parsed_object = utils.what_is_being_parsed(file)
+        logger.debug(f"Creating destination group from {parsed_object}")
+        self.start_position = file.tell()
+        logger.debug(f"Starting at file position {self.start_position}")
+        probe = file.read(GROUP_START)
+        logger.debug(f"Read file up to position {file.tell()}, read {probe = }")
+        if match := re_patterns.group_start.match(probe):
+            self.known = bool(match.group("group_start"))
+            self.ignorable = bool(match.group("ignorable"))
+            if not self.ignorable:
+                file.seek(self.start_position + GROUP_START - IGNORABLE)
+                logger.debug(f"Returned to position {file.tell()}")
+        else:
+            logger.warning(
+                utils.warn(f"Expected a group but found no group start. Creating unknown group")
+            )
+            file.seek(self.start_position)
+        while True:
+            probed = self.probe(re_patterns.probe, file)
+            if probed is Bytestring_Type.CONTROL_WORD:
+                self.structure.append(Control_Word(self.encoding, file))
+            elif probed is Bytestring_Type.GROUP_END:
+                file.read(GROUP_END)
+                break
+            elif probed is Bytestring_Type.GROUP_START:
+                self.structure.append(Group(self.encoding, file))
+            elif probed is Bytestring_Type.CONTROL_SYMBOL:
+                self.structure.append(Control_Symbol(self.encoding, file))
+            else:
+                self.structure.append(Plain_Text(self.encoding, file))
+        # name the group like its first Control Word
+        # this way the renderer will be able to ignore entire groups based on their first control word
+        try:
+            if isinstance(self.structure[0], Control_Word):
+                self.name = self.structure[0].control_name
+        except IndexError:
+            pass
+
+    def __repr__(self) -> str:
+        return f"<Group {self.name}>"
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `rtfparse-0.7.8/src/rtfparse/entry.py` & `rtfparse-0.8.0/src/rtfparse/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,131 @@
 #!/usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 
-
-import pathlib
+import io
 import logging
 import logging.config
-import argparse
+from argparse import ArgumentParser, Namespace
+from pathlib import Path
+
 import argcomplete
-from argcomplete.completers import EnvironCompleter as EC
-from itertools import filterfalse
-import io
-import extract_msg as em
 import compressed_rtf as cr
-# Own modules
+import extract_msg as em
+from provide_dir import provide_dir
+
 from rtfparse import logging_conf
-from rtfparse import errors
-from rtfparse import utils
-from rtfparse import config_loader
-from rtfparse import version
+from rtfparse.__about__ import __version__
 from rtfparse.parser import Rtf_Parser
 from rtfparse.renderers import de_encapsulate_html
 
 
-# Setup logging
-def setup_logging_directory(directory: pathlib.Path) -> tuple[logging.Logger, pathlib.Path]:
+def setup_logger(directory: Path) -> logging.Logger:
     """
     Returns a logger and a path to directory where the logs are saved
     """
     try:
-        path_to_dir = utils.provide_dir(directory)
-        logger_config = logging_conf.create_dict_config(path_to_dir, "debug.log", "info.log", "errors.log")
+        provide_dir(directory)
+        logger_config = logging_conf.create_dict_config(
+            directory, "rtfparse.debug.log", "rtfparse.info.log", "rtfparse.errors.log"
+        )
     except FileExistsError:
-        logger.error(f"Failed to create the directory `{str(path_to_dir)}` because it already exists as a file.")
-        logger.error(f"Please create the directory `{str(path_to_dir)}`")
+        logger.error(
+            f"Failed to create the directory `{str(directory)}` because it already exists as a file."
+        )
+        logger.error(f"Please create the directory `{str(directory)}`")
     finally:
         logging.config.dictConfig(logger_config)
         logger = logging.getLogger(__name__)
-    return logger, path_to_dir
+    return logger
 
 
-logger, path_to_dir = setup_logging_directory(pathlib.Path.home() / utils.dir_name)
+logger = setup_logger(Path.home() / "rtfparse")
 
 
-def argument_parser() -> argparse.ArgumentParser:
+def argument_parser() -> ArgumentParser:
     """
     Creates an argument parser for command line arguments
     """
-    parser = argparse.ArgumentParser(description="RTF parser")
-    parser.add_argument("-v", "--version", action="store_true", help="print out rtfparse version and exit").completer = EC
-    parser.add_argument("--autoconfig", action="store_true", help="Configure rtfparse automatically").completer = EC
-    parser.add_argument("-f", "--file", action="store", metavar="PATH", type=pathlib.Path, help="path to the rtf file").completer = EC
-    parser.add_argument("-m", "--msg", action="store", metavar="PATH", type=pathlib.Path, help="Parse RTF from MS Outlook's .msg file").completer = EC
-    parser.add_argument("-d", "--de-encapsulate-html", action="store_true", help="De-encapsulate HTML from RTF").completer = EC
-    parser.add_argument("-i", "--embed-img", action="store_true", help="Embed images from email to HTML").completer = EC
+    parser = ArgumentParser(description="RTF parser", prog="rtfparse")
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="version",
+        version=" ".join(("%(prog)s", __version__)),
+        help="print out rtfparse version and exit",
+    )
+    parser.add_argument(
+        "-r", "--rtf-file", action="store", metavar="PATH", type=Path, help="path to the rtf file"
+    )
+    parser.add_argument(
+        "-m",
+        "--msg-file",
+        action="store",
+        metavar="PATH",
+        type=Path,
+        help="Parse RTF from MS Outlook's .msg file",
+    )
+    parser.add_argument(
+        "-d", "--de-encapsulate-html", action="store_true", help="De-encapsulate HTML from RTF"
+    )
+    parser.add_argument(
+        "-i", "--embed-img", action="store_true", help="Embed images from email to HTML"
+    )
+    parser.add_argument(
+        "-o", "--output-file", metavar="PATH", type=Path, help="path to the desired output file"
+    )
+    parser.add_argument(
+        "-a",
+        "--attachments-dir",
+        metavar="PATH",
+        type=Path,
+        help="path to directory where to save email attachments",
+    )
     return parser
 
 
-def de_encapsulate(rp: Rtf_Parser, target_file: pathlib.Path) -> None:
+def de_encapsulate(rp: Rtf_Parser, target_file: Path) -> None:
     renderer = de_encapsulate_html.De_encapsulate_HTML()
     with open(target_file, mode="w", encoding="utf-8") as htmlfile:
         logger.info(f"Rendering the encapsulated HTML")
         renderer.render(rp.parsed, htmlfile)
         logger.info(f"Encapsulated HTML rendered")
 
 
-def run(config: config_loader.Config) -> None:
-    if config.cli_args.file and config.cli_args.file.exists():
-        file_name = config.cli_args.file.name
-        with open(config.cli_args.file, mode="rb") as rtf_file:
+def run(cli_args: Namespace) -> None:
+    if cli_args.rtf_file and cli_args.rtf_file.exists():
+        with open(cli_args.rtf_file, mode="rb") as rtf_file:
             rp = Rtf_Parser(rtf_file=rtf_file)
             rp.parse_file()
-    elif config.cli_args.msg:
-        file_name = config.cli_args.msg.name
-        msg = em.openMsg(f"{config.cli_args.msg}")
-        for attachment in msg.attachments:
-            with open(config.html / f"{attachment.longFilename}", mode="wb") as att_file:
-                att_file.write(attachment.data)
+    elif cli_args.msg_file:
+        msg = em.openMsg(f"{cli_args.msg_file}")
+        if cli_args.attachments_dir:
+            provide_dir(cli_args.attachments_dir)
+            for attachment in msg.attachments:
+                with open(
+                    cli_args.attachments_dir / f"{attachment.longFilename}", mode="wb"
+                ) as att_file:
+                    att_file.write(attachment.data)
         decompressed_rtf = cr.decompress(msg.compressedRtf)
-        with open((config.email_rtf / config.cli_args.msg.name).with_suffix(".rtf"), mode="wb") as email_rtf:
+        with open(cli_args.msg_file.with_suffix(".rtf"), mode="wb") as email_rtf:
             email_rtf.write(decompressed_rtf)
         with io.BytesIO(decompressed_rtf) as rtf_file:
             rp = Rtf_Parser(rtf_file=rtf_file)
             rp.parse_file()
-    if config.cli_args.de_encapsulate_html:
-        de_encapsulate(rp, (config.html / file_name).with_suffix(".html"))
+    if cli_args.de_encapsulate_html and cli_args.output_file:
+        de_encapsulate(rp, cli_args.output_file.with_suffix(".html"))
 
 
-def cli_start(version) -> None:
+def main() -> None:
     """
     Entry point for any component start from the commmand line
     """
-    logger.debug(f"{utils.program_name} started")
+    logger.debug(f"rtfparse started")
     parser = argument_parser()
     argcomplete.autocomplete(parser)
     cli_args = parser.parse_args()
     logger.debug(f"Parsed arguments: {cli_args}")
-    path_to_config = path_to_dir / utils.configuration_file_name
     try:
-        if cli_args.version:
-            logger.info(f"{version}")
-        else:
-            with config_loader.Config(path_to_config, cli_args.autoconfig) as config:
-                config.cli_args = cli_args
-                run(config)
-    except errors.WrongConfiguration as err:
-        logger.error(err.message)
+        run(cli_args)
     except Exception as err:
         logger.exception(f"Uncaught exception {repr(err)} occurred.")
-    logger.debug(f"{utils.program_name} ended")
-
-
-if __name__ == "__main__":
-    pass
+    logger.debug(f"rtfparse ended")
```

### Comparing `rtfparse-0.7.8/src/rtfparse/logging_conf.py` & `rtfparse-0.8.0/src/rtfparse/logging_conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,124 @@
-#!/usr/bin/env python
-
-# Logger Configuration module
-# Import this for easy logger configuration
-# See example in the comment of the set_logfile_path function below
-
-# Author: Sven Siegmund
-# Version 4
-
-"""
-This is to easily set the logfile name for the root logger's
-file handler from the module where logging_conf
-is imported. Like this:
-
-    import logging_conf
-    logging.config.dictConfig(logging_conf.create_dict_cofig(pathlib.Path.home(), "debug.log", "info.log", "error.log")
-    logging.getLogger()
-
-If you want an additional custom logger, get it like this:
-
-    logger = logging.getLogger("custom_logger")
-
-The custom logger is configured to propagate its log records to the root logger
-"""
-
-
-import pathlib
-
-
-def create_dict_config(directory: pathlib.Path, all_log: str, info_log: str, error_log: str) -> dict:
-    """
-    Creates a logging configuration with path to logfiles set as
-    given by the arguments
-    """
-    file_formatter_conf = {
-        "format": "{message:<50s} {levelname:>9s} {asctime}.{msecs:03.0f} {module} {funcName} ",
-        "style": "{",
-        # "datefmt": "%Y-%m-%d %H:%M:%S",
-        "datefmt": "%H:%M:%S",
-    }
-
-    console_formatter_conf = {
-        "format": "{message}",
-        # "format": "{asctime},{msecs:03.0f} {levelname:>9s} {module} {funcName}: {message}",
-        "style": "{",
-        "datefmt": "%a %H:%M:%S",
-    }
-
-    formatters_dict = {
-        "file_formatter": file_formatter_conf,
-        "console_formatter": console_formatter_conf,
-    }
-
-    root_console_handler_conf = {
-        "class": "logging.StreamHandler",
-        "level": "INFO",
-        "formatter": "console_formatter",
-        "stream": "ext://sys.stdout",
-    }
-
-    root_file_handler_conf = {
-        "class": "logging.FileHandler",
-        "level": "DEBUG",
-        "formatter": "file_formatter",
-        "filename": directory / all_log,
-        "mode": "w",
-        "encoding": "utf-8",
-    }
-
-    custom_error_file_handler_conf = {
-        "class": "logging.FileHandler",
-        "level": "ERROR",
-        "formatter": "file_formatter",
-        "filename": directory / error_log,
-        "mode": "w",
-        "encoding": "utf-8",
-    }
-
-    custom_info_file_handler_conf = {
-        "class": "logging.FileHandler",
-        "level": "INFO",
-        "formatter": "file_formatter",
-        "filename": directory / info_log,
-        "mode": "w",
-        "encoding": "utf-8",
-    }
-
-    handlers_dict = {
-        "root_console_handler": root_console_handler_conf,
-        "root_file_handler": root_file_handler_conf,
-        "custom_error_file_handler": custom_error_file_handler_conf,
-        "custom_info_file_handler": custom_info_file_handler_conf,
-    }
-
-    custom_logger_conf = {
-        "propagate": True,
-        "handlers": ["custom_error_file_handler", "custom_info_file_handler"],
-        "level": "DEBUG",
-    }
-
-    root_logger_conf = {
-        "handlers": ["root_file_handler", "root_console_handler", "custom_error_file_handler", "custom_info_file_handler"],
-        "level": "DEBUG",
-    }
-
-    loggers_dict = {
-        "custom_logger": custom_logger_conf,
-    }
-
-    dict_config = {
-        "version": 1,
-        "disable_existing_loggers": False,
-        "formatters": formatters_dict,
-        "handlers": handlers_dict,
-        "loggers": loggers_dict,
-        "root": root_logger_conf,
-        "incremental": False,
-    }
-    return dict_config
-
+#!/usr/bin/env python
+
+# Logger Configuration module
+# Import this for easy logger configuration
+# See example in the comment of the set_logfile_path function below
+
+# Author: Sven Siegmund
+# Version 4
+
+"""
+This is to easily set the logfile name for the root logger's
+file handler from the module where logging_conf
+is imported. Like this:
+
+    import logging_conf
+    logging.config.dictConfig(logging_conf.create_dict_cofig(pathlib.Path.home(), "debug.log", "info.log", "error.log")
+    logging.getLogger()
+
+If you want an additional custom logger, get it like this:
+
+    logger = logging.getLogger("custom_logger")
+
+The custom logger is configured to propagate its log records to the root logger
+"""
+
+
+import pathlib
+
+
+def create_dict_config(directory: pathlib.Path, all_log: str, info_log: str, error_log: str) -> dict:
+    """
+    Creates a logging configuration with path to logfiles set as
+    given by the arguments
+    """
+    file_formatter_conf = {
+        "format": "{message:<50s} {levelname:>9s} {asctime}.{msecs:03.0f} {module} {funcName} ",
+        "style": "{",
+        # "datefmt": "%Y-%m-%d %H:%M:%S",
+        "datefmt": "%H:%M:%S",
+    }
+
+    console_formatter_conf = {
+        "format": "{message}",
+        # "format": "{asctime},{msecs:03.0f} {levelname:>9s} {module} {funcName}: {message}",
+        "style": "{",
+        "datefmt": "%a %H:%M:%S",
+    }
+
+    formatters_dict = {
+        "file_formatter": file_formatter_conf,
+        "console_formatter": console_formatter_conf,
+    }
+
+    root_console_handler_conf = {
+        "class": "logging.StreamHandler",
+        "level": "INFO",
+        "formatter": "console_formatter",
+        "stream": "ext://sys.stdout",
+    }
+
+    root_file_handler_conf = {
+        "class": "logging.FileHandler",
+        "level": "DEBUG",
+        "formatter": "file_formatter",
+        "filename": directory / all_log,
+        "mode": "w",
+        "encoding": "utf-8",
+    }
+
+    custom_error_file_handler_conf = {
+        "class": "logging.FileHandler",
+        "level": "ERROR",
+        "formatter": "file_formatter",
+        "filename": directory / error_log,
+        "mode": "w",
+        "encoding": "utf-8",
+    }
+
+    custom_info_file_handler_conf = {
+        "class": "logging.FileHandler",
+        "level": "INFO",
+        "formatter": "file_formatter",
+        "filename": directory / info_log,
+        "mode": "w",
+        "encoding": "utf-8",
+    }
+
+    handlers_dict = {
+        "root_console_handler": root_console_handler_conf,
+        "root_file_handler": root_file_handler_conf,
+        "custom_error_file_handler": custom_error_file_handler_conf,
+        "custom_info_file_handler": custom_info_file_handler_conf,
+    }
+
+    custom_logger_conf = {
+        "propagate": True,
+        "handlers": ["custom_error_file_handler", "custom_info_file_handler"],
+        "level": "DEBUG",
+    }
+
+    root_logger_conf = {
+        "handlers": [
+            "root_file_handler",
+            "root_console_handler",
+            "custom_error_file_handler",
+            "custom_info_file_handler",
+        ],
+        "level": "DEBUG",
+    }
+
+    loggers_dict = {
+        "custom_logger": custom_logger_conf,
+    }
+
+    dict_config = {
+        "version": 1,
+        "disable_existing_loggers": False,
+        "formatters": formatters_dict,
+        "handlers": handlers_dict,
+        "loggers": loggers_dict,
+        "root": root_logger_conf,
+        "incremental": False,
+    }
+    return dict_config
```

### Comparing `rtfparse-0.7.8/src/rtfparse/parser.py` & `rtfparse-0.8.0/src/rtfparse/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,99 @@
-#!/usr/bin/env python
-
-
-import io
-import re
-import logging
-import pathlib
-# Own modules
-from rtfparse import re_patterns
-from rtfparse import entities
-from rtfparse import utils
-# Typing
-from typing import Optional
-from typing import Union
-from rtfparse import config_loader
-
-
-# Setup logging
-logger = logging.getLogger(__name__)
-
-
-class Rtf_Parser:
-    def __init__(self,
-                rtf_path: Optional[pathlib.Path]=None,
-                rtf_file: Optional[Union[io.BufferedReader, io.BytesIO]]=None,
-            ) -> None:
-        self.rtf_path = rtf_path
-        self.rtf_file = rtf_file
-        if not (self.rtf_path or self.rtf_file):
-            raise ValueError("Need `rtf_path` or `rtf_file` argument")
-        self.ENCODING_PROBE = 48 # look for encoding information in the first 48 bytes of the file
-    def read_encoding(self, file: Union[io.BufferedReader, io.BytesIO]) -> str:
-        probed = file.read(self.ENCODING_PROBE)
-        group = entities.Group("cp1252", io.BytesIO(probed))
-        recognized_encodings = (
-                    "ansi",
-                    "ansicpg",
-                    "mac",
-                    "pc",
-                    "pca",
-                )
-        # Gather all control words, which could define an encoding:
-        names = tuple(filter(lambda item: isinstance(item, entities.Control_Word) and item.control_name in recognized_encodings, group.structure))
-        # Check if the ANSI code page is set as a parameter of any of the control words:
-        cp = None
-        for item in names:
-            # if any item is a Control_Word which has a parameter, we assume that this is the parameter of \ansicpg, and that corresponds to the codepage we are looking for
-            if item.parameter:
-                param = item.parameter
-        if param:
-            encoding = f"cp{param}"
-        else:
-            if names[0].control_name == "ansi":
-                encoding = "ansi"
-            elif names[0].control_name == "mac":
-                encoding = "mac_roman"
-            elif names[0].control_name == "pc":
-                encoding = "cp437"
-            elif names[0].control_name == "pca":
-                encoding = "cp850"
-        file.seek(0)
-        logger.info(f"recognized encoding {encoding}")
-        return encoding
-    def parse_file(self) -> entities.Group:
-        if self.rtf_path is not None:
-            file = open(self.rtf_path, mode="rb")
-        elif self.rtf_file is not None:
-            file = self.rtf_file
-        else:
-            file = io.BytesIO(b"")
-        parsed_object = utils.what_is_being_parsed(file)
-        logger.info(f"Parsing the structure of {parsed_object}")
-        try:
-            encoding = self.read_encoding(file)
-            self.parsed = entities.Group(encoding, file)
-        except Exception as err:
-            logger.exception(err)
-        finally:
-            if self.rtf_path is not None:
-                logger.debug(f"Closing {parsed_object}")
-                file.close()
-            logger.info(f"Structure of {parsed_object} parsed")
-            return self.parsed
-
-
-if __name__ == "__main__":
-    pass
+#!/usr/bin/env python
+
+
+import io
+import logging
+import pathlib
+import re
+
+# Typing
+from typing import Optional, Union
+
+# Own modules
+from rtfparse import entities, re_patterns, utils
+
+# Setup logging
+logger = logging.getLogger(__name__)
+
+
+class Rtf_Parser:
+    def __init__(
+        self,
+        rtf_path: Optional[pathlib.Path] = None,
+        rtf_file: Optional[Union[io.BufferedReader, io.BytesIO]] = None,
+    ) -> None:
+        self.rtf_path = rtf_path
+        self.rtf_file = rtf_file
+        if not (self.rtf_path or self.rtf_file):
+            raise ValueError("Need `rtf_path` or `rtf_file` argument")
+        self.ENCODING_PROBE = 48  # look for encoding information in the first 48 bytes of the file
+
+    def read_encoding(self, file: Union[io.BufferedReader, io.BytesIO]) -> str:
+        probed = file.read(self.ENCODING_PROBE)
+        group = entities.Group("cp1252", io.BytesIO(probed))
+        recognized_encodings = (
+            "ansi",
+            "ansicpg",
+            "mac",
+            "pc",
+            "pca",
+        )
+        # Gather all control words, which could define an encoding:
+        names = tuple(
+            filter(
+                lambda item: isinstance(item, entities.Control_Word)
+                and item.control_name in recognized_encodings,
+                group.structure,
+            )
+        )
+        # Check if the ANSI code page is set as a parameter of any of the control words:
+        cp = None
+        for item in names:
+            # if any item is a Control_Word which has a parameter, we assume that this is the parameter of \ansicpg, and that corresponds to the codepage we are looking for
+            if item.parameter:
+                param = item.parameter
+        if param:
+            if param == 65001:
+                logger.warning(
+                    "Found encoding 65001, but often this is actually cp1252, so I'm overriding it"
+                )
+                encoding = "cp1252"
+            else:
+                encoding = f"cp{param}"
+        else:
+            if names[0].control_name == "ansi":
+                encoding = "ansi"
+            elif names[0].control_name == "mac":
+                encoding = "mac_roman"
+            elif names[0].control_name == "pc":
+                encoding = "cp437"
+            elif names[0].control_name == "pca":
+                encoding = "cp850"
+        file.seek(0)
+        logger.info(f"recognized encoding {encoding}")
+        return encoding
+
+    def parse_file(self) -> entities.Group:
+        if self.rtf_path is not None:
+            file = open(self.rtf_path, mode="rb")
+        elif self.rtf_file is not None:
+            file = self.rtf_file
+        else:
+            file = io.BytesIO(b"")
+        parsed_object = utils.what_is_being_parsed(file)
+        logger.info(f"Parsing the structure of {parsed_object}")
+        try:
+            encoding = self.read_encoding(file)
+            self.parsed = entities.Group(encoding, file)
+        except Exception as err:
+            logger.exception(err)
+        finally:
+            if self.rtf_path is not None:
+                logger.debug(f"Closing {parsed_object}")
+                file.close()
+            logger.info(f"Structure of {parsed_object} parsed")
+            return self.parsed
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `rtfparse-0.7.8/src/rtfparse/re_patterns.py` & `rtfparse-0.8.0/src/rtfparse/re_patterns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-#!/usr/bin/env python
-
-
-import re
-
-
-# Helper functions to construct raw regular expressions "strings" (actually byte strings)
-
-
-def group(content: bytes) -> bytes:
-    return rb"[" + content + rb"]"
-
-
-def named_regex_group(name: str, content: bytes) -> bytes:
-    group_start = rb"(?P<" + name.encode("ascii") + rb">"
-    group_end = rb")"
-    return rb"".join((group_start, content, group_end))
-
-
-def not_preceded_by(preceding: bytes, actual: bytes) -> bytes:
-    return rb"(?<!" + preceding + rb")" + actual
-
-
-def not_followed_by(preceding: bytes, actual: bytes) -> bytes:
-    return rb"(?<!" + preceding + rb")" + actual
-
-
-def no_capture(content: bytes) -> bytes:
-    return rb"(?:" + content + rb")"
-
-
-# Raw regular expression "strings"" (actually byte strings)
-
-
-_control_characters = rb"\\\{\}"
-_newline = b"\\" + rb"r" + b"\\" + rb"n"
-control_character = group(_control_characters)
-not_control_character = group(rb"^" + _control_characters)
-_control_characters_or_newline = _control_characters + _newline
-control_character_or_newline = group(_control_characters + _newline)
-not_control_character_or_newline = group(rb"^" + _control_characters_or_newline)
-rtf_backslash = named_regex_group("backslash", not_preceded_by(rb"\\", rb"\\"))
-unnamed_rtf_backslash = not_preceded_by(rb"\\", rb"\\")
-_letters = rb"a-zA-Z"
-ascii_letters = group(_letters) + rb"{1,32}"
-_digits = rb"0-9"
-_hdigits = rb"0-9a-f"
-ignorable = named_regex_group("ignorable", rb"\\\*")
-rtf_brace_open = named_regex_group("group_start", not_preceded_by(unnamed_rtf_backslash, rb"\{") + ignorable + rb"?")
-rtf_brace_close = named_regex_group("group_end", not_preceded_by(unnamed_rtf_backslash, rb"\}"))
-
-
-minus = named_regex_group("minus", rb"-?")
-digit = named_regex_group("digit", minus + group(_digits) + rb"{1,10}")
-hdigit = named_regex_group("hdigit", group(_hdigits))
-# int16 = minus + digit + rb"{1,5}"
-parameter_pattern = named_regex_group("parameter", digit)
-space = named_regex_group("space", rb" ")
-newline = named_regex_group("newline", _newline)
-other = named_regex_group("other", group(rb"^" + _letters + _digits))
-
-
-ascii_letter_sequence = named_regex_group("control_name", ascii_letters + parameter_pattern + rb"?")
-delimiter = named_regex_group("delimiter", rb"|".join((space, newline, other, rb"$")))
-symbol = named_regex_group("symbol", other)
-control_word_pattern = named_regex_group("control_word", rtf_backslash + ascii_letter_sequence + delimiter)
-pcdata_delimiter = no_capture(rb"|".join((rtf_brace_open, rtf_brace_close, control_word_pattern)))
-plain_text_pattern = named_regex_group("text", not_control_character_or_newline + rb"+") + no_capture(rb"|".join((control_character_or_newline, rb"$")))
-probe_pattern = rb".."
-
-
-class Bytes_Regex():
-    """
-    This wraps `re.pattern` objects and gives them a method `regex101` which
-    prints out the pattern in such a manner that it can be copy-pasted
-    to regex101.com.
-    """
-    def __init__(self, Bytes: bytes, flags:re.RegexFlag=0) -> None:
-        self.pattern_bytes = Bytes
-        self.pattern = re.compile(Bytes, flags)
-        self.match = self.pattern.match
-    def regex101(self) -> None:
-        print(self.pattern_bytes.decode("ascii"))
-
-
-meaningful_bs = Bytes_Regex(rtf_backslash)
-probe = Bytes_Regex(named_regex_group("probe", probe_pattern), flags=re.DOTALL)
-parameter = Bytes_Regex(parameter_pattern)
-control_word = Bytes_Regex(control_word_pattern)
-control_symbol = Bytes_Regex(rtf_backslash + symbol)
-group_start = Bytes_Regex(rtf_brace_open)
-group_end = Bytes_Regex(rtf_brace_close)
-plain_text = Bytes_Regex(plain_text_pattern)
-
-
-raw_pcdata = Bytes_Regex(named_regex_group("pcdata", rb".*?") + pcdata_delimiter, flags=re.DOTALL)
-raw_sdata = Bytes_Regex(named_regex_group("sdata", group(_hdigits + rb"\r\n") + rb"+"), flags=re.DOTALL)
+#!/usr/bin/env python
+
+
+import re
+
+# Helper functions to construct raw regular expressions "strings" (actually byte strings)
+
+
+def group(content: bytes) -> bytes:
+    return rb"[" + content + rb"]"
+
+
+def named_regex_group(name: str, content: bytes) -> bytes:
+    group_start = rb"(?P<" + name.encode("ascii") + rb">"
+    group_end = rb")"
+    return rb"".join((group_start, content, group_end))
+
+
+def not_preceded_by(preceding: bytes, actual: bytes) -> bytes:
+    return rb"(?<!" + preceding + rb")" + actual
+
+
+def not_followed_by(preceding: bytes, actual: bytes) -> bytes:
+    return rb"(?<!" + preceding + rb")" + actual
+
+
+def no_capture(content: bytes) -> bytes:
+    return rb"(?:" + content + rb")"
+
+
+# Raw regular expression "strings"" (actually byte strings)
+
+
+_control_characters = rb"\\\{\}"
+_newline = b"\\" + rb"r" + b"\\" + rb"n"
+control_character = group(_control_characters)
+not_control_character = group(rb"^" + _control_characters)
+_control_characters_or_newline = _control_characters + _newline
+control_character_or_newline = group(_control_characters + _newline)
+not_control_character_or_newline = group(rb"^" + _control_characters_or_newline)
+rtf_backslash = named_regex_group("backslash", not_preceded_by(rb"\\", rb"\\"))
+unnamed_rtf_backslash = not_preceded_by(rb"\\", rb"\\")
+_letters = rb"a-zA-Z"
+ascii_letters = group(_letters) + rb"{1,32}"
+_digits = rb"0-9"
+_hdigits = rb"0-9a-f"
+ignorable = named_regex_group("ignorable", rb"\\\*")
+rtf_brace_open = named_regex_group(
+    "group_start", not_preceded_by(unnamed_rtf_backslash, rb"\{") + ignorable + rb"?"
+)
+rtf_brace_close = named_regex_group("group_end", not_preceded_by(unnamed_rtf_backslash, rb"\}"))
+
+
+minus = named_regex_group("minus", rb"-?")
+digit = named_regex_group("digit", minus + group(_digits) + rb"{1,10}")
+hdigit = named_regex_group("hdigit", group(_hdigits))
+# int16 = minus + digit + rb"{1,5}"
+parameter_pattern = named_regex_group("parameter", digit)
+space = named_regex_group("space", rb" ")
+newline = named_regex_group("newline", _newline)
+other = named_regex_group("other", group(rb"^" + _letters + _digits))
+
+
+ascii_letter_sequence = named_regex_group("control_name", ascii_letters + parameter_pattern + rb"?")
+delimiter = named_regex_group("delimiter", rb"|".join((space, newline, other, rb"$")))
+symbol = named_regex_group("symbol", other)
+control_word_pattern = named_regex_group(
+    "control_word", rtf_backslash + ascii_letter_sequence + delimiter
+)
+pcdata_delimiter = no_capture(rb"|".join((rtf_brace_open, rtf_brace_close, control_word_pattern)))
+plain_text_pattern = named_regex_group("text", not_control_character_or_newline + rb"+") + no_capture(
+    rb"|".join((control_character_or_newline, rb"$"))
+)
+probe_pattern = rb".."
+
+
+class Bytes_Regex:
+    """
+    This wraps `re.pattern` objects and gives them a method `regex101` which
+    prints out the pattern in such a manner that it can be copy-pasted
+    to regex101.com.
+    """
+
+    def __init__(self, Bytes: bytes, flags: re.RegexFlag = 0) -> None:
+        self.pattern_bytes = Bytes
+        self.pattern = re.compile(Bytes, flags)
+        self.match = self.pattern.match
+
+    def regex101(self) -> None:
+        print(self.pattern_bytes.decode("ascii"))
+
+
+meaningful_bs = Bytes_Regex(rtf_backslash)
+probe = Bytes_Regex(named_regex_group("probe", probe_pattern), flags=re.DOTALL)
+parameter = Bytes_Regex(parameter_pattern)
+control_word = Bytes_Regex(control_word_pattern)
+control_symbol = Bytes_Regex(rtf_backslash + symbol)
+group_start = Bytes_Regex(rtf_brace_open)
+group_end = Bytes_Regex(rtf_brace_close)
+plain_text = Bytes_Regex(plain_text_pattern)
+
+
+raw_pcdata = Bytes_Regex(named_regex_group("pcdata", rb".*?") + pcdata_delimiter, flags=re.DOTALL)
+raw_sdata = Bytes_Regex(
+    named_regex_group("sdata", group(_hdigits + rb"\r\n") + rb"+"), flags=re.DOTALL
+)
```

### Comparing `rtfparse-0.7.8/src/rtfparse/renderers/de_encapsulate_html.py` & `rtfparse-0.8.0/src/rtfparse/renderers/de_encapsulate_html.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,111 @@
-#!/usr/bin/env python
-
-
-# Own modules
-from rtfparse import entities
-from rtfparse.renderers import Renderer
-import logging
-# Typing
-import io
-
-
-# Setup logging
-logger = logging.getLogger(__name__)
-
-
-class De_encapsulate_HTML(Renderer):
-    def __init__(self, ) -> None:
-        super().__init__()
-        self.ignore_rtf = False
-        self.render_word_func = dict((
-            ("par", self.newline),
-            ("line", self.newline),
-            ("tab", self.tab),
-            ("fromhtml", self.check_fromhtml),
-            ("htmlrtf", self.ignore_rtf_toggle),
-            ))
-        self.ignore_groups = (
-                "fonttbl",
-                "colortbl",
-                "generator",
-                "formatConverter",
-            )
-    def ignore_rtf_toggle(self, cw: entities.Control_Word) -> str:
-        if cw.parameter == "" or cw.parameter == 1:
-            self.ignore_rtf = True
-        elif cw.parameter == 0:
-            self.ignore_rtf = False
-        return ""
-    def check_fromhtml(self, cw: entities.Control_Word) -> str:
-        if cw.parameter == 1:
-            logger.info(f"Confirming that RTF was indeed generated from HTML")
-        else:
-            logger.warning(utils.warn(f"Encountered a part of RTF which was not generated from HTML"))
-            logger.warning(utils.warn(f"This might not be the right renderer for it."))
-        return ""
-    def newline(self, cw: entities.Control_Word) -> str:
-        if self.ignore_rtf:
-            return ""
-        else:
-            return "\n"
-    def tab(self, cw: entities.Control_Word) -> str:
-        if self.ignore_rtf:
-            return ""
-        else:
-            return "\t"
-    def render_symbol(self, item: entities.Control_Symbol, file: io.TextIOWrapper) -> None:
-        if not self.ignore_rtf:
-            # Obsolete formula character used by Word 5.1 for Macintosh
-            if item.text == "|":
-                pass
-            # Non-breaking space
-            elif item.text == "~":
-                file.write("\u00a0")
-            # Optional hyphen
-            elif item.text == "-":
-                pass
-            # Non-breaking hyphen
-            elif item.text == "_":
-                file.write("\u2011")
-            # Subentry in an index entry
-            elif item.text == ":":
-                pass
-            # Ignorable outside of Group
-            elif item.text == "*":
-                logger.warning(utils.warn(f"Found an IGNORABLE control symbol which is not a group start!"))
-            # Probably any symbol converted from a hex code: \'hh
-            else:
-                file.write(item.text)
-    def render(self, parsed: entities.Group, file: io.TextIOWrapper) -> None:
-        for item in parsed.structure:
-            if isinstance(item, entities.Group):
-                if item.name not in self.ignore_groups:
-                    self.render(item, file)
-            elif isinstance(item, entities.Control_Word):
-                try:
-                    file.write(self.render_word_func[item.control_name](item))
-                except KeyError:
-                    pass
-            elif isinstance(item, entities.Control_Symbol):
-                self.render_symbol(item, file)
-            elif isinstance(item, entities.Plain_Text):
-                if not self.ignore_rtf:
-                    file.write(item.text)
-            else:
-                pass
-
-
-if __name__ == "__main__":
-    pass
+#!/usr/bin/env python
+
+
+# Typing
+import io
+import logging
+
+# Own modules
+from rtfparse import entities
+from rtfparse.renderers import Renderer
+
+# Setup logging
+logger = logging.getLogger(__name__)
+
+
+class De_encapsulate_HTML(Renderer):
+    def __init__(
+        self,
+    ) -> None:
+        super().__init__()
+        self.ignore_rtf = False
+        self.render_word_func = dict(
+            (
+                ("par", self.newline),
+                ("line", self.newline),
+                ("tab", self.tab),
+                ("fromhtml", self.check_fromhtml),
+                ("htmlrtf", self.ignore_rtf_toggle),
+            )
+        )
+        self.ignore_groups = (
+            "fonttbl",
+            "colortbl",
+            "generator",
+            "formatConverter",
+        )
+
+    def ignore_rtf_toggle(self, cw: entities.Control_Word) -> str:
+        if cw.parameter == "" or cw.parameter == 1:
+            self.ignore_rtf = True
+        elif cw.parameter == 0:
+            self.ignore_rtf = False
+        return ""
+
+    def check_fromhtml(self, cw: entities.Control_Word) -> str:
+        if cw.parameter == 1:
+            logger.info(f"Confirming that RTF was indeed generated from HTML")
+        else:
+            logger.warning(utils.warn(f"Encountered a part of RTF which was not generated from HTML"))
+            logger.warning(utils.warn(f"This might not be the right renderer for it."))
+        return ""
+
+    def newline(self, cw: entities.Control_Word) -> str:
+        if self.ignore_rtf:
+            return ""
+        else:
+            return "\n"
+
+    def tab(self, cw: entities.Control_Word) -> str:
+        if self.ignore_rtf:
+            return ""
+        else:
+            return "\t"
+
+    def render_symbol(self, item: entities.Control_Symbol, file: io.TextIOWrapper) -> None:
+        if not self.ignore_rtf:
+            # Obsolete formula character used by Word 5.1 for Macintosh
+            if item.text == "|":
+                pass
+            # Non-breaking space
+            elif item.text == "~":
+                file.write("\u00a0")
+            # Optional hyphen
+            elif item.text == "-":
+                pass
+            # Non-breaking hyphen
+            elif item.text == "_":
+                file.write("\u2011")
+            # Subentry in an index entry
+            elif item.text == ":":
+                pass
+            # Ignorable outside of Group
+            elif item.text == "*":
+                logger.warning(
+                    utils.warn(f"Found an IGNORABLE control symbol which is not a group start!")
+                )
+            # Probably any symbol converted from a hex code: \'hh
+            else:
+                file.write(item.text)
+
+    def render(self, parsed: entities.Group, file: io.TextIOWrapper) -> None:
+        for item in parsed.structure:
+            if isinstance(item, entities.Group):
+                if item.name not in self.ignore_groups:
+                    self.render(item, file)
+            elif isinstance(item, entities.Control_Word):
+                try:
+                    file.write(self.render_word_func[item.control_name](item))
+                except KeyError:
+                    pass
+            elif isinstance(item, entities.Control_Symbol):
+                self.render_symbol(item, file)
+            elif isinstance(item, entities.Plain_Text):
+                if not self.ignore_rtf:
+                    file.write(item.text)
+            else:
+                pass
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `rtfparse-0.7.8/src/rtfparse/utils.py` & `rtfparse-0.8.0/src/rtfparse/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python
-
-
-import logging
-import pathlib
-import io
-# Typing
-from typing import Union
-
-
-# Setup logging
-logger = logging.getLogger(__name__)
-
-
-program_name = home_dir_name = "rtfparse"
-dir_name = "".join((".", program_name))
-configuration_file_name = f"{program_name}_configuration.ini"
-
-
-def provide_dir(directory: pathlib.Path) -> pathlib.Path:
-    """
-    Checks if there is a directory of name `dir_name` in the user home path.
-    If not, it will try to create one. 
-    """
-    if directory.exists() and directory.is_dir():
-        logger.debug(f"Found directory {str(directory)}")
-    else:
-        while True:
-            try:
-                directory.mkdir()
-                logger.info(f"Created directory {str(directory)}")
-                break
-            except FileNotFoundError:
-                provide_dir(directory.parent)
-                continue
-            except FileExistsError:
-                logger.debug(f"{directory} already exists")
-                break
-    return directory
-
-
-def warn(s: str) -> str:
-    """
-    Creates a string highlighted as warning in log output
-    """
-    return " ".join(("◊", s))
-
-
-def what_is_being_parsed(file: Union[io.BufferedReader, io.BytesIO]) -> str:
-    if isinstance(file, io.BufferedReader):
-        return file.name
-    elif isinstance(file, io.BytesIO):
-        return repr(file)
-
-
-def twos_complement(val, nbits):
-    """Compute the 2's complement of int value val. Credit: https://stackoverflow.com/a/37075643/9235421"""
-    if val < 0:
-        if (val + 1).bit_length() >= nbits:
-            raise ValueError(f"Value {val} is out of range of {nbits}-bit value.")
-        val = (1 << nbits) + val
-    else:
-        if val.bit_length() > nbits:
-            raise ValueError(f"Value {val} is out of range of {nbits}-bit value.")
-        # If sign bit is set.
-        if (val & (1 << (nbits - 1))) != 0:
-            # compute negative value.
-            val = val - (1 << nbits)
-    return val
+#!/usr/bin/env python
+
+
+import io
+import logging
+import pathlib
+
+# Typing
+from typing import Union
+
+# Setup logging
+logger = logging.getLogger(__name__)
+
+
+program_name = home_dir_name = "rtfparse"
+dir_name = "".join((".", program_name))
+configuration_file_name = f"{program_name}_configuration.ini"
+
+
+def provide_dir(directory: pathlib.Path) -> pathlib.Path:
+    """
+    Checks if there is a directory of name `dir_name` in the user home path.
+    If not, it will try to create one.
+    """
+    if directory.exists() and directory.is_dir():
+        logger.debug(f"Found directory {str(directory)}")
+    else:
+        while True:
+            try:
+                directory.mkdir()
+                logger.info(f"Created directory {str(directory)}")
+                break
+            except FileNotFoundError:
+                provide_dir(directory.parent)
+                continue
+            except FileExistsError:
+                logger.debug(f"{directory} already exists")
+                break
+    return directory
+
+
+def warn(s: str) -> str:
+    """
+    Creates a string highlighted as warning in log output
+    """
+    return " ".join(("◊", s))
+
+
+def what_is_being_parsed(file: Union[io.BufferedReader, io.BytesIO]) -> str:
+    if isinstance(file, io.BufferedReader):
+        return file.name
+    elif isinstance(file, io.BytesIO):
+        return repr(file)
+
+
+def twos_complement(val, nbits):
+    """Compute the 2's complement of int value val. Credit: https://stackoverflow.com/a/37075643/9235421"""
+    if val < 0:
+        if (val + 1).bit_length() >= nbits:
+            raise ValueError(f"Value {val} is out of range of {nbits}-bit value.")
+        val = (1 << nbits) + val
+    else:
+        if val.bit_length() > nbits:
+            raise ValueError(f"Value {val} is out of range of {nbits}-bit value.")
+        # If sign bit is set.
+        if (val & (1 << (nbits - 1))) != 0:
+            # compute negative value.
+            val = val - (1 << nbits)
+    return val
```

