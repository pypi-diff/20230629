# Comparing `tmp/utf8-locale-1.0.0.tar.gz` & `tmp/utf8_locale-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utf8-locale-1.0.0.tar", last modified: Sat Oct 22 21:33:28 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `utf8-locale-1.0.0.tar` & `utf8_locale-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/
--rw-r--r--   0 roam      (1000) roam      (1000)      640 2022-08-25 07:57:19.000000 utf8-locale-1.0.0/.editorconfig
--rw-r--r--   0 roam      (1000) roam      (1000)      147 2022-02-01 16:07:39.000000 utf8-locale-1.0.0/MANIFEST.in
--rw-r--r--   0 roam      (1000) roam      (1000)     4459 2022-10-22 21:23:00.000000 utf8-locale-1.0.0/NEWS.md
--rw-r--r--   0 roam      (1000) roam      (1000)     4430 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     3376 2022-02-20 11:58:03.000000 utf8-locale-1.0.0/README.md
--rw-r--r--   0 roam      (1000) roam      (1000)      122 2022-01-30 21:50:05.000000 utf8-locale-1.0.0/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/python/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/python/unit_tests/
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2022-02-01 09:52:03.000000 utf8-locale-1.0.0/python/unit_tests/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     7913 2022-10-01 22:30:00.000000 utf8-locale-1.0.0/python/unit_tests/test_detect.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2538 2022-08-21 21:16:26.000000 utf8-locale-1.0.0/python/unit_tests/test_object.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/python/utf8_locale/
--rw-r--r--   0 roam      (1000) roam      (1000)     2302 2022-10-01 22:30:24.000000 utf8-locale-1.0.0/python/utf8_locale/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     6362 2022-10-01 22:30:31.000000 utf8-locale-1.0.0/python/utf8_locale/__main__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     8819 2022-10-01 22:30:36.000000 utf8-locale-1.0.0/python/utf8_locale/detect.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-01-03 11:43:53.000000 utf8-locale-1.0.0/python/utf8_locale/py.typed
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/python/utf8_locale.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)     4430 2022-10-22 21:33:28.000000 utf8-locale-1.0.0/python/utf8_locale.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)      585 2022-10-22 21:33:28.000000 utf8-locale-1.0.0/python/utf8_locale.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2022-10-22 21:33:28.000000 utf8-locale-1.0.0/python/utf8_locale.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       52 2022-10-22 21:33:28.000000 utf8-locale-1.0.0/python/utf8_locale.egg-info/entry_points.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       12 2022-10-22 21:33:28.000000 utf8-locale-1.0.0/python/utf8_locale.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2022-10-22 21:33:28.000000 utf8-locale-1.0.0/python/utf8_locale.egg-info/zip-safe
--rw-r--r--   0 roam      (1000) roam      (1000)     1315 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/setup.cfg
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2022-10-22 21:33:28.682426 utf8-locale-1.0.0/tests/
--rw-r--r--   0 roam      (1000) roam      (1000)      730 2022-02-20 11:58:03.000000 utf8-locale-1.0.0/tests/data.json
--rw-r--r--   0 roam      (1000) roam      (1000)    10065 2022-08-21 21:05:42.000000 utf8-locale-1.0.0/tests/functional.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2475 2022-10-01 22:34:15.000000 utf8-locale-1.0.0/tox.ini
--rw-r--r--   0 roam      (1000) roam      (1000)     4557 2022-02-01 15:56:30.000000 utf8-locale-1.0.0/u8loc.1
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/.editorconfig
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/NEWS.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/tox.ini
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/u8loc.1
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/LICENSES/BSD-2-Clause.txt
+-rwxr-xr-x   0        0        0      495 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/nix/cleanpy.sh
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/nix/python-pytest.nix
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/nix/python-tox.nix
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/nix/reformat.sh
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/nix/run-pytest.sh
+-rwxr-xr-x   0        0        0      433 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/nix/run-tox.sh
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/config/ruff-most/pyproject.toml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/unit_tests/__init__.py
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/unit_tests/test_detect.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/unit_tests/test_object.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/utf8_locale/__init__.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/utf8_locale/__main__.py
+-rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/utf8_locale/detect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/python/utf8_locale/py.typed
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/tests/data.json
+-rwxr-xr-x   0        0        0     1232 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/tests/full.sh
+-rwxr-xr-x   0        0        0     8919 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/tests/functional.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/.gitignore
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/README.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 utf8_locale-1.0.1/PKG-INFO
```

### Comparing `utf8-locale-1.0.0/.editorconfig` & `utf8_locale-1.0.1/.editorconfig`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # https://editorconfig.org/
+#
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
 
 root = true
 
 [*]
 end_of_line = lf
 insert_final_newline = true
 charset = utf-8
```

