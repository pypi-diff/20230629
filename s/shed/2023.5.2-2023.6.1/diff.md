# Comparing `tmp/shed-2023.5.2.tar.gz` & `tmp/shed-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shed-2023.5.2.tar", last modified: Fri May 26 14:54:17 2023, max compression
+gzip compressed data, was "shed-2023.6.1.tar", last modified: Thu Jun 29 16:47:13 2023, max compression
```

## Comparing `shed-2023.5.2.tar` & `shed-2023.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.593455 shed-2023.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 14:54:01.000000 shed-2023.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-26 14:54:17.593455 shed-2023.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-26 14:54:01.000000 shed-2023.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:54:17.593455 shed-2023.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-26 14:54:01.000000 shed-2023.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.589455 shed-2023.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.589455 shed-2023.5.2/src/shed/
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30931 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/_codemods.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.589455 shed-2023.5.2/src/shed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.593455 shed-2023.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_expected_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_shed.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_suggest_different_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:47:13.761401 shed-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 16:47:00.000000 shed-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-29 16:47:13.761401 shed-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-29 16:47:00.000000 shed-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:47:13.761401 shed-2023.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-29 16:47:00.000000 shed-2023.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:47:13.757401 shed-2023.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:47:13.757401 shed-2023.6.1/src/shed/
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-06-29 16:47:00.000000 shed-2023.6.1/src/shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 16:47:00.000000 shed-2023.6.1/src/shed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-29 16:47:00.000000 shed-2023.6.1/src/shed/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30931 2023-06-29 16:47:00.000000 shed-2023.6.1/src/shed/_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:47:00.000000 shed-2023.6.1/src/shed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:47:13.761401 shed-2023.6.1/src/shed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-29 16:47:13.000000 shed-2023.6.1/src/shed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 16:47:13.000000 shed-2023.6.1/src/shed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:47:13.000000 shed-2023.6.1/src/shed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 16:47:13.000000 shed-2023.6.1/src/shed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 16:47:13.000000 shed-2023.6.1/src/shed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 16:47:13.000000 shed-2023.6.1/src/shed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:47:13.761401 shed-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-29 16:47:00.000000 shed-2023.6.1/tests/test_expected_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-29 16:47:00.000000 shed-2023.6.1/tests/test_shed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-29 16:47:00.000000 shed-2023.6.1/tests/test_suggest_different_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-29 16:47:00.000000 shed-2023.6.1/tests/test_version.py
```

### Comparing `shed-2023.5.2/LICENSE` & `shed-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shed-2023.5.2/PKG-INFO` & `shed-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.5.2
+Version: 2023.6.1
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,18 +77,18 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.5.2
+  rev: 2023.6.1
   hooks:
     - id: shed
-      # args: [--refactor, --py39-plus]
+      # args: [--refactor, --py311-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `shed` on unchanged files.
 
 ## See also
```

### Comparing `shed-2023.5.2/README.md` & `shed-2023.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,18 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.5.2
+  rev: 2023.6.1
   hooks:
     - id: shed
-      # args: [--refactor, --py39-plus]
+      # args: [--refactor, --py311-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `shed` on unchanged files.
 
 ## See also