### Comparing `utf8-locale-1.0.0/PKG-INFO` & `utf8_locale-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: utf8-locale
-Version: 1.0.0
-Summary: Detect a UTF-8-capable locale for running programs in.
-Home-page: https://gitlab.com/ppentchev/utf8-locale
-Author: Peter Pentchev
-Author-email: roam@ringlet.net
-License: BSD-2
+Version: 1.0.1
+Summary: Detect a UTF-8-capable locale for running programs in
+Project-URL: Homepage, https://devel.ringlet.net/devel/utf8-locale/
+Project-URL: Issue Tracker, https://gitlab.com/ppentchev/utf8-locale/-/issues
+Project-URL: Source Code, https://gitlab.com/ppentchev/utf8-locale
+Author-email: Peter Pentchev <roam@ringlet.net>
+License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
+<!--
+SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+SPDX-License-Identifier: BSD-2-Clause
+-->
+
 # Detect a UTF-8-capable locale for running child processes in
 
 Sometimes it is useful for a program to be able to run a child process and
 more or less depend on its output being valid UTF-8. This can usually be
 accomplished by setting one or more environment variables, but there is
 the question of what to set them to - what UTF-8-capable locale is present
 on this particular system? This is where the `utf8_locale` module comes in.
```

### Comparing `utf8-locale-1.0.0/README.md` & `utf8_locale-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<!--
+SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+SPDX-License-Identifier: BSD-2-Clause
+-->
+
 # Detect a UTF-8-capable locale for running child processes in
 
 Sometimes it is useful for a program to be able to run a child process and
 more or less depend on its output being valid UTF-8. This can usually be
 accomplished by setting one or more environment variables, but there is
 the question of what to set them to - what UTF-8-capable locale is present
 on this particular system? This is where the `utf8_locale` module comes in.
```

### Comparing `utf8-locale-1.0.0/python/unit_tests/test_detect.py` & `utf8_locale-1.0.1/python/utf8_locale/detect.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,224 +1,245 @@
-# Copyright (c) 2020 - 2022  Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
-"""Test the UTF-8 locale detection functions."""
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
+
+"""Implement the actual UTF-8 locale detection."""
 
 from __future__ import annotations
 
-import json
+import dataclasses
 import os
-import pathlib
+import re
 import subprocess
-import unittest
-
-from unittest import mock
-
 from typing import Iterable, NamedTuple
 
-import ddt  # type: ignore
-import pytest
 
-import utf8_locale
+VERSION = "1.0.1"
 
+UTF8_LANGUAGES = ("C", "en", "de", "es", "it")
+UTF8_ENCODINGS = ("UTF-8", "utf8")
 