```

### Comparing `shed-2023.5.2/setup.py` & `shed-2023.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "Funding": "https://github.com/sponsors/Zac-HD",
     },
     license="AGPL-3.0",
     description="`shed` canonicalises Python code.",
     install_requires=[
         "autoflake >= 1.4",
         "black >= 23.3.0",
-        "com2ann >= 0.3.0 ; python_version >= '3.8'",
+        "com2ann >= 0.3.0",
         "isort >= 5.10.1",
         "libcst >= 0.4.10",
         "pyupgrade >= 3.0.0",
     ],
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `shed-2023.5.2/src/shed/__init__.py` & `shed-2023.6.1/src/shed/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,43 +17,39 @@
 import black
 import isort
 import pyupgrade._main
 from black.mode import TargetVersion
 from black.parsing import lib2to3_parse
 from isort.exceptions import FileSkipComment
 
-__version__ = "2023.5.2"
+__version__ = "2023.6.1"
 __all__ = ["shed", "docshed"]
 
 # Conditionally imported in refactor mode to reduce startup latency in the common case
 com2ann: Any = None
 _run_codemods: Any = None
 
 _version_map = {
     k: (int(k.name[2]), int(k.name[3:]))
     for k in TargetVersion
-    if k.value >= TargetVersion.PY37.value
+    if k.value >= TargetVersion.PY38.value
 }
 _default_min_version = min(_version_map.values())
 _SUGGESTIONS = (
     # If we fail on invalid syntax, check for detectable wrong-codeblock types
     (r"^(>>> | ?In \[\d+\]: )", "pycon"),
     (r"^Traceback \(most recent call last\):$", "python-traceback"),
 )
 
 
 class ShedSyntaxWarning(SyntaxWarning):
     """Warns that shed has been called on something with invalid syntax."""
 
 
-def _fallback(source: str, **kw: object) -> Tuple[str, object]:
-    return source, None  # pragma: no cover
-
-
-@functools.lru_cache()
+@functools.lru_cache
 def shed(
     source_code: str,
     *,
     refactor: bool = False,
     is_pyi: bool = False,
     first_party_imports: FrozenSet[str] = frozenset(),
     min_version: Tuple[int, int] = _default_min_version,
@@ -110,26 +106,21 @@
         # It does however have one crucial advantage: several hundred milliseconds
         # of startup latency in the common case where --refactor was *not* passed.
         # This is a big deal for interactive use-cases such as pre-commit hooks
         # or format-on-save in editors (though I prefer Black for the latter).
         global com2ann
         global _run_codemods
         if com2ann is None:
-            from ._codemods import _run_codemods  # type: ignore
+            from com2ann import com2ann
 
-            try:
-                from com2ann import com2ann
-            except ImportError:  # pragma: no cover  # on Python 3.8
-                assert sys.version_info < (3, 8)
-                com2ann = _fallback
-            # OK, everything's imported, back to the runtime logic!
+            from ._codemods import _run_codemods  # type: ignore
 
         # Some tools assume that the file is multi-line, but empty files are valid input.
         source_code += "\n"
-        # Use com2ann to comvert type comments to annotations on Python 3.8+
+        # Use com2ann to comvert type comments to annotations
         annotated = com2ann(
             source_code,
             drop_ellipsis=True,
             silent=True,
             python_minor_version=min(min_version[1], sys.version_info[1]),
         )
         if annotated:  # pragma: no branch
@@ -187,15 +178,15 @@
     if source_code != blackened:
         source_code = black.format_str(source_code, mode=black_mode)
 
     # Remove any extra trailing whitespace
     return source_code.rstrip() + "\n"
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def docshed(
     source: str,
     *,
     refactor: bool = False,
     first_party_imports: FrozenSet[str] = frozenset(),
     min_version: Tuple[int, int] = _default_min_version,
     _location: str = "string passed to shed.docshed()",
```

### Comparing `shed-2023.5.2/src/shed/_cli.py` & `shed-2023.6.1/src/shed/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 import autoflake
 from isort.api import place_module
 
 from . import ShedSyntaxWarning, _version_map, docshed, shed
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def _get_git_repo_root(cwd: Optional[str] = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
         check=True,
         timeout=10,
         capture_output=True,
         text=True,
         cwd=cwd,
     ).stdout.strip()
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def _guess_first_party_modules(cwd: Optional[str] = None) -> FrozenSet[str]:
     """Guess the name of the current package for first-party imports."""
     try:
         base = _get_git_repo_root(cwd)
     except (subprocess.SubprocessError, FileNotFoundError):
         return frozenset()
     provides = {init.parent.name for init in Path(base).glob("**/src/*/__init__.py")}
@@ -62,15 +62,18 @@
         with open(fname, mode="rb") as handle:
             bytes_on_disk = handle.read()
         encoding, _ = tokenize.detect_encoding(io.BytesIO(bytes_on_disk).readline)
         with io.TextIOWrapper(io.BytesIO(bytes_on_disk), encoding) as wrapper:
             on_disk = wrapper.read()
     except (OSError, UnicodeError) as err:
         # Permissions or encoding issue, or file deleted since last commit.