-class TLangData(NamedTuple):
-    """The test data for a single preferred languages test case."""
+LOCALE_VARIABLES = (
+    "LC_ALL",
+    "LANG",
+    "LC_MESSAGES",
+    "LC_COLLATE",
+    "LC_NAME",
+    "LC_IDENTIFICATION",
+    "LC_CTYPE",
+    "LC_NUMERIC",
+    "LC_TIME",
+    "LC_MONETARY",
+    "LC_PAPER",
+    "LC_ADDRESS",
+    "LC_TELEPHONE",
+    "LC_MEASUREMENT",
+)
+
+RE_LOCALE_NAME = re.compile(
+    r""" ^
+    (?P<lang> [a-zA-Z0-9]+ )
+    (?:
+        _
+        (?P<territory> [a-zA-Z0-9]+ )
+    )?
+    (?:
+        \.
+        (?P<codeset> [a-zA-Z0-9-]+ )
+    )?
+    (?:
+        @
+        (?P<modifier> [a-zA-Z0-9]+ )
+    )?
+    $ """,
+    re.X,
+)
+
+
+class NoLanguagesError(ValueError):
+    """No languages were specified to detect from."""
+
+    def __str__(self) -> str:
+        """Provide a human-readable representation of the error."""
+        return "No languages specified"
+
+
+class _DetectState(NamedTuple):
+    """The state of processing consecutive lines of `locale -a` output."""
+
+    priority: int
+    name: str
+
+
+def detect_utf8_locale(*, languages: Iterable[str] = UTF8_LANGUAGES) -> str:
+    """Get a locale name that may hopefully be used for UTF-8 output.
+
+    The `detect_utf8_locale()` function runs the external `locale` command to
+    obtain a list of the supported locale names, and then picks a suitable one
+    to use so that programs are more likely to output valid UTF-8 characters
+    and language-neutral messages. It prefers the `C` base locale, but if
+    neither `C.UTF-8` nor `C.utf8` is available, it will fall back to a list of
+    other locale names that are likely to be present on the system.
+
+    The `utf8_locale` package has a predefined list of preferred languages.
+    If a program has different preferences, e.g. only expecting to parse
+    messages written in English, the `detect_utf8_locale()` function may be
+    passed a `languages` parameter - an iterable of strings - containing
+    the language names in the preferred order. Note that `languages` should
+    only contain the language name (e.g. "en") and not a territory name
+    (e.g. "en_US"); locale names for the same language and different
+    territories are considered equivalent. Thus, the abovementioned program
+    that expects to parse messages in English may do:
+
+        name = detect_utf8_locale(languages=["C", "en"])
+    """
+    weights = {}
+    unweight = 0
+    for lang in languages:
+        if lang not in weights:
+            weights[lang] = unweight
+            unweight = unweight + 1
+    if not weights:
+        raise NoLanguagesError
+
+    state = _DetectState(unweight, "C")
+    for line in subprocess.check_output(
+        ["env", "LC_ALL=C", "LANGUAGE=", "locale", "-a"],
+        shell=False,
+        encoding="ISO-8859-1",
+    ).splitlines():
+        data = RE_LOCALE_NAME.match(line)
+        if not data:
+            continue
+        if data.group("codeset") not in UTF8_ENCODINGS:
+            continue
+
+        lang = data.group("lang")
+        prio = weights.get(lang, weights.get("*", unweight))
+        if prio == 0:
+            return line
+        if prio < state.priority:
+            state = _DetectState(prio, line)
+
+    return state.name
+
+
+def get_utf8_vars(*, languages: Iterable[str] = UTF8_LANGUAGES) -> dict[str, str]:
+    """Prepare the environment variables that need to be changed.
+
+    The `get_utf8_vars()` function invokes `detect_utf8_locale()` and then
+    returns a dictionary containing the `LC_ALL` variable set to the obtained
+    locale name and `LANGUAGE` set to an empty string so that recent versions
+    of the gettext library do not choose a different language to output
+    messages in.
+
+    The `get_utf8_vars()` function also has an optional `languages` parameter
+    that is passed directory to `detect_utf8_locale()`.
+    """
+    return {"LC_ALL": detect_utf8_locale(languages=languages), "LANGUAGE": ""}
+
+
+def get_utf8_env(
+    env: dict[str, str] | None = None,
+    *,
+    languages: Iterable[str] = UTF8_LANGUAGES,
+) -> dict[str, str]:
+    """Prepare the environment to run subprocesses in.
+
+    The `get_utf8_env()` function invokes `detect_utf8_locale()` and then
+    returns a dictionary similar to `os.environ`, but with `LC_ALL` set to
+    the obtained locale name and `LANGUAGE` set to an empty string so that
+    recent versions of the gettext library do not choose a different language
+    to output messages in. If a dictionary is passed as the `env` parameter,
+    `get_utf8_env()` uses it as a base instead of the value of `os.environ`.
+
+    The `get_utf8_env()` function also has an optional `languages` parameter
+    that is passed directory to `detect_utf8_locale()`.
+    """
+    subenv = dict(os.environ if env is None else env)
+    subenv.update(get_utf8_vars(languages=languages))
+    return subenv
+
+
+def get_preferred_languages(
+    env: dict[str, str] | None = None,
+    *,
+    names: Iterable[str] = LOCALE_VARIABLES,
+) -> list[str]:
+    """Determine preferred languages as per the current locale settings.
+
+    The `get_preferred_languages()` function examines either the current
+    process environment or the provided dictionary and returns a list of
+    the languages specified in the locale variables (`LC_ALL`, `LANG`,
+    `LC_MESSAGES`, etc) in order of preference as defined by either
+    the `names` parameter passed or by the `LOCALE_VARIABLES` constant.
+    It may be used by programs to add the user's currently preferred locale
+    to their own settings, e.g.:
+
+        name = detect_utf8_locale(get_preferred_languages() + ["en"])
+
+    Note that "C" is always appended to the end of the list if it is not
+    already present.
+    """
+    if env is None:
+        env = dict(os.environ)
+
+    res = []
+    for name in names:
+        value = env.get(name)
+        if value is None:
+            continue
+        data = RE_LOCALE_NAME.match(value)
+        if data is None:
+            continue
+        if data.group("codeset") not in UTF8_ENCODINGS:
+            continue
+
+        lang = data.group("lang")
+        if lang not in res:
+            res.append(lang)
+
+    # Make sure "C" is always in the list.
+    if "C" not in res:
+        res.append("C")
+    return res
+
+
+@dataclasses.dataclass(frozen=True)
+class LanguagesDetect:
+    """Set up the desired parameters for detecting the preferred languages."""
+
+    env: dict[str, str] | None = None
+    names: Iterable[str] | None = None
+
+    def detect(self) -> list[str]:
+        """Determine the preferred languages."""
+        names = self.names if self.names is not None else LOCALE_VARIABLES
+        return get_preferred_languages(self.env, names=names)
+
+
+@dataclasses.dataclass(frozen=True)
+class UTF8Environment:
+    """The parameters for a UTF-8-capable environment."""
 
     env: dict[str, str]