-        return f"skipping {fname!r} due to {err}"
+        err_msg = f"skipping {fname!r} due to {err}"
+        if "*" in fname:
+            err_msg += ", maybe due to unexpanded glob pattern?"
+        return err_msg
     if fname.endswith((".md", ".rst")):
         writer: Callable[..., str] = docshed
     elif fname.endswith(".pyi"):
         writer = functools.partial(shed, is_pyi=True)
     else:
         writer = shed
```

### Comparing `shed-2023.5.2/src/shed/_codemods.py` & `shed-2023.6.1/src/shed/_codemods.py`

 * *Files identical despite different names*

### Comparing `shed-2023.5.2/src/shed.egg-info/PKG-INFO` & `shed-2023.6.1/src/shed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.5.2
+Version: 2023.6.1
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,18 +77,18 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.5.2
+  rev: 2023.6.1
   hooks:
     - id: shed
-      # args: [--refactor, --py39-plus]
+      # args: [--refactor, --py311-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `shed` on unchanged files.
 
 ## See also
```

### Comparing `shed-2023.5.2/tests/test_expected_output.py` & `shed-2023.6.1/tests/test_expected_output.py`

 * *Files identical despite different names*

### Comparing `shed-2023.5.2/tests/test_shed.py` & `shed-2023.6.1/tests/test_shed.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 )
 @example(source_code=TEYIT_TWO_PASS, **example_kwargs)
 @example(source_code="class A:\n\x0c pass\n", **example_kwargs)
 @example(
     source_code="from.import(A)#",
     refactor=False,
     provides=frozenset(),
-    min_version=(3, 7),
+    min_version=_default_min_version,
 )
 # Minimum-version examples via https://github.com/jwilk/python-syntax-errors/
 @example(source_code="lambda: (x := 0)\n", **example_kwargs)
 @example(source_code="@0\ndef f(): pass\n", **example_kwargs)
 @example(source_code="match 0:\n  case 0: ...\n", **example_kwargs)
 @example(source_code="try: pass\nexcept* 0: pass\n", **example_kwargs)
 @example(
@@ -162,20 +162,27 @@
         f.write_text(contents)
         ret = _rewrite_on_disk(str(f), **kwargs)
         result = f.read_text()
     assert ret == changed, repr(result)
     assert changed == (contents != result)
 
 
-def test_rewrite_returns_error_message_for_nonexistent_file():
+@pytest.mark.parametrize(
+    "fname, err_msg",
+    [
+        ("nonexistent", "No such file or directory"),
+        ("*.nonexistent", "maybe due to unexpanded glob pattern?"),
+    ],
+)
+def test_rewrite_returns_error_message_for_nonexistent_file(fname, err_msg):
     kwargs = {"refactor": True, "first_party_imports": frozenset()}
     with tempfile.TemporaryDirectory() as dirname:
-        f = Path(dirname) / "nonexistent"
+        f = Path(dirname) / fname
         result = _rewrite_on_disk(str(f), **kwargs)
-        assert isinstance(result, str)
+        assert err_msg in result
         f.write_text("# comment\n")
         assert _rewrite_on_disk(str(f), **kwargs) is False
 
 
 @pytest.mark.parametrize("refactor", [True, False])
 def test_empty_stays_empty(refactor):
     assert shed(source_code="", refactor=refactor) == ""
```

### Comparing `shed-2023.5.2/tests/test_suggest_different_block.py` & `shed-2023.6.1/tests/test_suggest_different_block.py`

 * *Files identical despite different names*

### Comparing `shed-2023.5.2/tests/test_version.py` & `shed-2023.6.1/tests/test_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def from_string(cls, string):
         return cls(*map(int, string.split(".")))
 
     def __str__(self):
         return ".".join(map(str, self))
 
 
-@lru_cache()
+@lru_cache
 def get_releases():
     pattern = re.compile(r"^#### (\d+\.\d+\.\d+) - (\d\d\d\d-\d\d-\d\d)$")
     return tuple(
         (Version.from_string(match.group(1)), match.group(2))
         for match in map(pattern.match, CHANGELOG.read_text().splitlines())
         if match is not None
     )
```