-    expected: list[str]
-
-
-class TData(NamedTuple):
-    """The test data loaded from the JSON definitions file."""
-
-    locales: list[str]
-    languages: list[TLangData]
-
-
-class TDataHolder:
-    """A singleton object holding the test data."""
-
-    # pylint: disable=too-few-public-methods
-
-    data: TData | None = None
-
-    @classmethod
-    def load(cls) -> TData:
-        """Load the test data from the JSON definitions file."""
-        if cls.data is not None:
-            return cls.data
-
-        raw = json.loads(
-            (pathlib.Path(__file__).absolute().parent.parent.parent / "tests/data.json").read_text(
-                encoding="UTF-8"
-            )
-        )
-        assert raw["format"]["version"] == {"major": 0, "minor": 1}
-
-        cls.data = TData(
-            locales=raw["locales"],
-            languages=[
-                TLangData(env=item["env"], expected=item["expected"]) for item in raw["languages"]
-            ],
+    env_vars: dict[str, str]
+    languages: list[str]
+    locale: str
+
+
+@dataclasses.dataclass(frozen=True)
+class UTF8Detect:
+    """Set up the desired parameters for detecting the UTF-8-capable environment."""
+
+    env: dict[str, str] | None = None
+    languages: Iterable[str] | None = None
+
+    def detect(self) -> UTF8Environment:
+        """Run the detection, return the results."""
+        languages = list(self.languages if self.languages is not None else UTF8_LANGUAGES)
+        env = get_utf8_env(self.env, languages=languages)
+        return UTF8Environment(
+            env=env,
+            env_vars={key: env[key] for key in ("LC_ALL", "LANGUAGE")},
+            languages=languages,
+            locale=env["LC_ALL"],
         )
-        return cls.data
-
-
-LANG_KEYS = set(["LC_ALL", "LANGUAGE"])
-
-LANG_EXPECTED = [
-    (["C", "en"], "C.UTF-8"),
-    (["en", "C"], "en_XX.UTF-8"),
-    (["es", "bg", "*"], "it_IT.UTF-8"),
-    (["en", "bg", "*"], "en_XX.UTF-8"),
-    (["es", "*", "en"], "it_IT.UTF-8"),
-    (["es", "*", "it"], "de_DE.UTF-8"),
-    (["en", "bg", "en"], "en_XX.UTF-8"),
-    (["it", "en", "it"], "it_IT.UTF-8"),
-    (["xy", "yz", "xy", "en"], "en_XX.UTF-8"),
-]
-
-
-def check_env(env: dict[str, str]) -> None:
-    """Make sure a UTF8-capable environment was setup correctly."""
-    # Everything except LANG_KEYS is the same as in os.environ
-    assert {key: value for key, value in env.items() if key not in LANG_KEYS} == {
-        key: value for key, value in os.environ.items() if key not in LANG_KEYS
-    }
-
-    # The rest of this function makes sure that locale(1) and date(1), when
-    # run in this environment, output reasonable values
-    loc = {
-        fields[0]: fields[1].strip('"')
-        for fields in (
-            line.split("=", 1)
-            for line in subprocess.check_output(
-                ["locale"], shell=False, env=env, encoding="UTF-8"
-            ).splitlines()
-        )
-    }
-    non_lc = set(name for name in loc if not name.startswith("LC_"))
-    assert non_lc.issubset(set(("LANG", "LANGUAGE")))
-    loc = {name: value for name, value in loc.items() if name.startswith("LC_")}
-    values = list(set(loc.values()))
-    assert len(values) == 1, values
-    assert values[0].lower().endswith(".utf8") or values[0].lower().endswith(".utf-8")
-
-    utc_env = dict(env)
-    utc_env["TZ"] = "UTC"
-    lines = subprocess.check_output(
-        ["date", "-d", "@1000000000", "+%A"],
-        shell=False,
-        env=utc_env,
-        encoding="UTF-8",
-    ).splitlines()
-    assert lines in [["Sunday"], ["Sonntag"], ["domenica"], ["domingo"]]
-
-
-def get_mod_env() -> dict[str, str]:
-    """Get a slightly modified copy of os.environ for test purposes."""
-    mod_env = {
-        key: value
-        for key, value in os.environ.items()
-        if key not in ("HOME", "USER", "PS1", "PATH")
-    }
-    mod_env["TEST_KEY"] = "test value"
-    return mod_env
-
-
-def check_mod_env(env: dict[str, str], mod_env: dict[str, str], env2: dict[str, str]) -> None:
-    """Make sure very little has changed in the prepared environment."""
-    # Nothing besides LANG_KEYS has changed
-    assert {key: value for key, value in env2.items() if key not in LANG_KEYS} == {
-        key: value for key, value in mod_env.items() if key not in LANG_KEYS
-    }
-
-    # LANG_KEYS have changed in the same way as before
-    assert {key: value for key, value in env2.items() if key in LANG_KEYS} == {
-        key: value for key, value in env.items() if key in LANG_KEYS
-    }
-
-
-def test_utf8_env() -> None:
-    """Test get_utf8_env() and, indirectly, detect_utf8_locale()."""
-    env = utf8_locale.get_utf8_env()
-    check_env(env)
-
-    mod_env = get_mod_env()
-    env2 = utf8_locale.get_utf8_env(mod_env)
-    check_mod_env(env, mod_env, env2)
-
-
-def mock_locale():  # type: ignore
-    """Mock subprocess.check_output("locale -a")."""
-    locales = TDataHolder.load().locales
-    mock_check_output = mock.Mock(spec=["__call__"])
-    mock_check_output.return_value = "".join(item + "\n" for item in locales)
-    return mock.patch("subprocess.check_output", new=mock_check_output)
-
-
-@ddt.ddt
-class TestLanguages(unittest.TestCase):
-    """Test the language preference handling of detect_utf8_locale()."""
-
-    @staticmethod
-    def detect_locale(languages: Iterable[str]) -> str:
-        """Get the locale name using the appropriate mechanism."""
-        with mock_locale():  # type: ignore
-            return utf8_locale.detect_utf8_locale(languages=languages)
-
-    @staticmethod
-    def get_vars(languages: Iterable[str]) -> dict[str, str]:
-        """Get the variables dict using the appropriate mechanism."""
-        with mock_locale():  # type: ignore
-            return utf8_locale.get_utf8_vars(languages=languages)
-
-    @staticmethod
-    def get_langs(env: dict[str, str]) -> list[str]:
-        """Get the preferred languages using the appropriate mechanism."""
-        return utf8_locale.get_preferred_languages(env)
-
-    @ddt.data(*LANG_EXPECTED)
-    @ddt.unpack
-    def test_language(self, languages: list[str], result: str) -> None:
-        """Test detect_utf8_locale() with some languages specified."""
-        assert self.detect_locale(iter(languages)) == result
-
-    @ddt.data(*LANG_EXPECTED)
-    @ddt.unpack
-    def test_language_vars(self, languages: list[str], result: str) -> None:
-        """Test detect_utf8_locale() with some languages specified."""
-        assert self.get_vars(iter(languages)) == {
-            "LC_ALL": result,
-            "LANGUAGE": "",
-        }
-
-    def test_no_languages(self) -> None:
-        """Test detect_utf8_locale() with no languages specified."""
-        with pytest.raises(ValueError):
-            self.detect_locale(languages=iter([]))
-
-    @ddt.data(*TDataHolder.load().languages)
-    def test_preferred(self, tcase: TLangData) -> None:
-        """Test get_preferred_languages() with the specified environment."""
-        assert self.get_langs(tcase.env) == tcase.expected
```

### Comparing `utf8-locale-1.0.0/python/utf8_locale/__main__.py` & `utf8_locale-1.0.1/python/utf8_locale/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,18 @@
-# Copyright (c) 2022  Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
 """The u8loc command-line tool."""
 
 from __future__ import annotations
 
 import argparse
 import dataclasses
 import os
+import subprocess
 import sys
-
 from typing import Callable, NamedTuple
 
 from . import detect
 
 
 @dataclasses.dataclass(frozen=True)
 class Config:
@@ -150,44 +129,45 @@
         return QueryConfig(preferred=args.preferred, query=args.query)
 
     if args.run:
         if not args.program:
             sys.exit("No program to run specified")
         return RunConfig(preferred=args.preferred, run_program=args.program)
 
-    raise NotImplementedError(f"Did not expect to reach the end of parse_args() with {args!r}")
+    sys.exit(f"Did not expect to reach the end of parse_args() with {args!r}")
 
 
 def main() -> None:
-    """The main routine for the u8loc command-line tool."""
+    """Parse command-line arguments, dispatch commands."""
     cfg = parse_args()
 
     if isinstance(cfg, QueryConfig) and QUERY_HANDLERS[cfg.query].early:
         QUERY_HANDLERS[cfg.query].handler(
             cfg, detect.UTF8Environment(env={}, env_vars={}, locale="", languages=[])
         )
         return
 
     try:
         languages = (
             detect.LanguagesDetect().detect() if cfg.preferred else list(detect.UTF8_LANGUAGES)
         )
         env = detect.UTF8Detect(languages=iter(languages)).detect()
-        assert env.languages == languages, f"{env.languages!r} != {languages!r}"
-    except Exception as err:  # pylint: disable=broad-except
+        if env.languages != languages:
+            sys.exit("utf8-locale internal error: env {env.languages!r} != {languages!r}")
+    except (detect.NoLanguagesError, OSError, subprocess.CalledProcessError) as err:
         sys.exit(f"Could not determine an appropriate UTF-8 locale: {err}")
 
     if isinstance(cfg, RunConfig):
         try:
             os.execvpe(cfg.run_program[0], cfg.run_program, env.env)
-        except Exception as err:  # pylint: disable=broad-except
+        except OSError as err:
             sys.exit(f"Could not run '{' '.join(cfg.run_program)}': {err}")
 
     if isinstance(cfg, QueryConfig):
         QUERY_HANDLERS[cfg.query].handler(cfg, env)
         return
 
-    raise NotImplementedError(f"Did not expect to reach the end of main() with {cfg!r}")
+    sys.exit(f"Did not expect to reach the end of main() with {cfg!r}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `utf8-locale-1.0.0/tests/data.json` & `utf8_locale-1.0.1/tests/data.json`

 * *Files identical despite different names*

### Comparing `utf8-locale-1.0.0/u8loc.1` & `utf8_locale-1.0.1/u8loc.1`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,9 @@
-.\" Copyright (c) 2022  Peter Pentchev
-.\" All rights reserved.
-.\"
-.\" Redistribution and use in source and binary forms, with or without
-.\" modification, are permitted provided that the following conditions
-.\" are met:
-.\" 1. Redistributions of source code must retain the above copyright
-.\"    notice, this list of conditions and the following disclaimer.
-.\" 2. Redistributions in binary form must reproduce the above copyright
-.\"    notice, this list of conditions and the following disclaimer in the
-.\"    documentation and/or other materials provided with the distribution.
-.\"
-.\" THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-.\" ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-.\" IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-.\" ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-.\" FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-.\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-.\" OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-.\" HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-.\" LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-.\" OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-.\" SUCH DAMAGE.
+.\" SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+.\" SPDX-License-Identifier: BSD-2-Clause
 .\"
 .Dd February 1, 2021
 .Dt U8LOC 1
 .Os
 .Sh NAME
 .Nm u8loc
 .Nd run a program in a UTF-8-capable environment
```

